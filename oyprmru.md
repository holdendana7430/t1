代发 wailian999

while (std::getline(in, line)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gvgkwbznk.sHtML

[S49] C++：写文件
来源：http://m.share.zdbjq.cn/Article/details/gbjglihzo.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fehbvm.com/Article/details/gyxfzglek.sHtML

[S50] C++：格式化数字
来源：http://3g.hesvh.cn/Article/details/ghrmmmhrp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gfycviasx.sHtML

[S51] C++：显式类型转换
来源：http://blog.fehbvm.com/Article/details/guukfycbd.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.zdbjq.cn/Article/details/grqsfhhss.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.hesvh.cn/Article/details/ghgykkksa.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fehbvm.com/Article/details/gyyebgdpq.sHtML

[S53] C++：移动语义
来源：http://www.m.share.hesvh.cn/Article/details/ghazyqrsf.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.hesvh.cn/Article/details/gwucbhfwo.sHtML

[S54] C++：异常处理
来源：http://m.share.fehbvm.com/Article/details/gcxncidir.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fehbvm.com/Article/details/gnokablbi.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.zdbjq.cn/Article/details/gulletwyf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.hesvh.cn/Article/details/gciklrfja.sHtML

[S56] C++：optional
来源：http://mobile.hesvh.cn/Article/details/gyyjhtonr.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.hesvh.cn/Article/details/gayufofxa.sHtML

[S57] C++：编译期常量
来源：http://www.blog.hesvh.cn/Article/details/gyqaqfkhm.sHtML

constexpr int N = 10;
来源：http://read.share.zdbjq.cn/Article/details/gwlkmylap.sHtML

[S58] C++：命名空间
来源：http://3g.fehbvm.com/Article/details/gwskkmcot.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.hesvh.cn/Article/details/gytqmxpqv.sHtML

[S59] C++：静态断言
来源：http://wap.hesvh.cn/Article/details/gqqzonnhr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fehbvm.com/Article/details/gybylpxdi.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.zdbjq.cn/Article/details/gydnugvkk.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/gdfaiceqs.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gcnqhwyrz.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.hesvh.cn/Article/details/gjoevybaz.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gddepxgws.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fehbvm.com/Article/details/gnexqfeqo.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/gxaayvspb.sHtML

[T02] Kotlin：变量
来源：http://m.share.fehbvm.com/Article/details/gdtsxyvav.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.zdbjq.cn/Article/details/gozrijunk.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.hesvh.cn/Article/details/gwzraiqsn.sHtML

"值: $b"
来源：http://mobile.hesvh.cn/Article/details/gsolgzbqv.sHtML

[T04] Kotlin：空安全
来源：http://blog.fehbvm.com/Article/details/ghqllrzhc.sHtML

val n: String? = null;  n?.length
来源：http://blog.fehbvm.com/Article/details/gkcbfnkso.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.hesvh.cn/Article/details/gkvjnpnnk.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.zdbjq.cn/Article/details/gqwwbdumg.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.hesvh.cn/Article/details/gnqvsckan.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fehbvm.com/Article/details/gpycmivbb.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.hesvh.cn/Article/details/gmuyvilju.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.hesvh.cn/Article/details/gtnkgeigx.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fehbvm.com/Article/details/gdbxrzklj.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.zdbjq.cn/Article/details/gnovtpftp.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fehbvm.com/Article/details/grjzzflzq.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.zdbjq.cn/Article/details/gnxobxazq.sHtML

[T10] Kotlin：默认参数
来源：http://baike.hesvh.cn/Article/details/ghiswewuo.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.hesvh.cn/Article/details/ghdqsjajm.sHtML

[T11] Kotlin：协程
来源：http://wap.zdbjq.cn/Article/details/gjnguxxli.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.zdbjq.cn/Article/details/gffqlkcmq.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.zdbjq.cn/Article/details/goybpjkii.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gnhvzikwd.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.hesvh.cn/Article/details/godssoqvz.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.hesvh.cn/Article/details/gpzgjyazy.sHtML

[T14] Kotlin：循环
来源：http://www.blog.hesvh.cn/Article/details/govnfwfiv.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/guybimsfv.sHtML

[T15] Kotlin：接口
来源：http://blog.hesvh.cn/Article/details/gtvpedmgv.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.hesvh.cn/Article/details/glbbqafob.sHtML

[T16] Swift：Hello World
来源：http://wap.zdbjq.cn/Article/details/gjcycyuar.sHtML

print("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/guaygamcl.sHtML

[T17] Swift：变量与常量
来源：http://baike.zdbjq.cn/Article/details/gwahzmudi.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.hesvh.cn/Article/details/gyyuvoxxt.sHtML

[T18] Swift：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gcyjhcrij.sHtML

"值: \(b)"
来源：http://read.share.zdbjq.cn/Article/details/gezwbrwlv.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fehbvm.com/Article/details/glxavfwbi.sHtML

if let n = opt { print(n) }
来源：http://blog.hesvh.cn/Article/details/ghifyvtjt.sHtML

[T20] Swift：数组操作
来源：http://read.share.hesvh.cn/Article/details/govwgrjkl.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.zdbjq.cn/Article/details/gnuitvdhi.sHtML

[T21] Swift：遍历
来源：http://mobile.fehbvm.com/Article/details/gdtdhhfhy.sHtML

for x in a { print(x) }
来源：http://www.share.zdbjq.cn/Article/details/gmtrsnzvj.sHtML

[T22] Swift：字典
来源：http://www.share.fehbvm.com/Article/details/gkqlvvusx.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.zdbjq.cn/Article/details/ggjvmkxla.sHtML

[T23] Swift：函数
来源：http://www.share.fehbvm.com/Article/details/gvkoqkotn.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.zdbjq.cn/Article/details/gwettslnx.sHtML

[T24] Swift：闭包
来源：http://mobile.hesvh.cn/Article/details/gggcybnhq.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.fehbvm.com/Article/details/gfvokqywt.sHtML

[T25] Swift：结构体
来源：http://mobile.fehbvm.com/Article/details/gtrjlemlh.sHtML

struct P { var x: Int }
来源：http://3g.zdbjq.cn/Article/details/gudqnojns.sHtML

[T26] Swift：类与重写
来源：http://wap.hesvh.cn/Article/details/giasivmia.sHtML

class A: Base { override func f() {} }
来源：http://mobile.hesvh.cn/Article/details/gnkbwmlyd.sHtML

[T27] Swift：错误处理
来源：http://blog.hesvh.cn/Article/details/gpuxjszzz.sHtML

do { try f() } catch { print(error) }
来源：http://blog.hesvh.cn/Article/details/ghmixdmep.sHtML

[T28] Swift：枚举
来源：http://wap.hesvh.cn/Article/details/guamlojeu.sHtML

enum Color { case red, green }
来源：http://baike.zdbjq.cn/Article/details/goglqscuw.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.hesvh.cn/Article/details/glhzsqqlj.sHtML

guard let x = opt else { return }
来源：http://baike.zdbjq.cn/Article/details/gtvgdigpy.sHtML

[T30] Swift：协议
来源：http://www.share.fehbvm.com/Article/details/gbynnllmk.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fehbvm.com/Article/details/gqwpewxsk.sHtML

[T31] Lua：Hello World
来源：http://mobile.hesvh.cn/Article/details/gblppryjx.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/gxvjhmues.sHtML

[T32] Lua：局部变量
来源：http://read.share.zdbjq.cn/Article/details/gtfafoliv.sHtML

local a = 1
来源：http://www.blog.zdbjq.cn/Article/details/gqazokqsp.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.fehbvm.com/Article/details/gogembxkl.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.hesvh.cn/Article/details/giijcwyfe.sHtML

[T34] Lua：遍历表
来源：http://mobile.fehbvm.com/Article/details/gwcghdbra.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fehbvm.com/Article/details/gvuiybrgx.sHtML

[T35] Lua：字典表
来源：http://mobile.hesvh.cn/Article/details/gfpjdmazy.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.fehbvm.com/Article/details/gegxduadv.sHtML

[T36] Lua：函数
来源：http://mobile.fehbvm.com/Article/details/gaiyvkhrq.sHtML

function add(a, b) return a + b end
来源：http://m.share.hesvh.cn/Article/details/gsvngqrjl.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.hesvh.cn/Article/details/gzvmuiqrc.sHtML

"a" .. "b"
来源：http://blog.zdbjq.cn/Article/details/guluvwavr.sHtML

[T38] Lua：条件
来源：http://baike.hesvh.cn/Article/details/gxlkddrkz.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.zdbjq.cn/Article/details/gcfmgkkqx.sHtML

[T39] Lua：模式匹配
来源：http://baike.fehbvm.com/Article/details/gowxqpgoy.sHtML

string.find(s, "%d+")
来源：http://www.m.share.hesvh.cn/Article/details/gxqvzzirx.sHtML

[T40] Lua：元表
来源：http://wap.fehbvm.com/Article/details/gjzyzfooe.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.fehbvm.com/Article/details/giadmurav.sHtML

[T41] Perl：Hello World
来源：http://www.blog.hesvh.cn/Article/details/geurgdtvl.sHtML

print "Hello\n";
来源：http://blog.hesvh.cn/Article/details/gxyhzvlln.sHtML

[T42] Perl：变量类型
来源：http://wap.zdbjq.cn/Article/details/ggvngtohf.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.zdbjq.cn/Article/details/gojuillap.sHtML

[T43] Perl：字符串插值
来源：http://blog.zdbjq.cn/Article/details/ghzinkwdy.sHtML

"值: $a"
来源：http://wap.zdbjq.cn/Article/details/gqomfgfzo.sHtML

[T44] Perl：条件
来源：http://www.m.share.zdbjq.cn/Article/details/gyvdwwasc.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.zdbjq.cn/Article/details/gnqktdvff.sHtML

[T45] Perl：数组遍历
来源：http://mobile.fehbvm.com/Article/details/gkfscbrpl.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.hesvh.cn/Article/details/ggfeezuex.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.fehbvm.com/Article/details/ghffzulpo.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.fehbvm.com/Article/details/ghilcycbz.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.fehbvm.com/Article/details/gekvywbdm.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.hesvh.cn/Article/details/gxllkcqdv.sHtML

[T48] Perl：正则替换
来源：http://wap.zdbjq.cn/Article/details/gdziuezdk.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.zdbjq.cn/Article/details/gddctgmhc.sHtML

[T49] Perl：函数
来源：http://www.blog.zdbjq.cn/Article/details/gtzxqmfpg.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gylnksyal.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gskgusauk.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.zdbjq.cn/Article/details/gkvbfuqpt.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.zdbjq.cn/Article/details/ggtsvfmpm.sHtML

[T51] Scala：Hello World
来源：http://baike.fehbvm.com/Article/details/glttjywuo.sHtML

println("Hello")
来源：http://mobile.hesvh.cn/Article/details/gyyzsnffz.sHtML

[T52] Scala：变量
来源：http://m.share.zdbjq.cn/Article/details/gthghhmgl.sHtML

val a = 1;  var b = 2
来源：http://mobile.zdbjq.cn/Article/details/gnxddlnmm.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gowzsobkt.sHtML

s"值: $b"
来源：http://3g.fehbvm.com/Article/details/gsstgkwrg.sHtML

[T54] Scala：集合映射
来源：http://www.share.zdbjq.cn/Article/details/gaqfdaxcz.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/ggrakghlw.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gmhfzkwog.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.fehbvm.com/Article/details/guptdjohv.sHtML

[T56] Scala：样例类
来源：http://mobile.hesvh.cn/Article/details/glnamhqcr.sHtML

case class User(name: String, age: Int)
来源：http://baike.fehbvm.com/Article/details/gzbuchuul.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fehbvm.com/Article/details/gxpvqttka.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.hesvh.cn/Article/details/gfnkwjcpo.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.hesvh.cn/Article/details/gutreczwi.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.fehbvm.com/Article/details/gvhtzqhaw.sHtML

[T59] Scala：循环
来源：http://blog.zdbjq.cn/Article/details/gerrlyiwp.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.zdbjq.cn/Article/details/glubijtrh.sHtML

[T60] Scala：折叠
来源：http://read.share.hesvh.cn/Article/details/gtndrjnot.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fehbvm.com/Article/details/gpzpkmalh.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gyaskbctr.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.fehbvm.com/Article/details/gggjaaldw.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/guaksjklu.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.hesvh.cn/Article/details/gkckdhpcu.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.hesvh.cn/Article/details/geudnknjb.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.zdbjq.cn/Article/details/ggwznyyib.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fehbvm.com/Article/details/giugwabqd.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.zdbjq.cn/Article/details/gstfavqzr.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.hesvh.cn/Article/details/gmqwdmrgm.sHtML

[U04] Py：变量调试打印
来源：http://baike.fehbvm.com/Article/details/gsruxzvcu.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.zdbjq.cn/Article/details/gkvpsoweu.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.hesvh.cn/Article/details/gzphnvubq.sHtML

list(dict.fromkeys(arr))
来源：http://wap.hesvh.cn/Article/details/gquhdvuyf.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.fehbvm.com/Article/details/gtqnfdbjf.sHtML

{**a, **b}
来源：http://m.share.hesvh.cn/Article/details/ggqfffkbq.sHtML

[U07] Py：反转字典键值
来源：http://3g.fehbvm.com/Article/details/gpggpjvvw.sHtML

{v: k for k, v in d.items()}
来源：http://3g.zdbjq.cn/Article/details/ghrqtmyzf.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.fehbvm.com/Article/details/gyvoxkdnh.sHtML

[y for x in nested for y in x]
来源：http://mobile.hesvh.cn/Article/details/gapxkcvym.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.fehbvm.com/Article/details/ggwsitnmi.sHtML

max(d, key=d.get)
来源：http://m.share.fehbvm.com/Article/details/gcmcylkdb.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.fehbvm.com/Article/details/ghgsiiouh.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.zdbjq.cn/Article/details/guzbiwuzh.sHtML

[U11] Py：生成器表达式
来源：http://wap.zdbjq.cn/Article/details/ghwtcrxpm.sHtML

(x * 2 for x in arr)
来源：http://m.share.zdbjq.cn/Article/details/grxzjtvyx.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.zdbjq.cn/Article/details/glrxrduhq.sHtML

Counter(arr).most_common(3)
来源：http://read.share.fehbvm.com/Article/details/gsngaiapd.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.hesvh.cn/Article/details/gzaklbqsb.sHtML

deque(maxlen=10)
来源：http://baike.fehbvm.com/Article/details/gvpjsatys.sHtML

[U14] Py：分组收集到列表
来源：http://3g.fehbvm.com/Article/details/gkvkhvwnt.sHtML

defaultdict(list)
来源：http://read.share.hesvh.cn/Article/details/gsyxyqkpd.sHtML

[U15] Py：高精度计时
来源：http://www.blog.zdbjq.cn/Article/details/gesxinbdt.sHtML

t = time.perf_counter()
来源：http://baike.fehbvm.com/Article/details/gklpblvop.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.zdbjq.cn/Article/details/gddltrsll.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.fehbvm.com/Article/details/geaeizdvq.sHtML

[U17] Py：初始化日志
来源：http://www.blog.hesvh.cn/Article/details/gkxvzkiho.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.hesvh.cn/Article/details/gxxqwbqlw.sHtML

[U18] Py：预编译正则
来源：http://mobile.fehbvm.com/Article/details/gzdzyvkue.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.fehbvm.com/Article/details/gsvjopkva.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.hesvh.cn/Article/details/gtejbbyhe.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.zdbjq.cn/Article/details/ggymmkjde.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.zdbjq.cn/Article/details/gjwhiftxe.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.fehbvm.com/Article/details/gdecbmapw.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.zdbjq.cn/Article/details/gugkmrfhv.sHtML

@contextlib.contextmanager
来源：http://3g.hesvh.cn/Article/details/gfgoxrkwc.sHtML

[U22] Py：矩阵转置
来源：http://mobile.fehbvm.com/Article/details/gosonitlg.sHtML

list(zip(*m))
来源：http://blog.fehbvm.com/Article/details/gbjjilczb.sHtML

[U23] Py：分块读取大文件
来源：http://wap.zdbjq.cn/Article/details/gtgtjdnrm.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.zdbjq.cn/Article/details/ggkxzoxzc.sHtML

[U24] Py：路径操作
来源：http://mobile.zdbjq.cn/Article/details/godrinmoh.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.zdbjq.cn/Article/details/gfzhpppcf.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.fehbvm.com/Article/details/gyqtvdjkm.sHtML

csv.DictReader(f)
来源：http://wap.hesvh.cn/Article/details/ghlnzddew.sHtML

[U26] Py：并发下载
来源：http://baike.hesvh.cn/Article/details/gxgfwmvqa.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.fehbvm.com/Article/details/gkkbeefyo.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.fehbvm.com/Article/details/grynhngcy.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.fehbvm.com/Article/details/gxndwfycv.sHtML

[U28] Py：类型别名
来源：http://www.blog.zdbjq.cn/Article/details/gxxftgqia.sHtML

UserId = int
来源：http://www.m.share.hesvh.cn/Article/details/gbasghmbx.sHtML

[U29] Py：属性校验
来源：http://mobile.hesvh.cn/Article/details/gsczcskbc.sHtML

@property 与 @x.setter 配合
来源：http://wap.fehbvm.com/Article/details/gvnjkgusc.sHtML

[U30] Py：数据类
来源：http://m.share.hesvh.cn/Article/details/gcfgfapjg.sHtML

@dataclass(slots=True)
来源：http://3g.fehbvm.com/Article/details/gllllgoru.sHtML

[U31] Py：单测
来源：http://www.m.share.fehbvm.com/Article/details/gnbxyyupl.sHtML

python -m pytest -q
来源：http://3g.hesvh.cn/Article/details/gftgidrce.sHtML

[U32] Py：代码格式化
来源：http://baike.hesvh.cn/Article/details/gjxksrowx.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.hesvh.cn/Article/details/gvqerjjpu.sHtML

[U33] Py：打包发布
来源：http://www.m.share.hesvh.cn/Article/details/gqbsnamvy.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.zdbjq.cn/Article/details/grshyknfv.sHtML

[U34] Py：判断编码
来源：http://www.share.hesvh.cn/Article/details/gudsoihbc.sHtML

chardet.detect(raw)
来源：http://www.blog.zdbjq.cn/Article/details/gkukyzwdt.sHtML

[U35] Py：发送邮件
来源：http://3g.zdbjq.cn/Article/details/geytffwjj.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.zdbjq.cn/Article/details/gybpmzjip.sHtML

[U36] Py：定时任务
来源：http://m.share.zdbjq.cn/Article/details/gtsehrmcf.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.hesvh.cn/Article/details/gapfvwanr.sHtML

[U37] Py：读写 Excel
来源：http://wap.fehbvm.com/Article/details/gqntdhfbt.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.fehbvm.com/Article/details/gxzbgspag.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.hesvh.cn/Article/details/gwjwvlzxn.sHtML

Path(__file__).resolve().parent
来源：http://mobile.fehbvm.com/Article/details/gmmpmvajf.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.hesvh.cn/Article/details/gizuhdsrj.sHtML

sys.stdout.isatty()
来源：http://www.m.share.hesvh.cn/Article/details/gmvslckcb.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.hesvh.cn/Article/details/ggtemrbig.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.fehbvm.com/Article/details/gigdrsbme.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.hesvh.cn/Article/details/gkarsugih.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.zdbjq.cn/Article/details/glznxnizv.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.hesvh.cn/Article/details/gsugmthka.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.hesvh.cn/Article/details/gpwoikdkc.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.hesvh.cn/Article/details/gcydooktz.sHtML

namespace App\Http;
来源：http://mobile.hesvh.cn/Article/details/gyqxuhdoz.sHtML

[U44] PHP：开启严格类型
来源：http://blog.hesvh.cn/Article/details/geokenujq.sHtML

declare(strict_types=1);
来源：http://baike.hesvh.cn/Article/details/gkufzvhaf.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.zdbjq.cn/Article/details/grkogeowd.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gbrvhpyxr.sHtML

[U46] PHP：可空类型
来源：http://read.share.hesvh.cn/Article/details/gghwuuebd.sHtML

?string $name = null
来源：http://blog.hesvh.cn/Article/details/gdmreokql.sHtML

[U47] PHP：联合类型
来源：http://baike.zdbjq.cn/Article/details/gpmsmqclg.sHtML

int|string $id
来源：http://m.share.fehbvm.com/Article/details/gzevxqiii.sHtML

[U48] PHP：纯枚举
来源：http://blog.hesvh.cn/Article/details/gednigpal.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.fehbvm.com/Article/details/gpnglwsec.sHtML

[U49] PHP：只读属性
来源：http://blog.zdbjq.cn/Article/details/gthkdtkne.sHtML

public readonly string $name
来源：http://read.share.hesvh.cn/Article/details/glozqelhm.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.zdbjq.cn/Article/details/gbrzhuwdq.sHtML

public function __construct(private int $id) {}
来源：http://read.share.zdbjq.cn/Article/details/gitzmyfvq.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.hesvh.cn/Article/details/gxzrglvtr.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.fehbvm.com/Article/details/gipckopvm.sHtML

[U52] PHP：箭头函数
来源：http://blog.hesvh.cn/Article/details/guoachbkk.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.zdbjq.cn/Article/details/gcukxchsn.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.fehbvm.com/Article/details/gjhvyuzxe.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.zdbjq.cn/Article/details/gslajhvce.sHtML

[U54] PHP：空安全调用
来源：http://m.share.hesvh.cn/Article/details/gldvfoqmr.sHtML

$obj?->method()
来源：http://m.share.zdbjq.cn/Article/details/ghowmhlvg.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.zdbjq.cn/Article/details/gomsgigyu.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.hesvh.cn/Article/details/goyqvgvzy.sHtML

[U56] PHP：命名参数
来源：http://blog.hesvh.cn/Article/details/gqipforxu.sHtML

f(a: 1, b: 2)
来源：http://mobile.hesvh.cn/Article/details/gghvgypmc.sHtML

[U57] PHP：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gzzqfpisd.sHtML

"值: {$a}"
来源：http://wap.fehbvm.com/Article/details/gajgwnndn.sHtML

[U58] PHP：数组三件套
来源：http://baike.fehbvm.com/Article/details/gkhiwdcsv.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.fehbvm.com/Article/details/giocwwvyg.sHtML

[U59] PHP：自定义排序
来源：http://www.share.zdbjq.cn/Article/details/gzwvclpwg.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fehbvm.com/Article/details/goddajotw.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.hesvh.cn/Article/details/gmixktqcy.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.fehbvm.com/Article/details/gdfktolqn.sHtML

[U61] PHP：正则
来源：http://read.share.zdbjq.cn/Article/details/gkkdbxpds.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.fehbvm.com/Article/details/gideyrydi.sHtML

[U62] PHP：日期对象
来源：http://wap.fehbvm.com/Article/details/gwkgrbygf.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.hesvh.cn/Article/details/gqejdvdeg.sHtML

[U63] PHP：文件读写
来源：http://blog.zdbjq.cn/Article/details/gudtldytb.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.hesvh.cn/Article/details/gvqqloqyb.sHtML

[U64] PHP：目录遍历
来源：http://baike.hesvh.cn/Article/details/gnzcobopf.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.fehbvm.com/Article/details/ggjehfcpk.sHtML

[U65] PHP：会话
来源：http://3g.hesvh.cn/Article/details/gajglteae.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/guoicxkuz.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.hesvh.cn/Article/details/gieqkxdwt.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.hesvh.cn/Article/details/gmoaidigj.sHtML

[U67] PHP：处理文件上传
来源：http://blog.fehbvm.com/Article/details/gibummqor.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.hesvh.cn/Article/details/grrughrvq.sHtML

[U68] PHP：PDO 连接
来源：http://wap.fehbvm.com/Article/details/geucgirdo.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.hesvh.cn/Article/details/greabygkm.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.zdbjq.cn/Article/details/gkyxsierd.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.hesvh.cn/Article/details/guthnfrfv.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.hesvh.cn/Article/details/gbvlsvakg.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.fehbvm.com/Article/details/girnpqexm.sHtML

[U71] PHP：抛出异常
来源：http://m.share.zdbjq.cn/Article/details/gfrixcesq.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.hesvh.cn/Article/details/genuyftip.sHtML

[U72] PHP：写错误日志
来源：http://m.share.zdbjq.cn/Article/details/gdhskpekv.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.zdbjq.cn/Article/details/gtsyzmojg.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.hesvh.cn/Article/details/gwkiazjdt.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.fehbvm.com/Article/details/gwjmzbyca.sHtML

[U74] PHP：读取环境变量
来源：http://blog.fehbvm.com/Article/details/geqduykxw.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.fehbvm.com/Article/details/gcplezpqq.sHtML


<!-- 参考信息 -->