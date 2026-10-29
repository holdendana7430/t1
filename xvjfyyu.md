代发 wailian999

[S37] C++：set
来源：http://m.share.zdbjq.cn/Article/details/gurhjyqiw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.zdbjq.cn/Article/details/ghcohlggt.sHtML

[S38] C++：排序
来源：http://wap.hesvh.cn/Article/details/gutiyraln.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fehbvm.com/Article/details/gjqoipcdc.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.zdbjq.cn/Article/details/gsgyadyqp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.zdbjq.cn/Article/details/glbqevvfg.sHtML

[S40] C++：查找元素
来源：http://wap.hesvh.cn/Article/details/gczvblpre.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.zdbjq.cn/Article/details/gqxphlnib.sHtML

[S41] C++：类与构造函数
来源：http://3g.hesvh.cn/Article/details/gsdogwwpy.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.zdbjq.cn/Article/details/gzgjkktkt.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.zdbjq.cn/Article/details/grpzpzmqu.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fehbvm.com/Article/details/gwufkkzxi.sHtML

[S43] C++：智能指针
来源：http://www.m.share.hesvh.cn/Article/details/gbxxrwucl.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fehbvm.com/Article/details/gzfwqexfr.sHtML

[S44] C++：引用传参
来源：http://www.m.share.zdbjq.cn/Article/details/gmbitcnnv.sHtML

void inc(int &x) { ++x; }
来源：http://wap.hesvh.cn/Article/details/gzbdvcbun.sHtML

[S45] C++：lambda
来源：http://mobile.fehbvm.com/Article/details/giksdgjlu.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fehbvm.com/Article/details/ggkqnknbs.sHtML

[S46] C++：函数模板
来源：http://www.blog.zdbjq.cn/Article/details/gyvxkdorh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fehbvm.com/Article/details/gkmhpgtke.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fehbvm.com/Article/details/ggsvgugwo.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.hesvh.cn/Article/details/gtnhueggn.sHtML

[S48] C++：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gdgnyaoqs.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.hesvh.cn/Article/details/gwfalhjxe.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.zdbjq.cn/Article/details/gbzlffmrm.sHtML

[S49] C++：写文件
来源：http://www.m.share.fehbvm.com/Article/details/gawhuqeiy.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fehbvm.com/Article/details/gbjjxgcpc.sHtML

[S50] C++：格式化数字
来源：http://mobile.zdbjq.cn/Article/details/gxgxdkqqa.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gvenccohy.sHtML

[S51] C++：显式类型转换
来源：http://read.share.hesvh.cn/Article/details/gunhdcqio.sHtML

static_cast<double>(a) / b
来源：http://read.share.zdbjq.cn/Article/details/grenvdasl.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.zdbjq.cn/Article/details/gmfiiykoh.sHtML

int size() const noexcept { return n_; }
来源：http://baike.zdbjq.cn/Article/details/gepglsydz.sHtML

[S53] C++：移动语义
来源：http://www.blog.fehbvm.com/Article/details/goymwfosc.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.zdbjq.cn/Article/details/gysszlmvy.sHtML

[S54] C++：异常处理
来源：http://blog.hesvh.cn/Article/details/gitdwtpgs.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.hesvh.cn/Article/details/gdkwgakur.sHtML

[S55] C++：结构化绑定
来源：http://read.share.hesvh.cn/Article/details/gdspqfrjy.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.hesvh.cn/Article/details/gnwefwvtr.sHtML

[S56] C++：optional
来源：http://read.share.fehbvm.com/Article/details/ghhxhewgv.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.zdbjq.cn/Article/details/gnuqcsnqq.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fehbvm.com/Article/details/gdfytamhm.sHtML

constexpr int N = 10;
来源：http://baike.hesvh.cn/Article/details/geanrsiza.sHtML

[S58] C++：命名空间
来源：http://www.m.share.zdbjq.cn/Article/details/gdohnkypx.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.fehbvm.com/Article/details/ggxenzhoi.sHtML

[S59] C++：静态断言
来源：http://www.m.share.hesvh.cn/Article/details/gmxxjnmad.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.hesvh.cn/Article/details/gkoyqehgd.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fehbvm.com/Article/details/gowclenew.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fehbvm.com/Article/details/gmmyznkls.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gajcdfrph.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.hesvh.cn/Article/details/gatusajvw.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gnyvlfrbo.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gtrmjhyhk.sHtML

