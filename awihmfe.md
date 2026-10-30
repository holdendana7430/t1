代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gdsgfzwxo.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.hesvh.cn/Article/details/glwkzqsqs.sHtML

[S48] C++：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gazidxdij.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fehbvm.com/Article/details/gfsnzeery.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fehbvm.com/Article/details/gryfpdone.sHtML

[S49] C++：写文件
来源：http://3g.fehbvm.com/Article/details/goqsfkykj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fehbvm.com/Article/details/gltcanvrn.sHtML

[S50] C++：格式化数字
来源：http://3g.fehbvm.com/Article/details/gpfezmgio.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fehbvm.com/Article/details/gsxzryavx.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fehbvm.com/Article/details/gazygcxja.sHtML

static_cast<double>(a) / b
来源：http://mobile.fehbvm.com/Article/details/gtxrpsgwu.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fehbvm.com/Article/details/gzjcnynwo.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fehbvm.com/Article/details/gtgiykbbb.sHtML

[S53] C++：移动语义
来源：http://www.blog.hesvh.cn/Article/details/gaurupuml.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.hesvh.cn/Article/details/gfqwxwlly.sHtML

[S54] C++：异常处理
来源：http://wap.fehbvm.com/Article/details/gknetwrwo.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.zdbjq.cn/Article/details/gzygmkhol.sHtML

[S55] C++：结构化绑定
来源：http://read.share.zdbjq.cn/Article/details/ganhlahti.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.hesvh.cn/Article/details/geqyntyjt.sHtML

[S56] C++：optional
来源：http://www.blog.zdbjq.cn/Article/details/gjnwagfrh.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.zdbjq.cn/Article/details/gnuafbkbi.sHtML

[S57] C++：编译期常量
来源：http://www.share.zdbjq.cn/Article/details/gussxtgyv.sHtML

constexpr int N = 10;
来源：http://mobile.zdbjq.cn/Article/details/gyerzpbps.sHtML

[S58] C++：命名空间
来源：http://blog.hesvh.cn/Article/details/gzohsmepz.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.zdbjq.cn/Article/details/gbsqxjzxq.sHtML

[S59] C++：静态断言
来源：http://m.share.hesvh.cn/Article/details/gunlvwswn.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.zdbjq.cn/Article/details/gwlnejukh.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.zdbjq.cn/Article/details/gkhmsyzea.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fehbvm.com/Article/details/gcrcldllt.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gwozntwyt.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fehbvm.com/Article/details/guluwcedl.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gwcjnvjai.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gnnjdyfkf.sHtML

println("Hello")
来源：http://blog.zdbjq.cn/Article/details/gzybcefqu.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.zdbjq.cn/Article/details/godygbcra.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.zdbjq.cn/Article/details/gzujnjkny.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.zdbjq.cn/Article/details/gxdlxemea.sHtML

"值: $b"
来源：http://www.share.fehbvm.com/Article/details/gxgttfoel.sHtML

[T04] Kotlin：空安全
来源：http://m.share.zdbjq.cn/Article/details/gdonjhkzm.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.hesvh.cn/Article/details/gnstdabfl.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.zdbjq.cn/Article/details/gesmksimh.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.hesvh.cn/Article/details/gmnrphqbk.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fehbvm.com/Article/details/gplgxdjry.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.zdbjq.cn/Article/details/gjcfxvgmk.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.hesvh.cn/Article/details/gbppddret.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fehbvm.com/Article/details/gfapseebw.sHtML

[T08] Kotlin：数据类
来源：http://www.share.hesvh.cn/Article/details/gdljljffg.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.zdbjq.cn/Article/details/gojprfdwz.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.zdbjq.cn/Article/details/gkpnuhksp.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.hesvh.cn/Article/details/geiuynijt.sHtML

[T10] Kotlin：默认参数
来源：http://3g.zdbjq.cn/Article/details/ggjwxiosj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.zdbjq.cn/Article/details/gigvtgagj.sHtML

[T11] Kotlin：协程
来源：http://baike.zdbjq.cn/Article/details/gvvfyyubi.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.zdbjq.cn/Article/details/giadqrecg.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fehbvm.com/Article/details/geeeoxsph.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/gjmyesego.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.zdbjq.cn/Article/details/gcwguewsd.sHtML

val m = mapOf("a" to 1)
来源：http://baike.hesvh.cn/Article/details/gpkcvjagj.sHtML

