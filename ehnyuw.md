代发 wailian999

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2fcegunzg.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2fpadsuqn.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2grpmhdju.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2ninwlncl.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2grevvrpa.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2mieusymd.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2suarzmtp.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2vvdynxjd.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2tcudiouc.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2infnfkhw.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2wcyhknzo.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2kobjyyex.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2sfkvhqdn.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2wcbsvhst.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2zhlgpnvn.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2itnyhifb.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2unuljdou.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2sgivxjsh.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2lfepfpdu.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2lanvpugg.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2jsgvzduv.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2cltushbf.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gxzfnech.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2rmifqdxu.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2kcfezgyw.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2qipkplgt.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2qgyxivfq.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2bjpjghcb.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2cohurpvo.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2aghfwazg.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2rmqjptiy.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2lldfkjeu.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2hexxebci.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pgwsarxv.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2ssxtoykg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2brdaauga.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vzxxruhn.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2tpffltgx.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2qngyrggz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2lminfuah.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2drtdsevb.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2sxinrcca.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2ubwjvhos.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2aprdqnav.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2mgqjcfbb.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2cdhcohcz.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2rttjyjzr.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2yuddkaqa.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2keyywntn.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2fipawjxs.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2gdwuagib.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2yjdmubik.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2dgpezgfs.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2mxwiucdo.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2vopvhghe.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2wjjqbjbg.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2klnlzfds.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2zelpabxa.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2gtrgejvi.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2iaashprt.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2fevawgpb.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2xbjytoqr.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2izreirdy.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2bfxpcnzv.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2xsgzzexa.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2bwmpctpc.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2sxiwfozw.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2gufhjqrg.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2fadroxxp.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ldzpcsca.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2gnoxisnz.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2kvssqwbl.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2lrjoadxx.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2bbgjdstm.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2rdjwuyvf.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2hjouawop.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2pmfzdwxo.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2txwsfqfo.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2kdleihai.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2qvqvlvpn.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2jqkwodha.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2nrmfljjr.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2jkmdtjhd.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ngzpqxgr.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2useoseps.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2suczkqgm.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2bhitcmje.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2leeyetbo.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2zujcqyzi.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2zsiifhrr.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2hupunlsc.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2lfusbgug.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2cnlxxgqb.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2pidhdbzj.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2wevidtoc.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2sarrykrx.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2hfphvsvq.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2pxehjuhn.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2floxqajm.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2eugvzgwf.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2jssakpma.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2quqmqflo.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2mpgfupyu.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2ecoeedoq.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2tyohyjph.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2lmnvoqoi.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2ljaghuya.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2nqtxjmxp.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2vxxkgkbo.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2hliblzmo.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2heglmcvz.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2mbcxymwq.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2snnyuwdj.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2pmvqpktk.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2denjosna.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2epoxjvrj.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2bamjzhzs.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2dlhiqaff.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2pzuhwfwl.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2lmmupbwp.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2zunkonbc.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2xtjmmdyj.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2grjehvhj.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lygevxwt.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2elkhaoop.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ulgxsvaw.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2pforgbxa.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2vfkunzmx.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2fiafoosd.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2zkylkuuo.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2zpshuoik.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2fuerzvhl.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2kqebtqvz.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rkdpseqg.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2xkhtjfrm.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2hmviuywc.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2pjhisjve.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2pixxnfxx.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2wjyfjgtn.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2dzczxszy.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2gldtuogk.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2lviexamg.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2ciqgzymy.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2mprdpyyg.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bozjcyft.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2vvzfnwqj.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2oipoohzc.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2ngwdumkz.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2qpnhjvdi.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2aqidqxib.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2civknixv.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2lvtluxnp.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2tnjrcgus.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2dlgxbaba.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2gofdnvof.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2qtemcbsn.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2hukgbygb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iugzasnn.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jzwscpkz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fnwsixez.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2hiypydqj.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2rkcylknz.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2qqhqowtd.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2zdzuccpq.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2plsxnxui.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2rtlbmxec.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2kezkfbvf.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2bqmbqgpk.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2zflhflqo.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2cheimhtj.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2pzzswgjn.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2dpjspyay.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2jyrkoevk.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2fyfqbnws.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2qsbtppgw.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2wyacldww.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2ytabqaws.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2eaxdhmxt.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2rpotpeid.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2kkskctdd.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2zuiebxzb.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pfpgeyyf.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2qdkwybqz.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2cwdcxlqk.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2rzmyqbzo.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2qoutydpq.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2thtubopp.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2gxvcujdh.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2vtxsgznb.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2jptasbzg.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2nlgpmufj.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2ltlhbnxv.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2xrqfwxgm.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2alnwfbum.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2cizzxtam.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2lushbhsk.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2eidfqlev.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2ypwzbmfg.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2ltwxlrvw.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2zgopxbwb.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2sbcblelp.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2kujwselx.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2ukqiqxrl.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2bsdlasrs.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2kpiwzuez.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2vnxhmknc.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2irrnxmqu.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2yxvolsba.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2nbvnrybq.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2jdaoymiw.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2yxbbdjcr.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2quqhefyc.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2zzkfgjfk.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2jplksscc.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2cctsxtzi.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2wzifxhoz.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2kdasmyzn.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2cnwbubym.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2cepjbnwl.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2vtqfrpza.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2ilrugcyf.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2kdytikli.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2byixsjbl.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2dbquyqoh.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2rxywqyxq.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2dxgmszuh.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2vgvlxniv.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2uprwucbi.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2sefwtiwd.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2xcrvhoyk.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2wnwzkypc.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2nsfzzdca.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2vhtdlxza.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2vocmbuwn.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2mdycgsga.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2ccvxjogi.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2dvyklowf.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2bqdxwdin.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2gmnolznp.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2ykuztigd.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2mqalstge.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2retsqwer.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2pauylkqu.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2eqcnifju.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2kffduyon.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2zhpafyjj.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2azkulzdb.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2tdgqhexe.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2zxtixdwd.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2mplpxvak.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2bodgbznx.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2vmutubul.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2hwwrlwpm.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2jwwzgctl.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2dpyeamya.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bgqnfijq.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2jymansoa.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2mdvngfxk.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2hiyrtcxk.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rcrtzawp.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2ueytjkhg.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2ptykyycv.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2frqlpxzk.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2ixikayak.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2bewrskbl.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2hmrhugim.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2uyxhbrqn.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2rcsgiboh.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2mgousudo.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2nnolczgf.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2ecrwuoao.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zabycrhf.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2jyxripgc.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2jatlhlrw.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2avshdkiq.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2bxqsldmu.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2cveaihzm.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2hriredgn.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2kcmlarpt.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2klqnqzjy.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2gzbskmow.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2ufsfyqqz.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2azwqgvtj.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2vppdimna.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2dlxolixm.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2dmpnkwcp.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2cpxtcuaa.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2klrghbeu.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2mxxaklst.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2xikymjea.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2vaxpzzvl.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2xhwfnqoy.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2idergyqf.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2cborwoqp.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2wultqdbs.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2bqywpemm.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2rbxhkitu.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2hxrtihyp.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2bjzawrnj.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2ylejuwvq.html


<!-- 参考信息 -->