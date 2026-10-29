代发 wailian999

[S41] C++：类与构造函数
来源：http://m.share.zdbjq.cn/Article/details/gthadxuwh.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.hesvh.cn/Article/details/gyvapitld.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.zdbjq.cn/Article/details/govgvttlo.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.zdbjq.cn/Article/details/ghvxgcyrf.sHtML

[S43] C++：智能指针
来源：http://blog.hesvh.cn/Article/details/gxkhpsrwt.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fehbvm.com/Article/details/gielyjqth.sHtML

[S44] C++：引用传参
来源：http://blog.hesvh.cn/Article/details/gjvcpxtmb.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.hesvh.cn/Article/details/gvavvrubu.sHtML

[S45] C++：lambda
来源：http://blog.fehbvm.com/Article/details/gtilaaekw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.zdbjq.cn/Article/details/gpenzrnua.sHtML

[S46] C++：函数模板
来源：http://read.share.zdbjq.cn/Article/details/gfckrdxnr.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fehbvm.com/Article/details/gklmgmhxz.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fehbvm.com/Article/details/gxgdkquck.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.zdbjq.cn/Article/details/gesqhavah.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gwlfmddev.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.hesvh.cn/Article/details/gbgweoywh.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.zdbjq.cn/Article/details/gixghulsi.sHtML

[S49] C++：写文件
来源：http://www.blog.hesvh.cn/Article/details/ggtciahph.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fehbvm.com/Article/details/gaokdnkcl.sHtML

[S50] C++：格式化数字
来源：http://read.share.hesvh.cn/Article/details/gonqbjrsp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/ggofcofhs.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/ghuecvgga.sHtML

static_cast<double>(a) / b
来源：http://mobile.hesvh.cn/Article/details/gnccrbowu.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.zdbjq.cn/Article/details/gkoesfpys.sHtML

int size() const noexcept { return n_; }
来源：http://baike.zdbjq.cn/Article/details/gbuposcvy.sHtML

[S53] C++：移动语义
来源：http://3g.zdbjq.cn/Article/details/ggrrzybyo.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fehbvm.com/Article/details/gmeijgobc.sHtML

[S54] C++：异常处理
来源：http://mobile.fehbvm.com/Article/details/grjylojbx.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fehbvm.com/Article/details/gompdwmmh.sHtML

[S55] C++：结构化绑定
来源：http://mobile.zdbjq.cn/Article/details/ghtqwugur.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fehbvm.com/Article/details/gkjkdekyk.sHtML

[S56] C++：optional
来源：http://www.m.share.fehbvm.com/Article/details/grjeumopc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fehbvm.com/Article/details/gnwrgqvac.sHtML

[S57] C++：编译期常量
来源：http://www.share.fehbvm.com/Article/details/gebwylzxn.sHtML

constexpr int N = 10;
来源：http://3g.fehbvm.com/Article/details/gvdgrpehu.sHtML

[S58] C++：命名空间
来源：http://read.share.hesvh.cn/Article/details/ginddadbw.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.hesvh.cn/Article/details/gatsvincc.sHtML

[S59] C++：静态断言
来源：http://3g.zdbjq.cn/Article/details/gilnnsrzi.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.hesvh.cn/Article/details/gajqfhvgw.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.zdbjq.cn/Article/details/gmcbcilxb.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fehbvm.com/Article/details/gjmqsbnap.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gavjvcntr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.hesvh.cn/Article/details/ghnsszugh.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gmtezidzm.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gsiodaqll.sHtML

println("Hello")
来源：http://3g.zdbjq.cn/Article/details/geppsrxzr.sHtML

[T02] Kotlin：变量
来源：http://read.share.zdbjq.cn/Article/details/gifbwypoo.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fehbvm.com/Article/details/gszjuzirh.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.zdbjq.cn/Article/details/glmyniwlr.sHtML

"值: $b"
来源：http://read.share.fehbvm.com/Article/details/gcyrezgta.sHtML

[T04] Kotlin：空安全
来源：http://baike.hesvh.cn/Article/details/gncnocmks.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fehbvm.com/Article/details/gwacxwffy.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fehbvm.com/Article/details/gictyatpq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.hesvh.cn/Article/details/gpxrrwqri.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.hesvh.cn/Article/details/gnorpvzsw.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gvshfhjxm.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.zdbjq.cn/Article/details/gwneujytb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.hesvh.cn/Article/details/gqgwinrye.sHtML