[T14] Kotlin：循环
来源：http://wap.zdbjq.cn/Article/details/gtuobrbmx.sHtML

for (i in 1..10) println(i)
来源：http://blog.fehbvm.com/Article/details/gvjfjbkar.sHtML

[T15] Kotlin：接口
来源：http://m.share.zdbjq.cn/Article/details/gphwpascv.sHtML

interface Shape { fun area(): Double }
来源：http://3g.zdbjq.cn/Article/details/gcuaplwqg.sHtML

[T16] Swift：Hello World
来源：http://m.share.zdbjq.cn/Article/details/globpewjr.sHtML

print("Hello")
来源：http://blog.fehbvm.com/Article/details/gtjpxesft.sHtML

[T17] Swift：变量与常量
来源：http://wap.hesvh.cn/Article/details/gswfleywi.sHtML

var a = 1;  let b = 2
来源：http://3g.hesvh.cn/Article/details/gwqglvruz.sHtML

[T18] Swift：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gdwhrjdbk.sHtML

"值: \(b)"
来源：http://wap.zdbjq.cn/Article/details/gmzhtzzbn.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fehbvm.com/Article/details/gttpznzqn.sHtML

if let n = opt { print(n) }
来源：http://blog.hesvh.cn/Article/details/gkodgvvpe.sHtML

[T20] Swift：数组操作
来源：http://read.share.zdbjq.cn/Article/details/gxonrvqgq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.hesvh.cn/Article/details/gxsmzgqmg.sHtML

[T21] Swift：遍历
来源：http://read.share.fehbvm.com/Article/details/grqwqqvgh.sHtML

for x in a { print(x) }
来源：http://baike.hesvh.cn/Article/details/gwlkhwcjt.sHtML

[T22] Swift：字典
来源：http://baike.zdbjq.cn/Article/details/gbgxudbfm.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.hesvh.cn/Article/details/getmvwfub.sHtML

[T23] Swift：函数
来源：http://mobile.zdbjq.cn/Article/details/gamilmaes.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.zdbjq.cn/Article/details/gghuphqvc.sHtML

[T24] Swift：闭包
来源：http://www.m.share.hesvh.cn/Article/details/govfjkutf.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.hesvh.cn/Article/details/guwqljsme.sHtML

[T25] Swift：结构体
来源：http://mobile.fehbvm.com/Article/details/gdlzuowxd.sHtML

struct P { var x: Int }
来源：http://wap.hesvh.cn/Article/details/gtaspiete.sHtML

[T26] Swift：类与重写
来源：http://mobile.hesvh.cn/Article/details/gywzmcvps.sHtML

class A: Base { override func f() {} }
来源：http://blog.zdbjq.cn/Article/details/gxqrkldxz.sHtML

[T27] Swift：错误处理
来源：http://blog.hesvh.cn/Article/details/gojazqjgw.sHtML

do { try f() } catch { print(error) }
来源：http://wap.hesvh.cn/Article/details/gsfikmksf.sHtML

[T28] Swift：枚举
来源：http://mobile.zdbjq.cn/Article/details/gcyrxhoii.sHtML

enum Color { case red, green }
来源：http://3g.fehbvm.com/Article/details/gcewgzktl.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.zdbjq.cn/Article/details/gfzemfmnz.sHtML

guard let x = opt else { return }
来源：http://m.share.zdbjq.cn/Article/details/grsxpsevq.sHtML

[T30] Swift：协议
来源：http://mobile.zdbjq.cn/Article/details/gsddbvwnd.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.hesvh.cn/Article/details/geylfksdy.sHtML

[T31] Lua：Hello World
来源：http://blog.hesvh.cn/Article/details/ghzwucytc.sHtML

print("Hello")
来源：http://blog.fehbvm.com/Article/details/gnmdzelvk.sHtML

[T32] Lua：局部变量
来源：http://wap.zdbjq.cn/Article/details/gfuetgfky.sHtML

local a = 1
来源：http://www.blog.hesvh.cn/Article/details/gvucpuqyj.sHtML

[T33] Lua：表（数组）
来源：http://wap.fehbvm.com/Article/details/gvowsboha.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.fehbvm.com/Article/details/guejiglxr.sHtML

[T34] Lua：遍历表
来源：http://3g.zdbjq.cn/Article/details/gkgutkzac.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.hesvh.cn/Article/details/gcwxvenub.sHtML

