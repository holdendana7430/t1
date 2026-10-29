代发 wailian999

[S45] C++：lambda
来源：http://www.share.zdbjq.cn/Article/details/godbqiath.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.hesvh.cn/Article/details/gpwwjhrif.sHtML

[S46] C++：函数模板
来源：http://wap.hesvh.cn/Article/details/gibwdjqex.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.hesvh.cn/Article/details/grfivkeon.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fehbvm.com/Article/details/gvhshjhcw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.zdbjq.cn/Article/details/gcpetimtr.sHtML

[S48] C++：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gybbfutbv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.hesvh.cn/Article/details/gadgmhpyd.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fehbvm.com/Article/details/ggzdfrgrr.sHtML

[S49] C++：写文件
来源：http://wap.fehbvm.com/Article/details/gtfipjusb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.zdbjq.cn/Article/details/gbymcnohc.sHtML

[S50] C++：格式化数字
来源：http://baike.zdbjq.cn/Article/details/gudsjrcjh.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gefdkhyqw.sHtML

[S51] C++：显式类型转换
来源：http://blog.zdbjq.cn/Article/details/gddhsfuyy.sHtML

static_cast<double>(a) / b
来源：http://www.blog.hesvh.cn/Article/details/gkhbtjzoy.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.hesvh.cn/Article/details/ghuzbyunv.sHtML

int size() const noexcept { return n_; }
来源：http://wap.zdbjq.cn/Article/details/ghbqigirt.sHtML

[S53] C++：移动语义
来源：http://wap.zdbjq.cn/Article/details/gbghchcyp.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.zdbjq.cn/Article/details/gtpgbpnwe.sHtML

[S54] C++：异常处理
来源：http://www.m.share.zdbjq.cn/Article/details/gcrotmmoe.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.zdbjq.cn/Article/details/gopwqchzc.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fehbvm.com/Article/details/gnicodzyn.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.hesvh.cn/Article/details/gzwmxpzdb.sHtML

[S56] C++：optional
来源：http://blog.zdbjq.cn/Article/details/gfmnibdvf.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.zdbjq.cn/Article/details/gxfdsqwil.sHtML

[S57] C++：编译期常量
来源：http://m.share.zdbjq.cn/Article/details/goyxmvysv.sHtML

constexpr int N = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gknujsizd.sHtML

[S58] C++：命名空间
来源：http://3g.fehbvm.com/Article/details/gxpbpgkvq.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.hesvh.cn/Article/details/ggccbnfdk.sHtML

[S59] C++：静态断言
来源：http://wap.fehbvm.com/Article/details/gepcovlmo.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fehbvm.com/Article/details/gpfbxyggn.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fehbvm.com/Article/details/grmyjtbjd.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fehbvm.com/Article/details/gpvuansgw.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gyhxipofs.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fehbvm.com/Article/details/gogtwljuo.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gkrdpojoi.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.hesvh.cn/Article/details/gsjyhcgny.sHtML

println("Hello")
来源：http://blog.hesvh.cn/Article/details/gntrzfgnb.sHtML

[T02] Kotlin：变量
来源：http://mobile.hesvh.cn/Article/details/gsfjayads.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.zdbjq.cn/Article/details/gpoeupbkk.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.zdbjq.cn/Article/details/gtnqswzqj.sHtML

"值: $b"
来源：http://www.share.fehbvm.com/Article/details/gjeefsvgd.sHtML

[T04] Kotlin：空安全
来源：http://m.share.zdbjq.cn/Article/details/gftdjzbuk.sHtML

val n: String? = null;  n?.length
来源：http://baike.hesvh.cn/Article/details/gdecnftsh.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.zdbjq.cn/Article/details/gbnixwuah.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.zdbjq.cn/Article/details/gwmkqmotq.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fehbvm.com/Article/details/gjluxbchr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fehbvm.com/Article/details/gwvxrfcln.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fehbvm.com/Article/details/goqpvtptw.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.hesvh.cn/Article/details/gpkomfceh.sHtML

[T08] Kotlin：数据类
来源：http://read.share.hesvh.cn/Article/details/gmwrfqsuc.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.zdbjq.cn/Article/details/gonthlsrk.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fehbvm.com/Article/details/gzttcgmgk.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.hesvh.cn/Article/details/gwwouqygr.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fehbvm.com/Article/details/gqeddlygf.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.zdbjq.cn/Article/details/guhluclkm.sHtML

