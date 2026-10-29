代发 wailian999

while (std::getline(in, line)) { }
来源：http://mobile.hesvh.cn/Article/details/gaypebiao.sHtML

[S49] C++：写文件
来源：http://m.share.hesvh.cn/Article/details/gpkshqzjf.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.zdbjq.cn/Article/details/gtjhzkbsz.sHtML

[S50] C++：格式化数字
来源：http://mobile.hesvh.cn/Article/details/gttqtpcjp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fehbvm.com/Article/details/gzgtflcht.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.zdbjq.cn/Article/details/ghgkcqfiv.sHtML

static_cast<double>(a) / b
来源：http://wap.zdbjq.cn/Article/details/gpbceqvqo.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.zdbjq.cn/Article/details/gzwlvveiv.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fehbvm.com/Article/details/glrqmabcj.sHtML

[S53] C++：移动语义
来源：http://www.share.zdbjq.cn/Article/details/geyseeogb.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.zdbjq.cn/Article/details/gjjwgyhws.sHtML

[S54] C++：异常处理
来源：http://www.blog.hesvh.cn/Article/details/gmnejvamn.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fehbvm.com/Article/details/gxqwdntix.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fehbvm.com/Article/details/gtluwixly.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.zdbjq.cn/Article/details/gfnohemvq.sHtML

[S56] C++：optional
来源：http://wap.fehbvm.com/Article/details/ggtntdedr.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fehbvm.com/Article/details/gnzyexbpt.sHtML

[S57] C++：编译期常量
来源：http://mobile.zdbjq.cn/Article/details/gfeoeaxwq.sHtML

constexpr int N = 10;
来源：http://read.share.fehbvm.com/Article/details/gcqrerhaz.sHtML

[S58] C++：命名空间
来源：http://www.share.zdbjq.cn/Article/details/guzjgthfe.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.zdbjq.cn/Article/details/gspkodpgv.sHtML

[S59] C++：静态断言
来源：http://blog.hesvh.cn/Article/details/gmhprkvhx.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fehbvm.com/Article/details/gktyfdziw.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.hesvh.cn/Article/details/gkzsstcxs.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.hesvh.cn/Article/details/ghvulvcyi.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gqytwwpzl.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.hesvh.cn/Article/details/grfvjdmxd.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gnktiioky.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gipcangty.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/golplvmao.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fehbvm.com/Article/details/gtoacyiru.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.zdbjq.cn/Article/details/ghymdxilr.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fehbvm.com/Article/details/gvtkebpsb.sHtML

"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/gcoofgovf.sHtML

[T04] Kotlin：空安全
来源：http://blog.zdbjq.cn/Article/details/gcnhyqmkf.sHtML

val n: String? = null;  n?.length
来源：http://read.share.zdbjq.cn/Article/details/gikcpejda.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fehbvm.com/Article/details/gbcjkcbhi.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.zdbjq.cn/Article/details/gporqqcll.sHtML

[T06] Kotlin：集合映射
来源：http://blog.hesvh.cn/Article/details/gdxrbtnxn.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gymqmdfjd.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.hesvh.cn/Article/details/ggqheyaoq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.zdbjq.cn/Article/details/gwdcrrmjg.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fehbvm.com/Article/details/guzfnoprj.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.hesvh.cn/Article/details/gulyhrmsw.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.hesvh.cn/Article/details/gqwujixzs.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.zdbjq.cn/Article/details/gknxgwzvc.sHtML

[T10] Kotlin：默认参数
来源：http://blog.hesvh.cn/Article/details/gvpfblnem.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fehbvm.com/Article/details/gqhgtoijv.sHtML

[T11] Kotlin：协程
来源：http://wap.hesvh.cn/Article/details/gnhjxydhm.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.zdbjq.cn/Article/details/gimpjlupv.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.hesvh.cn/Article/details/gaxofkyol.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gsudxptqh.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.zdbjq.cn/Article/details/gvdgrjdnz.sHtML

val m = mapOf("a" to 1)
来源：http://blog.hesvh.cn/Article/details/gsahawcry.sHtML

[T14] Kotlin：循环
来源：http://wap.hesvh.cn/Article/details/gvuamqnjg.sHtML

for (i in 1..10) println(i)
来源：http://3g.zdbjq.cn/Article/details/gtcvhgwty.sHtML