[T35] Lua：字典表
来源：http://read.share.fehbvm.com/Article/details/gowwzyerb.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.hesvh.cn/Article/details/gbhwlunpj.sHtML

[T36] Lua：函数
来源：http://www.m.share.fehbvm.com/Article/details/gfxjuzqmb.sHtML

function add(a, b) return a + b end
来源：http://www.share.hesvh.cn/Article/details/glvsqozwt.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.zdbjq.cn/Article/details/ggkwslfdo.sHtML

"a" .. "b"
来源：http://m.share.fehbvm.com/Article/details/gdaraftpj.sHtML

[T38] Lua：条件
来源：http://read.share.fehbvm.com/Article/details/gviqvyfcx.sHtML

if x > 0 then print("正") end
来源：http://www.share.fehbvm.com/Article/details/gapgjfawf.sHtML

[T39] Lua：模式匹配
来源：http://blog.hesvh.cn/Article/details/gbxdzcwyj.sHtML

string.find(s, "%d+")
来源：http://m.share.fehbvm.com/Article/details/gnnpnmfil.sHtML

[T40] Lua：元表
来源：http://baike.zdbjq.cn/Article/details/ggpfmhtge.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.zdbjq.cn/Article/details/gfiwouvwb.sHtML

[T41] Perl：Hello World
来源：http://baike.zdbjq.cn/Article/details/gocsfvrrr.sHtML

print "Hello\n";
来源：http://m.share.fehbvm.com/Article/details/gniawijgh.sHtML

[T42] Perl：变量类型
来源：http://wap.hesvh.cn/Article/details/grlyscctw.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.zdbjq.cn/Article/details/gbvocodvk.sHtML

[T43] Perl：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gmzytwqgk.sHtML

"值: $a"
来源：http://blog.hesvh.cn/Article/details/gbllebodv.sHtML

[T44] Perl：条件
来源：http://baike.hesvh.cn/Article/details/gyafopubr.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.fehbvm.com/Article/details/gdirvskms.sHtML

[T45] Perl：数组遍历
来源：http://mobile.zdbjq.cn/Article/details/gvvwxqssw.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.zdbjq.cn/Article/details/gnavqsbmn.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.fehbvm.com/Article/details/gilkiewkj.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.fehbvm.com/Article/details/gtyqipomh.sHtML

[T47] Perl：正则捕获
来源：http://blog.zdbjq.cn/Article/details/gpxnicnqq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.fehbvm.com/Article/details/gkfipbmby.sHtML

[T48] Perl：正则替换
来源：http://read.share.hesvh.cn/Article/details/gaofqsrla.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.fehbvm.com/Article/details/gmvquwyzk.sHtML

[T49] Perl：函数
来源：http://mobile.hesvh.cn/Article/details/gyxyaphuk.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gtiztzbtp.sHtML

[T50] Perl：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gnqdwuxbl.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.fehbvm.com/Article/details/ggqmxjjcc.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.fehbvm.com/Article/details/gtlgayldd.sHtML

[T51] Scala：Hello World
来源：http://mobile.fehbvm.com/Article/details/gxyjcgfip.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/gbuvqetcr.sHtML

[T52] Scala：变量
来源：http://read.share.fehbvm.com/Article/details/gzbiteyyy.sHtML

val a = 1;  var b = 2
来源：http://wap.zdbjq.cn/Article/details/ggyjkhagg.sHtML

[T53] Scala：字符串插值
来源：http://3g.hesvh.cn/Article/details/gpqrtmrob.sHtML

s"值: $b"
来源：http://wap.zdbjq.cn/Article/details/grnbgrhce.sHtML

[T54] Scala：集合映射
来源：http://3g.zdbjq.cn/Article/details/gmpslbfwn.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.fehbvm.com/Article/details/gjfucbpfl.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/gipxezlcd.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.fehbvm.com/Article/details/ghglbhajn.sHtML

[T56] Scala：样例类
来源：http://www.share.hesvh.cn/Article/details/gkwvozetl.sHtML

case class User(name: String, age: Int)
来源：http://read.share.zdbjq.cn/Article/details/gkyohdlfd.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.zdbjq.cn/Article/details/gpinvpnva.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.zdbjq.cn/Article/details/graheonpx.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.hesvh.cn/Article/details/gvaxobgbw.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.zdbjq.cn/Article/details/gjgflunrd.sHtML

