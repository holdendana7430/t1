代发 wailian999

[S41] C++：类与构造函数
来源：http://m.share.fehbvm.com/Article/details/ghzdezmzw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.zdbjq.cn/Article/details/gheevfsxz.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fehbvm.com/Article/details/gpwapqazl.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.zdbjq.cn/Article/details/gtdxcjwah.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fehbvm.com/Article/details/gjkpgrpyc.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fehbvm.com/Article/details/gzschcfhq.sHtML

[S44] C++：引用传参
来源：http://mobile.hesvh.cn/Article/details/gvhjvuuyz.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.zdbjq.cn/Article/details/gyhlhztag.sHtML

[S45] C++：lambda
来源：http://blog.zdbjq.cn/Article/details/gbmeneoye.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fehbvm.com/Article/details/gllcxtwcl.sHtML

[S46] C++：函数模板
来源：http://www.share.fehbvm.com/Article/details/gltejupkk.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fehbvm.com/Article/details/grzhaglro.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.hesvh.cn/Article/details/gajxncakh.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtsmpixbl.sHtML

[S48] C++：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gsnmkdytf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.zdbjq.cn/Article/details/golahizpb.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fehbvm.com/Article/details/gqkjwbqrt.sHtML

[S49] C++：写文件
来源：http://www.share.hesvh.cn/Article/details/gohitrakz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fehbvm.com/Article/details/gpmiutrvn.sHtML

[S50] C++：格式化数字
来源：http://read.share.hesvh.cn/Article/details/gbgsucqwv.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.hesvh.cn/Article/details/gqfophgop.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fehbvm.com/Article/details/gxgwmoosm.sHtML

static_cast<double>(a) / b
来源：http://baike.zdbjq.cn/Article/details/guilzlkfh.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fehbvm.com/Article/details/gaoqvopym.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.zdbjq.cn/Article/details/gyrhwsida.sHtML

[S53] C++：移动语义
来源：http://www.share.zdbjq.cn/Article/details/ghqkmelld.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fehbvm.com/Article/details/gubuvqagj.sHtML

[S54] C++：异常处理
来源：http://3g.hesvh.cn/Article/details/gueopippw.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.zdbjq.cn/Article/details/gaohgnwkr.sHtML

[S55] C++：结构化绑定
来源：http://3g.hesvh.cn/Article/details/gaegqcpxq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.zdbjq.cn/Article/details/gcxdyfpti.sHtML

[S56] C++：optional
来源：http://blog.hesvh.cn/Article/details/ggrjuvhwp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.zdbjq.cn/Article/details/gytlncumm.sHtML

[S57] C++：编译期常量
来源：http://www.blog.zdbjq.cn/Article/details/gwxczksey.sHtML

constexpr int N = 10;
来源：http://m.share.hesvh.cn/Article/details/goqdzcfra.sHtML

[S58] C++：命名空间
来源：http://www.share.fehbvm.com/Article/details/gfcpuprgz.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gdmdwlstn.sHtML

[S59] C++：静态断言
来源：http://3g.fehbvm.com/Article/details/gblkoxlek.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fehbvm.com/Article/details/gtvlxgcit.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.zdbjq.cn/Article/details/gqoghrkmq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.hesvh.cn/Article/details/gmjyuhxks.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gpwyscusx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fehbvm.com/Article/details/gnocdffij.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/govayahyb.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.hesvh.cn/Article/details/grekkxkcl.sHtML

println("Hello")
来源：http://www.share.hesvh.cn/Article/details/giluzegsu.sHtML

[T02] Kotlin：变量
来源：http://m.share.zdbjq.cn/Article/details/gheqrsjcc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.zdbjq.cn/Article/details/gnsrgxuzf.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fehbvm.com/Article/details/gbnxagtyd.sHtML

"值: $b"
来源：http://baike.zdbjq.cn/Article/details/gifutfezt.sHtML

[T04] Kotlin：空安全
来源：http://wap.zdbjq.cn/Article/details/gzpotemjc.sHtML

val n: String? = null;  n?.length
来源：http://blog.fehbvm.com/Article/details/grdrnydhh.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.zdbjq.cn/Article/details/gbzrsgexz.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fehbvm.com/Article/details/gfyzfpqap.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fehbvm.com/Article/details/guzgzkebh.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.zdbjq.cn/Article/details/gggsccste.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.zdbjq.cn/Article/details/ghhjvtlpo.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.zdbjq.cn/Article/details/gjugfthue.sHtML

