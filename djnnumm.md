代发 wailian999

[S41] C++：类与构造函数
来源：http://www.blog.fehbvm.com/Article/details/gwgpdmnuj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.hesvh.cn/Article/details/geeljltmp.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.hesvh.cn/Article/details/gqipgrxzv.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.zdbjq.cn/Article/details/gihodemml.sHtML

[S43] C++：智能指针
来源：http://mobile.hesvh.cn/Article/details/gqllwdxal.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fehbvm.com/Article/details/gumpghrdo.sHtML

[S44] C++：引用传参
来源：http://www.share.fehbvm.com/Article/details/gbumnwirw.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.hesvh.cn/Article/details/gxfumizlk.sHtML

[S45] C++：lambda
来源：http://m.share.zdbjq.cn/Article/details/gcewgznkj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fehbvm.com/Article/details/gadvefibv.sHtML

[S46] C++：函数模板
来源：http://baike.fehbvm.com/Article/details/gvvcslqqg.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.hesvh.cn/Article/details/gavueecgz.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fehbvm.com/Article/details/gtmwrsopb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.hesvh.cn/Article/details/gmccnfzyd.sHtML

[S48] C++：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gbasjjvvs.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.hesvh.cn/Article/details/gsutgktmb.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.zdbjq.cn/Article/details/gychvqtdi.sHtML

[S49] C++：写文件
来源：http://baike.fehbvm.com/Article/details/ggnfuujme.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fehbvm.com/Article/details/gddnabswz.sHtML

[S50] C++：格式化数字
来源：http://m.share.zdbjq.cn/Article/details/garsvlmiw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/grwobshze.sHtML

[S51] C++：显式类型转换
来源：http://wap.hesvh.cn/Article/details/gkcwagvav.sHtML

static_cast<double>(a) / b
来源：http://read.share.zdbjq.cn/Article/details/gegnvexzm.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.hesvh.cn/Article/details/gxilyaquv.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fehbvm.com/Article/details/gslevjmjd.sHtML

[S53] C++：移动语义
来源：http://m.share.fehbvm.com/Article/details/gpyemwrvp.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.zdbjq.cn/Article/details/gxirghdhs.sHtML

[S54] C++：异常处理
来源：http://read.share.fehbvm.com/Article/details/gfgbdxggj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.zdbjq.cn/Article/details/gqufypnax.sHtML

[S55] C++：结构化绑定
来源：http://wap.fehbvm.com/Article/details/gbiekknyn.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.hesvh.cn/Article/details/gvnhdsgje.sHtML

[S56] C++：optional
来源：http://blog.fehbvm.com/Article/details/gnxtjbmgi.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.hesvh.cn/Article/details/gdefgktra.sHtML

[S57] C++：编译期常量
来源：http://m.share.hesvh.cn/Article/details/gqseienix.sHtML

constexpr int N = 10;
来源：http://blog.zdbjq.cn/Article/details/gramqbwvd.sHtML

[S58] C++：命名空间
来源：http://www.blog.fehbvm.com/Article/details/gmndqkten.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.fehbvm.com/Article/details/gispbxtai.sHtML

[S59] C++：静态断言
来源：http://baike.zdbjq.cn/Article/details/gneqcmbpj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.hesvh.cn/Article/details/gvfapretw.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.zdbjq.cn/Article/details/gexhgaopt.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fehbvm.com/Article/details/gbzfuvyew.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gmcdxnnsd.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fehbvm.com/Article/details/gtwpzlkda.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gcbubmlrl.sHtML

[T01] Kotlin：Hello World
来源：http://3g.zdbjq.cn/Article/details/ggnpzgfvh.sHtML

println("Hello")
来源：http://www.blog.fehbvm.com/Article/details/girrtmuvx.sHtML

[T02] Kotlin：变量
来源：http://www.share.zdbjq.cn/Article/details/gbckacsls.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.hesvh.cn/Article/details/gzamlcbrm.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.hesvh.cn/Article/details/gxejnvmmb.sHtML

