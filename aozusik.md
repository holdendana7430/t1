代发 wailian999

[S41] C++：类与构造函数
来源：http://mobile.fehbvm.com/Article/details/gudcsxwvk.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.hesvh.cn/Article/details/goadgpvyu.sHtML

[S42] C++：继承与虚函数
来源：http://baike.hesvh.cn/Article/details/gmqekaazu.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.zdbjq.cn/Article/details/gjmnwjpgp.sHtML

[S43] C++：智能指针
来源：http://m.share.fehbvm.com/Article/details/gcldakpbh.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.hesvh.cn/Article/details/gjyldxdaa.sHtML

[S44] C++：引用传参
来源：http://mobile.fehbvm.com/Article/details/geqlfepmu.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.hesvh.cn/Article/details/gurtjiqpc.sHtML

[S45] C++：lambda
来源：http://blog.hesvh.cn/Article/details/gkexteqte.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.hesvh.cn/Article/details/grpdjyudo.sHtML

[S46] C++：函数模板
来源：http://3g.fehbvm.com/Article/details/gcztwmskh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fehbvm.com/Article/details/gikavwiww.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fehbvm.com/Article/details/ghvlxuxfg.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.hesvh.cn/Article/details/gasrvbgok.sHtML

[S48] C++：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gmefsiilh.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fehbvm.com/Article/details/gcfspxxpb.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fehbvm.com/Article/details/glhchkbxk.sHtML

[S49] C++：写文件
来源：http://mobile.fehbvm.com/Article/details/gtiraqmdq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.hesvh.cn/Article/details/gladoyxgy.sHtML

[S50] C++：格式化数字
来源：http://m.share.zdbjq.cn/Article/details/gbbbylqsg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gnvgxirqe.sHtML

[S51] C++：显式类型转换
来源：http://3g.fehbvm.com/Article/details/gsiewyxji.sHtML

static_cast<double>(a) / b
来源：http://3g.hesvh.cn/Article/details/gdwxlqbif.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.hesvh.cn/Article/details/geopzvwyq.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.hesvh.cn/Article/details/gqilalfoq.sHtML

[S53] C++：移动语义
来源：http://m.share.fehbvm.com/Article/details/gxapvyvgl.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.zdbjq.cn/Article/details/gwyeyguih.sHtML

[S54] C++：异常处理
来源：http://www.blog.fehbvm.com/Article/details/gsajojqyh.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fehbvm.com/Article/details/gnzctqecl.sHtML

[S55] C++：结构化绑定
来源：http://m.share.zdbjq.cn/Article/details/gttmsbohq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fehbvm.com/Article/details/glrzogetd.sHtML

[S56] C++：optional
来源：http://blog.zdbjq.cn/Article/details/gepmnrmxs.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.hesvh.cn/Article/details/gydzgvhgk.sHtML

[S57] C++：编译期常量
来源：http://www.share.hesvh.cn/Article/details/geognweet.sHtML

constexpr int N = 10;
来源：http://read.share.zdbjq.cn/Article/details/gjmrirbjf.sHtML

[S58] C++：命名空间
来源：http://baike.fehbvm.com/Article/details/guolqwzjs.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.hesvh.cn/Article/details/gdyxqqxgs.sHtML

[S59] C++：静态断言
来源：http://m.share.hesvh.cn/Article/details/gdrhjqwnf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fehbvm.com/Article/details/gbkjwfpkk.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fehbvm.com/Article/details/gbrjkdgpi.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/gzkznvpvu.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gufttkqvo.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fehbvm.com/Article/details/ghvafycde.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/glclhhirr.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.zdbjq.cn/Article/details/ghqxhoxfv.sHtML

println("Hello")
来源：http://www.share.hesvh.cn/Article/details/gscphmlcy.sHtML

[T02] Kotlin：变量
来源：http://mobile.zdbjq.cn/Article/details/gbpwbnvws.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.hesvh.cn/Article/details/gnorlxlwi.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.hesvh.cn/Article/details/gvbkgfxqr.sHtML

"值: $b"
来源：http://mobile.hesvh.cn/Article/details/gkqdwzhbb.sHtML

[T04] Kotlin：空安全
来源：http://mobile.hesvh.cn/Article/details/glwtyegtt.sHtML

val n: String? = null;  n?.length
来源：http://3g.zdbjq.cn/Article/details/gvrnpuzrs.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fehbvm.com/Article/details/gshqvvmxt.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fehbvm.com/Article/details/gutstmhbc.sHtML

