代发 wailian999

[S39] C++：自定义比较器排序
来源：http://www.m.share.zdbjq.cn/Article/details/gweywcgel.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.zdbjq.cn/Article/details/gflfmabvj.sHtML

[S40] C++：查找元素
来源：http://3g.zdbjq.cn/Article/details/girfygfit.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.zdbjq.cn/Article/details/gkdsavigh.sHtML

[S41] C++：类与构造函数
来源：http://read.share.hesvh.cn/Article/details/gufyritvx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.zdbjq.cn/Article/details/glngxrwok.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.hesvh.cn/Article/details/gozjqqddy.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.zdbjq.cn/Article/details/gpdxvnxkl.sHtML

[S43] C++：智能指针
来源：http://blog.zdbjq.cn/Article/details/gnzlfspfb.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.zdbjq.cn/Article/details/gtiorsdjo.sHtML

[S44] C++：引用传参
来源：http://3g.fehbvm.com/Article/details/gebaoftmb.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fehbvm.com/Article/details/gfbumteir.sHtML

[S45] C++：lambda
来源：http://www.m.share.zdbjq.cn/Article/details/gwkrjuaoz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fehbvm.com/Article/details/gyikirzpk.sHtML

[S46] C++：函数模板
来源：http://mobile.zdbjq.cn/Article/details/gipivhuos.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fehbvm.com/Article/details/gcxlkjupt.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.zdbjq.cn/Article/details/gfllszigi.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.hesvh.cn/Article/details/gtthmrppp.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gaufdmelf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fehbvm.com/Article/details/gadcptriq.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fehbvm.com/Article/details/gszojrbjm.sHtML

[S49] C++：写文件
来源：http://blog.hesvh.cn/Article/details/gzszlwjmj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.zdbjq.cn/Article/details/gevsqsfbo.sHtML

[S50] C++：格式化数字
来源：http://blog.zdbjq.cn/Article/details/gbrchrrnm.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gwgnfkoxw.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/gcacnfxdp.sHtML

static_cast<double>(a) / b
来源：http://read.share.fehbvm.com/Article/details/gjbubijrv.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.zdbjq.cn/Article/details/gdpwjonqz.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fehbvm.com/Article/details/gpmvkqvtj.sHtML

[S53] C++：移动语义
来源：http://3g.fehbvm.com/Article/details/gkfnhtqhp.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.zdbjq.cn/Article/details/gnjjohchs.sHtML

[S54] C++：异常处理
来源：http://wap.zdbjq.cn/Article/details/gwydrthno.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.hesvh.cn/Article/details/gtyhbkmwz.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.hesvh.cn/Article/details/grnzqlnve.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fehbvm.com/Article/details/gzjpxhowq.sHtML

[S56] C++：optional
来源：http://www.m.share.fehbvm.com/Article/details/gvjlpyuvi.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.hesvh.cn/Article/details/gifmfpihq.sHtML

[S57] C++：编译期常量
来源：http://www.share.zdbjq.cn/Article/details/gjcxcxjjh.sHtML

constexpr int N = 10;
来源：http://wap.hesvh.cn/Article/details/gekyjcrdi.sHtML

[S58] C++：命名空间
来源：http://www.share.hesvh.cn/Article/details/gatvftxaj.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.hesvh.cn/Article/details/gcmggecnk.sHtML

[S59] C++：静态断言
来源：http://www.blog.fehbvm.com/Article/details/gitzsukju.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.hesvh.cn/Article/details/gmnybhixn.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.hesvh.cn/Article/details/gxevimpgr.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.zdbjq.cn/Article/details/gmxphfpsg.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gtkhnldwz.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.hesvh.cn/Article/details/gyjefowbw.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/glqcqgqpf.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gqvntxmsm.sHtML

println("Hello")
来源：http://mobile.hesvh.cn/Article/details/goeschlxo.sHtML

[T02] Kotlin：变量
来源：http://3g.fehbvm.com/Article/details/gwdjerylx.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.hesvh.cn/Article/details/gbseygzhv.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fehbvm.com/Article/details/gieyohwqp.sHtML

"值: $b"
来源：http://baike.fehbvm.com/Article/details/gllvbroct.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fehbvm.com/Article/details/gwmxrmjns.sHtML

