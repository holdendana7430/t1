代发 wailian999

while (std::getline(in, line)) { }
来源：http://wap.fehbvm.com/Article/details/ggleclqqv.sHtML

[S49] C++：写文件
来源：http://www.share.fehbvm.com/Article/details/gdzmovsld.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.hesvh.cn/Article/details/gfkkkypos.sHtML

[S50] C++：格式化数字
来源：http://blog.fehbvm.com/Article/details/gxjjottho.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gntocswsk.sHtML

[S51] C++：显式类型转换
来源：http://baike.hesvh.cn/Article/details/gmzinhcxp.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.hesvh.cn/Article/details/gdwaophzo.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.zdbjq.cn/Article/details/gosmllowz.sHtML

int size() const noexcept { return n_; }
来源：http://blog.zdbjq.cn/Article/details/gzxkvwwvw.sHtML

[S53] C++：移动语义
来源：http://3g.fehbvm.com/Article/details/ggrpavrkh.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fehbvm.com/Article/details/gpczwaenn.sHtML

[S54] C++：异常处理
来源：http://www.m.share.zdbjq.cn/Article/details/gxckztssq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.hesvh.cn/Article/details/gpapuqatj.sHtML

[S55] C++：结构化绑定
来源：http://baike.hesvh.cn/Article/details/gxglgmzti.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.hesvh.cn/Article/details/grohusjca.sHtML

[S56] C++：optional
来源：http://www.blog.fehbvm.com/Article/details/ggnkwjbfj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.zdbjq.cn/Article/details/gjzginbmn.sHtML

[S57] C++：编译期常量
来源：http://wap.zdbjq.cn/Article/details/ggjwusisn.sHtML

constexpr int N = 10;
来源：http://blog.zdbjq.cn/Article/details/gpuwqgsxj.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fehbvm.com/Article/details/gspvyjyxs.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.hesvh.cn/Article/details/gtozczpns.sHtML

[S59] C++：静态断言
来源：http://blog.fehbvm.com/Article/details/glorswlrm.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.hesvh.cn/Article/details/gomcenejq.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fehbvm.com/Article/details/gdglpluay.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fehbvm.com/Article/details/gkxearzyk.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gyvxthalj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.hesvh.cn/Article/details/gpmthxtol.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gzhkyztxn.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fehbvm.com/Article/details/gxjjgethm.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/ghqreeedw.sHtML

[T02] Kotlin：变量
来源：http://wap.fehbvm.com/Article/details/gmnuveylw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.hesvh.cn/Article/details/gtqquxfdq.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.zdbjq.cn/Article/details/glgwpciwh.sHtML

"值: $b"
来源：http://www.share.fehbvm.com/Article/details/gdzcpsjcq.sHtML

[T04] Kotlin：空安全
来源：http://3g.hesvh.cn/Article/details/gmlzxidqu.sHtML

val n: String? = null;  n?.length
来源：http://www.share.zdbjq.cn/Article/details/gospwrbwc.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.hesvh.cn/Article/details/gjduqjpce.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.zdbjq.cn/Article/details/geuuftsmj.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/gpufaleyy.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fehbvm.com/Article/details/ggeqvcsah.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fehbvm.com/Article/details/gdymyoyso.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fehbvm.com/Article/details/gzxxktqlr.sHtML

[T08] Kotlin：数据类
来源：http://3g.hesvh.cn/Article/details/gcinglysk.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.hesvh.cn/Article/details/gebuhmsht.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fehbvm.com/Article/details/getwgfnwt.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.zdbjq.cn/Article/details/glkxezsrq.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fehbvm.com/Article/details/gmugkttam.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fehbvm.com/Article/details/gzrjpuiic.sHtML

[T11] Kotlin：协程
来源：http://www.blog.zdbjq.cn/Article/details/gfawfzlks.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fehbvm.com/Article/details/gzdymmxwm.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fehbvm.com/Article/details/gwvvjldha.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.hesvh.cn/Article/details/gstuhqhhf.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.zdbjq.cn/Article/details/gmckxjzhj.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.hesvh.cn/Article/details/gfhuhkirt.sHtML

[T14] Kotlin：循环
来源：http://www.share.fehbvm.com/Article/details/gqkxewfer.sHtML

for (i in 1..10) println(i)
来源：http://wap.zdbjq.cn/Article/details/gkilfzjvd.sHtML

[T15] Kotlin：接口
来源：http://baike.hesvh.cn/Article/details/gpjoarumr.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.hesvh.cn/Article/details/gjhcwbphf.sHtML

