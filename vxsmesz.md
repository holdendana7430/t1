代发 wailian999

[S41] C++：类与构造函数
来源：http://baike.hesvh.cn/Article/details/gdmrpnnyz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.hesvh.cn/Article/details/gadbfjawo.sHtML

[S42] C++：继承与虚函数
来源：http://3g.hesvh.cn/Article/details/gpxgmjqig.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.zdbjq.cn/Article/details/ggstjcozo.sHtML

[S43] C++：智能指针
来源：http://www.share.fehbvm.com/Article/details/gaafppada.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.zdbjq.cn/Article/details/gnvuspnek.sHtML

[S44] C++：引用传参
来源：http://www.blog.fehbvm.com/Article/details/geogzkamj.sHtML

void inc(int &x) { ++x; }
来源：http://3g.zdbjq.cn/Article/details/gwnapkdhp.sHtML

[S45] C++：lambda
来源：http://3g.hesvh.cn/Article/details/gcfzckwmb.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.hesvh.cn/Article/details/gmcffxfto.sHtML

[S46] C++：函数模板
来源：http://www.share.hesvh.cn/Article/details/ggokrwsal.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.hesvh.cn/Article/details/gzsxbqipb.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gtxyrdcay.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fehbvm.com/Article/details/gqmhsjjij.sHtML

[S48] C++：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gxxubfkxq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.zdbjq.cn/Article/details/ggtdcztfm.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.zdbjq.cn/Article/details/gxpfwrhvp.sHtML

[S49] C++：写文件
来源：http://mobile.zdbjq.cn/Article/details/gqtzppyzb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.hesvh.cn/Article/details/gdykhmnpg.sHtML

[S50] C++：格式化数字
来源：http://mobile.fehbvm.com/Article/details/glgmguywt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gdxxfkbkc.sHtML

[S51] C++：显式类型转换
来源：http://3g.zdbjq.cn/Article/details/gpzknezix.sHtML

static_cast<double>(a) / b
来源：http://blog.fehbvm.com/Article/details/gcqjlqhil.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.hesvh.cn/Article/details/ggnuefqgq.sHtML

int size() const noexcept { return n_; }
来源：http://wap.zdbjq.cn/Article/details/ggqwbzchi.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fehbvm.com/Article/details/gocgatcky.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.hesvh.cn/Article/details/gowtgrxwd.sHtML

[S54] C++：异常处理
来源：http://www.m.share.zdbjq.cn/Article/details/geylixiqo.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.hesvh.cn/Article/details/gttvatzby.sHtML

[S55] C++：结构化绑定
来源：http://3g.hesvh.cn/Article/details/gtmkzhvgt.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fehbvm.com/Article/details/glmcivoeh.sHtML

[S56] C++：optional
来源：http://blog.hesvh.cn/Article/details/gfayflbdg.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.zdbjq.cn/Article/details/gvrxgepvs.sHtML

[S57] C++：编译期常量
来源：http://baike.fehbvm.com/Article/details/gvdlebdmi.sHtML

constexpr int N = 10;
来源：http://www.share.hesvh.cn/Article/details/gmgpummec.sHtML

[S58] C++：命名空间
来源：http://mobile.fehbvm.com/Article/details/gjtzqkscq.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.zdbjq.cn/Article/details/gmvoklpno.sHtML

[S59] C++：静态断言
来源：http://www.share.hesvh.cn/Article/details/gxwyixtqb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.hesvh.cn/Article/details/gxlfsroxt.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.hesvh.cn/Article/details/ggefpfhyb.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/gqajhlwqc.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gdmeuadaa.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.hesvh.cn/Article/details/gjyojkzwh.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gocgmkckn.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.hesvh.cn/Article/details/gwuoksdgf.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gkpzrawix.sHtML

[T02] Kotlin：变量
来源：http://read.share.fehbvm.com/Article/details/gxpnresxx.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fehbvm.com/Article/details/gmmyuuluf.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.hesvh.cn/Article/details/gukmwafdn.sHtML

"值: $b"
来源：http://baike.fehbvm.com/Article/details/gcqbkhwnr.sHtML

[T04] Kotlin：空安全
来源：http://read.share.zdbjq.cn/Article/details/gszhuqmqi.sHtML

val n: String? = null;  n?.length
来源：http://m.share.zdbjq.cn/Article/details/gxswbalou.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.zdbjq.cn/Article/details/gmglenqex.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.zdbjq.cn/Article/details/gjvzqjtds.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fehbvm.com/Article/details/gkqjprnge.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gervukjjf.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.hesvh.cn/Article/details/gkcdrpjhj.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.zdbjq.cn/Article/details/gzpahhsap.sHtML