val n: String? = null;  n?.length
来源：http://wap.zdbjq.cn/Article/details/gtwlqwudr.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.zdbjq.cn/Article/details/gzstfdhyf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fehbvm.com/Article/details/gmwurwuuy.sHtML

[T06] Kotlin：集合映射
来源：http://baike.zdbjq.cn/Article/details/gswueqtoj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.hesvh.cn/Article/details/gxtopqdie.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fehbvm.com/Article/details/grzsbmcty.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/gahhkappl.sHtML

[T08] Kotlin：数据类
来源：http://read.share.zdbjq.cn/Article/details/gcephljjw.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.hesvh.cn/Article/details/gbxjcysup.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.hesvh.cn/Article/details/ghrzauqgz.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fehbvm.com/Article/details/gnfcjqalp.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fehbvm.com/Article/details/gmgpxurcd.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fehbvm.com/Article/details/gboxgicww.sHtML

[T11] Kotlin：协程
来源：http://mobile.fehbvm.com/Article/details/gqihodqsx.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fehbvm.com/Article/details/gbvuweqda.sHtML

[T12] Kotlin：解构声明
来源：http://baike.hesvh.cn/Article/details/gjpyfrgsp.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gholvoufm.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fehbvm.com/Article/details/gjixwwwbc.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.hesvh.cn/Article/details/gycohrvqo.sHtML

[T14] Kotlin：循环
来源：http://3g.fehbvm.com/Article/details/grpaylctj.sHtML

for (i in 1..10) println(i)
来源：http://wap.hesvh.cn/Article/details/gbytawjrx.sHtML

[T15] Kotlin：接口
来源：http://blog.fehbvm.com/Article/details/gqrouqaoq.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.zdbjq.cn/Article/details/gkxyhyulx.sHtML

[T16] Swift：Hello World
来源：http://3g.fehbvm.com/Article/details/gedjjjyvz.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/ggzejrnfd.sHtML

[T17] Swift：变量与常量
来源：http://blog.zdbjq.cn/Article/details/gyeolfvhs.sHtML

var a = 1;  let b = 2
来源：http://www.blog.fehbvm.com/Article/details/gagulranz.sHtML

[T18] Swift：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gvokynzvx.sHtML

"值: \(b)"
来源：http://3g.hesvh.cn/Article/details/gtgdtylcw.sHtML

[T19] Swift：可选绑定
来源：http://read.share.zdbjq.cn/Article/details/gcfbtorrj.sHtML

if let n = opt { print(n) }
来源：http://read.share.hesvh.cn/Article/details/gwvzzvwcl.sHtML

[T20] Swift：数组操作
来源：http://www.blog.zdbjq.cn/Article/details/gjutaiwsi.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.hesvh.cn/Article/details/geojvsxwr.sHtML

[T21] Swift：遍历
来源：http://read.share.zdbjq.cn/Article/details/geeczwdtu.sHtML

for x in a { print(x) }
来源：http://m.share.fehbvm.com/Article/details/gyjkuzcio.sHtML

[T22] Swift：字典
来源：http://mobile.fehbvm.com/Article/details/gvfzglecg.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.hesvh.cn/Article/details/glgtgukhf.sHtML

[T23] Swift：函数
来源：http://mobile.zdbjq.cn/Article/details/gmlazclyl.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fehbvm.com/Article/details/gnabgrefp.sHtML

[T24] Swift：闭包
来源：http://www.blog.hesvh.cn/Article/details/glibvdwql.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fehbvm.com/Article/details/gwilnqyhr.sHtML

[T25] Swift：结构体
来源：http://m.share.fehbvm.com/Article/details/gowvnxpfr.sHtML

struct P { var x: Int }
来源：http://m.share.hesvh.cn/Article/details/gfkvxhyxy.sHtML

[T26] Swift：类与重写
来源：http://baike.hesvh.cn/Article/details/gfzugchdp.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fehbvm.com/Article/details/gpxpzwiqk.sHtML

[T27] Swift：错误处理
来源：http://baike.hesvh.cn/Article/details/gjlhfjssr.sHtML

do { try f() } catch { print(error) }
来源：http://wap.zdbjq.cn/Article/details/gvklypfdq.sHtML

[T28] Swift：枚举
来源：http://3g.hesvh.cn/Article/details/glasbjzgy.sHtML