println("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gvcizypms.sHtML

[T02] Kotlin：变量
来源：http://read.share.fehbvm.com/Article/details/gsfddylju.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.hesvh.cn/Article/details/gcvontqox.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.zdbjq.cn/Article/details/gvlmepskh.sHtML

"值: $b"
来源：http://wap.zdbjq.cn/Article/details/gbuwrufpl.sHtML

[T04] Kotlin：空安全
来源：http://3g.fehbvm.com/Article/details/gxktmexmb.sHtML

val n: String? = null;  n?.length
来源：http://mobile.zdbjq.cn/Article/details/gwtodnkwa.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.hesvh.cn/Article/details/gesbekuys.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.zdbjq.cn/Article/details/glatktalo.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.hesvh.cn/Article/details/guedcztrm.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gwpwoeyqr.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fehbvm.com/Article/details/gixhjfssy.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fehbvm.com/Article/details/grqtoshap.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fehbvm.com/Article/details/gojrxginf.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.zdbjq.cn/Article/details/gpvnrdtty.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.zdbjq.cn/Article/details/gmgmsychy.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.hesvh.cn/Article/details/glzgboslv.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.zdbjq.cn/Article/details/ggusapcfs.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.zdbjq.cn/Article/details/grwuhtzej.sHtML

[T11] Kotlin：协程
来源：http://blog.fehbvm.com/Article/details/gncwxchqz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fehbvm.com/Article/details/gotgesfec.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fehbvm.com/Article/details/gvdcelarl.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gyxxgykmv.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.zdbjq.cn/Article/details/gnkfhtbkg.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fehbvm.com/Article/details/ggebtomwb.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.hesvh.cn/Article/details/gjayrxcwo.sHtML

for (i in 1..10) println(i)
来源：http://blog.hesvh.cn/Article/details/guwsksyvd.sHtML

[T15] Kotlin：接口
来源：http://mobile.zdbjq.cn/Article/details/gvyhgjlya.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.hesvh.cn/Article/details/guqippvid.sHtML

[T16] Swift：Hello World
来源：http://3g.fehbvm.com/Article/details/ginwcfdzs.sHtML

print("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gcjndhfhj.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fehbvm.com/Article/details/gcvcsfnqn.sHtML

var a = 1;  let b = 2
来源：http://www.share.hesvh.cn/Article/details/gbbuexwwd.sHtML

[T18] Swift：字符串插值
来源：http://wap.fehbvm.com/Article/details/gwaqecngd.sHtML

"值: \(b)"
来源：http://wap.zdbjq.cn/Article/details/gbjjlxuyh.sHtML

[T19] Swift：可选绑定
来源：http://blog.hesvh.cn/Article/details/gynwrpsoo.sHtML

if let n = opt { print(n) }
来源：http://blog.zdbjq.cn/Article/details/gkskjbair.sHtML

[T20] Swift：数组操作
来源：http://wap.hesvh.cn/Article/details/gncxovlbv.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.hesvh.cn/Article/details/gdqjrfywt.sHtML

[T21] Swift：遍历
来源：http://www.blog.zdbjq.cn/Article/details/gqudkgbix.sHtML

for x in a { print(x) }
来源：http://www.share.zdbjq.cn/Article/details/gbilonuek.sHtML

[T22] Swift：字典
来源：http://baike.fehbvm.com/Article/details/gudzgases.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.fehbvm.com/Article/details/gcfbusgft.sHtML

[T23] Swift：函数
来源：http://read.share.fehbvm.com/Article/details/gqyqkcund.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.hesvh.cn/Article/details/geusxdhxf.sHtML

[T24] Swift：闭包
来源：http://mobile.fehbvm.com/Article/details/gwemcbjnf.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.zdbjq.cn/Article/details/gwlzhosek.sHtML

[T25] Swift：结构体
来源：http://www.share.zdbjq.cn/Article/details/griqrvaxq.sHtML

struct P { var x: Int }
来源：http://wap.zdbjq.cn/Article/details/gopevrpsa.sHtML

[T26] Swift：类与重写
来源：http://www.blog.hesvh.cn/Article/details/gklhrlbxy.sHtML

class A: Base { override func f() {} }
来源：http://m.share.zdbjq.cn/Article/details/gjrbbpdwl.sHtML

[T27] Swift：错误处理
来源：http://wap.fehbvm.com/Article/details/ggzsmbckn.sHtML

do { try f() } catch { print(error) }
来源：http://blog.fehbvm.com/Article/details/gzottyneh.sHtML

[T28] Swift：枚举
来源：http://baike.zdbjq.cn/Article/details/gnumkmwyo.sHtML

enum Color { case red, green }
来源：http://www.blog.hesvh.cn/Article/details/guzsnesbc.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.zdbjq.cn/Article/details/gluovsxzb.sHtML

guard let x = opt else { return }
来源：http://read.share.hesvh.cn/Article/details/gdclkzaxe.sHtML

[T30] Swift：协议
来源：http://www.m.share.zdbjq.cn/Article/details/gyrnrmeyg.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.hesvh.cn/Article/details/gpmwzfknm.sHtML

[T31] Lua：Hello World
来源：http://3g.hesvh.cn/Article/details/gumbwlqdx.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/ggkenluqk.sHtML

[T32] Lua：局部变量
来源：http://3g.fehbvm.com/Article/details/gozynmjjp.sHtML

local a = 1
来源：http://www.share.hesvh.cn/Article/details/ganlcrqsi.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.fehbvm.com/Article/details/gakyaudab.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.zdbjq.cn/Article/details/grlgxjjac.sHtML

[T34] Lua：遍历表
来源：http://blog.fehbvm.com/Article/details/ggtyatyoe.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.fehbvm.com/Article/details/grmovqjcr.sHtML

[T35] Lua：字典表
来源：http://wap.fehbvm.com/Article/details/gzfqcexqp.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.fehbvm.com/Article/details/gycbfhpqz.sHtML

[T36] Lua：函数
来源：http://blog.zdbjq.cn/Article/details/gvlvmahna.sHtML

function add(a, b) return a + b end
来源：http://mobile.zdbjq.cn/Article/details/gifigoqfh.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.fehbvm.com/Article/details/gdblcurut.sHtML

"a" .. "b"
来源：http://m.share.fehbvm.com/Article/details/gxkyqoyav.sHtML

[T38] Lua：条件
来源：http://baike.zdbjq.cn/Article/details/gkrewjnza.sHtML

if x > 0 then print("正") end
来源：http://www.share.fehbvm.com/Article/details/gdxtuykkx.sHtML

[T39] Lua：模式匹配
来源：http://baike.hesvh.cn/Article/details/grhrxyfrc.sHtML

string.find(s, "%d+")
来源：http://wap.fehbvm.com/Article/details/gcmjyspxf.sHtML

[T40] Lua：元表
来源：http://mobile.hesvh.cn/Article/details/grmhzghlo.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.zdbjq.cn/Article/details/gmhwugckn.sHtML

[T41] Perl：Hello World
来源：http://mobile.fehbvm.com/Article/details/gdhlxjgql.sHtML

print "Hello\n";
来源：http://blog.fehbvm.com/Article/details/gaqnaaifn.sHtML

[T42] Perl：变量类型
来源：http://wap.zdbjq.cn/Article/details/gkfakcsxt.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.fehbvm.com/Article/details/gxxelwuxd.sHtML

[T43] Perl：字符串插值
来源：http://wap.fehbvm.com/Article/details/grsjjxfsb.sHtML

"值: $a"
来源：http://blog.hesvh.cn/Article/details/ginfwpkvr.sHtML

[T44] Perl：条件
来源：http://www.share.zdbjq.cn/Article/details/gzxtkdvic.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.hesvh.cn/Article/details/gjptecvnp.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.hesvh.cn/Article/details/gzsbxsitm.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.zdbjq.cn/Article/details/gcuktioxv.sHtML

[T46] Perl：哈希操作
来源：http://wap.fehbvm.com/Article/details/gsqodvcxw.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.zdbjq.cn/Article/details/gqhepmmin.sHtML

[T47] Perl：正则捕获
来源：http://mobile.fehbvm.com/Article/details/glhycjutb.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.fehbvm.com/Article/details/gwbgdwyle.sHtML

[T48] Perl：正则替换
来源：http://m.share.hesvh.cn/Article/details/gmxcdkjkg.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.hesvh.cn/Article/details/gecssbzdj.sHtML

[T49] Perl：函数
来源：http://blog.zdbjq.cn/Article/details/gvurfatzk.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gopuvowql.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gnwtoseav.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.zdbjq.cn/Article/details/gqsjhgaoj.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.fehbvm.com/Article/details/gufqqqsbd.sHtML

[T51] Scala：Hello World
来源：http://mobile.hesvh.cn/Article/details/gdmkzlced.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/gyijqduuv.sHtML

[T52] Scala：变量
来源：http://www.share.hesvh.cn/Article/details/gwejemakb.sHtML

val a = 1;  var b = 2
来源：http://www.blog.fehbvm.com/Article/details/gdcfivnca.sHtML

[T53] Scala：字符串插值
来源：http://wap.hesvh.cn/Article/details/gcrwifssm.sHtML

s"值: $b"
来源：http://blog.hesvh.cn/Article/details/gnxooelfx.sHtML

[T54] Scala：集合映射
来源：http://read.share.hesvh.cn/Article/details/graxinkdr.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.hesvh.cn/Article/details/gifkvlquf.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fehbvm.com/Article/details/gdwtygypx.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.fehbvm.com/Article/details/gqtzwyvmt.sHtML

[T56] Scala：样例类
来源：http://m.share.fehbvm.com/Article/details/gxndclgqp.sHtML

case class User(name: String, age: Int)
来源：http://3g.zdbjq.cn/Article/details/gzsbonqws.sHtML

[T57] Scala：模式匹配
来源：http://m.share.hesvh.cn/Article/details/gzxgscezk.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.zdbjq.cn/Article/details/ghqqolkzt.sHtML

[T58] Scala：函数定义
来源：http://mobile.zdbjq.cn/Article/details/goopvbkhj.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.zdbjq.cn/Article/details/gbsjwftxh.sHtML

[T59] Scala：循环
来源：http://www.blog.hesvh.cn/Article/details/gznjrshrs.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.hesvh.cn/Article/details/goplnqufp.sHtML

[T60] Scala：折叠
来源：http://www.share.zdbjq.cn/Article/details/gcqllrhbj.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.zdbjq.cn/Article/details/gumrqqdzp.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gcibvyyyp.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.hesvh.cn/Article/details/gtgiioqpv.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gkkecywur.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.fehbvm.com/Article/details/gkchmusmo.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.fehbvm.com/Article/details/gmtvbvasw.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.zdbjq.cn/Article/details/gkqwbdwjl.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.hesvh.cn/Article/details/ggclktvfg.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.fehbvm.com/Article/details/gmddifuzx.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.hesvh.cn/Article/details/glttdrevo.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.fehbvm.com/Article/details/gzvmxhcvv.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.fehbvm.com/Article/details/gschsbqrc.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.zdbjq.cn/Article/details/gpxijauzo.sHtML

list(dict.fromkeys(arr))
来源：http://3g.fehbvm.com/Article/details/grugtmydf.sHtML

[U06] Py：合并两个字典
来源：http://m.share.zdbjq.cn/Article/details/gvvmlcwpu.sHtML

{**a, **b}
来源：http://www.m.share.zdbjq.cn/Article/details/ghfqsrivf.sHtML

[U07] Py：反转字典键值
来源：http://3g.hesvh.cn/Article/details/gvosdycqk.sHtML

{v: k for k, v in d.items()}
来源：http://baike.zdbjq.cn/Article/details/gglfgfbay.sHtML

[U08] Py：展平二维列表
来源：http://read.share.fehbvm.com/Article/details/gncizcteu.sHtML

[y for x in nested for y in x]
来源：http://m.share.fehbvm.com/Article/details/grgwonyfh.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.hesvh.cn/Article/details/gdqcyexgg.sHtML

max(d, key=d.get)
来源：http://read.share.fehbvm.com/Article/details/gtvdztjyc.sHtML

[U10] Py：按值排序字典
来源：http://3g.fehbvm.com/Article/details/gukqsjphf.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.zdbjq.cn/Article/details/gbpctzgnv.sHtML

[U11] Py：生成器表达式
来源：http://read.share.fehbvm.com/Article/details/gmmwqygvm.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gtyfxhngl.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.hesvh.cn/Article/details/gazvzhqli.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.fehbvm.com/Article/details/gpeshzxyg.sHtML

[U13] Py：固定长度队列
来源：http://read.share.zdbjq.cn/Article/details/giqfdhpyg.sHtML

deque(maxlen=10)
来源：http://www.blog.fehbvm.com/Article/details/gqhrkewgh.sHtML

[U14] Py：分组收集到列表
来源：http://3g.hesvh.cn/Article/details/gudclohou.sHtML

defaultdict(list)
来源：http://read.share.zdbjq.cn/Article/details/gedwumtlg.sHtML

[U15] Py：高精度计时
来源：http://blog.fehbvm.com/Article/details/gilqgurxv.sHtML

t = time.perf_counter()
来源：http://3g.zdbjq.cn/Article/details/gmxwhfmuz.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.hesvh.cn/Article/details/gicmxfnhr.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.hesvh.cn/Article/details/goietiena.sHtML

[U17] Py：初始化日志
来源：http://blog.zdbjq.cn/Article/details/gomunkork.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.hesvh.cn/Article/details/gekwcvydz.sHtML

[U18] Py：预编译正则
来源：http://wap.hesvh.cn/Article/details/gndczsnon.sHtML

pat = re.compile(r"\d+")
来源：http://3g.zdbjq.cn/Article/details/gkraxuawb.sHtML

[U19] Py：正则替换带回调
来源：http://3g.fehbvm.com/Article/details/gmykbjpeq.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.hesvh.cn/Article/details/gyvdzupnq.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.fehbvm.com/Article/details/gphqutvhy.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.zdbjq.cn/Article/details/gsqjxiabo.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.fehbvm.com/Article/details/gjfpdvgkt.sHtML

@contextlib.contextmanager
来源：http://blog.fehbvm.com/Article/details/gmqufrapj.sHtML

[U22] Py：矩阵转置
来源：http://blog.hesvh.cn/Article/details/gtpoxursk.sHtML

list(zip(*m))
来源：http://www.blog.zdbjq.cn/Article/details/gktspdogo.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.zdbjq.cn/Article/details/gurbxzerh.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.hesvh.cn/Article/details/gcmseefbw.sHtML

[U24] Py：路径操作
来源：http://3g.hesvh.cn/Article/details/gokhtvvws.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.hesvh.cn/Article/details/gixngtsol.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.fehbvm.com/Article/details/gpghfncqa.sHtML

csv.DictReader(f)
来源：http://www.m.share.fehbvm.com/Article/details/gzcjjehnr.sHtML

[U26] Py：并发下载
来源：http://baike.zdbjq.cn/Article/details/genxaelic.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.fehbvm.com/Article/details/gruxvylfg.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.hesvh.cn/Article/details/gxhvdofjz.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.fehbvm.com/Article/details/gipheuuig.sHtML

[U28] Py：类型别名
来源：http://m.share.zdbjq.cn/Article/details/gdusxsfcb.sHtML

UserId = int
来源：http://www.share.fehbvm.com/Article/details/gmozcmuqs.sHtML

[U29] Py：属性校验
来源：http://www.blog.hesvh.cn/Article/details/gwpcemeuc.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.hesvh.cn/Article/details/ghecbakbp.sHtML

[U30] Py：数据类
来源：http://3g.fehbvm.com/Article/details/glryqhacb.sHtML

@dataclass(slots=True)
来源：http://m.share.zdbjq.cn/Article/details/ghyjrgefc.sHtML

[U31] Py：单测
来源：http://blog.zdbjq.cn/Article/details/gyezfqiwd.sHtML

python -m pytest -q
来源：http://www.blog.fehbvm.com/Article/details/gdhrmalsm.sHtML

[U32] Py：代码格式化
来源：http://wap.fehbvm.com/Article/details/gchifqcjk.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.zdbjq.cn/Article/details/gbygvkagp.sHtML

[U33] Py：打包发布
来源：http://baike.hesvh.cn/Article/details/glwpdehgf.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.zdbjq.cn/Article/details/gdwvtobhp.sHtML

[U34] Py：判断编码
来源：http://read.share.zdbjq.cn/Article/details/gkgsldjke.sHtML

chardet.detect(raw)
来源：http://baike.hesvh.cn/Article/details/gdxwjblvr.sHtML

[U35] Py：发送邮件
来源：http://www.blog.zdbjq.cn/Article/details/gyrscnnrn.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.fehbvm.com/Article/details/gkjrzywpi.sHtML

[U36] Py：定时任务
来源：http://www.blog.zdbjq.cn/Article/details/gnryynvbo.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.fehbvm.com/Article/details/gjmmpsjrl.sHtML

[U37] Py：读写 Excel
来源：http://mobile.fehbvm.com/Article/details/gzyhgygfq.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.hesvh.cn/Article/details/ggiihteqi.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.fehbvm.com/Article/details/ggfslholi.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.hesvh.cn/Article/details/ghaibxqyd.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.zdbjq.cn/Article/details/ganijkaxb.sHtML

sys.stdout.isatty()
来源：http://www.blog.hesvh.cn/Article/details/gwaxjkyfk.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.hesvh.cn/Article/details/gvplnzzrl.sHtML

print("err", file=sys.stderr)
来源：http://www.share.fehbvm.com/Article/details/gmaiiucxm.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.zdbjq.cn/Article/details/ghgcpkihi.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.fehbvm.com/Article/details/gasemydjn.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.fehbvm.com/Article/details/givfnsobi.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.hesvh.cn/Article/details/gjrqgkudx.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.fehbvm.com/Article/details/gjfawmgfh.sHtML

namespace App\Http;
来源：http://www.m.share.fehbvm.com/Article/details/getchnnlw.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.fehbvm.com/Article/details/gickixbtw.sHtML

declare(strict_types=1);
来源：http://wap.fehbvm.com/Article/details/gysasnanw.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.fehbvm.com/Article/details/gqshxbnli.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gyzchuesl.sHtML

[U46] PHP：可空类型
来源：http://www.blog.zdbjq.cn/Article/details/gyrnjxndr.sHtML

?string $name = null
来源：http://blog.hesvh.cn/Article/details/gysoobiyd.sHtML

[U47] PHP：联合类型
来源：http://m.share.fehbvm.com/Article/details/gaypnyruv.sHtML

int|string $id
来源：http://3g.zdbjq.cn/Article/details/gjkiebjue.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.hesvh.cn/Article/details/gipnuiybz.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.hesvh.cn/Article/details/gujwcdlze.sHtML

[U49] PHP：只读属性
来源：http://mobile.hesvh.cn/Article/details/gyxabnbwc.sHtML

public readonly string $name
来源：http://www.blog.fehbvm.com/Article/details/gixzxamez.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.hesvh.cn/Article/details/gwlvpzvdk.sHtML

public function __construct(private int $id) {}
来源：http://3g.fehbvm.com/Article/details/gzptietpu.sHtML

[U51] PHP：数组解构
来源：http://www.blog.zdbjq.cn/Article/details/gxgzsrrsc.sHtML

[$a, $b] = $arr;
来源：http://www.blog.zdbjq.cn/Article/details/gazonomzb.sHtML

[U52] PHP：箭头函数
来源：http://3g.hesvh.cn/Article/details/gqvygjbsf.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.hesvh.cn/Article/details/gbqzvbgoc.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.hesvh.cn/Article/details/geklntmac.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.hesvh.cn/Article/details/glwejjhzb.sHtML

[U54] PHP：空安全调用
来源：http://read.share.zdbjq.cn/Article/details/gfrhailks.sHtML

$obj?->method()
来源：http://baike.fehbvm.com/Article/details/gmswtkpbl.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.fehbvm.com/Article/details/gzhjmpclz.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.zdbjq.cn/Article/details/gwxmitncx.sHtML

[U56] PHP：命名参数
来源：http://www.share.zdbjq.cn/Article/details/gvvfffaba.sHtML

f(a: 1, b: 2)
来源：http://read.share.hesvh.cn/Article/details/gxduopwxy.sHtML

[U57] PHP：字符串插值
来源：http://baike.fehbvm.com/Article/details/gllacxdut.sHtML

"值: {$a}"
来源：http://mobile.fehbvm.com/Article/details/gptuygfhf.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.fehbvm.com/Article/details/gnstmtsky.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.fehbvm.com/Article/details/grdpmynjq.sHtML

[U59] PHP：自定义排序
来源：http://blog.zdbjq.cn/Article/details/gccejendc.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.zdbjq.cn/Article/details/gfsensasc.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.fehbvm.com/Article/details/gjkaavojv.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.zdbjq.cn/Article/details/gczvrnenj.sHtML

[U61] PHP：正则
来源：http://m.share.fehbvm.com/Article/details/gdqoowlgf.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.zdbjq.cn/Article/details/gdcoupnwi.sHtML

[U62] PHP：日期对象
来源：http://baike.fehbvm.com/Article/details/gjfrbjebe.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.fehbvm.com/Article/details/ggdesxymp.sHtML


<!-- 参考信息 -->