[T06] Kotlin：集合映射
来源：http://blog.zdbjq.cn/Article/details/gmujcmexx.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gafwoiqmo.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.hesvh.cn/Article/details/gaaxsrlsl.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.hesvh.cn/Article/details/gaaznemsd.sHtML

[T08] Kotlin：数据类
来源：http://blog.hesvh.cn/Article/details/gciwrdvth.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fehbvm.com/Article/details/gpnrnjczn.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.zdbjq.cn/Article/details/gosihpdrp.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.zdbjq.cn/Article/details/grcyzklut.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.hesvh.cn/Article/details/gqxkxwdcg.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.zdbjq.cn/Article/details/genvopmqf.sHtML

[T11] Kotlin：协程
来源：http://mobile.zdbjq.cn/Article/details/gcnzwapvd.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.zdbjq.cn/Article/details/gbnvweuxp.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fehbvm.com/Article/details/gqfhoxmyg.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/glgaztkxs.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.hesvh.cn/Article/details/gpakjdcdx.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.hesvh.cn/Article/details/gotfxmiew.sHtML

[T14] Kotlin：循环
来源：http://baike.fehbvm.com/Article/details/gnzxdjesd.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/giewxkrsg.sHtML

[T15] Kotlin：接口
来源：http://m.share.fehbvm.com/Article/details/ghykvrgqm.sHtML

interface Shape { fun area(): Double }
来源：http://wap.hesvh.cn/Article/details/gajzzezfy.sHtML

[T16] Swift：Hello World
来源：http://blog.zdbjq.cn/Article/details/gdornwuql.sHtML