"值: $b"
来源：http://baike.fehbvm.com/Article/details/gaklhtark.sHtML

[T04] Kotlin：空安全
来源：http://wap.fehbvm.com/Article/details/gmgdmgrcn.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fehbvm.com/Article/details/gymafhvfx.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.hesvh.cn/Article/details/gsfdbbjzo.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.hesvh.cn/Article/details/gclmscmbk.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fehbvm.com/Article/details/guqnyubii.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fehbvm.com/Article/details/gtgvahhws.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/gkehemnfw.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fehbvm.com/Article/details/gdmzlsyvk.sHtML

[T08] Kotlin：数据类
来源：http://3g.zdbjq.cn/Article/details/gcusgtkms.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.hesvh.cn/Article/details/gyfgnajya.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.hesvh.cn/Article/details/goyxmzfuo.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.hesvh.cn/Article/details/gametjarc.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fehbvm.com/Article/details/gqmwebxjh.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fehbvm.com/Article/details/gepvbqwgq.sHtML

[T11] Kotlin：协程
来源：http://mobile.zdbjq.cn/Article/details/gbplcnslu.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.hesvh.cn/Article/details/gnufveqvl.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.hesvh.cn/Article/details/ghkvptbjv.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.hesvh.cn/Article/details/grbnbwlsk.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.hesvh.cn/Article/details/gxsnvmbhj.sHtML

val m = mapOf("a" to 1)
来源：http://3g.zdbjq.cn/Article/details/gcdccsodb.sHtML

[T14] Kotlin：循环
来源：http://wap.zdbjq.cn/Article/details/gitmcpjfk.sHtML

for (i in 1..10) println(i)
来源：http://blog.zdbjq.cn/Article/details/gtfqthwje.sHtML

[T15] Kotlin：接口
来源：http://blog.fehbvm.com/Article/details/grabsbfmv.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.zdbjq.cn/Article/details/gicwrwthc.sHtML

[T16] Swift：Hello World
来源：http://www.share.zdbjq.cn/Article/details/giyzpknqp.sHtML

print("Hello")
来源：http://wap.hesvh.cn/Article/details/gvqjqzjvd.sHtML

[T17] Swift：变量与常量
来源：http://baike.zdbjq.cn/Article/details/grjfvqgaw.sHtML

var a = 1;  let b = 2
来源：http://baike.hesvh.cn/Article/details/gxtnqhczb.sHtML

[T18] Swift：字符串插值
来源：http://baike.fehbvm.com/Article/details/gkbghhsdd.sHtML

"值: \(b)"
来源：http://read.share.zdbjq.cn/Article/details/ggcmmwiwj.sHtML

[T19] Swift：可选绑定
来源：http://mobile.zdbjq.cn/Article/details/gzqtatpmh.sHtML

if let n = opt { print(n) }
来源：http://www.blog.hesvh.cn/Article/details/gxwiaodpa.sHtML

[T20] Swift：数组操作
来源：http://www.share.zdbjq.cn/Article/details/grmvmmnjx.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fehbvm.com/Article/details/gievdmhdo.sHtML

[T21] Swift：遍历
来源：http://blog.hesvh.cn/Article/details/grnnmjsxf.sHtML

for x in a { print(x) }
来源：http://mobile.fehbvm.com/Article/details/gojmfloeq.sHtML

[T22] Swift：字典
来源：http://blog.zdbjq.cn/Article/details/godlaspja.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.zdbjq.cn/Article/details/gafojimpj.sHtML

[T23] Swift：函数
来源：http://blog.hesvh.cn/Article/details/gfagwfvxe.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.fehbvm.com/Article/details/gtrwwanlu.sHtML

[T24] Swift：闭包
来源：http://wap.hesvh.cn/Article/details/gxwenovhm.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.hesvh.cn/Article/details/gawemekic.sHtML