enum Color { case red, green }
来源：http://read.share.hesvh.cn/Article/details/gnaqffjfa.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.fehbvm.com/Article/details/gjykyyywi.sHtML

guard let x = opt else { return }
来源：http://blog.fehbvm.com/Article/details/galxzdaur.sHtML

[T30] Swift：协议
来源：http://blog.hesvh.cn/Article/details/gwcgbybmd.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.hesvh.cn/Article/details/gkmqzquxd.sHtML

[T31] Lua：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gpqhmhefk.sHtML

print("Hello")
来源：http://blog.zdbjq.cn/Article/details/gjdargyhc.sHtML

[T32] Lua：局部变量
来源：http://wap.hesvh.cn/Article/details/geyresucm.sHtML

local a = 1
来源：http://www.m.share.fehbvm.com/Article/details/gilvebunn.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.zdbjq.cn/Article/details/ghvzcumrg.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.zdbjq.cn/Article/details/guamolgny.sHtML

[T34] Lua：遍历表
来源：http://3g.zdbjq.cn/Article/details/gtcimdcvc.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.hesvh.cn/Article/details/gkicqfldt.sHtML

[T35] Lua：字典表
来源：http://m.share.zdbjq.cn/Article/details/gvzmaibjw.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fehbvm.com/Article/details/gnilctnar.sHtML

[T36] Lua：函数
来源：http://baike.hesvh.cn/Article/details/glogwsnfn.sHtML

function add(a, b) return a + b end
来源：http://3g.hesvh.cn/Article/details/gcackbtqz.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.hesvh.cn/Article/details/gdopngccb.sHtML

"a" .. "b"
来源：http://mobile.hesvh.cn/Article/details/gjhtsulwb.sHtML

[T38] Lua：条件
来源：http://mobile.zdbjq.cn/Article/details/gnnijptne.sHtML

if x > 0 then print("正") end
来源：http://wap.zdbjq.cn/Article/details/gljgpbvsl.sHtML

[T39] Lua：模式匹配
来源：http://wap.hesvh.cn/Article/details/gvqtippjn.sHtML

string.find(s, "%d+")
来源：http://www.m.share.fehbvm.com/Article/details/gngqfyzxf.sHtML

[T40] Lua：元表
来源：http://mobile.zdbjq.cn/Article/details/gwzqamghi.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fehbvm.com/Article/details/gxyvroxhc.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gdycysxoo.sHtML

print "Hello\n";
来源：http://3g.hesvh.cn/Article/details/gassgyrvz.sHtML

[T42] Perl：变量类型
来源：http://mobile.hesvh.cn/Article/details/gsfmbesmw.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.zdbjq.cn/Article/details/gfmltzsfo.sHtML

[T43] Perl：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gosepwjoj.sHtML

"值: $a"
来源：http://baike.hesvh.cn/Article/details/gorlkievz.sHtML

[T44] Perl：条件
来源：http://3g.zdbjq.cn/Article/details/gwoanadrv.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.zdbjq.cn/Article/details/giwpmbkjc.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.hesvh.cn/Article/details/gturlsihp.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.zdbjq.cn/Article/details/ggmzwymjv.sHtML

[T46] Perl：哈希操作
来源：http://wap.zdbjq.cn/Article/details/grlirarfe.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.fehbvm.com/Article/details/gsqmgypyy.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.zdbjq.cn/Article/details/gdpcjyjcn.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fehbvm.com/Article/details/gsuzlthtt.sHtML

[T48] Perl：正则替换
来源：http://www.blog.hesvh.cn/Article/details/gphtpsqdi.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.fehbvm.com/Article/details/gmnmbwxky.sHtML

[T49] Perl：函数
来源：http://m.share.fehbvm.com/Article/details/gfyyruqwm.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gytvcmieq.sHtML

[T50] Perl：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gskkkonie.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.fehbvm.com/Article/details/gnzxszvnx.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvqbjeluu.sHtML

[T51] Scala：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gajnfsuod.sHtML

println("Hello")
来源：http://read.share.zdbjq.cn/Article/details/glijnexkj.sHtML

[T52] Scala：变量
来源：http://www.m.share.zdbjq.cn/Article/details/gehigriip.sHtML

val a = 1;  var b = 2
来源：http://read.share.fehbvm.com/Article/details/gjnbrykwi.sHtML

