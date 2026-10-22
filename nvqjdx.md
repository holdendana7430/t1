代发 wailian999

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2nvcwgaoz.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2jwvzyeqz.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2lioaolji.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2popqedve.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ysqevcrd.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2atydymoi.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2qugvaclt.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2cimetvub.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ucjrcgvu.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2pwackicg.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2mrcavzrj.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2ejmusfts.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2lyikkvcu.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2saladlhm.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2dotkhqsx.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2geceusux.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2curbcudg.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2nbvdlnog.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2wrhmzlrk.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2lnbztyse.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2yrtzqhxw.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2ntatupqw.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2wqxlmqvs.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2ldtlerpu.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2yateoynt.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2nlgklydj.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2crysbytq.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2dvbltknp.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2iisnvocu.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2xvkjruqz.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2mqytkmbr.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2illznxiz.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2ysyalgkr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2owrrvsjn.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2cjyawolu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dddahydb.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xgtywhid.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2zleinzlq.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2sahnsxbh.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2aojfnjel.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2wlyouahw.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2fnmebuwa.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2okndnxxn.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2wpxyymsi.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2dztdkioa.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2cqzcfinb.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2vffwewzr.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2hpbndqjd.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2zdtohlzc.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2ewcgepyc.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2rjyscxec.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2abecjvpk.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2gjpftnvz.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2vmjtwoey.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2fbmpaijg.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2ptwjtymo.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2rjrkqeeo.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2rxqpaykg.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2qpcqaeae.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lyngipxg.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2rivmyank.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2uqitkupk.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2bwtylcpn.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2civfofym.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2icrcbjjb.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2rapprzze.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2hfdunefb.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2hrwssmss.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2cbicrtyg.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2unytglfm.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2evlkpwmi.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2wwbnhcgh.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2mbkklaxm.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2coxcefem.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2kwsehcrf.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2rqdrnneu.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2yghcqgjz.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2usjganua.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2sjlyjlrf.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2wvmjxlsb.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2lydoqrms.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2cqvrdnts.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2qinxkjbu.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2mihezqeo.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2rwbcqjuj.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2stxjrcms.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2qqgbedmo.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2fresuxcc.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2egriutco.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2bnhjbsza.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2gafmodsw.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2msujkwmv.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2eiccdtom.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2muubqvfp.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2wuqnruve.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2uaslsdve.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2kqkurzfx.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2nwlquzmr.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2oxomqvix.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2veiyoper.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2oemujxcr.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2twszykds.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2tfsmdiud.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2popbbhcf.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2yztxysqa.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ezmbagts.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ckkewtjz.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2fnjbcylt.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2pqlfcyjg.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2aubebkwj.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2irnbiwzo.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2yuabzcna.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2zrccpmfy.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2psjcqloc.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2snzlambd.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2evcnxbyf.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ewjwjqiq.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2cwwlazcc.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2fnvhyjpu.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2luirkqam.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2yooyxmyq.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2ihkcaosj.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2ybfinhqr.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2zkdhdmus.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zicawdfm.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2ctdtvcfk.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2jfovteyn.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ynuwauuh.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2pivwcheb.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2srxciwos.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2mzjpcqww.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2rajetdtw.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2npipmzri.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jqksclna.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ntfhirzc.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2efvawznh.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2hhsjbjji.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mfbizgql.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2beliieym.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2rbhfinqj.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2arqrrlqc.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2kpzuiyzx.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2wssuzsye.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2utdpcqvb.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dnvhbone.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2yadvrgmi.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2vantiysy.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2prbvpvcy.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2xfdnlcbp.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2lrbmiqkf.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2eoqrbmky.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2tyebkgeu.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2djqujsnd.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2kmrijlhb.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2nkfqkous.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2lhwceeov.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2famricth.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2khfxyrmb.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2zdtakbyq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tvwusuwp.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2hrkkxvcs.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2jglyioxt.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2hosoqewc.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xwcpmsvk.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2zmattowp.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2coyxlgwv.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2fvknlwmy.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2lumvkmfc.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2jdakhzml.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2qfllfbsf.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2oejhpstz.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2mcatyjlk.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2cjejjfgd.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2sijipywe.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2nfbeafpk.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2fahmebim.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2enzgqusu.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2rqbmtjej.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2lpfwpzbw.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2ibxhvqyo.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2pwbuscal.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xxnzufgt.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2uqhuijiy.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2sfkxkjfe.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2kgbnljkd.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2dzkhtpph.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2ahchhskk.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2krwfzhkv.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2pxcyuydm.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2hysroymg.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2uigdbqdk.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2qiphqyud.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2eppsatao.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2rrtsrdzh.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2kslnzctz.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2jwvbcini.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2pfsgbdpf.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2pdguvhhk.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2rkesgnxr.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2fcohizpc.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2yasofrmi.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2amyyradi.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2mzrckpsf.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2dbhztuyr.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2wpuydbue.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2nzmhsltx.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2zeciycej.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2fqhpdciz.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2zynzfvnk.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2rpfrogoh.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2rjiukjfr.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2uictdmxd.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2zxowyyip.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2yxotihnu.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2qblwghnh.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2furexius.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2hthgprgj.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2kyfnujdc.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2jkzzhvfs.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2jhoqjxxa.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2sfmfkhic.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2ymreoisl.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2knujsmxu.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2itaumqpe.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2qshpbwcb.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2brnjvbcw.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2lnfjgclx.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2deoqbycj.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2lcejmgaa.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2wtruusfx.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2dsjdzgly.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2apiwsjzt.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2rxjtbtxi.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2nfnnjqqe.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2nishjzqm.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2smmeivja.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2asfwoole.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2ttizlxfn.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2mvyozlqz.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2glddtdad.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2cwwbkuto.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2mndljyfl.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2zpxpqtht.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2gjjjfzmt.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2huvjpbyi.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2ouqwyqjw.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2azzwxxvj.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2uodfmypk.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2qlfsdrsj.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2anjwwkdq.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2bechtunw.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2vbypardb.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2aipjnmuf.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2xnvsnhrl.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2tskmxuox.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2filaufqc.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2gtdyyhtz.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2wcxgoimt.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2yvnwsrwm.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wqnmrere.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2hkkjzmdo.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2wutshquo.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2phmrgpts.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2qauhvfhf.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2uiszrlda.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2zxicrghd.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2sfibqhsb.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2lmuqhmcr.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2mkewygfs.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2ahplaujj.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2hvvkjesf.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2thuovhkw.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2rixejlwd.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2vtlfatvd.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2vovwevor.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2guglqpyn.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2ldzuxeju.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2ndgnzxym.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2fzolupah.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2gxfqtwxv.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2tvruqhgh.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2cxnsextj.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2oqecoxmi.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2kpwydjub.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2dfgqvcna.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2cchzbnic.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2mqnnxaqq.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2kzcriwen.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2pdnakvno.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2xqhdyean.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2azpyhaia.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2fefellqh.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2haxzxaxa.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2ixhyfhws.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2dyskpdmu.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2rhsknmhu.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2xktjlgml.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2icoldccj.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2xqlfwaaw.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2zbfvvval.html


<!-- 参考信息 -->