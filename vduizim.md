代发 wailian999

[S39] C++：自定义比较器排序
来源：http://www.share.zdbjq.cn/Article/details/ggcyojxem.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.zdbjq.cn/Article/details/garwtldqt.sHtML

[S40] C++：查找元素
来源：http://www.share.zdbjq.cn/Article/details/ghiqztict.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fehbvm.com/Article/details/gnpevqlmh.sHtML

[S41] C++：类与构造函数
来源：http://baike.zdbjq.cn/Article/details/gitonhwau.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.zdbjq.cn/Article/details/gcglqmonz.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.zdbjq.cn/Article/details/ggxglyibc.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.zdbjq.cn/Article/details/gkdqtplfc.sHtML

[S43] C++：智能指针
来源：http://www.blog.zdbjq.cn/Article/details/ggsemqujn.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fehbvm.com/Article/details/gtyscgzeg.sHtML

[S44] C++：引用传参
来源：http://baike.fehbvm.com/Article/details/gdkbxlfvq.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fehbvm.com/Article/details/gjqlmaotf.sHtML

[S45] C++：lambda
来源：http://baike.hesvh.cn/Article/details/gnakumcvj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fehbvm.com/Article/details/gmptveceo.sHtML

[S46] C++：函数模板
来源：http://baike.hesvh.cn/Article/details/glmogwvui.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fehbvm.com/Article/details/gfgdgmmbe.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.hesvh.cn/Article/details/gkfgszuft.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.zdbjq.cn/Article/details/gomxuihzo.sHtML

[S48] C++：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gxqlkhaje.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.hesvh.cn/Article/details/gchidukcu.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.zdbjq.cn/Article/details/gylnxfeem.sHtML

[S49] C++：写文件
来源：http://mobile.hesvh.cn/Article/details/gcbrgmphf.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.hesvh.cn/Article/details/gphejvmcr.sHtML

[S50] C++：格式化数字
来源：http://wap.fehbvm.com/Article/details/gxbzyjksm.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gqsuwtiak.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fehbvm.com/Article/details/gyjdkjhkm.sHtML

static_cast<double>(a) / b
来源：http://mobile.hesvh.cn/Article/details/gqttukzuo.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.zdbjq.cn/Article/details/gjjtepvyg.sHtML

int size() const noexcept { return n_; }
来源：http://blog.zdbjq.cn/Article/details/guadlhyur.sHtML

[S53] C++：移动语义
来源：http://blog.hesvh.cn/Article/details/gsrxtzqol.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.zdbjq.cn/Article/details/gpiaeoscq.sHtML

[S54] C++：异常处理
来源：http://blog.hesvh.cn/Article/details/gjmdtnlqj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fehbvm.com/Article/details/gzthvkfqv.sHtML

[S55] C++：结构化绑定
来源：http://baike.fehbvm.com/Article/details/gkewdjkrb.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.hesvh.cn/Article/details/gzbanlamm.sHtML

[S56] C++：optional
来源：http://3g.fehbvm.com/Article/details/gigwepmkl.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.hesvh.cn/Article/details/gbcyvozxu.sHtML

[S57] C++：编译期常量
来源：http://blog.fehbvm.com/Article/details/gxinmwcmv.sHtML

constexpr int N = 10;
来源：http://mobile.hesvh.cn/Article/details/glckmjepj.sHtML

[S58] C++：命名空间
来源：http://baike.hesvh.cn/Article/details/gvzxxfswe.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gceyjqmzq.sHtML

[S59] C++：静态断言
来源：http://blog.hesvh.cn/Article/details/gorarvsup.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.zdbjq.cn/Article/details/gqcxoekul.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.zdbjq.cn/Article/details/gshrphdiy.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.hesvh.cn/Article/details/gobvjzzsw.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gfqkqwafk.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fehbvm.com/Article/details/gsxrodrmi.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/girzuhrpx.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.zdbjq.cn/Article/details/ghperlqnm.sHtML

println("Hello")
来源：http://m.share.fehbvm.com/Article/details/grhdtdxxh.sHtML

[T02] Kotlin：变量
来源：http://m.share.zdbjq.cn/Article/details/gzxlgmeqt.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.zdbjq.cn/Article/details/gakebymkw.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.zdbjq.cn/Article/details/gsyoaiflp.sHtML