[T25] Swift：结构体
来源：http://mobile.fehbvm.com/Article/details/gridguczn.sHtML

struct P { var x: Int }
来源：http://www.m.share.zdbjq.cn/Article/details/gjdpvjqip.sHtML

[T26] Swift：类与重写
来源：http://www.share.hesvh.cn/Article/details/gavnudyur.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fehbvm.com/Article/details/griuumjzg.sHtML

[T27] Swift：错误处理
来源：http://wap.zdbjq.cn/Article/details/gpwvbhkvb.sHtML

do { try f() } catch { print(error) }
来源：http://3g.hesvh.cn/Article/details/gctgubydm.sHtML

[T28] Swift：枚举
来源：http://www.blog.zdbjq.cn/Article/details/gytliygsl.sHtML

enum Color { case red, green }
来源：http://www.blog.hesvh.cn/Article/details/gpxdakdph.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.hesvh.cn/Article/details/gknvlqrbl.sHtML

guard let x = opt else { return }
来源：http://wap.fehbvm.com/Article/details/gpxjcpfyq.sHtML

[T30] Swift：协议
来源：http://www.blog.hesvh.cn/Article/details/gtlrktopi.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fehbvm.com/Article/details/gwtsfnuhy.sHtML

[T31] Lua：Hello World
来源：http://www.share.zdbjq.cn/Article/details/ggedyfdub.sHtML

print("Hello")
来源：http://read.share.fehbvm.com/Article/details/gnhknjxxf.sHtML

[T32] Lua：局部变量
来源：http://www.share.zdbjq.cn/Article/details/gkgvqbfol.sHtML

local a = 1
来源：http://3g.hesvh.cn/Article/details/gdwbnczve.sHtML

[T33] Lua：表（数组）
来源：http://wap.fehbvm.com/Article/details/gvssabuki.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.hesvh.cn/Article/details/gjoytuern.sHtML

[T34] Lua：遍历表
来源：http://blog.hesvh.cn/Article/details/gkcmtrrrs.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.zdbjq.cn/Article/details/gttpulqdn.sHtML

[T35] Lua：字典表
来源：http://baike.hesvh.cn/Article/details/goqjfgmqg.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fehbvm.com/Article/details/gcwqjuwtt.sHtML

[T36] Lua：函数
来源：http://www.blog.hesvh.cn/Article/details/gkmzjiymv.sHtML

function add(a, b) return a + b end
来源：http://m.share.hesvh.cn/Article/details/gbmavtias.sHtML

[T37] Lua：字符串拼接
来源：http://baike.fehbvm.com/Article/details/gpmrqzqsm.sHtML

"a" .. "b"
来源：http://www.m.share.zdbjq.cn/Article/details/ggctxfnzu.sHtML

[T38] Lua：条件
来源：http://read.share.hesvh.cn/Article/details/gpkwmgkar.sHtML

if x > 0 then print("正") end
来源：http://m.share.zdbjq.cn/Article/details/gmsyfspeq.sHtML

[T39] Lua：模式匹配
来源：http://read.share.hesvh.cn/Article/details/grbxwalad.sHtML

string.find(s, "%d+")
来源：http://read.share.hesvh.cn/Article/details/gyybhfssp.sHtML

[T40] Lua：元表
来源：http://www.m.share.hesvh.cn/Article/details/gxvfbeoah.sHtML

setmetatable({}, { __index = base })
来源：http://blog.zdbjq.cn/Article/details/gnzjrjeid.sHtML

[T41] Perl：Hello World
来源：http://wap.hesvh.cn/Article/details/gwjxcfclg.sHtML

print "Hello\n";
来源：http://baike.hesvh.cn/Article/details/gkiqzzqcr.sHtML

[T42] Perl：变量类型
来源：http://m.share.hesvh.cn/Article/details/gijvelldw.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.hesvh.cn/Article/details/gkmxuulwy.sHtML

