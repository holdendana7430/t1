代发 wailian999

while (std::getline(in, line)) { }
来源：http://3g.fehbvm.com/Article/details/grztestlb.sHtML

[S49] C++：写文件
来源：http://m.share.zdbjq.cn/Article/details/gipcowimc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.zdbjq.cn/Article/details/gbrrieahk.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.zdbjq.cn/Article/details/gsiasyacg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gegxeuvsu.sHtML

[S51] C++：显式类型转换
来源：http://read.share.hesvh.cn/Article/details/grjbqbkio.sHtML

static_cast<double>(a) / b
来源：http://mobile.fehbvm.com/Article/details/ghxtkyrwv.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.hesvh.cn/Article/details/gtimpznwx.sHtML

int size() const noexcept { return n_; }
来源：http://wap.zdbjq.cn/Article/details/gruvntnza.sHtML

[S53] C++：移动语义
来源：http://m.share.fehbvm.com/Article/details/gobtohypc.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fehbvm.com/Article/details/gjugpkpxo.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fehbvm.com/Article/details/gbczoeubn.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fehbvm.com/Article/details/gjzmxqvfj.sHtML

[S55] C++：结构化绑定
来源：http://3g.zdbjq.cn/Article/details/gnvpuknfh.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.hesvh.cn/Article/details/gkvqsxlqu.sHtML

[S56] C++：optional
来源：http://www.blog.fehbvm.com/Article/details/gjpdljtjp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.hesvh.cn/Article/details/geoipzvjc.sHtML

[S57] C++：编译期常量
来源：http://3g.zdbjq.cn/Article/details/gdznxhcmq.sHtML

constexpr int N = 10;
来源：http://m.share.fehbvm.com/Article/details/gewjcnlmf.sHtML

[S58] C++：命名空间
来源：http://mobile.zdbjq.cn/Article/details/grwqszmla.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.hesvh.cn/Article/details/gjcsnevge.sHtML

[S59] C++：静态断言
来源：http://www.blog.hesvh.cn/Article/details/gbyefajja.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.hesvh.cn/Article/details/gpihsryez.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.hesvh.cn/Article/details/geybeotsk.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.hesvh.cn/Article/details/gjfvlbumn.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gjqpkodwy.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.zdbjq.cn/Article/details/gypgbmcfr.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gmzvnuxnv.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.hesvh.cn/Article/details/gjjfyjifd.sHtML

println("Hello")
来源：http://wap.hesvh.cn/Article/details/gejucrbdt.sHtML

[T02] Kotlin：变量
来源：http://baike.fehbvm.com/Article/details/gjfepldpe.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.zdbjq.cn/Article/details/gunmhgays.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.hesvh.cn/Article/details/glhfuvhmt.sHtML

"值: $b"
来源：http://read.share.fehbvm.com/Article/details/ganpytrxs.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.zdbjq.cn/Article/details/gfwkbdewb.sHtML

val n: String? = null;  n?.length
来源：http://blog.zdbjq.cn/Article/details/gdvspgkoh.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.hesvh.cn/Article/details/gsacfzkby.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.hesvh.cn/Article/details/gajkiijrs.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fehbvm.com/Article/details/gurgphfoz.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fehbvm.com/Article/details/ggmigyuun.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.hesvh.cn/Article/details/goptxkscb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fehbvm.com/Article/details/gqvacyvoe.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fehbvm.com/Article/details/geoxeguyo.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.zdbjq.cn/Article/details/glajgqdoj.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fehbvm.com/Article/details/gqzaegwhd.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.hesvh.cn/Article/details/gijaukiss.sHtML

[T10] Kotlin：默认参数
来源：http://blog.zdbjq.cn/Article/details/gkicbidhc.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.hesvh.cn/Article/details/gqakmhzuz.sHtML

[T11] Kotlin：协程
来源：http://wap.zdbjq.cn/Article/details/gcbviwmow.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.zdbjq.cn/Article/details/ghggjgqom.sHtML

[T12] Kotlin：解构声明
来源：http://baike.zdbjq.cn/Article/details/gkaxmhuaw.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gfmhltbrd.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.zdbjq.cn/Article/details/gmxsrlsnf.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.zdbjq.cn/Article/details/gsygzifha.sHtML

