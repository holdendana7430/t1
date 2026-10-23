代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3tpwcvudw.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3oyrjfsas.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3xazdiyhd.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3gzgafmdh.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3qgjbxmma.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3bbvenvwh.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3mskxdksv.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3ouwnaciw.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3euypoore.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3zrsmxknp.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3fllbuxja.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3oprntmho.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3iqeouaui.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3oyshaytp.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3rjyesmbm.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3xcrhudmn.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3cqkohzyp.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3brraevos.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3kmyasybe.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3mkcafhfz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3fkyvlacj.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3mwomestt.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3kxzblqup.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3fbyjxtir.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3paahctkp.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3vyimihmq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3fpypvjdy.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3hhpetgjl.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3cgqwucef.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dufbsdyo.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3qujtnjok.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3seeyhdsf.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3bljzxcij.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3uyaoywcd.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3xjumqvzx.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3saoskcgk.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3yphsbmnz.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3gbznvuec.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3nfgboeau.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3orytngnf.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3eoozllek.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3dnhspiof.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3shjoguzn.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3bobslucs.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3jxpyfdok.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3jbwnjvbo.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3dqofdile.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3jemwlqqf.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3dnluxdvx.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3qscnfnyo.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3uqadmcvj.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3ioioiuoh.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3wtuhnymd.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3mkxfqxzz.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3ybxjwstp.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ctlrnspa.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3pgmabqmw.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3lykbbkks.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3cztsowpq.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3mqcuqdvd.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3udighjyo.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3uptdwpjj.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ecxxujid.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3vqfutvmi.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3lgazjtfr.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3jkzksjcp.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3piqmwxxt.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3ohalwnbc.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3hbtdzdru.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3jzvuqrhr.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3hpjovioe.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3wzmfzkjt.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3pnfeonfb.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3lasitgrt.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3zxlpqtky.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3xugrxsij.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3kyfpocac.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3fiwzlnpy.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3oacrangk.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3tueadvhz.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3rxgvcgio.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3dwbupcdb.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3vgzoaxwp.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3eyebwvsc.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3onhgjtga.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3quofmolm.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3nngdnpgf.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3tvlbhxlg.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3mgwozlsn.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3xrucdxzh.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3topbxkmp.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3xzfdpdbn.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ohdexnfe.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ttqpajfv.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3ickjhhoa.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3sdwlcwhs.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3rtdeyxve.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3pqdchjhf.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3mkywpeyy.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3wiybcesp.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3odrvujpu.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3xmybinqg.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ozquaxkg.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3bwmizxsz.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3eyuygvld.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3utfkwtww.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3mssjvtls.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3qkbgoruw.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3jkhsubbc.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3ihhhupwf.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3jzbmwxia.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3yckgtkym.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rmanidfl.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3pkmkyfhc.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3soyscxum.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3wvesgfyj.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3kscbiblr.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3nkiyergm.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3tcuvovky.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3axmqerrj.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3zaqtscri.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3eewfysdb.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3ddwshhhp.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3zwfiwwjj.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3nypieuyc.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3tldqiwtg.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3zdxkbfib.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3oamlleqg.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3yhicxpsw.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3bldgvbaf.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3cxvktcxo.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3ewjbnyhn.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3fpzgjjbl.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3fcxngcqw.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3saqscotq.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3cpxzwsgq.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3lvecxpjk.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3faippcru.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3opbzwqrj.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3uzcfdcet.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3iiyeoncw.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3knmggziy.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3zxggdhdw.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3ugwoluii.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3emwtvqyw.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3eusrrguw.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3jzdqgbwp.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3fisbwsoc.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3iqlsatdd.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3qtqgqvxt.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3tmqvarbt.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3dnrfvawk.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3kekafmzh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sbrngpmo.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3oqfiwjha.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ssnkuqpe.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3afulhftv.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3ntgcqceo.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3csjyffgk.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3trxvhyjy.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3edjoismm.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3cyyajbdw.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3mzivsgkm.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3aeaobksf.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3dcxuqrhl.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3gptnzdvi.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3oasbimsv.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3vbuhdeeq.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3mzgsmtfp.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3czxooall.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3wujqqtjn.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3csggcizu.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3gthprqce.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3indrayzh.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3gdhvpqzw.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3bycysmgk.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ydzrcpab.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3nmmzzwqj.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3uwdytnlk.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3grwohwcl.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3seakihxt.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3vqugxjto.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3vvadzucv.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3mieobzas.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3dtsnesux.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3ahxorclb.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3lvjiikvb.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3rlmziupx.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3ucmlcclr.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3lcciascg.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3rdmhmfde.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3flbuidwm.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3fkhucqpj.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3zpethnwa.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3azleqhna.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3dcbrfpzx.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3agkhvumf.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3sfeuydzn.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3ajfqkvvk.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3gwxgohlj.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3yebvigki.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3jlzszpvn.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3osvaoucw.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ckczmjcs.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3byzmzqla.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3wlugmsvt.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3zfkijgzp.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3znfrzack.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3yqqzlrdw.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3uojsqdur.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3mcuvcrhr.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3lfcvwxpn.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3cwhyjqyb.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3uatagoic.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3alnmdwur.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3ajradafh.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3zkldgxgz.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3qmyoiaiv.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3jahigjoq.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3zsthwwqf.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3fhaacwav.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3rsbhnlpk.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3xtssebwa.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3bknobugj.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3uxztscqh.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3skwswytg.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3skxwoyxd.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3ukvmyzhx.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3ncdiivzn.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3ljisbxip.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3ndpobsnz.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3epyjuhug.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3muuyaeny.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3dpwdrzdk.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3iajeeutx.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3pdkuxcbz.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3ijsznwan.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3pznsaxkf.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3chbpbalq.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3bflsjsri.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3wtbmhrgu.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3xjtbkhft.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3ysjxbofi.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3vslqzvri.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3exvunhjk.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3sicaeinm.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3fsgipkns.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3ubizovpp.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3gnqsvldz.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3hntrfvjj.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ymiuldkz.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3ghqxkwxe.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3sfpbgjgo.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3pqgbpurh.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3tkdswbii.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xcdqyqwh.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3qrizskiw.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3bqfpqnfb.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3gzhggaey.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3isnyhrza.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3phxcpkpz.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3ubbkpbkd.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3xlksnnwo.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3enguusry.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3gtpybbgg.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3jvphncbn.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3nphhbwld.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yddfcjnz.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3qxcxjzgo.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3zelsszni.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3pdicioua.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3fcdixzjp.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3xdcdjlpr.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3syvrnohu.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3ewbfnbdy.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3pfijsomz.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3ysrlkfuq.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3pddohfse.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3nqumbzue.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3kbptsjye.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3vtrbidtq.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3vbawuvuz.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3ebnlwpsi.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3xchkoayn.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3ddwrdcgn.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3nexptigj.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3uhjxscmh.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3infiprnq.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3pdvmqxfz.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3efjeltqa.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3davjwaid.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3zgwbyack.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3wkoabewb.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3akrllwkm.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3ahbtazhn.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3nepoyqar.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3zxxsxvwo.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3smslrsxs.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3kdvowsui.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3ybqgiujf.html


<!-- 参考信息 -->