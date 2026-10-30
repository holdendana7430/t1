代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gnfvgunyj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fanxiaobao.xyz/Article/details/gayfjndrc.sHtML

[S48] C++：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gmaajvflt.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fanxiaobao.xyz/Article/details/guwfxdetf.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gqjvfjuan.sHtML

[S49] C++：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gbztkeybn.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fanxiaobao.xyz/Article/details/grmaqzibk.sHtML

[S50] C++：格式化数字
来源：http://3g.fanxiaobao.xyz/Article/details/gfxhkorwg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdoomdaxi.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/ggbejizzs.sHtML

static_cast<double>(a) / b
来源：http://read.share.fanxiaobao.xyz/Article/details/glnggzduv.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fanxiaobao.xyz/Article/details/gznpyzrfb.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfklyofwx.sHtML

[S53] C++：移动语义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gubngktwl.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fanxiaobao.xyz/Article/details/gekiglegt.sHtML

[S54] C++：异常处理
来源：http://3g.fanxiaobao.xyz/Article/details/gurdrdnuy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gkogocyca.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyhknchxx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghplbbxrh.sHtML

[S56] C++：optional
来源：http://mobile.fanxiaobao.xyz/Article/details/guzujthxo.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fanxiaobao.xyz/Article/details/ghnwjggxj.sHtML

[S57] C++：编译期常量
来源：http://m.share.fanxiaobao.xyz/Article/details/ganinkhfe.sHtML

constexpr int N = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/giryalrfl.sHtML

[S58] C++：命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/gyxlrvnxi.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gboghsyso.sHtML

[S59] C++：静态断言
来源：http://read.share.fanxiaobao.xyz/Article/details/gyfynadpn.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fanxiaobao.xyz/Article/details/gyyipyqiz.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fanxiaobao.xyz/Article/details/gwjrurncl.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/gyqvrypxi.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/goudsyrbq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkyflkeuj.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gnxgszoup.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/grdsmamhw.sHtML