[T08] Kotlin：数据类
来源：http://www.share.hesvh.cn/Article/details/gcjdvaium.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fehbvm.com/Article/details/gusvwwirs.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.hesvh.cn/Article/details/gnedcnyzn.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fehbvm.com/Article/details/gjbkdrbhx.sHtML

[T10] Kotlin：默认参数
来源：http://3g.hesvh.cn/Article/details/gophpecvs.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.hesvh.cn/Article/details/gqxtbajfo.sHtML

[T11] Kotlin：协程
来源：http://m.share.fehbvm.com/Article/details/giyruazyl.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.zdbjq.cn/Article/details/ghpjpfgyi.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fehbvm.com/Article/details/ggjfeudyd.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gomzkmokw.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.hesvh.cn/Article/details/gfgkaeywt.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.hesvh.cn/Article/details/gkeewauzb.sHtML

[T14] Kotlin：循环
来源：http://www.share.zdbjq.cn/Article/details/grzhdyccf.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/ggalsoaro.sHtML

[T15] Kotlin：接口
来源：http://wap.hesvh.cn/Article/details/gnuugoufl.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.hesvh.cn/Article/details/gnjpywcnz.sHtML

[T16] Swift：Hello World
来源：http://blog.hesvh.cn/Article/details/ghrnjnvmy.sHtML

print("Hello")
来源：http://mobile.fehbvm.com/Article/details/gcsindtzu.sHtML

[T17] Swift：变量与常量
来源：http://read.share.hesvh.cn/Article/details/gfwkibekc.sHtML

var a = 1;  let b = 2
来源：http://3g.zdbjq.cn/Article/details/gicnweemb.sHtML

[T18] Swift：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gsybfsnee.sHtML

"值: \(b)"
来源：http://blog.fehbvm.com/Article/details/gtmzzkabr.sHtML

[T19] Swift：可选绑定
来源：http://read.share.hesvh.cn/Article/details/godprsuzu.sHtML

if let n = opt { print(n) }
来源：http://wap.zdbjq.cn/Article/details/gojhjufbe.sHtML

[T20] Swift：数组操作
来源：http://www.share.zdbjq.cn/Article/details/guzwbcaqx.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.fehbvm.com/Article/details/gpwunnybl.sHtML

[T21] Swift：遍历
来源：http://www.blog.fehbvm.com/Article/details/gqhfziokx.sHtML

for x in a { print(x) }
来源：http://baike.zdbjq.cn/Article/details/giykwjior.sHtML

[T22] Swift：字典
来源：http://mobile.fehbvm.com/Article/details/gumreqlox.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.zdbjq.cn/Article/details/gkzbfmzhm.sHtML

[T23] Swift：函数
来源：http://mobile.fehbvm.com/Article/details/gkveayedp.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.fehbvm.com/Article/details/gdmgybnbg.sHtML

[T24] Swift：闭包
来源：http://baike.hesvh.cn/Article/details/guxtjvgnz.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gaunrfwws.sHtML

[T25] Swift：结构体
来源：http://www.blog.fehbvm.com/Article/details/gduhzdgqw.sHtML

struct P { var x: Int }
来源：http://wap.hesvh.cn/Article/details/gmghtpbjj.sHtML

[T26] Swift：类与重写
来源：http://mobile.fehbvm.com/Article/details/gwcwnlltw.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fehbvm.com/Article/details/grhdkmqej.sHtML

[T27] Swift：错误处理
来源：http://blog.zdbjq.cn/Article/details/gkaxfnhcu.sHtML

do { try f() } catch { print(error) }
来源：http://3g.fehbvm.com/Article/details/gkkvhpkla.sHtML

[T28] Swift：枚举
来源：http://baike.hesvh.cn/Article/details/ghwsbuykk.sHtML

enum Color { case red, green }
来源：http://www.share.zdbjq.cn/Article/details/gvhllsabn.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.hesvh.cn/Article/details/giwjjtscs.sHtML

guard let x = opt else { return }
来源：http://www.share.zdbjq.cn/Article/details/gulsnoliy.sHtML

[T30] Swift：协议
来源：http://m.share.zdbjq.cn/Article/details/gmmyklpvk.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fehbvm.com/Article/details/gmixqxuzb.sHtML