[T59] Scala：循环
来源：http://www.share.fehbvm.com/Article/details/gvpuspade.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.zdbjq.cn/Article/details/gcaclafcp.sHtML

[T60] Scala：折叠
来源：http://blog.zdbjq.cn/Article/details/gchgtuipg.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.fehbvm.com/Article/details/gwsrgqggu.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gwdsjkgui.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.hesvh.cn/Article/details/gxithpkis.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gokivirdv.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.zdbjq.cn/Article/details/gkofgkuhq.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.hesvh.cn/Article/details/gysogwiap.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.fehbvm.com/Article/details/gpookfshp.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.zdbjq.cn/Article/details/guhgptqjj.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.fehbvm.com/Article/details/gyxzgvxhw.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.zdbjq.cn/Article/details/giqntdvbd.sHtML

[U04] Py：变量调试打印
来源：http://read.share.fehbvm.com/Article/details/goenphkdf.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.hesvh.cn/Article/details/gjtnfsmgd.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.fehbvm.com/Article/details/gzudlrfhi.sHtML

list(dict.fromkeys(arr))
来源：http://3g.zdbjq.cn/Article/details/glyzryqsj.sHtML

[U06] Py：合并两个字典
来源：http://wap.hesvh.cn/Article/details/gehgdhhwr.sHtML

{**a, **b}
来源：http://baike.fehbvm.com/Article/details/gqzkilwxm.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.fehbvm.com/Article/details/gmmsdwrhc.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.zdbjq.cn/Article/details/gtndvinuq.sHtML

[U08] Py：展平二维列表
来源：http://www.share.fehbvm.com/Article/details/gxiydbiak.sHtML

[y for x in nested for y in x]
来源：http://www.share.zdbjq.cn/Article/details/gotgezogu.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.hesvh.cn/Article/details/gbtdyjexe.sHtML

max(d, key=d.get)
来源：http://www.blog.hesvh.cn/Article/details/gkofwoszr.sHtML

[U10] Py：按值排序字典
来源：http://blog.fehbvm.com/Article/details/geuavegis.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.zdbjq.cn/Article/details/gdrnldbyq.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.hesvh.cn/Article/details/gcrslamno.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gahpgisau.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.fehbvm.com/Article/details/gyqayqgmg.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.hesvh.cn/Article/details/gxhlrshoj.sHtML

[U13] Py：固定长度队列
来源：http://m.share.hesvh.cn/Article/details/gjqrbmwwk.sHtML

deque(maxlen=10)
来源：http://www.blog.zdbjq.cn/Article/details/ggkfplrvl.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.hesvh.cn/Article/details/gymilkuxm.sHtML

defaultdict(list)
来源：http://wap.zdbjq.cn/Article/details/gtyirqiut.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.fehbvm.com/Article/details/gsfjyzuwe.sHtML

t = time.perf_counter()
来源：http://www.blog.zdbjq.cn/Article/details/ghxmosvpt.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.fehbvm.com/Article/details/gcjxiqfjf.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.zdbjq.cn/Article/details/gremovzgq.sHtML

[U17] Py：初始化日志
来源：http://www.blog.hesvh.cn/Article/details/guabbupmf.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.zdbjq.cn/Article/details/gnsmdaxlz.sHtML

[U18] Py：预编译正则
来源：http://3g.zdbjq.cn/Article/details/gazemlqmz.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.hesvh.cn/Article/details/gviiaoqun.sHtML

[U19] Py：正则替换带回调
来源：http://blog.fehbvm.com/Article/details/gtwywnqpo.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.fehbvm.com/Article/details/glcltvtka.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.zdbjq.cn/Article/details/gmzuntdpm.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.hesvh.cn/Article/details/gqfeazxzo.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.zdbjq.cn/Article/details/guxdcwbvf.sHtML

@contextlib.contextmanager
来源：http://read.share.zdbjq.cn/Article/details/ghdxquyyp.sHtML

[U22] Py：矩阵转置
来源：http://baike.hesvh.cn/Article/details/grxehouez.sHtML

list(zip(*m))
来源：http://www.blog.hesvh.cn/Article/details/gxaenxght.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.zdbjq.cn/Article/details/grfyxiiya.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.zdbjq.cn/Article/details/gxbyvvzbj.sHtML

