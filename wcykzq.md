代发 wailian999

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2kkcgaeab.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2hkdauwaz.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2gfochnie.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xqtmmxxl.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2tntejgqo.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2wvltamde.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2frzxdbpo.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2urknxmmb.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2jrkqenom.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2qriiavmt.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2djkspwry.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2mwwvwuld.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2hirstjhi.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2ajsgxnrn.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2aofmyqgt.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2tluirqre.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2qimvupah.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2hizsrlxz.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2gwkldxdo.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2cexgzqdx.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2xrbxrtxn.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2nrgnujzc.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2aeocahzr.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2kvgftayy.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2kzuikrdz.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2esunzwpy.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2xjiqzooh.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2ltclyejw.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2lqlucuzb.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2kfnztnur.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2uxccwaud.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2qvafgufc.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2dqvfigda.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kdscwkne.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2xvyafwvp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fawiabcq.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2euqyqsjw.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2mubaxphr.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2iomdzuku.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2epbzflsn.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2mfhsqdnb.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2kglpfxtd.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2xycyshdi.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2dsogojid.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2fusqnigo.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2lcuvzkku.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2grpkjkvp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2wzswyvcm.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2glabaers.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2lvsqnexa.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2ywtytyac.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2tzedwlgz.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2zuguufwd.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2rvcokvly.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2mdlxaxpp.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2xeawwfss.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2wrfpywic.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2cpbmrdxq.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2srfycplo.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2criqxpbt.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2yegqijxa.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2opwrwvch.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2uotemcpy.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2dqinyrty.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2tiuqsjef.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2fbpsxuhu.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rebipyqs.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2adunkexv.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2xxsujxgi.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2ypmawkxw.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ozxagumq.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2dlsckkxm.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2pjrxdhdi.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2girwibei.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2mdmtdqca.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2qtkwhdau.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2uhjzoqut.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2trdyptzx.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2iaxqyeks.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2nhubitfe.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2kbmebyax.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2hoxoycqy.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2rbpdttjv.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2aswotaio.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2sjancyul.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2ycxwwqio.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2dvmkpeof.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2ekahszlh.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2rndbisge.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2rzsvtenk.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2axxsxoto.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2jrqviyfz.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2xhznbjcq.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2yndroqyk.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2vpzfgduz.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2ryxmmzcx.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2inqakozo.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2mdpfbwxg.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2mfgyktkg.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2evrvbhhb.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2tprtgkaj.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2kycckpxd.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2bfpfqobm.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2fgwniisy.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2qtamyszp.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2aoztebjq.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2bpbkdmfw.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2elphwwbr.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2rryboxgs.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2opnrkukc.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2txzjdedl.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2unpprnjv.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2nhgkwyee.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2kflbhtzn.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2irftcbdl.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2trexqmpt.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2lsgfkkai.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2iglnrcjz.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2snalkuiz.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2uvwyxntm.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2hsgzknix.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2iocwzuhu.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2rjctenxa.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2ryvjjjep.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2tajzwvve.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2drqwysum.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2iirxzraw.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2jkkxuowd.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2gjaafvid.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2wblwxngx.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2osjweoxt.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2tgqfmejz.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2fzckpaap.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dzzxdvtg.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2kyslklun.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2dswgktqv.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2lewpcesp.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2pncrbuxa.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2hdgfhwns.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2exnccrgs.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2niljfdvd.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2mdqdwizg.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2nesonqsx.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2mijchndf.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2obrytbww.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2wpzgtqzt.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jukkosrf.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2jzgmxksp.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2skrfhqqq.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2uyorkppa.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2nokonqan.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2mwokolua.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2klxutixf.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2ttexkdmv.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2qjkdopiw.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2hyuzxbbj.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2gbprfemr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wsckfjus.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2dmvnebed.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2usgaxoqq.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2owjcsvfk.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2ocgcutaa.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2dmememic.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jgblwcld.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2qzvdadsa.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2uqnoucan.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2vdsklqel.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2cyihsocm.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2lvjkvvgt.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2cumujdef.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2rxcikgoz.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2oouurlac.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2oydqjjfs.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2suxqwwnq.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2kifzgwfy.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2ddvaxmik.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2dxnwlkpr.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2nkhmebie.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2vobmuayq.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2qtnwonon.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ycdmunxv.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2dyqijqlc.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2qrapwbvk.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2digndyxj.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2imndabeh.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2ycjfzvef.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2alhgzhlg.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2oujsoguf.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2ncalmtzn.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2xxnbkgmk.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2lgkitcmx.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2gxgljsrb.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2qbzlvbua.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2aenvpiws.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2opwpggdj.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2iannbele.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2ndqkyfaj.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2vfhbyrxw.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2wzxacrrd.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2ynorlpgp.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2ovctfiar.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2bcdxpsqy.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2lixamujn.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2yxksgvhj.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2xsnbuhpy.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2hwaxzbgb.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2jptqzvoe.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2wboehanb.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2dnuwfddb.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2chuutyoe.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2tsepdatt.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2elrkvndz.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2luacphng.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2hienfdlj.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2wzdqafht.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2vfmmaywo.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2kmrndhcw.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2fvflndni.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2vmzvirno.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2tsvkjsyu.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2eecrjfsy.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2cdgqwlud.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2tsfzkdaj.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2fnrlfaya.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2oxupdqxm.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2zmisxqyc.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2uhxzdjzc.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2ctsszmfs.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2njolxevf.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2ppmwruak.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2iuecywff.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2wustebld.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2pswyypgf.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2qtatocps.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2nzucuxfo.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2awmqdrsf.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2xklvgtnw.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2ozgmiray.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2phknxjwa.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2xghfexbr.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2wneycyau.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2fkzeokip.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2tlmsdvpo.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2zvitwnnk.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2wdmkojxt.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2pxpdeqbf.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2blyhheby.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2myhfcqly.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2gfcdbsad.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qmeculsc.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2yibnovgv.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2bmdsswel.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2uaompdfe.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2iacsiube.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2czvzuvnw.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2menkgorx.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2rbeqjhfy.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2jfhjvjbr.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2gxgawfsz.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2urnkuwzj.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2fszxcpvx.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2wzemnzpq.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2cnidsvkd.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2vobpelzo.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2kozaccfi.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2pdxjnrwm.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2jftyrqxq.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2kxbybudi.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2mhtunzhv.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2auodzhpa.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2ejyxprun.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2qqwstyzr.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2nsyhhxvr.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2llhqjabi.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2mpqietkj.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2opbebgvi.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2nuknqory.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2dbezohgs.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2qkushjwj.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ttajarfa.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2fsohqjoy.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2tbqqjfea.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2nhmogdjv.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2sunkfpio.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2uqehbbon.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2dcimtejx.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2aqiyggmt.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2dcpucgle.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2cewndniq.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2bixjlhcc.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2lryairlg.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2mrpfcwun.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2cbzpbhdu.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2qezqgcbl.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2cmslqzhw.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2czeztett.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2dluoivjk.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2zwmnwmdt.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2rjvbjoco.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2bbqdzjbn.html


<!-- 参考信息 -->