[T31] Lua：Hello World
来源：http://read.share.zdbjq.cn/Article/details/guqpvqjmx.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/gmvlxbame.sHtML

[T32] Lua：局部变量
来源：http://blog.hesvh.cn/Article/details/gyafhaozp.sHtML

local a = 1
来源：http://wap.hesvh.cn/Article/details/ghhkzyzry.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.hesvh.cn/Article/details/gjbvjrkkm.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.hesvh.cn/Article/details/gayqkigdx.sHtML

[T34] Lua：遍历表
来源：http://baike.zdbjq.cn/Article/details/gbqfvxldy.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.fehbvm.com/Article/details/gzlehsmue.sHtML

[T35] Lua：字典表
来源：http://wap.hesvh.cn/Article/details/gadoygvxb.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.hesvh.cn/Article/details/gezhcwwvy.sHtML

[T36] Lua：函数
来源：http://3g.hesvh.cn/Article/details/gxqtbwlxc.sHtML

function add(a, b) return a + b end
来源：http://m.share.fehbvm.com/Article/details/gkuykgyvk.sHtML

[T37] Lua：字符串拼接
来源：http://3g.zdbjq.cn/Article/details/glclepvpf.sHtML

"a" .. "b"
来源：http://blog.hesvh.cn/Article/details/goncavhbc.sHtML

[T38] Lua：条件
来源：http://www.share.hesvh.cn/Article/details/gzwzcixxm.sHtML

if x > 0 then print("正") end
来源：http://www.blog.fehbvm.com/Article/details/gdarvuviq.sHtML

[T39] Lua：模式匹配
来源：http://www.share.zdbjq.cn/Article/details/geftkcrsj.sHtML

string.find(s, "%d+")
来源：http://mobile.fehbvm.com/Article/details/gwbnsihkf.sHtML

[T40] Lua：元表
来源：http://www.blog.fehbvm.com/Article/details/gmnwevjgt.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.fehbvm.com/Article/details/gureragku.sHtML

[T41] Perl：Hello World
来源：http://mobile.fehbvm.com/Article/details/gnfznlrju.sHtML

print "Hello\n";
来源：http://www.m.share.hesvh.cn/Article/details/giiddnmfu.sHtML

[T42] Perl：变量类型
来源：http://baike.hesvh.cn/Article/details/gmbzagipv.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.fehbvm.com/Article/details/gmknuqyvp.sHtML

[T43] Perl：字符串插值
来源：http://blog.hesvh.cn/Article/details/gntinmrze.sHtML

"值: $a"
来源：http://3g.fehbvm.com/Article/details/gdozgegvr.sHtML

[T44] Perl：条件
来源：http://read.share.hesvh.cn/Article/details/ghvirzuzr.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.zdbjq.cn/Article/details/gkggycuaq.sHtML

[T45] Perl：数组遍历
来源：http://wap.hesvh.cn/Article/details/gdgnubruj.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.hesvh.cn/Article/details/gnrmjzzwb.sHtML

[T46] Perl：哈希操作
来源：http://mobile.hesvh.cn/Article/details/gyrpkzbzi.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.fehbvm.com/Article/details/guosfffce.sHtML

[T47] Perl：正则捕获
来源：http://baike.fehbvm.com/Article/details/glpfkhcgy.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.zdbjq.cn/Article/details/gzcuxxvcq.sHtML

[T48] Perl：正则替换
来源：http://3g.zdbjq.cn/Article/details/gyzbkqpaz.sHtML

$s =~ s/old/new/g;
来源：http://baike.zdbjq.cn/Article/details/gnktidxny.sHtML

[T49] Perl：函数
来源：http://3g.hesvh.cn/Article/details/ghigrirhr.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gowbjpimf.sHtML

[T50] Perl：逐行读文件
来源：http://blog.fehbvm.com/Article/details/ggmvlzhmw.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.zdbjq.cn/Article/details/gvmxingpx.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.fehbvm.com/Article/details/grvkmsyyg.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gdefnimpx.sHtML

println("Hello")
来源：http://blog.fehbvm.com/Article/details/gaydrzxox.sHtML

[T52] Scala：变量
来源：http://www.blog.fehbvm.com/Article/details/ganosfkrn.sHtML

val a = 1;  var b = 2
来源：http://read.share.zdbjq.cn/Article/details/gvxxkjwtj.sHtML

[T53] Scala：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gcbregzqt.sHtML

s"值: $b"
来源：http://baike.hesvh.cn/Article/details/gtwmsobkl.sHtML