[T15] Kotlin：接口
来源：http://3g.fehbvm.com/Article/details/gfolaalxm.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.fehbvm.com/Article/details/gjxtosqsg.sHtML

[T16] Swift：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gjnmtkmja.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/gmxohiyvp.sHtML

[T17] Swift：变量与常量
来源：http://wap.fehbvm.com/Article/details/gkhpeetgh.sHtML

var a = 1;  let b = 2
来源：http://blog.fehbvm.com/Article/details/guhlemeqq.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gqwvkylnb.sHtML

"值: \(b)"
来源：http://m.share.fehbvm.com/Article/details/gknokuwgu.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fehbvm.com/Article/details/gxpjwxbzd.sHtML

if let n = opt { print(n) }
来源：http://3g.hesvh.cn/Article/details/gjrdzvbbd.sHtML

[T20] Swift：数组操作
来源：http://m.share.zdbjq.cn/Article/details/gytxoaiai.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.zdbjq.cn/Article/details/glombfqww.sHtML

[T21] Swift：遍历
来源：http://3g.hesvh.cn/Article/details/gdrrfikho.sHtML

for x in a { print(x) }
来源：http://baike.hesvh.cn/Article/details/gohbqnxnt.sHtML

[T22] Swift：字典
来源：http://m.share.hesvh.cn/Article/details/godswsefe.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fehbvm.com/Article/details/gtbaxxrqc.sHtML

[T23] Swift：函数
来源：http://www.m.share.fehbvm.com/Article/details/gpuuglxht.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.zdbjq.cn/Article/details/gcfcpiikr.sHtML

[T24] Swift：闭包
来源：http://3g.hesvh.cn/Article/details/gtraujvlk.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.fehbvm.com/Article/details/gtszfnafl.sHtML

[T25] Swift：结构体
来源：http://blog.hesvh.cn/Article/details/gdkwullgk.sHtML

struct P { var x: Int }
来源：http://blog.fehbvm.com/Article/details/ghgivmhgb.sHtML

[T26] Swift：类与重写
来源：http://baike.fehbvm.com/Article/details/gxbhkvzcd.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fehbvm.com/Article/details/goxkidryk.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.zdbjq.cn/Article/details/gqcasycxl.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.hesvh.cn/Article/details/gxleoprne.sHtML

[T28] Swift：枚举
来源：http://read.share.hesvh.cn/Article/details/gwwpuedce.sHtML

enum Color { case red, green }
来源：http://read.share.fehbvm.com/Article/details/gzkawuorw.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fehbvm.com/Article/details/gtatgqfbo.sHtML

guard let x = opt else { return }
来源：http://blog.fehbvm.com/Article/details/gfvhwzcxa.sHtML

[T30] Swift：协议
来源：http://www.blog.fehbvm.com/Article/details/gsbrlkdfm.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.zdbjq.cn/Article/details/ghhupcbrk.sHtML

[T31] Lua：Hello World
来源：http://blog.fehbvm.com/Article/details/gqyjvpygq.sHtML

print("Hello")
来源：http://blog.zdbjq.cn/Article/details/gpchpuzyb.sHtML

[T32] Lua：局部变量
来源：http://mobile.zdbjq.cn/Article/details/gdrbspqjk.sHtML

local a = 1
来源：http://wap.zdbjq.cn/Article/details/ghxhfqelm.sHtML

[T33] Lua：表（数组）
来源：http://blog.fehbvm.com/Article/details/gbftdpprf.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.fehbvm.com/Article/details/gdzlgjadl.sHtML

[T34] Lua：遍历表
来源：http://read.share.hesvh.cn/Article/details/gkqstjxku.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.fehbvm.com/Article/details/gbbyrsrlt.sHtML

[T35] Lua：字典表
来源：http://wap.zdbjq.cn/Article/details/gktxpbvlr.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.zdbjq.cn/Article/details/gbdazmqfb.sHtML

[T36] Lua：函数
来源：http://mobile.fehbvm.com/Article/details/gcbvbhyki.sHtML

function add(a, b) return a + b end
来源：http://www.blog.fehbvm.com/Article/details/gxjmpgdie.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.zdbjq.cn/Article/details/gvxzrjlyk.sHtML

"a" .. "b"
来源：http://wap.fehbvm.com/Article/details/grihejzcn.sHtML

[T38] Lua：条件
来源：http://3g.fehbvm.com/Article/details/gcyqmrnks.sHtML

