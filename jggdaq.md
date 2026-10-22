代发 wailian999

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2quhsplaq.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2efidhttu.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2fuotxftx.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2xeadukwk.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2dcegwnla.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2wrzuraxu.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2qjwznfgd.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2jtoiodlp.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2rctvgzqx.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2nlhzekls.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2yzsazkiu.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2rcblccvn.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2behprhig.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2lmbvtsci.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2yxqnpeii.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2yetwqzne.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2wdburywa.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2pouoxivj.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2ckwsskjh.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2psaiexum.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2aroqlnpp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uqkvruyy.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2padxyssv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vaxskfrg.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2pskxiqie.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2iguuybul.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2juwngcma.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2uiyojsps.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2fijpcayt.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2tycuiczl.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2tnjrjsgm.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2xqndtbrx.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2ysexuexn.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2mxiglaux.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2chltvtcb.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2kdeuuktk.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2veijpqsm.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2duonloel.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2alwyhqzn.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2jqdzrqsq.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2vcixnwri.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2wjyuitax.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2psugvliz.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2asfckcch.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2gjayorlp.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2javkrcku.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2hnnosjed.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hegbiewn.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2hbcexouo.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2yxjlufhn.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2uvasgojz.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2mxroulzc.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2prclbwvw.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2kgdtydga.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wjxvqvsu.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2jcoziujx.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2ptfuyutq.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2mdwssems.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2cgnubjgj.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2ekflnkdp.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2fwocxenz.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2inwamzpf.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2mrkrvtcf.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2eqjkqkyj.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2mknapnwz.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2eonvjiii.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2ljcllwda.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2oqaefrfk.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2bqqisnto.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2vuyxstxu.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2ljcbbzmh.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2hlzufvts.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2gzdvinll.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2wtibekfo.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2tiozqufw.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2tffwqjgs.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2qloonmdb.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2mdemhczi.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2brftgnxo.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2iwenvdkh.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2pfoskvht.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2gyxtpbbn.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2vqguhpkb.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2rzkmqlxp.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2eujmfcnw.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2vifmeacj.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2rumpgbvd.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2aygvzick.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2eqvhsvwi.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2prnlgmac.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2oyebabqg.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2nyotyykm.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2evezqnbg.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2fzneawsq.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2wilcgdnh.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2bdqkblnb.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2jvoskoxr.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2uzdbphvh.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2ulfwmhwo.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2uajbsewa.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2zdetlbnk.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2kutbiajq.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2jdsfgbsc.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2yijlitqv.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ubihxbrj.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2ybmaefmw.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2ylxeburf.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2xuuncvfa.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2rkcskxfw.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2ykhgmhgg.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2anosyspp.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lqjhtuym.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xubvshnn.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2eyhvtlub.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2pnvucsbl.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2seieukmv.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2mqnbpoig.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2gporchhc.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2resajgky.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2bnduhyyp.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2iifcxkto.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2tkjwoarm.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2rshlabod.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2wochrmfk.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2fezkzdgw.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vepvwkdo.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2sbkubuei.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2hpvwdamp.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2komtldqa.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2tmjdilus.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2mlnqruqv.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2bzebajqh.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kkyneyyy.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2zksanvsp.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2fdtgdhgi.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2rlsakpge.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2bosrbfdq.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2htsbfeee.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2nclfoobx.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2kucihcns.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2qbgpxrvl.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2dyltizae.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2sbhwbwfx.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2znfnnqkk.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2tsuplbna.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fqyyjhsu.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pewyowrw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tbaswudn.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2anqjzomf.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2ocdbweya.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2hpcwsxpb.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ixjwgrbd.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2dzknylbn.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2yfogvock.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2fghjlvom.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2cdgivalv.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2uylhsxll.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ntassyjy.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2hojuthoh.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2txteqshm.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2vxmqdafd.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2dkahtvxc.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2haqbbzaf.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2ntybfmlu.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2fhmnwrmj.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2gpmmsapt.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2yfrrzezy.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2glmbujij.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2eynquple.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2hsieujtn.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2lhmgmuij.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2wapyfbqg.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2kzxtfrgm.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2ixkbjoar.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2dutdsmrc.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2dfdbbczu.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2jqtgwknh.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2iubftznh.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2wtnabpuz.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2dcmqqrqc.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2ynzgwocp.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2xtdrhhvt.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2grpljrdb.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2grhwbbkn.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2agwrgcfh.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2emcdzkim.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2zujvrsdq.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2zmjiixhq.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2eyucetaq.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2rjbekwpd.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2bjvvurab.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2hnkebxop.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2swsjxuor.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2qtolqiru.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2liktvwmh.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2fqlavvya.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2lbjfrlpg.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2njbhncjg.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2nvpufjus.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2tyzwksqm.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2stehfuab.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2sttqmqiy.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2gnhsiqrl.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2ebpgssna.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2fiwzpsxx.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2sosolqfj.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2nqwdunjn.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2fedgmlof.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2cnjkgktu.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2dkbogumn.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2ouhvuwal.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2ilvtzjwy.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2mzxqtuup.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2nijvnujj.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2osowxinu.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2xriqhauk.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2cxxbzola.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2fxheuzrx.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2qysfrfwq.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2oddhekzk.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2yyugkdzx.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2hvopvpka.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2pvszebky.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2qnxgzbpi.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2ghnhzgsv.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2nrhinxpw.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2rufxlesz.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2ogckhknz.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2sgkitbxh.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2azmcrciw.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2epswhtfw.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2setvgdye.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2mfprgfcs.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2rrmwajuf.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2hqwdluil.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2vpscuzfy.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2ixcesyzn.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dtjpylxp.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2nkklunzc.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2pdskblaz.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2ooritehc.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2lpaqzkfw.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2cntmgvwo.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2gndgdjfp.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2ywbpfouw.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2exsisibj.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2jxcekopp.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2mkhkdwez.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2rlrfifbz.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2xlddduka.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2mbdpdoiy.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2cypqwoip.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2kworsblp.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2xxcsxwca.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2gjcmgejn.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2ersedhvs.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2kjztapsb.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2zpfwoznr.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2obyfmqdb.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ymjrtkbt.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2rhrdgase.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2gaffmshu.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2gucphjny.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ynsmnemt.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2tamasdhb.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2jodyvhyn.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2ygrtdqcq.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2beydffct.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2udxeybki.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2olsxrmxm.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2vpwnxdma.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2kncffdzd.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2fatmsnil.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2jusfnjzb.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xcsczqhj.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2zkybtkbm.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2zikgxamc.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2bjdmabif.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2dlexzwyh.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2ymnswahs.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2tfadhtxh.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2vjvfmvvu.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2kvdvmaoj.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2pfxjjaoj.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2kjxafwsi.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2kaifdgrx.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2pbxsjadu.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2bebzoluq.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2deinhsll.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2mcpdeyae.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2ivallbxp.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2agvzfnzc.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2nlbwilco.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2uysklobf.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ancgbdmo.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2pjsvdntn.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2wawumtyj.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2gmblaziz.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2vfwkieao.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2binbdmzq.html


<!-- 参考信息 -->