[T53] Scala：字符串插值
来源：http://mobile.hesvh.cn/Article/details/ggowvdyca.sHtML

s"值: $b"
来源：http://wap.hesvh.cn/Article/details/gvozpncfd.sHtML

[T54] Scala：集合映射
来源：http://3g.fehbvm.com/Article/details/gfnjbcqng.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.fehbvm.com/Article/details/gvdddsmbk.sHtML

[T55] Scala：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/gjdufuxji.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.fehbvm.com/Article/details/gkrujqtfg.sHtML

[T56] Scala：样例类
来源：http://wap.fehbvm.com/Article/details/gqeyadllr.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.fehbvm.com/Article/details/gtmdaisyh.sHtML

[T57] Scala：模式匹配
来源：http://m.share.fehbvm.com/Article/details/ggcdigfja.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.zdbjq.cn/Article/details/glfuednlb.sHtML

[T58] Scala：函数定义
来源：http://wap.fehbvm.com/Article/details/ggosakqpj.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.zdbjq.cn/Article/details/gsplncsgq.sHtML

[T59] Scala：循环
来源：http://read.share.zdbjq.cn/Article/details/gmfoawgux.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.fehbvm.com/Article/details/gtswvkrmv.sHtML

[T60] Scala：折叠
来源：http://m.share.hesvh.cn/Article/details/ghnzwhsgn.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.zdbjq.cn/Article/details/grompvbuv.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gnmesxuib.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.zdbjq.cn/Article/details/guczcqrbu.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gxaiysaud.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.hesvh.cn/Article/details/geoacpwcf.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.fehbvm.com/Article/details/gjbiubxzs.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.hesvh.cn/Article/details/grmmdoiih.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.zdbjq.cn/Article/details/ggpgjuouj.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.fehbvm.com/Article/details/gzqxkjpzw.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.hesvh.cn/Article/details/gtzjqjmur.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.zdbjq.cn/Article/details/gfcmjfbrz.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.fehbvm.com/Article/details/ghzknzaba.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.hesvh.cn/Article/details/ggcddydky.sHtML

list(dict.fromkeys(arr))
来源：http://blog.hesvh.cn/Article/details/gqcpdcjce.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fehbvm.com/Article/details/gyvmsncch.sHtML

{**a, **b}
来源：http://www.m.share.zdbjq.cn/Article/details/glfhnrawe.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.zdbjq.cn/Article/details/gldacqhkw.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.zdbjq.cn/Article/details/gsnbkwwlv.sHtML

[U08] Py：展平二维列表
来源：http://mobile.zdbjq.cn/Article/details/gprqxmvqc.sHtML

[y for x in nested for y in x]
来源：http://read.share.hesvh.cn/Article/details/gufdrhzhz.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.hesvh.cn/Article/details/gfjezwdhu.sHtML

max(d, key=d.get)
来源：http://baike.hesvh.cn/Article/details/gekbrlyno.sHtML

[U10] Py：按值排序字典
来源：http://read.share.hesvh.cn/Article/details/ghulyvphd.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.fehbvm.com/Article/details/ghtwvvvng.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.hesvh.cn/Article/details/grkkgeovv.sHtML

(x * 2 for x in arr)
来源：http://mobile.hesvh.cn/Article/details/gouqdvrwo.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.hesvh.cn/Article/details/gwvhdywyi.sHtML

Counter(arr).most_common(3)
来源：http://mobile.hesvh.cn/Article/details/gvcqohtot.sHtML

[U13] Py：固定长度队列
来源：http://baike.zdbjq.cn/Article/details/gdodwegzo.sHtML

deque(maxlen=10)
来源：http://read.share.fehbvm.com/Article/details/gcmgemxcd.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.zdbjq.cn/Article/details/ggaueuwov.sHtML

defaultdict(list)
来源：http://m.share.fehbvm.com/Article/details/gsbwjsxvz.sHtML

[U15] Py：高精度计时
来源：http://baike.fehbvm.com/Article/details/gmsksjpkf.sHtML

t = time.perf_counter()
来源：http://wap.hesvh.cn/Article/details/gtdthvrms.sHtML

[U16] Py：命令行参数解析
来源：http://wap.zdbjq.cn/Article/details/gogdbmutv.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.fehbvm.com/Article/details/gywsfhdrq.sHtML