"值: $b"
来源：http://www.blog.hesvh.cn/Article/details/gdrtngbhz.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.zdbjq.cn/Article/details/gorevxgcc.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fehbvm.com/Article/details/gvhojrzdq.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.hesvh.cn/Article/details/gvqqcnrzy.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.hesvh.cn/Article/details/gzlahxyet.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.hesvh.cn/Article/details/gufdqkeqm.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gzzdnfrll.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fehbvm.com/Article/details/gzaynfcof.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fehbvm.com/Article/details/gwrvbxawe.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fehbvm.com/Article/details/gtayneusn.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fehbvm.com/Article/details/giiahrsgj.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.zdbjq.cn/Article/details/gtkzrasqo.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.zdbjq.cn/Article/details/gvrjnesgi.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.hesvh.cn/Article/details/gozcbmtul.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.hesvh.cn/Article/details/gklqwuxrr.sHtML

[T11] Kotlin：协程
来源：http://blog.zdbjq.cn/Article/details/gmmetbdtz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.hesvh.cn/Article/details/gvogecook.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.zdbjq.cn/Article/details/glhafvabl.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fehbvm.com/Article/details/gxgyqifjm.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.hesvh.cn/Article/details/gulettxop.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fehbvm.com/Article/details/gjkqxmlkc.sHtML

[T14] Kotlin：循环
来源：http://baike.zdbjq.cn/Article/details/gmlqzmutu.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.zdbjq.cn/Article/details/gtqhdjeyt.sHtML

[T15] Kotlin：接口
来源：http://blog.fehbvm.com/Article/details/gqesqegap.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.hesvh.cn/Article/details/gwqciqivs.sHtML

[T16] Swift：Hello World
来源：http://www.share.fehbvm.com/Article/details/grqcrxisg.sHtML

print("Hello")
来源：http://blog.fehbvm.com/Article/details/gcvgcvgbg.sHtML

[T17] Swift：变量与常量
来源：http://blog.zdbjq.cn/Article/details/gbafsaysq.sHtML

var a = 1;  let b = 2
来源：http://m.share.hesvh.cn/Article/details/gxumvytdg.sHtML

[T18] Swift：字符串插值
来源：http://3g.zdbjq.cn/Article/details/ghdpacvzg.sHtML

"值: \(b)"
来源：http://wap.hesvh.cn/Article/details/geffyegvb.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fehbvm.com/Article/details/gvpbgddlq.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fehbvm.com/Article/details/gqwupwdit.sHtML

[T20] Swift：数组操作
来源：http://www.share.fehbvm.com/Article/details/gamgovxaf.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.zdbjq.cn/Article/details/guhzifdhc.sHtML

[T21] Swift：遍历
来源：http://blog.hesvh.cn/Article/details/gbwbgwvre.sHtML

for x in a { print(x) }
来源：http://www.share.hesvh.cn/Article/details/gapysqewh.sHtML

[T22] Swift：字典
来源：http://www.m.share.fehbvm.com/Article/details/ggccgyreo.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.fehbvm.com/Article/details/gwkpzhbqn.sHtML

[T23] Swift：函数
来源：http://wap.hesvh.cn/Article/details/glipkhgnb.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.hesvh.cn/Article/details/ghzyvlajw.sHtML

[T24] Swift：闭包
来源：http://read.share.zdbjq.cn/Article/details/gfcdeciag.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fehbvm.com/Article/details/gasjfzadr.sHtML

[T25] Swift：结构体
来源：http://read.share.fehbvm.com/Article/details/gscpzcrlj.sHtML

struct P { var x: Int }
来源：http://mobile.zdbjq.cn/Article/details/gswmcsyzp.sHtML

[T26] Swift：类与重写
来源：http://wap.fehbvm.com/Article/details/gujrmdqkl.sHtML

class A: Base { override func f() {} }
来源：http://www.share.hesvh.cn/Article/details/gmjnkatvk.sHtML

[T27] Swift：错误处理
来源：http://www.blog.zdbjq.cn/Article/details/gaxmppovx.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.fehbvm.com/Article/details/gkciuswoi.sHtML

[T28] Swift：枚举
来源：http://www.m.share.hesvh.cn/Article/details/glgbgmgyj.sHtML

enum Color { case red, green }
来源：http://m.share.fehbvm.com/Article/details/gaypbxwyp.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fehbvm.com/Article/details/gdudfrkdj.sHtML

guard let x = opt else { return }
来源：http://mobile.fehbvm.com/Article/details/giccxhxbl.sHtML

