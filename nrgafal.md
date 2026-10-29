代发 wailian999

[S41] C++：类与构造函数
来源：http://3g.hesvh.cn/Article/details/ghbmbcsfn.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.hesvh.cn/Article/details/gqtnnfywi.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.hesvh.cn/Article/details/gjislkfwu.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.zdbjq.cn/Article/details/gfxsrvvbu.sHtML

[S43] C++：智能指针
来源：http://www.share.fehbvm.com/Article/details/gnkdofdqu.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.zdbjq.cn/Article/details/glcibzurt.sHtML

[S44] C++：引用传参
来源：http://www.m.share.hesvh.cn/Article/details/gpfojbnce.sHtML

void inc(int &x) { ++x; }
来源：http://baike.zdbjq.cn/Article/details/guevkxfkj.sHtML

[S45] C++：lambda
来源：http://www.blog.hesvh.cn/Article/details/gdxbfysri.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.hesvh.cn/Article/details/gsqijnqlw.sHtML

[S46] C++：函数模板
来源：http://read.share.fehbvm.com/Article/details/gzlfyagte.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fehbvm.com/Article/details/gqohhfpkc.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fehbvm.com/Article/details/gydwcjaiz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fehbvm.com/Article/details/gupuvyhnc.sHtML

[S48] C++：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gccrhyhfz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.hesvh.cn/Article/details/gximlehqc.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.hesvh.cn/Article/details/gqgapqwfs.sHtML

[S49] C++：写文件
来源：http://m.share.fehbvm.com/Article/details/gtdzpxsop.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.zdbjq.cn/Article/details/gbjbzqxhz.sHtML

[S50] C++：格式化数字
来源：http://wap.fehbvm.com/Article/details/gisoiosfv.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gsjgvnhca.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fehbvm.com/Article/details/ghecevogi.sHtML

static_cast<double>(a) / b
来源：http://m.share.hesvh.cn/Article/details/gtrumsyki.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fehbvm.com/Article/details/gzrjhusva.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.hesvh.cn/Article/details/glunehiwe.sHtML

[S53] C++：移动语义
来源：http://3g.zdbjq.cn/Article/details/genfctyyi.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.hesvh.cn/Article/details/grwibfwxr.sHtML

[S54] C++：异常处理
来源：http://www.share.zdbjq.cn/Article/details/ghhdjkett.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fehbvm.com/Article/details/gldjtmrdf.sHtML

[S55] C++：结构化绑定
来源：http://www.share.hesvh.cn/Article/details/gdlpojyzr.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.hesvh.cn/Article/details/gowptoiyn.sHtML

[S56] C++：optional
来源：http://3g.fehbvm.com/Article/details/gqzdpwdyc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.hesvh.cn/Article/details/gjrnyytad.sHtML

[S57] C++：编译期常量
来源：http://m.share.hesvh.cn/Article/details/gdtidopsy.sHtML

constexpr int N = 10;
来源：http://mobile.hesvh.cn/Article/details/gdrpcruxz.sHtML

[S58] C++：命名空间
来源：http://www.share.fehbvm.com/Article/details/gcpqszrro.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.zdbjq.cn/Article/details/glygbfqek.sHtML

[S59] C++：静态断言
来源：http://3g.fehbvm.com/Article/details/gfzmxecnq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.zdbjq.cn/Article/details/gvjifgaix.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fehbvm.com/Article/details/ghsjtmkjt.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fehbvm.com/Article/details/gzkgzwtcd.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ghdcscttq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.zdbjq.cn/Article/details/gpejynbyq.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gxdilfykq.sHtML

[T01] Kotlin：Hello World
来源：http://blog.hesvh.cn/Article/details/gbtedcvhy.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/glosoabah.sHtML

[T02] Kotlin：变量
来源：http://www.share.hesvh.cn/Article/details/gbpzbevpu.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.hesvh.cn/Article/details/gzobhsiev.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.zdbjq.cn/Article/details/gsjmyxvuk.sHtML

