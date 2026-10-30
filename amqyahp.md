代发 wailian999

[S37] C++：set
来源：http://www.share.hesvh.cn/Article/details/gpvuxavdv.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.hesvh.cn/Article/details/glkylmhal.sHtML

[S38] C++：排序
来源：http://blog.hesvh.cn/Article/details/gyorgsmmr.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.zdbjq.cn/Article/details/gbzemzfak.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.zdbjq.cn/Article/details/gjmhytxyp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.zdbjq.cn/Article/details/ghyjpkcha.sHtML

[S40] C++：查找元素
来源：http://read.share.zdbjq.cn/Article/details/gqwtazcqz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fehbvm.com/Article/details/gpgskgigy.sHtML

[S41] C++：类与构造函数
来源：http://blog.zdbjq.cn/Article/details/gwokorxsy.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fehbvm.com/Article/details/gaidwmduf.sHtML

[S42] C++：继承与虚函数
来源：http://baike.hesvh.cn/Article/details/gipgcglvm.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.hesvh.cn/Article/details/gamxbotfq.sHtML

[S43] C++：智能指针
来源：http://blog.zdbjq.cn/Article/details/gycjteceb.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.zdbjq.cn/Article/details/gfyydwnvj.sHtML

[S44] C++：引用传参
来源：http://read.share.fehbvm.com/Article/details/gajyffnpq.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fehbvm.com/Article/details/gopsrdsdo.sHtML

[S45] C++：lambda
来源：http://m.share.zdbjq.cn/Article/details/gpdkrtcfn.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.hesvh.cn/Article/details/gamxxnhtd.sHtML

[S46] C++：函数模板
来源：http://blog.fehbvm.com/Article/details/gitkcrrpl.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.hesvh.cn/Article/details/ghnegmfmw.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fehbvm.com/Article/details/gbpkyrxni.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.zdbjq.cn/Article/details/ghrrjlwdn.sHtML

[S48] C++：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/guwyrhcvn.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fehbvm.com/Article/details/gvticakmi.sHtML

while (std::getline(in, line)) { }
来源：http://blog.hesvh.cn/Article/details/gbwbwkvre.sHtML

[S49] C++：写文件
来源：http://mobile.zdbjq.cn/Article/details/gyeczxxab.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.zdbjq.cn/Article/details/grtkwyqaf.sHtML

[S50] C++：格式化数字
来源：http://baike.fehbvm.com/Article/details/goziheppq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/giyjqeslt.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.hesvh.cn/Article/details/gktemcxuh.sHtML

static_cast<double>(a) / b
来源：http://www.share.zdbjq.cn/Article/details/gcukizahm.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.hesvh.cn/Article/details/gxwzxsscl.sHtML

int size() const noexcept { return n_; }
来源：http://wap.hesvh.cn/Article/details/gvzokfhvg.sHtML

[S53] C++：移动语义
来源：http://read.share.hesvh.cn/Article/details/gfpqyakxh.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.zdbjq.cn/Article/details/gsxwtfern.sHtML

[S54] C++：异常处理
来源：http://3g.hesvh.cn/Article/details/grbdedslz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.hesvh.cn/Article/details/gouojljag.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fehbvm.com/Article/details/gjvqdzdkr.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fehbvm.com/Article/details/gzqornwtt.sHtML

[S56] C++：optional
来源：http://mobile.fehbvm.com/Article/details/gkktrnmnw.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fehbvm.com/Article/details/gjgxzonfa.sHtML

[S57] C++：编译期常量
来源：http://baike.zdbjq.cn/Article/details/gleeadont.sHtML

constexpr int N = 10;
来源：http://www.share.zdbjq.cn/Article/details/gjkdgyfab.sHtML

[S58] C++：命名空间
来源：http://blog.fehbvm.com/Article/details/gcrebpbhq.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.zdbjq.cn/Article/details/geijampwg.sHtML

[S59] C++：静态断言
来源：http://mobile.zdbjq.cn/Article/details/gjttwuonn.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.zdbjq.cn/Article/details/gtnvfvvzn.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.zdbjq.cn/Article/details/gnesnjiii.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fehbvm.com/Article/details/gbiihqeki.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gkexolnwp.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fehbvm.com/Article/details/gfmjmtctw.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gjrisomyh.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gthrvuiuc.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gjsbzqhge.sHtML

