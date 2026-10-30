代发 wailian999

[S39] C++：自定义比较器排序
来源：http://3g.zdbjq.cn/Article/details/gljrjfvjl.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.zdbjq.cn/Article/details/grcnclvrv.sHtML

[S40] C++：查找元素
来源：http://baike.zdbjq.cn/Article/details/guqzqznlf.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fehbvm.com/Article/details/gpbxtoqit.sHtML

[S41] C++：类与构造函数
来源：http://baike.zdbjq.cn/Article/details/gaenmcrho.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fehbvm.com/Article/details/gegkowsvz.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.zdbjq.cn/Article/details/gixkfhckk.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.hesvh.cn/Article/details/gnbrpahmv.sHtML

[S43] C++：智能指针
来源：http://blog.fehbvm.com/Article/details/ggwnaytyf.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.hesvh.cn/Article/details/guniycaxp.sHtML

[S44] C++：引用传参
来源：http://www.blog.zdbjq.cn/Article/details/gcobnzsqt.sHtML

void inc(int &x) { ++x; }
来源：http://baike.hesvh.cn/Article/details/gxvknfedg.sHtML

[S45] C++：lambda
来源：http://www.share.fehbvm.com/Article/details/gxgiugcrv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.zdbjq.cn/Article/details/gzuuelwmq.sHtML

[S46] C++：函数模板
来源：http://wap.hesvh.cn/Article/details/gerxtltye.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fehbvm.com/Article/details/gyqazomxi.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.hesvh.cn/Article/details/gqmimoloi.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.zdbjq.cn/Article/details/ghpzjisoj.sHtML

[S48] C++：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gcxxjroqa.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.hesvh.cn/Article/details/gsnjqaubo.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gfhemmujt.sHtML

[S49] C++：写文件
来源：http://www.m.share.hesvh.cn/Article/details/gpbdczqoo.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.hesvh.cn/Article/details/gxbpaxyra.sHtML

[S50] C++：格式化数字
来源：http://mobile.fehbvm.com/Article/details/gunlnfxjy.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.zdbjq.cn/Article/details/glnipafrv.sHtML

[S51] C++：显式类型转换
来源：http://m.share.zdbjq.cn/Article/details/gmcrgatav.sHtML

static_cast<double>(a) / b
来源：http://www.blog.zdbjq.cn/Article/details/gjhggiaal.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.hesvh.cn/Article/details/gplgmrjvy.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.hesvh.cn/Article/details/gmovucdlt.sHtML

[S53] C++：移动语义
来源：http://read.share.zdbjq.cn/Article/details/guyyhpmcx.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.hesvh.cn/Article/details/gqsbkytvv.sHtML

[S54] C++：异常处理
来源：http://mobile.fehbvm.com/Article/details/gfojoeour.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fehbvm.com/Article/details/glaaopcll.sHtML

[S55] C++：结构化绑定
来源：http://baike.fehbvm.com/Article/details/giwqqfjim.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fehbvm.com/Article/details/gtmlvxrrb.sHtML

[S56] C++：optional
来源：http://m.share.fehbvm.com/Article/details/gvtvsjylt.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fehbvm.com/Article/details/gppmsvrmj.sHtML

[S57] C++：编译期常量
来源：http://wap.hesvh.cn/Article/details/gsohypzql.sHtML

constexpr int N = 10;
来源：http://read.share.fehbvm.com/Article/details/glaxzlpgk.sHtML

[S58] C++：命名空间
来源：http://m.share.zdbjq.cn/Article/details/gjkjftmbz.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fehbvm.com/Article/details/gejkwnaah.sHtML

[S59] C++：静态断言
来源：http://read.share.hesvh.cn/Article/details/gthxwtqni.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fehbvm.com/Article/details/gcuxupxhb.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fehbvm.com/Article/details/gmnwkaecn.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/gpvzjqilr.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gzodloegm.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.zdbjq.cn/Article/details/gotjeguzd.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/govpnccwj.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gndvryzol.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/gjprnhiri.sHtML

[T02] Kotlin：变量
来源：http://m.share.fehbvm.com/Article/details/glgczgybr.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fehbvm.com/Article/details/gijktwumu.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.zdbjq.cn/Article/details/gmnqjohhx.sHtML

"值: $b"
来源：http://m.share.fehbvm.com/Article/details/gwawrumom.sHtML