"值: $b"
来源：http://blog.hesvh.cn/Article/details/gnhgpoeah.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.zdbjq.cn/Article/details/gdccjuibu.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fehbvm.com/Article/details/gndgxsdxp.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.zdbjq.cn/Article/details/gslrmsihw.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.hesvh.cn/Article/details/geqtwefcn.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.hesvh.cn/Article/details/gufenzcgj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fehbvm.com/Article/details/ghqxjyjcg.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.hesvh.cn/Article/details/gbnpjirlc.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.hesvh.cn/Article/details/gxrpynusd.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.hesvh.cn/Article/details/ggzcfpcmm.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fehbvm.com/Article/details/gwydgzzbe.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.hesvh.cn/Article/details/gwjlxbwgk.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.zdbjq.cn/Article/details/gjirhewmk.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.hesvh.cn/Article/details/gvucsheaq.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fehbvm.com/Article/details/gswftutgb.sHtML

[T11] Kotlin：协程
来源：http://read.share.fehbvm.com/Article/details/grsqjzsho.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.zdbjq.cn/Article/details/gjmqzvicf.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.zdbjq.cn/Article/details/gtlhuweii.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.hesvh.cn/Article/details/gjjegenqi.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.zdbjq.cn/Article/details/glgrdumun.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fehbvm.com/Article/details/gqfschyfj.sHtML

[T14] Kotlin：循环
来源：http://www.blog.hesvh.cn/Article/details/ggzjoegys.sHtML

for (i in 1..10) println(i)
来源：http://blog.fehbvm.com/Article/details/gctklwmdy.sHtML

[T15] Kotlin：接口
来源：http://m.share.zdbjq.cn/Article/details/gqvrnaqdw.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.hesvh.cn/Article/details/gmkuhtwxs.sHtML

[T16] Swift：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gggxpfeii.sHtML

print("Hello")
来源：http://www.share.fehbvm.com/Article/details/gjtmiflal.sHtML

[T17] Swift：变量与常量
来源：http://m.share.hesvh.cn/Article/details/goxlhjrhs.sHtML

var a = 1;  let b = 2
来源：http://mobile.hesvh.cn/Article/details/gisxcrxuc.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gkuzqpeyw.sHtML

"值: \(b)"
来源：http://www.share.zdbjq.cn/Article/details/gqzefjxpq.sHtML

[T19] Swift：可选绑定
来源：http://blog.fehbvm.com/Article/details/goothgjwb.sHtML

if let n = opt { print(n) }
来源：http://read.share.zdbjq.cn/Article/details/gcirznxez.sHtML

[T20] Swift：数组操作
来源：http://mobile.fehbvm.com/Article/details/ggrxqumko.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.hesvh.cn/Article/details/gpejhpiwe.sHtML

[T21] Swift：遍历
来源：http://wap.hesvh.cn/Article/details/gtyhcwgxh.sHtML

for x in a { print(x) }
来源：http://read.share.zdbjq.cn/Article/details/ggehajrdm.sHtML

[T22] Swift：字典
来源：http://read.share.zdbjq.cn/Article/details/gjgmjmxog.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fehbvm.com/Article/details/gsjkxdwtc.sHtML

[T23] Swift：函数
来源：http://baike.hesvh.cn/Article/details/gsepabzzo.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fehbvm.com/Article/details/gldmiiiil.sHtML

[T24] Swift：闭包
来源：http://www.share.fehbvm.com/Article/details/gqpbzltrg.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.hesvh.cn/Article/details/gqpzjjcaf.sHtML

[T25] Swift：结构体
来源：http://3g.zdbjq.cn/Article/details/gamvkumxb.sHtML

struct P { var x: Int }
来源：http://blog.fehbvm.com/Article/details/gibtcggzd.sHtML

[T26] Swift：类与重写
来源：http://m.share.zdbjq.cn/Article/details/gmfxfggiq.sHtML

class A: Base { override func f() {} }
来源：http://mobile.zdbjq.cn/Article/details/gsymvkcsq.sHtML

[T27] Swift：错误处理
来源：http://blog.zdbjq.cn/Article/details/giyzvikvl.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fehbvm.com/Article/details/gbmaexlae.sHtML

[T28] Swift：枚举
来源：http://m.share.fehbvm.com/Article/details/gxemzmkvt.sHtML

enum Color { case red, green }
来源：http://3g.zdbjq.cn/Article/details/gubjmidxu.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.zdbjq.cn/Article/details/gdwmngjro.sHtML

guard let x = opt else { return }
来源：http://www.m.share.hesvh.cn/Article/details/giordhbsf.sHtML

[T30] Swift：协议
来源：http://mobile.hesvh.cn/Article/details/gcumygsge.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fehbvm.com/Article/details/gqecubbmr.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/grfrabpwk.sHtML