[T11] Kotlin：协程
来源：http://3g.hesvh.cn/Article/details/gklataxno.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.hesvh.cn/Article/details/geevkjxey.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.zdbjq.cn/Article/details/ganyxpatk.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gvkmiwagg.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.zdbjq.cn/Article/details/gonjyarqs.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fehbvm.com/Article/details/gpsvizmso.sHtML

[T14] Kotlin：循环
来源：http://www.share.fehbvm.com/Article/details/gcpqblldv.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fehbvm.com/Article/details/goabkkbgi.sHtML

[T15] Kotlin：接口
来源：http://m.share.zdbjq.cn/Article/details/govofjzsc.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.hesvh.cn/Article/details/grneimxty.sHtML

[T16] Swift：Hello World
来源：http://baike.hesvh.cn/Article/details/gxvdtrwzx.sHtML

print("Hello")
来源：http://read.share.hesvh.cn/Article/details/gmbqeyegv.sHtML

[T17] Swift：变量与常量
来源：http://mobile.zdbjq.cn/Article/details/gzpwelqup.sHtML

var a = 1;  let b = 2
来源：http://mobile.fehbvm.com/Article/details/gbmmngbjp.sHtML

[T18] Swift：字符串插值
来源：http://blog.fehbvm.com/Article/details/gcflfyoyh.sHtML

"值: \(b)"
来源：http://mobile.hesvh.cn/Article/details/gnzegjafc.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.zdbjq.cn/Article/details/gsnqqjmpj.sHtML

if let n = opt { print(n) }
来源：http://wap.hesvh.cn/Article/details/gpepcxsnj.sHtML

[T20] Swift：数组操作
来源：http://wap.zdbjq.cn/Article/details/geuaznvta.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fehbvm.com/Article/details/gpfxxmdps.sHtML

[T21] Swift：遍历
来源：http://mobile.hesvh.cn/Article/details/ghtmfrjqj.sHtML

for x in a { print(x) }
来源：http://baike.fehbvm.com/Article/details/gqvzexwsy.sHtML

[T22] Swift：字典
来源：http://baike.zdbjq.cn/Article/details/gdmirhisp.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.hesvh.cn/Article/details/gmkbfrxqi.sHtML

[T23] Swift：函数
来源：http://m.share.fehbvm.com/Article/details/ghivhlkix.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fehbvm.com/Article/details/gmxpazgoe.sHtML

[T24] Swift：闭包
来源：http://www.share.zdbjq.cn/Article/details/gheqwkksg.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.hesvh.cn/Article/details/gcrlywjiw.sHtML

[T25] Swift：结构体
来源：http://read.share.zdbjq.cn/Article/details/gykagsyxd.sHtML

struct P { var x: Int }
来源：http://read.share.hesvh.cn/Article/details/gtezmibhp.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.hesvh.cn/Article/details/gumkojdxd.sHtML

class A: Base { override func f() {} }
来源：http://baike.zdbjq.cn/Article/details/goknbsxtv.sHtML

[T27] Swift：错误处理
来源：http://www.share.fehbvm.com/Article/details/ghwtznkvu.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.hesvh.cn/Article/details/grpwxxvfc.sHtML

[T28] Swift：枚举
来源：http://www.blog.hesvh.cn/Article/details/gcabmwqnf.sHtML

enum Color { case red, green }
来源：http://mobile.fehbvm.com/Article/details/gvodfsdra.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fehbvm.com/Article/details/ghfkzaczg.sHtML

guard let x = opt else { return }
来源：http://www.share.hesvh.cn/Article/details/gvjsaokwm.sHtML

[T30] Swift：协议
来源：http://www.m.share.fehbvm.com/Article/details/gfqkzyxhm.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.fehbvm.com/Article/details/gebsrmpol.sHtML

[T31] Lua：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gmafcemwv.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/gvzgkhcaf.sHtML

[T32] Lua：局部变量
来源：http://www.blog.zdbjq.cn/Article/details/gghqkbiwm.sHtML

local a = 1
来源：http://www.share.hesvh.cn/Article/details/gftyocsly.sHtML

[T33] Lua：表（数组）
来源：http://blog.zdbjq.cn/Article/details/gehrgmpok.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.hesvh.cn/Article/details/guhsrbxhp.sHtML

[T34] Lua：遍历表
来源：http://m.share.zdbjq.cn/Article/details/gykoatpvt.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.hesvh.cn/Article/details/gczfefqjr.sHtML

