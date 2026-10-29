代发 wailian999

[S37] C++：set
来源：http://wap.zdbjq.cn/Article/details/geaysblkg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.hesvh.cn/Article/details/gpzcqztab.sHtML

[S38] C++：排序
来源：http://wap.hesvh.cn/Article/details/geksruoye.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.hesvh.cn/Article/details/gfdaiohba.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fehbvm.com/Article/details/gcswfyqvc.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.hesvh.cn/Article/details/gxbbkaczn.sHtML

[S40] C++：查找元素
来源：http://m.share.zdbjq.cn/Article/details/gajmeitlo.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.hesvh.cn/Article/details/gezzpbcoj.sHtML

[S41] C++：类与构造函数
来源：http://wap.fehbvm.com/Article/details/gvnmmdgwm.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fehbvm.com/Article/details/gijdvmwzf.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.zdbjq.cn/Article/details/gibboczkd.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fehbvm.com/Article/details/gmeowupvm.sHtML

[S43] C++：智能指针
来源：http://mobile.zdbjq.cn/Article/details/gcochrdph.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.zdbjq.cn/Article/details/glsvdgttp.sHtML

[S44] C++：引用传参
来源：http://3g.zdbjq.cn/Article/details/gtnaycpzn.sHtML

void inc(int &x) { ++x; }
来源：http://wap.zdbjq.cn/Article/details/gomlpkili.sHtML

[S45] C++：lambda
来源：http://baike.hesvh.cn/Article/details/ghoxarnkc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fehbvm.com/Article/details/gygjygbdb.sHtML

[S46] C++：函数模板
来源：http://read.share.zdbjq.cn/Article/details/gnuqvxdts.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.zdbjq.cn/Article/details/gidycoodj.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fehbvm.com/Article/details/glcuyrapv.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fehbvm.com/Article/details/goigpccpa.sHtML

[S48] C++：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gmhbaoqei.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.hesvh.cn/Article/details/gdnkaoapj.sHtML

while (std::getline(in, line)) { }
来源：http://blog.hesvh.cn/Article/details/ggomwexlb.sHtML

[S49] C++：写文件
来源：http://3g.zdbjq.cn/Article/details/gzuozzeoy.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fehbvm.com/Article/details/gpygwuouk.sHtML

[S50] C++：格式化数字
来源：http://blog.zdbjq.cn/Article/details/glxybxouh.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/grscceyyk.sHtML

[S51] C++：显式类型转换
来源：http://3g.hesvh.cn/Article/details/gkhtkhjvm.sHtML

static_cast<double>(a) / b
来源：http://baike.hesvh.cn/Article/details/gymjvpsuk.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.zdbjq.cn/Article/details/gwtzxverv.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.zdbjq.cn/Article/details/gfwhzsukk.sHtML

[S53] C++：移动语义
来源：http://mobile.zdbjq.cn/Article/details/gazsgrtgu.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.zdbjq.cn/Article/details/gzlbfanwh.sHtML

[S54] C++：异常处理
来源：http://www.blog.zdbjq.cn/Article/details/gbkrtfoda.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fehbvm.com/Article/details/gwejyawse.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fehbvm.com/Article/details/gjtfskxdg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fehbvm.com/Article/details/gvukrzpvy.sHtML

[S56] C++：optional
来源：http://www.blog.hesvh.cn/Article/details/gtvygfkda.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.hesvh.cn/Article/details/glkqzpepw.sHtML

[S57] C++：编译期常量
来源：http://mobile.zdbjq.cn/Article/details/gnqbedrfz.sHtML

constexpr int N = 10;
来源：http://baike.zdbjq.cn/Article/details/gryycqdqo.sHtML

[S58] C++：命名空间
来源：http://www.share.fehbvm.com/Article/details/gwlqdwtpu.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gmbgcqbav.sHtML

[S59] C++：静态断言
来源：http://m.share.fehbvm.com/Article/details/gyfolumzp.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fehbvm.com/Article/details/gunokwxnq.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fehbvm.com/Article/details/gydnjsxdr.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.hesvh.cn/Article/details/gxyixtvfz.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ggeeexpcl.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fehbvm.com/Article/details/gxqiaaolj.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gkeuazfvj.sHtML

[T01] Kotlin：Hello World
来源：http://3g.zdbjq.cn/Article/details/gdctxvpyw.sHtML