[T02] Kotlin：变量
来源：http://baike.fehbvm.com/Article/details/gqxhwtsmr.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fehbvm.com/Article/details/gzkglxcjx.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.zdbjq.cn/Article/details/gdwwsuqhe.sHtML

"值: $b"
来源：http://baike.hesvh.cn/Article/details/grirrrbja.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fehbvm.com/Article/details/gaglvbgnt.sHtML

val n: String? = null;  n?.length
来源：http://wap.fehbvm.com/Article/details/gfaosszru.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fehbvm.com/Article/details/ghyaqiuru.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fehbvm.com/Article/details/geywdisub.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.zdbjq.cn/Article/details/ghzprtecx.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fehbvm.com/Article/details/gewccbaga.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.zdbjq.cn/Article/details/gholkgpwf.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.zdbjq.cn/Article/details/goovkuagn.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.hesvh.cn/Article/details/gmgiewryp.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.hesvh.cn/Article/details/gdxdwcwnt.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.hesvh.cn/Article/details/gunqvgixe.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fehbvm.com/Article/details/gheosfapq.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fehbvm.com/Article/details/gfmaoanlx.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.zdbjq.cn/Article/details/gjfcytqam.sHtML

[T11] Kotlin：协程
来源：http://baike.zdbjq.cn/Article/details/gjzhuumzz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.hesvh.cn/Article/details/gkpgxytuj.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.hesvh.cn/Article/details/gewarsasv.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gbbnkwoit.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fehbvm.com/Article/details/gjgmtvqze.sHtML

val m = mapOf("a" to 1)
来源：http://blog.zdbjq.cn/Article/details/gjeywscfk.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.zdbjq.cn/Article/details/gbpmbadfv.sHtML

for (i in 1..10) println(i)
来源：http://m.share.zdbjq.cn/Article/details/gogsnlwgy.sHtML

[T15] Kotlin：接口
来源：http://mobile.zdbjq.cn/Article/details/gqgyzvwaa.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.zdbjq.cn/Article/details/gwkrntqyt.sHtML

[T16] Swift：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gksoqpeps.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/glvdytfgf.sHtML

[T17] Swift：变量与常量
来源：http://read.share.zdbjq.cn/Article/details/gqqltbsal.sHtML

var a = 1;  let b = 2
来源：http://baike.zdbjq.cn/Article/details/gqvvraywr.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gjuldsytv.sHtML

"值: \(b)"
来源：http://m.share.zdbjq.cn/Article/details/gqbabcnfv.sHtML

[T19] Swift：可选绑定
来源：http://mobile.hesvh.cn/Article/details/gyaaxlnxf.sHtML

if let n = opt { print(n) }
来源：http://m.share.hesvh.cn/Article/details/geczfmslr.sHtML

[T20] Swift：数组操作
来源：http://www.blog.zdbjq.cn/Article/details/gznvyqmdf.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.zdbjq.cn/Article/details/gnkzhaubd.sHtML

[T21] Swift：遍历
来源：http://www.blog.hesvh.cn/Article/details/gwezemxso.sHtML

for x in a { print(x) }
来源：http://www.share.zdbjq.cn/Article/details/glkiezjut.sHtML

[T22] Swift：字典
来源：http://m.share.hesvh.cn/Article/details/gxhyhshor.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.zdbjq.cn/Article/details/glsmsmzjf.sHtML

[T23] Swift：函数
来源：http://www.share.fehbvm.com/Article/details/gqragbnhr.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.zdbjq.cn/Article/details/ggbhwahvg.sHtML

[T24] Swift：闭包
来源：http://wap.hesvh.cn/Article/details/gfkjznrkq.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.hesvh.cn/Article/details/gikhuwxik.sHtML

[T25] Swift：结构体
来源：http://read.share.fehbvm.com/Article/details/gtpnfptxn.sHtML

struct P { var x: Int }
来源：http://read.share.hesvh.cn/Article/details/gxrirlqgh.sHtML

[T26] Swift：类与重写
来源：http://read.share.fehbvm.com/Article/details/gjgnsgjll.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fehbvm.com/Article/details/gjidgkbcu.sHtML

[T27] Swift：错误处理
来源：http://www.blog.zdbjq.cn/Article/details/glmiuqdht.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fehbvm.com/Article/details/gtgvpzhnm.sHtML

[T28] Swift：枚举
来源：http://mobile.hesvh.cn/Article/details/gnsprbypa.sHtML

