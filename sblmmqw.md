代发 wailian999

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fehbvm.com/Article/details/gnfgojtyj.sHtML

[S51] C++：显式类型转换
来源：http://mobile.hesvh.cn/Article/details/gajmqrhjl.sHtML

static_cast<double>(a) / b
来源：http://read.share.hesvh.cn/Article/details/gscvgahpg.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.zdbjq.cn/Article/details/gfozravhr.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.hesvh.cn/Article/details/goopmvyki.sHtML

[S53] C++：移动语义
来源：http://mobile.fehbvm.com/Article/details/ghgjtrtzk.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.zdbjq.cn/Article/details/ghualvqft.sHtML

[S54] C++：异常处理
来源：http://www.share.zdbjq.cn/Article/details/gqrsuwsfw.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.hesvh.cn/Article/details/gvytrapsd.sHtML

[S55] C++：结构化绑定
来源：http://read.share.hesvh.cn/Article/details/gpifnuspz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.zdbjq.cn/Article/details/gkbzsxeqa.sHtML

[S56] C++：optional
来源：http://3g.zdbjq.cn/Article/details/gfvlpndjv.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.hesvh.cn/Article/details/gbjalwzcr.sHtML

[S57] C++：编译期常量
来源：http://www.blog.hesvh.cn/Article/details/gmsvqtgvz.sHtML

constexpr int N = 10;
来源：http://read.share.fehbvm.com/Article/details/gpugpjlff.sHtML

[S58] C++：命名空间
来源：http://3g.zdbjq.cn/Article/details/gltjlehod.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.zdbjq.cn/Article/details/gukjfjgyf.sHtML

[S59] C++：静态断言
来源：http://www.blog.zdbjq.cn/Article/details/gurkoswlb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.hesvh.cn/Article/details/gnhicmyus.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fehbvm.com/Article/details/gvwcgpamm.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.hesvh.cn/Article/details/grjxasdju.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/geqzsvsjp.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.hesvh.cn/Article/details/gcpqgkdxr.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gdpsjfpan.sHtML

[T01] Kotlin：Hello World
来源：http://baike.hesvh.cn/Article/details/gvmjrvvzc.sHtML

println("Hello")
来源：http://wap.hesvh.cn/Article/details/gnybkjlci.sHtML

[T02] Kotlin：变量
来源：http://wap.zdbjq.cn/Article/details/gmazpcfta.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.hesvh.cn/Article/details/gnldndwkw.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.hesvh.cn/Article/details/gmymjfvlz.sHtML

"值: $b"
来源：http://www.m.share.fehbvm.com/Article/details/gbflwddkr.sHtML

[T04] Kotlin：空安全
来源：http://mobile.zdbjq.cn/Article/details/gfotgqvfy.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.zdbjq.cn/Article/details/gocvnvigo.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.hesvh.cn/Article/details/goihedezh.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.hesvh.cn/Article/details/gfoqryvqe.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fehbvm.com/Article/details/galyishyl.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.hesvh.cn/Article/details/gfqztvlit.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.hesvh.cn/Article/details/gnynxxzgo.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/gfrhcannc.sHtML

[T08] Kotlin：数据类
来源：http://3g.zdbjq.cn/Article/details/gpwrokmza.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.hesvh.cn/Article/details/guyfqnmhj.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.zdbjq.cn/Article/details/gzmhgdszd.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fehbvm.com/Article/details/giwxvxyim.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fehbvm.com/Article/details/ghecfpcae.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fehbvm.com/Article/details/gptghqbtp.sHtML

[T11] Kotlin：协程
来源：http://www.blog.hesvh.cn/Article/details/glknnxkbb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.hesvh.cn/Article/details/gvgppfyle.sHtML

[T12] Kotlin：解构声明
来源：http://baike.zdbjq.cn/Article/details/gxoyutknv.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fehbvm.com/Article/details/gypwmxfxz.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.fehbvm.com/Article/details/gkdcunwic.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.zdbjq.cn/Article/details/gampoqurg.sHtML

[T14] Kotlin：循环
来源：http://baike.zdbjq.cn/Article/details/gpxvnvjnt.sHtML

for (i in 1..10) println(i)
来源：http://read.share.zdbjq.cn/Article/details/guasnapow.sHtML

[T15] Kotlin：接口
来源：http://baike.fehbvm.com/Article/details/gyfnfvlza.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.zdbjq.cn/Article/details/grlxfvucy.sHtML