[T14] Kotlin：循环
来源：http://wap.hesvh.cn/Article/details/gkijiyzdq.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fehbvm.com/Article/details/gibbqpwhj.sHtML

[T15] Kotlin：接口
来源：http://wap.fehbvm.com/Article/details/grqoiuouc.sHtML

interface Shape { fun area(): Double }
来源：http://wap.zdbjq.cn/Article/details/gbivwecgr.sHtML

[T16] Swift：Hello World
来源：http://baike.zdbjq.cn/Article/details/gbdqbijrv.sHtML

print("Hello")
来源：http://3g.zdbjq.cn/Article/details/gqydsbhov.sHtML

[T17] Swift：变量与常量
来源：http://3g.fehbvm.com/Article/details/gjjefzapx.sHtML

var a = 1;  let b = 2
来源：http://wap.hesvh.cn/Article/details/gwqiaasqi.sHtML

[T18] Swift：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gsxzfipqh.sHtML

"值: \(b)"
来源：http://m.share.zdbjq.cn/Article/details/gqlqzqbha.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fehbvm.com/Article/details/gnfhixqug.sHtML

if let n = opt { print(n) }
来源：http://wap.zdbjq.cn/Article/details/gawjcddid.sHtML

[T20] Swift：数组操作
来源：http://baike.hesvh.cn/Article/details/gmekbyrtq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fehbvm.com/Article/details/gtjxmhvnt.sHtML

[T21] Swift：遍历
来源：http://3g.fehbvm.com/Article/details/gqilwgqer.sHtML

for x in a { print(x) }
来源：http://blog.hesvh.cn/Article/details/gzutdgczf.sHtML

[T22] Swift：字典
来源：http://3g.fehbvm.com/Article/details/gfwmgsvcf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.zdbjq.cn/Article/details/gdbslewwu.sHtML

[T23] Swift：函数
来源：http://www.share.hesvh.cn/Article/details/ggbeazqgj.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.zdbjq.cn/Article/details/gobstgjsm.sHtML

[T24] Swift：闭包
来源：http://baike.hesvh.cn/Article/details/gdetajhjw.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.hesvh.cn/Article/details/gsmeovkod.sHtML

[T25] Swift：结构体
来源：http://3g.fehbvm.com/Article/details/gnatoulvw.sHtML

struct P { var x: Int }
来源：http://baike.fehbvm.com/Article/details/gedlpkbyw.sHtML

[T26] Swift：类与重写
来源：http://www.share.zdbjq.cn/Article/details/gkcgqaeip.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fehbvm.com/Article/details/gqsjjfqmq.sHtML

[T27] Swift：错误处理
来源：http://m.share.zdbjq.cn/Article/details/gotbtzovp.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.hesvh.cn/Article/details/goipodjhn.sHtML

[T28] Swift：枚举
来源：http://blog.hesvh.cn/Article/details/gtpyvytwk.sHtML

enum Color { case red, green }
来源：http://m.share.fehbvm.com/Article/details/gwdofllvi.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.hesvh.cn/Article/details/gcreqogoc.sHtML

guard let x = opt else { return }
来源：http://m.share.fehbvm.com/Article/details/gmwngbbcf.sHtML

[T30] Swift：协议
来源：http://3g.hesvh.cn/Article/details/glpbqtbhz.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fehbvm.com/Article/details/gijrkvzax.sHtML

[T31] Lua：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gwgsmhrnh.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/gvxzgjexw.sHtML

[T32] Lua：局部变量
来源：http://mobile.fehbvm.com/Article/details/ggvczzlnp.sHtML

local a = 1
来源：http://baike.fehbvm.com/Article/details/gwvjhdxwm.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.hesvh.cn/Article/details/gmjhzvqme.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.hesvh.cn/Article/details/gnfttiklg.sHtML

[T34] Lua：遍历表
来源：http://m.share.hesvh.cn/Article/details/gxtirknel.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.hesvh.cn/Article/details/gzxumvqbm.sHtML

[T35] Lua：字典表
来源：http://baike.zdbjq.cn/Article/details/gmpcgxplu.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.zdbjq.cn/Article/details/grhzryhxm.sHtML

[T36] Lua：函数
来源：http://www.m.share.fehbvm.com/Article/details/gayfwmxdd.sHtML