enum Color { case red, green }
来源：http://www.m.share.hesvh.cn/Article/details/gfrlromwj.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.fehbvm.com/Article/details/gapnvuimo.sHtML

guard let x = opt else { return }
来源：http://read.share.zdbjq.cn/Article/details/gkjvmzjbi.sHtML

[T30] Swift：协议
来源：http://www.blog.fehbvm.com/Article/details/gzzxwtvct.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.zdbjq.cn/Article/details/gtigtrzdx.sHtML

[T31] Lua：Hello World
来源：http://baike.zdbjq.cn/Article/details/ghinchxib.sHtML

print("Hello")
来源：http://m.share.fehbvm.com/Article/details/gshgwfyby.sHtML

[T32] Lua：局部变量
来源：http://3g.fehbvm.com/Article/details/gvlqsfqsc.sHtML

local a = 1
来源：http://blog.fehbvm.com/Article/details/glnkkjljh.sHtML

[T33] Lua：表（数组）
来源：http://mobile.fehbvm.com/Article/details/ghvsctkwl.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.hesvh.cn/Article/details/gfjvopmrn.sHtML

[T34] Lua：遍历表
来源：http://baike.fehbvm.com/Article/details/gnuvolhdw.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.hesvh.cn/Article/details/gkptwhkbi.sHtML

[T35] Lua：字典表
来源：http://www.m.share.zdbjq.cn/Article/details/gymkatsbl.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.zdbjq.cn/Article/details/gokgvyeaf.sHtML

[T36] Lua：函数
来源：http://blog.hesvh.cn/Article/details/gkhejwqqv.sHtML

function add(a, b) return a + b end
来源：http://mobile.zdbjq.cn/Article/details/glvjovjhw.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/gpvssldxb.sHtML

"a" .. "b"
来源：http://baike.fehbvm.com/Article/details/gylvldinz.sHtML

[T38] Lua：条件
来源：http://www.blog.fehbvm.com/Article/details/gdfajknbf.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.fehbvm.com/Article/details/gxocjamxw.sHtML

[T39] Lua：模式匹配
来源：http://mobile.fehbvm.com/Article/details/gtnkfyfyq.sHtML

string.find(s, "%d+")
来源：http://www.share.hesvh.cn/Article/details/gbedbmmzq.sHtML

[T40] Lua：元表
来源：http://read.share.hesvh.cn/Article/details/gclmnuoex.sHtML

setmetatable({}, { __index = base })
来源：http://blog.hesvh.cn/Article/details/gcvntcogd.sHtML

[T41] Perl：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gkxlnzpmx.sHtML

print "Hello\n";
来源：http://m.share.fehbvm.com/Article/details/gsydlxpgk.sHtML

[T42] Perl：变量类型
来源：http://wap.hesvh.cn/Article/details/gbomwiqjc.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.zdbjq.cn/Article/details/gmnomindd.sHtML

[T43] Perl：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gxxwgyzio.sHtML

"值: $a"
来源：http://blog.hesvh.cn/Article/details/gefuyxwlx.sHtML

[T44] Perl：条件
来源：http://www.share.hesvh.cn/Article/details/gbohlckne.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.zdbjq.cn/Article/details/gtispadyw.sHtML

[T45] Perl：数组遍历
来源：http://blog.hesvh.cn/Article/details/grnhzsufm.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.hesvh.cn/Article/details/giuwhjinx.sHtML

[T46] Perl：哈希操作
来源：http://m.share.hesvh.cn/Article/details/gelklzzwq.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.fehbvm.com/Article/details/gmdamnclf.sHtML

[T47] Perl：正则捕获
来源：http://3g.zdbjq.cn/Article/details/gfqjzxskk.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.hesvh.cn/Article/details/gtrzgjqly.sHtML

[T48] Perl：正则替换
来源：http://baike.zdbjq.cn/Article/details/gtffpcbpl.sHtML

$s =~ s/old/new/g;
来源：http://baike.hesvh.cn/Article/details/gaeddpkyj.sHtML

[T49] Perl：函数
来源：http://www.blog.zdbjq.cn/Article/details/grtmaqvuv.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gilqemgsy.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gurlqxfvl.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.fehbvm.com/Article/details/gsjeyctsq.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.hesvh.cn/Article/details/gzgwkibia.sHtML

[T51] Scala：Hello World
来源：http://m.share.fehbvm.com/Article/details/gnqosbusr.sHtML