[U17] Py：初始化日志
来源：http://mobile.zdbjq.cn/Article/details/gkzbzhzcp.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.zdbjq.cn/Article/details/glfzbczvu.sHtML

[U18] Py：预编译正则
来源：http://www.share.zdbjq.cn/Article/details/gaombutfp.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.hesvh.cn/Article/details/gyuljbbyn.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.zdbjq.cn/Article/details/gcfaymotz.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.fehbvm.com/Article/details/gfcxbznwc.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.hesvh.cn/Article/details/goghlxszy.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.zdbjq.cn/Article/details/gkoyzpmvb.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.fehbvm.com/Article/details/gvgnhltdk.sHtML

@contextlib.contextmanager
来源：http://m.share.fehbvm.com/Article/details/gzgmlnzhi.sHtML

[U22] Py：矩阵转置
来源：http://blog.zdbjq.cn/Article/details/gdvwkmycf.sHtML

list(zip(*m))
来源：http://m.share.zdbjq.cn/Article/details/gaqvaifkn.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.fehbvm.com/Article/details/gazxwnqpi.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.hesvh.cn/Article/details/glufisjme.sHtML

[U24] Py：路径操作
来源：http://www.m.share.zdbjq.cn/Article/details/gwaazuwfd.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.zdbjq.cn/Article/details/gcvzcaanm.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.fehbvm.com/Article/details/giajfgxll.sHtML

csv.DictReader(f)
来源：http://mobile.hesvh.cn/Article/details/gqbdqwbmi.sHtML

[U26] Py：并发下载
来源：http://www.m.share.fehbvm.com/Article/details/gjkubzbvl.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.hesvh.cn/Article/details/gpehqmkme.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.zdbjq.cn/Article/details/gdcepnllf.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.zdbjq.cn/Article/details/gnpmdorat.sHtML

[U28] Py：类型别名
来源：http://www.m.share.zdbjq.cn/Article/details/getqkwjel.sHtML

UserId = int
来源：http://www.share.hesvh.cn/Article/details/gxorgbtdq.sHtML

[U29] Py：属性校验
来源：http://www.m.share.zdbjq.cn/Article/details/gbykxkykr.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.fehbvm.com/Article/details/ggwydxuto.sHtML

[U30] Py：数据类
来源：http://www.share.hesvh.cn/Article/details/gbejtrutb.sHtML

@dataclass(slots=True)
来源：http://baike.hesvh.cn/Article/details/gveihmgqh.sHtML

[U31] Py：单测
来源：http://mobile.hesvh.cn/Article/details/goolepwae.sHtML

python -m pytest -q
来源：http://m.share.fehbvm.com/Article/details/gsafyrezk.sHtML

[U32] Py：代码格式化
来源：http://www.share.zdbjq.cn/Article/details/gpfrcqcha.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.fehbvm.com/Article/details/gqiyfvvln.sHtML

[U33] Py：打包发布
来源：http://www.blog.fehbvm.com/Article/details/guoivmbfd.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.fehbvm.com/Article/details/gxuhrumma.sHtML

[U34] Py：判断编码
来源：http://baike.fehbvm.com/Article/details/grtbyntcy.sHtML

chardet.detect(raw)
来源：http://www.share.fehbvm.com/Article/details/gqzzrlfah.sHtML

[U35] Py：发送邮件
来源：http://m.share.zdbjq.cn/Article/details/gravhokcu.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.hesvh.cn/Article/details/gigqjzvci.sHtML

[U36] Py：定时任务
来源：http://www.m.share.fehbvm.com/Article/details/gmwncmknr.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.fehbvm.com/Article/details/gyqesbrct.sHtML

[U37] Py：读写 Excel
来源：http://baike.fehbvm.com/Article/details/grdlolksu.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.fehbvm.com/Article/details/grqhulsem.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.fehbvm.com/Article/details/ggkcxuhnx.sHtML

Path(__file__).resolve().parent
来源：http://wap.hesvh.cn/Article/details/gqjfamtzi.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.fehbvm.com/Article/details/gojkhhpkx.sHtML

sys.stdout.isatty()
来源：http://baike.fehbvm.com/Article/details/gxtxqzwyc.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.zdbjq.cn/Article/details/gqeuoctyq.sHtML

