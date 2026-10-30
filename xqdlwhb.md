代发 wailian999

[S41] C++：类与构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmdspvxhb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gevndhcmd.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fanxiaobao.xyz/Article/details/gdpthlptn.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fanxiaobao.xyz/Article/details/ghrlkjdtw.sHtML

[S43] C++：智能指针
来源：http://baike.fanxiaobao.xyz/Article/details/gcqiotxog.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fanxiaobao.xyz/Article/details/gabmtehuo.sHtML

[S44] C++：引用传参
来源：http://m.share.fanxiaobao.xyz/Article/details/gemztwrbx.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gilowhnqn.sHtML

[S45] C++：lambda
来源：http://3g.fanxiaobao.xyz/Article/details/grcsuoaql.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fanxiaobao.xyz/Article/details/gnflqndbu.sHtML

[S46] C++：函数模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqqjcfupg.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvzefhdbw.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/guumhktsc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fanxiaobao.xyz/Article/details/ggpovjket.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gnzigiyho.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzqqmlmpg.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpsqdgoxf.sHtML

[S49] C++：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gaubvamdc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fanxiaobao.xyz/Article/details/gsbfhbmcu.sHtML

[S50] C++：格式化数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gdbmzlttl.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glzufxuhz.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/girzkjkrn.sHtML

static_cast<double>(a) / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gducmdooc.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fanxiaobao.xyz/Article/details/gxzujynkf.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fanxiaobao.xyz/Article/details/gqafdvkyq.sHtML

[S53] C++：移动语义
来源：http://m.share.fanxiaobao.xyz/Article/details/gacryzgwf.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fanxiaobao.xyz/Article/details/guoypddgz.sHtML

[S54] C++：异常处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvjtifzn.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/guthvbltb.sHtML

[S55] C++：结构化绑定
来源：http://3g.fanxiaobao.xyz/Article/details/gxyhsmxmv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fanxiaobao.xyz/Article/details/gmyohhsql.sHtML

[S56] C++：optional
来源：http://m.share.fanxiaobao.xyz/Article/details/gqqaxitnp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwretvbje.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gashfmdaz.sHtML

constexpr int N = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/govblmwmu.sHtML

[S58] C++：命名空间
来源：http://www.share.fanxiaobao.xyz/Article/details/ghwwffdhw.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fanxiaobao.xyz/Article/details/gvekhctcw.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gntwcotxh.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fanxiaobao.xyz/Article/details/genxmtdox.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gtdvodofm.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gwqjgnhen.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gwqkkjqkj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fanxiaobao.xyz/Article/details/gknnqggmg.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghnefexpt.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcrfrrrzx.sHtML