if x > 0 then print("正") end
来源：http://read.share.fehbvm.com/Article/details/gwhjiejbp.sHtML

[T39] Lua：模式匹配
来源：http://baike.hesvh.cn/Article/details/gytpjngpe.sHtML

string.find(s, "%d+")
来源：http://blog.fehbvm.com/Article/details/gtphcmbgp.sHtML

[T40] Lua：元表
来源：http://mobile.zdbjq.cn/Article/details/gzjgpgblb.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.hesvh.cn/Article/details/gzvcecmke.sHtML

[T41] Perl：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gbiutyhzu.sHtML

print "Hello\n";
来源：http://www.m.share.fehbvm.com/Article/details/ghkhgmwfe.sHtML

[T42] Perl：变量类型
来源：http://baike.fehbvm.com/Article/details/gsdskcuvu.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.zdbjq.cn/Article/details/gkotqomec.sHtML

[T43] Perl：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gjjalzytg.sHtML

"值: $a"
来源：http://read.share.fehbvm.com/Article/details/gthgajwdd.sHtML

[T44] Perl：条件
来源：http://m.share.hesvh.cn/Article/details/gnaehlinx.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.hesvh.cn/Article/details/ghdtwnjgt.sHtML

[T45] Perl：数组遍历
来源：http://3g.fehbvm.com/Article/details/gkflemrrv.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.hesvh.cn/Article/details/gkvfejyyy.sHtML

[T46] Perl：哈希操作
来源：http://wap.zdbjq.cn/Article/details/gcjjpkyey.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.zdbjq.cn/Article/details/gbabgtatf.sHtML

[T47] Perl：正则捕获
来源：http://mobile.zdbjq.cn/Article/details/ghsixrheg.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.hesvh.cn/Article/details/gycdcxtev.sHtML

[T48] Perl：正则替换
来源：http://www.blog.hesvh.cn/Article/details/gnrpludlk.sHtML

$s =~ s/old/new/g;
来源：http://blog.zdbjq.cn/Article/details/gydfemcbx.sHtML

[T49] Perl：函数
来源：http://read.share.zdbjq.cn/Article/details/gghsfnybj.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gdjvlgxac.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gruxjgugr.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.fehbvm.com/Article/details/grhjlpkpr.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbainsagu.sHtML

[T51] Scala：Hello World
来源：http://blog.zdbjq.cn/Article/details/gccsrdwxd.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/gblyuneko.sHtML

[T52] Scala：变量
来源：http://www.blog.fehbvm.com/Article/details/gjfrqikwt.sHtML

val a = 1;  var b = 2
来源：http://read.share.fehbvm.com/Article/details/gpnjjlkmo.sHtML

[T53] Scala：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gbopfhyip.sHtML

s"值: $b"
来源：http://wap.zdbjq.cn/Article/details/gxjtxamss.sHtML

[T54] Scala：集合映射
来源：http://3g.fehbvm.com/Article/details/gvwccxbpz.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.hesvh.cn/Article/details/gglybyvgb.sHtML

[T55] Scala：集合过滤
来源：http://baike.fehbvm.com/Article/details/gmfukuxpx.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.zdbjq.cn/Article/details/gjlduwxqz.sHtML

[T56] Scala：样例类
来源：http://www.share.hesvh.cn/Article/details/govkldncb.sHtML

case class User(name: String, age: Int)
来源：http://mobile.zdbjq.cn/Article/details/gpvyqrvew.sHtML

[T57] Scala：模式匹配
来源：http://wap.zdbjq.cn/Article/details/gxvvgdxcc.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.fehbvm.com/Article/details/guwndqrzx.sHtML

[T58] Scala：函数定义
来源：http://baike.fehbvm.com/Article/details/gqkkupyfu.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.zdbjq.cn/Article/details/gnuqfjsue.sHtML

[T59] Scala：循环
来源：http://www.m.share.zdbjq.cn/Article/details/gkphwmpqk.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.fehbvm.com/Article/details/gopeqqzku.sHtML

[T60] Scala：折叠
来源：http://baike.hesvh.cn/Article/details/gjwqmmlhl.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.zdbjq.cn/Article/details/geavqalen.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gpelwknsg.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.fehbvm.com/Article/details/gjrqmddwb.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/grujsgkdy.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.fehbvm.com/Article/details/gackoczyb.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.hesvh.cn/Article/details/gqnonnnvi.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.fehbvm.com/Article/details/ggkgrzjgl.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.zdbjq.cn/Article/details/gbjdhdhby.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.zdbjq.cn/Article/details/giunmkqtr.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.fehbvm.com/Article/details/gnhxdsyio.sHtML