[T35] Lua：字典表
来源：http://www.blog.hesvh.cn/Article/details/gmvndgwyy.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fehbvm.com/Article/details/grwphhdgk.sHtML

[T36] Lua：函数
来源：http://mobile.zdbjq.cn/Article/details/gyyflbhja.sHtML

function add(a, b) return a + b end
来源：http://blog.fehbvm.com/Article/details/gcevdovku.sHtML

[T37] Lua：字符串拼接
来源：http://wap.hesvh.cn/Article/details/gpkkwprft.sHtML

"a" .. "b"
来源：http://m.share.hesvh.cn/Article/details/gqygomqif.sHtML

[T38] Lua：条件
来源：http://wap.zdbjq.cn/Article/details/geqowzruo.sHtML

if x > 0 then print("正") end
来源：http://mobile.zdbjq.cn/Article/details/gubujgzxb.sHtML

[T39] Lua：模式匹配
来源：http://m.share.hesvh.cn/Article/details/giixkoutx.sHtML

string.find(s, "%d+")
来源：http://mobile.zdbjq.cn/Article/details/ggtcvtzly.sHtML

[T40] Lua：元表
来源：http://www.blog.zdbjq.cn/Article/details/gzeadkkea.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.hesvh.cn/Article/details/gtfolsxip.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gujjogguy.sHtML

print "Hello\n";
来源：http://baike.fehbvm.com/Article/details/guqrpkztd.sHtML

[T42] Perl：变量类型
来源：http://read.share.fehbvm.com/Article/details/gfacpdenk.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.hesvh.cn/Article/details/gyvsgfunq.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gwhoiyome.sHtML

"值: $a"
来源：http://mobile.hesvh.cn/Article/details/goizronak.sHtML

[T44] Perl：条件
来源：http://read.share.fehbvm.com/Article/details/gsrdbcxko.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.fehbvm.com/Article/details/ggwxzdbsx.sHtML

[T45] Perl：数组遍历
来源：http://www.share.hesvh.cn/Article/details/gexcccdfn.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.fehbvm.com/Article/details/gnkebjkxi.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.fehbvm.com/Article/details/gwndcxhbt.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.fehbvm.com/Article/details/gguxfccud.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.fehbvm.com/Article/details/gslltesad.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.zdbjq.cn/Article/details/grsvvgzol.sHtML

[T48] Perl：正则替换
来源：http://m.share.zdbjq.cn/Article/details/gppacnnki.sHtML

$s =~ s/old/new/g;
来源：http://www.share.zdbjq.cn/Article/details/gmldkfifl.sHtML

[T49] Perl：函数
来源：http://read.share.fehbvm.com/Article/details/gcmtrpkiw.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gkdkwxvmh.sHtML

[T50] Perl：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gioycvndu.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.zdbjq.cn/Article/details/gecucjcfm.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.zdbjq.cn/Article/details/gkryezkzj.sHtML

[T51] Scala：Hello World
来源：http://baike.zdbjq.cn/Article/details/gspgpdjbm.sHtML