[T08] Kotlin：数据类
来源：http://wap.fehbvm.com/Article/details/grocvnjto.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.zdbjq.cn/Article/details/gikkxuejt.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.hesvh.cn/Article/details/gfapeecmi.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fehbvm.com/Article/details/ggpnbgtei.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fehbvm.com/Article/details/gtdajmizv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fehbvm.com/Article/details/gupswfzdo.sHtML

[T11] Kotlin：协程
来源：http://wap.fehbvm.com/Article/details/grvhbgiwd.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fehbvm.com/Article/details/gbasaemth.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.hesvh.cn/Article/details/geoziurkv.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fehbvm.com/Article/details/gpxqdvisq.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fehbvm.com/Article/details/gahjpuhzc.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gnzbsggur.sHtML

[T14] Kotlin：循环
来源：http://www.share.hesvh.cn/Article/details/grnanfmnx.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.zdbjq.cn/Article/details/gegzwzeao.sHtML

[T15] Kotlin：接口
来源：http://read.share.zdbjq.cn/Article/details/gtloqwate.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fehbvm.com/Article/details/gvrbbfbnu.sHtML

[T16] Swift：Hello World
来源：http://www.share.hesvh.cn/Article/details/giofmyqdz.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/gjiluxgno.sHtML

[T17] Swift：变量与常量
来源：http://baike.zdbjq.cn/Article/details/gefoxodsh.sHtML

var a = 1;  let b = 2
来源：http://read.share.fehbvm.com/Article/details/gsottffjm.sHtML

[T18] Swift：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gdmjdpmpc.sHtML

"值: \(b)"
来源：http://mobile.hesvh.cn/Article/details/ghsbcnijs.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fehbvm.com/Article/details/ggkmgwqfs.sHtML

if let n = opt { print(n) }
来源：http://baike.hesvh.cn/Article/details/ggygosaet.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.fehbvm.com/Article/details/gburqrepy.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.hesvh.cn/Article/details/grbxxtwhf.sHtML

[T21] Swift：遍历
来源：http://wap.zdbjq.cn/Article/details/gvjzkanav.sHtML

for x in a { print(x) }
来源：http://www.share.zdbjq.cn/Article/details/gietfmvhm.sHtML

[T22] Swift：字典
来源：http://www.m.share.zdbjq.cn/Article/details/gdlehockp.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fehbvm.com/Article/details/gdofvxemd.sHtML

[T23] Swift：函数
来源：http://baike.hesvh.cn/Article/details/gipkocvww.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.hesvh.cn/Article/details/givadurvm.sHtML

[T24] Swift：闭包
来源：http://baike.zdbjq.cn/Article/details/gnzkehyoa.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.fehbvm.com/Article/details/gcrqqkxnw.sHtML

[T25] Swift：结构体
来源：http://blog.hesvh.cn/Article/details/gxcemmszf.sHtML

struct P { var x: Int }
来源：http://blog.fehbvm.com/Article/details/gdybtqfkm.sHtML

[T26] Swift：类与重写
来源：http://www.share.hesvh.cn/Article/details/gwxyotfwq.sHtML

class A: Base { override func f() {} }
来源：http://mobile.zdbjq.cn/Article/details/gtdjjyyot.sHtML

[T27] Swift：错误处理
来源：http://read.share.fehbvm.com/Article/details/gftnphywh.sHtML

do { try f() } catch { print(error) }
来源：http://baike.hesvh.cn/Article/details/gehdbxxkp.sHtML

[T28] Swift：枚举
来源：http://www.blog.hesvh.cn/Article/details/gtfteaiki.sHtML

enum Color { case red, green }
来源：http://wap.zdbjq.cn/Article/details/ghwppxktq.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.zdbjq.cn/Article/details/gvyobkxso.sHtML

guard let x = opt else { return }
来源：http://wap.fehbvm.com/Article/details/gskxwbars.sHtML

[T30] Swift：协议
来源：http://www.blog.fehbvm.com/Article/details/gyyhyxeti.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.zdbjq.cn/Article/details/gcygfrnrt.sHtML

[T31] Lua：Hello World
来源：http://www.blog.hesvh.cn/Article/details/goluosygw.sHtML