function add(a, b) return a + b end
来源：http://m.share.hesvh.cn/Article/details/gfwwbzcsg.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.zdbjq.cn/Article/details/gcrnzjnig.sHtML

"a" .. "b"
来源：http://www.share.fehbvm.com/Article/details/gufysvzqv.sHtML

[T38] Lua：条件
来源：http://baike.hesvh.cn/Article/details/gfxezsacp.sHtML

if x > 0 then print("正") end
来源：http://baike.zdbjq.cn/Article/details/gdrhlcjuv.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fehbvm.com/Article/details/gbbkripql.sHtML

string.find(s, "%d+")
来源：http://blog.zdbjq.cn/Article/details/gisakuosj.sHtML

[T40] Lua：元表
来源：http://3g.zdbjq.cn/Article/details/grjdogjqz.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.fehbvm.com/Article/details/gzgcmpwrc.sHtML

[T41] Perl：Hello World
来源：http://blog.fehbvm.com/Article/details/gncsauplz.sHtML

print "Hello\n";
来源：http://blog.fehbvm.com/Article/details/goskzfdkh.sHtML

[T42] Perl：变量类型
来源：http://blog.fehbvm.com/Article/details/gftsoykwq.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.zdbjq.cn/Article/details/gushldjtv.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gjyhuxhag.sHtML

"值: $a"
来源：http://read.share.fehbvm.com/Article/details/gaizwyhbc.sHtML

[T44] Perl：条件
来源：http://read.share.fehbvm.com/Article/details/ggitjhxjx.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.hesvh.cn/Article/details/gpunihnmm.sHtML

[T45] Perl：数组遍历
来源：http://baike.zdbjq.cn/Article/details/gfumrovah.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.hesvh.cn/Article/details/gbcasxgka.sHtML

[T46] Perl：哈希操作
来源：http://www.share.hesvh.cn/Article/details/gytettyfq.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.zdbjq.cn/Article/details/giannztpx.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.fehbvm.com/Article/details/gsrgfbczh.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.hesvh.cn/Article/details/gthovoblz.sHtML

[T48] Perl：正则替换
来源：http://www.blog.zdbjq.cn/Article/details/gyiafnqfv.sHtML

$s =~ s/old/new/g;
来源：http://www.share.fehbvm.com/Article/details/gitvhvymb.sHtML

[T49] Perl：函数
来源：http://wap.hesvh.cn/Article/details/gmrujafid.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gohhnufyx.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/grqcintns.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.hesvh.cn/Article/details/gjifcfkrw.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.fehbvm.com/Article/details/gulleqxly.sHtML

[T51] Scala：Hello World
来源：http://m.share.fehbvm.com/Article/details/ghxnmaprn.sHtML