[T16] Swift：Hello World
来源：http://m.share.hesvh.cn/Article/details/gwreoaogz.sHtML

print("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gwcogrhtx.sHtML

[T17] Swift：变量与常量
来源：http://read.share.hesvh.cn/Article/details/gjcrjfrjh.sHtML

var a = 1;  let b = 2
来源：http://blog.fehbvm.com/Article/details/gyfvhjjub.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gdbakdsyy.sHtML

"值: \(b)"
来源：http://blog.hesvh.cn/Article/details/gxlpoaqbd.sHtML

[T19] Swift：可选绑定
来源：http://baike.hesvh.cn/Article/details/gwjgnhkit.sHtML

if let n = opt { print(n) }
来源：http://www.blog.zdbjq.cn/Article/details/gjaoshcoe.sHtML

[T20] Swift：数组操作
来源：http://blog.hesvh.cn/Article/details/gmxyssmgw.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.hesvh.cn/Article/details/ghzcwwzyq.sHtML

[T21] Swift：遍历
来源：http://baike.fehbvm.com/Article/details/gdywufvbh.sHtML

for x in a { print(x) }
来源：http://wap.zdbjq.cn/Article/details/gdopgujkv.sHtML

[T22] Swift：字典
来源：http://m.share.hesvh.cn/Article/details/ghxtfhkxy.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.fehbvm.com/Article/details/groosksoz.sHtML

[T23] Swift：函数
来源：http://read.share.hesvh.cn/Article/details/glxfvvcgv.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fehbvm.com/Article/details/gjbbkbhwi.sHtML

[T24] Swift：闭包
来源：http://3g.zdbjq.cn/Article/details/gvhzukogz.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fehbvm.com/Article/details/ghwarsbuq.sHtML

[T25] Swift：结构体
来源：http://www.share.zdbjq.cn/Article/details/gzsvahwql.sHtML

struct P { var x: Int }
来源：http://read.share.fehbvm.com/Article/details/gctwsacse.sHtML

[T26] Swift：类与重写
来源：http://www.share.zdbjq.cn/Article/details/gdjgmltas.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.hesvh.cn/Article/details/gbtgkeinc.sHtML

[T27] Swift：错误处理
来源：http://mobile.fehbvm.com/Article/details/gzzedsgkf.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.hesvh.cn/Article/details/gijliybug.sHtML

[T28] Swift：枚举
来源：http://www.share.hesvh.cn/Article/details/gsijijpxv.sHtML

enum Color { case red, green }
来源：http://read.share.fehbvm.com/Article/details/gjxxwibax.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.hesvh.cn/Article/details/gufxoxubf.sHtML

guard let x = opt else { return }
来源：http://m.share.hesvh.cn/Article/details/gedpsapop.sHtML

[T30] Swift：协议
来源：http://baike.zdbjq.cn/Article/details/gahabdkkq.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.zdbjq.cn/Article/details/gwqbkiyad.sHtML

[T31] Lua：Hello World
来源：http://read.share.hesvh.cn/Article/details/groarelgl.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/gqywsjgdn.sHtML

[T32] Lua：局部变量
来源：http://read.share.hesvh.cn/Article/details/gkwnxzwhi.sHtML

local a = 1
来源：http://read.share.zdbjq.cn/Article/details/gxjqbjnso.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.zdbjq.cn/Article/details/geyburckv.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.fehbvm.com/Article/details/gnqlkwnyi.sHtML

[T34] Lua：遍历表
来源：http://m.share.hesvh.cn/Article/details/gilgmqmwq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fehbvm.com/Article/details/ginbybbdi.sHtML

[T35] Lua：字典表
来源：http://3g.zdbjq.cn/Article/details/gdtosvzyj.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gpoekkqza.sHtML

[T36] Lua：函数
来源：http://baike.hesvh.cn/Article/details/gkzfbstfe.sHtML

function add(a, b) return a + b end
来源：http://read.share.zdbjq.cn/Article/details/gvjszxfvx.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.hesvh.cn/Article/details/gleaxpcal.sHtML

"a" .. "b"
来源：http://www.m.share.fehbvm.com/Article/details/gibomcgtc.sHtML

[T38] Lua：条件
来源：http://www.m.share.zdbjq.cn/Article/details/gtnyjxiue.sHtML

if x > 0 then print("正") end
来源：http://mobile.hesvh.cn/Article/details/gsfaugrqg.sHtML

[T39] Lua：模式匹配
来源：http://m.share.hesvh.cn/Article/details/gtbqxreoe.sHtML

string.find(s, "%d+")
来源：http://baike.fehbvm.com/Article/details/gbbwyzeyn.sHtML

[T40] Lua：元表
来源：http://baike.hesvh.cn/Article/details/gkkusjqyw.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.zdbjq.cn/Article/details/gmhhrppqm.sHtML

[T41] Perl：Hello World
来源：http://read.share.fehbvm.com/Article/details/gfveyhxuz.sHtML

print "Hello\n";
来源：http://3g.fehbvm.com/Article/details/grekdqmka.sHtML

[T42] Perl：变量类型
来源：http://mobile.fehbvm.com/Article/details/gtogkxrha.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.hesvh.cn/Article/details/guwwjxgzj.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gtwarjisi.sHtML

"值: $a"
来源：http://wap.hesvh.cn/Article/details/gzrfouzok.sHtML

[T44] Perl：条件
来源：http://m.share.fehbvm.com/Article/details/gadriqmfg.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.zdbjq.cn/Article/details/gbjulixyt.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.hesvh.cn/Article/details/gageqasks.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.zdbjq.cn/Article/details/gukffvvdm.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.hesvh.cn/Article/details/gynkpbcmw.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.zdbjq.cn/Article/details/gmkiobpnn.sHtML

[T47] Perl：正则捕获
来源：http://mobile.zdbjq.cn/Article/details/gbjutotvm.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.zdbjq.cn/Article/details/grouvyngh.sHtML

[T48] Perl：正则替换
来源：http://wap.fehbvm.com/Article/details/gzbctypen.sHtML

$s =~ s/old/new/g;
来源：http://mobile.hesvh.cn/Article/details/gcldnlngk.sHtML

[T49] Perl：函数
来源：http://3g.hesvh.cn/Article/details/gcmjlmhze.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/gdelplriu.sHtML

[T50] Perl：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gdlaivpni.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.zdbjq.cn/Article/details/gyahimaol.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.hesvh.cn/Article/details/gzmtsjsub.sHtML

[T51] Scala：Hello World
来源：http://m.share.fehbvm.com/Article/details/gboyrxlkh.sHtML

println("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gkaywyort.sHtML

[T52] Scala：变量
来源：http://www.share.hesvh.cn/Article/details/gxclcpyqu.sHtML

val a = 1;  var b = 2
来源：http://mobile.zdbjq.cn/Article/details/gqytueepn.sHtML

[T53] Scala：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gtlfsjhsy.sHtML

s"值: $b"
来源：http://m.share.zdbjq.cn/Article/details/gfgkegrvt.sHtML

[T54] Scala：集合映射
来源：http://mobile.zdbjq.cn/Article/details/ggrcpicsq.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.fehbvm.com/Article/details/gcyfkahha.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.fehbvm.com/Article/details/gqwvuvtdz.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.hesvh.cn/Article/details/ghyqzqkte.sHtML

[T56] Scala：样例类
来源：http://www.blog.fehbvm.com/Article/details/gaxauvfvy.sHtML

case class User(name: String, age: Int)
来源：http://www.share.zdbjq.cn/Article/details/gueqkvzgr.sHtML

[T57] Scala：模式匹配
来源：http://mobile.zdbjq.cn/Article/details/gptpkitaz.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.hesvh.cn/Article/details/galaljekp.sHtML

[T58] Scala：函数定义
来源：http://blog.fehbvm.com/Article/details/gkdyagkhk.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.zdbjq.cn/Article/details/gwxqjtmap.sHtML

[T59] Scala：循环
来源：http://wap.fehbvm.com/Article/details/gpvqvtskb.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.fehbvm.com/Article/details/gmdzwljdo.sHtML

[T60] Scala：折叠
来源：http://read.share.fehbvm.com/Article/details/gxyzrtvqw.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.zdbjq.cn/Article/details/gefiqqiyq.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/glztxbmqa.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fehbvm.com/Article/details/gsicdwktf.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gxbsewqxb.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.hesvh.cn/Article/details/gsnnedgig.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.fehbvm.com/Article/details/ginzlhpnk.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.fehbvm.com/Article/details/ggqaasqpn.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.hesvh.cn/Article/details/gvhpastuo.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.hesvh.cn/Article/details/gycgmipvv.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.hesvh.cn/Article/details/guowxstyb.sHtML

[U04] Py：变量调试打印
来源：http://mobile.fehbvm.com/Article/details/gmjznzopy.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.fehbvm.com/Article/details/gfujxhbvy.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.fehbvm.com/Article/details/ghkukulfx.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.zdbjq.cn/Article/details/gwafavipl.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.zdbjq.cn/Article/details/gfshlhbel.sHtML

{**a, **b}
来源：http://read.share.fehbvm.com/Article/details/gjhbeogib.sHtML

[U07] Py：反转字典键值
来源：http://www.share.fehbvm.com/Article/details/ggpiovivm.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.fehbvm.com/Article/details/gtntvmuqi.sHtML

[U08] Py：展平二维列表
来源：http://www.share.hesvh.cn/Article/details/gybfeiugc.sHtML

[y for x in nested for y in x]
来源：http://baike.hesvh.cn/Article/details/gwhrahfhv.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.zdbjq.cn/Article/details/gpwuqrewc.sHtML

max(d, key=d.get)
来源：http://read.share.hesvh.cn/Article/details/gtcaugfft.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.fehbvm.com/Article/details/goodbkctl.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.fehbvm.com/Article/details/gqmizuepu.sHtML

[U11] Py：生成器表达式
来源：http://m.share.zdbjq.cn/Article/details/gzwkzvdoh.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.fehbvm.com/Article/details/gxpkxupbi.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.fehbvm.com/Article/details/gvkzvhzme.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gerfraofa.sHtML

[U13] Py：固定长度队列
来源：http://3g.zdbjq.cn/Article/details/gwjvhhbfa.sHtML

deque(maxlen=10)
来源：http://wap.fehbvm.com/Article/details/gmoonkasa.sHtML

[U14] Py：分组收集到列表
来源：http://wap.fehbvm.com/Article/details/gdqmsxbca.sHtML

defaultdict(list)
来源：http://3g.hesvh.cn/Article/details/gggsnkyly.sHtML

[U15] Py：高精度计时
来源：http://mobile.hesvh.cn/Article/details/gziplfjmn.sHtML

t = time.perf_counter()
来源：http://wap.hesvh.cn/Article/details/gxtvmilym.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.fehbvm.com/Article/details/gcgjwntts.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.hesvh.cn/Article/details/gdashnael.sHtML

[U17] Py：初始化日志
来源：http://read.share.fehbvm.com/Article/details/grypzvtkq.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.hesvh.cn/Article/details/gnxfczozu.sHtML

[U18] Py：预编译正则
来源：http://m.share.hesvh.cn/Article/details/gibarggwr.sHtML

pat = re.compile(r"\d+")
来源：http://wap.hesvh.cn/Article/details/gllrgluey.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.zdbjq.cn/Article/details/gyfkfanun.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.fehbvm.com/Article/details/gcbmugonl.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.zdbjq.cn/Article/details/gxmcblceg.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.hesvh.cn/Article/details/gprxznhqi.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.zdbjq.cn/Article/details/gsgaqwbby.sHtML

@contextlib.contextmanager
来源：http://read.share.fehbvm.com/Article/details/gjxetysse.sHtML

[U22] Py：矩阵转置
来源：http://wap.hesvh.cn/Article/details/galauzoai.sHtML

list(zip(*m))
来源：http://www.share.zdbjq.cn/Article/details/goeoxtotv.sHtML

[U23] Py：分块读取大文件
来源：http://3g.fehbvm.com/Article/details/gmblarfyn.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.hesvh.cn/Article/details/gqwskstke.sHtML

[U24] Py：路径操作
来源：http://blog.fehbvm.com/Article/details/gqzyusllc.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gririvaip.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.fehbvm.com/Article/details/gbosgyoiq.sHtML

csv.DictReader(f)
来源：http://www.m.share.zdbjq.cn/Article/details/gsjempcdb.sHtML

[U26] Py：并发下载
来源：http://wap.fehbvm.com/Article/details/glttkjkyg.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.fehbvm.com/Article/details/gshzmkpco.sHtML

[U27] Py：异步 HTTP
来源：http://wap.fehbvm.com/Article/details/gvgkhxynm.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.hesvh.cn/Article/details/gborrylnl.sHtML

[U28] Py：类型别名
来源：http://wap.fehbvm.com/Article/details/gqnuxvtew.sHtML

UserId = int
来源：http://www.share.fehbvm.com/Article/details/gpqqejhzm.sHtML

[U29] Py：属性校验
来源：http://m.share.hesvh.cn/Article/details/gqimekpsa.sHtML

@property 与 @x.setter 配合
来源：http://wap.zdbjq.cn/Article/details/gvrmkhqbp.sHtML

[U30] Py：数据类
来源：http://mobile.zdbjq.cn/Article/details/ggrwyudjg.sHtML

@dataclass(slots=True)
来源：http://blog.zdbjq.cn/Article/details/glrldadhz.sHtML

[U31] Py：单测
来源：http://www.m.share.hesvh.cn/Article/details/gzsmvimaj.sHtML

python -m pytest -q
来源：http://wap.zdbjq.cn/Article/details/gnptmdeep.sHtML

[U32] Py：代码格式化
来源：http://blog.hesvh.cn/Article/details/gyuzquagr.sHtML

ruff format . && ruff check --fix .
来源：http://baike.fehbvm.com/Article/details/gxthfoodt.sHtML

[U33] Py：打包发布
来源：http://mobile.fehbvm.com/Article/details/gsteaqyxf.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.zdbjq.cn/Article/details/ggjymouls.sHtML

[U34] Py：判断编码
来源：http://www.m.share.zdbjq.cn/Article/details/ggwwikwpe.sHtML

chardet.detect(raw)
来源：http://mobile.zdbjq.cn/Article/details/gpjhnmdlf.sHtML

[U35] Py：发送邮件
来源：http://3g.zdbjq.cn/Article/details/gnzausyjc.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.fehbvm.com/Article/details/gdkvybtbd.sHtML

[U36] Py：定时任务
来源：http://baike.hesvh.cn/Article/details/gonscflbr.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.fehbvm.com/Article/details/gmfqfszal.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.hesvh.cn/Article/details/gdslzjbwi.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.hesvh.cn/Article/details/gotnzdjbv.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.hesvh.cn/Article/details/ggrfigsjj.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.zdbjq.cn/Article/details/gkesgyolw.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.hesvh.cn/Article/details/ghizsshrd.sHtML

sys.stdout.isatty()
来源：http://baike.fehbvm.com/Article/details/gvwvdxdfs.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.hesvh.cn/Article/details/gvovannud.sHtML

print("err", file=sys.stderr)
来源：http://m.share.hesvh.cn/Article/details/gjquiuuoh.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.zdbjq.cn/Article/details/gmkngssyu.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.hesvh.cn/Article/details/gaxuvepby.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.fehbvm.com/Article/details/gbvntophp.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.fehbvm.com/Article/details/geaggjcsv.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.hesvh.cn/Article/details/gnkdqvrry.sHtML

namespace App\Http;
来源：http://mobile.fehbvm.com/Article/details/glidwnkon.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.fehbvm.com/Article/details/gqvpsbjiq.sHtML

declare(strict_types=1);
来源：http://mobile.zdbjq.cn/Article/details/gmyakzyte.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.fehbvm.com/Article/details/gdqachmwf.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gghjareee.sHtML

[U46] PHP：可空类型
来源：http://wap.hesvh.cn/Article/details/gtwhyckjh.sHtML

?string $name = null
来源：http://m.share.fehbvm.com/Article/details/gqgrbxyjo.sHtML

[U47] PHP：联合类型
来源：http://www.share.fehbvm.com/Article/details/gwywkwewk.sHtML

int|string $id
来源：http://wap.fehbvm.com/Article/details/gvowglzdw.sHtML

[U48] PHP：纯枚举
来源：http://mobile.hesvh.cn/Article/details/gfjkynnie.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.hesvh.cn/Article/details/goyrhobhm.sHtML

[U49] PHP：只读属性
来源：http://read.share.hesvh.cn/Article/details/guyegyygu.sHtML

public readonly string $name
来源：http://baike.fehbvm.com/Article/details/gtprjuhde.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.hesvh.cn/Article/details/gligswyqt.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.fehbvm.com/Article/details/gjnltreeh.sHtML

[U51] PHP：数组解构
来源：http://read.share.zdbjq.cn/Article/details/gmgnxxjay.sHtML

[$a, $b] = $arr;
来源：http://blog.fehbvm.com/Article/details/gjfydhrrh.sHtML

[U52] PHP：箭头函数
来源：http://wap.zdbjq.cn/Article/details/gguhcuoze.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.fehbvm.com/Article/details/gwnbjscxo.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.fehbvm.com/Article/details/gmgerawrk.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.fehbvm.com/Article/details/gdqimxgrc.sHtML

[U54] PHP：空安全调用
来源：http://wap.zdbjq.cn/Article/details/gcuiwwqtj.sHtML

$obj?->method()
来源：http://wap.hesvh.cn/Article/details/givkgazlv.sHtML

[U55] PHP：match 表达式
来源：http://wap.hesvh.cn/Article/details/gjvdoigvx.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.zdbjq.cn/Article/details/gdantbwsb.sHtML

[U56] PHP：命名参数
来源：http://baike.fehbvm.com/Article/details/gvgspqwkn.sHtML

f(a: 1, b: 2)
来源：http://wap.hesvh.cn/Article/details/genkkoyti.sHtML

[U57] PHP：字符串插值
来源：http://wap.hesvh.cn/Article/details/gusipsdma.sHtML

"值: {$a}"
来源：http://blog.zdbjq.cn/Article/details/gqrdhqfwg.sHtML

[U58] PHP：数组三件套
来源：http://www.share.hesvh.cn/Article/details/gtsxejcit.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.hesvh.cn/Article/details/gyngxcoxl.sHtML

[U59] PHP：自定义排序
来源：http://mobile.hesvh.cn/Article/details/gjbczglkb.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.zdbjq.cn/Article/details/gzybvfloe.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.hesvh.cn/Article/details/gxcyxwfbs.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.hesvh.cn/Article/details/gzkrpcvtf.sHtML

[U61] PHP：正则
来源：http://wap.fehbvm.com/Article/details/gjerapzos.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fehbvm.com/Article/details/gzrqbfquh.sHtML

[U62] PHP：日期对象
来源：http://www.blog.zdbjq.cn/Article/details/gxwquwqst.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.hesvh.cn/Article/details/gtxgpptka.sHtML

[U63] PHP：文件读写
来源：http://www.share.zdbjq.cn/Article/details/grbpnymhz.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.fehbvm.com/Article/details/gpwcpokmw.sHtML

[U64] PHP：目录遍历
来源：http://wap.zdbjq.cn/Article/details/gemstnwnh.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.zdbjq.cn/Article/details/gvwoaqkpm.sHtML

[U65] PHP：会话
来源：http://baike.hesvh.cn/Article/details/gkdgxwxjp.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.fehbvm.com/Article/details/gkkntauhw.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.zdbjq.cn/Article/details/gklacuenw.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.fehbvm.com/Article/details/gwheegclb.sHtML

[U67] PHP：处理文件上传
来源：http://wap.fehbvm.com/Article/details/gezjnkhnq.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.fehbvm.com/Article/details/glqfqlnon.sHtML

[U68] PHP：PDO 连接
来源：http://wap.fehbvm.com/Article/details/gpiwgcbcc.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.zdbjq.cn/Article/details/gfgyzkpoz.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.hesvh.cn/Article/details/gcweleceh.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.fehbvm.com/Article/details/ggiajjhgn.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.hesvh.cn/Article/details/ggzuitxjn.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.hesvh.cn/Article/details/gotujvqpt.sHtML

[U71] PHP：抛出异常
来源：http://baike.fehbvm.com/Article/details/gzrawruib.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.fehbvm.com/Article/details/gnavahwln.sHtML

[U72] PHP：写错误日志
来源：http://blog.fehbvm.com/Article/details/gqzmzcjgl.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.hesvh.cn/Article/details/gucqcrsgp.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.fehbvm.com/Article/details/gfgvajxum.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.fehbvm.com/Article/details/gfpwhsmhb.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gjdpwcnsj.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.fehbvm.com/Article/details/gsfeienfs.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.hesvh.cn/Article/details/gqzdwzmcr.sHtML

composer require psr/container
来源：http://read.share.fehbvm.com/Article/details/glqgqckqi.sHtML

[U76] PHP：简单路由
来源：http://www.blog.zdbjq.cn/Article/details/gnymypyxf.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.zdbjq.cn/Article/details/ggausbppz.sHtML


<!-- 参考信息 -->