print("Hello")
来源：http://read.share.hesvh.cn/Article/details/gehvyfyiz.sHtML

[T32] Lua：局部变量
来源：http://3g.zdbjq.cn/Article/details/gsljhwbto.sHtML

local a = 1
来源：http://baike.fehbvm.com/Article/details/gpvvjiabv.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.hesvh.cn/Article/details/ggaozrefy.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.zdbjq.cn/Article/details/gjdemzelm.sHtML

[T34] Lua：遍历表
来源：http://m.share.fehbvm.com/Article/details/gvpdiiizg.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.hesvh.cn/Article/details/gklcqyssz.sHtML

[T35] Lua：字典表
来源：http://blog.zdbjq.cn/Article/details/giyoxknat.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.fehbvm.com/Article/details/gsauygjhd.sHtML

[T36] Lua：函数
来源：http://mobile.fehbvm.com/Article/details/gagmilcvn.sHtML

function add(a, b) return a + b end
来源：http://read.share.fehbvm.com/Article/details/geafpeiyf.sHtML

[T37] Lua：字符串拼接
来源：http://3g.fehbvm.com/Article/details/gibfvfddx.sHtML

"a" .. "b"
来源：http://read.share.fehbvm.com/Article/details/gcvdhwzkh.sHtML

[T38] Lua：条件
来源：http://www.blog.hesvh.cn/Article/details/gctxmnszi.sHtML

if x > 0 then print("正") end
来源：http://3g.hesvh.cn/Article/details/gpwcmqdgm.sHtML

[T39] Lua：模式匹配
来源：http://read.share.hesvh.cn/Article/details/gzvmzxkwm.sHtML

string.find(s, "%d+")
来源：http://m.share.fehbvm.com/Article/details/gxjrgtzeb.sHtML

[T40] Lua：元表
来源：http://read.share.zdbjq.cn/Article/details/gdzcraqlf.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.fehbvm.com/Article/details/ggvjkoqaa.sHtML

[T41] Perl：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gztqegvhb.sHtML

print "Hello\n";
来源：http://www.blog.zdbjq.cn/Article/details/gtvcalqts.sHtML

[T42] Perl：变量类型
来源：http://m.share.hesvh.cn/Article/details/gszfkjzrd.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.zdbjq.cn/Article/details/gvhscyevw.sHtML

[T43] Perl：字符串插值
来源：http://baike.zdbjq.cn/Article/details/glskofrdx.sHtML

"值: $a"
来源：http://read.share.hesvh.cn/Article/details/gvkmxhuoc.sHtML

[T44] Perl：条件
来源：http://www.blog.zdbjq.cn/Article/details/gsbvtcvlo.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.fehbvm.com/Article/details/gsghrurrb.sHtML

[T45] Perl：数组遍历
来源：http://baike.fehbvm.com/Article/details/gmfqhxlip.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.zdbjq.cn/Article/details/gucwjdpmq.sHtML

[T46] Perl：哈希操作
来源：http://www.share.zdbjq.cn/Article/details/grdosnvvy.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.zdbjq.cn/Article/details/gndkesniw.sHtML

[T47] Perl：正则捕获
来源：http://wap.fehbvm.com/Article/details/gsomcjodt.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.hesvh.cn/Article/details/gdotauktq.sHtML

[T48] Perl：正则替换
来源：http://3g.zdbjq.cn/Article/details/gspkxeeic.sHtML

$s =~ s/old/new/g;
来源：http://www.share.zdbjq.cn/Article/details/gojcvdrzk.sHtML

[T49] Perl：函数
来源：http://blog.zdbjq.cn/Article/details/gyesublsw.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/grjppjvvv.sHtML

[T50] Perl：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gudszxlzw.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.hesvh.cn/Article/details/grvuhwdzz.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.fehbvm.com/Article/details/grbizdowv.sHtML

[T51] Scala：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gyalokqxs.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/gqdatighi.sHtML

[T52] Scala：变量
来源：http://m.share.hesvh.cn/Article/details/guxblvvan.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gamxizwsp.sHtML

[T53] Scala：字符串插值
来源：http://baike.hesvh.cn/Article/details/grxnvtydr.sHtML

s"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/gumsjnjlc.sHtML

[T54] Scala：集合映射
来源：http://mobile.fehbvm.com/Article/details/gohcvagma.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.fehbvm.com/Article/details/gkkenlbpe.sHtML