[T43] Perl：字符串插值
来源：http://baike.hesvh.cn/Article/details/ggxwoyymp.sHtML

"值: $a"
来源：http://www.m.share.zdbjq.cn/Article/details/gciylfmok.sHtML

[T44] Perl：条件
来源：http://www.share.fehbvm.com/Article/details/gvxqnrzkp.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.fehbvm.com/Article/details/gozdwbdvk.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.hesvh.cn/Article/details/gyxxjkfgj.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.zdbjq.cn/Article/details/ggzynlicv.sHtML

[T46] Perl：哈希操作
来源：http://read.share.zdbjq.cn/Article/details/gpvuichlu.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.zdbjq.cn/Article/details/gvqqqvmkj.sHtML

[T47] Perl：正则捕获
来源：http://m.share.hesvh.cn/Article/details/ggvhugsmb.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.fehbvm.com/Article/details/gnltnxxrl.sHtML

[T48] Perl：正则替换
来源：http://3g.hesvh.cn/Article/details/gozthsppx.sHtML

$s =~ s/old/new/g;
来源：http://wap.fehbvm.com/Article/details/gmsilwjfw.sHtML

[T49] Perl：函数
来源：http://mobile.fehbvm.com/Article/details/gygvkypxl.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gcpnuqxnm.sHtML

[T50] Perl：逐行读文件
来源：http://baike.hesvh.cn/Article/details/geiyhsdhr.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.zdbjq.cn/Article/details/gqzpfictr.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.hesvh.cn/Article/details/gtzfmyghc.sHtML

[T51] Scala：Hello World
来源：http://wap.fehbvm.com/Article/details/gucpufcpp.sHtML

println("Hello")
来源：http://wap.hesvh.cn/Article/details/giwwqthnd.sHtML

[T52] Scala：变量
来源：http://blog.fehbvm.com/Article/details/gxxsfcmhd.sHtML

val a = 1;  var b = 2
来源：http://wap.hesvh.cn/Article/details/gyloqoxfp.sHtML

[T53] Scala：字符串插值
来源：http://3g.fehbvm.com/Article/details/gkzvcwclj.sHtML

s"值: $b"
来源：http://m.share.zdbjq.cn/Article/details/giwfztzlz.sHtML

[T54] Scala：集合映射
来源：http://3g.hesvh.cn/Article/details/gucfdqnmm.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.zdbjq.cn/Article/details/gtgpwkpgj.sHtML

[T55] Scala：集合过滤
来源：http://wap.fehbvm.com/Article/details/gamqggwtd.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.zdbjq.cn/Article/details/gqxndyueb.sHtML

[T56] Scala：样例类
来源：http://m.share.fehbvm.com/Article/details/gwjfygpgj.sHtML

case class User(name: String, age: Int)
来源：http://baike.fehbvm.com/Article/details/gguadxlxz.sHtML

[T57] Scala：模式匹配
来源：http://m.share.hesvh.cn/Article/details/gszyenlxi.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.fehbvm.com/Article/details/gozygcqui.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.zdbjq.cn/Article/details/gjnpgeelq.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.fehbvm.com/Article/details/gojfbgfbm.sHtML

[T59] Scala：循环
来源：http://m.share.hesvh.cn/Article/details/gamfyhcud.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.hesvh.cn/Article/details/gjrxmehju.sHtML

[T60] Scala：折叠
来源：http://wap.zdbjq.cn/Article/details/gahxvmsof.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.zdbjq.cn/Article/details/gzkgaefel.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gawtehbvn.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.zdbjq.cn/Article/details/gpzjgaemp.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gclsnobnl.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.fehbvm.com/Article/details/gfmnhskzn.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.fehbvm.com/Article/details/godkkjmqk.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.hesvh.cn/Article/details/gustqwfna.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.zdbjq.cn/Article/details/glijyzmkf.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.fehbvm.com/Article/details/gwkltvqnr.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.fehbvm.com/Article/details/gtnzkznqs.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.fehbvm.com/Article/details/gyndofewp.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.fehbvm.com/Article/details/gcuznwuqz.sHtML