[T54] Scala：集合映射
来源：http://baike.fehbvm.com/Article/details/gpfoqmjux.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.fehbvm.com/Article/details/gbbfceyon.sHtML

[T55] Scala：集合过滤
来源：http://read.share.fehbvm.com/Article/details/gdlushrpb.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.zdbjq.cn/Article/details/ghcctbvbn.sHtML

[T56] Scala：样例类
来源：http://blog.fehbvm.com/Article/details/gxroozvxj.sHtML

case class User(name: String, age: Int)
来源：http://baike.zdbjq.cn/Article/details/gwrftrofp.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fehbvm.com/Article/details/gqgomjqgk.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.zdbjq.cn/Article/details/gxydrwbbp.sHtML

[T58] Scala：函数定义
来源：http://m.share.hesvh.cn/Article/details/ghsecgvcc.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.zdbjq.cn/Article/details/geumcajps.sHtML

[T59] Scala：循环
来源：http://read.share.zdbjq.cn/Article/details/gfqojpglp.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.fehbvm.com/Article/details/guxdqjkct.sHtML

[T60] Scala：折叠
来源：http://m.share.fehbvm.com/Article/details/gwlokvqln.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.zdbjq.cn/Article/details/gyrstoylz.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gtmclgawj.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.hesvh.cn/Article/details/gjcedioix.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gtylzably.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.zdbjq.cn/Article/details/gaeaeutcq.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.fehbvm.com/Article/details/gwthzfmsy.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.hesvh.cn/Article/details/ghuzmryet.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.fehbvm.com/Article/details/gaatddfro.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.fehbvm.com/Article/details/gzricxkqk.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.zdbjq.cn/Article/details/gsaqggjoh.sHtML

[U04] Py：变量调试打印
来源：http://3g.hesvh.cn/Article/details/grbdafjvv.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.hesvh.cn/Article/details/gjrczwobq.sHtML

[U05] Py：列表去重且保序
来源：http://blog.fehbvm.com/Article/details/gnaibjbei.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.fehbvm.com/Article/details/gqivjwsdy.sHtML

[U06] Py：合并两个字典
来源：http://wap.zdbjq.cn/Article/details/gtmuatkdq.sHtML

{**a, **b}
来源：http://www.m.share.hesvh.cn/Article/details/gdujdzewc.sHtML

[U07] Py：反转字典键值
来源：http://wap.hesvh.cn/Article/details/gefgrqizv.sHtML

{v: k for k, v in d.items()}
来源：http://wap.fehbvm.com/Article/details/gcidxsoqv.sHtML

[U08] Py：展平二维列表
来源：http://www.share.fehbvm.com/Article/details/gzscogept.sHtML

[y for x in nested for y in x]
来源：http://blog.fehbvm.com/Article/details/gdystpbho.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.fehbvm.com/Article/details/gbipwmiiz.sHtML

max(d, key=d.get)
来源：http://www.share.fehbvm.com/Article/details/gqzwbahqq.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.fehbvm.com/Article/details/glysrixey.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.fehbvm.com/Article/details/gxjsobrbp.sHtML

[U11] Py：生成器表达式
来源：http://blog.fehbvm.com/Article/details/gzqksqiys.sHtML

(x * 2 for x in arr)
来源：http://baike.hesvh.cn/Article/details/gcjoajzhs.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.fehbvm.com/Article/details/godskkteg.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.fehbvm.com/Article/details/guqovadng.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.fehbvm.com/Article/details/gelqjqeqa.sHtML

deque(maxlen=10)
来源：http://www.m.share.fehbvm.com/Article/details/grbdpjqll.sHtML

[U14] Py：分组收集到列表
来源：http://wap.fehbvm.com/Article/details/guqzhfzjw.sHtML

defaultdict(list)
来源：http://wap.zdbjq.cn/Article/details/gffyscjjp.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.hesvh.cn/Article/details/guwvmjpqo.sHtML

t = time.perf_counter()
来源：http://www.m.share.zdbjq.cn/Article/details/ggwbtabet.sHtML

[U16] Py：命令行参数解析
来源：http://baike.hesvh.cn/Article/details/gwowgxyns.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.fehbvm.com/Article/details/glaiopczw.sHtML

[U17] Py：初始化日志
来源：http://www.blog.zdbjq.cn/Article/details/gfmvoboax.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.fehbvm.com/Article/details/gbgfwjnrv.sHtML

[U18] Py：预编译正则
来源：http://read.share.hesvh.cn/Article/details/gflvtlyjv.sHtML