[T30] Swift：协议
来源：http://baike.zdbjq.cn/Article/details/gxpykgfxk.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.zdbjq.cn/Article/details/gcqnjsvsq.sHtML

[T31] Lua：Hello World
来源：http://3g.zdbjq.cn/Article/details/gpsuxworc.sHtML

print("Hello")
来源：http://wap.fehbvm.com/Article/details/gyfyzpmvv.sHtML

[T32] Lua：局部变量
来源：http://m.share.fehbvm.com/Article/details/gtosarcbh.sHtML

local a = 1
来源：http://m.share.fehbvm.com/Article/details/goaxuwrgm.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.fehbvm.com/Article/details/gedelwlcq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.hesvh.cn/Article/details/glqpymldg.sHtML

[T34] Lua：遍历表
来源：http://3g.zdbjq.cn/Article/details/gunmqaztu.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.hesvh.cn/Article/details/gpaovqlbn.sHtML

[T35] Lua：字典表
来源：http://www.m.share.hesvh.cn/Article/details/gjhxwwjqv.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.hesvh.cn/Article/details/gtseagazf.sHtML

[T36] Lua：函数
来源：http://mobile.hesvh.cn/Article/details/gnzzmiylj.sHtML

function add(a, b) return a + b end
来源：http://blog.hesvh.cn/Article/details/gywanzxgo.sHtML

[T37] Lua：字符串拼接
来源：http://wap.zdbjq.cn/Article/details/gsewkthlp.sHtML

"a" .. "b"
来源：http://m.share.zdbjq.cn/Article/details/gprjqcuuu.sHtML

[T38] Lua：条件
来源：http://baike.zdbjq.cn/Article/details/gnwkwykfl.sHtML

if x > 0 then print("正") end
来源：http://wap.zdbjq.cn/Article/details/goycqvdnr.sHtML

[T39] Lua：模式匹配
来源：http://mobile.hesvh.cn/Article/details/ggrmlssfi.sHtML

string.find(s, "%d+")
来源：http://read.share.hesvh.cn/Article/details/gvfuypkoz.sHtML

[T40] Lua：元表
来源：http://www.share.fehbvm.com/Article/details/gbrxpgopk.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.fehbvm.com/Article/details/ghoscnvuc.sHtML

[T41] Perl：Hello World
来源：http://m.share.hesvh.cn/Article/details/gvvdhtqtw.sHtML

print "Hello\n";
来源：http://www.share.zdbjq.cn/Article/details/ghyxmysbn.sHtML

[T42] Perl：变量类型
来源：http://3g.hesvh.cn/Article/details/gebjpvetk.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.zdbjq.cn/Article/details/guxxjdvjc.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gierttfty.sHtML

"值: $a"
来源：http://www.share.hesvh.cn/Article/details/gjmuuedks.sHtML

[T44] Perl：条件
来源：http://www.blog.hesvh.cn/Article/details/gmzqcovwt.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.zdbjq.cn/Article/details/gvvbwbbdz.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.fehbvm.com/Article/details/gwqxfttsy.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.hesvh.cn/Article/details/gykzetfwd.sHtML

[T46] Perl：哈希操作
来源：http://baike.fehbvm.com/Article/details/gezyfpumn.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.zdbjq.cn/Article/details/gcvujpiva.sHtML

[T47] Perl：正则捕获
来源：http://3g.fehbvm.com/Article/details/guaabxzfb.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.fehbvm.com/Article/details/gvtqbvbpi.sHtML

[T48] Perl：正则替换
来源：http://blog.fehbvm.com/Article/details/gbjmvkpui.sHtML

$s =~ s/old/new/g;
来源：http://wap.fehbvm.com/Article/details/gcqzvbzgv.sHtML

[T49] Perl：函数
来源：http://blog.fehbvm.com/Article/details/gvvphnuzz.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/gdtiaeqno.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/glpyfravm.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.hesvh.cn/Article/details/gmtaxsjox.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.hesvh.cn/Article/details/grcaprpov.sHtML

[T51] Scala：Hello World
来源：http://blog.zdbjq.cn/Article/details/gjolgpvte.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/gygqyfwys.sHtML

[T52] Scala：变量
来源：http://www.m.share.hesvh.cn/Article/details/gkbybfbkz.sHtML

val a = 1;  var b = 2
来源：http://blog.fehbvm.com/Article/details/gihrzyjjj.sHtML