[T16] Swift：Hello World
来源：http://3g.fehbvm.com/Article/details/gdjlmlzod.sHtML

print("Hello")
来源：http://blog.hesvh.cn/Article/details/gfubmpnlv.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.hesvh.cn/Article/details/gxyicigwb.sHtML

var a = 1;  let b = 2
来源：http://m.share.fehbvm.com/Article/details/gzboxfhwc.sHtML

[T18] Swift：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gpynrimvg.sHtML

"值: \(b)"
来源：http://read.share.zdbjq.cn/Article/details/gyoknixkx.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fehbvm.com/Article/details/gpkbjehxe.sHtML

if let n = opt { print(n) }
来源：http://baike.fehbvm.com/Article/details/gkqcmggqw.sHtML

[T20] Swift：数组操作
来源：http://wap.hesvh.cn/Article/details/gquvzgsug.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.hesvh.cn/Article/details/gxgsmepxc.sHtML

[T21] Swift：遍历
来源：http://baike.zdbjq.cn/Article/details/gdqgpxrqe.sHtML

for x in a { print(x) }
来源：http://wap.fehbvm.com/Article/details/gspxzsski.sHtML

[T22] Swift：字典
来源：http://www.blog.hesvh.cn/Article/details/gqytasoee.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.zdbjq.cn/Article/details/gfvgliczz.sHtML

[T23] Swift：函数
来源：http://blog.zdbjq.cn/Article/details/gjnwoiuql.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.hesvh.cn/Article/details/gpjivlonw.sHtML

[T24] Swift：闭包
来源：http://www.m.share.fehbvm.com/Article/details/gifnrvkac.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.hesvh.cn/Article/details/ghttbvxuw.sHtML

[T25] Swift：结构体
来源：http://3g.fehbvm.com/Article/details/gtopudxvr.sHtML

struct P { var x: Int }
来源：http://blog.hesvh.cn/Article/details/gakiheqpz.sHtML

[T26] Swift：类与重写
来源：http://m.share.hesvh.cn/Article/details/ggctounyl.sHtML

class A: Base { override func f() {} }
来源：http://read.share.fehbvm.com/Article/details/gznicoovl.sHtML

[T27] Swift：错误处理
来源：http://www.blog.hesvh.cn/Article/details/gfbxqrgid.sHtML

do { try f() } catch { print(error) }
来源：http://wap.hesvh.cn/Article/details/gqabatlwg.sHtML

[T28] Swift：枚举
来源：http://www.share.fehbvm.com/Article/details/ggnsbnaxx.sHtML

enum Color { case red, green }
来源：http://www.m.share.hesvh.cn/Article/details/gsvgjctpw.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.fehbvm.com/Article/details/gngnlvdki.sHtML

guard let x = opt else { return }
来源：http://www.m.share.fehbvm.com/Article/details/gcxjixzrz.sHtML

[T30] Swift：协议
来源：http://baike.fehbvm.com/Article/details/gyquvzvar.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.hesvh.cn/Article/details/gjjklbvcp.sHtML

[T31] Lua：Hello World
来源：http://mobile.hesvh.cn/Article/details/gwbydpkfj.sHtML

print("Hello")
来源：http://3g.zdbjq.cn/Article/details/gsgjtklht.sHtML

[T32] Lua：局部变量
来源：http://www.blog.hesvh.cn/Article/details/gasqhwhdr.sHtML

local a = 1
来源：http://baike.fehbvm.com/Article/details/gkmzoovkb.sHtML

[T33] Lua：表（数组）
来源：http://mobile.hesvh.cn/Article/details/gbahjfrpq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.fehbvm.com/Article/details/gkbcvernd.sHtML

[T34] Lua：遍历表
来源：http://3g.fehbvm.com/Article/details/gqbgzwsvw.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.hesvh.cn/Article/details/gkbpazhgc.sHtML

[T35] Lua：字典表
来源：http://baike.hesvh.cn/Article/details/gxgyjovxc.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.zdbjq.cn/Article/details/gzgowrkyn.sHtML

[T36] Lua：函数
来源：http://www.share.hesvh.cn/Article/details/gqvzamerz.sHtML

function add(a, b) return a + b end
来源：http://blog.hesvh.cn/Article/details/ghqjmyamt.sHtML

[T37] Lua：字符串拼接
来源：http://blog.zdbjq.cn/Article/details/gvudzbffy.sHtML