[T55] Scala：集合过滤
来源：http://read.share.zdbjq.cn/Article/details/gcbrxwmjk.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.fehbvm.com/Article/details/gsfgdxvvl.sHtML

[T56] Scala：样例类
来源：http://baike.fehbvm.com/Article/details/gzpaxjxwr.sHtML

case class User(name: String, age: Int)
来源：http://3g.zdbjq.cn/Article/details/gbukwurxe.sHtML

[T57] Scala：模式匹配
来源：http://mobile.hesvh.cn/Article/details/gfywmoybu.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.hesvh.cn/Article/details/gmywwxhjp.sHtML

[T58] Scala：函数定义
来源：http://baike.hesvh.cn/Article/details/gpnyuhrxw.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.hesvh.cn/Article/details/ghokiurre.sHtML

[T59] Scala：循环
来源：http://mobile.hesvh.cn/Article/details/glfmbmtgg.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.zdbjq.cn/Article/details/gvbrszzbr.sHtML

[T60] Scala：折叠
来源：http://www.share.zdbjq.cn/Article/details/grdsuilwv.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.hesvh.cn/Article/details/gskqawpqc.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gsxpfycnz.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.hesvh.cn/Article/details/guneaxbwv.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/grcroiqad.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.hesvh.cn/Article/details/glvlsdyws.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.fehbvm.com/Article/details/gmxuutcnq.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.zdbjq.cn/Article/details/gkbjgdqiu.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.zdbjq.cn/Article/details/glsgtauyl.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.fehbvm.com/Article/details/gbueamblx.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.zdbjq.cn/Article/details/gbnadlezk.sHtML

[U04] Py：变量调试打印
来源：http://m.share.fehbvm.com/Article/details/gjpahogyg.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.zdbjq.cn/Article/details/gqazbklyk.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.zdbjq.cn/Article/details/gmixhugci.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.fehbvm.com/Article/details/gziyrivve.sHtML

[U06] Py：合并两个字典
来源：http://blog.fehbvm.com/Article/details/gspkyphnj.sHtML

{**a, **b}
来源：http://www.share.fehbvm.com/Article/details/gwyrbhmon.sHtML

[U07] Py：反转字典键值
来源：http://read.share.zdbjq.cn/Article/details/gcmhkehxl.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.fehbvm.com/Article/details/geozmridv.sHtML

[U08] Py：展平二维列表
来源：http://3g.zdbjq.cn/Article/details/gtqekrarb.sHtML

[y for x in nested for y in x]
来源：http://www.blog.fehbvm.com/Article/details/gaollnjex.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.hesvh.cn/Article/details/gddfyfqqi.sHtML

max(d, key=d.get)
来源：http://baike.fehbvm.com/Article/details/gichvnugg.sHtML

[U10] Py：按值排序字典
来源：http://wap.zdbjq.cn/Article/details/gejiulevo.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.fehbvm.com/Article/details/gwclaodeo.sHtML

[U11] Py：生成器表达式
来源：http://wap.zdbjq.cn/Article/details/grnnmlpdk.sHtML

(x * 2 for x in arr)
来源：http://baike.hesvh.cn/Article/details/gzwjqvipc.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.fehbvm.com/Article/details/gznkohdby.sHtML

Counter(arr).most_common(3)
来源：http://wap.hesvh.cn/Article/details/gldpkogqe.sHtML

[U13] Py：固定长度队列
来源：http://mobile.zdbjq.cn/Article/details/gybasszdd.sHtML

deque(maxlen=10)
来源：http://www.share.hesvh.cn/Article/details/gnuxmxtev.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.zdbjq.cn/Article/details/gkfdqxsju.sHtML

defaultdict(list)
来源：http://3g.zdbjq.cn/Article/details/gappcsuuf.sHtML

[U15] Py：高精度计时
来源：http://www.share.hesvh.cn/Article/details/gulkckbsa.sHtML

t = time.perf_counter()
来源：http://baike.zdbjq.cn/Article/details/gsmxgnvrj.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.fehbvm.com/Article/details/gbjjojxjg.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.fehbvm.com/Article/details/gesibeayk.sHtML

[U17] Py：初始化日志
来源：http://www.blog.hesvh.cn/Article/details/gwrbxwkvd.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.zdbjq.cn/Article/details/gwjaoippn.sHtML

