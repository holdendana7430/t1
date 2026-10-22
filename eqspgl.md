代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2agvclmuf.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2tapwwlkq.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2zhrtfajb.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2deylujks.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2mrdevktb.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2hujwjqwh.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2fxwhrcfm.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2mrxhfqky.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2wdtdgkig.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2yhmhnrgr.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2nsolplkl.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2oydnxucn.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2mwhkmtcw.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2xkxkxxye.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2hrjzenff.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2phabscxo.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2gwdwbwrg.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2dflygpev.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2vfiulkrd.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2dixvvhvr.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2rujyywah.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2tivjrdug.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2oowsqcne.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2gikbknyg.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2eulqgstx.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2wumzlnqn.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2cclhwglt.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2tuzmltwd.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2fkaztaoa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yxowpvjx.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2rmphzllp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jsezpduo.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vsjxlwks.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2xzfsovko.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2kqdcuhql.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2gnxhqtrv.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2iqmfomdp.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2pojgklek.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2qpjvsmmk.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2zqcfgeky.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2vgsfgxrs.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2uujeejpy.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2daqnhyqn.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ddkqzker.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2mjhfflqb.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2dolgancz.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2orckcbhw.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2opiubatt.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2tljybdzh.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2xvsqzvvy.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2iuqgouuy.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2bwzhrorj.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2wspjetpv.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2iodxyatm.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2ryrpfdon.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2adrrzsvw.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2nuvsfymq.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2daddshfd.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2olnnwftq.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2cozjccms.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2zzzbzpvw.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2hvndeppi.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2tkugcxap.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2btvayhvo.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2xezaegxb.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2poriogof.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2meqppedi.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2ltrybulm.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2vyjmgcab.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2gpqekyhv.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2reshyqcq.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2nbsjfkes.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2dkzzzmef.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2ktcpamcp.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2ylcdciie.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ihokbsfj.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2agkygwqt.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2ngzczhnc.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2tetwjdvd.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2hmqswcym.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2lfxvixgw.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2odldiuwj.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2gtypkugh.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2rgqsgdko.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2ckezpazu.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2zhaqatzn.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2kjmvoxsh.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2zhhxmmxu.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2gcvclcnk.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2nnlctrti.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2rcaukexz.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2ttypzdmo.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2arqnepsd.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2buyueguy.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2ozlohbfw.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2vvtdzmxh.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2jxxvloca.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2ouyyxbyo.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2upjhurcp.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2fagtivcr.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2malrcfcg.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2naepdhdr.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2mdbkfelo.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2rsjyehym.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2hcdrfvtn.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2fwrnaixp.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2tjgqysxy.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2fuhotxpc.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2keqjlccg.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2bnfmcndt.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2wxgqlfxd.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2iavdvpdw.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2tafucchl.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2fqatrqxy.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2bfywrair.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2kfldwtlv.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2pinbgxsc.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2ckazivrg.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2jsimoutv.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2pcwfriuq.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2norlihgw.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2rjxfwvrp.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2adqppvjk.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2zbzybltc.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2anagehah.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2mhbwixmg.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2tisarezv.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2xizilqbz.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2wiqxzwoq.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2whzydkfh.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2xxvbhjjt.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2gdmefbcv.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2kzlhiqnt.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2smmqtvuf.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2nfzibmin.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2qpvfvkry.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2ylykhiqb.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2kugohjbr.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2ddshlswg.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2lpyartjt.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tzaavtjx.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2flzmlvxt.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qthxnpqv.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2vakefzhp.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2etaxnwlr.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2dgswiiaq.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2vmwyayyf.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2jsijfuyv.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2ciibyueh.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2mbhajngi.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2jyysmtmy.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2hofxcvhi.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2nryyisfr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2luwwdkzo.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kzmqebrl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wfqdcfax.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2zeefevbv.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2gamghllr.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2qtzzgtqm.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2rzisuufy.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2espsoggg.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2eltbcmva.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2cgxvutkf.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2gvdgeftw.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2teiejosf.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2idxtwscn.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2hrqoqebq.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2tkrqrvsk.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2grufamqt.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2rnnavycn.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2hmpamoqj.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2mrfaygtj.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2xfbrpolq.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2elanoffu.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2ndnefroh.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2iqnzjxkm.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2hpsayock.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mweiedkh.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2osyyljwu.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2lhpzjzbv.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2tjnyheom.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2auonahbm.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2ouohwnud.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2eckibqnb.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2nhynhnhw.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2mgzknfze.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2ujacwzxt.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2hkwvqqxb.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2jddcsbsl.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2kwhdefap.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2ywugyfxz.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2kqyblgca.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2xpbpnsqf.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2oebcsene.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2jmuqeufa.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2fywgftyx.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2nzaalxax.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2rzczuirc.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2owdlbigs.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2ytnpvtla.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2tuqruqzk.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2pqjtbxld.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2pehmfnir.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2embjgyke.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2yskkrlgc.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2psfyetvr.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2htdybvrz.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2lnsrlgwu.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2pvvbplpr.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2hustppjh.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2lnabnutu.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2imqbgunc.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2xxidbzqu.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2bytzmeuw.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2uskhftna.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2iizxbdcm.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2kgirykha.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2dlfzvqxx.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2onisqvdn.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2pptvwdtq.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2iwgonmpv.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2fzubmvqx.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2mmaoxeel.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2kyayfiog.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2btdedfko.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2ywihxbbu.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2lhfnnemd.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2rjhslkal.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2pjkfxgzo.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2pdzamrbk.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2mrxhkhew.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2kkrsltoo.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2gbduzutt.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2lddsmcmt.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2tqjhrlrb.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2ogcqosgo.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2ulisdyxk.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2evaglhfj.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2ystreldn.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2gjbyoead.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2yvfzegym.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2sxzyukxl.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2xccqgdhw.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2tcwgxfro.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2nwahvehe.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2hngcxyia.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2jikruntw.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2zjppirtk.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2aukmpzzy.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2bptouioy.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2equzrsqp.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2pjjgfhjs.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2wzdhdstw.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2pecfsalp.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2dodaypwh.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cmirbyom.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2pwcjbjxk.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2kibkczyn.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2kaetlhyy.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2agejhlzv.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2wisgopnq.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2gtotyonv.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2gsztafbb.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2fquothks.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2xrsvfnbj.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2kbeukjuo.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2aauyptjz.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zfqqckhp.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ringtdxc.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2xjhnlihi.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2qlaucukz.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2sfvdnmja.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2bmdtktwr.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2pgxxxjqz.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2izjcmohc.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2hnsvkcgu.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2fzwblwxw.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2ciwbdetx.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2ndjjrsyu.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2zuhgentq.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2vgxrykwz.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2urdfywsh.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2utqctfdx.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2ugyzjwvw.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2fikwniar.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ayaetuyk.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2zpmmmije.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2kbojgeuh.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2pjjhgayd.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2fvfadssf.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2mbwyhtps.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2fnkmayib.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2zrcmqokq.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2cdmawhow.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2numsvonf.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2smywfzeb.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2uetegkrv.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2thwhkgcw.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2kcnimkcf.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2lpdfojwc.html


<!-- 参考信息 -->