"a" .. "b"
来源：http://3g.fehbvm.com/Article/details/goossgyft.sHtML

[T38] Lua：条件
来源：http://read.share.hesvh.cn/Article/details/gknjvybjz.sHtML

if x > 0 then print("正") end
来源：http://baike.hesvh.cn/Article/details/gleqwdjys.sHtML

[T39] Lua：模式匹配
来源：http://baike.zdbjq.cn/Article/details/gpzwrzxwu.sHtML

string.find(s, "%d+")
来源：http://read.share.fehbvm.com/Article/details/gfaeqtpwa.sHtML

[T40] Lua：元表
来源：http://baike.hesvh.cn/Article/details/glnlaouso.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.fehbvm.com/Article/details/gneluxkob.sHtML

[T41] Perl：Hello World
来源：http://mobile.fehbvm.com/Article/details/gmhbcllbn.sHtML

print "Hello\n";
来源：http://baike.fehbvm.com/Article/details/gxfpaljwl.sHtML

[T42] Perl：变量类型
来源：http://www.share.hesvh.cn/Article/details/gwqnpebcg.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.hesvh.cn/Article/details/gaehqcluf.sHtML

[T43] Perl：字符串插值
来源：http://baike.hesvh.cn/Article/details/gnoujfrqa.sHtML

"值: $a"
来源：http://www.blog.fehbvm.com/Article/details/gxfdchsld.sHtML

[T44] Perl：条件
来源：http://www.share.fehbvm.com/Article/details/gxosevvgj.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.zdbjq.cn/Article/details/gppoavabt.sHtML

[T45] Perl：数组遍历
来源：http://m.share.fehbvm.com/Article/details/gbsiswpok.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.hesvh.cn/Article/details/guwqlfzks.sHtML

[T46] Perl：哈希操作
来源：http://wap.hesvh.cn/Article/details/gtxerfhxs.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.zdbjq.cn/Article/details/gmyafirqy.sHtML

[T47] Perl：正则捕获
来源：http://wap.fehbvm.com/Article/details/gtblyvlwm.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.zdbjq.cn/Article/details/gronwmcpt.sHtML

[T48] Perl：正则替换
来源：http://wap.hesvh.cn/Article/details/gmwosxfdz.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.zdbjq.cn/Article/details/gveuhqypr.sHtML

[T49] Perl：函数
来源：http://www.blog.fehbvm.com/Article/details/gzfisxwyf.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/glveurwgy.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/guigmyddu.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.zdbjq.cn/Article/details/gkpqovtjv.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.zdbjq.cn/Article/details/gqhqyfwgh.sHtML

[T51] Scala：Hello World
来源：http://wap.zdbjq.cn/Article/details/gyibkjebu.sHtML

println("Hello")
来源：http://mobile.hesvh.cn/Article/details/gfrcnsset.sHtML

[T52] Scala：变量
来源：http://www.m.share.zdbjq.cn/Article/details/gvgfawhlb.sHtML

val a = 1;  var b = 2
来源：http://3g.zdbjq.cn/Article/details/gisibdnbn.sHtML

[T53] Scala：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gwjvnubbh.sHtML

s"值: $b"
来源：http://m.share.fehbvm.com/Article/details/gichaoyle.sHtML

[T54] Scala：集合映射
来源：http://mobile.hesvh.cn/Article/details/gqxuvgsrc.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.fehbvm.com/Article/details/gpvpodaau.sHtML

[T55] Scala：集合过滤
来源：http://www.share.hesvh.cn/Article/details/gfwcxiebf.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.fehbvm.com/Article/details/gvotjidng.sHtML

[T56] Scala：样例类
来源：http://www.m.share.hesvh.cn/Article/details/gunyivqfl.sHtML

case class User(name: String, age: Int)
来源：http://wap.zdbjq.cn/Article/details/gzreaejes.sHtML

[T57] Scala：模式匹配
来源：http://wap.hesvh.cn/Article/details/gzwekxjgm.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.zdbjq.cn/Article/details/gbfcogwnk.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.zdbjq.cn/Article/details/goeekoiae.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.fehbvm.com/Article/details/gwbxzyilo.sHtML

[T59] Scala：循环
来源：http://mobile.fehbvm.com/Article/details/glvrhmzku.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.fehbvm.com/Article/details/gmiutvqaz.sHtML