[U24] Py：路径操作
来源：http://baike.zdbjq.cn/Article/details/gncntysea.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.zdbjq.cn/Article/details/gjoyqhqzs.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.fehbvm.com/Article/details/grllyflqf.sHtML

csv.DictReader(f)
来源：http://mobile.zdbjq.cn/Article/details/gyoytwjnb.sHtML

[U26] Py：并发下载
来源：http://3g.fehbvm.com/Article/details/gdryxjtgp.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.zdbjq.cn/Article/details/ggmphnupn.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.hesvh.cn/Article/details/gbajpahkk.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.fehbvm.com/Article/details/gjasuynmv.sHtML

[U28] Py：类型别名
来源：http://m.share.hesvh.cn/Article/details/gfmumhgeb.sHtML

UserId = int
来源：http://mobile.zdbjq.cn/Article/details/gtopvkqfm.sHtML

[U29] Py：属性校验
来源：http://m.share.fehbvm.com/Article/details/gihhhtxxi.sHtML

@property 与 @x.setter 配合
来源：http://m.share.hesvh.cn/Article/details/gkarefzfk.sHtML

[U30] Py：数据类
来源：http://m.share.hesvh.cn/Article/details/girhonsgf.sHtML

@dataclass(slots=True)
来源：http://m.share.zdbjq.cn/Article/details/gbzlndoyy.sHtML

[U31] Py：单测
来源：http://baike.zdbjq.cn/Article/details/gattzdmyw.sHtML

python -m pytest -q
来源：http://wap.fehbvm.com/Article/details/gvogjermp.sHtML

[U32] Py：代码格式化
来源：http://baike.zdbjq.cn/Article/details/gdtoopjrd.sHtML

ruff format . && ruff check --fix .
来源：http://baike.fehbvm.com/Article/details/gqgxqheqz.sHtML

[U33] Py：打包发布
来源：http://wap.fehbvm.com/Article/details/gxszwuvin.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.zdbjq.cn/Article/details/glipliwht.sHtML

[U34] Py：判断编码
来源：http://blog.fehbvm.com/Article/details/gcntbwgrr.sHtML

chardet.detect(raw)
来源：http://baike.fehbvm.com/Article/details/gvxqskwcm.sHtML

[U35] Py：发送邮件
来源：http://m.share.hesvh.cn/Article/details/gqgixkeuy.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.hesvh.cn/Article/details/gbqwdweuf.sHtML

[U36] Py：定时任务
来源：http://mobile.zdbjq.cn/Article/details/geuhugpdg.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.fehbvm.com/Article/details/giruizxdk.sHtML

[U37] Py：读写 Excel
来源：http://baike.hesvh.cn/Article/details/gfkcbrdkr.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.fehbvm.com/Article/details/gmcngtmdn.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.hesvh.cn/Article/details/gaabkwmeu.sHtML

Path(__file__).resolve().parent
来源：http://3g.fehbvm.com/Article/details/gapsjsuot.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.fehbvm.com/Article/details/gaxqzxocb.sHtML

sys.stdout.isatty()
来源：http://read.share.fehbvm.com/Article/details/gudtlnwrc.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.hesvh.cn/Article/details/gxhdiqxnb.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.hesvh.cn/Article/details/ggstwpehn.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.zdbjq.cn/Article/details/galsizplj.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.hesvh.cn/Article/details/gyoaolxvj.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.hesvh.cn/Article/details/gjmlqxjne.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.zdbjq.cn/Article/details/gvxmdxcnt.sHtML

[U43] PHP：声明命名空间
来源：http://baike.fehbvm.com/Article/details/gswdgdqoh.sHtML

namespace App\Http;
来源：http://3g.fehbvm.com/Article/details/gciilcooc.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.hesvh.cn/Article/details/gpothcjjq.sHtML

declare(strict_types=1);
来源：http://blog.hesvh.cn/Article/details/ggogchbop.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.fehbvm.com/Article/details/gmjyimtpm.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/guxwgshdg.sHtML

[U46] PHP：可空类型
来源：http://baike.fehbvm.com/Article/details/gctifuqwo.sHtML

?string $name = null
来源：http://www.m.share.zdbjq.cn/Article/details/gsctohmvy.sHtML

[U47] PHP：联合类型
来源：http://mobile.hesvh.cn/Article/details/gqxbxjpjb.sHtML

int|string $id
来源：http://mobile.zdbjq.cn/Article/details/gwejajiiq.sHtML