println("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gpsvclrou.sHtML

[T02] Kotlin：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gqnwczzhe.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fanxiaobao.xyz/Article/details/giudhmvce.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fanxiaobao.xyz/Article/details/gggfqdapa.sHtML

"值: $b"
来源：http://wap.fanxiaobao.xyz/Article/details/grunvvchi.sHtML

[T04] Kotlin：空安全
来源：http://3g.fanxiaobao.xyz/Article/details/gyxukeeni.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gagmttcgj.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnmbrwrge.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fanxiaobao.xyz/Article/details/gokgspwjw.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/gausgkuxm.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/ggzpfldxm.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvsujyzaw.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkiygswiy.sHtML

[T08] Kotlin：数据类
来源：http://blog.fanxiaobao.xyz/Article/details/gjdriizqi.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gatgtccll.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjxzvcarj.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fanxiaobao.xyz/Article/details/gjmnatwyi.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gtpgrykbz.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fanxiaobao.xyz/Article/details/gqlcpvjht.sHtML

[T11] Kotlin：协程
来源：http://blog.fanxiaobao.xyz/Article/details/gvwkuahpi.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.fanxiaobao.xyz/Article/details/gidesdrmd.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkflkdexy.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gvyeekabt.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gefvfodyq.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gksnonwxz.sHtML

[T14] Kotlin：循环
来源：http://baike.fanxiaobao.xyz/Article/details/gefzxzvoq.sHtML

for (i in 1..10) println(i)
来源：http://wap.fanxiaobao.xyz/Article/details/gplhkwusk.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gogmizdxh.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fanxiaobao.xyz/Article/details/gfncnatae.sHtML

[T16] Swift：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gfqilwqak.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnuijikam.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gniclgima.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxbaitymg.sHtML

[T18] Swift：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gicqsetpd.sHtML

"值: \(b)"
来源：http://mobile.fanxiaobao.xyz/Article/details/gtierbrpp.sHtML

[T19] Swift：可选绑定
来源：http://3g.fanxiaobao.xyz/Article/details/gxnttgsxy.sHtML

if let n = opt { print(n) }
来源：http://3g.fanxiaobao.xyz/Article/details/gxsxeztid.sHtML

[T20] Swift：数组操作
来源：http://wap.fanxiaobao.xyz/Article/details/gvnmjtszb.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.fanxiaobao.xyz/Article/details/geoziwtiq.sHtML

[T21] Swift：遍历
来源：http://baike.fanxiaobao.xyz/Article/details/godspgxsf.sHtML

for x in a { print(x) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkoexivww.sHtML

[T22] Swift：字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gjhcojkqt.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gdjiqosor.sHtML

[T23] Swift：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gqtnlatbz.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fanxiaobao.xyz/Article/details/gfgwlyxia.sHtML

[T24] Swift：闭包
来源：http://wap.fanxiaobao.xyz/Article/details/gubbyughg.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcjxaylts.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqdyacmml.sHtML

struct P { var x: Int }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghyporqkv.sHtML

[T26] Swift：类与重写
来源：http://mobile.fanxiaobao.xyz/Article/details/gqvhslnio.sHtML

class A: Base { override func f() {} }
来源：http://blog.fanxiaobao.xyz/Article/details/glznuhqei.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxqxnktzv.sHtML

do { try f() } catch { print(error) }
来源：http://3g.fanxiaobao.xyz/Article/details/gmqyfhrms.sHtML

[T28] Swift：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gqekzsfhw.sHtML

enum Color { case red, green }
来源：http://m.share.fanxiaobao.xyz/Article/details/gktwzvzya.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geoesvkdg.sHtML

guard let x = opt else { return }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvmpbszle.sHtML

[T30] Swift：协议
来源：http://m.share.fanxiaobao.xyz/Article/details/gctwvmcwv.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdophaqkl.sHtML

[T31] Lua：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gecidtlke.sHtML

print("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gjtnfyuci.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtzfpcewq.sHtML

local a = 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gjxtrsjnh.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxadnziij.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.fanxiaobao.xyz/Article/details/gvwcyfuwa.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfzpeafbz.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.fanxiaobao.xyz/Article/details/gyrqkjcjq.sHtML

[T35] Lua：字典表
来源：http://m.share.fanxiaobao.xyz/Article/details/gzkjtadtz.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/guactyzbu.sHtML

[T36] Lua：函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grlhtfdjg.sHtML

function add(a, b) return a + b end
来源：http://baike.fanxiaobao.xyz/Article/details/gmckbflyc.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gptcsikuy.sHtML

"a" .. "b"
来源：http://baike.fanxiaobao.xyz/Article/details/gqplrjvsm.sHtML

[T38] Lua：条件
来源：http://baike.fanxiaobao.xyz/Article/details/gzemeypkq.sHtML

if x > 0 then print("正") end
来源：http://baike.fanxiaobao.xyz/Article/details/ggbqnbwvm.sHtML

[T39] Lua：模式匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gyrbdqkjy.sHtML

string.find(s, "%d+")
来源：http://3g.fanxiaobao.xyz/Article/details/gpviireaz.sHtML

[T40] Lua：元表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfkspfelb.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.fanxiaobao.xyz/Article/details/gkdmdlzon.sHtML

[T41] Perl：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gdnvmpglw.sHtML

print "Hello\n";
来源：http://baike.fanxiaobao.xyz/Article/details/gvfoncbef.sHtML

[T42] Perl：变量类型
来源：http://wap.fanxiaobao.xyz/Article/details/gjuqldfpt.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.fanxiaobao.xyz/Article/details/genjabcae.sHtML

[T43] Perl：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gmqvtfltk.sHtML

"值: $a"
来源：http://read.share.fanxiaobao.xyz/Article/details/gdxnuijpd.sHtML

[T44] Perl：条件
来源：http://3g.fanxiaobao.xyz/Article/details/gbbdpdoal.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gyyppylej.sHtML

[T45] Perl：数组遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gbafyrqfg.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdlqsdrep.sHtML

[T46] Perl：哈希操作
来源：http://m.share.fanxiaobao.xyz/Article/details/giqpfgzqm.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gioehmuas.sHtML

[T47] Perl：正则捕获
来源：http://mobile.fanxiaobao.xyz/Article/details/glyzlohtk.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjpayphca.sHtML

[T48] Perl：正则替换
来源：http://baike.fanxiaobao.xyz/Article/details/gbumoievm.sHtML

$s =~ s/old/new/g;
来源：http://m.share.fanxiaobao.xyz/Article/details/glvbkkzdu.sHtML

[T49] Perl：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gspgxvfnv.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghokvibnd.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gencnrftt.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.fanxiaobao.xyz/Article/details/gmzsohcdc.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gopfscimv.sHtML

[T51] Scala：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gtdidqsbf.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gljlxawqi.sHtML

[T52] Scala：变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmgyhfgtp.sHtML

val a = 1;  var b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gyydxahsn.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gahxunmpp.sHtML

s"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gllekqsej.sHtML

[T54] Scala：集合映射
来源：http://wap.fanxiaobao.xyz/Article/details/guhuokxhz.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfsgflxan.sHtML

[T55] Scala：集合过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gdqosbtey.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gmgxfgxjr.sHtML

[T56] Scala：样例类
来源：http://m.share.fanxiaobao.xyz/Article/details/glgfoerrr.sHtML

case class User(name: String, age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/gwnqiadrr.sHtML

[T57] Scala：模式匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gjjwqwcrb.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkldvupjq.sHtML

[T58] Scala：函数定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gdeyecjps.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.fanxiaobao.xyz/Article/details/gosdbskla.sHtML

[T59] Scala：循环
来源：http://blog.fanxiaobao.xyz/Article/details/gaaspznvy.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.fanxiaobao.xyz/Article/details/ghnbdzxis.sHtML

[T60] Scala：折叠
来源：http://3g.fanxiaobao.xyz/Article/details/gvmytxgfx.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.fanxiaobao.xyz/Article/details/gmegmhwfy.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gcqvsmjlt.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gojfzgurc.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/guyxlhahz.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.fanxiaobao.xyz/Article/details/gjuyigppv.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnpzfhbds.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.fanxiaobao.xyz/Article/details/ghcymnyqw.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/ggayqrgbf.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.fanxiaobao.xyz/Article/details/ggmqqidje.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.fanxiaobao.xyz/Article/details/gmhpallsr.sHtML

[U04] Py：变量调试打印
来源：http://3g.fanxiaobao.xyz/Article/details/gmzupqwmx.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gttkfoaya.sHtML

[U05] Py：列表去重且保序
来源：http://3g.fanxiaobao.xyz/Article/details/gawaehcme.sHtML

list(dict.fromkeys(arr))
来源：http://blog.fanxiaobao.xyz/Article/details/gpiixfhvi.sHtML

[U06] Py：合并两个字典
来源：http://3g.fanxiaobao.xyz/Article/details/gyvdwrbim.sHtML

{**a, **b}
来源：http://baike.fanxiaobao.xyz/Article/details/gznfocfti.sHtML

[U07] Py：反转字典键值
来源：http://3g.fanxiaobao.xyz/Article/details/gvlepfznv.sHtML

{v: k for k, v in d.items()}
来源：http://blog.fanxiaobao.xyz/Article/details/gufwuaise.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtzygbvwa.sHtML

[y for x in nested for y in x]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcncwjqwl.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gidvcjevs.sHtML

max(d, key=d.get)
来源：http://m.share.fanxiaobao.xyz/Article/details/gepenfdsp.sHtML

[U10] Py：按值排序字典
来源：http://3g.fanxiaobao.xyz/Article/details/gyledqkpt.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.fanxiaobao.xyz/Article/details/ggmwtxaxd.sHtML

[U11] Py：生成器表达式
来源：http://blog.fanxiaobao.xyz/Article/details/giqksoosj.sHtML

(x * 2 for x in arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gukxntskk.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gmkutcubv.sHtML

Counter(arr).most_common(3)
来源：http://blog.fanxiaobao.xyz/Article/details/gqgouvemn.sHtML

[U13] Py：固定长度队列
来源：http://m.share.fanxiaobao.xyz/Article/details/gujczmcll.sHtML

deque(maxlen=10)
来源：http://mobile.fanxiaobao.xyz/Article/details/geipezhwx.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnhqvzwyr.sHtML

defaultdict(list)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnhshfzyx.sHtML

[U15] Py：高精度计时
来源：http://wap.fanxiaobao.xyz/Article/details/ggeuphdck.sHtML

t = time.perf_counter()
来源：http://wap.fanxiaobao.xyz/Article/details/gihbbaipr.sHtML

[U16] Py：命令行参数解析
来源：http://3g.fanxiaobao.xyz/Article/details/glebgmfrc.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fanxiaobao.xyz/Article/details/gehmbdkwu.sHtML

[U17] Py：初始化日志
来源：http://blog.fanxiaobao.xyz/Article/details/gzoeckjxo.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.fanxiaobao.xyz/Article/details/gcetxdcuu.sHtML

[U18] Py：预编译正则
来源：http://blog.fanxiaobao.xyz/Article/details/gghdrfpph.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/gcgirgvyk.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhgodxdn.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.fanxiaobao.xyz/Article/details/gpqfdeauk.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.fanxiaobao.xyz/Article/details/ghrueekcm.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.fanxiaobao.xyz/Article/details/goimepfue.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.fanxiaobao.xyz/Article/details/gbwpsumsb.sHtML

@contextlib.contextmanager
来源：http://wap.fanxiaobao.xyz/Article/details/gojyiymqt.sHtML

[U22] Py：矩阵转置
来源：http://baike.fanxiaobao.xyz/Article/details/ghfnvpzfw.sHtML

list(zip(*m))
来源：http://m.share.fanxiaobao.xyz/Article/details/gfgbmhtqz.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzrfsvvms.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.fanxiaobao.xyz/Article/details/gyptsrbue.sHtML

[U24] Py：路径操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gfltatyda.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.fanxiaobao.xyz/Article/details/gkbmdtdkm.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.fanxiaobao.xyz/Article/details/grnmpyzhb.sHtML

csv.DictReader(f)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdlbvfhpg.sHtML

[U26] Py：并发下载
来源：http://wap.fanxiaobao.xyz/Article/details/gnvoqnizo.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.fanxiaobao.xyz/Article/details/galwnzeuo.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.fanxiaobao.xyz/Article/details/ggtatjcit.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.fanxiaobao.xyz/Article/details/gnmnyifpg.sHtML

[U28] Py：类型别名
来源：http://read.share.fanxiaobao.xyz/Article/details/gxjokksxw.sHtML

UserId = int
来源：http://m.share.fanxiaobao.xyz/Article/details/grnirowyq.sHtML

[U29] Py：属性校验
来源：http://read.share.fanxiaobao.xyz/Article/details/gdxyjkvet.sHtML

@property 与 @x.setter 配合
来源：http://blog.fanxiaobao.xyz/Article/details/ggeljtfcv.sHtML

[U30] Py：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/gioqobics.sHtML

@dataclass(slots=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glhinzlrr.sHtML

[U31] Py：单测
来源：http://wap.fanxiaobao.xyz/Article/details/gdgwyhqvq.sHtML

python -m pytest -q
来源：http://3g.fanxiaobao.xyz/Article/details/gollewnjn.sHtML

[U32] Py：代码格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gpavfobsy.sHtML

ruff format . && ruff check --fix .
来源：http://blog.fanxiaobao.xyz/Article/details/gzdfewbmn.sHtML

[U33] Py：打包发布
来源：http://m.share.fanxiaobao.xyz/Article/details/gqedihnmg.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.fanxiaobao.xyz/Article/details/gtzfmcfti.sHtML

[U34] Py：判断编码
来源：http://baike.fanxiaobao.xyz/Article/details/giwvwlrbt.sHtML

chardet.detect(raw)
来源：http://baike.fanxiaobao.xyz/Article/details/gznmofqwr.sHtML

[U35] Py：发送邮件
来源：http://wap.fanxiaobao.xyz/Article/details/gvqsuaqma.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.fanxiaobao.xyz/Article/details/ggtarxmad.sHtML

[U36] Py：定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gulnhmmzj.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvwrorxwe.sHtML

[U37] Py：读写 Excel
来源：http://blog.fanxiaobao.xyz/Article/details/gklzyjzzi.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsqrdclsf.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.fanxiaobao.xyz/Article/details/gnocntjxg.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwddlgxxy.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpuvkmtvd.sHtML

sys.stdout.isatty()
来源：http://mobile.fanxiaobao.xyz/Article/details/gtfhmabpj.sHtML

[U40] Py：打印到标准错误
来源：http://baike.fanxiaobao.xyz/Article/details/gazrxjnvh.sHtML

print("err", file=sys.stderr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gajjbmtit.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbqvffmtf.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grvafpegp.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.fanxiaobao.xyz/Article/details/gbsddwhxc.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gshvozboy.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwohafkmh.sHtML

namespace App\Http;
来源：http://mobile.fanxiaobao.xyz/Article/details/geervhjux.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkktokynu.sHtML

declare(strict_types=1);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqwwjdghu.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.fanxiaobao.xyz/Article/details/gzojajyto.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gcwhsrguj.sHtML

[U46] PHP：可空类型
来源：http://wap.fanxiaobao.xyz/Article/details/gfmidiokt.sHtML

?string $name = null
来源：http://m.share.fanxiaobao.xyz/Article/details/gbswznlym.sHtML

[U47] PHP：联合类型
来源：http://3g.fanxiaobao.xyz/Article/details/gruxzerhl.sHtML

int|string $id
来源：http://m.share.fanxiaobao.xyz/Article/details/gqnxlhiow.sHtML

[U48] PHP：纯枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gqwfbzewd.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gltowsnic.sHtML

[U49] PHP：只读属性
来源：http://baike.fanxiaobao.xyz/Article/details/gtqclqdbs.sHtML

public readonly string $name
来源：http://wap.fanxiaobao.xyz/Article/details/giatptnux.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.fanxiaobao.xyz/Article/details/grfjksfwu.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmvknuznn.sHtML

[U51] PHP：数组解构
来源：http://mobile.fanxiaobao.xyz/Article/details/gxeaxnqbs.sHtML

[$a, $b] = $arr;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcurrgysi.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcfgvzjke.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.fanxiaobao.xyz/Article/details/gtjfllkrf.sHtML

[U53] PHP：空合并运算符
来源：http://wap.fanxiaobao.xyz/Article/details/glzhedoni.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.fanxiaobao.xyz/Article/details/ghkercbiq.sHtML

[U54] PHP：空安全调用
来源：http://mobile.fanxiaobao.xyz/Article/details/gzjraufml.sHtML

$obj?->method()
来源：http://mobile.fanxiaobao.xyz/Article/details/gyuxqjvjw.sHtML

[U55] PHP：match 表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gejdddnci.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.fanxiaobao.xyz/Article/details/gtfnmholc.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxmtalvrq.sHtML

f(a: 1, b: 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmlemqhvx.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbpsfsxyc.sHtML

"值: {$a}"
来源：http://baike.fanxiaobao.xyz/Article/details/gmkdzerfk.sHtML

[U58] PHP：数组三件套
来源：http://www.share.fanxiaobao.xyz/Article/details/gbyqcdmux.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.fanxiaobao.xyz/Article/details/gjnhsbauo.sHtML

[U59] PHP：自定义排序
来源：http://wap.fanxiaobao.xyz/Article/details/gffqocztn.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggtojstkw.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.fanxiaobao.xyz/Article/details/gppmnrfzj.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmgehauxl.sHtML

[U61] PHP：正则
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpdqinrpm.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.fanxiaobao.xyz/Article/details/glauugxha.sHtML

[U62] PHP：日期对象
来源：http://baike.fanxiaobao.xyz/Article/details/gdraimiht.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.fanxiaobao.xyz/Article/details/gxnhuwusk.sHtML

[U63] PHP：文件读写
来源：http://wap.fanxiaobao.xyz/Article/details/gwwcnnydu.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvvvyozei.sHtML

[U64] PHP：目录遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gopowatcf.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.fanxiaobao.xyz/Article/details/glrmskzce.sHtML

[U65] PHP：会话
来源：http://blog.fanxiaobao.xyz/Article/details/gsoypamco.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvnqwkeyl.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.fanxiaobao.xyz/Article/details/gzwlgulim.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.fanxiaobao.xyz/Article/details/gszdwhtex.sHtML

[U67] PHP：处理文件上传
来源：http://blog.fanxiaobao.xyz/Article/details/ghzdiwrgq.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.fanxiaobao.xyz/Article/details/grficnwzu.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giutgkfkx.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gewjeffpx.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.fanxiaobao.xyz/Article/details/glhzmosdz.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.fanxiaobao.xyz/Article/details/gvavctnnw.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmzedxtmy.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggtvvknub.sHtML

[U71] PHP：抛出异常
来源：http://baike.fanxiaobao.xyz/Article/details/gdcgjlsvx.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.fanxiaobao.xyz/Article/details/geifkovqk.sHtML

[U72] PHP：写错误日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gfhlftwae.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.fanxiaobao.xyz/Article/details/gfdvgynmo.sHtML


<!-- 参考信息 -->