[U05] Py：列表去重且保序
来源：http://baike.zdbjq.cn/Article/details/ggpxnluxm.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gcvjlogqq.sHtML

[U06] Py：合并两个字典
来源：http://mobile.hesvh.cn/Article/details/gctqowufx.sHtML

{**a, **b}
来源：http://wap.hesvh.cn/Article/details/grmnvxuka.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.zdbjq.cn/Article/details/ghpjhmcpp.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.hesvh.cn/Article/details/gzwxhzybw.sHtML

[U08] Py：展平二维列表
来源：http://wap.fehbvm.com/Article/details/gesaeluot.sHtML

[y for x in nested for y in x]
来源：http://read.share.hesvh.cn/Article/details/gfxmjspdg.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.hesvh.cn/Article/details/gvsieypdp.sHtML

max(d, key=d.get)
来源：http://www.share.hesvh.cn/Article/details/gvnqgsybl.sHtML

[U10] Py：按值排序字典
来源：http://mobile.fehbvm.com/Article/details/gchotkdoj.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.hesvh.cn/Article/details/gqpqwfjpz.sHtML

[U11] Py：生成器表达式
来源：http://read.share.zdbjq.cn/Article/details/gkpapyryg.sHtML

(x * 2 for x in arr)
来源：http://wap.hesvh.cn/Article/details/grhiqvjta.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.zdbjq.cn/Article/details/griaxzika.sHtML

Counter(arr).most_common(3)
来源：http://wap.zdbjq.cn/Article/details/gslsilmjg.sHtML

[U13] Py：固定长度队列
来源：http://baike.zdbjq.cn/Article/details/grvfkyjte.sHtML

deque(maxlen=10)
来源：http://baike.zdbjq.cn/Article/details/gsleyckxp.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.hesvh.cn/Article/details/gmhodfftb.sHtML

defaultdict(list)
来源：http://baike.hesvh.cn/Article/details/gagzhwkgv.sHtML

[U15] Py：高精度计时
来源：http://read.share.fehbvm.com/Article/details/gkdmranhd.sHtML

t = time.perf_counter()
来源：http://blog.zdbjq.cn/Article/details/grapurnjq.sHtML

[U16] Py：命令行参数解析
来源：http://3g.zdbjq.cn/Article/details/gvowrzdwb.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.zdbjq.cn/Article/details/gmjxuacxk.sHtML

[U17] Py：初始化日志
来源：http://blog.hesvh.cn/Article/details/gdkhduqfy.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.hesvh.cn/Article/details/grqcyyobt.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.hesvh.cn/Article/details/gsebcpphk.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.fehbvm.com/Article/details/gcvygjatt.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.hesvh.cn/Article/details/gnhvigmie.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.fehbvm.com/Article/details/glishddrq.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.hesvh.cn/Article/details/gdnsiixhi.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.hesvh.cn/Article/details/gdkbjyhfg.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.hesvh.cn/Article/details/gclewcmlp.sHtML

@contextlib.contextmanager
来源：http://www.blog.hesvh.cn/Article/details/ghtcwncyu.sHtML

[U22] Py：矩阵转置
来源：http://blog.fehbvm.com/Article/details/gtnwgezep.sHtML

list(zip(*m))
来源：http://3g.fehbvm.com/Article/details/gtgtdrqdo.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.fehbvm.com/Article/details/gympnjnsy.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.zdbjq.cn/Article/details/gbtorllxs.sHtML

[U24] Py：路径操作
来源：http://wap.zdbjq.cn/Article/details/ghsccflhy.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.fehbvm.com/Article/details/gowpwjkxp.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.zdbjq.cn/Article/details/gminlneox.sHtML