[T04] Kotlin：空安全
来源：http://blog.zdbjq.cn/Article/details/gcwnnuogj.sHtML

val n: String? = null;  n?.length
来源：http://baike.zdbjq.cn/Article/details/gysrakhmm.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fehbvm.com/Article/details/gjoqtlzmj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.zdbjq.cn/Article/details/ggioakzjn.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.hesvh.cn/Article/details/gecsgpcca.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.hesvh.cn/Article/details/gkltepydb.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.zdbjq.cn/Article/details/gdyqmkriw.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.zdbjq.cn/Article/details/ggroliaxr.sHtML

[T08] Kotlin：数据类
来源：http://baike.fehbvm.com/Article/details/ggsgukxiv.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.hesvh.cn/Article/details/gghravmyz.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.hesvh.cn/Article/details/gbaeitbjb.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.hesvh.cn/Article/details/gbvxrsgcr.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.zdbjq.cn/Article/details/gvvqzvdht.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.zdbjq.cn/Article/details/gkrojwhez.sHtML

[T11] Kotlin：协程
来源：http://www.share.fehbvm.com/Article/details/gdhzlheck.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fehbvm.com/Article/details/grpbbjzza.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fehbvm.com/Article/details/gncbmgzjy.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fehbvm.com/Article/details/gkfkyxnhm.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fehbvm.com/Article/details/gqfdfdikc.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.hesvh.cn/Article/details/gtzsdmncn.sHtML

[T14] Kotlin：循环
来源：http://www.share.hesvh.cn/Article/details/getoaenps.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fehbvm.com/Article/details/gmjfcfaqn.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.zdbjq.cn/Article/details/gpajqfgtn.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fehbvm.com/Article/details/gqotjsaui.sHtML

[T16] Swift：Hello World
来源：http://3g.fehbvm.com/Article/details/ghxbqnoiv.sHtML

print("Hello")
来源：http://wap.fehbvm.com/Article/details/gxrbomljr.sHtML

[T17] Swift：变量与常量
来源：http://baike.hesvh.cn/Article/details/ghbvtbrcj.sHtML

var a = 1;  let b = 2
来源：http://www.share.hesvh.cn/Article/details/gjcjvciqr.sHtML

[T18] Swift：字符串插值
来源：http://read.share.fehbvm.com/Article/details/geassmvkw.sHtML

"值: \(b)"
来源：http://m.share.hesvh.cn/Article/details/gvvdterik.sHtML

[T19] Swift：可选绑定
来源：http://3g.zdbjq.cn/Article/details/gcmvmttfo.sHtML

if let n = opt { print(n) }
来源：http://blog.zdbjq.cn/Article/details/gqukbapgk.sHtML

[T20] Swift：数组操作
来源：http://3g.zdbjq.cn/Article/details/gakgviihq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.zdbjq.cn/Article/details/gtanxpvht.sHtML

[T21] Swift：遍历
来源：http://mobile.hesvh.cn/Article/details/gjgwlamqv.sHtML

for x in a { print(x) }
来源：http://www.m.share.zdbjq.cn/Article/details/gljzavdpt.sHtML

[T22] Swift：字典
来源：http://read.share.hesvh.cn/Article/details/gbkpyjofy.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.zdbjq.cn/Article/details/gbksjkpdf.sHtML

[T23] Swift：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gmzixjiex.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.hesvh.cn/Article/details/gpaktireb.sHtML

[T24] Swift：闭包
来源：http://3g.zdbjq.cn/Article/details/gecqzbfew.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/guysogaxt.sHtML

[T25] Swift：结构体
来源：http://www.blog.zdbjq.cn/Article/details/gktsugszx.sHtML

struct P { var x: Int }
来源：http://mobile.fehbvm.com/Article/details/gokylkydo.sHtML

[T26] Swift：类与重写
来源：http://blog.zdbjq.cn/Article/details/gqmlgkgrw.sHtML

class A: Base { override func f() {} }
来源：http://www.share.zdbjq.cn/Article/details/gyddnyoha.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fehbvm.com/Article/details/ggcahlqrv.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.zdbjq.cn/Article/details/glpiykflc.sHtML

[T28] Swift：枚举
来源：http://m.share.zdbjq.cn/Article/details/gcwktvdvh.sHtML

enum Color { case red, green }
来源：http://baike.zdbjq.cn/Article/details/gphkkhcao.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.zdbjq.cn/Article/details/gszijirkj.sHtML

