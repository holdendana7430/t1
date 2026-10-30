代发 wailian999

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gijfrpbyt.sHtML

[S55] C++：结构化绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gganugpjv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqubulttc.sHtML

[S56] C++：optional
来源：http://mobile.fanxiaobao.xyz/Article/details/ggodvugsp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gktqaknvh.sHtML

[S57] C++：编译期常量
来源：http://baike.fanxiaobao.xyz/Article/details/gvynndzeg.sHtML

constexpr int N = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpvqffdey.sHtML

[S58] C++：命名空间
来源：http://www.share.fanxiaobao.xyz/Article/details/gkcvtvxsi.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fanxiaobao.xyz/Article/details/gpmwmoygf.sHtML

[S59] C++：静态断言
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyqjjeeam.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fanxiaobao.xyz/Article/details/gkdfdqsnc.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fanxiaobao.xyz/Article/details/gqxjhjcqc.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gwjkowbzm.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/grzcyzeho.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfxaevdgk.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtzezskfr.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gvdplyhea.sHtML

println("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/giwymvqqo.sHtML

[T02] Kotlin：变量
来源：http://3g.fanxiaobao.xyz/Article/details/gvoqkvcul.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fanxiaobao.xyz/Article/details/gytlsulwv.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fanxiaobao.xyz/Article/details/gzppweqbl.sHtML

"值: $b"
来源：http://read.share.fanxiaobao.xyz/Article/details/giydjonsm.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fanxiaobao.xyz/Article/details/gwwhiddmh.sHtML

val n: String? = null;  n?.length
来源：http://baike.fanxiaobao.xyz/Article/details/gchaybbge.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fanxiaobao.xyz/Article/details/geamjmvyu.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fanxiaobao.xyz/Article/details/ghbouigza.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fanxiaobao.xyz/Article/details/gldfhuzhg.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/galeqrmjg.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fanxiaobao.xyz/Article/details/galomwlnk.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fanxiaobao.xyz/Article/details/gzgyaawfh.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fanxiaobao.xyz/Article/details/gufuzgdow.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/gjcyvwlnm.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fanxiaobao.xyz/Article/details/gxkjvtcnv.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fanxiaobao.xyz/Article/details/gcdxojksc.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/giowsjdad.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fanxiaobao.xyz/Article/details/gmspgumlr.sHtML

[T11] Kotlin：协程
来源：http://3g.fanxiaobao.xyz/Article/details/glslosbhs.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtigpnqtn.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fanxiaobao.xyz/Article/details/gvlfywqzy.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbngvsxiz.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.fanxiaobao.xyz/Article/details/gzgmdgvpz.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gbdbdkpjm.sHtML

[T14] Kotlin：循环
来源：http://mobile.fanxiaobao.xyz/Article/details/guabpvhsa.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gycckbyoq.sHtML

[T15] Kotlin：接口
来源：http://read.share.fanxiaobao.xyz/Article/details/gyjdumqah.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/grlixsjit.sHtML

[T16] Swift：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gtnijanjv.sHtML

print("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gcujkdoqm.sHtML

[T17] Swift：变量与常量
来源：http://baike.fanxiaobao.xyz/Article/details/ggwpncrlk.sHtML

var a = 1;  let b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gynfloexa.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gufcafotb.sHtML

"值: \(b)"
来源：http://read.share.fanxiaobao.xyz/Article/details/gvjokbjxb.sHtML

[T19] Swift：可选绑定
来源：http://wap.fanxiaobao.xyz/Article/details/glkelxxrl.sHtML

if let n = opt { print(n) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gktsmeevi.sHtML

[T20] Swift：数组操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gnoqjlxlm.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqquqnsxe.sHtML

[T21] Swift：遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/ghvlbmort.sHtML

for x in a { print(x) }
来源：http://blog.fanxiaobao.xyz/Article/details/gllsxmxhi.sHtML

[T22] Swift：字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gvhltvfhu.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.fanxiaobao.xyz/Article/details/ghtmgfnyj.sHtML

[T23] Swift：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gcunxltwo.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzhgaxnoj.sHtML

[T24] Swift：闭包
来源：http://read.share.fanxiaobao.xyz/Article/details/ghirsuywy.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkdnxpvgq.sHtML

[T25] Swift：结构体
来源：http://www.share.fanxiaobao.xyz/Article/details/gvxltsoiz.sHtML

struct P { var x: Int }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggehhmhwj.sHtML

[T26] Swift：类与重写
来源：http://wap.fanxiaobao.xyz/Article/details/gvnhgxayh.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvmuqsgzi.sHtML

[T27] Swift：错误处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gnhmrywwo.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnmdtujin.sHtML

[T28] Swift：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/glrlgpyst.sHtML

enum Color { case red, green }
来源：http://wap.fanxiaobao.xyz/Article/details/gcpdoucek.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqeljblig.sHtML

guard let x = opt else { return }
来源：http://baike.fanxiaobao.xyz/Article/details/gktkmtyzj.sHtML

[T30] Swift：协议
来源：http://mobile.fanxiaobao.xyz/Article/details/gbogaipso.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fanxiaobao.xyz/Article/details/giatzohsk.sHtML

[T31] Lua：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gmadksbph.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gwrxeksxk.sHtML

[T32] Lua：局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gcpxbdyfu.sHtML

local a = 1
来源：http://www.share.fanxiaobao.xyz/Article/details/glseseczs.sHtML

[T33] Lua：表（数组）
来源：http://blog.fanxiaobao.xyz/Article/details/giynmders.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.fanxiaobao.xyz/Article/details/gpkjhqpjy.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gabmmrzvk.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fanxiaobao.xyz/Article/details/gyatpdpgb.sHtML

[T35] Lua：字典表
来源：http://wap.fanxiaobao.xyz/Article/details/gawoavpqc.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gmiwsxcjr.sHtML

[T36] Lua：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gujbyvpil.sHtML

function add(a, b) return a + b end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdrvsgkxn.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.fanxiaobao.xyz/Article/details/gqosxkkrl.sHtML

"a" .. "b"
来源：http://baike.fanxiaobao.xyz/Article/details/giglfwhhq.sHtML

[T38] Lua：条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gjvxlgxxo.sHtML

if x > 0 then print("正") end
来源：http://baike.fanxiaobao.xyz/Article/details/goxizfuux.sHtML

[T39] Lua：模式匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gfagaszvk.sHtML

string.find(s, "%d+")
来源：http://www.share.fanxiaobao.xyz/Article/details/gmytylkry.sHtML

[T40] Lua：元表
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghdcyoxov.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fanxiaobao.xyz/Article/details/gdsyaeyeg.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbraxglqk.sHtML

print "Hello\n";
来源：http://read.share.fanxiaobao.xyz/Article/details/gambuhtxr.sHtML

[T42] Perl：变量类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gyltbcjxz.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.fanxiaobao.xyz/Article/details/gevccxbyt.sHtML

[T43] Perl：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gwhulatnl.sHtML

"值: $a"
来源：http://baike.fanxiaobao.xyz/Article/details/gijclprtj.sHtML

[T44] Perl：条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gizbirtra.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpkffsjbn.sHtML

[T45] Perl：数组遍历
来源：http://blog.fanxiaobao.xyz/Article/details/goqpginue.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.fanxiaobao.xyz/Article/details/geiqkapsn.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gapsbwcpw.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkhfzsjyu.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqoykwjgf.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gcgrjoeba.sHtML

[T48] Perl：正则替换
来源：http://blog.fanxiaobao.xyz/Article/details/gzcrvenhr.sHtML

$s =~ s/old/new/g;
来源：http://3g.fanxiaobao.xyz/Article/details/gnxrepzsl.sHtML

[T49] Perl：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/goerruxic.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmitajspy.sHtML

[T50] Perl：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gjpoyhtgu.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.fanxiaobao.xyz/Article/details/gctzouayq.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.fanxiaobao.xyz/Article/details/gqmtfydiu.sHtML

[T51] Scala：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gtzipnfxg.sHtML

println("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gmhcicpob.sHtML

[T52] Scala：变量
来源：http://baike.fanxiaobao.xyz/Article/details/guooxgohk.sHtML

val a = 1;  var b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gbmababzi.sHtML

[T53] Scala：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gajxkoahl.sHtML

s"值: $b"
来源：http://baike.fanxiaobao.xyz/Article/details/gwtkeckyo.sHtML

[T54] Scala：集合映射
来源：http://3g.fanxiaobao.xyz/Article/details/gjmygdbez.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gsokcpqvm.sHtML

[T55] Scala：集合过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gvkanfxck.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzwbcdzii.sHtML

[T56] Scala：样例类
来源：http://blog.fanxiaobao.xyz/Article/details/gyenhnvhc.sHtML

case class User(name: String, age: Int)
来源：http://baike.fanxiaobao.xyz/Article/details/grxzojgmw.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gurlypuhw.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.fanxiaobao.xyz/Article/details/gvzopbrwe.sHtML

[T58] Scala：函数定义
来源：http://3g.fanxiaobao.xyz/Article/details/gcnwxqtdl.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.fanxiaobao.xyz/Article/details/guajrtbzl.sHtML

[T59] Scala：循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gsjbexezg.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdfsumavy.sHtML

[T60] Scala：折叠
来源：http://wap.fanxiaobao.xyz/Article/details/grbibkknf.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxcaeoxqp.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/goyntsdrd.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gdzmxarym.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gtryjrolm.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcmdlphbh.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.fanxiaobao.xyz/Article/details/gbshzcwpa.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdghxpagi.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gkfagagdw.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.fanxiaobao.xyz/Article/details/gjqkbszcc.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.fanxiaobao.xyz/Article/details/gddbkgfwg.sHtML

[U04] Py：变量调试打印
来源：http://baike.fanxiaobao.xyz/Article/details/gtmpxdtki.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.fanxiaobao.xyz/Article/details/gcisiqhwq.sHtML

[U05] Py：列表去重且保序
来源：http://3g.fanxiaobao.xyz/Article/details/griqidsjc.sHtML

list(dict.fromkeys(arr))
来源：http://blog.fanxiaobao.xyz/Article/details/gnxgyoeza.sHtML

[U06] Py：合并两个字典
来源：http://m.share.fanxiaobao.xyz/Article/details/gxczayoqf.sHtML

{**a, **b}
来源：http://mobile.fanxiaobao.xyz/Article/details/gbyoiqfva.sHtML

[U07] Py：反转字典键值
来源：http://3g.fanxiaobao.xyz/Article/details/gawxwlmqb.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyoyhwvkt.sHtML

[U08] Py：展平二维列表
来源：http://baike.fanxiaobao.xyz/Article/details/gyomeadum.sHtML

[y for x in nested for y in x]
来源：http://blog.fanxiaobao.xyz/Article/details/gftxisvqi.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.fanxiaobao.xyz/Article/details/gmllinqbx.sHtML

max(d, key=d.get)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwkbmlbyo.sHtML

[U10] Py：按值排序字典
来源：http://m.share.fanxiaobao.xyz/Article/details/gwjpguhej.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.fanxiaobao.xyz/Article/details/gfgrafoin.sHtML

[U11] Py：生成器表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/ggyysfnbi.sHtML

(x * 2 for x in arr)
来源：http://3g.fanxiaobao.xyz/Article/details/grmszofru.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.fanxiaobao.xyz/Article/details/gbzfehkuo.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvqnnermv.sHtML

[U13] Py：固定长度队列
来源：http://wap.fanxiaobao.xyz/Article/details/gjxjihatp.sHtML

deque(maxlen=10)
来源：http://blog.fanxiaobao.xyz/Article/details/grhvgsiwk.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.fanxiaobao.xyz/Article/details/gwumvvoak.sHtML

defaultdict(list)
来源：http://read.share.fanxiaobao.xyz/Article/details/grekigdyc.sHtML

[U15] Py：高精度计时
来源：http://www.share.fanxiaobao.xyz/Article/details/gohiyucii.sHtML

t = time.perf_counter()
来源：http://baike.fanxiaobao.xyz/Article/details/gynhddzkr.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fanxiaobao.xyz/Article/details/gtaswfoiy.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzrlpokrb.sHtML

[U17] Py：初始化日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gqbodzhgd.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpvvjrold.sHtML

[U18] Py：预编译正则
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwhxchdo.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvfkepps.sHtML

[U19] Py：正则替换带回调
来源：http://blog.fanxiaobao.xyz/Article/details/gqdlosihu.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.fanxiaobao.xyz/Article/details/gpnaxubrx.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goykgklgq.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.fanxiaobao.xyz/Article/details/gyorbjqiz.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcgcwyxzt.sHtML

@contextlib.contextmanager
来源：http://read.share.fanxiaobao.xyz/Article/details/gonfjlhxr.sHtML

[U22] Py：矩阵转置
来源：http://blog.fanxiaobao.xyz/Article/details/gdvpgdyyn.sHtML

list(zip(*m))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqnweiffv.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkbzeohtu.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.fanxiaobao.xyz/Article/details/gydekfxep.sHtML

[U24] Py：路径操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gmgworuzc.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.fanxiaobao.xyz/Article/details/gxpyojnqd.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.fanxiaobao.xyz/Article/details/gsubuernb.sHtML

csv.DictReader(f)
来源：http://wap.fanxiaobao.xyz/Article/details/gvcipukve.sHtML

[U26] Py：并发下载
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwnclknao.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.fanxiaobao.xyz/Article/details/gumzniarw.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.fanxiaobao.xyz/Article/details/goqokwaqq.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.fanxiaobao.xyz/Article/details/gnwkdhytp.sHtML

[U28] Py：类型别名
来源：http://m.share.fanxiaobao.xyz/Article/details/gzropycfr.sHtML

UserId = int
来源：http://m.share.fanxiaobao.xyz/Article/details/gdenbahkz.sHtML

[U29] Py：属性校验
来源：http://m.share.fanxiaobao.xyz/Article/details/ggqnalrmq.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwqxvycrz.sHtML

[U30] Py：数据类
来源：http://mobile.fanxiaobao.xyz/Article/details/gnjoxdoor.sHtML

@dataclass(slots=True)
来源：http://blog.fanxiaobao.xyz/Article/details/gteqrzksn.sHtML

[U31] Py：单测
来源：http://mobile.fanxiaobao.xyz/Article/details/gdbdhffpk.sHtML

python -m pytest -q
来源：http://wap.fanxiaobao.xyz/Article/details/gotkmdwbg.sHtML

[U32] Py：代码格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwoyawof.sHtML

ruff format . && ruff check --fix .
来源：http://baike.fanxiaobao.xyz/Article/details/gfnvahyah.sHtML

[U33] Py：打包发布
来源：http://3g.fanxiaobao.xyz/Article/details/gpmwjacih.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxhjilqlb.sHtML

[U34] Py：判断编码
来源：http://baike.fanxiaobao.xyz/Article/details/gfquzfmta.sHtML

chardet.detect(raw)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvshkhkuv.sHtML

[U35] Py：发送邮件
来源：http://baike.fanxiaobao.xyz/Article/details/gvojyyxci.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.fanxiaobao.xyz/Article/details/gsbnahikm.sHtML

[U36] Py：定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/ghawbglud.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbzefuhgx.sHtML

[U37] Py：读写 Excel
来源：http://baike.fanxiaobao.xyz/Article/details/gvuswfxnr.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.fanxiaobao.xyz/Article/details/ggtyxohkw.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fanxiaobao.xyz/Article/details/gfljighns.sHtML

Path(__file__).resolve().parent
来源：http://blog.fanxiaobao.xyz/Article/details/grvqjkyzi.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmothlqov.sHtML

sys.stdout.isatty()
来源：http://m.share.fanxiaobao.xyz/Article/details/glsuwkzhf.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gezsuophc.sHtML

print("err", file=sys.stderr)
来源：http://baike.fanxiaobao.xyz/Article/details/gwllbndxk.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggybnhxls.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.fanxiaobao.xyz/Article/details/gwnypcdxo.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.fanxiaobao.xyz/Article/details/gychbywwy.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkuzdeomy.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gydjnozvu.sHtML

namespace App\Http;
来源：http://3g.fanxiaobao.xyz/Article/details/gfjvrtfbz.sHtML

[U44] PHP：开启严格类型
来源：http://3g.fanxiaobao.xyz/Article/details/giymxtgyg.sHtML

declare(strict_types=1);
来源：http://3g.fanxiaobao.xyz/Article/details/gqxgjlmkw.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gjajxrdgn.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gjheqcibt.sHtML

[U46] PHP：可空类型
来源：http://blog.fanxiaobao.xyz/Article/details/gzcyghoji.sHtML

?string $name = null
来源：http://m.share.fanxiaobao.xyz/Article/details/gfhvahzui.sHtML

[U47] PHP：联合类型
来源：http://wap.fanxiaobao.xyz/Article/details/ggsegafaq.sHtML

int|string $id
来源：http://www.share.fanxiaobao.xyz/Article/details/gnnysrqyy.sHtML

[U48] PHP：纯枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gnbewnmfg.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtjrdrupg.sHtML

[U49] PHP：只读属性
来源：http://mobile.fanxiaobao.xyz/Article/details/gnferpbev.sHtML

public readonly string $name
来源：http://m.share.fanxiaobao.xyz/Article/details/gfcjltdfg.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.fanxiaobao.xyz/Article/details/gqtjkaxzk.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnqpkklvb.sHtML

[U51] PHP：数组解构
来源：http://baike.fanxiaobao.xyz/Article/details/gnxpwpizy.sHtML

[$a, $b] = $arr;
来源：http://blog.fanxiaobao.xyz/Article/details/gtvagkaxv.sHtML

[U52] PHP：箭头函数
来源：http://wap.fanxiaobao.xyz/Article/details/gorxwjtmv.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.fanxiaobao.xyz/Article/details/gwxcwscqt.sHtML

[U53] PHP：空合并运算符
来源：http://wap.fanxiaobao.xyz/Article/details/gcofegpjw.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/genwbfnlm.sHtML

[U54] PHP：空安全调用
来源：http://3g.fanxiaobao.xyz/Article/details/gnmtvettk.sHtML

$obj?->method()
来源：http://www.share.fanxiaobao.xyz/Article/details/gienweffj.sHtML

[U55] PHP：match 表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gwamanfua.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.fanxiaobao.xyz/Article/details/gzaxxorzk.sHtML

[U56] PHP：命名参数
来源：http://m.share.fanxiaobao.xyz/Article/details/ghxoxuwdb.sHtML

f(a: 1, b: 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggivldqww.sHtML

[U57] PHP：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gyfemppxn.sHtML

"值: {$a}"
来源：http://3g.fanxiaobao.xyz/Article/details/gedcqrhyu.sHtML

[U58] PHP：数组三件套
来源：http://baike.fanxiaobao.xyz/Article/details/gofwukrhq.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.fanxiaobao.xyz/Article/details/gpzbdsfeg.sHtML

[U59] PHP：自定义排序
来源：http://wap.fanxiaobao.xyz/Article/details/ghuhqrsle.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fanxiaobao.xyz/Article/details/gyctzuxcp.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.fanxiaobao.xyz/Article/details/gprqysuev.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.fanxiaobao.xyz/Article/details/gduidzseg.sHtML

[U61] PHP：正则
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gktritisx.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.fanxiaobao.xyz/Article/details/gjsvibcgr.sHtML

[U62] PHP：日期对象
来源：http://www.share.fanxiaobao.xyz/Article/details/gmicsdhnn.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.fanxiaobao.xyz/Article/details/gzcqtfbwr.sHtML

[U63] PHP：文件读写
来源：http://3g.fanxiaobao.xyz/Article/details/gyqddhrwn.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaxiwjwsg.sHtML

[U64] PHP：目录遍历
来源：http://wap.fanxiaobao.xyz/Article/details/ghfqkjtbb.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.fanxiaobao.xyz/Article/details/gkemslryw.sHtML

[U65] PHP：会话
来源：http://3g.fanxiaobao.xyz/Article/details/gksiaguxv.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gyvirhbcb.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.fanxiaobao.xyz/Article/details/gefhvxikl.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gnfscjcxp.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.fanxiaobao.xyz/Article/details/gsskmidto.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.fanxiaobao.xyz/Article/details/ggtgnjyqd.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gumcnwmmf.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.fanxiaobao.xyz/Article/details/glauhulaj.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.fanxiaobao.xyz/Article/details/grtlzhqhy.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.fanxiaobao.xyz/Article/details/gdtcsicsp.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gnybaqowp.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.fanxiaobao.xyz/Article/details/gcahbeqax.sHtML

[U71] PHP：抛出异常
来源：http://blog.fanxiaobao.xyz/Article/details/gcfblwitw.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.fanxiaobao.xyz/Article/details/gacpdpttl.sHtML

[U72] PHP：写错误日志
来源：http://wap.fanxiaobao.xyz/Article/details/gxhldzjpk.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsoygrphm.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghpzqbkww.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.fanxiaobao.xyz/Article/details/gkbjcrenh.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gkqwpiqyi.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.fanxiaobao.xyz/Article/details/girfijzbf.sHtML

[U75] PHP：依赖注入
来源：http://3g.fanxiaobao.xyz/Article/details/gbxeniycr.sHtML

composer require psr/container
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjgvnnrvv.sHtML

[U76] PHP：简单路由
来源：http://read.share.fanxiaobao.xyz/Article/details/gaicjigfw.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.fanxiaobao.xyz/Article/details/ghsxntjgj.sHtML

[U77] PHP：模板渲染
来源：http://read.share.fanxiaobao.xyz/Article/details/gvhgbtmzl.sHtML

composer require twig/twig
来源：http://www.share.fanxiaobao.xyz/Article/details/grrcyvjhj.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmkstnidx.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.fanxiaobao.xyz/Article/details/gixsstwbs.sHtML

[U79] PHP：静态分析
来源：http://wap.fanxiaobao.xyz/Article/details/genirkylz.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.fanxiaobao.xyz/Article/details/gzqmuqpgs.sHtML

[U80] PHP：代码规范修复
来源：http://wap.fanxiaobao.xyz/Article/details/glmyoshjm.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.fanxiaobao.xyz/Article/details/gbvyvrotq.sHtML


<!-- 参考信息 -->