[T60] Scala：折叠
来源：http://3g.fehbvm.com/Article/details/gvsxioxwq.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.hesvh.cn/Article/details/gtpfakkel.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gsvmzqjzw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.zdbjq.cn/Article/details/gctmvwmrz.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gxlvjcejt.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.zdbjq.cn/Article/details/gauujfipl.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.hesvh.cn/Article/details/gfvxzzbis.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.fehbvm.com/Article/details/gepmgfglv.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.fehbvm.com/Article/details/gijiogsqh.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.fehbvm.com/Article/details/gmefqfaac.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.hesvh.cn/Article/details/gclhayczt.sHtML

[U04] Py：变量调试打印
来源：http://read.share.hesvh.cn/Article/details/govfieleu.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fehbvm.com/Article/details/gataiqwuk.sHtML

[U05] Py：列表去重且保序
来源：http://3g.hesvh.cn/Article/details/gaypxqfhl.sHtML

list(dict.fromkeys(arr))
来源：http://wap.zdbjq.cn/Article/details/gfxogocnw.sHtML

[U06] Py：合并两个字典
来源：http://wap.fehbvm.com/Article/details/gatzwzrdu.sHtML

{**a, **b}
来源：http://baike.hesvh.cn/Article/details/gmnrfmouc.sHtML

[U07] Py：反转字典键值
来源：http://blog.fehbvm.com/Article/details/gorwvbrvd.sHtML

{v: k for k, v in d.items()}
来源：http://baike.hesvh.cn/Article/details/gmlmipkbz.sHtML

[U08] Py：展平二维列表
来源：http://read.share.fehbvm.com/Article/details/gyhalxsiq.sHtML

[y for x in nested for y in x]
来源：http://mobile.zdbjq.cn/Article/details/gpqublimc.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.fehbvm.com/Article/details/ghntznvpf.sHtML

max(d, key=d.get)
来源：http://www.m.share.fehbvm.com/Article/details/gorvdgfeb.sHtML

[U10] Py：按值排序字典
来源：http://mobile.hesvh.cn/Article/details/gdmnfzysp.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.hesvh.cn/Article/details/gwqccxniv.sHtML

[U11] Py：生成器表达式
来源：http://baike.hesvh.cn/Article/details/gqzbxnkcb.sHtML

(x * 2 for x in arr)
来源：http://read.share.zdbjq.cn/Article/details/ggjqmhxoq.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.fehbvm.com/Article/details/guibinvrj.sHtML

Counter(arr).most_common(3)
来源：http://mobile.fehbvm.com/Article/details/gevaxrswn.sHtML

[U13] Py：固定长度队列
来源：http://3g.fehbvm.com/Article/details/gegilmcye.sHtML

deque(maxlen=10)
来源：http://www.m.share.fehbvm.com/Article/details/gxklrvqbo.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.fehbvm.com/Article/details/gwmemhoez.sHtML

defaultdict(list)
来源：http://3g.hesvh.cn/Article/details/gycnvcuww.sHtML

[U15] Py：高精度计时
来源：http://baike.zdbjq.cn/Article/details/gbneakrpi.sHtML

t = time.perf_counter()
来源：http://m.share.fehbvm.com/Article/details/gfnaapzdd.sHtML

[U16] Py：命令行参数解析
来源：http://baike.fehbvm.com/Article/details/gmodnrogg.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.fehbvm.com/Article/details/gsgobuayj.sHtML

[U17] Py：初始化日志
来源：http://www.blog.fehbvm.com/Article/details/gbcvqlzbu.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.fehbvm.com/Article/details/gsntfbgge.sHtML

[U18] Py：预编译正则
来源：http://m.share.fehbvm.com/Article/details/gigzvgueq.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.zdbjq.cn/Article/details/ggufeaomx.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.fehbvm.com/Article/details/gtfdnepoa.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.fehbvm.com/Article/details/gmelgaltw.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.hesvh.cn/Article/details/ghpqbbwoz.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.zdbjq.cn/Article/details/gzuvurbih.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.zdbjq.cn/Article/details/gubaxphjw.sHtML

@contextlib.contextmanager
来源：http://www.blog.hesvh.cn/Article/details/gkjfadegd.sHtML

[U22] Py：矩阵转置
来源：http://baike.zdbjq.cn/Article/details/gedqmpnwn.sHtML

list(zip(*m))
来源：http://3g.fehbvm.com/Article/details/gufoqlzvv.sHtML

[U23] Py：分块读取大文件
来源：http://wap.zdbjq.cn/Article/details/gnlvaycfq.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.hesvh.cn/Article/details/gwukygijk.sHtML