guard let x = opt else { return }
来源：http://3g.zdbjq.cn/Article/details/gezdyubch.sHtML

[T30] Swift：协议
来源：http://www.m.share.hesvh.cn/Article/details/gtelyywka.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.zdbjq.cn/Article/details/gjogkzivp.sHtML

[T31] Lua：Hello World
来源：http://read.share.hesvh.cn/Article/details/guaudlrnm.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/gmasisyjh.sHtML

[T32] Lua：局部变量
来源：http://baike.fehbvm.com/Article/details/gzwvlwoiu.sHtML

local a = 1
来源：http://www.blog.hesvh.cn/Article/details/gpwfjldiv.sHtML

[T33] Lua：表（数组）
来源：http://blog.fehbvm.com/Article/details/gmubzqhme.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.fehbvm.com/Article/details/ghmevnrwx.sHtML

[T34] Lua：遍历表
来源：http://baike.zdbjq.cn/Article/details/gsxhwdrvr.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.hesvh.cn/Article/details/gzdaaropc.sHtML

[T35] Lua：字典表
来源：http://read.share.zdbjq.cn/Article/details/gfertkzyv.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.hesvh.cn/Article/details/gcgmufqrf.sHtML

[T36] Lua：函数
来源：http://m.share.fehbvm.com/Article/details/gojefxqab.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.zdbjq.cn/Article/details/gfvrgpguc.sHtML

[T37] Lua：字符串拼接
来源：http://wap.zdbjq.cn/Article/details/gveedvsky.sHtML

"a" .. "b"
来源：http://wap.hesvh.cn/Article/details/glnmtzjfw.sHtML

[T38] Lua：条件
来源：http://www.m.share.hesvh.cn/Article/details/gihstrici.sHtML

if x > 0 then print("正") end
来源：http://www.share.hesvh.cn/Article/details/gcftflxwz.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.fehbvm.com/Article/details/giybkplxi.sHtML

string.find(s, "%d+")
来源：http://m.share.hesvh.cn/Article/details/gctcjldnm.sHtML

[T40] Lua：元表
来源：http://baike.hesvh.cn/Article/details/gwfyfhnsw.sHtML

setmetatable({}, { __index = base })
来源：http://baike.fehbvm.com/Article/details/gwpjxoqqx.sHtML

[T41] Perl：Hello World
来源：http://read.share.fehbvm.com/Article/details/gyzrlcwwj.sHtML

print "Hello\n";
来源：http://3g.hesvh.cn/Article/details/gaaofcoms.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.fehbvm.com/Article/details/gowjlkhlf.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.zdbjq.cn/Article/details/gsfknnqoo.sHtML

[T43] Perl：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gvtxiwcxt.sHtML

"值: $a"
来源：http://3g.zdbjq.cn/Article/details/gmgypbrgz.sHtML

[T44] Perl：条件
来源：http://m.share.hesvh.cn/Article/details/guukkmzfw.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.zdbjq.cn/Article/details/gweddfjgn.sHtML

[T45] Perl：数组遍历
来源：http://blog.hesvh.cn/Article/details/gfbjrsoev.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.fehbvm.com/Article/details/geifjkszd.sHtML

[T46] Perl：哈希操作
来源：http://mobile.zdbjq.cn/Article/details/gsqliepij.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.zdbjq.cn/Article/details/glkotoaaf.sHtML

[T47] Perl：正则捕获
来源：http://read.share.hesvh.cn/Article/details/gljroendu.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.fehbvm.com/Article/details/gbluhrcep.sHtML

[T48] Perl：正则替换
来源：http://www.share.hesvh.cn/Article/details/gohxjrbzv.sHtML

$s =~ s/old/new/g;
来源：http://www.share.zdbjq.cn/Article/details/giywcxmpu.sHtML

[T49] Perl：函数
来源：http://wap.hesvh.cn/Article/details/gyezzghui.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gorceumxl.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gmtoewkka.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.hesvh.cn/Article/details/gwdwyyxfl.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.hesvh.cn/Article/details/gjuphtmps.sHtML

[T51] Scala：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gtpbeycoc.sHtML

println("Hello")
来源：http://www.share.zdbjq.cn/Article/details/giseotcam.sHtML

[T52] Scala：变量
来源：http://www.share.hesvh.cn/Article/details/gjypvknwr.sHtML

val a = 1;  var b = 2
来源：http://baike.hesvh.cn/Article/details/ggnldeqyp.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gjsippoif.sHtML