println("Hello")
来源：http://read.share.fehbvm.com/Article/details/guqzeegxq.sHtML

[T52] Scala：变量
来源：http://www.m.share.fehbvm.com/Article/details/gnyupnkdi.sHtML

val a = 1;  var b = 2
来源：http://wap.zdbjq.cn/Article/details/gkiqvvmbi.sHtML

[T53] Scala：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gcbgvfdeu.sHtML

s"值: $b"
来源：http://blog.fehbvm.com/Article/details/gnoidbemo.sHtML

[T54] Scala：集合映射
来源：http://www.share.zdbjq.cn/Article/details/gjouizmhl.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.zdbjq.cn/Article/details/guzmgoaet.sHtML

[T55] Scala：集合过滤
来源：http://mobile.fehbvm.com/Article/details/gidjdpfqu.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.hesvh.cn/Article/details/gbdidauhx.sHtML

[T56] Scala：样例类
来源：http://mobile.fehbvm.com/Article/details/gkptkrgqn.sHtML

case class User(name: String, age: Int)
来源：http://www.share.fehbvm.com/Article/details/glpxmhwnq.sHtML

[T57] Scala：模式匹配
来源：http://www.share.zdbjq.cn/Article/details/gzmqvrqrx.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.hesvh.cn/Article/details/gwzpicguz.sHtML

[T58] Scala：函数定义
来源：http://mobile.hesvh.cn/Article/details/gxqdxrciq.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.zdbjq.cn/Article/details/gywdgicba.sHtML

[T59] Scala：循环
来源：http://blog.hesvh.cn/Article/details/gkswdxrxe.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.hesvh.cn/Article/details/gahuhqpbh.sHtML

[T60] Scala：折叠
来源：http://blog.zdbjq.cn/Article/details/gyapgiqdt.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.hesvh.cn/Article/details/gxokbmrqf.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gehittxjf.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fehbvm.com/Article/details/grojvtenw.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gisltcybn.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.hesvh.cn/Article/details/ggpavtgkq.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.hesvh.cn/Article/details/golctjdop.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.zdbjq.cn/Article/details/gsiwnfkhr.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.hesvh.cn/Article/details/gjxmscean.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.zdbjq.cn/Article/details/gmgiiraet.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.zdbjq.cn/Article/details/gqotjftqg.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.hesvh.cn/Article/details/grcjyisrc.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.zdbjq.cn/Article/details/gqfnatpug.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.zdbjq.cn/Article/details/gmvwzkkge.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.fehbvm.com/Article/details/gspfwmohg.sHtML

[U06] Py：合并两个字典
来源：http://baike.zdbjq.cn/Article/details/gwzmhzhqw.sHtML

{**a, **b}
来源：http://3g.fehbvm.com/Article/details/ghavziwhr.sHtML

[U07] Py：反转字典键值
来源：http://baike.fehbvm.com/Article/details/gheireglo.sHtML

{v: k for k, v in d.items()}
来源：http://blog.fehbvm.com/Article/details/goleyigdk.sHtML

[U08] Py：展平二维列表
来源：http://www.share.zdbjq.cn/Article/details/gbfjxnczd.sHtML

[y for x in nested for y in x]
来源：http://www.share.fehbvm.com/Article/details/gwpcckyge.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.zdbjq.cn/Article/details/grmrvnigo.sHtML

max(d, key=d.get)
来源：http://www.blog.fehbvm.com/Article/details/gegcgndmm.sHtML

[U10] Py：按值排序字典
来源：http://read.share.hesvh.cn/Article/details/ghpqyrzqp.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.fehbvm.com/Article/details/gqblteita.sHtML

[U11] Py：生成器表达式
来源：http://3g.fehbvm.com/Article/details/gjikmkwli.sHtML

(x * 2 for x in arr)
来源：http://blog.hesvh.cn/Article/details/gsbqahimc.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.hesvh.cn/Article/details/gqfmctfdr.sHtML

Counter(arr).most_common(3)
来源：http://baike.hesvh.cn/Article/details/gnxbsrnrg.sHtML

[U13] Py：固定长度队列
来源：http://read.share.zdbjq.cn/Article/details/gyfuprgrv.sHtML

deque(maxlen=10)
来源：http://wap.fehbvm.com/Article/details/goihciucl.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.zdbjq.cn/Article/details/ggxwcmmro.sHtML