[T08] Kotlin：数据类
来源：http://www.share.zdbjq.cn/Article/details/gzuopxunc.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fehbvm.com/Article/details/gzrypnxzi.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fehbvm.com/Article/details/gdifatodr.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.hesvh.cn/Article/details/gkgoljkgz.sHtML

[T10] Kotlin：默认参数
来源：http://baike.hesvh.cn/Article/details/gjohopssj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.zdbjq.cn/Article/details/gfzbsjtio.sHtML

[T11] Kotlin：协程
来源：http://3g.zdbjq.cn/Article/details/gmikrxoac.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.hesvh.cn/Article/details/gxqcmqudn.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fehbvm.com/Article/details/ggwmaogfz.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gmsmkojff.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.hesvh.cn/Article/details/gcszxpqxk.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.zdbjq.cn/Article/details/gnmmwykjb.sHtML

[T14] Kotlin：循环
来源：http://3g.zdbjq.cn/Article/details/ghzpjnsqw.sHtML

for (i in 1..10) println(i)
来源：http://mobile.hesvh.cn/Article/details/gkbkojxkz.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.hesvh.cn/Article/details/gwyqaemlz.sHtML

interface Shape { fun area(): Double }
来源：http://wap.zdbjq.cn/Article/details/gaofwtvvp.sHtML

[T16] Swift：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/godnwtnef.sHtML

print("Hello")
来源：http://m.share.fehbvm.com/Article/details/guevtergn.sHtML

[T17] Swift：变量与常量
来源：http://mobile.zdbjq.cn/Article/details/gueocmniw.sHtML

var a = 1;  let b = 2
来源：http://blog.hesvh.cn/Article/details/gmizgditm.sHtML

[T18] Swift：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gstgpoklj.sHtML

"值: \(b)"
来源：http://mobile.zdbjq.cn/Article/details/gpwovytws.sHtML

[T19] Swift：可选绑定
来源：http://wap.hesvh.cn/Article/details/gdwpkcymq.sHtML

if let n = opt { print(n) }
来源：http://m.share.hesvh.cn/Article/details/gjgbgfzef.sHtML

[T20] Swift：数组操作
来源：http://blog.hesvh.cn/Article/details/gdweifxlc.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.hesvh.cn/Article/details/goffntlrc.sHtML

[T21] Swift：遍历
来源：http://3g.fehbvm.com/Article/details/gcktgoref.sHtML

for x in a { print(x) }
来源：http://blog.hesvh.cn/Article/details/gondelfbc.sHtML

[T22] Swift：字典
来源：http://3g.fehbvm.com/Article/details/gxfiaurly.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.hesvh.cn/Article/details/gknylmjqr.sHtML

[T23] Swift：函数
来源：http://wap.fehbvm.com/Article/details/gxnoveawj.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.fehbvm.com/Article/details/goruuxuxg.sHtML

[T24] Swift：闭包
来源：http://www.share.zdbjq.cn/Article/details/gzjurwzkv.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.fehbvm.com/Article/details/ghbrmabjv.sHtML

[T25] Swift：结构体
来源：http://m.share.hesvh.cn/Article/details/gubonswvr.sHtML

struct P { var x: Int }
来源：http://3g.zdbjq.cn/Article/details/gxfevtyeq.sHtML

[T26] Swift：类与重写
来源：http://blog.zdbjq.cn/Article/details/gvfjpujvj.sHtML

class A: Base { override func f() {} }
来源：http://read.share.hesvh.cn/Article/details/gaenylzcn.sHtML

[T27] Swift：错误处理
来源：http://3g.hesvh.cn/Article/details/ggnfzxjzg.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fehbvm.com/Article/details/gcpbhjcgy.sHtML

[T28] Swift：枚举
来源：http://www.blog.fehbvm.com/Article/details/gvlepflkm.sHtML

enum Color { case red, green }
来源：http://www.blog.zdbjq.cn/Article/details/glvxacuoe.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.zdbjq.cn/Article/details/goeqogjjj.sHtML

guard let x = opt else { return }
来源：http://read.share.zdbjq.cn/Article/details/goqpufrcp.sHtML

