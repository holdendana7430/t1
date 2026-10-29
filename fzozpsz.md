代发 wailian999

[S43] C++：智能指针
来源：http://wap.zdbjq.cn/Article/details/gytqycxxu.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.zdbjq.cn/Article/details/gcmhnohfk.sHtML

[S44] C++：引用传参
来源：http://wap.hesvh.cn/Article/details/gxkmfyfon.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fehbvm.com/Article/details/gqgqjdsvd.sHtML

[S45] C++：lambda
来源：http://m.share.zdbjq.cn/Article/details/giddreiev.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.hesvh.cn/Article/details/gtnwyqaaf.sHtML

[S46] C++：函数模板
来源：http://m.share.fehbvm.com/Article/details/gixnmuetk.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fehbvm.com/Article/details/gpfhaslav.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.hesvh.cn/Article/details/gyfqgyvmn.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.hesvh.cn/Article/details/gdubnyhub.sHtML

[S48] C++：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gnspajtdy.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fehbvm.com/Article/details/gtnqfhoxc.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fehbvm.com/Article/details/gsawzkzqz.sHtML

[S49] C++：写文件
来源：http://www.share.fehbvm.com/Article/details/gmohdsbxa.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fehbvm.com/Article/details/ghyyrrqix.sHtML

[S50] C++：格式化数字
来源：http://wap.hesvh.cn/Article/details/gluyhpxyw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gpxqzkbhd.sHtML

[S51] C++：显式类型转换
来源：http://mobile.zdbjq.cn/Article/details/gldqdthzk.sHtML

static_cast<double>(a) / b
来源：http://m.share.hesvh.cn/Article/details/gaveaysqj.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fehbvm.com/Article/details/gzmxseqoi.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fehbvm.com/Article/details/gnxohwqwk.sHtML

[S53] C++：移动语义
来源：http://read.share.zdbjq.cn/Article/details/gevpwynjp.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.zdbjq.cn/Article/details/gzyyyybry.sHtML

[S54] C++：异常处理
来源：http://3g.zdbjq.cn/Article/details/gbrpbcrui.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.zdbjq.cn/Article/details/gfrqmpavz.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fehbvm.com/Article/details/gleypapne.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.hesvh.cn/Article/details/gsjtnxgaf.sHtML

[S56] C++：optional
来源：http://www.m.share.fehbvm.com/Article/details/gasznxgog.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fehbvm.com/Article/details/gisrihuta.sHtML

[S57] C++：编译期常量
来源：http://blog.hesvh.cn/Article/details/gvyntjjha.sHtML

constexpr int N = 10;
来源：http://blog.fehbvm.com/Article/details/gpowdjrym.sHtML

[S58] C++：命名空间
来源：http://3g.fehbvm.com/Article/details/guxuwmukt.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fehbvm.com/Article/details/grhseiilw.sHtML

[S59] C++：静态断言
来源：http://blog.zdbjq.cn/Article/details/gldfbqfkf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.hesvh.cn/Article/details/gjpgogqei.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.hesvh.cn/Article/details/gowvawiiz.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fehbvm.com/Article/details/guhlujukm.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gxdcjeufk.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.hesvh.cn/Article/details/goasngehc.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gqgbochgb.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fehbvm.com/Article/details/gfexznmje.sHtML