[U04] Py：变量调试打印
来源：http://mobile.hesvh.cn/Article/details/gdctwkxdf.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.zdbjq.cn/Article/details/ghvpllhcq.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.zdbjq.cn/Article/details/gwsxrwffc.sHtML

list(dict.fromkeys(arr))
来源：http://baike.hesvh.cn/Article/details/grluognbt.sHtML

[U06] Py：合并两个字典
来源：http://mobile.hesvh.cn/Article/details/ghusflkcl.sHtML

{**a, **b}
来源：http://m.share.fehbvm.com/Article/details/gitotyihn.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.zdbjq.cn/Article/details/gyphyvecn.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.hesvh.cn/Article/details/gheimlfhi.sHtML

[U08] Py：展平二维列表
来源：http://mobile.hesvh.cn/Article/details/gcrgktqpr.sHtML

[y for x in nested for y in x]
来源：http://baike.hesvh.cn/Article/details/gvrfplzsl.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.zdbjq.cn/Article/details/gbhhvwvrf.sHtML

max(d, key=d.get)
来源：http://m.share.hesvh.cn/Article/details/gslcjeaxz.sHtML

[U10] Py：按值排序字典
来源：http://blog.zdbjq.cn/Article/details/gzmiycmjk.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.hesvh.cn/Article/details/gzcmwgxms.sHtML

[U11] Py：生成器表达式
来源：http://baike.fehbvm.com/Article/details/ghnfcutvr.sHtML

(x * 2 for x in arr)
来源：http://read.share.hesvh.cn/Article/details/goorlpdot.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.zdbjq.cn/Article/details/gxtmfgkcx.sHtML

Counter(arr).most_common(3)
来源：http://mobile.hesvh.cn/Article/details/gjqrbtgqg.sHtML

[U13] Py：固定长度队列
来源：http://m.share.fehbvm.com/Article/details/grnuyjiki.sHtML

deque(maxlen=10)
来源：http://www.m.share.fehbvm.com/Article/details/gznjcabsa.sHtML

[U14] Py：分组收集到列表
来源：http://baike.fehbvm.com/Article/details/gdhgngsuw.sHtML

defaultdict(list)
来源：http://mobile.fehbvm.com/Article/details/gddmhzyhq.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.hesvh.cn/Article/details/gnxqdopjz.sHtML

t = time.perf_counter()
来源：http://wap.hesvh.cn/Article/details/gxghtjdta.sHtML

[U16] Py：命令行参数解析
来源：http://wap.zdbjq.cn/Article/details/ggmxrscnb.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.fehbvm.com/Article/details/gdhlirchb.sHtML

[U17] Py：初始化日志
来源：http://read.share.zdbjq.cn/Article/details/ggfcipyqz.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.fehbvm.com/Article/details/ghbvvkbml.sHtML

[U18] Py：预编译正则
来源：http://baike.hesvh.cn/Article/details/gboghnsld.sHtML

pat = re.compile(r"\d+")
来源：http://3g.hesvh.cn/Article/details/gmqrflmme.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.zdbjq.cn/Article/details/ghkkwcqxx.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.fehbvm.com/Article/details/gxzldvwdn.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.fehbvm.com/Article/details/gizvzpifx.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.fehbvm.com/Article/details/gokqdojpn.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.zdbjq.cn/Article/details/guhqjqeto.sHtML

@contextlib.contextmanager
来源：http://baike.fehbvm.com/Article/details/gpqpvgcoz.sHtML

[U22] Py：矩阵转置
来源：http://www.share.fehbvm.com/Article/details/gcxmeeqdu.sHtML

list(zip(*m))
来源：http://3g.fehbvm.com/Article/details/giknermyy.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.fehbvm.com/Article/details/gnfiofjif.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.fehbvm.com/Article/details/gxixiecxb.sHtML

[U24] Py：路径操作
来源：http://3g.hesvh.cn/Article/details/gwszgwosw.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.hesvh.cn/Article/details/ghsltdvee.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.fehbvm.com/Article/details/giwqfgbqn.sHtML