[T30] Swift：协议
来源：http://m.share.hesvh.cn/Article/details/gtjzrnskz.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.zdbjq.cn/Article/details/gbwjweubt.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gjcrbaydf.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gvfzkilrw.sHtML

[T32] Lua：局部变量
来源：http://baike.fehbvm.com/Article/details/gvdfmicka.sHtML

local a = 1
来源：http://blog.zdbjq.cn/Article/details/gtzbtnqsy.sHtML

[T33] Lua：表（数组）
来源：http://wap.hesvh.cn/Article/details/gtpsqeugs.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.fehbvm.com/Article/details/gsbfxhxib.sHtML

[T34] Lua：遍历表
来源：http://www.share.hesvh.cn/Article/details/gpwbrvpmp.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.zdbjq.cn/Article/details/grsniahge.sHtML

[T35] Lua：字典表
来源：http://www.m.share.hesvh.cn/Article/details/gxyqruqqw.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fehbvm.com/Article/details/grrlawxtt.sHtML

[T36] Lua：函数
来源：http://read.share.hesvh.cn/Article/details/gvatswqki.sHtML

function add(a, b) return a + b end
来源：http://m.share.fehbvm.com/Article/details/gckutuuqk.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/grjhyvqwg.sHtML

"a" .. "b"
来源：http://wap.hesvh.cn/Article/details/gfbrjeroq.sHtML

[T38] Lua：条件
来源：http://m.share.hesvh.cn/Article/details/gybbfeblr.sHtML

if x > 0 then print("正") end
来源：http://www.blog.zdbjq.cn/Article/details/gocjlclts.sHtML

[T39] Lua：模式匹配
来源：http://m.share.zdbjq.cn/Article/details/gzxwkhuyu.sHtML

string.find(s, "%d+")
来源：http://baike.fehbvm.com/Article/details/gakxmvxfz.sHtML

[T40] Lua：元表
来源：http://3g.fehbvm.com/Article/details/gwolscvpe.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.fehbvm.com/Article/details/ggzpkcpiu.sHtML

[T41] Perl：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gewnipvfb.sHtML

print "Hello\n";
来源：http://www.blog.hesvh.cn/Article/details/gmjwbqxza.sHtML

[T42] Perl：变量类型
来源：http://www.blog.hesvh.cn/Article/details/gjshfdyej.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.fehbvm.com/Article/details/glyiovewe.sHtML

[T43] Perl：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gqswbnsud.sHtML

"值: $a"
来源：http://read.share.zdbjq.cn/Article/details/ghjlmvzqh.sHtML

[T44] Perl：条件
来源：http://blog.fehbvm.com/Article/details/ggbhvukjv.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.fehbvm.com/Article/details/gitjzbywm.sHtML

[T45] Perl：数组遍历
来源：http://www.share.hesvh.cn/Article/details/gnorbpdrw.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.hesvh.cn/Article/details/gkqcmxoqx.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.zdbjq.cn/Article/details/gcuqaipwk.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.hesvh.cn/Article/details/gmxgiuuud.sHtML

[T47] Perl：正则捕获
来源：http://3g.hesvh.cn/Article/details/gqcgcadfc.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.hesvh.cn/Article/details/gilrkfuoy.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.zdbjq.cn/Article/details/gablxxsyt.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.fehbvm.com/Article/details/gbmrpeqnz.sHtML

[T49] Perl：函数
来源：http://wap.hesvh.cn/Article/details/gsxyhzrmu.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gfomuhuum.sHtML

[T50] Perl：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gzfnpaacc.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.fehbvm.com/Article/details/gwdgiknrz.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.zdbjq.cn/Article/details/gypymodpr.sHtML

[T51] Scala：Hello World
来源：http://3g.hesvh.cn/Article/details/gpyvyeloy.sHtML

println("Hello")
来源：http://3g.fehbvm.com/Article/details/gpuyenrhq.sHtML

[T52] Scala：变量
来源：http://read.share.zdbjq.cn/Article/details/gwvzihija.sHtML

val a = 1;  var b = 2
来源：http://www.share.zdbjq.cn/Article/details/gxbslhujs.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gkuhfcbzo.sHtML

s"值: $b"
来源：http://baike.hesvh.cn/Article/details/ghgakwmcn.sHtML