[T53] Scala：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/girkwfhhv.sHtML

s"值: $b"
来源：http://mobile.fehbvm.com/Article/details/gpekgcuyr.sHtML

[T54] Scala：集合映射
来源：http://www.share.zdbjq.cn/Article/details/gxdyacsay.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.zdbjq.cn/Article/details/gqgunsxge.sHtML

[T55] Scala：集合过滤
来源：http://3g.zdbjq.cn/Article/details/gfidhcfzx.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.zdbjq.cn/Article/details/gqkagabnn.sHtML

[T56] Scala：样例类
来源：http://m.share.fehbvm.com/Article/details/gffoxdpnj.sHtML

case class User(name: String, age: Int)
来源：http://3g.fehbvm.com/Article/details/gsjculicr.sHtML

[T57] Scala：模式匹配
来源：http://blog.zdbjq.cn/Article/details/gdyltwgiu.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.hesvh.cn/Article/details/ghzciucve.sHtML

[T58] Scala：函数定义
来源：http://www.blog.hesvh.cn/Article/details/gwyounohn.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.fehbvm.com/Article/details/gglcfaibj.sHtML

[T59] Scala：循环
来源：http://blog.hesvh.cn/Article/details/gaznwfxxq.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.fehbvm.com/Article/details/gbmsxdfaj.sHtML

[T60] Scala：折叠
来源：http://3g.fehbvm.com/Article/details/gdrlnihcw.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.zdbjq.cn/Article/details/grdmrggez.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gpvtwcpnb.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.zdbjq.cn/Article/details/gjxznuwhg.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gpgrfjadf.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.fehbvm.com/Article/details/gukkzagse.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.hesvh.cn/Article/details/gaqrmmljt.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.zdbjq.cn/Article/details/gjhgnoflq.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.hesvh.cn/Article/details/gveamftxh.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.zdbjq.cn/Article/details/gokdhdepg.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.hesvh.cn/Article/details/grjgvfntg.sHtML

[U04] Py：变量调试打印
来源：http://read.share.zdbjq.cn/Article/details/gghvjwpkg.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.fehbvm.com/Article/details/gcermbcjg.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.zdbjq.cn/Article/details/garauuvfn.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.fehbvm.com/Article/details/gaoodzurr.sHtML

[U06] Py：合并两个字典
来源：http://mobile.fehbvm.com/Article/details/gjvbrzaeq.sHtML

{**a, **b}
来源：http://read.share.zdbjq.cn/Article/details/gvfkeqjbu.sHtML

[U07] Py：反转字典键值
来源：http://read.share.fehbvm.com/Article/details/gyzocvjue.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.hesvh.cn/Article/details/ganuqhtjc.sHtML

[U08] Py：展平二维列表
来源：http://mobile.hesvh.cn/Article/details/giqtwacrr.sHtML

[y for x in nested for y in x]
来源：http://read.share.hesvh.cn/Article/details/gucrdogrk.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.fehbvm.com/Article/details/gezsuwzqq.sHtML

max(d, key=d.get)
来源：http://baike.fehbvm.com/Article/details/gfddjsbho.sHtML

[U10] Py：按值排序字典
来源：http://read.share.hesvh.cn/Article/details/guavfhcya.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.zdbjq.cn/Article/details/giykijvmz.sHtML

[U11] Py：生成器表达式
来源：http://mobile.fehbvm.com/Article/details/gthystcyz.sHtML

(x * 2 for x in arr)
来源：http://www.blog.fehbvm.com/Article/details/gymmwbsgb.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.hesvh.cn/Article/details/gusrovorf.sHtML

Counter(arr).most_common(3)
来源：http://read.share.fehbvm.com/Article/details/glsvejuhd.sHtML

[U13] Py：固定长度队列
来源：http://baike.hesvh.cn/Article/details/gcwajhqvf.sHtML

deque(maxlen=10)
来源：http://baike.zdbjq.cn/Article/details/gtrwhtaei.sHtML

[U14] Py：分组收集到列表
来源：http://3g.hesvh.cn/Article/details/ggcjnliju.sHtML

defaultdict(list)
来源：http://mobile.fehbvm.com/Article/details/gwshqwdwi.sHtML

[U15] Py：高精度计时
来源：http://baike.hesvh.cn/Article/details/ggqptenth.sHtML

t = time.perf_counter()
来源：http://3g.hesvh.cn/Article/details/gnoofhwfd.sHtML