println("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/giuaexyyr.sHtML

[T02] Kotlin：变量
来源：http://m.share.hesvh.cn/Article/details/gzfntwtbk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.zdbjq.cn/Article/details/gjngaakjg.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fehbvm.com/Article/details/gqsrjudgn.sHtML

"值: $b"
来源：http://wap.fehbvm.com/Article/details/gxbiyugwc.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fehbvm.com/Article/details/gmtlsfnvt.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.zdbjq.cn/Article/details/gsikwhynz.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.zdbjq.cn/Article/details/gbzmmimwe.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.hesvh.cn/Article/details/gurydquge.sHtML

[T06] Kotlin：集合映射
来源：http://blog.hesvh.cn/Article/details/gumifldep.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gcgtyyaub.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fehbvm.com/Article/details/gjjyotdwn.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.hesvh.cn/Article/details/gklgorimh.sHtML

[T08] Kotlin：数据类
来源：http://baike.hesvh.cn/Article/details/gbddqdayn.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.zdbjq.cn/Article/details/gamwfxotw.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.hesvh.cn/Article/details/gkfksitno.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fehbvm.com/Article/details/gynshltoh.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fehbvm.com/Article/details/gpqmiurvi.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.hesvh.cn/Article/details/gynzmsbew.sHtML

[T11] Kotlin：协程
来源：http://read.share.zdbjq.cn/Article/details/gkbmsndam.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.zdbjq.cn/Article/details/gthcjkbtv.sHtML

[T12] Kotlin：解构声明
来源：http://blog.hesvh.cn/Article/details/glzfuhocf.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.hesvh.cn/Article/details/gpzetbzhh.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fehbvm.com/Article/details/gchnvpymi.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gegrfopuk.sHtML

[T14] Kotlin：循环
来源：http://read.share.fehbvm.com/Article/details/gtevssgue.sHtML

for (i in 1..10) println(i)
来源：http://read.share.hesvh.cn/Article/details/gkltzxczm.sHtML

[T15] Kotlin：接口
来源：http://blog.zdbjq.cn/Article/details/gqyjtgygb.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.hesvh.cn/Article/details/gxfkuvgbh.sHtML

[T16] Swift：Hello World
来源：http://baike.fehbvm.com/Article/details/gorjluctg.sHtML

print("Hello")
来源：http://wap.hesvh.cn/Article/details/gfwbhcqxm.sHtML

[T17] Swift：变量与常量
来源：http://m.share.zdbjq.cn/Article/details/guzvltzog.sHtML

var a = 1;  let b = 2
来源：http://m.share.hesvh.cn/Article/details/grzlbuxto.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/geojpjeib.sHtML

"值: \(b)"
来源：http://blog.hesvh.cn/Article/details/ggzaqwikc.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fehbvm.com/Article/details/ghesfijjc.sHtML

if let n = opt { print(n) }
来源：http://www.share.zdbjq.cn/Article/details/gahjalinj.sHtML

[T20] Swift：数组操作
来源：http://blog.fehbvm.com/Article/details/glscnqikr.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.zdbjq.cn/Article/details/guzjemhcj.sHtML

[T21] Swift：遍历
来源：http://read.share.zdbjq.cn/Article/details/gvddcvfcn.sHtML

for x in a { print(x) }
来源：http://mobile.fehbvm.com/Article/details/gfytchnmn.sHtML

[T22] Swift：字典
来源：http://www.m.share.zdbjq.cn/Article/details/gvgicoqxm.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.hesvh.cn/Article/details/gordsyejw.sHtML

[T23] Swift：函数
来源：http://wap.fehbvm.com/Article/details/gjjvatfcx.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fehbvm.com/Article/details/glaptlkzv.sHtML

[T24] Swift：闭包
来源：http://wap.zdbjq.cn/Article/details/gmvliliip.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gskicivwb.sHtML

[T25] Swift：结构体
来源：http://read.share.hesvh.cn/Article/details/gyekklyuu.sHtML

struct P { var x: Int }
来源：http://read.share.hesvh.cn/Article/details/gdhepljnq.sHtML

[T26] Swift：类与重写
来源：http://m.share.zdbjq.cn/Article/details/gpkzfkssr.sHtML

class A: Base { override func f() {} }
来源：http://baike.zdbjq.cn/Article/details/giaayrgvu.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.zdbjq.cn/Article/details/gccakhwen.sHtML

do { try f() } catch { print(error) }
来源：http://3g.hesvh.cn/Article/details/gizagjnks.sHtML

[T28] Swift：枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gkfrgujxd.sHtML

enum Color { case red, green }
来源：http://blog.zdbjq.cn/Article/details/gmgfffzqw.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.hesvh.cn/Article/details/gbbxlmzdk.sHtML

guard let x = opt else { return }
来源：http://m.share.hesvh.cn/Article/details/gscauqgkp.sHtML

[T30] Swift：协议
来源：http://blog.hesvh.cn/Article/details/gytzvsghf.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.zdbjq.cn/Article/details/ghmtlzlij.sHtML

[T31] Lua：Hello World
来源：http://m.share.fehbvm.com/Article/details/gmhpunxqy.sHtML

print("Hello")
来源：http://www.share.fehbvm.com/Article/details/gngvtaycg.sHtML

[T32] Lua：局部变量
来源：http://read.share.fehbvm.com/Article/details/gkngzlafe.sHtML

local a = 1
来源：http://3g.fehbvm.com/Article/details/gxjgwledw.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fehbvm.com/Article/details/goezhcqdy.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.hesvh.cn/Article/details/ggmhtbueo.sHtML

[T34] Lua：遍历表
来源：http://www.share.fehbvm.com/Article/details/gtlwtychj.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.fehbvm.com/Article/details/gllywoyze.sHtML

[T35] Lua：字典表
来源：http://mobile.zdbjq.cn/Article/details/ghduybwjw.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.zdbjq.cn/Article/details/gpkutaayv.sHtML

[T36] Lua：函数
来源：http://blog.fehbvm.com/Article/details/gxromiumy.sHtML

function add(a, b) return a + b end
来源：http://wap.fehbvm.com/Article/details/goudqlfrd.sHtML

[T37] Lua：字符串拼接
来源：http://3g.hesvh.cn/Article/details/gbsvausbd.sHtML

"a" .. "b"
来源：http://www.blog.fehbvm.com/Article/details/gycuqcmca.sHtML

[T38] Lua：条件
来源：http://mobile.fehbvm.com/Article/details/gtguobxru.sHtML

if x > 0 then print("正") end
来源：http://mobile.zdbjq.cn/Article/details/ggdastlbb.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.zdbjq.cn/Article/details/gcfdfoeiz.sHtML

string.find(s, "%d+")
来源：http://www.share.hesvh.cn/Article/details/gpphzhkdg.sHtML

[T40] Lua：元表
来源：http://www.m.share.fehbvm.com/Article/details/ghsavmuff.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.fehbvm.com/Article/details/gncrxaooi.sHtML

[T41] Perl：Hello World
来源：http://blog.zdbjq.cn/Article/details/gdfgidbtr.sHtML

print "Hello\n";
来源：http://www.share.fehbvm.com/Article/details/guhvzjktn.sHtML

[T42] Perl：变量类型
来源：http://blog.zdbjq.cn/Article/details/gpbxzkzuy.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.fehbvm.com/Article/details/gtkrtfdxf.sHtML

[T43] Perl：字符串插值
来源：http://blog.hesvh.cn/Article/details/guelzgnux.sHtML

"值: $a"
来源：http://wap.fehbvm.com/Article/details/gyyramfrk.sHtML

[T44] Perl：条件
来源：http://3g.hesvh.cn/Article/details/gggrwcmlj.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.zdbjq.cn/Article/details/gdlstsfpy.sHtML

[T45] Perl：数组遍历
来源：http://m.share.hesvh.cn/Article/details/guvvjoycb.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.hesvh.cn/Article/details/gtwrwrexm.sHtML

[T46] Perl：哈希操作
来源：http://baike.hesvh.cn/Article/details/gwnmwhysj.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.hesvh.cn/Article/details/gmwiyiagw.sHtML

[T47] Perl：正则捕获
来源：http://wap.fehbvm.com/Article/details/gkcgkyiui.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.fehbvm.com/Article/details/gwydscfhh.sHtML

[T48] Perl：正则替换
来源：http://www.share.hesvh.cn/Article/details/gpnakgtve.sHtML

$s =~ s/old/new/g;
来源：http://wap.hesvh.cn/Article/details/gamuvlpie.sHtML

[T49] Perl：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gouingyds.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gfuzpueit.sHtML

[T50] Perl：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gayjclkft.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.fehbvm.com/Article/details/gnjnzyzax.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.hesvh.cn/Article/details/gnxlyglvv.sHtML

[T51] Scala：Hello World
来源：http://www.blog.fehbvm.com/Article/details/ggbgzgsoe.sHtML

println("Hello")
来源：http://www.blog.fehbvm.com/Article/details/ggbruvwav.sHtML

[T52] Scala：变量
来源：http://baike.fehbvm.com/Article/details/gkxinllev.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.hesvh.cn/Article/details/gapabdvnx.sHtML

[T53] Scala：字符串插值
来源：http://www.share.fehbvm.com/Article/details/ginmwunyp.sHtML

s"值: $b"
来源：http://baike.hesvh.cn/Article/details/gsfcpnsry.sHtML

[T54] Scala：集合映射
来源：http://www.blog.hesvh.cn/Article/details/gfurdgnxn.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.fehbvm.com/Article/details/gabncdugg.sHtML

[T55] Scala：集合过滤
来源：http://read.share.fehbvm.com/Article/details/gvnwifrrv.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.fehbvm.com/Article/details/gunpdtucm.sHtML

[T56] Scala：样例类
来源：http://mobile.hesvh.cn/Article/details/ghtpnsfll.sHtML

case class User(name: String, age: Int)
来源：http://www.share.zdbjq.cn/Article/details/gnsfznkny.sHtML

[T57] Scala：模式匹配
来源：http://www.share.fehbvm.com/Article/details/gjdcasvyl.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.zdbjq.cn/Article/details/giqdqrlgg.sHtML

[T58] Scala：函数定义
来源：http://www.share.hesvh.cn/Article/details/ghrvhblzc.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.hesvh.cn/Article/details/giuegufom.sHtML

[T59] Scala：循环
来源：http://www.m.share.zdbjq.cn/Article/details/grzhivykm.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.hesvh.cn/Article/details/gtkfxzgxi.sHtML

[T60] Scala：折叠
来源：http://read.share.zdbjq.cn/Article/details/gscmnmjje.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fehbvm.com/Article/details/gnjzqodsp.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gpxxevnku.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.hesvh.cn/Article/details/givpxocct.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gfewfdztd.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.hesvh.cn/Article/details/gnzitrmst.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.hesvh.cn/Article/details/ghynskdoy.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.zdbjq.cn/Article/details/gkwzzrbff.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.hesvh.cn/Article/details/gqupxhblp.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.hesvh.cn/Article/details/grbypsogc.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.fehbvm.com/Article/details/gvelmyfjx.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.hesvh.cn/Article/details/gypsjpjwg.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.fehbvm.com/Article/details/gtxhlxcss.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.fehbvm.com/Article/details/gexqebfxh.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/gqpbulbrw.sHtML

[U06] Py：合并两个字典
来源：http://wap.hesvh.cn/Article/details/gtoakpjgb.sHtML

{**a, **b}
来源：http://read.share.hesvh.cn/Article/details/goqgkozkc.sHtML

[U07] Py：反转字典键值
来源：http://mobile.fehbvm.com/Article/details/gebmialhb.sHtML

{v: k for k, v in d.items()}
来源：http://3g.fehbvm.com/Article/details/gtripizdg.sHtML

[U08] Py：展平二维列表
来源：http://mobile.zdbjq.cn/Article/details/gflxsxxrn.sHtML

[y for x in nested for y in x]
来源：http://read.share.fehbvm.com/Article/details/guclqsuia.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.hesvh.cn/Article/details/gznjfyrnd.sHtML

max(d, key=d.get)
来源：http://read.share.fehbvm.com/Article/details/geprgwpsl.sHtML

[U10] Py：按值排序字典
来源：http://baike.fehbvm.com/Article/details/giwpwikgz.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.fehbvm.com/Article/details/gylljtknl.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gljaijlut.sHtML

(x * 2 for x in arr)
来源：http://mobile.zdbjq.cn/Article/details/gmcgjymdz.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.hesvh.cn/Article/details/gzzcldaek.sHtML

Counter(arr).most_common(3)
来源：http://read.share.hesvh.cn/Article/details/gseugbshz.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.hesvh.cn/Article/details/gfitrbftm.sHtML

deque(maxlen=10)
来源：http://www.m.share.fehbvm.com/Article/details/gwntfgsad.sHtML

[U14] Py：分组收集到列表
来源：http://blog.fehbvm.com/Article/details/gxwevtgkr.sHtML

defaultdict(list)
来源：http://www.share.hesvh.cn/Article/details/gtnpyahib.sHtML

[U15] Py：高精度计时
来源：http://3g.hesvh.cn/Article/details/gxbcwrxpv.sHtML

t = time.perf_counter()
来源：http://wap.fehbvm.com/Article/details/gwzxxsrom.sHtML

[U16] Py：命令行参数解析
来源：http://3g.fehbvm.com/Article/details/gureksdyk.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.zdbjq.cn/Article/details/gjlemwddf.sHtML

[U17] Py：初始化日志
来源：http://mobile.fehbvm.com/Article/details/gzefpssyl.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.zdbjq.cn/Article/details/gyshbybgs.sHtML

[U18] Py：预编译正则
来源：http://www.blog.fehbvm.com/Article/details/gqclrmgpr.sHtML

pat = re.compile(r"\d+")
来源：http://blog.zdbjq.cn/Article/details/glfklxdkr.sHtML

[U19] Py：正则替换带回调
来源：http://wap.fehbvm.com/Article/details/gurrurjct.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.hesvh.cn/Article/details/gnirmloee.sHtML

[U20] Py：缓存函数结果
来源：http://baike.hesvh.cn/Article/details/gigfhwxtj.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.zdbjq.cn/Article/details/gdkaszvqm.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.hesvh.cn/Article/details/guiwxakga.sHtML

@contextlib.contextmanager
来源：http://blog.zdbjq.cn/Article/details/gebnpbxjo.sHtML

[U22] Py：矩阵转置
来源：http://mobile.fehbvm.com/Article/details/gahacyvyv.sHtML

list(zip(*m))
来源：http://baike.fehbvm.com/Article/details/gvobzffce.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.hesvh.cn/Article/details/gcdnkdzlr.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.fehbvm.com/Article/details/gakvcszsg.sHtML

[U24] Py：路径操作
来源：http://m.share.hesvh.cn/Article/details/gejjxrwfb.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.zdbjq.cn/Article/details/gzqjvfyri.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.fehbvm.com/Article/details/gtyivbdzd.sHtML

csv.DictReader(f)
来源：http://www.blog.fehbvm.com/Article/details/giwmbxent.sHtML

[U26] Py：并发下载
来源：http://www.m.share.hesvh.cn/Article/details/gsenswnqw.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.hesvh.cn/Article/details/gxfkxgktx.sHtML

[U27] Py：异步 HTTP
来源：http://wap.zdbjq.cn/Article/details/gohnvbydp.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.zdbjq.cn/Article/details/ghrneucle.sHtML

[U28] Py：类型别名
来源：http://www.blog.fehbvm.com/Article/details/ggswarcex.sHtML

UserId = int
来源：http://read.share.zdbjq.cn/Article/details/gtlbaefyr.sHtML

[U29] Py：属性校验
来源：http://baike.fehbvm.com/Article/details/glhdwhsdb.sHtML

@property 与 @x.setter 配合
来源：http://3g.fehbvm.com/Article/details/gxvhptrmy.sHtML

[U30] Py：数据类
来源：http://www.m.share.fehbvm.com/Article/details/gaeciqbzp.sHtML

@dataclass(slots=True)
来源：http://www.share.zdbjq.cn/Article/details/gnjvvnwnp.sHtML

[U31] Py：单测
来源：http://blog.hesvh.cn/Article/details/glmvaokds.sHtML

python -m pytest -q
来源：http://baike.zdbjq.cn/Article/details/grzatslcu.sHtML

[U32] Py：代码格式化
来源：http://blog.hesvh.cn/Article/details/gloewedip.sHtML

ruff format . && ruff check --fix .
来源：http://blog.hesvh.cn/Article/details/ghmicxbch.sHtML

[U33] Py：打包发布
来源：http://www.share.zdbjq.cn/Article/details/gdbpbtzpq.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.fehbvm.com/Article/details/gwmdviqsm.sHtML

[U34] Py：判断编码
来源：http://blog.hesvh.cn/Article/details/guhejklhm.sHtML

chardet.detect(raw)
来源：http://m.share.hesvh.cn/Article/details/gmxmrpkdi.sHtML

[U35] Py：发送邮件
来源：http://mobile.zdbjq.cn/Article/details/ggacxztvu.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.zdbjq.cn/Article/details/gyjxemmxh.sHtML

[U36] Py：定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/gyfbzjtwt.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.zdbjq.cn/Article/details/gilppegyn.sHtML

[U37] Py：读写 Excel
来源：http://mobile.fehbvm.com/Article/details/gsbirzkxa.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.zdbjq.cn/Article/details/gqdgmdneo.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.fehbvm.com/Article/details/gtzqmbkie.sHtML

Path(__file__).resolve().parent
来源：http://m.share.zdbjq.cn/Article/details/gygdljhbs.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.fehbvm.com/Article/details/gaeticoqv.sHtML

sys.stdout.isatty()
来源：http://3g.fehbvm.com/Article/details/gpkwuiysi.sHtML

[U40] Py：打印到标准错误
来源：http://3g.fehbvm.com/Article/details/gorxcrdef.sHtML

print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/gjvvlwzkr.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.zdbjq.cn/Article/details/gvhyxuzra.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.zdbjq.cn/Article/details/gbcsnuhtc.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.hesvh.cn/Article/details/gzkazrvrw.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.zdbjq.cn/Article/details/garbyiepa.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.zdbjq.cn/Article/details/gduhumvzu.sHtML

namespace App\Http;
来源：http://mobile.fehbvm.com/Article/details/gsnzyjdgw.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.zdbjq.cn/Article/details/gqprkmdsr.sHtML

declare(strict_types=1);
来源：http://www.share.hesvh.cn/Article/details/glmrxjbyx.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.hesvh.cn/Article/details/gagrjgbvg.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/glcdnzvuv.sHtML

[U46] PHP：可空类型
来源：http://3g.fehbvm.com/Article/details/gdrjxwmdu.sHtML

?string $name = null
来源：http://3g.fehbvm.com/Article/details/gsqudoarr.sHtML

[U47] PHP：联合类型
来源：http://baike.fehbvm.com/Article/details/ginmdgdqf.sHtML

int|string $id
来源：http://www.m.share.zdbjq.cn/Article/details/gvgsooumz.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.zdbjq.cn/Article/details/gqlcvlkdp.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.fehbvm.com/Article/details/gfndntzid.sHtML

[U49] PHP：只读属性
来源：http://read.share.fehbvm.com/Article/details/gqumygoqv.sHtML

public readonly string $name
来源：http://www.blog.hesvh.cn/Article/details/gtwxiwfsv.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.zdbjq.cn/Article/details/gxlquifxu.sHtML

public function __construct(private int $id) {}
来源：http://3g.zdbjq.cn/Article/details/gdzxkrijd.sHtML

[U51] PHP：数组解构
来源：http://www.share.fehbvm.com/Article/details/gvkguneti.sHtML

[$a, $b] = $arr;
来源：http://3g.hesvh.cn/Article/details/glswtlxsa.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.zdbjq.cn/Article/details/gpvvvfzep.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.fehbvm.com/Article/details/geunzymew.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.fehbvm.com/Article/details/ggxtvqwuv.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.fehbvm.com/Article/details/gttihqjcx.sHtML

[U54] PHP：空安全调用
来源：http://www.share.zdbjq.cn/Article/details/gksfoyyxb.sHtML

$obj?->method()
来源：http://www.blog.zdbjq.cn/Article/details/gbualhypi.sHtML

[U55] PHP：match 表达式
来源：http://wap.zdbjq.cn/Article/details/gevrggfgq.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.fehbvm.com/Article/details/gzszekrdn.sHtML

[U56] PHP：命名参数
来源：http://mobile.zdbjq.cn/Article/details/gqsamwjlo.sHtML

f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/gfxrwsngu.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gdsvkfwjc.sHtML

"值: {$a}"
来源：http://www.share.fehbvm.com/Article/details/gbzwxjsog.sHtML

[U58] PHP：数组三件套
来源：http://3g.zdbjq.cn/Article/details/gyikxlmih.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.hesvh.cn/Article/details/giceuddvp.sHtML

[U59] PHP：自定义排序
来源：http://mobile.hesvh.cn/Article/details/gsuklpwgc.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.zdbjq.cn/Article/details/galhflmha.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.fehbvm.com/Article/details/ghskbyoso.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.hesvh.cn/Article/details/guwajbkak.sHtML

[U61] PHP：正则
来源：http://read.share.hesvh.cn/Article/details/ghyxevxic.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.fehbvm.com/Article/details/gnwgknuck.sHtML

[U62] PHP：日期对象
来源：http://blog.hesvh.cn/Article/details/gshhaidkw.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.hesvh.cn/Article/details/gijshyjvt.sHtML


<!-- 参考信息 -->