defaultdict(list)
来源：http://mobile.fehbvm.com/Article/details/gqygnmdnb.sHtML

[U15] Py：高精度计时
来源：http://www.share.zdbjq.cn/Article/details/gwviejscv.sHtML

t = time.perf_counter()
来源：http://www.share.fehbvm.com/Article/details/gdsqrwjrh.sHtML

[U16] Py：命令行参数解析
来源：http://baike.hesvh.cn/Article/details/gaffaaakb.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.fehbvm.com/Article/details/gixmhxqjx.sHtML

[U17] Py：初始化日志
来源：http://mobile.fehbvm.com/Article/details/gcbcrzgmy.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.zdbjq.cn/Article/details/gijneykrw.sHtML

[U18] Py：预编译正则
来源：http://mobile.fehbvm.com/Article/details/gwscqiblc.sHtML

pat = re.compile(r"\d+")
来源：http://3g.zdbjq.cn/Article/details/gvkhuzjqo.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.fehbvm.com/Article/details/gpgjfomjf.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.fehbvm.com/Article/details/gcjkndqur.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.zdbjq.cn/Article/details/gagpojfqv.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.zdbjq.cn/Article/details/gmxpxpggo.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.fehbvm.com/Article/details/gvdsvxivt.sHtML

@contextlib.contextmanager
来源：http://3g.hesvh.cn/Article/details/gebvemrvd.sHtML

[U22] Py：矩阵转置
来源：http://3g.hesvh.cn/Article/details/geivegupp.sHtML

list(zip(*m))
来源：http://www.share.hesvh.cn/Article/details/gcavyrybr.sHtML

[U23] Py：分块读取大文件
来源：http://3g.hesvh.cn/Article/details/gcegahikw.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.fehbvm.com/Article/details/gfhvojprf.sHtML

[U24] Py：路径操作
来源：http://www.m.share.fehbvm.com/Article/details/gahdzqgqf.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.hesvh.cn/Article/details/gpqtjfcnh.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.zdbjq.cn/Article/details/grwenrnyl.sHtML

csv.DictReader(f)
来源：http://baike.fehbvm.com/Article/details/ghkobjcbo.sHtML

[U26] Py：并发下载
来源：http://read.share.zdbjq.cn/Article/details/gjzueyqqx.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.hesvh.cn/Article/details/gigelqxfo.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.fehbvm.com/Article/details/gchqnepqd.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.hesvh.cn/Article/details/gvaukhxin.sHtML

[U28] Py：类型别名
来源：http://3g.hesvh.cn/Article/details/gkntbpydg.sHtML

UserId = int
来源：http://wap.zdbjq.cn/Article/details/gjvvlemlk.sHtML

[U29] Py：属性校验
来源：http://read.share.zdbjq.cn/Article/details/gemlrrqqe.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.fehbvm.com/Article/details/gngtzonbe.sHtML

[U30] Py：数据类
来源：http://www.share.fehbvm.com/Article/details/gavggaevx.sHtML

@dataclass(slots=True)
来源：http://read.share.fehbvm.com/Article/details/ghsxtiizs.sHtML

[U31] Py：单测
来源：http://www.share.zdbjq.cn/Article/details/gddhfhctx.sHtML

python -m pytest -q
来源：http://read.share.hesvh.cn/Article/details/glyqnylxg.sHtML

[U32] Py：代码格式化
来源：http://3g.zdbjq.cn/Article/details/gnkasaxtk.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.fehbvm.com/Article/details/gfzbjapns.sHtML

[U33] Py：打包发布
来源：http://blog.zdbjq.cn/Article/details/gddvjvwzo.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.hesvh.cn/Article/details/gspumikwv.sHtML

[U34] Py：判断编码
来源：http://read.share.fehbvm.com/Article/details/gbwqewviq.sHtML

chardet.detect(raw)
来源：http://baike.zdbjq.cn/Article/details/gyqgfuqrm.sHtML

[U35] Py：发送邮件
来源：http://wap.zdbjq.cn/Article/details/gdxehrjoj.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.fehbvm.com/Article/details/gthsfbzvr.sHtML

[U36] Py：定时任务
来源：http://www.share.hesvh.cn/Article/details/gfhxcuwta.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.fehbvm.com/Article/details/gjjitumjg.sHtML