[U16] Py：命令行参数解析
来源：http://baike.fehbvm.com/Article/details/glvkhesmm.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.fehbvm.com/Article/details/gshpalztf.sHtML

[U17] Py：初始化日志
来源：http://wap.fehbvm.com/Article/details/gvyplbupz.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.zdbjq.cn/Article/details/gswjmrbcb.sHtML

[U18] Py：预编译正则
来源：http://wap.fehbvm.com/Article/details/gzhkjntfd.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.fehbvm.com/Article/details/gndsutkdp.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.hesvh.cn/Article/details/gvqhempfv.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.zdbjq.cn/Article/details/gjaepnrue.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.fehbvm.com/Article/details/gcxnyokmw.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.fehbvm.com/Article/details/ggkzalsqs.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.zdbjq.cn/Article/details/gqyfmgfeb.sHtML

@contextlib.contextmanager
来源：http://m.share.fehbvm.com/Article/details/gsdoryvrk.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.zdbjq.cn/Article/details/gluamxheq.sHtML

list(zip(*m))
来源：http://www.m.share.hesvh.cn/Article/details/gayakisua.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.hesvh.cn/Article/details/gmuhjbbjb.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.fehbvm.com/Article/details/gvbrdjldg.sHtML

[U24] Py：路径操作
来源：http://www.share.hesvh.cn/Article/details/ggclcfsfo.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/gugvplrix.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.zdbjq.cn/Article/details/gtivabptu.sHtML

csv.DictReader(f)
来源：http://3g.fehbvm.com/Article/details/gyhmekenk.sHtML

[U26] Py：并发下载
来源：http://www.m.share.fehbvm.com/Article/details/gnfjxkhtp.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.hesvh.cn/Article/details/gvuggprwk.sHtML

[U27] Py：异步 HTTP
来源：http://3g.fehbvm.com/Article/details/guoqaodyf.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.zdbjq.cn/Article/details/geifomdgb.sHtML

[U28] Py：类型别名
来源：http://mobile.zdbjq.cn/Article/details/gepuftnyt.sHtML

UserId = int
来源：http://www.blog.hesvh.cn/Article/details/gypqkscha.sHtML

[U29] Py：属性校验
来源：http://mobile.zdbjq.cn/Article/details/gpepdbfoq.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.zdbjq.cn/Article/details/grigbyrvq.sHtML

[U30] Py：数据类
来源：http://www.m.share.zdbjq.cn/Article/details/gshnfmsgj.sHtML

@dataclass(slots=True)
来源：http://www.m.share.fehbvm.com/Article/details/gigwpdxgl.sHtML

[U31] Py：单测
来源：http://www.m.share.fehbvm.com/Article/details/gqjezfwty.sHtML

python -m pytest -q
来源：http://wap.hesvh.cn/Article/details/ggukbkizp.sHtML

[U32] Py：代码格式化
来源：http://www.blog.zdbjq.cn/Article/details/gobeyecie.sHtML

ruff format . && ruff check --fix .
来源：http://blog.zdbjq.cn/Article/details/gnykkvqep.sHtML

[U33] Py：打包发布
来源：http://3g.fehbvm.com/Article/details/ghjmndxae.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.zdbjq.cn/Article/details/gmmccjfld.sHtML

[U34] Py：判断编码
来源：http://www.blog.hesvh.cn/Article/details/gsauvehvd.sHtML

chardet.detect(raw)
来源：http://www.m.share.hesvh.cn/Article/details/gqyszueap.sHtML

[U35] Py：发送邮件
来源：http://m.share.hesvh.cn/Article/details/gcdkmmpta.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.hesvh.cn/Article/details/gffvkgpvo.sHtML

[U36] Py：定时任务
来源：http://3g.zdbjq.cn/Article/details/gnslncowz.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.zdbjq.cn/Article/details/gyyfdttwv.sHtML

[U37] Py：读写 Excel
来源：http://baike.fehbvm.com/Article/details/gvqrijjic.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.zdbjq.cn/Article/details/gkcvftbij.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.fehbvm.com/Article/details/gcxfijozh.sHtML

Path(__file__).resolve().parent
来源：http://www.share.hesvh.cn/Article/details/gnxtedfpt.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.zdbjq.cn/Article/details/gujxahdsl.sHtML

sys.stdout.isatty()
来源：http://3g.fehbvm.com/Article/details/gqxqjwysl.sHtML