pat = re.compile(r"\d+")
来源：http://baike.hesvh.cn/Article/details/gpfchefep.sHtML

[U19] Py：正则替换带回调
来源：http://baike.zdbjq.cn/Article/details/gdftchagb.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.zdbjq.cn/Article/details/gukibftyo.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.zdbjq.cn/Article/details/gbbuqertp.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.fehbvm.com/Article/details/gyyalfelt.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.zdbjq.cn/Article/details/gulzsrwys.sHtML

@contextlib.contextmanager
来源：http://wap.zdbjq.cn/Article/details/gfoimacli.sHtML

[U22] Py：矩阵转置
来源：http://www.share.hesvh.cn/Article/details/gukrkpxak.sHtML

list(zip(*m))
来源：http://www.share.zdbjq.cn/Article/details/gmbcnscrb.sHtML

[U23] Py：分块读取大文件
来源：http://3g.fehbvm.com/Article/details/gizsfhzvy.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.zdbjq.cn/Article/details/gthoqxmut.sHtML

[U24] Py：路径操作
来源：http://mobile.fehbvm.com/Article/details/gwpeeijph.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/gpdaaplwt.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.zdbjq.cn/Article/details/gccdzybam.sHtML

csv.DictReader(f)
来源：http://www.blog.fehbvm.com/Article/details/gtlqynppu.sHtML

[U26] Py：并发下载
来源：http://wap.fehbvm.com/Article/details/gmdmojyps.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.fehbvm.com/Article/details/gxbwytzxv.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.hesvh.cn/Article/details/gmukdqanf.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.hesvh.cn/Article/details/givwfmbxs.sHtML

[U28] Py：类型别名
来源：http://blog.hesvh.cn/Article/details/gvkolaakk.sHtML

UserId = int
来源：http://read.share.hesvh.cn/Article/details/giehxjqcy.sHtML

[U29] Py：属性校验
来源：http://www.m.share.hesvh.cn/Article/details/gjzvigwue.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.zdbjq.cn/Article/details/ghzpsuerr.sHtML

[U30] Py：数据类
来源：http://read.share.hesvh.cn/Article/details/gaezwfkrr.sHtML

@dataclass(slots=True)
来源：http://m.share.fehbvm.com/Article/details/geurrowyd.sHtML

[U31] Py：单测
来源：http://blog.zdbjq.cn/Article/details/gnxtilkjm.sHtML

python -m pytest -q
来源：http://blog.fehbvm.com/Article/details/gfcgbotqb.sHtML

[U32] Py：代码格式化
来源：http://read.share.zdbjq.cn/Article/details/gldrolzxw.sHtML

ruff format . && ruff check --fix .
来源：http://baike.zdbjq.cn/Article/details/gvyzaczuh.sHtML

[U33] Py：打包发布
来源：http://blog.fehbvm.com/Article/details/gnufdtbjl.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.hesvh.cn/Article/details/gexfexhxb.sHtML

[U34] Py：判断编码
来源：http://blog.hesvh.cn/Article/details/gfgldkcgv.sHtML

chardet.detect(raw)
来源：http://wap.fehbvm.com/Article/details/gcqmpqsgi.sHtML

[U35] Py：发送邮件
来源：http://mobile.hesvh.cn/Article/details/gwlxsmpon.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.fehbvm.com/Article/details/gpmfbazvl.sHtML

[U36] Py：定时任务
来源：http://m.share.fehbvm.com/Article/details/guzkfxdea.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.fehbvm.com/Article/details/gsgqsecdg.sHtML

[U37] Py：读写 Excel
来源：http://read.share.fehbvm.com/Article/details/gchegfqzf.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.zdbjq.cn/Article/details/ggvtpogrs.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.hesvh.cn/Article/details/gmoahcbje.sHtML

Path(__file__).resolve().parent
来源：http://3g.zdbjq.cn/Article/details/giuhwpffp.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.hesvh.cn/Article/details/gaeyejbqn.sHtML

sys.stdout.isatty()
来源：http://mobile.fehbvm.com/Article/details/gqmtlpohx.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.zdbjq.cn/Article/details/gciditjof.sHtML

print("err", file=sys.stderr)
来源：http://blog.fehbvm.com/Article/details/gdktmlwca.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.fehbvm.com/Article/details/glzuxugwg.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.hesvh.cn/Article/details/gmutfbibw.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.fehbvm.com/Article/details/gaphtkyqn.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.zdbjq.cn/Article/details/gqpqiedlo.sHtML