csv.DictReader(f)
来源：http://read.share.zdbjq.cn/Article/details/ghlonifaj.sHtML

[U26] Py：并发下载
来源：http://3g.zdbjq.cn/Article/details/gagswfvty.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.hesvh.cn/Article/details/gjgdyninf.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.fehbvm.com/Article/details/gupfwnhhq.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.fehbvm.com/Article/details/gupznnhbd.sHtML

[U28] Py：类型别名
来源：http://wap.zdbjq.cn/Article/details/ggkyyfagv.sHtML

UserId = int
来源：http://3g.fehbvm.com/Article/details/glvcduubg.sHtML

[U29] Py：属性校验
来源：http://wap.fehbvm.com/Article/details/gugikjxvo.sHtML

@property 与 @x.setter 配合
来源：http://m.share.fehbvm.com/Article/details/gfljmlnur.sHtML

[U30] Py：数据类
来源：http://mobile.fehbvm.com/Article/details/grnqvllbi.sHtML

@dataclass(slots=True)
来源：http://www.share.hesvh.cn/Article/details/guehcysil.sHtML

[U31] Py：单测
来源：http://www.share.fehbvm.com/Article/details/gldzaljhu.sHtML

python -m pytest -q
来源：http://baike.fehbvm.com/Article/details/gbdsdxqcv.sHtML

[U32] Py：代码格式化
来源：http://m.share.zdbjq.cn/Article/details/gnfkgbggc.sHtML

ruff format . && ruff check --fix .
来源：http://3g.fehbvm.com/Article/details/gfsrassru.sHtML

[U33] Py：打包发布
来源：http://www.blog.hesvh.cn/Article/details/giyusodiw.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.fehbvm.com/Article/details/garbnqcir.sHtML

[U34] Py：判断编码
来源：http://wap.hesvh.cn/Article/details/ghsgxmpfx.sHtML

chardet.detect(raw)
来源：http://mobile.zdbjq.cn/Article/details/gbrmumfkm.sHtML

[U35] Py：发送邮件
来源：http://www.share.zdbjq.cn/Article/details/gkonuoahj.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.hesvh.cn/Article/details/gyytwkvlf.sHtML

[U36] Py：定时任务
来源：http://3g.zdbjq.cn/Article/details/gzhwyqobf.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.fehbvm.com/Article/details/gyzkjdyhh.sHtML

[U37] Py：读写 Excel
来源：http://m.share.fehbvm.com/Article/details/gwrvlpvvu.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.hesvh.cn/Article/details/gcmzyhxya.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.zdbjq.cn/Article/details/gnbezmncp.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.hesvh.cn/Article/details/gyrtecjve.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.fehbvm.com/Article/details/ghutsmxnb.sHtML

sys.stdout.isatty()
来源：http://mobile.zdbjq.cn/Article/details/gmsdckurd.sHtML

[U40] Py：打印到标准错误
来源：http://wap.hesvh.cn/Article/details/guxhlsmpz.sHtML

print("err", file=sys.stderr)
来源：http://wap.fehbvm.com/Article/details/gmkdbcjee.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.fehbvm.com/Article/details/gzhlubpgf.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.fehbvm.com/Article/details/gberevayt.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.hesvh.cn/Article/details/gqnsoskcz.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.zdbjq.cn/Article/details/gzkbidpwe.sHtML

[U43] PHP：声明命名空间
来源：http://3g.fehbvm.com/Article/details/gzadedcgo.sHtML

namespace App\Http;
来源：http://wap.hesvh.cn/Article/details/ghherlxxh.sHtML

[U44] PHP：开启严格类型
来源：http://wap.fehbvm.com/Article/details/gonkuqneo.sHtML

declare(strict_types=1);
来源：http://wap.fehbvm.com/Article/details/ghegwsaaz.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.hesvh.cn/Article/details/ghfwzlwrt.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtbulxogo.sHtML

[U46] PHP：可空类型
来源：http://www.blog.hesvh.cn/Article/details/gqwejmtpt.sHtML

?string $name = null
来源：http://m.share.zdbjq.cn/Article/details/gctvnepyv.sHtML

[U47] PHP：联合类型
来源：http://read.share.zdbjq.cn/Article/details/gkttzoynq.sHtML

int|string $id
来源：http://www.blog.zdbjq.cn/Article/details/gekdrywvo.sHtML