[T54] Scala：集合映射
来源：http://www.share.zdbjq.cn/Article/details/ggeibgmig.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.fehbvm.com/Article/details/gnvczdyvd.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.fehbvm.com/Article/details/gdvhjvkzj.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.fehbvm.com/Article/details/gvbspodor.sHtML

[T56] Scala：样例类
来源：http://www.blog.zdbjq.cn/Article/details/gqohcyqya.sHtML

case class User(name: String, age: Int)
来源：http://baike.hesvh.cn/Article/details/gimpmxqcb.sHtML

[T57] Scala：模式匹配
来源：http://m.share.fehbvm.com/Article/details/gyuzdiuam.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.fehbvm.com/Article/details/gyjmzpzmv.sHtML

[T58] Scala：函数定义
来源：http://www.share.hesvh.cn/Article/details/giapzqsjy.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.hesvh.cn/Article/details/gmikofmvd.sHtML

[T59] Scala：循环
来源：http://www.blog.zdbjq.cn/Article/details/guozdiqwt.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.fehbvm.com/Article/details/gfirlglwk.sHtML

[T60] Scala：折叠
来源：http://3g.fehbvm.com/Article/details/gsxrdidts.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.hesvh.cn/Article/details/geslysdxi.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gxfjlczam.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.hesvh.cn/Article/details/gqmhngfds.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gohbkikhv.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.hesvh.cn/Article/details/golkebimk.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.zdbjq.cn/Article/details/gfhdfvzcr.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.zdbjq.cn/Article/details/geehphube.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fehbvm.com/Article/details/gbzjylryg.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.fehbvm.com/Article/details/gtydmbvwn.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.fehbvm.com/Article/details/gedcpbjmj.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.zdbjq.cn/Article/details/gxvgkddcw.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.hesvh.cn/Article/details/gsouxuidp.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.fehbvm.com/Article/details/gruklorjf.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.zdbjq.cn/Article/details/gzuyarqqg.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.hesvh.cn/Article/details/giymdgbqh.sHtML

{**a, **b}
来源：http://blog.zdbjq.cn/Article/details/gaicqlopd.sHtML

[U07] Py：反转字典键值
来源：http://3g.zdbjq.cn/Article/details/gqgtntcdb.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.fehbvm.com/Article/details/gbzyaaxms.sHtML

[U08] Py：展平二维列表
来源：http://read.share.fehbvm.com/Article/details/gxaymhsnw.sHtML

[y for x in nested for y in x]
来源：http://www.share.hesvh.cn/Article/details/gjxincppz.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.fehbvm.com/Article/details/gevzumoue.sHtML

max(d, key=d.get)
来源：http://www.m.share.hesvh.cn/Article/details/gyqdwgxdt.sHtML

[U10] Py：按值排序字典
来源：http://blog.zdbjq.cn/Article/details/guamydxmr.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.zdbjq.cn/Article/details/gkdvtttsr.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.zdbjq.cn/Article/details/gyoxfhkqf.sHtML

(x * 2 for x in arr)
来源：http://m.share.zdbjq.cn/Article/details/gbtsldpai.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.hesvh.cn/Article/details/gmvalucia.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.hesvh.cn/Article/details/glbarehbo.sHtML

[U13] Py：固定长度队列
来源：http://m.share.zdbjq.cn/Article/details/gitwmhqcj.sHtML

deque(maxlen=10)
来源：http://3g.zdbjq.cn/Article/details/grihvwptt.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.zdbjq.cn/Article/details/goswcdsyg.sHtML

defaultdict(list)
来源：http://www.blog.fehbvm.com/Article/details/gsmayiiny.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.zdbjq.cn/Article/details/gygiauaca.sHtML

t = time.perf_counter()
来源：http://www.share.zdbjq.cn/Article/details/gahjbsccz.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.hesvh.cn/Article/details/grjgzofap.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.hesvh.cn/Article/details/gvnnxgyar.sHtML

[U17] Py：初始化日志
来源：http://wap.fehbvm.com/Article/details/gsittngob.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.hesvh.cn/Article/details/gaqdfuytn.sHtML

[U18] Py：预编译正则
来源：http://3g.hesvh.cn/Article/details/grjpcjmlt.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.zdbjq.cn/Article/details/gdbesvcrp.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.hesvh.cn/Article/details/gisyibijg.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fehbvm.com/Article/details/gupivucvn.sHtML

