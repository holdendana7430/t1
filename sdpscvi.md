代发 wailian999

[S41] C++：类与构造函数
来源：http://m.share.fanxiaobao.xyz/Article/details/ggymxrndc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fanxiaobao.xyz/Article/details/gyoyuavtu.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gwrrzwchw.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmsujycpi.sHtML

[S43] C++：智能指针
来源：http://baike.fanxiaobao.xyz/Article/details/gzyrxmtxl.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjgszmttv.sHtML

[S44] C++：引用传参
来源：http://wap.fanxiaobao.xyz/Article/details/gezsinoog.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqqzyqsq.sHtML

[S45] C++：lambda
来源：http://baike.fanxiaobao.xyz/Article/details/gctudpbmp.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fanxiaobao.xyz/Article/details/gmrxofpvv.sHtML

[S46] C++：函数模板
来源：http://blog.fanxiaobao.xyz/Article/details/gwknwahyg.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzivevgkd.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gtzshxxei.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fanxiaobao.xyz/Article/details/geohmvbgm.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gkkbrffyr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fanxiaobao.xyz/Article/details/glqhtwpku.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcalexqzz.sHtML

[S49] C++：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gclulyvsz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fanxiaobao.xyz/Article/details/grzsllkak.sHtML

[S50] C++：格式化数字
来源：http://wap.fanxiaobao.xyz/Article/details/gzmqrutpg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gmrgvhrhi.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gjcozbbzg.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvjezjxdo.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fanxiaobao.xyz/Article/details/giissmiaa.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gyygtniyb.sHtML

[S53] C++：移动语义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gntkbcpww.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fanxiaobao.xyz/Article/details/gvwkfwjmb.sHtML

[S54] C++：异常处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gkuzrnvai.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gutiowhfc.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gtjapygaz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fanxiaobao.xyz/Article/details/gbsyrajly.sHtML

[S56] C++：optional
来源：http://baike.fanxiaobao.xyz/Article/details/gmsbqmocp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fanxiaobao.xyz/Article/details/gtyvovknt.sHtML

[S57] C++：编译期常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gglzoprcr.sHtML

constexpr int N = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzpaqprdj.sHtML

[S58] C++：命名空间
来源：http://m.share.fanxiaobao.xyz/Article/details/ggrykfsxr.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fanxiaobao.xyz/Article/details/ghtrhtefq.sHtML

[S59] C++：静态断言
来源：http://blog.fanxiaobao.xyz/Article/details/gcvmtyupl.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fanxiaobao.xyz/Article/details/gppfajlsa.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fanxiaobao.xyz/Article/details/grptscigd.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/geyckghkb.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/ggtblmqea.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fanxiaobao.xyz/Article/details/gepjmzlxr.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gvdyzaflt.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gwpkvybub.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsmxaerms.sHtML

[T02] Kotlin：变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gykhblvxf.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fanxiaobao.xyz/Article/details/gvoklplsh.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fanxiaobao.xyz/Article/details/gumflndzr.sHtML

"值: $b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gkbjgbyno.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gotwunjqr.sHtML

val n: String? = null;  n?.length
来源：http://blog.fanxiaobao.xyz/Article/details/gujzgrios.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gxaqmdxub.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/grobadtoa.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.fanxiaobao.xyz/Article/details/glrycapru.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gkxkvnvee.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gzssbppiu.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxqocygai.sHtML

[T08] Kotlin：数据类
来源：http://3g.fanxiaobao.xyz/Article/details/gqmhmbmrx.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/gaycqgura.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fanxiaobao.xyz/Article/details/gjrpufmrf.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fanxiaobao.xyz/Article/details/gvjkwyixh.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnzfqkxdf.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fanxiaobao.xyz/Article/details/gezgkvsgk.sHtML

[T11] Kotlin：协程
来源：http://wap.fanxiaobao.xyz/Article/details/gplhjdxvn.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fanxiaobao.xyz/Article/details/gzhduirzd.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fanxiaobao.xyz/Article/details/gxnziwiuu.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdgoktwjc.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fanxiaobao.xyz/Article/details/gsctqpheo.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxjpsinrp.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtetwjvoe.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gflvuygmi.sHtML

[T15] Kotlin：接口
来源：http://3g.fanxiaobao.xyz/Article/details/gkfyqmeod.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxmtozkut.sHtML

