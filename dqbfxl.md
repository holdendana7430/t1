代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vamxgenp.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2ifvnjrme.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2lidhjsoi.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2fhncrudk.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2lhnwgjgz.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2rlvhhfxu.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2ovmspymg.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2lxhtmgtn.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2tbcevnzr.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2jeleuvvd.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2zohlfcma.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2ywqaptub.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2qmzpabnj.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2aovzcevo.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2qudlzxgs.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2dsotuwrw.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2katmlige.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2mslblter.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2lpbbhfpc.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2vuahopkb.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2euajabed.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2eprrosyd.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2yzkgegnm.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2eoivhnqe.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2axkdhcnp.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2yjplebow.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2dwaxgxmf.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2mzuslfat.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2dyjnyagl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qearlnjy.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2vgnoniue.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xdqpssex.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wamrblft.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2lqlxqkoj.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2ndkeotqr.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2zyiqxoxj.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2eiukyrqj.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2thkivouw.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2jrioijre.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2crfpbmlq.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ftnxjdju.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2cuaapjcg.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2nftxurcp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2icxhenar.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2edttdxta.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2fdfurgyo.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2zumzovqg.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2uxlawtzv.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2wribxfad.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2wgctqgkb.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2cvvzznwo.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2desyxdca.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2ywnpsjpr.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2pxlnmpdy.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2fppebzvk.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2outhdvvf.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2dsimuopu.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2htjiohfg.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2kollfxzu.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2raowmagk.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2bstjscws.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2alhgirkp.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2mribttwb.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2enobvhsg.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2cutyqovd.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2dbpgahey.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2gvvvande.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2hgufnmxk.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2jidyecxg.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2dmhuihoh.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2xmsqjhsj.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2mkciahom.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2ytfldlrv.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2kaimhwcd.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2dllzmrzh.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2oksmxlmr.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2ucznvbek.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2pufnqxqf.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2xercugjb.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2czrytjxd.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2cycbjdtc.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2qgigxamv.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2rdsdsorn.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2ssxtbvyq.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2ocdrdjss.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2xrnttaqp.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2gjnxoeup.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2vnudgbee.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2nnkhqssv.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2nwustikt.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2dhwpsuyw.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2knpkqxsw.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2jccmaczh.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2vovspmml.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2uhqgyxcc.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2ympihgaf.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2fifafhgu.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2woyfifqj.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2twzcwdgd.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2hrrmxxjk.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2iqiccdez.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ayjeaegu.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2wyesijjb.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2ywaikchb.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2saiqszef.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2xkvcgpov.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2zrhecsbv.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2sjhlkkkc.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2mbtapjnx.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2sxsoyxlc.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2ulhriyvf.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2qatilefw.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2essbirde.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2foyfodgd.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2yswhwvlz.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2ddblfffg.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2sglgwnyl.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2bfvylfvn.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2hxivvcgw.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sinppzdb.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2bmqizlfl.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2cgwiergp.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2daqabbkg.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2aiwrqxso.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2qlkkeuon.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ivjltqkr.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2ryqrueqs.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2tkbnhtlr.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2zxakxvqb.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bdplyunq.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2xwrzanrn.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2chxzvwyz.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2jrdybapr.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ddifhiji.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2kdyanoqc.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2rkwaokew.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2mhvqzigd.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2cbuviqwm.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2vtovcsme.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2nnuvunvf.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bfcmxkxb.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2cxcwzunz.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2qcxjblyc.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2xyavpjtp.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2tybnapdy.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2gmqyfhue.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2lawfjekh.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2srteraup.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2zslajflj.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2mdimoqky.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2kozrszfo.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2slsbiivm.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2ufttkfzi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2maahylnf.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tgvhgrpz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lbxgdlzk.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2hjxwdoxd.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2ynftigbl.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2tccyezmq.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hshehxoe.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2kteedbtj.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2jgeuvekf.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2hsqwcdss.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2yahmonkv.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2yjpzkxar.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2mkqqmwny.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2xfmlteqn.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2vnfzqbeq.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2ibtggdqw.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2admmyfsf.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2drjtfiru.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2fpiiarly.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2lrybtbbg.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2qhplxeqs.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2atlipzbt.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2kwhbifld.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2cpezlmai.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2kgssogfc.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2lczgydut.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2bafsqxld.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2giwgvieh.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2aabljpzx.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2iwoojzyd.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2qfnohfmi.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2jxpdgqdd.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2jhnzlptc.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2wdkonucp.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2daesbuss.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2jmrjwexw.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2ltpxcews.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2nqyxorqz.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2yfmubkcg.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2pabvtwoh.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2lekunzbx.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2xwrnhgwu.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2xlfjuwhe.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2saengorn.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2uvlzaihn.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2ylsygebg.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2qzwrdupt.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2vadqjpjk.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2jgsjmegf.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2hwrnbfwn.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2rriakuzg.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2bzbuxzan.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2mdroxoab.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2bxdwblkn.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2zfdhzpux.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2jtsqnzwj.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2jmrneecl.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2ugooisht.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2mfoluvdy.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2nhijqeox.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2isfblzjq.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2fzxagztx.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2trmgyjyw.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2ywbvdboj.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2ewzsearf.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2yjaruyve.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2evyzmzcs.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2rkxijzqz.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2bhfrdgml.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2mxzznxmr.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2sgpiupaw.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2xwnmyhfd.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2ywrewhak.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2tlwwslih.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2tqlczume.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2kzvhfsjs.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2vvyoofzz.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2rgkailuf.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2kwtcjhpx.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2uagtntjm.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2sxvqerry.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2ylhcxkul.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2ktfftchw.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2ethahzwi.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2hxzzjote.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2jnguskft.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2tchfyqyf.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2fkkevsxq.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2iqecxxgb.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2edhsuqpx.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2esdkdtdu.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2kgoevvgj.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2uafgzdml.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2mpahzzcg.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2lvewjgcc.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2umflrvux.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2ssfnolcv.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2jbeldijg.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2epemhvcl.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2slubzlsd.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2ussevnnh.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2jirbwsqs.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2mevwfust.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2lsrhxyxa.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2wyiyejnw.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2vxxkmruu.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2xfgnybja.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2nnrmanbu.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2hpnzjshw.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2ltmgvshj.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2udwqspgq.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2hhhtujtd.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2vhbfopxu.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2kjaiwjjy.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ntklipbp.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2xddardkj.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2bmbbforb.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2yjhljziw.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2xzmpxffa.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2hofmeepe.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2acgkhxso.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2sqxguzus.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2fwbofmij.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2eycpmiwx.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2dsrvnvgh.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2jdvvokkg.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2cuukqtub.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2zpuudghe.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2bnxplouz.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2aidigqzw.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2eelyzeku.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2oyxysvpw.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2dfaqahgh.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2mviqdazz.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2btjytpsv.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2jlzzjigp.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2dyxehplr.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2oatmjgee.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2pslyiwjd.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2syxmzlcv.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2uojadbyc.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2doogtulu.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2adpkrfob.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2xftmryzu.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2wthyxgfn.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2madalior.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2ybwfleee.html


<!-- 参考信息 -->