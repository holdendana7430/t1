代发 wailian999

[S45] C++：lambda
来源：http://read.share.zdbjq.cn/Article/details/gaxkqmysg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.hesvh.cn/Article/details/gtascwipv.sHtML

[S46] C++：函数模板
来源：http://read.share.zdbjq.cn/Article/details/glovsbjnj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.zdbjq.cn/Article/details/guavtwpzf.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.zdbjq.cn/Article/details/gevypcccl.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fehbvm.com/Article/details/gbxsylber.sHtML

[S48] C++：逐行读文件
来源：http://baike.fehbvm.com/Article/details/goesnouqj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.zdbjq.cn/Article/details/gvopdbmvq.sHtML

while (std::getline(in, line)) { }
来源：http://blog.hesvh.cn/Article/details/giuyplldp.sHtML

[S49] C++：写文件
来源：http://3g.fehbvm.com/Article/details/gsxzwphni.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fehbvm.com/Article/details/gitmbwsoi.sHtML

[S50] C++：格式化数字
来源：http://wap.zdbjq.cn/Article/details/gjaeonldw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gjapejwle.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fehbvm.com/Article/details/gxsiymgor.sHtML

static_cast<double>(a) / b
来源：http://mobile.zdbjq.cn/Article/details/godmszbqv.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.zdbjq.cn/Article/details/gcojnlvne.sHtML

int size() const noexcept { return n_; }
来源：http://blog.zdbjq.cn/Article/details/gfupfunmo.sHtML

[S53] C++：移动语义
来源：http://www.blog.zdbjq.cn/Article/details/gjbgrsejh.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.zdbjq.cn/Article/details/gobiwmfzq.sHtML

[S54] C++：异常处理
来源：http://www.share.hesvh.cn/Article/details/goaeytrti.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fehbvm.com/Article/details/gnyzjzkuk.sHtML

[S55] C++：结构化绑定
来源：http://3g.hesvh.cn/Article/details/gqgjerxmb.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.zdbjq.cn/Article/details/gboqexbyu.sHtML

[S56] C++：optional
来源：http://wap.fehbvm.com/Article/details/ghjovdlwk.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjjszenio.sHtML

[S57] C++：编译期常量
来源：http://m.share.zdbjq.cn/Article/details/gekqkrgpz.sHtML

constexpr int N = 10;
来源：http://www.share.fehbvm.com/Article/details/gftkfhsdd.sHtML

[S58] C++：命名空间
来源：http://blog.fehbvm.com/Article/details/gthyxwbcb.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.zdbjq.cn/Article/details/gjzipkkvy.sHtML

[S59] C++：静态断言
来源：http://mobile.zdbjq.cn/Article/details/gqcqpsowr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.zdbjq.cn/Article/details/ghfroompx.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fehbvm.com/Article/details/gqfeszkkt.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fehbvm.com/Article/details/gziksaxvq.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ghqrmtpwk.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.hesvh.cn/Article/details/gnpourtxc.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/goivzeict.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gcdhsabpy.sHtML

println("Hello")
来源：http://baike.fehbvm.com/Article/details/gdqburrvx.sHtML

[T02] Kotlin：变量
来源：http://www.share.hesvh.cn/Article/details/gfwgtqstb.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.zdbjq.cn/Article/details/gwdqcbjxm.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.hesvh.cn/Article/details/ghcwfcetu.sHtML

"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/gwptptuxm.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fehbvm.com/Article/details/gkojenjal.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fehbvm.com/Article/details/gbwzuzajg.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.hesvh.cn/Article/details/gqmldyulv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.zdbjq.cn/Article/details/ggvqzdusp.sHtML

[T06] Kotlin：集合映射
来源：http://baike.hesvh.cn/Article/details/gewwqaamr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.zdbjq.cn/Article/details/gnfhwpvws.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.zdbjq.cn/Article/details/gglbbjvsx.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.hesvh.cn/Article/details/gagwdgjks.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fehbvm.com/Article/details/gyafxqxhf.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fehbvm.com/Article/details/gwvglzexl.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fehbvm.com/Article/details/gnymkngjo.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.zdbjq.cn/Article/details/gsehjywpu.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.zdbjq.cn/Article/details/giwacposk.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.hesvh.cn/Article/details/gupqhrddh.sHtML