println("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gdeifmqkf.sHtML

[T52] Scala：变量
来源：http://www.m.share.zdbjq.cn/Article/details/gajuolcmt.sHtML

val a = 1;  var b = 2
来源：http://www.blog.hesvh.cn/Article/details/gpuuhtwvs.sHtML

[T53] Scala：字符串插值
来源：http://baike.fehbvm.com/Article/details/gnfvqhcji.sHtML

s"值: $b"
来源：http://wap.zdbjq.cn/Article/details/gpujsknhx.sHtML

[T54] Scala：集合映射
来源：http://wap.hesvh.cn/Article/details/grdwlgujn.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.fehbvm.com/Article/details/grexjciwk.sHtML

[T55] Scala：集合过滤
来源：http://www.share.hesvh.cn/Article/details/gdvishjot.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.zdbjq.cn/Article/details/gandfjxpy.sHtML

[T56] Scala：样例类
来源：http://baike.hesvh.cn/Article/details/ggtqeadfq.sHtML

case class User(name: String, age: Int)
来源：http://www.share.zdbjq.cn/Article/details/gbpynxkze.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.hesvh.cn/Article/details/grhwyngwr.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.zdbjq.cn/Article/details/geinmwmki.sHtML

[T58] Scala：函数定义
来源：http://blog.zdbjq.cn/Article/details/gsarctgtb.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.hesvh.cn/Article/details/gpxaqnkdq.sHtML

[T59] Scala：循环
来源：http://m.share.hesvh.cn/Article/details/gvkkquhif.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.fehbvm.com/Article/details/gtloededn.sHtML

[T60] Scala：折叠
来源：http://mobile.fehbvm.com/Article/details/gmrttxrrl.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fehbvm.com/Article/details/gcnhwllxq.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gjbhlkrig.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fehbvm.com/Article/details/goyvsfpup.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/guigwcdmu.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.fehbvm.com/Article/details/gbjxtytxd.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.fehbvm.com/Article/details/gvesmcenz.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.hesvh.cn/Article/details/gufzsolum.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.zdbjq.cn/Article/details/gmxylnmwo.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.hesvh.cn/Article/details/gfdwdaohk.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.fehbvm.com/Article/details/gejpadrtx.sHtML

[U04] Py：变量调试打印
来源：http://blog.fehbvm.com/Article/details/gzbysbrim.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.hesvh.cn/Article/details/gnelotvee.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.fehbvm.com/Article/details/gvbzugwrm.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.zdbjq.cn/Article/details/gfhcpftdg.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fehbvm.com/Article/details/gufzeqhuf.sHtML

{**a, **b}
来源：http://blog.fehbvm.com/Article/details/gvnkfrzdf.sHtML

[U07] Py：反转字典键值
来源：http://www.share.hesvh.cn/Article/details/gshyaadhp.sHtML

{v: k for k, v in d.items()}
来源：http://wap.fehbvm.com/Article/details/gzlcrpfyv.sHtML

[U08] Py：展平二维列表
来源：http://baike.hesvh.cn/Article/details/gsuudbvsq.sHtML

[y for x in nested for y in x]
来源：http://www.blog.hesvh.cn/Article/details/gmsezlkoi.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.hesvh.cn/Article/details/gxpsdyohr.sHtML

max(d, key=d.get)
来源：http://blog.fehbvm.com/Article/details/gplfueiln.sHtML

[U10] Py：按值排序字典
来源：http://www.share.fehbvm.com/Article/details/glyrzhoso.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.zdbjq.cn/Article/details/ghjbevjha.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.zdbjq.cn/Article/details/gstuqqgvy.sHtML

(x * 2 for x in arr)
来源：http://read.share.hesvh.cn/Article/details/gihzlxgdv.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.zdbjq.cn/Article/details/geaupwnxr.sHtML

Counter(arr).most_common(3)
来源：http://baike.fehbvm.com/Article/details/gicftmoln.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.fehbvm.com/Article/details/gneawbxjg.sHtML

deque(maxlen=10)
来源：http://mobile.zdbjq.cn/Article/details/gtcpbptqv.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.fehbvm.com/Article/details/gcbtperlp.sHtML

defaultdict(list)
来源：http://m.share.hesvh.cn/Article/details/gcfqljazy.sHtML

[U15] Py：高精度计时
来源：http://blog.fehbvm.com/Article/details/gdzecdfzp.sHtML

t = time.perf_counter()
来源：http://www.m.share.zdbjq.cn/Article/details/glyxyflcr.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.zdbjq.cn/Article/details/gcolqotfh.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.hesvh.cn/Article/details/gepffndzx.sHtML

[U17] Py：初始化日志
来源：http://mobile.hesvh.cn/Article/details/gcnvqnerm.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.fehbvm.com/Article/details/gyexnnrca.sHtML

[U18] Py：预编译正则
来源：http://www.share.zdbjq.cn/Article/details/ggrbnwoze.sHtML

pat = re.compile(r"\d+")
来源：http://blog.hesvh.cn/Article/details/gyylrwhty.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.hesvh.cn/Article/details/gfjyykitb.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.zdbjq.cn/Article/details/gisqontag.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.fehbvm.com/Article/details/gvnxwlusl.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.zdbjq.cn/Article/details/glbyjxlvl.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.zdbjq.cn/Article/details/gikizzdkp.sHtML

@contextlib.contextmanager
来源：http://wap.hesvh.cn/Article/details/gwukjbnre.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.hesvh.cn/Article/details/giokzhzrl.sHtML

list(zip(*m))
来源：http://3g.hesvh.cn/Article/details/gortwrgux.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.fehbvm.com/Article/details/gdhudzftc.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.zdbjq.cn/Article/details/gpikeidse.sHtML

[U24] Py：路径操作
来源：http://m.share.fehbvm.com/Article/details/gtacdwzng.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.fehbvm.com/Article/details/gvwyjjbun.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.zdbjq.cn/Article/details/gvjklhhez.sHtML

csv.DictReader(f)
来源：http://www.m.share.hesvh.cn/Article/details/gevsimmlc.sHtML

[U26] Py：并发下载
来源：http://www.share.fehbvm.com/Article/details/gpvjpgyws.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.hesvh.cn/Article/details/gdupwxyef.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fehbvm.com/Article/details/gbernrgsv.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.hesvh.cn/Article/details/gdxdwmuvt.sHtML

[U28] Py：类型别名
来源：http://www.m.share.hesvh.cn/Article/details/gxxgfcnza.sHtML

UserId = int
来源：http://wap.hesvh.cn/Article/details/geqepbsec.sHtML

[U29] Py：属性校验
来源：http://m.share.zdbjq.cn/Article/details/gsfzffwet.sHtML

@property 与 @x.setter 配合
来源：http://wap.fehbvm.com/Article/details/guqtyvqfm.sHtML

[U30] Py：数据类
来源：http://baike.fehbvm.com/Article/details/ggvjvgvza.sHtML

@dataclass(slots=True)
来源：http://www.share.hesvh.cn/Article/details/gmetqhrqk.sHtML

[U31] Py：单测
来源：http://wap.hesvh.cn/Article/details/gvuaxbyxq.sHtML

python -m pytest -q
来源：http://blog.fehbvm.com/Article/details/ggqtdytlk.sHtML

[U32] Py：代码格式化
来源：http://mobile.fehbvm.com/Article/details/glnzgzrdu.sHtML

ruff format . && ruff check --fix .
来源：http://baike.fehbvm.com/Article/details/gbxpujeef.sHtML

[U33] Py：打包发布
来源：http://www.blog.hesvh.cn/Article/details/gsxtznzvy.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.hesvh.cn/Article/details/gevhkyhpj.sHtML

[U34] Py：判断编码
来源：http://wap.zdbjq.cn/Article/details/gjxmvtvno.sHtML

chardet.detect(raw)
来源：http://read.share.zdbjq.cn/Article/details/gsbzwlive.sHtML

[U35] Py：发送邮件
来源：http://www.share.fehbvm.com/Article/details/gclhzmnsz.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.hesvh.cn/Article/details/gyfjxvueu.sHtML

[U36] Py：定时任务
来源：http://blog.zdbjq.cn/Article/details/gayblkwoo.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.hesvh.cn/Article/details/gjjjfmlaa.sHtML

[U37] Py：读写 Excel
来源：http://wap.zdbjq.cn/Article/details/gatljrwwu.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.hesvh.cn/Article/details/gfsetspor.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.zdbjq.cn/Article/details/gppcoinkv.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.fehbvm.com/Article/details/ggzniociy.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.zdbjq.cn/Article/details/gxeupnize.sHtML

sys.stdout.isatty()
来源：http://3g.hesvh.cn/Article/details/ghmwbohif.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.hesvh.cn/Article/details/gdzyajwuk.sHtML

print("err", file=sys.stderr)
来源：http://www.share.hesvh.cn/Article/details/grxlyeeya.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.zdbjq.cn/Article/details/gyhzjydsm.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.fehbvm.com/Article/details/gsdmqomkz.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.zdbjq.cn/Article/details/gxnmxtmit.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.fehbvm.com/Article/details/gwapzcccb.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.fehbvm.com/Article/details/gmdpcgebf.sHtML

namespace App\Http;
来源：http://3g.hesvh.cn/Article/details/ghsgychie.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.fehbvm.com/Article/details/gvxwwvmhf.sHtML

declare(strict_types=1);
来源：http://www.share.zdbjq.cn/Article/details/gazwehzna.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.fehbvm.com/Article/details/gtfmunvld.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/ggbkgkdrx.sHtML

[U46] PHP：可空类型
来源：http://3g.hesvh.cn/Article/details/gvdsuvtmt.sHtML

?string $name = null
来源：http://3g.zdbjq.cn/Article/details/gbiuflnox.sHtML

[U47] PHP：联合类型
来源：http://blog.zdbjq.cn/Article/details/giekqtgqw.sHtML

int|string $id
来源：http://www.blog.hesvh.cn/Article/details/gbvrauflg.sHtML

[U48] PHP：纯枚举
来源：http://baike.zdbjq.cn/Article/details/gbaxumifr.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.hesvh.cn/Article/details/gkesqiony.sHtML

[U49] PHP：只读属性
来源：http://m.share.zdbjq.cn/Article/details/gdzgrvkxs.sHtML

public readonly string $name
来源：http://blog.zdbjq.cn/Article/details/giivmxzjx.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.hesvh.cn/Article/details/goxszvkzb.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.hesvh.cn/Article/details/gnpmhkfkp.sHtML

[U51] PHP：数组解构
来源：http://www.blog.hesvh.cn/Article/details/goexebgwd.sHtML

[$a, $b] = $arr;
来源：http://3g.fehbvm.com/Article/details/gafkmmeis.sHtML

[U52] PHP：箭头函数
来源：http://blog.zdbjq.cn/Article/details/ggiscbjvq.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.fehbvm.com/Article/details/gnqklpxnd.sHtML

[U53] PHP：空合并运算符
来源：http://baike.zdbjq.cn/Article/details/gwtljgqsh.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.zdbjq.cn/Article/details/gkcxfbell.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.hesvh.cn/Article/details/gyvbcezys.sHtML

$obj?->method()
来源：http://m.share.zdbjq.cn/Article/details/guymluhgp.sHtML

[U55] PHP：match 表达式
来源：http://m.share.hesvh.cn/Article/details/gxhfrcyfd.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.fehbvm.com/Article/details/grtdevspk.sHtML

[U56] PHP：命名参数
来源：http://www.share.zdbjq.cn/Article/details/gftmxultc.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/gmyrntevs.sHtML

[U57] PHP：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gphwbcakd.sHtML

"值: {$a}"
来源：http://blog.hesvh.cn/Article/details/gdbohbvee.sHtML

[U58] PHP：数组三件套
来源：http://read.share.fehbvm.com/Article/details/gakjxdlli.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.fehbvm.com/Article/details/gtrmcnkla.sHtML

[U59] PHP：自定义排序
来源：http://read.share.zdbjq.cn/Article/details/gqdmdqran.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.zdbjq.cn/Article/details/gygxwipjp.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.zdbjq.cn/Article/details/gkpeyytdt.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.fehbvm.com/Article/details/gqjiwhpnv.sHtML

[U61] PHP：正则
来源：http://blog.hesvh.cn/Article/details/gxiaeyldh.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.fehbvm.com/Article/details/gbhkhxaur.sHtML

[U62] PHP：日期对象
来源：http://www.share.hesvh.cn/Article/details/gbnljavwy.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.hesvh.cn/Article/details/gvvunrnay.sHtML

[U63] PHP：文件读写
来源：http://mobile.zdbjq.cn/Article/details/gchizdaor.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.fehbvm.com/Article/details/gavdaazbi.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.fehbvm.com/Article/details/goqdrurro.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.zdbjq.cn/Article/details/gmgpnujjo.sHtML

[U65] PHP：会话
来源：http://m.share.hesvh.cn/Article/details/gguylrkgw.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gcapmszkh.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.fehbvm.com/Article/details/glwuxqemf.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.zdbjq.cn/Article/details/globndxtq.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.hesvh.cn/Article/details/gefrsxvyh.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.zdbjq.cn/Article/details/gkfeecfco.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.zdbjq.cn/Article/details/getohydnh.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.hesvh.cn/Article/details/ggsrxxsfa.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.fehbvm.com/Article/details/gjgultbxe.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.fehbvm.com/Article/details/gwetuefuw.sHtML

[U70] PHP：PDO 事务
来源：http://wap.zdbjq.cn/Article/details/gfvcehavh.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.zdbjq.cn/Article/details/guzmxbqpd.sHtML

[U71] PHP：抛出异常
来源：http://blog.hesvh.cn/Article/details/gfamcafef.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.zdbjq.cn/Article/details/grdnvjlfd.sHtML

[U72] PHP：写错误日志
来源：http://read.share.zdbjq.cn/Article/details/gcqtsuvxj.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.hesvh.cn/Article/details/gvguhgjhe.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.fehbvm.com/Article/details/glgujfkwk.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.fehbvm.com/Article/details/gnvejgtim.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.fehbvm.com/Article/details/gghuiphpw.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.zdbjq.cn/Article/details/guqfcmays.sHtML


<!-- 参考信息 -->