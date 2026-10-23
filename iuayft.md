代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ivnucfqd.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3uqzuzvfl.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3xfyhbgkj.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3gmnkeerq.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3glqjykrv.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3zefohfpd.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3qniferju.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3bfhprjmc.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3lbnjqevr.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3upkryyts.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3qqtvhaht.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3rpjzkpll.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3weemvfws.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3wbhqkxji.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3vdwxcext.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3izyokytn.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3dwfominx.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3xhjsftcm.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qwglafde.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3xwkhyrny.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3rmchbxru.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3yqzpnkxu.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3bujazqwu.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3idezljux.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3zlplqhvi.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3fkpaszmd.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3ytlhlruk.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3chpmfnfn.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3ycnaujtq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tbmbnsup.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3zoujqyhr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mnalbyfn.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qxtypqnq.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3xeuepzfb.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3jckznozm.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3abopclmz.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3dgcuqlwf.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3rcbmqfis.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3njqapzaj.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3ztsjegug.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3rltynxzg.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3iupgqgrc.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3miboutdj.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3pkvcpzrc.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ljwyiqao.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3hftubhic.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3bkzvcsno.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3wanxpyju.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3wvrdkcdh.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3bhbzxclu.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3cswqzhnr.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3xagftisj.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3risdvvmt.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3jjguzzvt.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3pqadizzc.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xmswqvdx.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3krkkddqn.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3horuseqc.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3ifbzbdpx.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3zvljyjwb.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3opsvzgda.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3ggyuhjuu.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3sjyhlxjb.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3krecrkhd.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3xwcyuaai.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3growvdtf.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3cvfvkaqc.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3onfyiluv.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3wycwuddf.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3cxklgjkv.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3awoirkvv.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3xqjaowgc.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3swiexasr.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3fysejhtw.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3bwdxuojz.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3uyjjflnv.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3mvzutiwq.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3jkwsdtjl.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3koqponvj.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3lmzoaoyy.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3wifwxdjr.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3hnllfrwv.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3efjlilsa.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3ngrbzwbn.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3wfwiphnt.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3fwfoxnif.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3smtbbxgi.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3ujvwujxi.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3wpvlnxnk.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3cmelmpag.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3ubgyqdko.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3fyvwknlu.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xzxuqdxs.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3igycvbcd.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3qubqfcir.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3uaqjruyc.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3zkghghvg.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3cusgymtf.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3vfjdzvlr.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3gochulzv.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3mvyezwqa.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3xomhscyz.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3rhrfxxll.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3bmkhyroi.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3wzyapmyy.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3sskvkafk.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3xdqogkzv.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3agpbjxwk.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3eiutbraa.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3sfxnxgsq.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3aqgtsfkn.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3wxejibxp.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3aynfqamc.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3stoeipgr.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3ubwvhpkm.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3imjqobqu.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3lszcnnpp.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3fpjtgtad.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3ewtvrueh.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bflibtlx.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3dyxpshaj.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3jmvoheyx.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3hyydxzhv.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3liwiptgs.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3ppeyyjoq.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3fhaitbmx.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3afkuzmgo.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3srdcegds.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3jhyadbzv.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3vfvocnyb.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3gppnrfcx.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3wgexsdga.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3ykqhuzur.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3eehvvupm.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3gzevmfrq.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3vqyyrckc.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3dflfnfuv.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3xvpnjaul.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3dvuyefpx.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3ybojyppf.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kzrkmoey.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3dflkmdlw.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3xzrblkcj.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3slgmwnao.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3oggxeive.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3jdjcvpve.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3rtxisofq.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3zvglbngv.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3nyiineby.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3hmicktld.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3ncoxbwch.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3smjdeibe.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3ajmonusl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sczmyrhx.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3sxqelzfz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3imkzasmv.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3uussbgsn.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3xhobwfhu.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3tolypvsh.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nazehonb.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3avxudrys.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3lwwpdwij.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3rezblfrh.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3nsieuqti.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3saabjhxk.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3rvioeprs.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3cswfflnv.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3lkgdkyym.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3leactclv.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3muaeiykv.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3tnpdcjiy.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3zapzntvs.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3urecuirf.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3hmfpqzcq.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3dwmvbyhg.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3jroaxalp.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3pzqfvdpw.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3hwbmekjx.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3dzwtekhc.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3pqedcrfs.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3wnmlpdnh.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3ilzefajx.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3drcqtrjz.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3zjicryqx.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3uqtnzqdi.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3vcmbesob.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3yuecjoiw.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3eblorhfr.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3picewnxa.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3filxytob.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3ckfheify.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3wifkipjo.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3fdxkioif.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3axzioapu.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3khhyqlim.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3jacnxigp.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3nadvucij.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3mtvebssi.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3zkahudrm.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3qzmmkjbn.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3rzmptnih.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3fqndbyhr.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3cffbtzam.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3slsbfawi.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3lhdcmraq.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3jcxddrsd.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3avajgwdi.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3efjvlonm.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3ozgdopxd.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3dhfbsazt.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3hahyflom.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3kdnngtug.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3livtrxjm.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3fzsnwdbg.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3clsozyic.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3evhmxoqj.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3girxbyln.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3ssjxkllm.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3zuknwqrl.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3qmytgdxu.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3doybfqpq.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3bwwfcdnu.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3xwupllmp.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3gpjgcfod.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3aflrndib.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3nzzbvlqq.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3ikwmwken.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3vkqitqej.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3vzpenjgr.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3omfbaivb.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3qatybpwb.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3ktfhvcoy.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3qzibdvst.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3qykysvro.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3aoeuebnb.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3cscasspq.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3ynbbxknd.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3fikswndt.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3tloouosj.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3ryupmjuu.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3bnrkesfm.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3vsnxibgr.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3psroxeuv.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3udkpffqi.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3yshrghfu.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3mafcohfw.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3ympuqdwk.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3fhlokxwf.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3lurtjqiw.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3izhumqtw.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3hmilmfzy.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3awsgtozs.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3ybvpcwbc.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3jrycthth.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3vxwgzorn.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bbxuuwtp.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3zasmdhnl.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3umcalxky.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3bysxvdqk.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3whooarda.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3iifsspch.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3gndtplnb.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3alzumlyo.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3xlmojiwn.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3rnhizsfk.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3mqxmrlls.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3hkcimcqw.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3euwvbepz.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3icfcczfm.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3ghqzzivl.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3fevtfjhh.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3xccyegxf.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3pcbkcmqc.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3oknnoyvz.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3vmsqpaju.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3fibzakjc.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3sagbwypt.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3cakaohui.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3wjpochip.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3aybfzhlv.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3uozhaoet.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3mosjyets.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3zszvndos.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3zsvqrdqq.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3axaertnj.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3dzphbvna.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3hrukjqki.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3seccytmw.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3jqbswefp.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3lnyholfk.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3yzwkpjoa.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3krjghaqa.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3tywoagor.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3whqythvf.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3ryouiamy.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3ajwdqjfa.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3ammsxvyt.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3uolfkiom.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3jbdtufgu.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3guxxpeie.html


<!-- 参考信息 -->