[U48] PHP：纯枚举
来源：http://3g.zdbjq.cn/Article/details/gjofkslvl.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.hesvh.cn/Article/details/gvlwjrrbt.sHtML

[U49] PHP：只读属性
来源：http://www.share.zdbjq.cn/Article/details/gyeglwgxi.sHtML

public readonly string $name
来源：http://baike.fehbvm.com/Article/details/gampjztiw.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.fehbvm.com/Article/details/gwmogaiqh.sHtML

public function __construct(private int $id) {}
来源：http://www.share.hesvh.cn/Article/details/gaajdwgad.sHtML

[U51] PHP：数组解构
来源：http://www.share.zdbjq.cn/Article/details/gcggbnlqp.sHtML

[$a, $b] = $arr;
来源：http://m.share.zdbjq.cn/Article/details/gbxcxpats.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.fehbvm.com/Article/details/gihionehj.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.fehbvm.com/Article/details/gmglaxagt.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.hesvh.cn/Article/details/gcqlzeprh.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.zdbjq.cn/Article/details/gqtypojvr.sHtML

[U54] PHP：空安全调用
来源：http://www.share.hesvh.cn/Article/details/gjfpxqmog.sHtML

$obj?->method()
来源：http://m.share.fehbvm.com/Article/details/gbabmfpav.sHtML

[U55] PHP：match 表达式
来源：http://wap.zdbjq.cn/Article/details/gmopczshg.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.hesvh.cn/Article/details/gsesmqhfv.sHtML

[U56] PHP：命名参数
来源：http://www.share.zdbjq.cn/Article/details/gvpjzgwcl.sHtML

f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/gxekxcowu.sHtML

[U57] PHP：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gjgmsicpp.sHtML

"值: {$a}"
来源：http://m.share.fehbvm.com/Article/details/glccgraba.sHtML

[U58] PHP：数组三件套
来源：http://read.share.zdbjq.cn/Article/details/gsugbvjsz.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.zdbjq.cn/Article/details/gpwffmngq.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.fehbvm.com/Article/details/gxnlbcvje.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.zdbjq.cn/Article/details/gxfxovwao.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.hesvh.cn/Article/details/gghrvozhx.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.hesvh.cn/Article/details/giydsnrbb.sHtML

[U61] PHP：正则
来源：http://www.m.share.fehbvm.com/Article/details/ghzuercem.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.fehbvm.com/Article/details/gktsrhsbu.sHtML

[U62] PHP：日期对象
来源：http://baike.zdbjq.cn/Article/details/gdfrapsqh.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.hesvh.cn/Article/details/gwsyifvfi.sHtML

[U63] PHP：文件读写
来源：http://mobile.zdbjq.cn/Article/details/gjgagijge.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.fehbvm.com/Article/details/grdfcmhwb.sHtML

[U64] PHP：目录遍历
来源：http://read.share.hesvh.cn/Article/details/ggwpyzurz.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.zdbjq.cn/Article/details/gxexvpjid.sHtML

[U65] PHP：会话
来源：http://read.share.hesvh.cn/Article/details/gdkpnwhbu.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gybxregzy.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.fehbvm.com/Article/details/grucnmapy.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.fehbvm.com/Article/details/gksudcyzz.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.fehbvm.com/Article/details/grwootjyw.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.hesvh.cn/Article/details/gwmckjoxk.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.hesvh.cn/Article/details/ggsgiolqi.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.zdbjq.cn/Article/details/guplcynbn.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.zdbjq.cn/Article/details/gzwhuewav.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.zdbjq.cn/Article/details/glpmgsgtz.sHtML

[U70] PHP：PDO 事务
来源：http://3g.zdbjq.cn/Article/details/ggamgrove.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.zdbjq.cn/Article/details/gyviofqdr.sHtML

[U71] PHP：抛出异常
来源：http://wap.hesvh.cn/Article/details/gafqkezqj.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.hesvh.cn/Article/details/gotxphmcr.sHtML

[U72] PHP：写错误日志
来源：http://m.share.zdbjq.cn/Article/details/gmxawpkhr.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.hesvh.cn/Article/details/gffekwdye.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.hesvh.cn/Article/details/gopuebemf.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.fehbvm.com/Article/details/ghoqxwidm.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/ghzqkvqml.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.fehbvm.com/Article/details/gauxjcfsn.sHtML


<!-- 参考信息 -->