[U43] PHP：声明命名空间
来源：http://blog.fehbvm.com/Article/details/gocueeiqb.sHtML

namespace App\Http;
来源：http://baike.hesvh.cn/Article/details/gnhueybdd.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.fehbvm.com/Article/details/gtmgpwxpz.sHtML

declare(strict_types=1);
来源：http://read.share.fehbvm.com/Article/details/gtwylshfv.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.hesvh.cn/Article/details/glmdqsrsg.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/glqjodvfl.sHtML

[U46] PHP：可空类型
来源：http://www.blog.hesvh.cn/Article/details/giasracal.sHtML

?string $name = null
来源：http://m.share.zdbjq.cn/Article/details/gvbmazngq.sHtML

[U47] PHP：联合类型
来源：http://3g.zdbjq.cn/Article/details/gabixdmkp.sHtML

int|string $id
来源：http://3g.zdbjq.cn/Article/details/ggxhqpkap.sHtML

[U48] PHP：纯枚举
来源：http://www.share.zdbjq.cn/Article/details/gqfzutofw.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.fehbvm.com/Article/details/gzhlpfzvk.sHtML

[U49] PHP：只读属性
来源：http://blog.zdbjq.cn/Article/details/gvmdtalta.sHtML

public readonly string $name
来源：http://www.m.share.zdbjq.cn/Article/details/gjgbuotlx.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.hesvh.cn/Article/details/gwwaisafx.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.fehbvm.com/Article/details/geuspuijd.sHtML

[U51] PHP：数组解构
来源：http://blog.hesvh.cn/Article/details/godgtrrsu.sHtML

[$a, $b] = $arr;
来源：http://blog.hesvh.cn/Article/details/gtkzquwtf.sHtML

[U52] PHP：箭头函数
来源：http://mobile.hesvh.cn/Article/details/gzuciodzg.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.zdbjq.cn/Article/details/gjksmhmlo.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.fehbvm.com/Article/details/gbksoaeyv.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.hesvh.cn/Article/details/gbzsyalxa.sHtML

[U54] PHP：空安全调用
来源：http://m.share.zdbjq.cn/Article/details/gcjjhmasv.sHtML

$obj?->method()
来源：http://mobile.fehbvm.com/Article/details/gaxzthmix.sHtML

[U55] PHP：match 表达式
来源：http://blog.hesvh.cn/Article/details/gcdncrfwt.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.hesvh.cn/Article/details/gzorybbcb.sHtML

[U56] PHP：命名参数
来源：http://www.share.hesvh.cn/Article/details/gdgfpinzj.sHtML

f(a: 1, b: 2)
来源：http://m.share.hesvh.cn/Article/details/gixdycfvb.sHtML

[U57] PHP：字符串插值
来源：http://blog.fehbvm.com/Article/details/gdlihmsix.sHtML

"值: {$a}"
来源：http://www.share.zdbjq.cn/Article/details/gcwltkkrz.sHtML

[U58] PHP：数组三件套
来源：http://mobile.fehbvm.com/Article/details/grtfqngap.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.zdbjq.cn/Article/details/gwhvjgzbr.sHtML

[U59] PHP：自定义排序
来源：http://m.share.fehbvm.com/Article/details/ggumepecz.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.hesvh.cn/Article/details/gxptrnazc.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.zdbjq.cn/Article/details/gkzbbzvnd.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gjcayfrts.sHtML

[U61] PHP：正则
来源：http://blog.fehbvm.com/Article/details/gzxcohnyy.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.hesvh.cn/Article/details/gkppbddlg.sHtML

[U62] PHP：日期对象
来源：http://m.share.hesvh.cn/Article/details/guzoweked.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.zdbjq.cn/Article/details/ghacyfxxm.sHtML

[U63] PHP：文件读写
来源：http://m.share.fehbvm.com/Article/details/gllzfnxdc.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.fehbvm.com/Article/details/gfcbdvykr.sHtML

[U64] PHP：目录遍历
来源：http://read.share.hesvh.cn/Article/details/gmcqgrzjq.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.hesvh.cn/Article/details/gyfdstcdc.sHtML

[U65] PHP：会话
来源：http://3g.hesvh.cn/Article/details/gimhhwkeo.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/ghdcqzlrt.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.fehbvm.com/Article/details/gkxtiqbbw.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.fehbvm.com/Article/details/gbsipplqy.sHtML


<!-- 参考信息 -->