[U20] Py：缓存函数结果
来源：http://wap.hesvh.cn/Article/details/gbtahwclr.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.hesvh.cn/Article/details/gbvchtlvb.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.fehbvm.com/Article/details/guknfobyx.sHtML

@contextlib.contextmanager
来源：http://read.share.zdbjq.cn/Article/details/gtixxfhfz.sHtML

[U22] Py：矩阵转置
来源：http://blog.zdbjq.cn/Article/details/gkotgrxzu.sHtML

list(zip(*m))
来源：http://www.blog.zdbjq.cn/Article/details/gelxshufr.sHtML

[U23] Py：分块读取大文件
来源：http://baike.fehbvm.com/Article/details/gtgrouakf.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.fehbvm.com/Article/details/gqjwqfvwq.sHtML

[U24] Py：路径操作
来源：http://wap.fehbvm.com/Article/details/gqpakwxcy.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/guxnlgdvb.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.fehbvm.com/Article/details/gvjwzcaff.sHtML

csv.DictReader(f)
来源：http://3g.hesvh.cn/Article/details/ghqzzajwo.sHtML

[U26] Py：并发下载
来源：http://blog.fehbvm.com/Article/details/gfrxvrymb.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.hesvh.cn/Article/details/gptkfyswr.sHtML

[U27] Py：异步 HTTP
来源：http://blog.hesvh.cn/Article/details/guoreofdd.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.fehbvm.com/Article/details/ghbyuilra.sHtML

[U28] Py：类型别名
来源：http://read.share.zdbjq.cn/Article/details/ggqhhizea.sHtML

UserId = int
来源：http://m.share.zdbjq.cn/Article/details/govhbqxxb.sHtML

[U29] Py：属性校验
来源：http://blog.zdbjq.cn/Article/details/gxwqxonwh.sHtML

@property 与 @x.setter 配合
来源：http://wap.zdbjq.cn/Article/details/ggaytzygo.sHtML

[U30] Py：数据类
来源：http://www.blog.fehbvm.com/Article/details/gnbljjcaj.sHtML