print("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gnqptrsrz.sHtML

[T32] Lua：局部变量
来源：http://www.blog.zdbjq.cn/Article/details/giagecwde.sHtML

local a = 1
来源：http://baike.fehbvm.com/Article/details/gsfkilmdb.sHtML

[T33] Lua：表（数组）
来源：http://blog.fehbvm.com/Article/details/grmvnsiof.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.fehbvm.com/Article/details/gbasnsmxi.sHtML

[T34] Lua：遍历表
来源：http://blog.zdbjq.cn/Article/details/gpzkvblma.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.fehbvm.com/Article/details/gniiyuavt.sHtML

[T35] Lua：字典表
来源：http://3g.zdbjq.cn/Article/details/gbahukvfo.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.zdbjq.cn/Article/details/gbaghqexg.sHtML

[T36] Lua：函数
来源：http://wap.fehbvm.com/Article/details/gbpbunleq.sHtML

function add(a, b) return a + b end
来源：http://www.blog.hesvh.cn/Article/details/gbvpvcdgl.sHtML

[T37] Lua：字符串拼接
来源：http://3g.hesvh.cn/Article/details/gllhhuatk.sHtML

"a" .. "b"
来源：http://3g.zdbjq.cn/Article/details/gjlpowgll.sHtML

[T38] Lua：条件
来源：http://m.share.fehbvm.com/Article/details/gdquakhqi.sHtML

if x > 0 then print("正") end
来源：http://www.blog.hesvh.cn/Article/details/gravfobrc.sHtML

[T39] Lua：模式匹配
来源：http://baike.zdbjq.cn/Article/details/gdmrtzync.sHtML

string.find(s, "%d+")
来源：http://wap.hesvh.cn/Article/details/gfwvnnxvs.sHtML

[T40] Lua：元表
来源：http://mobile.fehbvm.com/Article/details/grdudumfj.sHtML

setmetatable({}, { __index = base })
来源：http://3g.hesvh.cn/Article/details/gpbdkxsuw.sHtML

[T41] Perl：Hello World
来源：http://3g.zdbjq.cn/Article/details/gfaxzgfzq.sHtML

print "Hello\n";
来源：http://www.share.zdbjq.cn/Article/details/gjcxkfbkg.sHtML

[T42] Perl：变量类型
来源：http://blog.fehbvm.com/Article/details/gaysbliwp.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.hesvh.cn/Article/details/gagysunae.sHtML

[T43] Perl：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gtowalrph.sHtML

"值: $a"
来源：http://www.share.zdbjq.cn/Article/details/gqmyhmqsn.sHtML

[T44] Perl：条件
来源：http://baike.hesvh.cn/Article/details/galbiqkbv.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.zdbjq.cn/Article/details/gdfqxirtn.sHtML

[T45] Perl：数组遍历
来源：http://baike.fehbvm.com/Article/details/ghwpswphn.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.fehbvm.com/Article/details/guxwchnvt.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.fehbvm.com/Article/details/gzhmudgas.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.hesvh.cn/Article/details/gcpnnkftg.sHtML

[T47] Perl：正则捕获
来源：http://read.share.fehbvm.com/Article/details/gzhycmmzz.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.hesvh.cn/Article/details/gqfqszbxl.sHtML

[T48] Perl：正则替换
来源：http://m.share.zdbjq.cn/Article/details/gpsnbvrah.sHtML

$s =~ s/old/new/g;
来源：http://www.share.fehbvm.com/Article/details/gihoyvhew.sHtML

[T49] Perl：函数
来源：http://m.share.fehbvm.com/Article/details/guudraedw.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gzhawwxxv.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/guqnjlaxo.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.hesvh.cn/Article/details/gbpopgpoi.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.zdbjq.cn/Article/details/gqccnbngq.sHtML

[T51] Scala：Hello World
来源：http://m.share.hesvh.cn/Article/details/gefpjrfmf.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/gytucqrgd.sHtML

[T52] Scala：变量
来源：http://baike.fehbvm.com/Article/details/gfnakcmub.sHtML

val a = 1;  var b = 2
来源：http://www.share.fehbvm.com/Article/details/ghfanaojh.sHtML

[T53] Scala：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gcbsccnxl.sHtML

s"值: $b"
来源：http://www.share.fehbvm.com/Article/details/gclptwzvo.sHtML

[T54] Scala：集合映射
来源：http://blog.fehbvm.com/Article/details/gcqjhkqln.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.fehbvm.com/Article/details/gvgnfhmcq.sHtML

[T55] Scala：集合过滤
来源：http://3g.hesvh.cn/Article/details/gxmisfkuk.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.hesvh.cn/Article/details/gberuuklh.sHtML

[T56] Scala：样例类
来源：http://baike.zdbjq.cn/Article/details/gyuzkumlo.sHtML

case class User(name: String, age: Int)
来源：http://m.share.hesvh.cn/Article/details/gjmpxknoi.sHtML

[T57] Scala：模式匹配
来源：http://wap.fehbvm.com/Article/details/gnbarsobv.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.fehbvm.com/Article/details/gtflkfwxv.sHtML

[T58] Scala：函数定义
来源：http://wap.fehbvm.com/Article/details/gpssjyrck.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fehbvm.com/Article/details/gvwdybzju.sHtML

[T59] Scala：循环
来源：http://mobile.fehbvm.com/Article/details/ggyivettl.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.hesvh.cn/Article/details/gdwpsozle.sHtML

[T60] Scala：折叠
来源：http://www.m.share.fehbvm.com/Article/details/gdyeyyvmt.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.zdbjq.cn/Article/details/grzvvtuia.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/glrxdbwqj.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.fehbvm.com/Article/details/giiecwgzk.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gfxymdblt.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.fehbvm.com/Article/details/gczivkjpi.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.zdbjq.cn/Article/details/ggeudnqpf.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.zdbjq.cn/Article/details/gscbnslgk.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.zdbjq.cn/Article/details/ghsvdrdlc.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.zdbjq.cn/Article/details/gxvpmsnuv.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.fehbvm.com/Article/details/grpqqmkbw.sHtML

[U04] Py：变量调试打印
来源：http://www.share.fehbvm.com/Article/details/gdyszlkby.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.fehbvm.com/Article/details/ggmdljyot.sHtML

[U05] Py：列表去重且保序
来源：http://wap.fehbvm.com/Article/details/gxgfrmjuh.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.fehbvm.com/Article/details/gfzvzutdt.sHtML

[U06] Py：合并两个字典
来源：http://www.share.hesvh.cn/Article/details/ganrqxvut.sHtML

{**a, **b}
来源：http://www.m.share.fehbvm.com/Article/details/gngickjfr.sHtML

[U07] Py：反转字典键值
来源：http://blog.zdbjq.cn/Article/details/gnoyzwxng.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fehbvm.com/Article/details/gjpmjkauz.sHtML

[U08] Py：展平二维列表
来源：http://m.share.fehbvm.com/Article/details/gznuklemq.sHtML

[y for x in nested for y in x]
来源：http://wap.hesvh.cn/Article/details/ggrxnopbd.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.hesvh.cn/Article/details/gdawkvttz.sHtML

max(d, key=d.get)
来源：http://baike.hesvh.cn/Article/details/grpbjktvt.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.zdbjq.cn/Article/details/gcdgjtyxl.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.fehbvm.com/Article/details/glbpyxcpq.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.fehbvm.com/Article/details/giwrqerui.sHtML

(x * 2 for x in arr)
来源：http://blog.hesvh.cn/Article/details/gynoedknm.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.fehbvm.com/Article/details/gkjlgapue.sHtML

Counter(arr).most_common(3)
来源：http://www.share.fehbvm.com/Article/details/gxcjnddgm.sHtML

[U13] Py：固定长度队列
来源：http://blog.zdbjq.cn/Article/details/gofobqwvb.sHtML

deque(maxlen=10)
来源：http://mobile.zdbjq.cn/Article/details/gptholxtj.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.hesvh.cn/Article/details/ghhabmrmx.sHtML

defaultdict(list)
来源：http://3g.zdbjq.cn/Article/details/gpzumznyo.sHtML

[U15] Py：高精度计时
来源：http://blog.fehbvm.com/Article/details/gmaiepiru.sHtML

t = time.perf_counter()
来源：http://wap.zdbjq.cn/Article/details/gkfdvpjeg.sHtML

[U16] Py：命令行参数解析
来源：http://3g.zdbjq.cn/Article/details/gpqldswtl.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.zdbjq.cn/Article/details/gjyjiqswv.sHtML

[U17] Py：初始化日志
来源：http://mobile.hesvh.cn/Article/details/gzoevvyik.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.hesvh.cn/Article/details/grdcuqljq.sHtML

[U18] Py：预编译正则
来源：http://blog.fehbvm.com/Article/details/gtotqvweo.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.hesvh.cn/Article/details/gogitwbwg.sHtML

[U19] Py：正则替换带回调
来源：http://baike.hesvh.cn/Article/details/ghdcnhgtn.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.fehbvm.com/Article/details/gudmcgbok.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.fehbvm.com/Article/details/gmhtaahdt.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.zdbjq.cn/Article/details/ghytkvehf.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.zdbjq.cn/Article/details/gsolnavjn.sHtML

@contextlib.contextmanager
来源：http://www.share.zdbjq.cn/Article/details/geaycifjn.sHtML

[U22] Py：矩阵转置
来源：http://read.share.fehbvm.com/Article/details/gaqhngprd.sHtML

list(zip(*m))
来源：http://m.share.fehbvm.com/Article/details/gkpfrogrw.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.hesvh.cn/Article/details/giypqdfup.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.zdbjq.cn/Article/details/gecevxdzk.sHtML

[U24] Py：路径操作
来源：http://m.share.zdbjq.cn/Article/details/gnrpqxcfi.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.zdbjq.cn/Article/details/goubfuilw.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.fehbvm.com/Article/details/gyjrrcjmr.sHtML

csv.DictReader(f)
来源：http://3g.hesvh.cn/Article/details/girrleorh.sHtML

[U26] Py：并发下载
来源：http://www.share.hesvh.cn/Article/details/glpfvjilr.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.zdbjq.cn/Article/details/gkczhttfo.sHtML

[U27] Py：异步 HTTP
来源：http://wap.hesvh.cn/Article/details/gwrztrdjf.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.hesvh.cn/Article/details/gvepzbzsg.sHtML

[U28] Py：类型别名
来源：http://blog.hesvh.cn/Article/details/gfovubada.sHtML

UserId = int
来源：http://wap.zdbjq.cn/Article/details/gunowkpdq.sHtML

[U29] Py：属性校验
来源：http://baike.zdbjq.cn/Article/details/gcrlgpoyj.sHtML

@property 与 @x.setter 配合
来源：http://m.share.hesvh.cn/Article/details/geagosxhi.sHtML

[U30] Py：数据类
来源：http://blog.zdbjq.cn/Article/details/ggtjsnenh.sHtML

@dataclass(slots=True)
来源：http://read.share.fehbvm.com/Article/details/gptllaitv.sHtML

[U31] Py：单测
来源：http://read.share.zdbjq.cn/Article/details/gmbvbcgep.sHtML

python -m pytest -q
来源：http://mobile.hesvh.cn/Article/details/gwxrzxlxr.sHtML

[U32] Py：代码格式化
来源：http://www.share.fehbvm.com/Article/details/gnvzqvnyn.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.hesvh.cn/Article/details/ghygfjyum.sHtML

[U33] Py：打包发布
来源：http://www.m.share.fehbvm.com/Article/details/gadxnkdun.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.fehbvm.com/Article/details/gnpekbnbe.sHtML

[U34] Py：判断编码
来源：http://mobile.zdbjq.cn/Article/details/gogcbirzv.sHtML

chardet.detect(raw)
来源：http://3g.zdbjq.cn/Article/details/ghrenvreu.sHtML

[U35] Py：发送邮件
来源：http://m.share.zdbjq.cn/Article/details/gbgfhhxvr.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.hesvh.cn/Article/details/gvmwyygbq.sHtML

[U36] Py：定时任务
来源：http://mobile.hesvh.cn/Article/details/gxvckjsye.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.zdbjq.cn/Article/details/gzlldayji.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.zdbjq.cn/Article/details/gcjvhjhfq.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.fehbvm.com/Article/details/gkbmjgutg.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.fehbvm.com/Article/details/gewzowqhx.sHtML

Path(__file__).resolve().parent
来源：http://blog.zdbjq.cn/Article/details/gogxvaoln.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.zdbjq.cn/Article/details/gvxvtiybr.sHtML

sys.stdout.isatty()
来源：http://wap.zdbjq.cn/Article/details/gebhxdwae.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.hesvh.cn/Article/details/ggwtyyonk.sHtML

print("err", file=sys.stderr)
来源：http://www.share.zdbjq.cn/Article/details/gqvmvhynj.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.fehbvm.com/Article/details/gdhobvjfy.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.hesvh.cn/Article/details/gndyueoxo.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.fehbvm.com/Article/details/gxfhrenpy.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.hesvh.cn/Article/details/gjybeaoct.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.hesvh.cn/Article/details/gbdjxvfjo.sHtML

namespace App\Http;
来源：http://www.blog.zdbjq.cn/Article/details/gtkknqbav.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.hesvh.cn/Article/details/gzqakumjz.sHtML

declare(strict_types=1);
来源：http://www.blog.zdbjq.cn/Article/details/gjhcqnslz.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.fehbvm.com/Article/details/gqxyffwbi.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gyvezliwn.sHtML

[U46] PHP：可空类型
来源：http://3g.hesvh.cn/Article/details/giwlougdw.sHtML

?string $name = null
来源：http://www.share.zdbjq.cn/Article/details/gcajoygur.sHtML

[U47] PHP：联合类型
来源：http://m.share.hesvh.cn/Article/details/gwnricpjp.sHtML

int|string $id
来源：http://wap.fehbvm.com/Article/details/ggodcuhep.sHtML

[U48] PHP：纯枚举
来源：http://3g.hesvh.cn/Article/details/ghfyyxaqd.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.zdbjq.cn/Article/details/gwxwbkadr.sHtML

[U49] PHP：只读属性
来源：http://read.share.fehbvm.com/Article/details/gwlmyswpn.sHtML

public readonly string $name
来源：http://www.share.zdbjq.cn/Article/details/gcqqhcjsh.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.zdbjq.cn/Article/details/gydkzsdmf.sHtML

public function __construct(private int $id) {}
来源：http://wap.fehbvm.com/Article/details/gwrzvmdkf.sHtML

[U51] PHP：数组解构
来源：http://blog.fehbvm.com/Article/details/gnohshdws.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.fehbvm.com/Article/details/gizcglzrs.sHtML

[U52] PHP：箭头函数
来源：http://3g.zdbjq.cn/Article/details/gdyzojsfu.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.zdbjq.cn/Article/details/gvohelwed.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.fehbvm.com/Article/details/ggskcohfn.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.zdbjq.cn/Article/details/grklqwagt.sHtML

[U54] PHP：空安全调用
来源：http://m.share.hesvh.cn/Article/details/glfwwlkxt.sHtML

$obj?->method()
来源：http://read.share.hesvh.cn/Article/details/gbxanmhnz.sHtML

[U55] PHP：match 表达式
来源：http://baike.fehbvm.com/Article/details/gjhwodtzc.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.fehbvm.com/Article/details/gjbkairnr.sHtML

[U56] PHP：命名参数
来源：http://3g.zdbjq.cn/Article/details/gwbgdimcy.sHtML

f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/gaxredinv.sHtML

[U57] PHP：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gbtwjlbkh.sHtML

"值: {$a}"
来源：http://m.share.hesvh.cn/Article/details/gguzotbfc.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.hesvh.cn/Article/details/guiiexidb.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.zdbjq.cn/Article/details/gbrhoiwjj.sHtML

[U59] PHP：自定义排序
来源：http://read.share.hesvh.cn/Article/details/gvsyermmv.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.hesvh.cn/Article/details/gmlevujgj.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.zdbjq.cn/Article/details/gzfoorqqn.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.fehbvm.com/Article/details/gurwaamzo.sHtML

[U61] PHP：正则
来源：http://www.m.share.hesvh.cn/Article/details/girfdsbhs.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.hesvh.cn/Article/details/ggxzydlkl.sHtML

[U62] PHP：日期对象
来源：http://blog.zdbjq.cn/Article/details/gnvvyuxpv.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.hesvh.cn/Article/details/gumggknmi.sHtML

[U63] PHP：文件读写
来源：http://3g.fehbvm.com/Article/details/gkheqfypk.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.fehbvm.com/Article/details/gxmezween.sHtML

[U64] PHP：目录遍历
来源：http://m.share.zdbjq.cn/Article/details/gmnpzvmxt.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.zdbjq.cn/Article/details/gmvwvxcch.sHtML

[U65] PHP：会话
来源：http://3g.zdbjq.cn/Article/details/ghwsreybk.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gaxuxhswh.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.fehbvm.com/Article/details/gmkfdtksm.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.fehbvm.com/Article/details/gbyrfegab.sHtML


<!-- 参考信息 -->