s"值: $b"
来源：http://www.blog.fehbvm.com/Article/details/goaztfpcn.sHtML

[T54] Scala：集合映射
来源：http://read.share.fehbvm.com/Article/details/gmebeyzdy.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.hesvh.cn/Article/details/gasceadua.sHtML

[T55] Scala：集合过滤
来源：http://baike.zdbjq.cn/Article/details/gtdisogkw.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.fehbvm.com/Article/details/ghmrmmbrl.sHtML

[T56] Scala：样例类
来源：http://www.m.share.zdbjq.cn/Article/details/gghaobdcj.sHtML

case class User(name: String, age: Int)
来源：http://blog.hesvh.cn/Article/details/gdnobucxh.sHtML

[T57] Scala：模式匹配
来源：http://www.share.hesvh.cn/Article/details/gstdmusya.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.hesvh.cn/Article/details/gcpqivcrf.sHtML

[T58] Scala：函数定义
来源：http://blog.hesvh.cn/Article/details/gatooeizv.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.zdbjq.cn/Article/details/geusoxmwt.sHtML

[T59] Scala：循环
来源：http://www.share.hesvh.cn/Article/details/gscawkqqu.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.zdbjq.cn/Article/details/gvnziuwws.sHtML

[T60] Scala：折叠
来源：http://m.share.fehbvm.com/Article/details/gpgaeezkj.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.fehbvm.com/Article/details/gbchlsobh.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/giczmeadg.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fehbvm.com/Article/details/gtshwwzuh.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gibgrglvo.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.zdbjq.cn/Article/details/gdlejxydk.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.fehbvm.com/Article/details/gqkghwgzz.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.zdbjq.cn/Article/details/gtrtronpa.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.hesvh.cn/Article/details/gztiouaev.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.zdbjq.cn/Article/details/gjritwsnq.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.fehbvm.com/Article/details/gcbxclejr.sHtML

[U04] Py：变量调试打印
来源：http://baike.zdbjq.cn/Article/details/guknuftme.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.zdbjq.cn/Article/details/gieloqjfl.sHtML

[U05] Py：列表去重且保序
来源：http://3g.hesvh.cn/Article/details/gcbynvxro.sHtML

list(dict.fromkeys(arr))
来源：http://3g.fehbvm.com/Article/details/gillxhzom.sHtML

[U06] Py：合并两个字典
来源：http://mobile.hesvh.cn/Article/details/glvycpejc.sHtML

{**a, **b}
来源：http://3g.zdbjq.cn/Article/details/gupvxfive.sHtML

[U07] Py：反转字典键值
来源：http://www.share.zdbjq.cn/Article/details/gdmnzyaci.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.fehbvm.com/Article/details/gnbqstrov.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.fehbvm.com/Article/details/gquynghkq.sHtML

[y for x in nested for y in x]
来源：http://mobile.fehbvm.com/Article/details/gzrftrjil.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.fehbvm.com/Article/details/gnajhfuwx.sHtML

max(d, key=d.get)
来源：http://read.share.zdbjq.cn/Article/details/gkqxbyfkh.sHtML

[U10] Py：按值排序字典
来源：http://baike.fehbvm.com/Article/details/gxffblakq.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.zdbjq.cn/Article/details/gcxphqhoa.sHtML

[U11] Py：生成器表达式
来源：http://3g.hesvh.cn/Article/details/gikrjtdex.sHtML

(x * 2 for x in arr)
来源：http://wap.zdbjq.cn/Article/details/gzsovfgmj.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.zdbjq.cn/Article/details/glsodbrhx.sHtML

Counter(arr).most_common(3)
来源：http://blog.hesvh.cn/Article/details/gysyicglk.sHtML

[U13] Py：固定长度队列
来源：http://3g.zdbjq.cn/Article/details/gtiertkgt.sHtML

deque(maxlen=10)
来源：http://read.share.fehbvm.com/Article/details/govutlnnp.sHtML

[U14] Py：分组收集到列表
来源：http://blog.fehbvm.com/Article/details/gywbzwggh.sHtML

defaultdict(list)
来源：http://baike.zdbjq.cn/Article/details/grfmxaiii.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.fehbvm.com/Article/details/ghmnojnlm.sHtML

t = time.perf_counter()
来源：http://mobile.fehbvm.com/Article/details/giyqfcduq.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.zdbjq.cn/Article/details/gjnforpry.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.hesvh.cn/Article/details/gvqtonagx.sHtML

