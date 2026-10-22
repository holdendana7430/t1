代发 wailian999

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2qrjbwjgu.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2mbuffgil.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2xagcvovt.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2qvlfnqdo.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2zckkytsc.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2yfrfeivr.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2qutlxbwk.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2cigttkcv.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2bbsgqlmr.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2worjlrhn.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2kpqrxbgo.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2qgfxwrco.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2csubujjf.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2axbagwvz.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qthknrpx.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2vhicayle.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2xzesmqsw.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2myozabek.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2oulpbafn.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2lrfhdokw.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2scwamwwx.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2njhnydsb.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2dzalfokn.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2fahgesxj.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2egirgnct.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vzbynjmv.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2vdxxqbau.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vyvktqbh.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2gsfxzyxa.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ztibmboe.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2kdqxwnur.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2snjazzch.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2exgsfdgw.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2ercucnfl.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2swjnrhdn.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2otkcpcdk.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ncgrfszt.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2regijfol.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2byrqskel.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2nnbejbpp.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2kvbdbpap.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2nzoqzzhi.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2aohziwbo.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2mazsactk.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2vywxvjza.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2fzvpnsog.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2sgonbhse.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2abjkkpqk.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2udpmtatn.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2ekrwjced.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2gdzkimts.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2getliarz.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2nuisovbx.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2gvbpueew.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2cnapemnt.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2deeuwxqj.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2jwtdzomp.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2xzfclizb.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2lxfkkyvi.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2drbrmwul.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2wbmsxgsd.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2bkbnooyz.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2vrpttwrf.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2pnppshdb.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2slcgpyec.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2ydpgkaki.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2lnvgfsos.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2yhxjxpgu.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2wrqvrixr.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2lzjfkalz.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2wtalebob.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2gdlwqqpy.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2goyuydan.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2bjaaymxk.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2admvjlvw.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2uidbtenj.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2xiplmbio.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2zbyutbbz.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2blhubcbg.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2iyebnrdn.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2rntnfcwc.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2knqmaagj.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ubqflgeu.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2diyemczo.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2pczkwwwp.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2jlmzrcdq.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2ptozzuvu.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2ngjdqxvo.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2gypyuczu.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2yabzpybu.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2jeetkimk.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2cavjporg.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2mwtuevbn.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2bkawibqt.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2ylmuvirs.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2udsgfchg.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2aabayscf.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2ajxyovwq.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2wvkysuis.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2oaoyqtgd.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2jlnltqpv.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2ebivkwal.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2kewxusst.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2adqgidzw.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2ycymbtuf.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2mgvuyupg.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2lwmvsntp.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2xyslmony.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2cavdcygh.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2apedgjog.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2jiyeqskv.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2hxigscre.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2qexvcjxf.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2zcnpcuwj.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2qiiufvwo.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2txjwplex.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2gevwalyv.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2oevbqwlq.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2bvdnhofm.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2sniqopdu.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2toqlwxzk.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2gpwbbdff.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2wedluejo.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2hslylfqv.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2jbwwbaik.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2xzperfvl.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2zikfkigo.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2niennomb.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2qmfshynd.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2hzjwjsuz.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2adhkjwnl.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2wmzyghrn.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ywyqzruf.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2lhahsofe.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2iwgwioro.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2vfyjymth.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fhdypylz.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2olefcqqe.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2nqamigbc.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2ydkmhmff.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2domlqzey.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2jxnqptnr.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2ymqxjvxp.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2qrfbhdhp.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2zdicfjor.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2agwyheit.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2yyxswsan.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2aylkgdwd.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2oolyrncp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2quwiimlh.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2fvgshotc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gatjlobt.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2xmrixoaa.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2hvecwndo.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2hjtwxggr.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2dtdphbar.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2aexqqjgh.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2ulyompju.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2dmpsecvd.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2etfkyhvz.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2nckphwjl.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2njfiitih.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2zffqeikc.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2iydrzbpg.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2jbntpcqv.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2vpjwxbrx.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2omouttyz.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2rbesebmf.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2ydpylprv.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2dgvvxuqw.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2gdrkjpza.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2rwcddkwb.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2bdzcghic.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rvyjtdow.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2ewoxjyqm.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2ppwohxxy.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2kwtwfwbd.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2xzjacztc.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2tcpqmkbt.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2cfbmiarc.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2qpedmeoi.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2zoxleuzk.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2ywamhieu.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2pdcmrwgc.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2ipozqlgv.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2krnngqid.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2lgwttlsr.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2qhgbekvb.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2whnjrmzj.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2aikkblvf.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2ngpabesm.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2eypwxrfz.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2qlvsjyje.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2bwtzjiwe.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2nkejraly.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2etvnpedd.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2qlqzojod.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2poogrfxu.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2sdxqdgip.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2huyqccqo.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2vtvcznsu.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2pfdmkwzs.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2gswfunfu.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2oamqxxie.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2nhzuuobs.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2nvldehoy.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2vvggvsbe.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2awjsoloh.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2tnglmapi.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2psylmtfh.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2ggbqkthb.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2omznvwzi.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2iuevmnyb.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2tporcntk.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2aoazghrq.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2qsonqaaj.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2dvkvfodu.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2ilwfbolu.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2rialcdck.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2mvbfbbvi.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2lnwvjfsx.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2dwflalap.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2karxqikx.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2zzcmwedc.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2tzucqrzp.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2opiaeivs.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2mzhjdltq.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2kbfsphdi.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2uqrtedtf.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2mjyrlacb.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2zxvcrnnm.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2aownoqat.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2gkiiwtdi.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2wjswftbr.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2skeylhtd.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2irhkxekf.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2iablvyum.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2woxpxpyv.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2udpqmvzm.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2ettnxian.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2dzjjiomy.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cvscuzsj.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2hriptssg.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2jacxamwb.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2skbsjjgy.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2kstjudws.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2wbukujzi.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bdolnqwb.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2vbodbbbo.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2iutkxwzc.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2hiknbmqf.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nynnfhzv.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2qkcrknza.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2xgfnjnge.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2nseyipbk.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2ahtcotaj.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2fjgdctwf.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2zxkcxpzu.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2vkwjqfht.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2fvkgznwi.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2yxetrbkd.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2tnebrpgh.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2efcizaec.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2tljuqxhg.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ocmvwlzu.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2pzcnuzko.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2brlqufzu.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wfrllbbj.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2xrjwbbvr.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2wnfhdngm.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2ykaiofwp.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2fbxiampy.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2bhqirozs.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2nimxelhd.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2jzegdwwl.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2mlrskyad.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2yfwqgcdi.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2xwalamrn.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2czymtuxj.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2fgpgkzhj.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2nbyjxatq.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2qveyuqix.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2oqvskjph.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2linoipuo.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2pwzgffqf.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2tieklblj.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2uvyldzxb.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2gwgyltvc.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2koyfbvfi.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2apabigkc.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2rffzodvh.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2cjbuklan.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2qukfjtyz.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2xqkqalck.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2kasylzwd.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2aseemion.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2bkhrujcr.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2izwlezku.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2wqnfieoo.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2qtszzail.html


<!-- 参考信息 -->