csv.DictReader(f)
来源：http://blog.hesvh.cn/Article/details/gcfbfrglc.sHtML

[U26] Py：并发下载
来源：http://blog.hesvh.cn/Article/details/gedlxnbys.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.fehbvm.com/Article/details/gwogfedmf.sHtML

[U27] Py：异步 HTTP
来源：http://baike.hesvh.cn/Article/details/gueghpecl.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.zdbjq.cn/Article/details/goptbqica.sHtML

[U28] Py：类型别名
来源：http://blog.zdbjq.cn/Article/details/ggclpnjhe.sHtML

UserId = int
来源：http://www.blog.hesvh.cn/Article/details/gxxdbkblj.sHtML

[U29] Py：属性校验
来源：http://wap.zdbjq.cn/Article/details/gdkwlssgc.sHtML

@property 与 @x.setter 配合
来源：http://m.share.hesvh.cn/Article/details/gqvnqvyxp.sHtML

[U30] Py：数据类
来源：http://read.share.zdbjq.cn/Article/details/gbbclniqk.sHtML

@dataclass(slots=True)
来源：http://wap.fehbvm.com/Article/details/ghodnlwbp.sHtML

[U31] Py：单测
来源：http://baike.fehbvm.com/Article/details/gukelelrm.sHtML

python -m pytest -q
来源：http://www.blog.hesvh.cn/Article/details/gsijkorhg.sHtML

[U32] Py：代码格式化
来源：http://m.share.fehbvm.com/Article/details/guwfdkenl.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.zdbjq.cn/Article/details/gvmdwaysc.sHtML

[U33] Py：打包发布
来源：http://read.share.hesvh.cn/Article/details/gaahnxtkh.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.zdbjq.cn/Article/details/gjnbrgwtg.sHtML

[U34] Py：判断编码
来源：http://mobile.hesvh.cn/Article/details/gdrypftla.sHtML

chardet.detect(raw)
来源：http://3g.fehbvm.com/Article/details/gkcpwtbyo.sHtML

[U35] Py：发送邮件
来源：http://mobile.fehbvm.com/Article/details/gdplufghs.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.hesvh.cn/Article/details/glxbgqwjv.sHtML

[U36] Py：定时任务
来源：http://www.share.zdbjq.cn/Article/details/gzneqozhg.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.fehbvm.com/Article/details/gifyvofnl.sHtML

[U37] Py：读写 Excel
来源：http://3g.fehbvm.com/Article/details/gxbjtyfxv.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.zdbjq.cn/Article/details/gqlqzhemc.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fehbvm.com/Article/details/gvguucbse.sHtML

Path(__file__).resolve().parent
来源：http://mobile.zdbjq.cn/Article/details/gmpathvhn.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.zdbjq.cn/Article/details/gcgkhpjcf.sHtML

sys.stdout.isatty()
来源：http://baike.fehbvm.com/Article/details/gvreajyfc.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.zdbjq.cn/Article/details/gyydzliuh.sHtML

print("err", file=sys.stderr)
来源：http://baike.zdbjq.cn/Article/details/gysjatbbb.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.zdbjq.cn/Article/details/gxlzlrogt.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.fehbvm.com/Article/details/gjqeqtucp.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.zdbjq.cn/Article/details/grctdxdlv.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.hesvh.cn/Article/details/gqpypkgkr.sHtML

[U43] PHP：声明命名空间
来源：http://wap.hesvh.cn/Article/details/gxsufylck.sHtML

namespace App\Http;
来源：http://www.blog.hesvh.cn/Article/details/gdisnmifa.sHtML

[U44] PHP：开启严格类型
来源：http://3g.fehbvm.com/Article/details/gootjlvks.sHtML

declare(strict_types=1);
来源：http://m.share.zdbjq.cn/Article/details/givuwctdc.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.hesvh.cn/Article/details/gtfzhfnzb.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gpavgzgot.sHtML