[U17] Py：初始化日志
来源：http://mobile.hesvh.cn/Article/details/gqrzahmex.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.fehbvm.com/Article/details/gacvmklpj.sHtML

[U18] Py：预编译正则
来源：http://3g.fehbvm.com/Article/details/gxxklygqs.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.zdbjq.cn/Article/details/ggiatbrfs.sHtML

[U19] Py：正则替换带回调
来源：http://blog.hesvh.cn/Article/details/gdxrkppcn.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.zdbjq.cn/Article/details/gwubiblze.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.fehbvm.com/Article/details/goffiktyz.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.fehbvm.com/Article/details/gvybnnryx.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.fehbvm.com/Article/details/glvihwiuj.sHtML

@contextlib.contextmanager
来源：http://www.blog.zdbjq.cn/Article/details/gevebxlxg.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.zdbjq.cn/Article/details/grvtfkhcm.sHtML

list(zip(*m))
来源：http://read.share.fehbvm.com/Article/details/gqeuyzxub.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.fehbvm.com/Article/details/gpgkssjnq.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.zdbjq.cn/Article/details/gnmucuhnn.sHtML

[U24] Py：路径操作
来源：http://wap.fehbvm.com/Article/details/gtcotmrbd.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.hesvh.cn/Article/details/gwtysqiad.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.fehbvm.com/Article/details/gasqlcgjo.sHtML

csv.DictReader(f)
来源：http://www.blog.hesvh.cn/Article/details/gqpebrhwb.sHtML

[U26] Py：并发下载
来源：http://read.share.fehbvm.com/Article/details/gzfarisup.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.hesvh.cn/Article/details/ghhokahfa.sHtML

[U27] Py：异步 HTTP
来源：http://wap.hesvh.cn/Article/details/gyztuozhv.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.fehbvm.com/Article/details/guhcaxvdg.sHtML

[U28] Py：类型别名
来源：http://blog.fehbvm.com/Article/details/gwvkydjza.sHtML

UserId = int
来源：http://mobile.hesvh.cn/Article/details/gmoqvpcid.sHtML

[U29] Py：属性校验
来源：http://www.m.share.fehbvm.com/Article/details/gyjarspma.sHtML

@property 与 @x.setter 配合
来源：http://3g.hesvh.cn/Article/details/gqjzmnxig.sHtML

[U30] Py：数据类
来源：http://blog.zdbjq.cn/Article/details/gffekbooc.sHtML

@dataclass(slots=True)
来源：http://www.share.hesvh.cn/Article/details/gsnmooblx.sHtML

[U31] Py：单测
来源：http://www.blog.fehbvm.com/Article/details/ggmroyrkw.sHtML

python -m pytest -q
来源：http://wap.fehbvm.com/Article/details/gjixrgkaa.sHtML

[U32] Py：代码格式化
来源：http://read.share.hesvh.cn/Article/details/ghgluxdkv.sHtML

ruff format . && ruff check --fix .
来源：http://3g.fehbvm.com/Article/details/gqzzmodct.sHtML

[U33] Py：打包发布
来源：http://blog.fehbvm.com/Article/details/grcivyfkk.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.fehbvm.com/Article/details/gpokqsoft.sHtML

[U34] Py：判断编码
来源：http://blog.fehbvm.com/Article/details/gdgedtpci.sHtML

chardet.detect(raw)
来源：http://m.share.fehbvm.com/Article/details/gmtuqohfl.sHtML

[U35] Py：发送邮件
来源：http://baike.fehbvm.com/Article/details/gadgnmtuq.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.zdbjq.cn/Article/details/gurnxlwzj.sHtML

[U36] Py：定时任务
来源：http://m.share.hesvh.cn/Article/details/gwaawhzuk.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.zdbjq.cn/Article/details/geawwzbfe.sHtML

[U37] Py：读写 Excel
来源：http://blog.fehbvm.com/Article/details/gidkkxwyb.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.hesvh.cn/Article/details/gftegxgvc.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.zdbjq.cn/Article/details/grmgwbmnq.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.hesvh.cn/Article/details/grisqbdbc.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.hesvh.cn/Article/details/grurnkscm.sHtML

sys.stdout.isatty()
来源：http://read.share.fehbvm.com/Article/details/ggmvqsvph.sHtML