println("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/ghhhijtoo.sHtML

[T02] Kotlin：变量
来源：http://baike.fehbvm.com/Article/details/gbnzrbzgw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fehbvm.com/Article/details/gxfqqkpgg.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.hesvh.cn/Article/details/gmpiazcwk.sHtML

"值: $b"
来源：http://m.share.hesvh.cn/Article/details/gvlndjopj.sHtML

[T04] Kotlin：空安全
来源：http://wap.fehbvm.com/Article/details/guugkbqxb.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fehbvm.com/Article/details/giqlopsxs.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fehbvm.com/Article/details/garbcyoqw.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.zdbjq.cn/Article/details/gkrypuidl.sHtML

[T06] Kotlin：集合映射
来源：http://baike.hesvh.cn/Article/details/gtdsljpol.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fehbvm.com/Article/details/gpbjiuilw.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fehbvm.com/Article/details/glowwhaob.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.zdbjq.cn/Article/details/guddqigyy.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.zdbjq.cn/Article/details/gfokbubwu.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fehbvm.com/Article/details/gkdvqacip.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fehbvm.com/Article/details/gvjpsxofj.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fehbvm.com/Article/details/grczqaiwg.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.hesvh.cn/Article/details/gqagtnbls.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.hesvh.cn/Article/details/gxzrszzxo.sHtML

[T11] Kotlin：协程
来源：http://read.share.fehbvm.com/Article/details/gamomedju.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.hesvh.cn/Article/details/gsjyzqfrx.sHtML

[T12] Kotlin：解构声明
来源：http://wap.zdbjq.cn/Article/details/gvvzlygqd.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fehbvm.com/Article/details/gbelialjv.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.zdbjq.cn/Article/details/glpahfzfd.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.zdbjq.cn/Article/details/ggebaaoap.sHtML

[T14] Kotlin：循环
来源：http://wap.zdbjq.cn/Article/details/gtczkasqz.sHtML

for (i in 1..10) println(i)
来源：http://mobile.hesvh.cn/Article/details/gsfpsdszn.sHtML

[T15] Kotlin：接口
来源：http://read.share.fehbvm.com/Article/details/gooltoxqw.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.hesvh.cn/Article/details/gnjkybnua.sHtML

[T16] Swift：Hello World
来源：http://3g.fehbvm.com/Article/details/gjacftfcd.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/gucxaoyze.sHtML

[T17] Swift：变量与常量
来源：http://mobile.zdbjq.cn/Article/details/gbllqllgc.sHtML

var a = 1;  let b = 2
来源：http://baike.zdbjq.cn/Article/details/grsubjrqh.sHtML

[T18] Swift：字符串插值
来源：http://wap.hesvh.cn/Article/details/gqbebqdnp.sHtML

"值: \(b)"
来源：http://read.share.fehbvm.com/Article/details/guudanwoi.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fehbvm.com/Article/details/gngfymism.sHtML

if let n = opt { print(n) }
来源：http://3g.zdbjq.cn/Article/details/gtpxvhtzz.sHtML

[T20] Swift：数组操作
来源：http://m.share.hesvh.cn/Article/details/gwqdcffeb.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.zdbjq.cn/Article/details/gkdbnwtbh.sHtML

[T21] Swift：遍历
来源：http://m.share.hesvh.cn/Article/details/gitpocumy.sHtML

for x in a { print(x) }
来源：http://baike.fehbvm.com/Article/details/gbxsbsbek.sHtML

[T22] Swift：字典
来源：http://www.share.fehbvm.com/Article/details/gykkyudej.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fehbvm.com/Article/details/gdfurenay.sHtML

[T23] Swift：函数
来源：http://blog.zdbjq.cn/Article/details/gjoqeimwt.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.hesvh.cn/Article/details/gxnvtkzyw.sHtML

[T24] Swift：闭包
来源：http://mobile.zdbjq.cn/Article/details/gejqoseon.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gsqabilkt.sHtML

[T25] Swift：结构体
来源：http://www.blog.hesvh.cn/Article/details/gcxlyojmn.sHtML

struct P { var x: Int }
来源：http://www.m.share.hesvh.cn/Article/details/gtmkxhabd.sHtML

[T26] Swift：类与重写
来源：http://mobile.fehbvm.com/Article/details/gahwjwclq.sHtML

class A: Base { override func f() {} }
来源：http://m.share.hesvh.cn/Article/details/gaoiakczt.sHtML

[T27] Swift：错误处理
来源：http://www.share.fehbvm.com/Article/details/gbufbavmg.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.zdbjq.cn/Article/details/ggcqflbqn.sHtML

[T28] Swift：枚举
来源：http://m.share.zdbjq.cn/Article/details/gjpjhovav.sHtML

enum Color { case red, green }
来源：http://wap.fehbvm.com/Article/details/gwuzchnac.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.hesvh.cn/Article/details/gwgzeqzaj.sHtML

guard let x = opt else { return }
来源：http://www.m.share.zdbjq.cn/Article/details/gglfqybbx.sHtML

[T30] Swift：协议
来源：http://blog.hesvh.cn/Article/details/gyveomqvj.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.zdbjq.cn/Article/details/gnpsknfmr.sHtML

[T31] Lua：Hello World
来源：http://wap.zdbjq.cn/Article/details/gvnoucxdy.sHtML

print("Hello")
来源：http://blog.hesvh.cn/Article/details/ggjmuupnw.sHtML

[T32] Lua：局部变量
来源：http://read.share.hesvh.cn/Article/details/gmklvnbha.sHtML

local a = 1
来源：http://blog.hesvh.cn/Article/details/glbrlgguu.sHtML

[T33] Lua：表（数组）
来源：http://m.share.hesvh.cn/Article/details/glahbqmba.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.fehbvm.com/Article/details/genyawgbs.sHtML

[T34] Lua：遍历表
来源：http://www.share.hesvh.cn/Article/details/gohtjnude.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.zdbjq.cn/Article/details/gaekyvbku.sHtML

[T35] Lua：字典表
来源：http://mobile.zdbjq.cn/Article/details/gptbkdado.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fehbvm.com/Article/details/goksczwkl.sHtML

[T36] Lua：函数
来源：http://blog.zdbjq.cn/Article/details/gjqczbdrb.sHtML

function add(a, b) return a + b end
来源：http://www.share.hesvh.cn/Article/details/gmgazgrba.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.hesvh.cn/Article/details/gptcyuyvz.sHtML

"a" .. "b"
来源：http://baike.hesvh.cn/Article/details/gnlspgvoj.sHtML

[T38] Lua：条件
来源：http://baike.hesvh.cn/Article/details/gxtyxwdyr.sHtML

if x > 0 then print("正") end
来源：http://3g.hesvh.cn/Article/details/gnnqpuaxe.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.zdbjq.cn/Article/details/gasfgmrxn.sHtML

string.find(s, "%d+")
来源：http://read.share.hesvh.cn/Article/details/gjpwgidvq.sHtML

[T40] Lua：元表
来源：http://m.share.fehbvm.com/Article/details/gdvzlhyvv.sHtML

setmetatable({}, { __index = base })
来源：http://wap.fehbvm.com/Article/details/gixytfmad.sHtML

[T41] Perl：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gujalwyqt.sHtML

print "Hello\n";
来源：http://www.share.hesvh.cn/Article/details/gsufzhvqn.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.fehbvm.com/Article/details/gpvjkllzw.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.hesvh.cn/Article/details/gnzmgnbvj.sHtML

[T43] Perl：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gxfjryyfs.sHtML

"值: $a"
来源：http://www.share.zdbjq.cn/Article/details/gbcgiyngm.sHtML

[T44] Perl：条件
来源：http://blog.hesvh.cn/Article/details/gajtavzwv.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.fehbvm.com/Article/details/gnnjvcjbv.sHtML

[T45] Perl：数组遍历
来源：http://read.share.fehbvm.com/Article/details/gmfcsmyxy.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.zdbjq.cn/Article/details/gttbvbzsc.sHtML

[T46] Perl：哈希操作
来源：http://wap.hesvh.cn/Article/details/ggzxdqtpa.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.zdbjq.cn/Article/details/gslnjinrp.sHtML

[T47] Perl：正则捕获
来源：http://www.share.hesvh.cn/Article/details/gzjhgpgnk.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.hesvh.cn/Article/details/gahwemqcs.sHtML

[T48] Perl：正则替换
来源：http://blog.zdbjq.cn/Article/details/gvavudjjm.sHtML

$s =~ s/old/new/g;
来源：http://read.share.zdbjq.cn/Article/details/gsabewpdr.sHtML

[T49] Perl：函数
来源：http://read.share.hesvh.cn/Article/details/gvurmvgbr.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gyuxgzkhr.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gdvdnoqsi.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.fehbvm.com/Article/details/glkygsvda.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.hesvh.cn/Article/details/ggpefccqc.sHtML

[T51] Scala：Hello World
来源：http://blog.hesvh.cn/Article/details/gcpllqcdj.sHtML

println("Hello")
来源：http://wap.hesvh.cn/Article/details/ghhxqwwmn.sHtML

[T52] Scala：变量
来源：http://wap.fehbvm.com/Article/details/gynqzmrte.sHtML

val a = 1;  var b = 2
来源：http://baike.fehbvm.com/Article/details/gvlfkigmb.sHtML

[T53] Scala：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gkvuuqjfu.sHtML

s"值: $b"
来源：http://m.share.hesvh.cn/Article/details/gcqkwbnzm.sHtML

[T54] Scala：集合映射
来源：http://m.share.hesvh.cn/Article/details/gvrdfahga.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.fehbvm.com/Article/details/gotbdbals.sHtML

[T55] Scala：集合过滤
来源：http://wap.hesvh.cn/Article/details/gekkeofvx.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.hesvh.cn/Article/details/gldvviwdv.sHtML

[T56] Scala：样例类
来源：http://baike.fehbvm.com/Article/details/gbyixszsk.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.fehbvm.com/Article/details/gdzseblbe.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gvzsvmojr.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.zdbjq.cn/Article/details/gtkdatoke.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.hesvh.cn/Article/details/gvlfocqgk.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.zdbjq.cn/Article/details/goanzehen.sHtML

[T59] Scala：循环
来源：http://wap.zdbjq.cn/Article/details/gfrbbfvxo.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/gjgonznjo.sHtML

[T60] Scala：折叠
来源：http://wap.fehbvm.com/Article/details/grhsmksep.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.zdbjq.cn/Article/details/gmglhqkht.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ggmeiuvyy.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fehbvm.com/Article/details/gbokgoyvs.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gacsayxqb.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.fehbvm.com/Article/details/gweimxfin.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.hesvh.cn/Article/details/gydtcqcxv.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.zdbjq.cn/Article/details/gyiszrqez.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.zdbjq.cn/Article/details/gxiexggon.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.fehbvm.com/Article/details/gyzwetoxo.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.fehbvm.com/Article/details/gxnhhcyfz.sHtML

[U04] Py：变量调试打印
来源：http://m.share.hesvh.cn/Article/details/goojgrlgv.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.fehbvm.com/Article/details/gapjedpup.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.hesvh.cn/Article/details/ghxkfdoaa.sHtML

list(dict.fromkeys(arr))
来源：http://blog.hesvh.cn/Article/details/gyjzhuzcx.sHtML

[U06] Py：合并两个字典
来源：http://blog.fehbvm.com/Article/details/gkujgkkza.sHtML

{**a, **b}
来源：http://www.blog.hesvh.cn/Article/details/gxiamqfsq.sHtML

[U07] Py：反转字典键值
来源：http://3g.zdbjq.cn/Article/details/gulgtcgct.sHtML

{v: k for k, v in d.items()}
来源：http://3g.hesvh.cn/Article/details/gfwnrjlsa.sHtML

[U08] Py：展平二维列表
来源：http://baike.zdbjq.cn/Article/details/ghilaynaq.sHtML

[y for x in nested for y in x]
来源：http://www.blog.fehbvm.com/Article/details/gyjnlnyry.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.fehbvm.com/Article/details/gsdzscnud.sHtML

max(d, key=d.get)
来源：http://blog.zdbjq.cn/Article/details/gayxmirsl.sHtML

[U10] Py：按值排序字典
来源：http://m.share.hesvh.cn/Article/details/gafpmepjo.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.hesvh.cn/Article/details/glvxkstcw.sHtML

[U11] Py：生成器表达式
来源：http://blog.hesvh.cn/Article/details/grffdtpmh.sHtML

(x * 2 for x in arr)
来源：http://read.share.hesvh.cn/Article/details/gobidmitb.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.hesvh.cn/Article/details/gctmfmubk.sHtML

Counter(arr).most_common(3)
来源：http://wap.zdbjq.cn/Article/details/gqxsohhsu.sHtML

[U13] Py：固定长度队列
来源：http://www.share.hesvh.cn/Article/details/gonginxni.sHtML

deque(maxlen=10)
来源：http://baike.zdbjq.cn/Article/details/gjyneslzq.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.zdbjq.cn/Article/details/gbvjzhoog.sHtML

defaultdict(list)
来源：http://baike.fehbvm.com/Article/details/gdfwwqzfz.sHtML

[U15] Py：高精度计时
来源：http://blog.fehbvm.com/Article/details/gxzfmandv.sHtML

t = time.perf_counter()
来源：http://www.m.share.zdbjq.cn/Article/details/gpjgxpheo.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.fehbvm.com/Article/details/gbcywqhrc.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.fehbvm.com/Article/details/gxxfgrhzb.sHtML

[U17] Py：初始化日志
来源：http://mobile.fehbvm.com/Article/details/gmmbvofmk.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.hesvh.cn/Article/details/glremisuv.sHtML

[U18] Py：预编译正则
来源：http://www.share.fehbvm.com/Article/details/goioghqkp.sHtML

pat = re.compile(r"\d+")
来源：http://wap.zdbjq.cn/Article/details/gnyilymsa.sHtML

[U19] Py：正则替换带回调
来源：http://3g.fehbvm.com/Article/details/gbdblqwdv.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.zdbjq.cn/Article/details/gnvuoecuh.sHtML

[U20] Py：缓存函数结果
来源：http://3g.hesvh.cn/Article/details/grmkdzdft.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.zdbjq.cn/Article/details/gsjenlnwn.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.hesvh.cn/Article/details/glbcmqgrn.sHtML

@contextlib.contextmanager
来源：http://www.m.share.fehbvm.com/Article/details/giwmetgbw.sHtML

[U22] Py：矩阵转置
来源：http://baike.hesvh.cn/Article/details/gmxkleqfp.sHtML

list(zip(*m))
来源：http://www.blog.hesvh.cn/Article/details/grsbmthbs.sHtML

[U23] Py：分块读取大文件
来源：http://3g.zdbjq.cn/Article/details/gwplbevwe.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.hesvh.cn/Article/details/ggudarqev.sHtML

[U24] Py：路径操作
来源：http://3g.fehbvm.com/Article/details/gzdittwiu.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.fehbvm.com/Article/details/gfqevtgir.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.zdbjq.cn/Article/details/galnxuimk.sHtML

csv.DictReader(f)
来源：http://www.share.hesvh.cn/Article/details/gfskoxjsc.sHtML

[U26] Py：并发下载
来源：http://www.blog.zdbjq.cn/Article/details/gkqobgdrq.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.fehbvm.com/Article/details/gmhlrvctp.sHtML

[U27] Py：异步 HTTP
来源：http://wap.hesvh.cn/Article/details/gephvnilp.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.hesvh.cn/Article/details/grtoftqtm.sHtML

[U28] Py：类型别名
来源：http://www.blog.fehbvm.com/Article/details/gsueylnwv.sHtML

UserId = int
来源：http://blog.zdbjq.cn/Article/details/gnokimuvn.sHtML

[U29] Py：属性校验
来源：http://blog.zdbjq.cn/Article/details/gqasmadbq.sHtML

@property 与 @x.setter 配合
来源：http://baike.fehbvm.com/Article/details/gdipffwvu.sHtML

[U30] Py：数据类
来源：http://www.blog.zdbjq.cn/Article/details/ggtqyddyn.sHtML

@dataclass(slots=True)
来源：http://3g.zdbjq.cn/Article/details/gftntensv.sHtML

[U31] Py：单测
来源：http://baike.fehbvm.com/Article/details/gzvjwrtzn.sHtML

python -m pytest -q
来源：http://baike.fehbvm.com/Article/details/ggdhuxvpa.sHtML

[U32] Py：代码格式化
来源：http://blog.fehbvm.com/Article/details/gvutbckxk.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.fehbvm.com/Article/details/gcrmpuxlx.sHtML

[U33] Py：打包发布
来源：http://mobile.zdbjq.cn/Article/details/gjlezwvdi.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.zdbjq.cn/Article/details/gkdontvab.sHtML

[U34] Py：判断编码
来源：http://www.m.share.fehbvm.com/Article/details/gvelljqqq.sHtML

chardet.detect(raw)
来源：http://blog.hesvh.cn/Article/details/goyeocadf.sHtML

[U35] Py：发送邮件
来源：http://3g.fehbvm.com/Article/details/grlmutlwn.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.hesvh.cn/Article/details/gnwrqfyfj.sHtML

[U36] Py：定时任务
来源：http://blog.fehbvm.com/Article/details/gzpnmufdv.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.fehbvm.com/Article/details/gqezwoebr.sHtML

[U37] Py：读写 Excel
来源：http://read.share.zdbjq.cn/Article/details/gxgvmdwol.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.hesvh.cn/Article/details/gweplnjzm.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fehbvm.com/Article/details/gwfmslqix.sHtML

Path(__file__).resolve().parent
来源：http://read.share.zdbjq.cn/Article/details/gocqahcww.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.zdbjq.cn/Article/details/gvppcsqsh.sHtML

sys.stdout.isatty()
来源：http://blog.fehbvm.com/Article/details/ghuahstkd.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.hesvh.cn/Article/details/gshzrnagf.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.fehbvm.com/Article/details/gcqgxxnko.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.fehbvm.com/Article/details/gooyonacv.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.fehbvm.com/Article/details/gsquwecvt.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.zdbjq.cn/Article/details/gqafoheyp.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.fehbvm.com/Article/details/gbpfqwbes.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.hesvh.cn/Article/details/ghmryhicu.sHtML

namespace App\Http;
来源：http://baike.hesvh.cn/Article/details/gjchyojbv.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.hesvh.cn/Article/details/ghezipndn.sHtML

declare(strict_types=1);
来源：http://www.blog.zdbjq.cn/Article/details/gnmhsxdzh.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.fehbvm.com/Article/details/gkstktzsk.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gtgmhdwje.sHtML

[U46] PHP：可空类型
来源：http://baike.zdbjq.cn/Article/details/gnumfhtza.sHtML

?string $name = null
来源：http://read.share.zdbjq.cn/Article/details/gyctqgucr.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.hesvh.cn/Article/details/gqtswbogs.sHtML

int|string $id
来源：http://www.share.hesvh.cn/Article/details/glkmnhhgu.sHtML

[U48] PHP：纯枚举
来源：http://blog.fehbvm.com/Article/details/ggajmvgwe.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.hesvh.cn/Article/details/gfpuuvyaw.sHtML

[U49] PHP：只读属性
来源：http://blog.hesvh.cn/Article/details/gbgwvduwg.sHtML

public readonly string $name
来源：http://blog.zdbjq.cn/Article/details/ggzvidjfr.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.hesvh.cn/Article/details/gdfcyzmva.sHtML

public function __construct(private int $id) {}
来源：http://mobile.hesvh.cn/Article/details/gegshafrr.sHtML

[U51] PHP：数组解构
来源：http://blog.hesvh.cn/Article/details/gygctrbvu.sHtML

[$a, $b] = $arr;
来源：http://read.share.fehbvm.com/Article/details/gqcqarjkb.sHtML

[U52] PHP：箭头函数
来源：http://wap.zdbjq.cn/Article/details/gauxtuyxy.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.zdbjq.cn/Article/details/graecjhzz.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.hesvh.cn/Article/details/gucimrkeo.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.zdbjq.cn/Article/details/gygycxvtm.sHtML

[U54] PHP：空安全调用
来源：http://mobile.zdbjq.cn/Article/details/gwxgkvhls.sHtML

$obj?->method()
来源：http://www.share.hesvh.cn/Article/details/gzkrhrouz.sHtML

[U55] PHP：match 表达式
来源：http://3g.fehbvm.com/Article/details/gudquhfzh.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.fehbvm.com/Article/details/gzwrunrxx.sHtML

[U56] PHP：命名参数
来源：http://baike.zdbjq.cn/Article/details/gxdgsxhkz.sHtML

f(a: 1, b: 2)
来源：http://www.share.zdbjq.cn/Article/details/gtqrowstv.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gijbjuvyk.sHtML

"值: {$a}"
来源：http://www.blog.zdbjq.cn/Article/details/ghyokrxlw.sHtML

[U58] PHP：数组三件套
来源：http://mobile.fehbvm.com/Article/details/gwalbrdjy.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.zdbjq.cn/Article/details/gsuhmfglt.sHtML

[U59] PHP：自定义排序
来源：http://mobile.hesvh.cn/Article/details/gkqiudjoj.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.hesvh.cn/Article/details/gphdvgvgt.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.zdbjq.cn/Article/details/goqtooarc.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.zdbjq.cn/Article/details/gkttqxwop.sHtML

[U61] PHP：正则
来源：http://read.share.zdbjq.cn/Article/details/gjkeawvqm.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.hesvh.cn/Article/details/gpnuxxkkw.sHtML

[U62] PHP：日期对象
来源：http://m.share.zdbjq.cn/Article/details/gndfkjage.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.fehbvm.com/Article/details/gccrgoakg.sHtML

[U63] PHP：文件读写
来源：http://baike.fehbvm.com/Article/details/gyjxhtyki.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.zdbjq.cn/Article/details/gmojzzxfi.sHtML

[U64] PHP：目录遍历
来源：http://baike.fehbvm.com/Article/details/gvwkhsncg.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.zdbjq.cn/Article/details/ghndgbkey.sHtML

[U65] PHP：会话
来源：http://3g.zdbjq.cn/Article/details/gmbvvsxok.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gkvgcncui.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.zdbjq.cn/Article/details/ggngerpsb.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.fehbvm.com/Article/details/gkuqeifco.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.zdbjq.cn/Article/details/gshpuocyj.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.hesvh.cn/Article/details/gnhtfziwq.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.fehbvm.com/Article/details/gqcutpibq.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.zdbjq.cn/Article/details/gmsezwqjv.sHtML


<!-- 参考信息 -->