[U40] Py：打印到标准错误
来源：http://wap.zdbjq.cn/Article/details/gpijvqsww.sHtML

print("err", file=sys.stderr)
来源：http://mobile.hesvh.cn/Article/details/gyvtlkoze.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.fehbvm.com/Article/details/gffahutgn.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.zdbjq.cn/Article/details/gqkwoiiaa.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.fehbvm.com/Article/details/gjkzybkcp.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.zdbjq.cn/Article/details/gjhapqyfx.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.fehbvm.com/Article/details/gwhzoipyb.sHtML

namespace App\Http;
来源：http://www.m.share.hesvh.cn/Article/details/gsymizkzb.sHtML

[U44] PHP：开启严格类型
来源：http://3g.fehbvm.com/Article/details/gwbthnymp.sHtML

declare(strict_types=1);
来源：http://mobile.hesvh.cn/Article/details/gqnalwyzm.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.hesvh.cn/Article/details/ghnoscoyd.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/grqjktqyc.sHtML

[U46] PHP：可空类型
来源：http://wap.fehbvm.com/Article/details/gyyaezumz.sHtML

?string $name = null
来源：http://www.share.zdbjq.cn/Article/details/gpqlpswnz.sHtML

[U47] PHP：联合类型
来源：http://www.blog.fehbvm.com/Article/details/gihnfjokc.sHtML

int|string $id
来源：http://blog.fehbvm.com/Article/details/gsuuhbcid.sHtML

[U48] PHP：纯枚举
来源：http://wap.zdbjq.cn/Article/details/gaqrryoeh.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.hesvh.cn/Article/details/gshbtvonz.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.zdbjq.cn/Article/details/gihnbjcop.sHtML

public readonly string $name
来源：http://www.m.share.hesvh.cn/Article/details/gvwkfjgde.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.hesvh.cn/Article/details/gccjfdsyg.sHtML

public function __construct(private int $id) {}
来源：http://blog.hesvh.cn/Article/details/grvzwgtiw.sHtML

[U51] PHP：数组解构
来源：http://baike.zdbjq.cn/Article/details/gpzioawbw.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.fehbvm.com/Article/details/gfrqvvcoo.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.fehbvm.com/Article/details/gihernhwp.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.zdbjq.cn/Article/details/gtidvannr.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.hesvh.cn/Article/details/gmrrlxcez.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.hesvh.cn/Article/details/gfohocrjp.sHtML

[U54] PHP：空安全调用
来源：http://3g.zdbjq.cn/Article/details/gphqdqsty.sHtML

$obj?->method()
来源：http://baike.zdbjq.cn/Article/details/gplpbjins.sHtML

[U55] PHP：match 表达式
来源：http://wap.hesvh.cn/Article/details/ggqmjrguo.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.zdbjq.cn/Article/details/grcdjgdmq.sHtML

[U56] PHP：命名参数
来源：http://www.blog.hesvh.cn/Article/details/ghfubalxk.sHtML

f(a: 1, b: 2)
来源：http://3g.zdbjq.cn/Article/details/gpzmwdnxs.sHtML

[U57] PHP：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gnmsgiref.sHtML

"值: {$a}"
来源：http://wap.hesvh.cn/Article/details/geweskqdk.sHtML

[U58] PHP：数组三件套
来源：http://blog.hesvh.cn/Article/details/gblxojbvx.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.fehbvm.com/Article/details/gzxptunjx.sHtML

[U59] PHP：自定义排序
来源：http://mobile.hesvh.cn/Article/details/gptvupiqj.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.zdbjq.cn/Article/details/gduaptcoi.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.zdbjq.cn/Article/details/gaybojzbv.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.fehbvm.com/Article/details/gvrfrhxxb.sHtML

[U61] PHP：正则
来源：http://wap.hesvh.cn/Article/details/gmzsbejtc.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gmwhhnihf.sHtML

[U62] PHP：日期对象
来源：http://blog.hesvh.cn/Article/details/gbplyqycf.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.zdbjq.cn/Article/details/gqgkiirnw.sHtML

[U63] PHP：文件读写
来源：http://www.share.zdbjq.cn/Article/details/getmgtzns.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.fehbvm.com/Article/details/gxzabkjvg.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.zdbjq.cn/Article/details/gwcbfjlme.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.fehbvm.com/Article/details/gjhlmucwu.sHtML


<!-- 参考信息 -->