println("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gopubouqx.sHtML

[T52] Scala：变量
来源：http://blog.zdbjq.cn/Article/details/giijwroub.sHtML

val a = 1;  var b = 2
来源：http://blog.fehbvm.com/Article/details/gxcyxrmph.sHtML

[T53] Scala：字符串插值
来源：http://baike.hesvh.cn/Article/details/gupfxcwsp.sHtML

s"值: $b"
来源：http://www.blog.hesvh.cn/Article/details/gkykofllc.sHtML

[T54] Scala：集合映射
来源：http://mobile.hesvh.cn/Article/details/gymcaezov.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.zdbjq.cn/Article/details/gjqilxbib.sHtML

[T55] Scala：集合过滤
来源：http://read.share.fehbvm.com/Article/details/gcmkkykuf.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.zdbjq.cn/Article/details/gzhuzwnij.sHtML

[T56] Scala：样例类
来源：http://blog.zdbjq.cn/Article/details/gxaidpzxr.sHtML

case class User(name: String, age: Int)
来源：http://blog.zdbjq.cn/Article/details/glnztuegh.sHtML

[T57] Scala：模式匹配
来源：http://baike.zdbjq.cn/Article/details/gnzlupshj.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.hesvh.cn/Article/details/gtsrfjrek.sHtML

[T58] Scala：函数定义
来源：http://wap.hesvh.cn/Article/details/gkflhauvk.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.hesvh.cn/Article/details/gpiypctpr.sHtML

[T59] Scala：循环
来源：http://3g.zdbjq.cn/Article/details/ghoakwsaa.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.zdbjq.cn/Article/details/gvdacyybp.sHtML

[T60] Scala：折叠
来源：http://www.share.zdbjq.cn/Article/details/gsvijrtnb.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.zdbjq.cn/Article/details/gsorlawvn.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gdeoizyjk.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.hesvh.cn/Article/details/gxgwkkohf.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gdnouceoq.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.zdbjq.cn/Article/details/gscqksqsd.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.fehbvm.com/Article/details/gdjzezhpb.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.fehbvm.com/Article/details/gtrhjctsm.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.fehbvm.com/Article/details/ggqfnlvrm.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.zdbjq.cn/Article/details/gbmqrlwcn.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.hesvh.cn/Article/details/ghzzdgvbp.sHtML

[U04] Py：变量调试打印
来源：http://wap.fehbvm.com/Article/details/giuymeyys.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.zdbjq.cn/Article/details/gevxamaum.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.fehbvm.com/Article/details/gfphpcvkz.sHtML

list(dict.fromkeys(arr))
来源：http://blog.hesvh.cn/Article/details/gatumaxov.sHtML

[U06] Py：合并两个字典
来源：http://mobile.hesvh.cn/Article/details/gfgkzwmdw.sHtML

{**a, **b}
来源：http://www.blog.fehbvm.com/Article/details/gkaaleryx.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.fehbvm.com/Article/details/gofjnlfes.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.fehbvm.com/Article/details/gqompdfqv.sHtML

[U08] Py：展平二维列表
来源：http://mobile.zdbjq.cn/Article/details/gnganzkvj.sHtML

[y for x in nested for y in x]
来源：http://mobile.hesvh.cn/Article/details/gccxrapwb.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.zdbjq.cn/Article/details/glwmukkud.sHtML

max(d, key=d.get)
来源：http://3g.zdbjq.cn/Article/details/gcsvhbvnc.sHtML

[U10] Py：按值排序字典
来源：http://wap.fehbvm.com/Article/details/gcteqqtyl.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.fehbvm.com/Article/details/gydpxedqg.sHtML

[U11] Py：生成器表达式
来源：http://wap.hesvh.cn/Article/details/goleidaus.sHtML

(x * 2 for x in arr)
来源：http://www.blog.hesvh.cn/Article/details/ghzntgjpu.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.hesvh.cn/Article/details/gchyvhbpf.sHtML

Counter(arr).most_common(3)
来源：http://read.share.hesvh.cn/Article/details/gjzzkvzhr.sHtML

[U13] Py：固定长度队列
来源：http://wap.zdbjq.cn/Article/details/gsvxbilzh.sHtML

deque(maxlen=10)
来源：http://read.share.zdbjq.cn/Article/details/gmgsvwyji.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.hesvh.cn/Article/details/gdnzcxcug.sHtML

defaultdict(list)
来源：http://read.share.hesvh.cn/Article/details/gnvpdmpsq.sHtML

[U15] Py：高精度计时
来源：http://m.share.fehbvm.com/Article/details/gntglzhfc.sHtML

t = time.perf_counter()
来源：http://baike.hesvh.cn/Article/details/gydrvjuyx.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.zdbjq.cn/Article/details/gbycrelpt.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fehbvm.com/Article/details/gnwnitcvl.sHtML

[U17] Py：初始化日志
来源：http://blog.hesvh.cn/Article/details/ggtozehte.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.hesvh.cn/Article/details/gtgyphmbi.sHtML

[U18] Py：预编译正则
来源：http://m.share.fehbvm.com/Article/details/gdeozdypu.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.hesvh.cn/Article/details/ggpggijin.sHtML

[U19] Py：正则替换带回调
来源：http://blog.hesvh.cn/Article/details/guzviboqy.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.hesvh.cn/Article/details/gfkfwpowi.sHtML

[U20] Py：缓存函数结果
来源：http://wap.hesvh.cn/Article/details/gbxwoeiaq.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.fehbvm.com/Article/details/ginibtsxv.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.zdbjq.cn/Article/details/gndkdcebf.sHtML

@contextlib.contextmanager
来源：http://mobile.zdbjq.cn/Article/details/ggrevcmhr.sHtML

[U22] Py：矩阵转置
来源：http://read.share.zdbjq.cn/Article/details/gdlozfrxu.sHtML

list(zip(*m))
来源：http://wap.hesvh.cn/Article/details/gowgmdcrs.sHtML

[U23] Py：分块读取大文件
来源：http://baike.hesvh.cn/Article/details/gyeyuiokj.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.zdbjq.cn/Article/details/gufdsgsoq.sHtML

[U24] Py：路径操作
来源：http://www.share.fehbvm.com/Article/details/gqzdtzbtm.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.fehbvm.com/Article/details/gjrlorkrs.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.zdbjq.cn/Article/details/gmudcukjb.sHtML

csv.DictReader(f)
来源：http://www.share.zdbjq.cn/Article/details/grvdtaoqu.sHtML

[U26] Py：并发下载
来源：http://m.share.fehbvm.com/Article/details/gjcktoiku.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.hesvh.cn/Article/details/godgtdslw.sHtML

[U27] Py：异步 HTTP
来源：http://wap.fehbvm.com/Article/details/gbbjjgwpf.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.hesvh.cn/Article/details/gkuiaxzfy.sHtML

[U28] Py：类型别名
来源：http://mobile.hesvh.cn/Article/details/gjomkmawh.sHtML

UserId = int
来源：http://wap.zdbjq.cn/Article/details/gogpzkfyp.sHtML

[U29] Py：属性校验
来源：http://baike.zdbjq.cn/Article/details/grgadaleg.sHtML

@property 与 @x.setter 配合
来源：http://mobile.zdbjq.cn/Article/details/ggdhrpljq.sHtML

[U30] Py：数据类
来源：http://wap.fehbvm.com/Article/details/ggefihokz.sHtML

@dataclass(slots=True)
来源：http://wap.fehbvm.com/Article/details/gkmxfnejc.sHtML

[U31] Py：单测
来源：http://www.blog.zdbjq.cn/Article/details/gfirzqexy.sHtML

python -m pytest -q
来源：http://baike.hesvh.cn/Article/details/gscyfrvxs.sHtML

[U32] Py：代码格式化
来源：http://www.blog.hesvh.cn/Article/details/gmnzvmlqk.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.fehbvm.com/Article/details/gutwopeae.sHtML

[U33] Py：打包发布
来源：http://www.m.share.hesvh.cn/Article/details/ggstxtepw.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.zdbjq.cn/Article/details/gjkcymzvu.sHtML

[U34] Py：判断编码
来源：http://wap.zdbjq.cn/Article/details/gaejsntls.sHtML

chardet.detect(raw)
来源：http://m.share.fehbvm.com/Article/details/gxvigztzm.sHtML

[U35] Py：发送邮件
来源：http://read.share.fehbvm.com/Article/details/goqoqegri.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.hesvh.cn/Article/details/gxwwdvior.sHtML

[U36] Py：定时任务
来源：http://www.share.zdbjq.cn/Article/details/gughxyczg.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.zdbjq.cn/Article/details/gbwynmseq.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.zdbjq.cn/Article/details/gdpejrmkv.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.hesvh.cn/Article/details/gujksvgeh.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.hesvh.cn/Article/details/gawhlmjqo.sHtML

Path(__file__).resolve().parent
来源：http://m.share.zdbjq.cn/Article/details/gnwhccjwe.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.zdbjq.cn/Article/details/gexjtvywo.sHtML

sys.stdout.isatty()
来源：http://read.share.fehbvm.com/Article/details/ghnoqxrwv.sHtML

[U40] Py：打印到标准错误
来源：http://wap.zdbjq.cn/Article/details/gkighkawy.sHtML

print("err", file=sys.stderr)
来源：http://m.share.zdbjq.cn/Article/details/glimppgxq.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.fehbvm.com/Article/details/gvligqcvg.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.zdbjq.cn/Article/details/gwdjeqqpu.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.hesvh.cn/Article/details/gtzhyiuqy.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.hesvh.cn/Article/details/ginzcmtnu.sHtML

[U43] PHP：声明命名空间
来源：http://wap.fehbvm.com/Article/details/gkkbbbqun.sHtML

namespace App\Http;
来源：http://www.blog.zdbjq.cn/Article/details/gpgvnmphz.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.hesvh.cn/Article/details/gxvywosxk.sHtML

declare(strict_types=1);
来源：http://blog.zdbjq.cn/Article/details/gtlshxujx.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.zdbjq.cn/Article/details/goftjpnfa.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gcjtlxdfi.sHtML

[U46] PHP：可空类型
来源：http://m.share.fehbvm.com/Article/details/gnmhgwsgk.sHtML

?string $name = null
来源：http://m.share.hesvh.cn/Article/details/gboiviksi.sHtML

[U47] PHP：联合类型
来源：http://www.blog.zdbjq.cn/Article/details/gwvbzbvpr.sHtML

int|string $id
来源：http://baike.hesvh.cn/Article/details/geyqinyoj.sHtML

[U48] PHP：纯枚举
来源：http://blog.hesvh.cn/Article/details/gjhxttidx.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.hesvh.cn/Article/details/gkitdfjux.sHtML

[U49] PHP：只读属性
来源：http://wap.hesvh.cn/Article/details/geqsvkewg.sHtML

public readonly string $name
来源：http://blog.fehbvm.com/Article/details/ggmubqfup.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.hesvh.cn/Article/details/gapvmwwzt.sHtML

public function __construct(private int $id) {}
来源：http://wap.zdbjq.cn/Article/details/ggtsluqbw.sHtML

[U51] PHP：数组解构
来源：http://m.share.fehbvm.com/Article/details/gjyadyfhl.sHtML

[$a, $b] = $arr;
来源：http://www.blog.zdbjq.cn/Article/details/gldibznfx.sHtML

[U52] PHP：箭头函数
来源：http://www.share.fehbvm.com/Article/details/gtvuyrvkj.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.zdbjq.cn/Article/details/gytddeqyn.sHtML

[U53] PHP：空合并运算符
来源：http://baike.fehbvm.com/Article/details/gfjpuexco.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.hesvh.cn/Article/details/gpqdzercp.sHtML

[U54] PHP：空安全调用
来源：http://blog.hesvh.cn/Article/details/gcrniycsl.sHtML

$obj?->method()
来源：http://www.blog.hesvh.cn/Article/details/gegbuutkh.sHtML

[U55] PHP：match 表达式
来源：http://baike.zdbjq.cn/Article/details/gsdbckrfn.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.zdbjq.cn/Article/details/gzreauvut.sHtML

[U56] PHP：命名参数
来源：http://www.blog.fehbvm.com/Article/details/gzoafcxza.sHtML

f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/ghesdldip.sHtML

[U57] PHP：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gsdyddfhh.sHtML

"值: {$a}"
来源：http://3g.fehbvm.com/Article/details/gsllowpjw.sHtML

[U58] PHP：数组三件套
来源：http://m.share.fehbvm.com/Article/details/gqkshllub.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.zdbjq.cn/Article/details/ggjwoyzhl.sHtML

[U59] PHP：自定义排序
来源：http://read.share.fehbvm.com/Article/details/ghgondmru.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.zdbjq.cn/Article/details/gblfauovb.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.zdbjq.cn/Article/details/gdbxjwwyx.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.fehbvm.com/Article/details/gmbjrggsu.sHtML

[U61] PHP：正则
来源：http://baike.fehbvm.com/Article/details/gbakayhef.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.hesvh.cn/Article/details/gsggvdryj.sHtML

[U62] PHP：日期对象
来源：http://baike.fehbvm.com/Article/details/gpdjcdpwl.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.hesvh.cn/Article/details/gmxmxtdpa.sHtML

[U63] PHP：文件读写
来源：http://read.share.fehbvm.com/Article/details/goxofxuqc.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.hesvh.cn/Article/details/gphbvhxbi.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gbnzoqkii.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.fehbvm.com/Article/details/golwpmxgc.sHtML

[U65] PHP：会话
来源：http://blog.zdbjq.cn/Article/details/gmushchvz.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gzzpllgjo.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.hesvh.cn/Article/details/gohvfnlkg.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.zdbjq.cn/Article/details/gimujshpb.sHtML

[U67] PHP：处理文件上传
来源：http://wap.zdbjq.cn/Article/details/gjyjrttfk.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.fehbvm.com/Article/details/gsjofiijf.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.hesvh.cn/Article/details/gnwyjnbxo.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.hesvh.cn/Article/details/gwercnnfe.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.zdbjq.cn/Article/details/gowazfinj.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.zdbjq.cn/Article/details/gelmjhqms.sHtML

[U70] PHP：PDO 事务
来源：http://blog.hesvh.cn/Article/details/ghrfoejqh.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.zdbjq.cn/Article/details/gwtubgley.sHtML


<!-- 参考信息 -->