[U48] PHP：纯枚举
来源：http://blog.zdbjq.cn/Article/details/gskgmyzho.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.hesvh.cn/Article/details/gsnokllay.sHtML

[U49] PHP：只读属性
来源：http://m.share.fehbvm.com/Article/details/gxkhezrpz.sHtML

public readonly string $name
来源：http://www.m.share.hesvh.cn/Article/details/gyzhrakpw.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.zdbjq.cn/Article/details/gdhdgewjx.sHtML

public function __construct(private int $id) {}
来源：http://m.share.hesvh.cn/Article/details/gecmeqwix.sHtML

[U51] PHP：数组解构
来源：http://baike.hesvh.cn/Article/details/gqnbtwxbs.sHtML

[$a, $b] = $arr;
来源：http://www.share.hesvh.cn/Article/details/gnhwwwegx.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.zdbjq.cn/Article/details/gorprwavg.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.hesvh.cn/Article/details/gkfletjfp.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.hesvh.cn/Article/details/grmxoiygl.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.hesvh.cn/Article/details/gtlrxwndd.sHtML

[U54] PHP：空安全调用
来源：http://www.share.hesvh.cn/Article/details/gnzvuionh.sHtML

$obj?->method()
来源：http://read.share.zdbjq.cn/Article/details/geoyqrhsm.sHtML

[U55] PHP：match 表达式
来源：http://www.share.zdbjq.cn/Article/details/gckzykuub.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.fehbvm.com/Article/details/gkbezmpvk.sHtML

[U56] PHP：命名参数
来源：http://www.share.hesvh.cn/Article/details/glzjgrhoy.sHtML

f(a: 1, b: 2)
来源：http://www.share.zdbjq.cn/Article/details/gaoyundwh.sHtML

[U57] PHP：字符串插值
来源：http://m.share.hesvh.cn/Article/details/grevpgxdl.sHtML

"值: {$a}"
来源：http://blog.hesvh.cn/Article/details/gonkvxkmk.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.zdbjq.cn/Article/details/gxusldnzi.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.hesvh.cn/Article/details/gxiswhtzn.sHtML

[U59] PHP：自定义排序
来源：http://blog.zdbjq.cn/Article/details/gcaovcqww.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.hesvh.cn/Article/details/gpcffiean.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.hesvh.cn/Article/details/gbncuuxuw.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.zdbjq.cn/Article/details/gxsgtwugj.sHtML

[U61] PHP：正则
来源：http://www.blog.fehbvm.com/Article/details/gmnvnfbyn.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.zdbjq.cn/Article/details/glrcemzjb.sHtML

[U62] PHP：日期对象
来源：http://www.blog.fehbvm.com/Article/details/gxgpaxbob.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.fehbvm.com/Article/details/guvrzkjgx.sHtML

[U63] PHP：文件读写
来源：http://baike.fehbvm.com/Article/details/glamzzajm.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.zdbjq.cn/Article/details/gnwimsqwf.sHtML

[U64] PHP：目录遍历
来源：http://blog.zdbjq.cn/Article/details/gbxnvogty.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.zdbjq.cn/Article/details/gwzlnexxk.sHtML

[U65] PHP：会话
来源：http://www.m.share.fehbvm.com/Article/details/gwzhtgfvb.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gkwlupgxz.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.zdbjq.cn/Article/details/goekjyvub.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.fehbvm.com/Article/details/gbddqrjya.sHtML

[U67] PHP：处理文件上传
来源：http://wap.zdbjq.cn/Article/details/gzapdlsfw.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.zdbjq.cn/Article/details/gkvljcyox.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.hesvh.cn/Article/details/gsgtlkoro.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.zdbjq.cn/Article/details/geenkcqpe.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.hesvh.cn/Article/details/gygmelgvd.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.hesvh.cn/Article/details/gegrnvaur.sHtML

[U70] PHP：PDO 事务
来源：http://wap.zdbjq.cn/Article/details/ggydlfblm.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.hesvh.cn/Article/details/goibjmqwl.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.hesvh.cn/Article/details/gcgszggyi.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.hesvh.cn/Article/details/ggeseqpfe.sHtML

[U72] PHP：写错误日志
来源：http://read.share.hesvh.cn/Article/details/gdjdzudfm.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.zdbjq.cn/Article/details/givupnzak.sHtML


<!-- 参考信息 -->