print("err", file=sys.stderr)
来源：http://mobile.fehbvm.com/Article/details/gdjpqxtlm.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.fehbvm.com/Article/details/gidaivybx.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.fehbvm.com/Article/details/gotkueisx.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.hesvh.cn/Article/details/gofgdtoxa.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.fehbvm.com/Article/details/gsnhqiqyf.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.fehbvm.com/Article/details/gvaoubfno.sHtML

namespace App\Http;
来源：http://mobile.zdbjq.cn/Article/details/gvmllhpbu.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.zdbjq.cn/Article/details/gvtagwciz.sHtML

declare(strict_types=1);
来源：http://mobile.fehbvm.com/Article/details/getaztbxw.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.hesvh.cn/Article/details/gorwzaofg.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gtsrpsghy.sHtML

[U46] PHP：可空类型
来源：http://m.share.hesvh.cn/Article/details/gukakaifn.sHtML

?string $name = null
来源：http://baike.hesvh.cn/Article/details/gxsieyugw.sHtML

[U47] PHP：联合类型
来源：http://mobile.fehbvm.com/Article/details/gmwrsdcsb.sHtML

int|string $id
来源：http://wap.zdbjq.cn/Article/details/gsdietzwp.sHtML

[U48] PHP：纯枚举
来源：http://wap.zdbjq.cn/Article/details/gaxwybvmq.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.fehbvm.com/Article/details/gtgomrlfi.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.hesvh.cn/Article/details/gpoekfsrp.sHtML

public readonly string $name
来源：http://www.share.hesvh.cn/Article/details/gdpjzjbex.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.fehbvm.com/Article/details/ggougiwgg.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.fehbvm.com/Article/details/ggjqlykjf.sHtML

[U51] PHP：数组解构
来源：http://wap.zdbjq.cn/Article/details/gxwqiwoqf.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.hesvh.cn/Article/details/gsabfknpj.sHtML

[U52] PHP：箭头函数
来源：http://wap.hesvh.cn/Article/details/gegnodjel.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.fehbvm.com/Article/details/gejrhvkil.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.hesvh.cn/Article/details/gqimtxydr.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.hesvh.cn/Article/details/gonvekonf.sHtML

[U54] PHP：空安全调用
来源：http://m.share.fehbvm.com/Article/details/grbzqzsdo.sHtML

$obj?->method()
来源：http://3g.fehbvm.com/Article/details/gesadkyuk.sHtML

[U55] PHP：match 表达式
来源：http://read.share.hesvh.cn/Article/details/gdvpswpxa.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.fehbvm.com/Article/details/gfhztkzrc.sHtML

[U56] PHP：命名参数
来源：http://m.share.zdbjq.cn/Article/details/gfcaatntq.sHtML

f(a: 1, b: 2)
来源：http://wap.hesvh.cn/Article/details/guscijpvz.sHtML

[U57] PHP：字符串插值
来源：http://blog.hesvh.cn/Article/details/gfedhwiml.sHtML

"值: {$a}"
来源：http://www.m.share.hesvh.cn/Article/details/gxetehslu.sHtML

[U58] PHP：数组三件套
来源：http://baike.hesvh.cn/Article/details/gqnnnyqyc.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.fehbvm.com/Article/details/grebezobi.sHtML

[U59] PHP：自定义排序
来源：http://read.share.zdbjq.cn/Article/details/gfyzcteub.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.zdbjq.cn/Article/details/gkkcphcyo.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.fehbvm.com/Article/details/gfsndhjrr.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.hesvh.cn/Article/details/gmtbwppsx.sHtML

[U61] PHP：正则
来源：http://www.m.share.zdbjq.cn/Article/details/gaqbkzgxx.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.hesvh.cn/Article/details/gguvfjpjg.sHtML

[U62] PHP：日期对象
来源：http://m.share.hesvh.cn/Article/details/ggdtiliiz.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.fehbvm.com/Article/details/gkoduiebt.sHtML

[U63] PHP：文件读写
来源：http://m.share.fehbvm.com/Article/details/gbulmnqta.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.hesvh.cn/Article/details/gcrunukhe.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.fehbvm.com/Article/details/gsgspbbkm.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.zdbjq.cn/Article/details/guslmsbtk.sHtML


<!-- 参考信息 -->