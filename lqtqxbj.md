代发 wailian999

while (std::getline(in, line)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjooduiac.sHtML

[S49] C++：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gfdrqvitd.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gekquelax.sHtML

[S50] C++：格式化数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gmoumrapn.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gywrmqqbn.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gvytsmoyq.sHtML

static_cast<double>(a) / b
来源：http://mobile.fanxiaobao.xyz/Article/details/ghjwvwijc.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fanxiaobao.xyz/Article/details/gwjtxcrsg.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fanxiaobao.xyz/Article/details/gxcmlnecr.sHtML

[S53] C++：移动语义
来源：http://m.share.fanxiaobao.xyz/Article/details/ggutskvvz.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fanxiaobao.xyz/Article/details/gtyynunmh.sHtML

[S54] C++：异常处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gtwmftesm.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gxebaiqmq.sHtML

[S55] C++：结构化绑定
来源：http://wap.fanxiaobao.xyz/Article/details/gmpliobim.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gwaqcskiu.sHtML

[S56] C++：optional
来源：http://3g.fanxiaobao.xyz/Article/details/gdbvhigdr.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjtbfqahb.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvaffngtz.sHtML

constexpr int N = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gxcskwqus.sHtML

[S58] C++：命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtfbfbpeq.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fanxiaobao.xyz/Article/details/glnaakvwl.sHtML

[S59] C++：静态断言
来源：http://wap.fanxiaobao.xyz/Article/details/gxzmwkajl.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fanxiaobao.xyz/Article/details/gieubwphe.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fanxiaobao.xyz/Article/details/galltlemu.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghhsxkovg.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gkjysxmzb.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fanxiaobao.xyz/Article/details/gdwqxemkd.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gctbeutio.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gbmxvtpuu.sHtML

println("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gxefixyfz.sHtML

[T02] Kotlin：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gvybzqilc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fanxiaobao.xyz/Article/details/gckrwydhd.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fanxiaobao.xyz/Article/details/gmdjktwsp.sHtML

"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gsozjaief.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fanxiaobao.xyz/Article/details/gugmoxcpg.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fanxiaobao.xyz/Article/details/gxwbzslqu.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gxvkkwpmu.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fanxiaobao.xyz/Article/details/ggfsrqmdg.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/gesvhrjtt.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxdqppmix.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcrlbfurp.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzxwjoker.sHtML

[T08] Kotlin：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/gdzrxjwuh.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fanxiaobao.xyz/Article/details/gcmzrdycq.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gnanxdorn.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fanxiaobao.xyz/Article/details/giwnifcgq.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gwlodzpho.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fanxiaobao.xyz/Article/details/gqllholmi.sHtML

[T11] Kotlin：协程
来源：http://3g.fanxiaobao.xyz/Article/details/gzkzaclpe.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fanxiaobao.xyz/Article/details/glqapidkl.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fanxiaobao.xyz/Article/details/ghrndcwyv.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gajkpalcz.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaiusvcum.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gnbqtxuza.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcgcxjuow.sHtML

for (i in 1..10) println(i)
来源：http://baike.fanxiaobao.xyz/Article/details/gyqphmagr.sHtML

[T15] Kotlin：接口
来源：http://m.share.fanxiaobao.xyz/Article/details/gubrgvbpa.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fanxiaobao.xyz/Article/details/gpnyucyjv.sHtML

[T16] Swift：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gpxiiakhj.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gpqnukahu.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gqpftpgki.sHtML

var a = 1;  let b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gpcrihpxz.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gqhdtxmcp.sHtML

"值: \(b)"
来源：http://3g.fanxiaobao.xyz/Article/details/ggwvbkbjg.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/gnddfkxlr.sHtML

if let n = opt { print(n) }
来源：http://www.share.fanxiaobao.xyz/Article/details/grbsnuccm.sHtML

[T20] Swift：数组操作
来源：http://blog.fanxiaobao.xyz/Article/details/gkfnyewqp.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzvoqoncp.sHtML

[T21] Swift：遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gqcqzxxsz.sHtML

for x in a { print(x) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxjgpflfz.sHtML

[T22] Swift：字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvwbummbb.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gefcegoqa.sHtML

[T23] Swift：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcrlzgmwj.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsgpegttr.sHtML

[T24] Swift：闭包
来源：http://www.share.fanxiaobao.xyz/Article/details/gcfoacyoi.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/gavsdrsjx.sHtML

[T25] Swift：结构体
来源：http://mobile.fanxiaobao.xyz/Article/details/ggnjncukq.sHtML

struct P { var x: Int }
来源：http://www.share.fanxiaobao.xyz/Article/details/geqmhtlyy.sHtML

[T26] Swift：类与重写
来源：http://mobile.fanxiaobao.xyz/Article/details/gjllzyrzc.sHtML

class A: Base { override func f() {} }
来源：http://3g.fanxiaobao.xyz/Article/details/grqctlvgn.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnlzfgkks.sHtML

do { try f() } catch { print(error) }
来源：http://baike.fanxiaobao.xyz/Article/details/gborhirkr.sHtML

[T28] Swift：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwlswjyhr.sHtML

enum Color { case red, green }
来源：http://www.share.fanxiaobao.xyz/Article/details/gyyfrskvt.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnauegryg.sHtML

guard let x = opt else { return }
来源：http://blog.fanxiaobao.xyz/Article/details/gawvhgoce.sHtML

[T30] Swift：协议
来源：http://m.share.fanxiaobao.xyz/Article/details/golkoaqjc.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fanxiaobao.xyz/Article/details/gpoafgkkz.sHtML

[T31] Lua：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gwvmtllzx.sHtML

print("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gknihcbtv.sHtML

[T32] Lua：局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/gjcylbduw.sHtML

local a = 1
来源：http://wap.fanxiaobao.xyz/Article/details/grhhzxenz.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fanxiaobao.xyz/Article/details/gxnshelfs.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghugcnfgr.sHtML

[T34] Lua：遍历表
来源：http://wap.fanxiaobao.xyz/Article/details/gzwhaprjr.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gknvkzxoj.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcbnhbtfm.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/grvjknfgo.sHtML

[T36] Lua：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gooskxhje.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjdhkktwa.sHtML

[T37] Lua：字符串拼接
来源：http://3g.fanxiaobao.xyz/Article/details/gxladejsn.sHtML

"a" .. "b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtoegkiqk.sHtML

[T38] Lua：条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gphanahbb.sHtML

if x > 0 then print("正") end
来源：http://www.share.fanxiaobao.xyz/Article/details/gztxswxzg.sHtML

[T39] Lua：模式匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gwzzkilqu.sHtML

string.find(s, "%d+")
来源：http://3g.fanxiaobao.xyz/Article/details/gjyomedyt.sHtML

[T40] Lua：元表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gthlvahnl.sHtML

setmetatable({}, { __index = base })
来源：http://wap.fanxiaobao.xyz/Article/details/gbqrivods.sHtML

[T41] Perl：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gjeqgcvzy.sHtML

print "Hello\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/gfvvasgpi.sHtML

[T42] Perl：变量类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gdtehbhsy.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gphjvnbup.sHtML

[T43] Perl：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gacnkfsvs.sHtML

"值: $a"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjfcxvwa.sHtML

[T44] Perl：条件
来源：http://blog.fanxiaobao.xyz/Article/details/griovbfnn.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.fanxiaobao.xyz/Article/details/grgdoijvl.sHtML

[T45] Perl：数组遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gnotjlfsi.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gisegxrkw.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gjjclfntb.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gahtbjase.sHtML

[T47] Perl：正则捕获
来源：http://mobile.fanxiaobao.xyz/Article/details/gukacfvge.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fanxiaobao.xyz/Article/details/ghdpwpslb.sHtML

[T48] Perl：正则替换
来源：http://3g.fanxiaobao.xyz/Article/details/gizcqfjlt.sHtML

$s =~ s/old/new/g;
来源：http://3g.fanxiaobao.xyz/Article/details/gwniksygw.sHtML

[T49] Perl：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gkgozduez.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxkscufwf.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gsakipzbh.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.fanxiaobao.xyz/Article/details/gennrrvei.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvlcigmfp.sHtML

[T51] Scala：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gghlmyvgr.sHtML

println("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gmmdibkqa.sHtML

[T52] Scala：变量
来源：http://blog.fanxiaobao.xyz/Article/details/gxsvwsttr.sHtML

val a = 1;  var b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gtgmjyziq.sHtML

[T53] Scala：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/glauawdvr.sHtML

s"值: $b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwjctrcar.sHtML

[T54] Scala：集合映射
来源：http://baike.fanxiaobao.xyz/Article/details/gypwoomgr.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gecspzcag.sHtML

[T55] Scala：集合过滤
来源：http://wap.fanxiaobao.xyz/Article/details/glbqshazn.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gymxtbxds.sHtML

[T56] Scala：样例类
来源：http://blog.fanxiaobao.xyz/Article/details/goybkkgio.sHtML

case class User(name: String, age: Int)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxpdehjti.sHtML

[T57] Scala：模式匹配
来源：http://blog.fanxiaobao.xyz/Article/details/glnxffllh.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.fanxiaobao.xyz/Article/details/gahhbcqmr.sHtML

[T58] Scala：函数定义
来源：http://blog.fanxiaobao.xyz/Article/details/groqkiefk.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fanxiaobao.xyz/Article/details/gfptlasod.sHtML

[T59] Scala：循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gfnhzihzb.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.fanxiaobao.xyz/Article/details/glyauxyyl.sHtML

[T60] Scala：折叠
来源：http://wap.fanxiaobao.xyz/Article/details/gotqosdwe.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.fanxiaobao.xyz/Article/details/gxvscyqab.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/ghppmwtqy.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gtpgexdbv.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdibutnnr.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.fanxiaobao.xyz/Article/details/gckceckbf.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.fanxiaobao.xyz/Article/details/gyyfoeyxj.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fanxiaobao.xyz/Article/details/gxhxqzcbq.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvctfcjfs.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.fanxiaobao.xyz/Article/details/gkoallvzr.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.fanxiaobao.xyz/Article/details/goxtptusm.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzrftixjj.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.fanxiaobao.xyz/Article/details/gmzdbotqe.sHtML

[U05] Py：列表去重且保序
来源：http://3g.fanxiaobao.xyz/Article/details/gpgxshppd.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.fanxiaobao.xyz/Article/details/gqbicveah.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gawgvumgr.sHtML

{**a, **b}
来源：http://baike.fanxiaobao.xyz/Article/details/gbylhhqts.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwiyvosbv.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fanxiaobao.xyz/Article/details/gbqscbbhc.sHtML

[U08] Py：展平二维列表
来源：http://m.share.fanxiaobao.xyz/Article/details/gritsjarc.sHtML

[y for x in nested for y in x]
来源：http://blog.fanxiaobao.xyz/Article/details/gyvzbgkrc.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.fanxiaobao.xyz/Article/details/gnxdihtia.sHtML

max(d, key=d.get)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnmumvcys.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnyyonmrq.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.fanxiaobao.xyz/Article/details/ghhhhxmif.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/grwlslzaq.sHtML

(x * 2 for x in arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gciptbajx.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gpnogpeyj.sHtML

Counter(arr).most_common(3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzyqbddaz.sHtML

[U13] Py：固定长度队列
来源：http://3g.fanxiaobao.xyz/Article/details/gakhsnbmv.sHtML

deque(maxlen=10)
来源：http://m.share.fanxiaobao.xyz/Article/details/giotsbffw.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxxmfxndh.sHtML

defaultdict(list)
来源：http://baike.fanxiaobao.xyz/Article/details/gxisorucd.sHtML

[U15] Py：高精度计时
来源：http://www.blog.fanxiaobao.xyz/Article/details/grdmuivvp.sHtML

t = time.perf_counter()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvkcwtzcm.sHtML

[U16] Py：命令行参数解析
来源：http://blog.fanxiaobao.xyz/Article/details/gumblnjte.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.fanxiaobao.xyz/Article/details/gwrxajkuq.sHtML

[U17] Py：初始化日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gbszpgxix.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzobxankl.sHtML

[U18] Py：预编译正则
来源：http://www.share.fanxiaobao.xyz/Article/details/gcsqqmxdm.sHtML

pat = re.compile(r"\d+")
来源：http://baike.fanxiaobao.xyz/Article/details/gucdtkgsu.sHtML

[U19] Py：正则替换带回调
来源：http://wap.fanxiaobao.xyz/Article/details/gdsrurhuh.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmioipduo.sHtML

[U20] Py：缓存函数结果
来源：http://3g.fanxiaobao.xyz/Article/details/gyxeuwcdp.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.fanxiaobao.xyz/Article/details/gwzhbulyb.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.fanxiaobao.xyz/Article/details/gwxwhyfqa.sHtML

@contextlib.contextmanager
来源：http://wap.fanxiaobao.xyz/Article/details/gsxnddwdp.sHtML

[U22] Py：矩阵转置
来源：http://www.share.fanxiaobao.xyz/Article/details/gdzalhkwi.sHtML

list(zip(*m))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gybyawbta.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcryxgwmx.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.fanxiaobao.xyz/Article/details/gieqwdumf.sHtML

[U24] Py：路径操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gikvpmcyg.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjalohrel.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.fanxiaobao.xyz/Article/details/gkqjghszt.sHtML

csv.DictReader(f)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwcrujscz.sHtML

[U26] Py：并发下载
来源：http://mobile.fanxiaobao.xyz/Article/details/gjlethdjm.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.fanxiaobao.xyz/Article/details/gzpwcqeco.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.fanxiaobao.xyz/Article/details/gpggajtjq.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.fanxiaobao.xyz/Article/details/gfucgmiob.sHtML

[U28] Py：类型别名
来源：http://read.share.fanxiaobao.xyz/Article/details/gnnbzkckj.sHtML

UserId = int
来源：http://baike.fanxiaobao.xyz/Article/details/gwzunqkbp.sHtML

[U29] Py：属性校验
来源：http://blog.fanxiaobao.xyz/Article/details/ghltfibcc.sHtML

@property 与 @x.setter 配合
来源：http://blog.fanxiaobao.xyz/Article/details/gefiryzeu.sHtML

[U30] Py：数据类
来源：http://mobile.fanxiaobao.xyz/Article/details/gihdrjuji.sHtML

@dataclass(slots=True)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvhipsupy.sHtML

[U31] Py：单测
来源：http://wap.fanxiaobao.xyz/Article/details/gfrddosds.sHtML

python -m pytest -q
来源：http://blog.fanxiaobao.xyz/Article/details/gzvxhtbdx.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gocmnphos.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.fanxiaobao.xyz/Article/details/gieclqnqt.sHtML

[U33] Py：打包发布
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyqdulhvo.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.fanxiaobao.xyz/Article/details/gvrtaoqvl.sHtML

[U34] Py：判断编码
来源：http://baike.fanxiaobao.xyz/Article/details/gskbrzbbz.sHtML

chardet.detect(raw)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggdjcjjeu.sHtML

[U35] Py：发送邮件
来源：http://wap.fanxiaobao.xyz/Article/details/gekforsev.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyeqymzay.sHtML

[U36] Py：定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/ggmxchqgk.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvohcppvh.sHtML

[U37] Py：读写 Excel
来源：http://m.share.fanxiaobao.xyz/Article/details/gzrpxjwuk.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghynzwmmb.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.fanxiaobao.xyz/Article/details/gwobdvcck.sHtML

Path(__file__).resolve().parent
来源：http://baike.fanxiaobao.xyz/Article/details/ghcfgtxnp.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.fanxiaobao.xyz/Article/details/gjlijcyws.sHtML

sys.stdout.isatty()
来源：http://www.share.fanxiaobao.xyz/Article/details/glpmefhvz.sHtML

[U40] Py：打印到标准错误
来源：http://3g.fanxiaobao.xyz/Article/details/gownxcfvg.sHtML

print("err", file=sys.stderr)
来源：http://wap.fanxiaobao.xyz/Article/details/gqppttxmm.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsfsvbvly.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.fanxiaobao.xyz/Article/details/gdzzhryja.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gglpehlyv.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.fanxiaobao.xyz/Article/details/gydkwoejg.sHtML

[U43] PHP：声明命名空间
来源：http://3g.fanxiaobao.xyz/Article/details/gtubfther.sHtML

namespace App\Http;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdminysxv.sHtML

[U44] PHP：开启严格类型
来源：http://baike.fanxiaobao.xyz/Article/details/gihznmhei.sHtML

declare(strict_types=1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdifibvvh.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gmvsnbgoj.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdvzurwda.sHtML

[U46] PHP：可空类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyibdyojr.sHtML

?string $name = null
来源：http://read.share.fanxiaobao.xyz/Article/details/gsuxjskbs.sHtML

[U47] PHP：联合类型
来源：http://blog.fanxiaobao.xyz/Article/details/grdrnjuoe.sHtML

int|string $id
来源：http://www.blog.fanxiaobao.xyz/Article/details/gseuccrun.sHtML

[U48] PHP：纯枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gjnjnxpxg.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gxcpcyatm.sHtML

[U49] PHP：只读属性
来源：http://www.share.fanxiaobao.xyz/Article/details/guiwbievs.sHtML

public readonly string $name
来源：http://blog.fanxiaobao.xyz/Article/details/galwbxksu.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.fanxiaobao.xyz/Article/details/giewnkjew.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjgmggpgj.sHtML

[U51] PHP：数组解构
来源：http://baike.fanxiaobao.xyz/Article/details/gurpcfbtu.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwiikcdns.sHtML

[U52] PHP：箭头函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gxvzgctbd.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.fanxiaobao.xyz/Article/details/gwiztolzm.sHtML

[U53] PHP：空合并运算符
来源：http://wap.fanxiaobao.xyz/Article/details/ghbxmoopc.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.fanxiaobao.xyz/Article/details/gknkmnufm.sHtML

[U54] PHP：空安全调用
来源：http://baike.fanxiaobao.xyz/Article/details/gczbfpedp.sHtML

$obj?->method()
来源：http://m.share.fanxiaobao.xyz/Article/details/gipcusqit.sHtML

[U55] PHP：match 表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gpdyydmhk.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.fanxiaobao.xyz/Article/details/gvhlkvloy.sHtML

[U56] PHP：命名参数
来源：http://baike.fanxiaobao.xyz/Article/details/gkjogfomh.sHtML

f(a: 1, b: 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gnflwefju.sHtML

[U57] PHP：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gdvymtfkg.sHtML

"值: {$a}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gmuqymptc.sHtML

[U58] PHP：数组三件套
来源：http://blog.fanxiaobao.xyz/Article/details/gkdvvlvdu.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfqynjpja.sHtML

[U59] PHP：自定义排序
来源：http://baike.fanxiaobao.xyz/Article/details/gnzfuqodc.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fanxiaobao.xyz/Article/details/gpmyutuvy.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gerbbetcl.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.fanxiaobao.xyz/Article/details/giegphfyz.sHtML

[U61] PHP：正则
来源：http://baike.fanxiaobao.xyz/Article/details/gknvlegra.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gchdabnoe.sHtML

[U62] PHP：日期对象
来源：http://baike.fanxiaobao.xyz/Article/details/gbepiywnk.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gypbiubka.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtsfxetht.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.fanxiaobao.xyz/Article/details/gbafhawrv.sHtML

[U64] PHP：目录遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gqnieufna.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.fanxiaobao.xyz/Article/details/ghmsgdmvg.sHtML

[U65] PHP：会话
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggmtxclhe.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyjkqusry.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdtfcwgjx.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbukgzjmt.sHtML

[U67] PHP：处理文件上传
来源：http://baike.fanxiaobao.xyz/Article/details/gqkqsrrmy.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.fanxiaobao.xyz/Article/details/gkkzghwjq.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gckzkjjts.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyzfiijng.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjpbjlpvc.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gawegphos.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gptfhobuo.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.fanxiaobao.xyz/Article/details/gddfwbizt.sHtML

[U71] PHP：抛出异常
来源：http://read.share.fanxiaobao.xyz/Article/details/gvxvdaaia.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.fanxiaobao.xyz/Article/details/gyxmezxcw.sHtML

[U72] PHP：写错误日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gikqmoinw.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gamedoyxh.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmwcoqiae.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gysmibscu.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gkxulgszn.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.fanxiaobao.xyz/Article/details/gnjadwtgs.sHtML


<!-- 参考信息 -->