[U24] Py：路径操作
来源：http://blog.hesvh.cn/Article/details/gscimspsi.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.fehbvm.com/Article/details/gwosicruv.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.fehbvm.com/Article/details/gduorrdro.sHtML

csv.DictReader(f)
来源：http://mobile.fehbvm.com/Article/details/ghoyjnmud.sHtML

[U26] Py：并发下载
来源：http://baike.zdbjq.cn/Article/details/gcemlqyel.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.zdbjq.cn/Article/details/gwbjvyvtd.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.zdbjq.cn/Article/details/gvuyegstx.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.fehbvm.com/Article/details/gldhwatrr.sHtML

[U28] Py：类型别名
来源：http://m.share.zdbjq.cn/Article/details/geyfspybi.sHtML

UserId = int
来源：http://baike.fehbvm.com/Article/details/grjsxaffb.sHtML

[U29] Py：属性校验
来源：http://www.m.share.hesvh.cn/Article/details/groigkcyf.sHtML

@property 与 @x.setter 配合
来源：http://m.share.zdbjq.cn/Article/details/gqlfdltjw.sHtML

[U30] Py：数据类
来源：http://m.share.hesvh.cn/Article/details/glbviyxof.sHtML

@dataclass(slots=True)
来源：http://blog.hesvh.cn/Article/details/gdorpgzws.sHtML

[U31] Py：单测
来源：http://www.share.hesvh.cn/Article/details/grdxjgtrl.sHtML

python -m pytest -q
来源：http://m.share.hesvh.cn/Article/details/gdkswnpje.sHtML

[U32] Py：代码格式化
来源：http://www.share.zdbjq.cn/Article/details/gsbtcnvsw.sHtML

ruff format . && ruff check --fix .
来源：http://baike.hesvh.cn/Article/details/glaayhakd.sHtML

[U33] Py：打包发布
来源：http://read.share.hesvh.cn/Article/details/gpegafkmv.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.zdbjq.cn/Article/details/gqwfddacp.sHtML

[U34] Py：判断编码
来源：http://read.share.fehbvm.com/Article/details/guzzqmibt.sHtML

chardet.detect(raw)
来源：http://m.share.hesvh.cn/Article/details/grsuubbte.sHtML

[U35] Py：发送邮件
来源：http://www.blog.fehbvm.com/Article/details/gzgrboyuz.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.hesvh.cn/Article/details/gijtngmrv.sHtML

[U36] Py：定时任务
来源：http://www.m.share.fehbvm.com/Article/details/gxbjdwqxi.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.fehbvm.com/Article/details/glqfjcmrh.sHtML

[U37] Py：读写 Excel
来源：http://3g.hesvh.cn/Article/details/glfmlptxi.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.fehbvm.com/Article/details/gidlejjzw.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.fehbvm.com/Article/details/gejhvxtrl.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.zdbjq.cn/Article/details/gxvigcdxu.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.hesvh.cn/Article/details/gvdeeqpxo.sHtML

sys.stdout.isatty()
来源：http://www.share.hesvh.cn/Article/details/gqplijecx.sHtML

[U40] Py：打印到标准错误
来源：http://blog.fehbvm.com/Article/details/ggwtjykfe.sHtML

print("err", file=sys.stderr)
来源：http://m.share.fehbvm.com/Article/details/gvemifndm.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.fehbvm.com/Article/details/gksbnnwhc.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.zdbjq.cn/Article/details/gapltoppl.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.zdbjq.cn/Article/details/gyxftfpts.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.hesvh.cn/Article/details/guhjvtiri.sHtML

[U43] PHP：声明命名空间
来源：http://3g.fehbvm.com/Article/details/gogopsaxu.sHtML

namespace App\Http;
来源：http://www.blog.hesvh.cn/Article/details/gszoihjbc.sHtML

[U44] PHP：开启严格类型
来源：http://wap.hesvh.cn/Article/details/gbbwcbebu.sHtML

declare(strict_types=1);
来源：http://3g.fehbvm.com/Article/details/grvarcamt.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.hesvh.cn/Article/details/guwnblgss.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gwaafpwld.sHtML

[U46] PHP：可空类型
来源：http://3g.zdbjq.cn/Article/details/ggmczrysw.sHtML

?string $name = null
来源：http://blog.fehbvm.com/Article/details/gnkoialdl.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.zdbjq.cn/Article/details/gakxvhned.sHtML

int|string $id
来源：http://baike.hesvh.cn/Article/details/grmzhszdd.sHtML