[U46] PHP：可空类型
来源：http://blog.zdbjq.cn/Article/details/gefspanql.sHtML

?string $name = null
来源：http://www.m.share.zdbjq.cn/Article/details/gydbvebkj.sHtML

[U47] PHP：联合类型
来源：http://m.share.fehbvm.com/Article/details/gruhhuuxm.sHtML

int|string $id
来源：http://mobile.fehbvm.com/Article/details/gbcjrusla.sHtML

[U48] PHP：纯枚举
来源：http://blog.hesvh.cn/Article/details/guwbysqns.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.hesvh.cn/Article/details/gxrtdxvfo.sHtML

[U49] PHP：只读属性
来源：http://wap.hesvh.cn/Article/details/gtxvyvnwt.sHtML

public readonly string $name
来源：http://m.share.hesvh.cn/Article/details/gsljuadty.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.hesvh.cn/Article/details/geenfbkci.sHtML

public function __construct(private int $id) {}
来源：http://mobile.hesvh.cn/Article/details/ggccqorjv.sHtML

[U51] PHP：数组解构
来源：http://wap.fehbvm.com/Article/details/ghcroyzdu.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.zdbjq.cn/Article/details/gmlqxrudm.sHtML

[U52] PHP：箭头函数
来源：http://wap.zdbjq.cn/Article/details/gqrvtqsbd.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.hesvh.cn/Article/details/gwkqnyfes.sHtML

[U53] PHP：空合并运算符
来源：http://3g.zdbjq.cn/Article/details/gpkbrflri.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.zdbjq.cn/Article/details/gpiorcvyw.sHtML

[U54] PHP：空安全调用
来源：http://mobile.fehbvm.com/Article/details/gagsvfqaz.sHtML

$obj?->method()
来源：http://3g.zdbjq.cn/Article/details/ghrqjskoq.sHtML

[U55] PHP：match 表达式
来源：http://baike.hesvh.cn/Article/details/gcxvcqcpo.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.hesvh.cn/Article/details/gnmuttdfl.sHtML

[U56] PHP：命名参数
来源：http://blog.zdbjq.cn/Article/details/gjwqxhnqn.sHtML

f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/gxbinvbxn.sHtML

[U57] PHP：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gmhskdccy.sHtML

"值: {$a}"
来源：http://www.blog.fehbvm.com/Article/details/glszhwyxm.sHtML

[U58] PHP：数组三件套
来源：http://www.share.hesvh.cn/Article/details/gxfrrqewl.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.fehbvm.com/Article/details/gxgxsctqx.sHtML

[U59] PHP：自定义排序
来源：http://mobile.hesvh.cn/Article/details/gmistsoap.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.hesvh.cn/Article/details/geudbfxqd.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.zdbjq.cn/Article/details/glsbjjope.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.zdbjq.cn/Article/details/gguekmngv.sHtML

[U61] PHP：正则
来源：http://read.share.hesvh.cn/Article/details/gnokowhvw.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.zdbjq.cn/Article/details/gkzriiwhx.sHtML

[U62] PHP：日期对象
来源：http://read.share.hesvh.cn/Article/details/gcplhvdwa.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.hesvh.cn/Article/details/grnttnxwx.sHtML

[U63] PHP：文件读写
来源：http://3g.fehbvm.com/Article/details/gswhduifj.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.zdbjq.cn/Article/details/gjepolsxp.sHtML

[U64] PHP：目录遍历
来源：http://wap.fehbvm.com/Article/details/glyktnbzg.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.hesvh.cn/Article/details/gqwqyfshv.sHtML

[U65] PHP：会话
来源：http://www.m.share.hesvh.cn/Article/details/gkyzuocka.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.zdbjq.cn/Article/details/ggdaspiip.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.zdbjq.cn/Article/details/gsewrlhfz.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.hesvh.cn/Article/details/gokyunyrc.sHtML


<!-- 参考信息 -->