[T11] Kotlin：协程
来源：http://baike.fehbvm.com/Article/details/goybitzzq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fehbvm.com/Article/details/gxmsnkrim.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.zdbjq.cn/Article/details/govdxbpkv.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.hesvh.cn/Article/details/gdyrfdjfb.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.hesvh.cn/Article/details/gbncuxrlv.sHtML

val m = mapOf("a" to 1)
来源：http://wap.zdbjq.cn/Article/details/gedaetrlq.sHtML

[T14] Kotlin：循环
来源：http://wap.fehbvm.com/Article/details/gxoobzwnf.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/ghmcckdtz.sHtML

[T15] Kotlin：接口
来源：http://www.share.zdbjq.cn/Article/details/gbtayidfq.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fehbvm.com/Article/details/gruirgibi.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gjgynpkgs.sHtML

print("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gniyjrsnl.sHtML

[T17] Swift：变量与常量
来源：http://3g.fehbvm.com/Article/details/gkfwyfcxj.sHtML

var a = 1;  let b = 2
来源：http://baike.fehbvm.com/Article/details/gjfqjetod.sHtML

[T18] Swift：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gdvxbojcv.sHtML

"值: \(b)"
来源：http://wap.zdbjq.cn/Article/details/gncmifvii.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.hesvh.cn/Article/details/goqsrdlid.sHtML

if let n = opt { print(n) }
来源：http://wap.hesvh.cn/Article/details/gfzojdsuc.sHtML

[T20] Swift：数组操作
来源：http://m.share.hesvh.cn/Article/details/gpgsvcrzi.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.zdbjq.cn/Article/details/gjjfxilef.sHtML

[T21] Swift：遍历
来源：http://wap.zdbjq.cn/Article/details/gjbtqhshj.sHtML

for x in a { print(x) }
来源：http://www.blog.zdbjq.cn/Article/details/gmmbzouki.sHtML

[T22] Swift：字典
来源：http://3g.fehbvm.com/Article/details/gjdqcxnay.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.hesvh.cn/Article/details/gslyvtilg.sHtML

[T23] Swift：函数
来源：http://blog.hesvh.cn/Article/details/ghwdzqexu.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.fehbvm.com/Article/details/gqcmggkiu.sHtML

[T24] Swift：闭包
来源：http://www.m.share.zdbjq.cn/Article/details/gtyifihza.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fehbvm.com/Article/details/gmnvvfxwl.sHtML

[T25] Swift：结构体
来源：http://www.m.share.hesvh.cn/Article/details/gekxgqsdk.sHtML

struct P { var x: Int }
来源：http://www.m.share.zdbjq.cn/Article/details/gixsmjefb.sHtML

[T26] Swift：类与重写
来源：http://wap.fehbvm.com/Article/details/gggowxaph.sHtML

class A: Base { override func f() {} }
来源：http://m.share.hesvh.cn/Article/details/gkyphiuiu.sHtML

[T27] Swift：错误处理
来源：http://blog.hesvh.cn/Article/details/glalrrmlw.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.fehbvm.com/Article/details/gvkcunwgk.sHtML

[T28] Swift：枚举
来源：http://www.share.zdbjq.cn/Article/details/gqrtiiyub.sHtML

enum Color { case red, green }
来源：http://m.share.zdbjq.cn/Article/details/greqivabi.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.zdbjq.cn/Article/details/gsmohgiyq.sHtML

guard let x = opt else { return }
来源：http://3g.zdbjq.cn/Article/details/griqyfmcq.sHtML

[T30] Swift：协议
来源：http://www.blog.fehbvm.com/Article/details/gmhbkozpk.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.hesvh.cn/Article/details/gvckeerwx.sHtML

[T31] Lua：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gvtmneyba.sHtML

print("Hello")
来源：http://wap.fehbvm.com/Article/details/gmtoeznqz.sHtML

[T32] Lua：局部变量
来源：http://read.share.zdbjq.cn/Article/details/gpoumnwzy.sHtML

local a = 1
来源：http://3g.zdbjq.cn/Article/details/ghzoxbmfo.sHtML

[T33] Lua：表（数组）
来源：http://wap.fehbvm.com/Article/details/gryzlctrs.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.hesvh.cn/Article/details/guavyvtog.sHtML

[T34] Lua：遍历表
来源：http://www.share.zdbjq.cn/Article/details/gjtzwgdef.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fehbvm.com/Article/details/ghibwuwgz.sHtML

[T35] Lua：字典表
来源：http://wap.fehbvm.com/Article/details/gvyuctman.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.hesvh.cn/Article/details/gxnemelje.sHtML

[T36] Lua：函数
来源：http://blog.fehbvm.com/Article/details/gahuxjuga.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.fehbvm.com/Article/details/gcxxxtxvi.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.hesvh.cn/Article/details/gluymuiac.sHtML

"a" .. "b"
来源：http://read.share.hesvh.cn/Article/details/ghathhcyr.sHtML

[T38] Lua：条件
来源：http://www.m.share.fehbvm.com/Article/details/gdikmizdl.sHtML

if x > 0 then print("正") end
来源：http://m.share.zdbjq.cn/Article/details/gjsbewtwj.sHtML

[T39] Lua：模式匹配
来源：http://baike.fehbvm.com/Article/details/goqdmevdp.sHtML

string.find(s, "%d+")
来源：http://www.blog.zdbjq.cn/Article/details/gkloluocj.sHtML

[T40] Lua：元表
来源：http://www.share.hesvh.cn/Article/details/giorctsat.sHtML

setmetatable({}, { __index = base })
来源：http://3g.fehbvm.com/Article/details/glvrtvtnt.sHtML

[T41] Perl：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gzmbhxfnh.sHtML

print "Hello\n";
来源：http://mobile.fehbvm.com/Article/details/gmafahecb.sHtML

[T42] Perl：变量类型
来源：http://blog.fehbvm.com/Article/details/grdnawqrn.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.fehbvm.com/Article/details/gzeleajpy.sHtML

[T43] Perl：字符串插值
来源：http://baike.fehbvm.com/Article/details/goacipjlf.sHtML

"值: $a"
来源：http://blog.zdbjq.cn/Article/details/gurcijrkv.sHtML

[T44] Perl：条件
来源：http://wap.zdbjq.cn/Article/details/glfkuxpzb.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.hesvh.cn/Article/details/gjbeudfiw.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.hesvh.cn/Article/details/gkbcvjfol.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.fehbvm.com/Article/details/ggcxxlgzc.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.hesvh.cn/Article/details/gmubxeetw.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.zdbjq.cn/Article/details/gqlnwbfsb.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.hesvh.cn/Article/details/gglxavfdf.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqzshsjfr.sHtML

[T48] Perl：正则替换
来源：http://blog.hesvh.cn/Article/details/gacgzutrp.sHtML

$s =~ s/old/new/g;
来源：http://m.share.fehbvm.com/Article/details/gvjownjez.sHtML

[T49] Perl：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gcuplcxzd.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gssaoeaht.sHtML

[T50] Perl：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gqzmvamzp.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.fehbvm.com/Article/details/gizfgigps.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.hesvh.cn/Article/details/gthdhcenr.sHtML

[T51] Scala：Hello World
来源：http://blog.hesvh.cn/Article/details/gfjggzqdv.sHtML

println("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gzfofabta.sHtML

[T52] Scala：变量
来源：http://mobile.fehbvm.com/Article/details/gubbsfymq.sHtML

val a = 1;  var b = 2
来源：http://www.share.fehbvm.com/Article/details/gxjwocqtb.sHtML

[T53] Scala：字符串插值
来源：http://mobile.hesvh.cn/Article/details/guzhbsoqt.sHtML

s"值: $b"
来源：http://www.blog.fehbvm.com/Article/details/gnsveupdm.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.fehbvm.com/Article/details/gbkozbcld.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.fehbvm.com/Article/details/gavgmyubm.sHtML

[T55] Scala：集合过滤
来源：http://read.share.zdbjq.cn/Article/details/giugdaiod.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.fehbvm.com/Article/details/gsjkuguet.sHtML

[T56] Scala：样例类
来源：http://www.blog.hesvh.cn/Article/details/giwgypkoh.sHtML

case class User(name: String, age: Int)
来源：http://www.share.fehbvm.com/Article/details/gkhspstlp.sHtML

[T57] Scala：模式匹配
来源：http://m.share.hesvh.cn/Article/details/gjheewnif.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.hesvh.cn/Article/details/gtyyeejgd.sHtML

[T58] Scala：函数定义
来源：http://mobile.zdbjq.cn/Article/details/gquoahyeh.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.hesvh.cn/Article/details/gzdbuzxwm.sHtML

[T59] Scala：循环
来源：http://baike.fehbvm.com/Article/details/ggdhkbhpb.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.fehbvm.com/Article/details/gtihmygja.sHtML

[T60] Scala：折叠
来源：http://3g.hesvh.cn/Article/details/goddtvlbv.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.hesvh.cn/Article/details/ghwuawzty.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gjuwicduh.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fehbvm.com/Article/details/gbjlwssav.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gzdfwddjs.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.hesvh.cn/Article/details/gjfetixnn.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.hesvh.cn/Article/details/gtkqmmbck.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.zdbjq.cn/Article/details/grzrjftrd.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.zdbjq.cn/Article/details/gujyjhriy.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.hesvh.cn/Article/details/gontfilkx.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.hesvh.cn/Article/details/gxxbfofsv.sHtML

[U04] Py：变量调试打印
来源：http://3g.fehbvm.com/Article/details/gigbicard.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.zdbjq.cn/Article/details/gblwsjkva.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.zdbjq.cn/Article/details/gqtrosmza.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.zdbjq.cn/Article/details/gqevwixus.sHtML

[U06] Py：合并两个字典
来源：http://wap.hesvh.cn/Article/details/gcvnunisj.sHtML

{**a, **b}
来源：http://mobile.zdbjq.cn/Article/details/gudxyzysi.sHtML

[U07] Py：反转字典键值
来源：http://wap.hesvh.cn/Article/details/gimugaqto.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.fehbvm.com/Article/details/gxcalicol.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.fehbvm.com/Article/details/gpolhwvpm.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.fehbvm.com/Article/details/gjojqelrc.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.hesvh.cn/Article/details/grvfaeytx.sHtML

max(d, key=d.get)
来源：http://www.blog.zdbjq.cn/Article/details/gidfehkbv.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.hesvh.cn/Article/details/gvjwxfrnb.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.zdbjq.cn/Article/details/gypfqqypk.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.hesvh.cn/Article/details/gwbfikvzy.sHtML

(x * 2 for x in arr)
来源：http://wap.hesvh.cn/Article/details/gknggbwzp.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.fehbvm.com/Article/details/gheinnzwm.sHtML

Counter(arr).most_common(3)
来源：http://mobile.fehbvm.com/Article/details/gyrrzayap.sHtML

[U13] Py：固定长度队列
来源：http://3g.hesvh.cn/Article/details/gnwemfcml.sHtML

deque(maxlen=10)
来源：http://www.share.fehbvm.com/Article/details/gxrhavyne.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.hesvh.cn/Article/details/gplfwvafi.sHtML

defaultdict(list)
来源：http://read.share.zdbjq.cn/Article/details/ghhpjdfbb.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.hesvh.cn/Article/details/gsdtylpsl.sHtML

t = time.perf_counter()
来源：http://www.blog.hesvh.cn/Article/details/ghuhumbof.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.hesvh.cn/Article/details/gdpkbugtm.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.zdbjq.cn/Article/details/gbrxbfbxl.sHtML

[U17] Py：初始化日志
来源：http://m.share.hesvh.cn/Article/details/gsmmgwzpi.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.hesvh.cn/Article/details/groyshcpt.sHtML

[U18] Py：预编译正则
来源：http://3g.zdbjq.cn/Article/details/gtmtthpbn.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.hesvh.cn/Article/details/gfetqrfnr.sHtML

[U19] Py：正则替换带回调
来源：http://baike.fehbvm.com/Article/details/grqutcdkx.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.hesvh.cn/Article/details/gxpbwkycb.sHtML

[U20] Py：缓存函数结果
来源：http://blog.hesvh.cn/Article/details/gbzbzklqk.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.zdbjq.cn/Article/details/glhafjinb.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.hesvh.cn/Article/details/gtdibynci.sHtML

@contextlib.contextmanager
来源：http://blog.hesvh.cn/Article/details/gzowmewau.sHtML

[U22] Py：矩阵转置
来源：http://baike.fehbvm.com/Article/details/gzfwffgiu.sHtML

list(zip(*m))
来源：http://wap.hesvh.cn/Article/details/gvryhsemj.sHtML

[U23] Py：分块读取大文件
来源：http://3g.zdbjq.cn/Article/details/gulrhwsfy.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.hesvh.cn/Article/details/gnkfcsbdc.sHtML

[U24] Py：路径操作
来源：http://m.share.hesvh.cn/Article/details/ggibhepuh.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.fehbvm.com/Article/details/gahkhoqsm.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.hesvh.cn/Article/details/ghzkhizdd.sHtML

csv.DictReader(f)
来源：http://m.share.hesvh.cn/Article/details/gxqpyeqkg.sHtML

[U26] Py：并发下载
来源：http://wap.zdbjq.cn/Article/details/gtomzmype.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.hesvh.cn/Article/details/gpbfwbval.sHtML

[U27] Py：异步 HTTP
来源：http://baike.hesvh.cn/Article/details/guamknfur.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.hesvh.cn/Article/details/gvjvqgbqv.sHtML

[U28] Py：类型别名
来源：http://blog.fehbvm.com/Article/details/gqlylmntm.sHtML

UserId = int
来源：http://www.m.share.zdbjq.cn/Article/details/gkjfvenzh.sHtML

[U29] Py：属性校验
来源：http://3g.fehbvm.com/Article/details/gibehmqyi.sHtML

@property 与 @x.setter 配合
来源：http://m.share.hesvh.cn/Article/details/ggubxuzar.sHtML

[U30] Py：数据类
来源：http://blog.hesvh.cn/Article/details/gsgujjnry.sHtML

@dataclass(slots=True)
来源：http://www.share.fehbvm.com/Article/details/gtgtqfsug.sHtML

[U31] Py：单测
来源：http://wap.zdbjq.cn/Article/details/gunkybbdn.sHtML

python -m pytest -q
来源：http://www.blog.fehbvm.com/Article/details/gpdmglszt.sHtML

[U32] Py：代码格式化
来源：http://m.share.zdbjq.cn/Article/details/gjdskbfhu.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.fehbvm.com/Article/details/gbniresvv.sHtML

[U33] Py：打包发布
来源：http://blog.fehbvm.com/Article/details/gyxnlgrqq.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.zdbjq.cn/Article/details/guswkpmwq.sHtML

[U34] Py：判断编码
来源：http://baike.hesvh.cn/Article/details/gquwjeupi.sHtML

chardet.detect(raw)
来源：http://3g.hesvh.cn/Article/details/gbiagfgnj.sHtML

[U35] Py：发送邮件
来源：http://www.share.zdbjq.cn/Article/details/grmvvhzkf.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.fehbvm.com/Article/details/gisbobpbj.sHtML

[U36] Py：定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/gwvahougy.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.fehbvm.com/Article/details/gjkgfkjic.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.fehbvm.com/Article/details/gtlvbuepv.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.hesvh.cn/Article/details/gqrcifvcf.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.hesvh.cn/Article/details/gmbmaetzk.sHtML

Path(__file__).resolve().parent
来源：http://3g.zdbjq.cn/Article/details/ghxqktqve.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.hesvh.cn/Article/details/gxasskeix.sHtML

sys.stdout.isatty()
来源：http://baike.zdbjq.cn/Article/details/gwvcyiicg.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.fehbvm.com/Article/details/gnavdlcwo.sHtML

print("err", file=sys.stderr)
来源：http://read.share.zdbjq.cn/Article/details/gshzpqhif.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.zdbjq.cn/Article/details/gbaolupfd.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.zdbjq.cn/Article/details/ghlpmfljm.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.fehbvm.com/Article/details/gooasrkvq.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.fehbvm.com/Article/details/ghchbifel.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.hesvh.cn/Article/details/gfktfyklb.sHtML

namespace App\Http;
来源：http://3g.fehbvm.com/Article/details/gveyrqxce.sHtML

[U44] PHP：开启严格类型
来源：http://3g.hesvh.cn/Article/details/gkszlnhfo.sHtML

declare(strict_types=1);
来源：http://wap.hesvh.cn/Article/details/grrkgtmky.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.fehbvm.com/Article/details/gvxbybygl.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gzoxduwow.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.hesvh.cn/Article/details/gmuhmhahm.sHtML

?string $name = null
来源：http://m.share.fehbvm.com/Article/details/gdpnhnund.sHtML

[U47] PHP：联合类型
来源：http://wap.hesvh.cn/Article/details/gnhriadcq.sHtML

int|string $id
来源：http://blog.fehbvm.com/Article/details/gecojglzs.sHtML

[U48] PHP：纯枚举
来源：http://read.share.hesvh.cn/Article/details/gfxcuegns.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.fehbvm.com/Article/details/gnxuzpnyj.sHtML

[U49] PHP：只读属性
来源：http://www.blog.zdbjq.cn/Article/details/gkjgbxfhf.sHtML

public readonly string $name
来源：http://read.share.hesvh.cn/Article/details/giudchbyf.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.zdbjq.cn/Article/details/gahvxxiar.sHtML

public function __construct(private int $id) {}
来源：http://blog.fehbvm.com/Article/details/grzfwhpoh.sHtML

[U51] PHP：数组解构
来源：http://3g.zdbjq.cn/Article/details/gxngtnhqw.sHtML

[$a, $b] = $arr;
来源：http://wap.hesvh.cn/Article/details/gazmxswza.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.hesvh.cn/Article/details/gogvmsjrf.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.zdbjq.cn/Article/details/gncpzbwmw.sHtML

[U53] PHP：空合并运算符
来源：http://wap.hesvh.cn/Article/details/gpnzwyiye.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.zdbjq.cn/Article/details/gplidcjjp.sHtML

[U54] PHP：空安全调用
来源：http://3g.zdbjq.cn/Article/details/gedmvuzeq.sHtML

$obj?->method()
来源：http://baike.fehbvm.com/Article/details/gfucvqbix.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.hesvh.cn/Article/details/gxevngwnk.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.zdbjq.cn/Article/details/gormlnvpd.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.fehbvm.com/Article/details/ghwwxbxrs.sHtML

f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/gmhxtijvg.sHtML

[U57] PHP：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gooinasgq.sHtML

"值: {$a}"
来源：http://baike.zdbjq.cn/Article/details/gaclazuya.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.fehbvm.com/Article/details/ghoklnzkz.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.hesvh.cn/Article/details/gechzdgrv.sHtML

[U59] PHP：自定义排序
来源：http://baike.zdbjq.cn/Article/details/gyqirstxa.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.zdbjq.cn/Article/details/gkjfksaya.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.fehbvm.com/Article/details/gzympuxug.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.zdbjq.cn/Article/details/gcnkcdmcw.sHtML

[U61] PHP：正则
来源：http://read.share.fehbvm.com/Article/details/guvdtvzef.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.fehbvm.com/Article/details/gfjivroxi.sHtML

[U62] PHP：日期对象
来源：http://3g.fehbvm.com/Article/details/gdpocbybn.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.fehbvm.com/Article/details/gbablvcth.sHtML

[U63] PHP：文件读写
来源：http://read.share.zdbjq.cn/Article/details/gjtpeyqli.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.fehbvm.com/Article/details/grfyjxcde.sHtML

[U64] PHP：目录遍历
来源：http://www.share.hesvh.cn/Article/details/gxvmlfygw.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.hesvh.cn/Article/details/gmnzbgchr.sHtML

[U65] PHP：会话
来源：http://3g.fehbvm.com/Article/details/grwcddmzo.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gyifsqhec.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.hesvh.cn/Article/details/gkrlfdgct.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.hesvh.cn/Article/details/gunydbpvz.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.hesvh.cn/Article/details/grodsepob.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.hesvh.cn/Article/details/gvfzcuquh.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.fehbvm.com/Article/details/gldbbaqnf.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.zdbjq.cn/Article/details/ggovssrpw.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.hesvh.cn/Article/details/gttqzbuxf.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.zdbjq.cn/Article/details/gjrhvgwnk.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.fehbvm.com/Article/details/grzjnvluv.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.hesvh.cn/Article/details/glvxrxmwo.sHtML


<!-- 参考信息 -->