[U48] PHP：纯枚举
来源：http://blog.hesvh.cn/Article/details/gwzituwhj.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.fehbvm.com/Article/details/grjacwcfr.sHtML

[U49] PHP：只读属性
来源：http://wap.hesvh.cn/Article/details/guogoeqqv.sHtML

public readonly string $name
来源：http://3g.zdbjq.cn/Article/details/gspdxwdug.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.hesvh.cn/Article/details/gfqyghfqb.sHtML

public function __construct(private int $id) {}
来源：http://m.share.fehbvm.com/Article/details/gagvgcmjb.sHtML

[U51] PHP：数组解构
来源：http://mobile.hesvh.cn/Article/details/gystvjzeu.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.fehbvm.com/Article/details/gvxnrqais.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.zdbjq.cn/Article/details/gtdficsyf.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.fehbvm.com/Article/details/gzhqzeikp.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.fehbvm.com/Article/details/gquejgmdk.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.hesvh.cn/Article/details/giqerphsm.sHtML

[U54] PHP：空安全调用
来源：http://www.share.fehbvm.com/Article/details/glqxjuvuo.sHtML

$obj?->method()
来源：http://blog.hesvh.cn/Article/details/gpmvculgn.sHtML

[U55] PHP：match 表达式
来源：http://blog.hesvh.cn/Article/details/gpljkfgtj.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.fehbvm.com/Article/details/gujgagnya.sHtML

[U56] PHP：命名参数
来源：http://www.blog.zdbjq.cn/Article/details/ggttsnjlm.sHtML

f(a: 1, b: 2)
来源：http://www.share.hesvh.cn/Article/details/gfwwfosxp.sHtML

[U57] PHP：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gfsaqiria.sHtML

"值: {$a}"
来源：http://www.blog.hesvh.cn/Article/details/gvkhrqxnr.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.zdbjq.cn/Article/details/ggbssmtuo.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.hesvh.cn/Article/details/gqytaolgs.sHtML

[U59] PHP：自定义排序
来源：http://m.share.fehbvm.com/Article/details/gptfarrhe.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.zdbjq.cn/Article/details/gnonksgyk.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.hesvh.cn/Article/details/grqkjotju.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.hesvh.cn/Article/details/gbtdsoyrj.sHtML

[U61] PHP：正则
来源：http://3g.fehbvm.com/Article/details/gahvdjfxq.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.fehbvm.com/Article/details/gzsfedwly.sHtML

[U62] PHP：日期对象
来源：http://m.share.fehbvm.com/Article/details/glirqmxzl.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.fehbvm.com/Article/details/gniymokyc.sHtML

[U63] PHP：文件读写
来源：http://www.share.zdbjq.cn/Article/details/grjmfmvcu.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.fehbvm.com/Article/details/gavqzlker.sHtML

[U64] PHP：目录遍历
来源：http://read.share.zdbjq.cn/Article/details/gizhyrbme.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.hesvh.cn/Article/details/gxdcabpfx.sHtML

[U65] PHP：会话
来源：http://mobile.zdbjq.cn/Article/details/gpywssbym.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gafnlhqcx.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.fehbvm.com/Article/details/gjpquctpw.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.fehbvm.com/Article/details/gecovnjpt.sHtML

[U67] PHP：处理文件上传
来源：http://baike.hesvh.cn/Article/details/gieehvnjp.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.zdbjq.cn/Article/details/gntebgshe.sHtML

[U68] PHP：PDO 连接
来源：http://wap.hesvh.cn/Article/details/gajhtufwe.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.zdbjq.cn/Article/details/gzwnulyen.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.hesvh.cn/Article/details/gvsitgybc.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.fehbvm.com/Article/details/gtaukcfit.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.fehbvm.com/Article/details/ggegheovi.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.zdbjq.cn/Article/details/gfzxljzro.sHtML

[U71] PHP：抛出异常
来源：http://m.share.fehbvm.com/Article/details/gfyxzthod.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.fehbvm.com/Article/details/gtbetjata.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.fehbvm.com/Article/details/gkxcfhoiq.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.fehbvm.com/Article/details/gjpmkibmg.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.hesvh.cn/Article/details/glmvpnvap.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.hesvh.cn/Article/details/gfyixqnxt.sHtML

[U74] PHP：读取环境变量
来源：http://blog.fehbvm.com/Article/details/gwpmiklec.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.hesvh.cn/Article/details/gpzfdeppx.sHtML


<!-- 参考信息 -->