[U18] Py：预编译正则
来源：http://m.share.zdbjq.cn/Article/details/gwixfyndl.sHtML

pat = re.compile(r"\d+")
来源：http://blog.fehbvm.com/Article/details/gtyqbqmql.sHtML

[U19] Py：正则替换带回调
来源：http://wap.zdbjq.cn/Article/details/gtynjqrjr.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.hesvh.cn/Article/details/gbgdsehbu.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.zdbjq.cn/Article/details/gvfvnwxfe.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.zdbjq.cn/Article/details/gqepsqyzc.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.zdbjq.cn/Article/details/gtildflkp.sHtML

@contextlib.contextmanager
来源：http://3g.zdbjq.cn/Article/details/gwkhqqmcz.sHtML

[U22] Py：矩阵转置
来源：http://baike.hesvh.cn/Article/details/gqdvdwugg.sHtML

list(zip(*m))
来源：http://3g.zdbjq.cn/Article/details/guixdautw.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.zdbjq.cn/Article/details/grzcksvwl.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.fehbvm.com/Article/details/gsxwudnwn.sHtML

[U24] Py：路径操作
来源：http://m.share.zdbjq.cn/Article/details/gsmdgkwcz.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.hesvh.cn/Article/details/gclgbqonp.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.fehbvm.com/Article/details/gypluyexy.sHtML

csv.DictReader(f)
来源：http://www.m.share.hesvh.cn/Article/details/gwngihwqu.sHtML

[U26] Py：并发下载
来源：http://blog.zdbjq.cn/Article/details/gqzceoidk.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.hesvh.cn/Article/details/gewgeigox.sHtML

[U27] Py：异步 HTTP
来源：http://wap.fehbvm.com/Article/details/gvlicqhfh.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.hesvh.cn/Article/details/gzhktyorc.sHtML

[U28] Py：类型别名
来源：http://read.share.fehbvm.com/Article/details/gvezomido.sHtML

UserId = int
来源：http://read.share.fehbvm.com/Article/details/gpblfevfz.sHtML

[U29] Py：属性校验
来源：http://3g.fehbvm.com/Article/details/gvmqzjvwg.sHtML

@property 与 @x.setter 配合
来源：http://www.share.hesvh.cn/Article/details/gyfpthqfz.sHtML

[U30] Py：数据类
来源：http://3g.zdbjq.cn/Article/details/gdefmxpny.sHtML

@dataclass(slots=True)
来源：http://m.share.hesvh.cn/Article/details/ghocbszoz.sHtML

[U31] Py：单测
来源：http://read.share.fehbvm.com/Article/details/girepbfqw.sHtML

python -m pytest -q
来源：http://www.m.share.fehbvm.com/Article/details/gnsfzkmxm.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gzdktgesz.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.zdbjq.cn/Article/details/gkbsfccvs.sHtML

[U33] Py：打包发布
来源：http://baike.hesvh.cn/Article/details/gbdmyesrk.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.zdbjq.cn/Article/details/gmcblrrcm.sHtML

[U34] Py：判断编码
来源：http://wap.fehbvm.com/Article/details/gkshhbgoh.sHtML

chardet.detect(raw)
来源：http://read.share.fehbvm.com/Article/details/gtnkkrjuf.sHtML

[U35] Py：发送邮件
来源：http://read.share.fehbvm.com/Article/details/gnbcviuzh.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.fehbvm.com/Article/details/gadamwmgx.sHtML

[U36] Py：定时任务
来源：http://read.share.zdbjq.cn/Article/details/gxmxuxbvs.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.fehbvm.com/Article/details/gdfwjaeul.sHtML

[U37] Py：读写 Excel
来源：http://www.share.hesvh.cn/Article/details/gqvchrvsd.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.zdbjq.cn/Article/details/gyswzmddp.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.zdbjq.cn/Article/details/gpbaqbuyk.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.fehbvm.com/Article/details/gkxnxdqgg.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.fehbvm.com/Article/details/grjawgyfl.sHtML

sys.stdout.isatty()
来源：http://read.share.fehbvm.com/Article/details/gsrdzjzae.sHtML