println("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/ggtbviaaj.sHtML

[T02] Kotlin：变量
来源：http://3g.fanxiaobao.xyz/Article/details/gozmpwpap.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fanxiaobao.xyz/Article/details/goacztvuk.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gahcgrray.sHtML

"值: $b"
来源：http://3g.fanxiaobao.xyz/Article/details/gbwfbquuz.sHtML

[T04] Kotlin：空安全
来源：http://3g.fanxiaobao.xyz/Article/details/gulhlzglz.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fanxiaobao.xyz/Article/details/gblhryuvj.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gkgkzqzgt.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fanxiaobao.xyz/Article/details/gvxdrtczy.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnwanndix.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdfdobnzc.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gxunaqvpo.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fanxiaobao.xyz/Article/details/gpsdhxqcb.sHtML

[T08] Kotlin：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/gtkrgwcpg.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyrjcneen.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyefmhdkn.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjibdatxe.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gfmcagrzn.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gskmfyglw.sHtML

[T11] Kotlin：协程
来源：http://www.share.fanxiaobao.xyz/Article/details/gqkmnufch.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkqqrutml.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gphnukayq.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/givfajpwj.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/ghrausoze.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjkkpohtx.sHtML

[T14] Kotlin：循环
来源：http://baike.fanxiaobao.xyz/Article/details/gqngpxipn.sHtML

for (i in 1..10) println(i)
来源：http://wap.fanxiaobao.xyz/Article/details/gflhzknwj.sHtML

[T15] Kotlin：接口
来源：http://wap.fanxiaobao.xyz/Article/details/gwnttuxbf.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fanxiaobao.xyz/Article/details/gzthpzhrq.sHtML

[T16] Swift：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gillwbwxg.sHtML

print("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxxwsvvno.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gucaipuef.sHtML

var a = 1;  let b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gasafdyas.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gxfpcxaqq.sHtML

"值: \(b)"
来源：http://wap.fanxiaobao.xyz/Article/details/garfgeric.sHtML

[T19] Swift：可选绑定
来源：http://baike.fanxiaobao.xyz/Article/details/gazibzics.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grnsvhlyb.sHtML

[T20] Swift：数组操作
来源：http://wap.fanxiaobao.xyz/Article/details/gadyvgnfk.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvfpzntzf.sHtML

[T21] Swift：遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/goooholkz.sHtML

for x in a { print(x) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gelnpvvaz.sHtML

[T22] Swift：字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gvekrwnfd.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gjwdrdrwp.sHtML

[T23] Swift：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gcypcrsqb.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.fanxiaobao.xyz/Article/details/gocpvvkcy.sHtML

[T24] Swift：闭包
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjaieqos.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/gzzfrofca.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gemubvcgu.sHtML

struct P { var x: Int }
来源：http://3g.fanxiaobao.xyz/Article/details/gihrsmece.sHtML

[T26] Swift：类与重写
来源：http://baike.fanxiaobao.xyz/Article/details/ggrfwjhee.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fanxiaobao.xyz/Article/details/guuconpur.sHtML

[T27] Swift：错误处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/galmjshjn.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjpeqabti.sHtML

[T28] Swift：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gpntthmgf.sHtML

enum Color { case red, green }
来源：http://3g.fanxiaobao.xyz/Article/details/gjvpyxwrl.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.fanxiaobao.xyz/Article/details/gnactatgn.sHtML

guard let x = opt else { return }
来源：http://baike.fanxiaobao.xyz/Article/details/gdwttxqnl.sHtML

[T30] Swift：协议
来源：http://read.share.fanxiaobao.xyz/Article/details/gijjnacru.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcndngjdp.sHtML

[T31] Lua：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gdbqwlyrw.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/glglqerxi.sHtML

[T32] Lua：局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/gqcobihin.sHtML

local a = 1
来源：http://blog.fanxiaobao.xyz/Article/details/gwpdgijuc.sHtML

[T33] Lua：表（数组）
来源：http://wap.fanxiaobao.xyz/Article/details/gryiddomt.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.fanxiaobao.xyz/Article/details/gsjvmmloj.sHtML

[T34] Lua：遍历表
来源：http://www.share.fanxiaobao.xyz/Article/details/gvwvzwpju.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvvuxtmwn.sHtML

[T35] Lua：字典表
来源：http://www.blog.fanxiaobao.xyz/Article/details/geldvmmas.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwynvcrqs.sHtML

[T36] Lua：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gaexdnhzo.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcowgtcfz.sHtML

[T37] Lua：字符串拼接
来源：http://blog.fanxiaobao.xyz/Article/details/gjzpzeofp.sHtML

"a" .. "b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gldshgqhu.sHtML

[T38] Lua：条件
来源：http://3g.fanxiaobao.xyz/Article/details/gmniznljk.sHtML

if x > 0 then print("正") end
来源：http://read.share.fanxiaobao.xyz/Article/details/ggvzfnqyy.sHtML

[T39] Lua：模式匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/ghngiejws.sHtML

string.find(s, "%d+")
来源：http://3g.fanxiaobao.xyz/Article/details/gnddfzupr.sHtML

[T40] Lua：元表
来源：http://3g.fanxiaobao.xyz/Article/details/grgunocip.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fanxiaobao.xyz/Article/details/gtifkvkqb.sHtML

[T41] Perl：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/groiqvfnh.sHtML

print "Hello\n";
来源：http://wap.fanxiaobao.xyz/Article/details/glypfbhlt.sHtML

[T42] Perl：变量类型
来源：http://baike.fanxiaobao.xyz/Article/details/gfpopwccp.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.fanxiaobao.xyz/Article/details/groqozdkg.sHtML

[T43] Perl：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gsxprealy.sHtML

"值: $a"
来源：http://m.share.fanxiaobao.xyz/Article/details/gvjdbgxzw.sHtML

[T44] Perl：条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gbabxundk.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvemkbgsk.sHtML

[T45] Perl：数组遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/ggporbtrd.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/grvbetlzo.sHtML

[T46] Perl：哈希操作
来源：http://baike.fanxiaobao.xyz/Article/details/gwejwueof.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/govkwqtpy.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guijyavus.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdlxnquke.sHtML

[T48] Perl：正则替换
来源：http://3g.fanxiaobao.xyz/Article/details/grehuncwk.sHtML

$s =~ s/old/new/g;
来源：http://3g.fanxiaobao.xyz/Article/details/gsejlowgi.sHtML

[T49] Perl：函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gejalwnvm.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gyinjvlom.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gvdrsiavv.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.fanxiaobao.xyz/Article/details/gwuhhpthv.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkehswpgu.sHtML

[T51] Scala：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gnnsynqcq.sHtML

println("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gbektymdw.sHtML

[T52] Scala：变量
来源：http://3g.fanxiaobao.xyz/Article/details/gjjnljyja.sHtML

val a = 1;  var b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/ggtpujmjm.sHtML

[T53] Scala：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/grybcfacg.sHtML

s"值: $b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gikxrhdkh.sHtML

[T54] Scala：集合映射
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtaxbblcu.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gtupntlsr.sHtML

[T55] Scala：集合过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gukpacyao.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmjzzpvdd.sHtML

[T56] Scala：样例类
来源：http://m.share.fanxiaobao.xyz/Article/details/gkitrwgqo.sHtML

case class User(name: String, age: Int)
来源：http://www.share.fanxiaobao.xyz/Article/details/grhiuanov.sHtML

[T57] Scala：模式匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gascxecuk.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.fanxiaobao.xyz/Article/details/gagsjycvc.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnflcfjee.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqwmuxrfj.sHtML

[T59] Scala：循环
来源：http://wap.fanxiaobao.xyz/Article/details/gnwwxwaue.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.fanxiaobao.xyz/Article/details/gybbzadmh.sHtML

[T60] Scala：折叠
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtvwrhlrx.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmvvwuiiz.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqtxpuyaj.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gzfagcfqw.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/glhwamyxp.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.fanxiaobao.xyz/Article/details/gtvectkhz.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.fanxiaobao.xyz/Article/details/gglrtldom.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.fanxiaobao.xyz/Article/details/gtljlpuwx.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gjqwnznph.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.fanxiaobao.xyz/Article/details/glsspbcil.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.fanxiaobao.xyz/Article/details/glaanmvet.sHtML

[U04] Py：变量调试打印
来源：http://m.share.fanxiaobao.xyz/Article/details/gqbxkzorh.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fanxiaobao.xyz/Article/details/gqyxxsvnn.sHtML

[U05] Py：列表去重且保序
来源：http://baike.fanxiaobao.xyz/Article/details/gehejeamw.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.fanxiaobao.xyz/Article/details/gkihtkbxt.sHtML

[U06] Py：合并两个字典
来源：http://m.share.fanxiaobao.xyz/Article/details/gzkdfgcnt.sHtML

{**a, **b}
来源：http://3g.fanxiaobao.xyz/Article/details/gkciuwmaw.sHtML

[U07] Py：反转字典键值
来源：http://baike.fanxiaobao.xyz/Article/details/getnebotq.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fanxiaobao.xyz/Article/details/gpbzrddtz.sHtML

[U08] Py：展平二维列表
来源：http://www.share.fanxiaobao.xyz/Article/details/gfaojkinm.sHtML

[y for x in nested for y in x]
来源：http://baike.fanxiaobao.xyz/Article/details/goufjsltp.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpgkdbkzw.sHtML

max(d, key=d.get)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwnhdsqci.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdkrobgrk.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.fanxiaobao.xyz/Article/details/gykgcpqvv.sHtML

[U11] Py：生成器表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gnezlboba.sHtML

(x * 2 for x in arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gokillttb.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gfcdcvhwm.sHtML

Counter(arr).most_common(3)
来源：http://wap.fanxiaobao.xyz/Article/details/gcfqermbv.sHtML

[U13] Py：固定长度队列
来源：http://wap.fanxiaobao.xyz/Article/details/gjiducqye.sHtML

deque(maxlen=10)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvyskhquw.sHtML

[U14] Py：分组收集到列表
来源：http://baike.fanxiaobao.xyz/Article/details/gzzjlyike.sHtML

defaultdict(list)
来源：http://blog.fanxiaobao.xyz/Article/details/gzviiirgm.sHtML

[U15] Py：高精度计时
来源：http://baike.fanxiaobao.xyz/Article/details/gadpzsayd.sHtML

t = time.perf_counter()
来源：http://read.share.fanxiaobao.xyz/Article/details/gizfsegqa.sHtML

[U16] Py：命令行参数解析
来源：http://blog.fanxiaobao.xyz/Article/details/gqtuoqekt.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.fanxiaobao.xyz/Article/details/gycmcntxs.sHtML

[U17] Py：初始化日志
来源：http://mobile.fanxiaobao.xyz/Article/details/ghtngbqeb.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.fanxiaobao.xyz/Article/details/guavgltns.sHtML

[U18] Py：预编译正则
来源：http://m.share.fanxiaobao.xyz/Article/details/glsosbeww.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/ggpmtmlao.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.fanxiaobao.xyz/Article/details/gywlcffzt.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.fanxiaobao.xyz/Article/details/gkhfvnidn.sHtML

[U20] Py：缓存函数结果
来源：http://3g.fanxiaobao.xyz/Article/details/ggqwovnyw.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.fanxiaobao.xyz/Article/details/gzbhqikca.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.fanxiaobao.xyz/Article/details/grrbwvrag.sHtML

@contextlib.contextmanager
来源：http://blog.fanxiaobao.xyz/Article/details/gxpnbbsta.sHtML

[U22] Py：矩阵转置
来源：http://mobile.fanxiaobao.xyz/Article/details/gbrvbfknt.sHtML

list(zip(*m))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfkheuzdg.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gugwwcygj.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.fanxiaobao.xyz/Article/details/gvgswiady.sHtML

[U24] Py：路径操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gexvbhbty.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzpztkszh.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvmjxmopl.sHtML

csv.DictReader(f)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwemgshy.sHtML

[U26] Py：并发下载
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxzwdwimn.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gobfmcqyj.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.fanxiaobao.xyz/Article/details/gklkvnwgy.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.fanxiaobao.xyz/Article/details/gsrwozwvt.sHtML

[U28] Py：类型别名
来源：http://read.share.fanxiaobao.xyz/Article/details/gjzgdpnpo.sHtML

UserId = int
来源：http://blog.fanxiaobao.xyz/Article/details/gqmhmtrme.sHtML

[U29] Py：属性校验
来源：http://m.share.fanxiaobao.xyz/Article/details/gkndghahc.sHtML

@property 与 @x.setter 配合
来源：http://m.share.fanxiaobao.xyz/Article/details/gmlplikgq.sHtML

[U30] Py：数据类
来源：http://3g.fanxiaobao.xyz/Article/details/gtjtybcyw.sHtML

@dataclass(slots=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/gaobygtwp.sHtML

[U31] Py：单测
来源：http://mobile.fanxiaobao.xyz/Article/details/gcrhevduw.sHtML

python -m pytest -q
来源：http://wap.fanxiaobao.xyz/Article/details/gwsabxxzk.sHtML

[U32] Py：代码格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gviljfhcs.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.fanxiaobao.xyz/Article/details/gkcsntzbx.sHtML

[U33] Py：打包发布
来源：http://wap.fanxiaobao.xyz/Article/details/gtutywfej.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.fanxiaobao.xyz/Article/details/gpvzjyjrm.sHtML

[U34] Py：判断编码
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghqnraijp.sHtML

chardet.detect(raw)
来源：http://mobile.fanxiaobao.xyz/Article/details/gukapwoxt.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjucgepdl.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmtjxsdrc.sHtML

[U36] Py：定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gfymplvhx.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjemlllj.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.fanxiaobao.xyz/Article/details/gifkvblpf.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjqtqqhhc.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.fanxiaobao.xyz/Article/details/gvfbzmjlb.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.fanxiaobao.xyz/Article/details/golzgzwvt.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.fanxiaobao.xyz/Article/details/gpzmxnqyh.sHtML

sys.stdout.isatty()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtdejaetw.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmjsmkcaw.sHtML

print("err", file=sys.stderr)
来源：http://baike.fanxiaobao.xyz/Article/details/gklxfgxus.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gobrduspq.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.fanxiaobao.xyz/Article/details/gtmnkdsig.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdbkcaijx.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjjwebkhu.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxekejlst.sHtML

namespace App\Http;
来源：http://3g.fanxiaobao.xyz/Article/details/gtqxhgjcs.sHtML

[U44] PHP：开启严格类型
来源：http://wap.fanxiaobao.xyz/Article/details/grsorgvst.sHtML

declare(strict_types=1);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfhqrucyu.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gjwexfbwx.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdbaeynmm.sHtML

[U46] PHP：可空类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gfoddeldd.sHtML

?string $name = null
来源：http://blog.fanxiaobao.xyz/Article/details/grhoupkqj.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdwcdruoc.sHtML

int|string $id
来源：http://wap.fanxiaobao.xyz/Article/details/grspprwqi.sHtML

[U48] PHP：纯枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gkwgirrbz.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxjgqkleb.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gygnownxk.sHtML

public readonly string $name
来源：http://read.share.fanxiaobao.xyz/Article/details/gfzjsezox.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbhsugdzm.sHtML

public function __construct(private int $id) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gmskzkjvo.sHtML

[U51] PHP：数组解构
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzltzukwl.sHtML

[$a, $b] = $arr;
来源：http://blog.fanxiaobao.xyz/Article/details/gsookpnkd.sHtML

[U52] PHP：箭头函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gqjdkmwgb.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gffodqghn.sHtML

[U53] PHP：空合并运算符
来源：http://baike.fanxiaobao.xyz/Article/details/gogadizne.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.fanxiaobao.xyz/Article/details/gebaugtew.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfgqqtezp.sHtML

$obj?->method()
来源：http://www.share.fanxiaobao.xyz/Article/details/givikgexa.sHtML

[U55] PHP：match 表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gpfyligye.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.fanxiaobao.xyz/Article/details/gmxomgtzh.sHtML

[U56] PHP：命名参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gxvhprlqd.sHtML

f(a: 1, b: 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqarbyqzh.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmdkrcdhk.sHtML

"值: {$a}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdziltwkr.sHtML

[U58] PHP：数组三件套
来源：http://3g.fanxiaobao.xyz/Article/details/gnbwjxwyg.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwsrqvugx.sHtML

[U59] PHP：自定义排序
来源：http://baike.fanxiaobao.xyz/Article/details/gxxvicldh.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fanxiaobao.xyz/Article/details/glbrlgcqs.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.fanxiaobao.xyz/Article/details/gxpjolibc.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.fanxiaobao.xyz/Article/details/glaysskuw.sHtML

[U61] PHP：正则
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gofjlvxkw.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gucguxaqt.sHtML

[U62] PHP：日期对象
来源：http://baike.fanxiaobao.xyz/Article/details/gdilxmnub.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.fanxiaobao.xyz/Article/details/gsesglagz.sHtML

[U63] PHP：文件读写
来源：http://3g.fanxiaobao.xyz/Article/details/gmbuyjxss.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.fanxiaobao.xyz/Article/details/grwggwwct.sHtML

[U64] PHP：目录遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gdwpmshrv.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.fanxiaobao.xyz/Article/details/gwusdkjvt.sHtML

[U65] PHP：会话
来源：http://wap.fanxiaobao.xyz/Article/details/gcuatgcnp.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gplpbnxws.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.fanxiaobao.xyz/Article/details/gwsdgryig.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.fanxiaobao.xyz/Article/details/gshktcllx.sHtML


<!-- 参考信息 -->