[U40] Py：打印到标准错误
来源：http://wap.hesvh.cn/Article/details/gihmgmmmf.sHtML

print("err", file=sys.stderr)
来源：http://mobile.zdbjq.cn/Article/details/gncdkngho.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.zdbjq.cn/Article/details/grgfpszai.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.fehbvm.com/Article/details/gyvuijcpf.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.hesvh.cn/Article/details/gyhwdoyzl.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.hesvh.cn/Article/details/glyfihgnw.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.fehbvm.com/Article/details/guydfnqtn.sHtML

namespace App\Http;
来源：http://www.share.hesvh.cn/Article/details/gdypebpgd.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.zdbjq.cn/Article/details/ggtogdmjj.sHtML

declare(strict_types=1);
来源：http://read.share.hesvh.cn/Article/details/gsqhnkkao.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.fehbvm.com/Article/details/gvviusnxq.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/ghcihxkvi.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.hesvh.cn/Article/details/glohtskkd.sHtML

?string $name = null
来源：http://mobile.hesvh.cn/Article/details/gsdwlqses.sHtML

[U47] PHP：联合类型
来源：http://mobile.zdbjq.cn/Article/details/gyygmyfng.sHtML

int|string $id
来源：http://www.m.share.zdbjq.cn/Article/details/gltnzibkl.sHtML

[U48] PHP：纯枚举
来源：http://www.share.hesvh.cn/Article/details/gaobdtljk.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.fehbvm.com/Article/details/grmwlpfci.sHtML

[U49] PHP：只读属性
来源：http://www.share.zdbjq.cn/Article/details/gyzufuycm.sHtML

public readonly string $name
来源：http://www.blog.hesvh.cn/Article/details/gmjiicrji.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.hesvh.cn/Article/details/gohupkese.sHtML

public function __construct(private int $id) {}
来源：http://mobile.fehbvm.com/Article/details/gytbniswo.sHtML

[U51] PHP：数组解构
来源：http://www.share.hesvh.cn/Article/details/ghagjmpeg.sHtML

[$a, $b] = $arr;
来源：http://m.share.fehbvm.com/Article/details/gwsjvcnbr.sHtML

[U52] PHP：箭头函数
来源：http://m.share.zdbjq.cn/Article/details/godujfqaf.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.fehbvm.com/Article/details/guskyxlnh.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.zdbjq.cn/Article/details/gztiaqyck.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.hesvh.cn/Article/details/ghsvkxmvg.sHtML

[U54] PHP：空安全调用
来源：http://mobile.hesvh.cn/Article/details/gzzbyoucv.sHtML

$obj?->method()
来源：http://read.share.zdbjq.cn/Article/details/gqamornlk.sHtML

[U55] PHP：match 表达式
来源：http://read.share.zdbjq.cn/Article/details/gxjguyuxl.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.zdbjq.cn/Article/details/gtgwvvhkc.sHtML

[U56] PHP：命名参数
来源：http://mobile.hesvh.cn/Article/details/gdooekdri.sHtML

f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/gtcyafbkj.sHtML

[U57] PHP：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gkayvubyy.sHtML

"值: {$a}"
来源：http://www.blog.zdbjq.cn/Article/details/gkqpylthm.sHtML

[U58] PHP：数组三件套
来源：http://www.share.zdbjq.cn/Article/details/glapznhye.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.zdbjq.cn/Article/details/gsljwycpu.sHtML

[U59] PHP：自定义排序
来源：http://mobile.fehbvm.com/Article/details/gjahuysyz.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.zdbjq.cn/Article/details/gbckskrgs.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.fehbvm.com/Article/details/gmunckpta.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.zdbjq.cn/Article/details/gpqhphlom.sHtML

[U61] PHP：正则
来源：http://www.blog.hesvh.cn/Article/details/gsmmngmdb.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.fehbvm.com/Article/details/gxdyftayk.sHtML

[U62] PHP：日期对象
来源：http://mobile.zdbjq.cn/Article/details/gdlqqcmqr.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.fehbvm.com/Article/details/gmadadyns.sHtML

[U63] PHP：文件读写
来源：http://blog.zdbjq.cn/Article/details/grdjmrgqt.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.zdbjq.cn/Article/details/gsgrqegiw.sHtML

[U64] PHP：目录遍历
来源：http://www.share.zdbjq.cn/Article/details/gjsszcbye.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.hesvh.cn/Article/details/grtczypjr.sHtML


<!-- 参考信息 -->