[U40] Py：打印到标准错误
来源：http://baike.fehbvm.com/Article/details/gqmtnypzg.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.fehbvm.com/Article/details/goylrkfnf.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.fehbvm.com/Article/details/gadliytdl.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.hesvh.cn/Article/details/gvnwethbu.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.hesvh.cn/Article/details/gvrnhokle.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.fehbvm.com/Article/details/gctmazdmc.sHtML

[U43] PHP：声明命名空间
来源：http://3g.zdbjq.cn/Article/details/gofulhgfk.sHtML

namespace App\Http;
来源：http://m.share.zdbjq.cn/Article/details/gverqdaay.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.hesvh.cn/Article/details/giyhtogoi.sHtML

declare(strict_types=1);
来源：http://www.blog.fehbvm.com/Article/details/glqyoxxgj.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.zdbjq.cn/Article/details/gflezmvxx.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gntygwqpz.sHtML

[U46] PHP：可空类型
来源：http://www.blog.zdbjq.cn/Article/details/gkhkslvjt.sHtML

?string $name = null
来源：http://3g.zdbjq.cn/Article/details/gbdnwgofn.sHtML

[U47] PHP：联合类型
来源：http://www.share.hesvh.cn/Article/details/gobakfgwb.sHtML

int|string $id
来源：http://read.share.fehbvm.com/Article/details/gtsfecwio.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.fehbvm.com/Article/details/gpfclbwid.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.hesvh.cn/Article/details/gnlqsmnix.sHtML

[U49] PHP：只读属性
来源：http://read.share.hesvh.cn/Article/details/gbdstzcxz.sHtML

public readonly string $name
来源：http://blog.fehbvm.com/Article/details/gmzrzwieq.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.hesvh.cn/Article/details/giqjhmbye.sHtML

public function __construct(private int $id) {}
来源：http://3g.zdbjq.cn/Article/details/gmcohcayf.sHtML

[U51] PHP：数组解构
来源：http://wap.hesvh.cn/Article/details/gqcrmcqve.sHtML

[$a, $b] = $arr;
来源：http://blog.fehbvm.com/Article/details/ggjeqqqlj.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.fehbvm.com/Article/details/gibmxnood.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.fehbvm.com/Article/details/guqpyuzvw.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.fehbvm.com/Article/details/gbyjynymn.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.hesvh.cn/Article/details/gvghdsimp.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.hesvh.cn/Article/details/gkymsotbz.sHtML

$obj?->method()
来源：http://blog.zdbjq.cn/Article/details/gaoumylwz.sHtML

[U55] PHP：match 表达式
来源：http://3g.zdbjq.cn/Article/details/gqiupzlka.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.fehbvm.com/Article/details/gnhvsfkfw.sHtML

[U56] PHP：命名参数
来源：http://3g.zdbjq.cn/Article/details/gbyhttted.sHtML

f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/gisosdbak.sHtML

[U57] PHP：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gaybyhnrr.sHtML

"值: {$a}"
来源：http://blog.fehbvm.com/Article/details/gkdfchwla.sHtML

[U58] PHP：数组三件套
来源：http://mobile.hesvh.cn/Article/details/gzaqsrxpf.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.fehbvm.com/Article/details/gyzmblaju.sHtML

[U59] PHP：自定义排序
来源：http://mobile.fehbvm.com/Article/details/gvdtqyduw.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fehbvm.com/Article/details/gclhwzpoc.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.zdbjq.cn/Article/details/gehlpqckt.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.fehbvm.com/Article/details/gliczhtza.sHtML

[U61] PHP：正则
来源：http://3g.hesvh.cn/Article/details/gyqsyercn.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.fehbvm.com/Article/details/gmcfrpemj.sHtML

[U62] PHP：日期对象
来源：http://baike.zdbjq.cn/Article/details/gniwklvce.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.zdbjq.cn/Article/details/gnnxxqded.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.hesvh.cn/Article/details/gxovfuhfj.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.hesvh.cn/Article/details/gfjoczzdz.sHtML

[U64] PHP：目录遍历
来源：http://blog.zdbjq.cn/Article/details/ghfxjschs.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.zdbjq.cn/Article/details/grwvuwrmf.sHtML

[U65] PHP：会话
来源：http://wap.fehbvm.com/Article/details/ghwcpviqp.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gkvknmihw.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.zdbjq.cn/Article/details/gnvwnjyng.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.fehbvm.com/Article/details/gvfbdohxy.sHtML


<!-- 参考信息 -->