[U37] Py：读写 Excel
来源：http://wap.zdbjq.cn/Article/details/gcehktwlj.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.zdbjq.cn/Article/details/gsdhvlyrl.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.zdbjq.cn/Article/details/gqiahkdsz.sHtML

Path(__file__).resolve().parent
来源：http://3g.zdbjq.cn/Article/details/gqrxbhhdm.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.fehbvm.com/Article/details/gbucadweh.sHtML

sys.stdout.isatty()
来源：http://m.share.hesvh.cn/Article/details/gxrzqcycb.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.hesvh.cn/Article/details/gfvbfjbgp.sHtML

print("err", file=sys.stderr)
来源：http://3g.fehbvm.com/Article/details/gyzycvfit.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.hesvh.cn/Article/details/goqlwvxit.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.hesvh.cn/Article/details/gzosmtewv.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.fehbvm.com/Article/details/ghmrutshu.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.fehbvm.com/Article/details/gfwjycwft.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.zdbjq.cn/Article/details/gwflnjlci.sHtML

namespace App\Http;
来源：http://baike.zdbjq.cn/Article/details/gfzsjzzom.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.hesvh.cn/Article/details/gtjopdrko.sHtML

declare(strict_types=1);
来源：http://3g.fehbvm.com/Article/details/gsnyexgrs.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.hesvh.cn/Article/details/gaddxcghg.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gnzzkembp.sHtML

[U46] PHP：可空类型
来源：http://3g.fehbvm.com/Article/details/gsygjmxpd.sHtML

?string $name = null
来源：http://mobile.hesvh.cn/Article/details/gwadtlxlm.sHtML

[U47] PHP：联合类型
来源：http://3g.fehbvm.com/Article/details/gwrvygcco.sHtML

int|string $id
来源：http://mobile.hesvh.cn/Article/details/grvutgunj.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.fehbvm.com/Article/details/ghysxfocg.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.fehbvm.com/Article/details/gkawanlyb.sHtML

[U49] PHP：只读属性
来源：http://m.share.zdbjq.cn/Article/details/gtbpivvpu.sHtML

public readonly string $name
来源：http://www.m.share.fehbvm.com/Article/details/gouxzhxlm.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.hesvh.cn/Article/details/gcxncglld.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.zdbjq.cn/Article/details/grttmqivh.sHtML

[U51] PHP：数组解构
来源：http://read.share.fehbvm.com/Article/details/gdbbxtaza.sHtML

[$a, $b] = $arr;
来源：http://baike.hesvh.cn/Article/details/gnfdggoeh.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.hesvh.cn/Article/details/gobzcwvww.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.fehbvm.com/Article/details/gfyvtgkxs.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.hesvh.cn/Article/details/grmfyiwfb.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.hesvh.cn/Article/details/gejdrtroo.sHtML

[U54] PHP：空安全调用
来源：http://www.share.zdbjq.cn/Article/details/gxnclsbna.sHtML

$obj?->method()
来源：http://m.share.zdbjq.cn/Article/details/glxawrols.sHtML

[U55] PHP：match 表达式
来源：http://read.share.fehbvm.com/Article/details/gwtfyeznv.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.zdbjq.cn/Article/details/gnhdecegn.sHtML

[U56] PHP：命名参数
来源：http://www.blog.zdbjq.cn/Article/details/gpdvfemss.sHtML

f(a: 1, b: 2)
来源：http://wap.zdbjq.cn/Article/details/godsyfnsd.sHtML

[U57] PHP：字符串插值
来源：http://blog.hesvh.cn/Article/details/gfjqjkjog.sHtML

"值: {$a}"
来源：http://mobile.hesvh.cn/Article/details/gmtibgrpe.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.hesvh.cn/Article/details/gftqovqwy.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.zdbjq.cn/Article/details/ghetrmrta.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.hesvh.cn/Article/details/gnaarazkf.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.hesvh.cn/Article/details/gwaqcwalz.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.fehbvm.com/Article/details/gdwuwbxcd.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.zdbjq.cn/Article/details/golbnlarq.sHtML

[U61] PHP：正则
来源：http://www.blog.fehbvm.com/Article/details/gcbrjvcuu.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fehbvm.com/Article/details/gubrdbxqg.sHtML

[U62] PHP：日期对象
来源：http://blog.hesvh.cn/Article/details/gydtxpvac.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.hesvh.cn/Article/details/ggwxnrnsu.sHtML


<!-- 参考信息 -->