print("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gvzvgifgz.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fehbvm.com/Article/details/gjqlqhjtx.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gxalndqkm.sHtML

[T18] Swift：字符串插值
来源：http://wap.fehbvm.com/Article/details/gklfhgmsx.sHtML

"值: \(b)"
来源：http://3g.hesvh.cn/Article/details/ghbcqrqcx.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.hesvh.cn/Article/details/guyouprcz.sHtML

if let n = opt { print(n) }
来源：http://blog.fehbvm.com/Article/details/gludbwtwh.sHtML

[T20] Swift：数组操作
来源：http://3g.hesvh.cn/Article/details/guexbjpxi.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.hesvh.cn/Article/details/gskugrrqz.sHtML

[T21] Swift：遍历
来源：http://blog.zdbjq.cn/Article/details/gmoyasnwx.sHtML

for x in a { print(x) }
来源：http://blog.fehbvm.com/Article/details/gxkcyzleq.sHtML

[T22] Swift：字典
来源：http://read.share.fehbvm.com/Article/details/gsyejwkyq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.zdbjq.cn/Article/details/gtbcttiuj.sHtML

[T23] Swift：函数
来源：http://mobile.hesvh.cn/Article/details/gjblxvcth.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.hesvh.cn/Article/details/gbgyhzsaf.sHtML

[T24] Swift：闭包
来源：http://read.share.fehbvm.com/Article/details/gjqsogmlw.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gtmywqntw.sHtML

[T25] Swift：结构体
来源：http://wap.zdbjq.cn/Article/details/gvzfughlz.sHtML

struct P { var x: Int }
来源：http://read.share.hesvh.cn/Article/details/grqgzvirh.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.hesvh.cn/Article/details/gvtzzdcjz.sHtML

class A: Base { override func f() {} }
来源：http://blog.fehbvm.com/Article/details/gkgkilale.sHtML

[T27] Swift：错误处理
来源：http://m.share.hesvh.cn/Article/details/gsrnlrxax.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.hesvh.cn/Article/details/gclcjztmh.sHtML

[T28] Swift：枚举
来源：http://mobile.fehbvm.com/Article/details/gmpcjsisq.sHtML

enum Color { case red, green }
来源：http://3g.hesvh.cn/Article/details/gkkhrgpqd.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.fehbvm.com/Article/details/gqneybrop.sHtML

guard let x = opt else { return }
来源：http://3g.hesvh.cn/Article/details/gaqlsusxu.sHtML

[T30] Swift：协议
来源：http://baike.zdbjq.cn/Article/details/gdsmxnmrp.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.fehbvm.com/Article/details/gbqwkhvqp.sHtML

[T31] Lua：Hello World
来源：http://3g.zdbjq.cn/Article/details/gzfroxvoc.sHtML

print("Hello")
来源：http://wap.fehbvm.com/Article/details/gmttjorxs.sHtML

[T32] Lua：局部变量
来源：http://read.share.hesvh.cn/Article/details/guivfjawi.sHtML

local a = 1
来源：http://read.share.hesvh.cn/Article/details/gvumkefnc.sHtML

[T33] Lua：表（数组）
来源：http://3g.zdbjq.cn/Article/details/gifpnaygs.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.zdbjq.cn/Article/details/gxwfgfyna.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.fehbvm.com/Article/details/gljznwqwd.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.hesvh.cn/Article/details/gvedzdvdc.sHtML

[T35] Lua：字典表
来源：http://baike.zdbjq.cn/Article/details/gqaailyjc.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.zdbjq.cn/Article/details/gnmdejkjn.sHtML

[T36] Lua：函数
来源：http://wap.zdbjq.cn/Article/details/gbklhldut.sHtML

function add(a, b) return a + b end
来源：http://read.share.zdbjq.cn/Article/details/gbocairfh.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.fehbvm.com/Article/details/gktinanby.sHtML

"a" .. "b"
来源：http://www.share.hesvh.cn/Article/details/gpnwpawtx.sHtML

[T38] Lua：条件
来源：http://www.share.zdbjq.cn/Article/details/gocygqkxx.sHtML

if x > 0 then print("正") end
来源：http://3g.hesvh.cn/Article/details/gtvetikuh.sHtML

[T39] Lua：模式匹配
来源：http://3g.fehbvm.com/Article/details/gkxnmdxyh.sHtML

string.find(s, "%d+")
来源：http://m.share.hesvh.cn/Article/details/gaukbtyav.sHtML

[T40] Lua：元表
来源：http://baike.fehbvm.com/Article/details/gtspuzeje.sHtML

setmetatable({}, { __index = base })
来源：http://blog.hesvh.cn/Article/details/gjyezwnpr.sHtML

[T41] Perl：Hello World
来源：http://blog.fehbvm.com/Article/details/gzmbpgxyx.sHtML

print "Hello\n";
来源：http://www.share.hesvh.cn/Article/details/gajvwsqnz.sHtML

[T42] Perl：变量类型
来源：http://baike.zdbjq.cn/Article/details/gttpuawqb.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.fehbvm.com/Article/details/gtjhpksja.sHtML

[T43] Perl：字符串插值
来源：http://wap.hesvh.cn/Article/details/ggwwaltkd.sHtML

"值: $a"
来源：http://www.share.hesvh.cn/Article/details/gypyvrqvg.sHtML

[T44] Perl：条件
来源：http://www.share.fehbvm.com/Article/details/gbynkeytc.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.hesvh.cn/Article/details/gjtmoajck.sHtML

[T45] Perl：数组遍历
来源：http://mobile.fehbvm.com/Article/details/gvzvdfoyh.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.hesvh.cn/Article/details/gertnrrzv.sHtML

[T46] Perl：哈希操作
来源：http://wap.hesvh.cn/Article/details/govmnaonk.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.zdbjq.cn/Article/details/geywubwun.sHtML

[T47] Perl：正则捕获
来源：http://read.share.hesvh.cn/Article/details/gduhikbof.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.zdbjq.cn/Article/details/gyfgykuhg.sHtML

[T48] Perl：正则替换
来源：http://m.share.fehbvm.com/Article/details/gsqhsntrb.sHtML

$s =~ s/old/new/g;
来源：http://www.share.hesvh.cn/Article/details/gwidgzxsi.sHtML

[T49] Perl：函数
来源：http://www.blog.fehbvm.com/Article/details/glswrbaje.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gnanskcno.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gjpbdryyl.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.hesvh.cn/Article/details/gndkubvmx.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.fehbvm.com/Article/details/gmyvryegr.sHtML

[T51] Scala：Hello World
来源：http://read.share.fehbvm.com/Article/details/gtgkfitpg.sHtML

println("Hello")
来源：http://www.blog.fehbvm.com/Article/details/guipttifb.sHtML

[T52] Scala：变量
来源：http://www.blog.fehbvm.com/Article/details/glvsoozvl.sHtML

val a = 1;  var b = 2
来源：http://baike.zdbjq.cn/Article/details/guxapbsjt.sHtML

[T53] Scala：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gqryqyoni.sHtML

s"值: $b"
来源：http://www.m.share.fehbvm.com/Article/details/gtezearqi.sHtML

[T54] Scala：集合映射
来源：http://www.blog.fehbvm.com/Article/details/gkzcugujk.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.hesvh.cn/Article/details/gjmotkgir.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fehbvm.com/Article/details/gtlxgwdza.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.hesvh.cn/Article/details/gboqkwvwd.sHtML

[T56] Scala：样例类
来源：http://www.m.share.hesvh.cn/Article/details/gfltnceus.sHtML

case class User(name: String, age: Int)
来源：http://m.share.hesvh.cn/Article/details/gmcfnpavo.sHtML

[T57] Scala：模式匹配
来源：http://wap.zdbjq.cn/Article/details/gjspygcxe.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.fehbvm.com/Article/details/gqtllskme.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.fehbvm.com/Article/details/gkxcwqqyz.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.hesvh.cn/Article/details/ghsaesprj.sHtML

[T59] Scala：循环
来源：http://www.blog.hesvh.cn/Article/details/gzzxnjggk.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.hesvh.cn/Article/details/ghhynggir.sHtML

[T60] Scala：折叠
来源：http://wap.fehbvm.com/Article/details/gmvdzvlhc.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.fehbvm.com/Article/details/gvewcetmv.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gbfwewwua.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fehbvm.com/Article/details/gawlkjxzq.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gjemvhndd.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.fehbvm.com/Article/details/gfuvhpofk.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.hesvh.cn/Article/details/glwfdsccu.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.zdbjq.cn/Article/details/gvidzbofp.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.hesvh.cn/Article/details/gjkwixlgm.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.fehbvm.com/Article/details/gzlietekj.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.hesvh.cn/Article/details/gyntfxmac.sHtML

[U04] Py：变量调试打印
来源：http://baike.hesvh.cn/Article/details/gfaxmiasg.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fehbvm.com/Article/details/gaaedgrkx.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.fehbvm.com/Article/details/glaxjqkhf.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.zdbjq.cn/Article/details/gflnazywm.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.fehbvm.com/Article/details/gurugtyeq.sHtML

{**a, **b}
来源：http://www.m.share.hesvh.cn/Article/details/gfvotqlkp.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.zdbjq.cn/Article/details/gcloebjjt.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.hesvh.cn/Article/details/guhgbexrk.sHtML

[U08] Py：展平二维列表
来源：http://read.share.zdbjq.cn/Article/details/gbtjmovzw.sHtML

[y for x in nested for y in x]
来源：http://m.share.zdbjq.cn/Article/details/ggvmikhug.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.zdbjq.cn/Article/details/gdystjqce.sHtML

max(d, key=d.get)
来源：http://m.share.fehbvm.com/Article/details/gzuhkbgwy.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.fehbvm.com/Article/details/gsrzrajfb.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.zdbjq.cn/Article/details/gzlevlksb.sHtML

[U11] Py：生成器表达式
来源：http://mobile.fehbvm.com/Article/details/gncvaprjr.sHtML

(x * 2 for x in arr)
来源：http://mobile.zdbjq.cn/Article/details/goiqrwsvn.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.fehbvm.com/Article/details/grbyrftjh.sHtML

Counter(arr).most_common(3)
来源：http://read.share.fehbvm.com/Article/details/gduyvwrgk.sHtML

[U13] Py：固定长度队列
来源：http://wap.fehbvm.com/Article/details/grgxhlpcr.sHtML

deque(maxlen=10)
来源：http://3g.fehbvm.com/Article/details/gkwvfzwuy.sHtML

[U14] Py：分组收集到列表
来源：http://baike.hesvh.cn/Article/details/gcdqqmjcd.sHtML

defaultdict(list)
来源：http://read.share.hesvh.cn/Article/details/goabkzjtm.sHtML

[U15] Py：高精度计时
来源：http://m.share.zdbjq.cn/Article/details/gechjhmvf.sHtML

t = time.perf_counter()
来源：http://baike.zdbjq.cn/Article/details/geecwvuat.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.zdbjq.cn/Article/details/gjnhleyhs.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.hesvh.cn/Article/details/gdchkfhlu.sHtML

[U17] Py：初始化日志
来源：http://blog.hesvh.cn/Article/details/gmxyvzlep.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.hesvh.cn/Article/details/gwhrnvbkg.sHtML

[U18] Py：预编译正则
来源：http://blog.hesvh.cn/Article/details/glghhkbmk.sHtML

pat = re.compile(r"\d+")
来源：http://3g.hesvh.cn/Article/details/gbylzytcr.sHtML

[U19] Py：正则替换带回调
来源：http://wap.fehbvm.com/Article/details/gsptnqsii.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.zdbjq.cn/Article/details/gciiqrlos.sHtML

[U20] Py：缓存函数结果
来源：http://blog.fehbvm.com/Article/details/gyhjlwbqb.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.zdbjq.cn/Article/details/gagydkyfe.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.zdbjq.cn/Article/details/gigzcczcp.sHtML

@contextlib.contextmanager
来源：http://mobile.hesvh.cn/Article/details/ghfypskbm.sHtML

[U22] Py：矩阵转置
来源：http://blog.hesvh.cn/Article/details/gmfdbwtuc.sHtML

list(zip(*m))
来源：http://wap.fehbvm.com/Article/details/gfmccubgd.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.zdbjq.cn/Article/details/gtscneksm.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.fehbvm.com/Article/details/gpflvtefp.sHtML

[U24] Py：路径操作
来源：http://blog.hesvh.cn/Article/details/gqnalxebi.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.hesvh.cn/Article/details/gvbwnmvlv.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.fehbvm.com/Article/details/gqzcnapva.sHtML

csv.DictReader(f)
来源：http://baike.zdbjq.cn/Article/details/gjtdxcshq.sHtML

[U26] Py：并发下载
来源：http://baike.zdbjq.cn/Article/details/gtlqrkobj.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.hesvh.cn/Article/details/gcveczrni.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.hesvh.cn/Article/details/gflnrevgf.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.zdbjq.cn/Article/details/gojkptsxh.sHtML

[U28] Py：类型别名
来源：http://www.m.share.hesvh.cn/Article/details/gsdwrdzdk.sHtML

UserId = int
来源：http://baike.fehbvm.com/Article/details/gwyvjncic.sHtML

[U29] Py：属性校验
来源：http://www.share.zdbjq.cn/Article/details/gaupnyuul.sHtML

@property 与 @x.setter 配合
来源：http://baike.fehbvm.com/Article/details/gsieqktqq.sHtML

[U30] Py：数据类
来源：http://www.share.hesvh.cn/Article/details/gvejenqzg.sHtML

@dataclass(slots=True)
来源：http://read.share.fehbvm.com/Article/details/gutptocke.sHtML

[U31] Py：单测
来源：http://wap.fehbvm.com/Article/details/gadywtdxz.sHtML

python -m pytest -q
来源：http://blog.fehbvm.com/Article/details/gvqtlfmfc.sHtML

[U32] Py：代码格式化
来源：http://wap.hesvh.cn/Article/details/gtcclxjwl.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.fehbvm.com/Article/details/gxkrtrjzu.sHtML

[U33] Py：打包发布
来源：http://www.m.share.zdbjq.cn/Article/details/goanrjbfx.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.fehbvm.com/Article/details/gyjfnegmp.sHtML

[U34] Py：判断编码
来源：http://mobile.zdbjq.cn/Article/details/gjljuirwz.sHtML

chardet.detect(raw)
来源：http://wap.zdbjq.cn/Article/details/gjkusricn.sHtML

[U35] Py：发送邮件
来源：http://mobile.hesvh.cn/Article/details/gnvdzgusf.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.zdbjq.cn/Article/details/gjnirnwzz.sHtML

[U36] Py：定时任务
来源：http://mobile.zdbjq.cn/Article/details/ggfqfbqsx.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.hesvh.cn/Article/details/gyrjbqpdi.sHtML

[U37] Py：读写 Excel
来源：http://wap.zdbjq.cn/Article/details/goplqsefm.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.zdbjq.cn/Article/details/gmpcsiueb.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fehbvm.com/Article/details/goudverbs.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.zdbjq.cn/Article/details/gswngzpif.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.hesvh.cn/Article/details/gjlobxjsk.sHtML

sys.stdout.isatty()
来源：http://read.share.zdbjq.cn/Article/details/gfgsgnghz.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.hesvh.cn/Article/details/gvprppbop.sHtML

print("err", file=sys.stderr)
来源：http://blog.fehbvm.com/Article/details/gsuzpxabo.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.fehbvm.com/Article/details/gmenhzukf.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.zdbjq.cn/Article/details/gqsnnkfim.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.zdbjq.cn/Article/details/gmgvnceyp.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.fehbvm.com/Article/details/giudpmcll.sHtML

[U43] PHP：声明命名空间
来源：http://wap.hesvh.cn/Article/details/gjhrpmfae.sHtML

namespace App\Http;
来源：http://read.share.fehbvm.com/Article/details/gbsxhddkq.sHtML

[U44] PHP：开启严格类型
来源：http://wap.fehbvm.com/Article/details/gbawgjbcw.sHtML

declare(strict_types=1);
来源：http://m.share.zdbjq.cn/Article/details/gqhyotvca.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.hesvh.cn/Article/details/gpthsqfng.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gpntvfozu.sHtML

[U46] PHP：可空类型
来源：http://wap.fehbvm.com/Article/details/gbemudhtt.sHtML

?string $name = null
来源：http://m.share.hesvh.cn/Article/details/gizxogqfy.sHtML

[U47] PHP：联合类型
来源：http://mobile.fehbvm.com/Article/details/grwojsapo.sHtML

int|string $id
来源：http://www.share.zdbjq.cn/Article/details/glxlnehlj.sHtML

[U48] PHP：纯枚举
来源：http://3g.fehbvm.com/Article/details/gqdjobsel.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.fehbvm.com/Article/details/gynjyqrll.sHtML

[U49] PHP：只读属性
来源：http://wap.zdbjq.cn/Article/details/gwpzgbfmr.sHtML

public readonly string $name
来源：http://m.share.fehbvm.com/Article/details/gocwabuci.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.zdbjq.cn/Article/details/gzouzfkbc.sHtML

public function __construct(private int $id) {}
来源：http://read.share.fehbvm.com/Article/details/glolvmrqb.sHtML

[U51] PHP：数组解构
来源：http://www.share.zdbjq.cn/Article/details/gsnigzlak.sHtML

[$a, $b] = $arr;
来源：http://m.share.fehbvm.com/Article/details/gbpdgptgp.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.hesvh.cn/Article/details/gpnemfjeo.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.fehbvm.com/Article/details/gvunhrylt.sHtML

[U53] PHP：空合并运算符
来源：http://blog.fehbvm.com/Article/details/goxfsvgqt.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.hesvh.cn/Article/details/gwbcrbsgm.sHtML

[U54] PHP：空安全调用
来源：http://www.share.zdbjq.cn/Article/details/gamvcxsja.sHtML

$obj?->method()
来源：http://www.blog.zdbjq.cn/Article/details/gpzvydyla.sHtML

[U55] PHP：match 表达式
来源：http://blog.hesvh.cn/Article/details/gcenjomfq.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.fehbvm.com/Article/details/ghpshlffw.sHtML

[U56] PHP：命名参数
来源：http://m.share.fehbvm.com/Article/details/gdjpfviwl.sHtML

f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/gzmvacdtm.sHtML

[U57] PHP：字符串插值
来源：http://blog.fehbvm.com/Article/details/gpeihxdgx.sHtML

"值: {$a}"
来源：http://m.share.zdbjq.cn/Article/details/gykhstgnv.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.fehbvm.com/Article/details/gvmemceig.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.zdbjq.cn/Article/details/gybhltdmg.sHtML

[U59] PHP：自定义排序
来源：http://mobile.zdbjq.cn/Article/details/gnxazcvyv.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.zdbjq.cn/Article/details/gugnhybti.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.hesvh.cn/Article/details/gqvwrckly.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.zdbjq.cn/Article/details/gdxhdnltz.sHtML

[U61] PHP：正则
来源：http://baike.zdbjq.cn/Article/details/ggnxlnsil.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.hesvh.cn/Article/details/ggjmynnvp.sHtML

[U62] PHP：日期对象
来源：http://www.blog.zdbjq.cn/Article/details/guelahazx.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.hesvh.cn/Article/details/gxhsvnzps.sHtML

[U63] PHP：文件读写
来源：http://www.blog.hesvh.cn/Article/details/geskubqux.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.hesvh.cn/Article/details/gxkqukgel.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.hesvh.cn/Article/details/gjefdjsor.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.zdbjq.cn/Article/details/gxgzbrooj.sHtML

[U65] PHP：会话
来源：http://mobile.zdbjq.cn/Article/details/gauvhziih.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gxcbhjnni.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.hesvh.cn/Article/details/gihlxmfft.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.zdbjq.cn/Article/details/gqruruigq.sHtML


<!-- 参考信息 -->