[T16] Swift：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gzyqgzwgk.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvlyqydry.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gsxgfaste.sHtML

var a = 1;  let b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gjipbhftj.sHtML

[T18] Swift：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gprfkldrq.sHtML

"值: \(b)"
来源：http://www.share.fanxiaobao.xyz/Article/details/geajkeohj.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdzmyxfob.sHtML

if let n = opt { print(n) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzxlsqcag.sHtML

[T20] Swift：数组操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gvtsjlwsq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggcbgwrfb.sHtML

[T21] Swift：遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/grxkbfwod.sHtML

for x in a { print(x) }
来源：http://wap.fanxiaobao.xyz/Article/details/gvrhqfcer.sHtML

[T22] Swift：字典
来源：http://mobile.fanxiaobao.xyz/Article/details/geznzdymc.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gspmxykie.sHtML

[T23] Swift：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnwtfnqub.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fanxiaobao.xyz/Article/details/gsfzahbld.sHtML

[T24] Swift：闭包
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtlmtxlai.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gcnmhqqyf.sHtML

[T25] Swift：结构体
来源：http://read.share.fanxiaobao.xyz/Article/details/gunrbpvtl.sHtML

struct P { var x: Int }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmacgbpcn.sHtML

[T26] Swift：类与重写
来源：http://read.share.fanxiaobao.xyz/Article/details/gzllkcdjl.sHtML

class A: Base { override func f() {} }
来源：http://3g.fanxiaobao.xyz/Article/details/gzdnxxbnk.sHtML

[T27] Swift：错误处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcaiwocot.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwrdlueoc.sHtML

[T28] Swift：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gewhqxvpp.sHtML

enum Color { case red, green }
来源：http://www.blog.fanxiaobao.xyz/Article/details/goatepija.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzpbbfkyg.sHtML

guard let x = opt else { return }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqpuaxvfu.sHtML

[T30] Swift：协议
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gomhcowjg.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxpgsxhcs.sHtML

[T31] Lua：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/geqbycxky.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gchqvibqc.sHtML

[T32] Lua：局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gqghmdzev.sHtML

local a = 1
来源：http://blog.fanxiaobao.xyz/Article/details/gtdbuzult.sHtML

[T33] Lua：表（数组）
来源：http://3g.fanxiaobao.xyz/Article/details/gtmmxxsbi.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.fanxiaobao.xyz/Article/details/gessqqsli.sHtML

[T34] Lua：遍历表
来源：http://m.share.fanxiaobao.xyz/Article/details/gjbekhjwf.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.fanxiaobao.xyz/Article/details/gosttfdls.sHtML

[T35] Lua：字典表
来源：http://www.share.fanxiaobao.xyz/Article/details/ghpercgyd.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/goiiwuvci.sHtML

[T36] Lua：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gunfzeybg.sHtML

function add(a, b) return a + b end
来源：http://baike.fanxiaobao.xyz/Article/details/gsexahzrh.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/ghtlsgfzv.sHtML

"a" .. "b"
来源：http://www.share.fanxiaobao.xyz/Article/details/ggjnhandb.sHtML

[T38] Lua：条件
来源：http://blog.fanxiaobao.xyz/Article/details/gwxrtrtgp.sHtML

if x > 0 then print("正") end
来源：http://wap.fanxiaobao.xyz/Article/details/guqnkccta.sHtML

[T39] Lua：模式匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gltktlqim.sHtML

string.find(s, "%d+")
来源：http://www.share.fanxiaobao.xyz/Article/details/gptnlscmw.sHtML

[T40] Lua：元表
来源：http://3g.fanxiaobao.xyz/Article/details/gnjnyzpym.sHtML

setmetatable({}, { __index = base })
来源：http://wap.fanxiaobao.xyz/Article/details/gxjvzpjwo.sHtML

[T41] Perl：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gbxnqpaos.sHtML

print "Hello\n";
来源：http://blog.fanxiaobao.xyz/Article/details/gjdeiywuc.sHtML

[T42] Perl：变量类型
来源：http://3g.fanxiaobao.xyz/Article/details/gojcrcpct.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.fanxiaobao.xyz/Article/details/gxcjglsjh.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfavzfmrh.sHtML

"值: $a"
来源：http://www.share.fanxiaobao.xyz/Article/details/grvkzvfcr.sHtML

[T44] Perl：条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gwkkrlrzd.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gdweoexmt.sHtML

[T45] Perl：数组遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gcaybfpmg.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghsojkhqk.sHtML

[T46] Perl：哈希操作
来源：http://baike.fanxiaobao.xyz/Article/details/gdljjuuik.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqfmnyhrq.sHtML

[T47] Perl：正则捕获
来源：http://read.share.fanxiaobao.xyz/Article/details/gnjsxvuwx.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guvcqlmpr.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grblijurd.sHtML

$s =~ s/old/new/g;
来源：http://www.share.fanxiaobao.xyz/Article/details/gsllqdfhq.sHtML

[T49] Perl：函数
来源：http://blog.fanxiaobao.xyz/Article/details/gvjvswurw.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfdfxbxsg.sHtML

[T50] Perl：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gxqzwfsub.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.fanxiaobao.xyz/Article/details/gqxrekfqb.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcqwtttjy.sHtML

[T51] Scala：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gslzzpvbm.sHtML

println("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gllhapogt.sHtML

[T52] Scala：变量
来源：http://wap.fanxiaobao.xyz/Article/details/gvrxhoorv.sHtML

val a = 1;  var b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/grvorcxfu.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gkfsrzcxe.sHtML

s"值: $b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gutsvsefj.sHtML

[T54] Scala：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/getpjputu.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gawjfnimn.sHtML

[T55] Scala：集合过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gzmrjfryt.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/glaooujud.sHtML

[T56] Scala：样例类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjaopgxvl.sHtML

case class User(name: String, age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/ghqvsadwr.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjtukqjvk.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gcvmrrwlt.sHtML

[T58] Scala：函数定义
来源：http://blog.fanxiaobao.xyz/Article/details/gfpptdanj.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.fanxiaobao.xyz/Article/details/gpogstpif.sHtML

[T59] Scala：循环
来源：http://wap.fanxiaobao.xyz/Article/details/gaenyypjj.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.fanxiaobao.xyz/Article/details/gxfhtqlbi.sHtML

[T60] Scala：折叠
来源：http://mobile.fanxiaobao.xyz/Article/details/gzhrtoqhn.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfkwuciks.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gilutjhab.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gqnehrxjm.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gycajptkz.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.fanxiaobao.xyz/Article/details/gopwvlhft.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.fanxiaobao.xyz/Article/details/gckgjuyzj.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gepeydgtt.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gfjmwkdho.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.fanxiaobao.xyz/Article/details/gbhethsck.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.fanxiaobao.xyz/Article/details/gfcszfbzy.sHtML

[U04] Py：变量调试打印
来源：http://m.share.fanxiaobao.xyz/Article/details/gbthzbrme.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.fanxiaobao.xyz/Article/details/gwagvgbok.sHtML

[U05] Py：列表去重且保序
来源：http://blog.fanxiaobao.xyz/Article/details/gknikqugt.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.fanxiaobao.xyz/Article/details/gtyuaklim.sHtML

[U06] Py：合并两个字典
来源：http://3g.fanxiaobao.xyz/Article/details/gqkxcbazw.sHtML

{**a, **b}
来源：http://m.share.fanxiaobao.xyz/Article/details/gnbkxhvfu.sHtML

[U07] Py：反转字典键值
来源：http://blog.fanxiaobao.xyz/Article/details/gehgiagos.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvuorkdmq.sHtML

[U08] Py：展平二维列表
来源：http://baike.fanxiaobao.xyz/Article/details/geiqonbah.sHtML

[y for x in nested for y in x]
来源：http://www.share.fanxiaobao.xyz/Article/details/gnyqtacsf.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.fanxiaobao.xyz/Article/details/gmfazkkgq.sHtML

max(d, key=d.get)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grmjdvtwh.sHtML

[U10] Py：按值排序字典
来源：http://m.share.fanxiaobao.xyz/Article/details/gystndufb.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.fanxiaobao.xyz/Article/details/gzzambvqd.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtmyrxlqf.sHtML

(x * 2 for x in arr)
来源：http://blog.fanxiaobao.xyz/Article/details/guhpzekfg.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.fanxiaobao.xyz/Article/details/gnqkqncww.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gidzpeyax.sHtML

[U13] Py：固定长度队列
来源：http://www.share.fanxiaobao.xyz/Article/details/gtwjtxkwt.sHtML

deque(maxlen=10)
来源：http://3g.fanxiaobao.xyz/Article/details/gjmwzxlhi.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggbzenimd.sHtML

defaultdict(list)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggaswniwv.sHtML

[U15] Py：高精度计时
来源：http://www.share.fanxiaobao.xyz/Article/details/gloooehfl.sHtML

t = time.perf_counter()
来源：http://mobile.fanxiaobao.xyz/Article/details/ghhxxtoqb.sHtML

[U16] Py：命令行参数解析
来源：http://wap.fanxiaobao.xyz/Article/details/gxrqwmkcq.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.fanxiaobao.xyz/Article/details/gpiegwwcd.sHtML

[U17] Py：初始化日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gwzxxmhcu.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glhyryuwx.sHtML

[U18] Py：预编译正则
来源：http://www.share.fanxiaobao.xyz/Article/details/guvqbniek.sHtML

pat = re.compile(r"\d+")
来源：http://blog.fanxiaobao.xyz/Article/details/gxpuwbwlq.sHtML

[U19] Py：正则替换带回调
来源：http://3g.fanxiaobao.xyz/Article/details/gjxzcannh.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.fanxiaobao.xyz/Article/details/gfjcmjfks.sHtML

[U20] Py：缓存函数结果
来源：http://3g.fanxiaobao.xyz/Article/details/gmhlzthlm.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghokauoqs.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geobrydoi.sHtML

@contextlib.contextmanager
来源：http://3g.fanxiaobao.xyz/Article/details/gwxxfxueg.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsilqrgjc.sHtML

list(zip(*m))
来源：http://wap.fanxiaobao.xyz/Article/details/gpmmhkvpt.sHtML

[U23] Py：分块读取大文件
来源：http://wap.fanxiaobao.xyz/Article/details/gaahhaffy.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.fanxiaobao.xyz/Article/details/ghcjbjmxc.sHtML

[U24] Py：路径操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gnbdmznly.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.fanxiaobao.xyz/Article/details/gwwvmwlxm.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.fanxiaobao.xyz/Article/details/gmdfurnvz.sHtML

csv.DictReader(f)
来源：http://blog.fanxiaobao.xyz/Article/details/gmihalfji.sHtML

[U26] Py：并发下载
来源：http://m.share.fanxiaobao.xyz/Article/details/gbnsgglve.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.fanxiaobao.xyz/Article/details/gytdrmkjm.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.fanxiaobao.xyz/Article/details/gnxlrzscl.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.fanxiaobao.xyz/Article/details/gasuphbri.sHtML

[U28] Py：类型别名
来源：http://mobile.fanxiaobao.xyz/Article/details/gthnyzqmi.sHtML

UserId = int
来源：http://3g.fanxiaobao.xyz/Article/details/gchpapmmc.sHtML

[U29] Py：属性校验
来源：http://www.share.fanxiaobao.xyz/Article/details/gkpylxdnt.sHtML

@property 与 @x.setter 配合
来源：http://3g.fanxiaobao.xyz/Article/details/gosmnxjbl.sHtML

[U30] Py：数据类
来源：http://baike.fanxiaobao.xyz/Article/details/gzuzaargc.sHtML

@dataclass(slots=True)
来源：http://baike.fanxiaobao.xyz/Article/details/gofiufwbg.sHtML

[U31] Py：单测
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyijazvyi.sHtML

python -m pytest -q
来源：http://m.share.fanxiaobao.xyz/Article/details/goqksdqzq.sHtML

[U32] Py：代码格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gkwdzpotg.sHtML

ruff format . && ruff check --fix .
来源：http://3g.fanxiaobao.xyz/Article/details/gkurjjnwd.sHtML

[U33] Py：打包发布
来源：http://3g.fanxiaobao.xyz/Article/details/govorfmvs.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkbfqlgxl.sHtML

[U34] Py：判断编码
来源：http://3g.fanxiaobao.xyz/Article/details/gqyhxiugb.sHtML

chardet.detect(raw)
来源：http://www.share.fanxiaobao.xyz/Article/details/gihprldgz.sHtML

[U35] Py：发送邮件
来源：http://m.share.fanxiaobao.xyz/Article/details/gekgomdbk.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.fanxiaobao.xyz/Article/details/gvlhxilcy.sHtML

[U36] Py：定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gbrvgoweg.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtjdeskkh.sHtML

[U37] Py：读写 Excel
来源：http://baike.fanxiaobao.xyz/Article/details/ghqqhikbg.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.fanxiaobao.xyz/Article/details/gcdtwibjj.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzzfjmwup.sHtML

Path(__file__).resolve().parent
来源：http://blog.fanxiaobao.xyz/Article/details/guosaqqwj.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.fanxiaobao.xyz/Article/details/gjgutnhyw.sHtML

sys.stdout.isatty()
来源：http://read.share.fanxiaobao.xyz/Article/details/gbxhfzlnq.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gjfiinsai.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkabijjbg.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.fanxiaobao.xyz/Article/details/gellwdznw.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.fanxiaobao.xyz/Article/details/gytkzjaqs.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtzxsiasi.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfqbjavvx.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.fanxiaobao.xyz/Article/details/gztvqpvvb.sHtML

namespace App\Http;
来源：http://baike.fanxiaobao.xyz/Article/details/gprdmzrgq.sHtML

[U44] PHP：开启严格类型
来源：http://3g.fanxiaobao.xyz/Article/details/ggpgyruau.sHtML

declare(strict_types=1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/govjpbbsx.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.fanxiaobao.xyz/Article/details/guxuldgac.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gvzgucrse.sHtML

[U46] PHP：可空类型
来源：http://read.share.fanxiaobao.xyz/Article/details/genpuuoeu.sHtML

?string $name = null
来源：http://blog.fanxiaobao.xyz/Article/details/gapklyiai.sHtML

[U47] PHP：联合类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyacjbchh.sHtML

int|string $id
来源：http://wap.fanxiaobao.xyz/Article/details/ghirvwwjm.sHtML

[U48] PHP：纯枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gclesbdls.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grzzapigb.sHtML

[U49] PHP：只读属性
来源：http://mobile.fanxiaobao.xyz/Article/details/gbrmovvam.sHtML

public readonly string $name
来源：http://blog.fanxiaobao.xyz/Article/details/ggppqngyk.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjawrtrrl.sHtML

public function __construct(private int $id) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gtmthiugn.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsqztvumr.sHtML

[$a, $b] = $arr;
来源：http://blog.fanxiaobao.xyz/Article/details/gjxdefdte.sHtML

[U52] PHP：箭头函数
来源：http://wap.fanxiaobao.xyz/Article/details/gdycoebzw.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpuuxdlaj.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.fanxiaobao.xyz/Article/details/gtazffwei.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvrmddipn.sHtML

[U54] PHP：空安全调用
来源：http://3g.fanxiaobao.xyz/Article/details/goioashje.sHtML

$obj?->method()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gruqrrwhu.sHtML

[U55] PHP：match 表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gdmgjwfuh.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.fanxiaobao.xyz/Article/details/goawmumbf.sHtML

[U56] PHP：命名参数
来源：http://baike.fanxiaobao.xyz/Article/details/gehukrqwc.sHtML

f(a: 1, b: 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/glawrnauk.sHtML

[U57] PHP：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gjuxmwbtc.sHtML

"值: {$a}"
来源：http://baike.fanxiaobao.xyz/Article/details/glyubqslx.sHtML

[U58] PHP：数组三件套
来源：http://m.share.fanxiaobao.xyz/Article/details/gbfdxcksj.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.fanxiaobao.xyz/Article/details/gqfhfmxzj.sHtML

[U59] PHP：自定义排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gjnmqouhz.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fanxiaobao.xyz/Article/details/gzubadjsg.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.fanxiaobao.xyz/Article/details/gkpihpqyh.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.fanxiaobao.xyz/Article/details/gvrywppxn.sHtML

[U61] PHP：正则
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glxhzdgsn.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fanxiaobao.xyz/Article/details/gccosnxff.sHtML

[U62] PHP：日期对象
来源：http://www.share.fanxiaobao.xyz/Article/details/gjgvddkkl.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggcjedlhl.sHtML

[U63] PHP：文件读写
来源：http://read.share.fanxiaobao.xyz/Article/details/gedsyvjey.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.fanxiaobao.xyz/Article/details/gerlcyusn.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnutmexja.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjpsapptp.sHtML

[U65] PHP：会话
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpojdfwxj.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gxdqtkbzb.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.fanxiaobao.xyz/Article/details/gukfsocjc.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gguuvsyiv.sHtML


<!-- 参考信息 -->