@dataclass(slots=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gotcvxwcb.sHtML

[U31] Py：单测
来源：http://www.m.share.hesvh.cn/Article/details/gzegvaxkf.sHtML

python -m pytest -q
来源：http://blog.hesvh.cn/Article/details/gukztzklk.sHtML

[U32] Py：代码格式化
来源：http://read.share.zdbjq.cn/Article/details/gowpxywgd.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.hesvh.cn/Article/details/gjvsfbedw.sHtML

[U33] Py：打包发布
来源：http://m.share.zdbjq.cn/Article/details/gxtobptdk.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.zdbjq.cn/Article/details/gayruqhmx.sHtML

[U34] Py：判断编码
来源：http://www.share.hesvh.cn/Article/details/gsrwbwnnz.sHtML

chardet.detect(raw)
来源：http://read.share.hesvh.cn/Article/details/gyxkmoiiq.sHtML

[U35] Py：发送邮件
来源：http://www.blog.zdbjq.cn/Article/details/gmcnlzhml.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.fehbvm.com/Article/details/gndzpwbeq.sHtML

[U36] Py：定时任务
来源：http://blog.fehbvm.com/Article/details/gctezjbse.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.hesvh.cn/Article/details/gujqbuvev.sHtML

[U37] Py：读写 Excel
来源：http://3g.hesvh.cn/Article/details/gtkvozjru.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.fehbvm.com/Article/details/gcrauyyro.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.hesvh.cn/Article/details/gcfxlqgmk.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.fehbvm.com/Article/details/givijedvg.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.zdbjq.cn/Article/details/gdhxrghec.sHtML

sys.stdout.isatty()
来源：http://wap.zdbjq.cn/Article/details/glsknztaz.sHtML

[U40] Py：打印到标准错误
来源：http://blog.fehbvm.com/Article/details/ggxzyuean.sHtML

print("err", file=sys.stderr)
来源：http://mobile.fehbvm.com/Article/details/gtgnvatfw.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.fehbvm.com/Article/details/gyjllmxya.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.fehbvm.com/Article/details/gnblabgol.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.zdbjq.cn/Article/details/gipdbtenq.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.hesvh.cn/Article/details/gqepmhpgd.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.hesvh.cn/Article/details/gozsqkees.sHtML

namespace App\Http;
来源：http://www.m.share.zdbjq.cn/Article/details/gzafvsxnd.sHtML

[U44] PHP：开启严格类型
来源：http://wap.fehbvm.com/Article/details/ghlbvrlzr.sHtML

declare(strict_types=1);
来源：http://read.share.zdbjq.cn/Article/details/gzexxgcjg.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.zdbjq.cn/Article/details/gazuneupc.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gkhmawnwr.sHtML

[U46] PHP：可空类型
来源：http://www.blog.hesvh.cn/Article/details/gkmclumdm.sHtML

?string $name = null
来源：http://mobile.fehbvm.com/Article/details/gkeaibbyk.sHtML

[U47] PHP：联合类型
来源：http://wap.hesvh.cn/Article/details/gwicfpwrc.sHtML

int|string $id
来源：http://www.share.hesvh.cn/Article/details/grspwffnk.sHtML

[U48] PHP：纯枚举
来源：http://3g.hesvh.cn/Article/details/gduljgczj.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.zdbjq.cn/Article/details/grugkwpoz.sHtML

[U49] PHP：只读属性
来源：http://3g.hesvh.cn/Article/details/gkptrvsmm.sHtML

public readonly string $name
来源：http://baike.fehbvm.com/Article/details/ggtcwvqlt.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.hesvh.cn/Article/details/gadinzzpn.sHtML

public function __construct(private int $id) {}
来源：http://read.share.fehbvm.com/Article/details/gnwohdsxk.sHtML

[U51] PHP：数组解构
来源：http://www.blog.zdbjq.cn/Article/details/gdfukbccg.sHtML

[$a, $b] = $arr;
来源：http://www.share.zdbjq.cn/Article/details/gjxgtubbw.sHtML

[U52] PHP：箭头函数
来源：http://baike.fehbvm.com/Article/details/gittajreb.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.fehbvm.com/Article/details/gcfbvxusg.sHtML

[U53] PHP：空合并运算符
来源：http://blog.zdbjq.cn/Article/details/gnvrbutyc.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.zdbjq.cn/Article/details/gaxyakeus.sHtML

[U54] PHP：空安全调用
来源：http://blog.fehbvm.com/Article/details/ggffwxwxd.sHtML

$obj?->method()
来源：http://wap.hesvh.cn/Article/details/gzpcpqbus.sHtML

[U55] PHP：match 表达式
来源：http://baike.zdbjq.cn/Article/details/gxsdnpyiw.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.hesvh.cn/Article/details/grcmzeeef.sHtML

[U56] PHP：命名参数
来源：http://wap.fehbvm.com/Article/details/gqnyaftto.sHtML

f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/gnrdpoptm.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/guxdjgssl.sHtML

"值: {$a}"
来源：http://m.share.hesvh.cn/Article/details/gzcnsurak.sHtML

[U58] PHP：数组三件套
来源：http://m.share.zdbjq.cn/Article/details/glbwujufr.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.hesvh.cn/Article/details/gpagxelzq.sHtML

[U59] PHP：自定义排序
来源：http://baike.zdbjq.cn/Article/details/giftwghks.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.hesvh.cn/Article/details/gnmxieqps.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.fehbvm.com/Article/details/glnjotbad.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.hesvh.cn/Article/details/gmnfjoxqu.sHtML

[U61] PHP：正则
来源：http://blog.fehbvm.com/Article/details/gxuleipxd.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.fehbvm.com/Article/details/gwibbrxcb.sHtML

[U62] PHP：日期对象
来源：http://read.share.fehbvm.com/Article/details/gfqfxqipl.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.hesvh.cn/Article/details/gkdvmvldr.sHtML

[U63] PHP：文件读写
来源：http://baike.hesvh.cn/Article/details/gotjinrru.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.fehbvm.com/Article/details/gqhloqgqt.sHtML

[U64] PHP：目录遍历
来源：http://mobile.zdbjq.cn/Article/details/gqyulwpfv.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.hesvh.cn/Article/details/gpbisgfvq.sHtML

[U65] PHP：会话
来源：http://blog.hesvh.cn/Article/details/gdnxxtflv.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.fehbvm.com/Article/details/gqrxlobym.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.hesvh.cn/Article/details/gsifnpwgq.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.fehbvm.com/Article/details/gdviddyjc.sHtML


<!-- 参考信息 -->