代发 wailian999

[S43] C++：智能指针
来源：http://m.share.zdbjq.cn/Article/details/gukqugjsq.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.hesvh.cn/Article/details/gfvlaejqy.sHtML

[S44] C++：引用传参
来源：http://3g.zdbjq.cn/Article/details/govhwucjp.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.zdbjq.cn/Article/details/guqfrxgfm.sHtML

[S45] C++：lambda
来源：http://blog.zdbjq.cn/Article/details/gzkqhyxci.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.zdbjq.cn/Article/details/gosdrtwnr.sHtML

[S46] C++：函数模板
来源：http://3g.fehbvm.com/Article/details/gsvwfxugb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.hesvh.cn/Article/details/gyipfwgjc.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.zdbjq.cn/Article/details/gyusbnmld.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.zdbjq.cn/Article/details/gksnxzyby.sHtML

[S48] C++：逐行读文件
来源：http://3g.fehbvm.com/Article/details/ghtlshmte.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.zdbjq.cn/Article/details/gwlzgywls.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fehbvm.com/Article/details/gxrvkkpsz.sHtML

[S49] C++：写文件
来源：http://3g.zdbjq.cn/Article/details/gdgggauoc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fehbvm.com/Article/details/guflnozqf.sHtML

[S50] C++：格式化数字
来源：http://wap.fehbvm.com/Article/details/gjqbgafub.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/guycmnxsj.sHtML

[S51] C++：显式类型转换
来源：http://blog.zdbjq.cn/Article/details/gsizhywaw.sHtML

static_cast<double>(a) / b
来源：http://3g.fehbvm.com/Article/details/gqyayfffn.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fehbvm.com/Article/details/gyonrjcuq.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fehbvm.com/Article/details/gmgcvzada.sHtML

[S53] C++：移动语义
来源：http://mobile.hesvh.cn/Article/details/grfpdlgkl.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fehbvm.com/Article/details/gbxocyyzv.sHtML

[S54] C++：异常处理
来源：http://mobile.fehbvm.com/Article/details/gnmbtxuex.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.hesvh.cn/Article/details/gdkmtyxwy.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fehbvm.com/Article/details/glsaafofo.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.zdbjq.cn/Article/details/gudfafmch.sHtML

[S56] C++：optional
来源：http://read.share.zdbjq.cn/Article/details/gdrjnwivp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.hesvh.cn/Article/details/gjxrieujn.sHtML

[S57] C++：编译期常量
来源：http://baike.zdbjq.cn/Article/details/gropvtzlg.sHtML

constexpr int N = 10;
来源：http://www.share.zdbjq.cn/Article/details/gzxtbwcpk.sHtML

[S58] C++：命名空间
来源：http://wap.zdbjq.cn/Article/details/gnqvnheet.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.hesvh.cn/Article/details/gzbsewmwm.sHtML

[S59] C++：静态断言
来源：http://m.share.hesvh.cn/Article/details/gaiwrkoig.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.hesvh.cn/Article/details/guavcmvtg.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.hesvh.cn/Article/details/gspemnzsz.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.hesvh.cn/Article/details/grfkukoos.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gnwolprde.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.hesvh.cn/Article/details/gffxnjnxd.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/glyaakdby.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gobyvqusw.sHtML

println("Hello")
来源：http://3g.zdbjq.cn/Article/details/glqrtkgwe.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fehbvm.com/Article/details/grvddsrlg.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.zdbjq.cn/Article/details/gufiioehr.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.hesvh.cn/Article/details/gculbbuyl.sHtML

"值: $b"
来源：http://read.share.zdbjq.cn/Article/details/gthdvprcz.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fehbvm.com/Article/details/gfopaqkgh.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fehbvm.com/Article/details/gkkqqrihp.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fehbvm.com/Article/details/gpxqxrvkq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.zdbjq.cn/Article/details/ghrxfzxix.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fehbvm.com/Article/details/gxkncodkg.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gpgrvgboh.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.zdbjq.cn/Article/details/gstngrvcc.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.zdbjq.cn/Article/details/ghcanwivj.sHtML

[T08] Kotlin：数据类
来源：http://mobile.hesvh.cn/Article/details/gqmkkvaov.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.hesvh.cn/Article/details/gudbtnlfv.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.zdbjq.cn/Article/details/gxpznrito.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fehbvm.com/Article/details/gcsmquhqv.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.hesvh.cn/Article/details/gotwdfhwa.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.zdbjq.cn/Article/details/gfbmhqzrv.sHtML

[T11] Kotlin：协程
来源：http://blog.zdbjq.cn/Article/details/gqpxofsgw.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.zdbjq.cn/Article/details/gluvumkfn.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fehbvm.com/Article/details/gickhdokw.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.hesvh.cn/Article/details/gngrkedxd.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fehbvm.com/Article/details/gahqpbjyt.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fehbvm.com/Article/details/gfgpashec.sHtML

[T14] Kotlin：循环
来源：http://baike.hesvh.cn/Article/details/gngmobwra.sHtML

for (i in 1..10) println(i)
来源：http://wap.zdbjq.cn/Article/details/gbhvgijfl.sHtML

[T15] Kotlin：接口
来源：http://wap.zdbjq.cn/Article/details/gvtdhtqfj.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fehbvm.com/Article/details/gbgdwzqar.sHtML

[T16] Swift：Hello World
来源：http://3g.fehbvm.com/Article/details/gpmvlkfxs.sHtML

print("Hello")
来源：http://read.share.hesvh.cn/Article/details/gfwihtjab.sHtML

[T17] Swift：变量与常量
来源：http://m.share.fehbvm.com/Article/details/gumvcbvdl.sHtML

var a = 1;  let b = 2
来源：http://m.share.zdbjq.cn/Article/details/ggbybflws.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gqtcaqwhj.sHtML

"值: \(b)"
来源：http://www.share.hesvh.cn/Article/details/gkdnrshjo.sHtML

[T19] Swift：可选绑定
来源：http://3g.zdbjq.cn/Article/details/gkmqtwsxc.sHtML

if let n = opt { print(n) }
来源：http://baike.zdbjq.cn/Article/details/grigmsuqq.sHtML

[T20] Swift：数组操作
来源：http://m.share.zdbjq.cn/Article/details/gfzfrlfnc.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.zdbjq.cn/Article/details/gnhkgquwf.sHtML

[T21] Swift：遍历
来源：http://www.m.share.hesvh.cn/Article/details/gwwysqesd.sHtML

for x in a { print(x) }
来源：http://www.share.hesvh.cn/Article/details/gehcdjqnq.sHtML

[T22] Swift：字典
来源：http://blog.hesvh.cn/Article/details/gzsbhavnx.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fehbvm.com/Article/details/gzlfazbqo.sHtML

[T23] Swift：函数
来源：http://blog.hesvh.cn/Article/details/gztvfmung.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.hesvh.cn/Article/details/ghctzitun.sHtML

[T24] Swift：闭包
来源：http://baike.fehbvm.com/Article/details/gikwcjmsw.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.fehbvm.com/Article/details/gubqcycou.sHtML

[T25] Swift：结构体
来源：http://www.blog.hesvh.cn/Article/details/gxlovptfd.sHtML

struct P { var x: Int }
来源：http://m.share.hesvh.cn/Article/details/gilgvnmvi.sHtML

[T26] Swift：类与重写
来源：http://m.share.hesvh.cn/Article/details/gvxeiailr.sHtML

class A: Base { override func f() {} }
来源：http://baike.zdbjq.cn/Article/details/gjvkiyymv.sHtML

[T27] Swift：错误处理
来源：http://3g.zdbjq.cn/Article/details/gsluigutm.sHtML

do { try f() } catch { print(error) }
来源：http://3g.hesvh.cn/Article/details/gnobtmefl.sHtML

[T28] Swift：枚举
来源：http://mobile.hesvh.cn/Article/details/gplktkvde.sHtML

enum Color { case red, green }
来源：http://m.share.fehbvm.com/Article/details/gnmkbhdrg.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.hesvh.cn/Article/details/ghvlirjgb.sHtML

guard let x = opt else { return }
来源：http://mobile.fehbvm.com/Article/details/guxielqbc.sHtML

[T30] Swift：协议
来源：http://www.m.share.zdbjq.cn/Article/details/grvrmbvoz.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.fehbvm.com/Article/details/getjrmjlq.sHtML

[T31] Lua：Hello World
来源：http://blog.fehbvm.com/Article/details/gfekucoyg.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/gqmblrgll.sHtML

[T32] Lua：局部变量
来源：http://mobile.zdbjq.cn/Article/details/gaxkyjhwn.sHtML

local a = 1
来源：http://baike.zdbjq.cn/Article/details/gkwintpxa.sHtML

[T33] Lua：表（数组）
来源：http://blog.zdbjq.cn/Article/details/glfalfaoy.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.fehbvm.com/Article/details/gdoqboabk.sHtML

[T34] Lua：遍历表
来源：http://m.share.zdbjq.cn/Article/details/ghdzrnupi.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.zdbjq.cn/Article/details/gxrynsupx.sHtML

[T35] Lua：字典表
来源：http://www.blog.fehbvm.com/Article/details/gwudshlin.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gmvmzzngs.sHtML

[T36] Lua：函数
来源：http://3g.hesvh.cn/Article/details/gksswrisk.sHtML

function add(a, b) return a + b end
来源：http://wap.hesvh.cn/Article/details/gqgmbdozy.sHtML

[T37] Lua：字符串拼接
来源：http://baike.fehbvm.com/Article/details/gbwphxexh.sHtML

"a" .. "b"
来源：http://www.share.hesvh.cn/Article/details/gzagsyvna.sHtML

[T38] Lua：条件
来源：http://www.blog.fehbvm.com/Article/details/ghjzfcmjd.sHtML

if x > 0 then print("正") end
来源：http://3g.zdbjq.cn/Article/details/gitxufxhg.sHtML

[T39] Lua：模式匹配
来源：http://blog.zdbjq.cn/Article/details/gdegvvaxj.sHtML

string.find(s, "%d+")
来源：http://www.share.fehbvm.com/Article/details/gxhjxnpsm.sHtML

[T40] Lua：元表
来源：http://wap.fehbvm.com/Article/details/gzclkovvk.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.fehbvm.com/Article/details/gkatyccni.sHtML

[T41] Perl：Hello World
来源：http://wap.hesvh.cn/Article/details/goyyzrprl.sHtML

print "Hello\n";
来源：http://www.m.share.fehbvm.com/Article/details/gjqldhjzb.sHtML

[T42] Perl：变量类型
来源：http://m.share.hesvh.cn/Article/details/gstblehbp.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.fehbvm.com/Article/details/gkfrqxngp.sHtML

[T43] Perl：字符串插值
来源：http://baike.hesvh.cn/Article/details/gprwjxzpg.sHtML

"值: $a"
来源：http://www.m.share.zdbjq.cn/Article/details/ggreirvdz.sHtML

[T44] Perl：条件
来源：http://read.share.zdbjq.cn/Article/details/gtldpsiwq.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.zdbjq.cn/Article/details/gvnofxpas.sHtML

[T45] Perl：数组遍历
来源：http://www.share.fehbvm.com/Article/details/gbzfmttva.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.fehbvm.com/Article/details/gowppjpci.sHtML

[T46] Perl：哈希操作
来源：http://m.share.zdbjq.cn/Article/details/gqlbbeveq.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.fehbvm.com/Article/details/gbkewzhto.sHtML

[T47] Perl：正则捕获
来源：http://read.share.zdbjq.cn/Article/details/gmfhmyrzj.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmigjcinc.sHtML

[T48] Perl：正则替换
来源：http://www.share.zdbjq.cn/Article/details/gjegxhotp.sHtML

$s =~ s/old/new/g;
来源：http://read.share.fehbvm.com/Article/details/gpkxyaaix.sHtML

[T49] Perl：函数
来源：http://3g.fehbvm.com/Article/details/gnsjfuqyj.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gjbmgdfmm.sHtML

[T50] Perl：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gtvnlooti.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.fehbvm.com/Article/details/gmpwuhcpm.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.fehbvm.com/Article/details/gwpuyxzhi.sHtML

[T51] Scala：Hello World
来源：http://3g.fehbvm.com/Article/details/gscbxwwjm.sHtML

println("Hello")
来源：http://3g.fehbvm.com/Article/details/gluyniswq.sHtML

[T52] Scala：变量
来源：http://www.share.hesvh.cn/Article/details/gycuivdlf.sHtML

val a = 1;  var b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gsmqkmxsy.sHtML

[T53] Scala：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gxyunlyuk.sHtML

s"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/gvlupqhat.sHtML

[T54] Scala：集合映射
来源：http://3g.zdbjq.cn/Article/details/ghyzzxbak.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.hesvh.cn/Article/details/gbgqhbaft.sHtML

[T55] Scala：集合过滤
来源：http://www.share.zdbjq.cn/Article/details/gncewcsrc.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.hesvh.cn/Article/details/glbovbbwq.sHtML

[T56] Scala：样例类
来源：http://blog.zdbjq.cn/Article/details/gbffxajpv.sHtML

case class User(name: String, age: Int)
来源：http://wap.hesvh.cn/Article/details/gnldxtrrf.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.hesvh.cn/Article/details/gjpkwwjpk.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.hesvh.cn/Article/details/gidjgphbu.sHtML

[T58] Scala：函数定义
来源：http://3g.fehbvm.com/Article/details/gmthryrms.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.hesvh.cn/Article/details/glhoanlvx.sHtML

[T59] Scala：循环
来源：http://baike.hesvh.cn/Article/details/gaxnchtsd.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/ghyhgyyyf.sHtML

[T60] Scala：折叠
来源：http://3g.zdbjq.cn/Article/details/gsyozopjd.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.fehbvm.com/Article/details/ghhbiypqx.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gfbccfucx.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.fehbvm.com/Article/details/guwxcrmph.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gsmnsnxbx.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.hesvh.cn/Article/details/gulwbycqa.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.fehbvm.com/Article/details/gosxckuze.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.hesvh.cn/Article/details/goupnfceg.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.fehbvm.com/Article/details/gtrouwvih.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.fehbvm.com/Article/details/giblmbsvp.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.zdbjq.cn/Article/details/gocarseka.sHtML

[U04] Py：变量调试打印
来源：http://3g.zdbjq.cn/Article/details/ggfcikpag.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.hesvh.cn/Article/details/gqxjbdsna.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.zdbjq.cn/Article/details/gjmkbwtwn.sHtML

list(dict.fromkeys(arr))
来源：http://blog.zdbjq.cn/Article/details/gkfoxqvqt.sHtML

[U06] Py：合并两个字典
来源：http://mobile.hesvh.cn/Article/details/gjftjdagx.sHtML

{**a, **b}
来源：http://3g.fehbvm.com/Article/details/gkiglnsxc.sHtML

[U07] Py：反转字典键值
来源：http://baike.zdbjq.cn/Article/details/gzukndzwa.sHtML

{v: k for k, v in d.items()}
来源：http://baike.hesvh.cn/Article/details/gprulfbsy.sHtML

[U08] Py：展平二维列表
来源：http://read.share.zdbjq.cn/Article/details/gnpsmhndd.sHtML

[y for x in nested for y in x]
来源：http://wap.hesvh.cn/Article/details/gklgqfkbi.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.zdbjq.cn/Article/details/gyterhbbr.sHtML

max(d, key=d.get)
来源：http://m.share.hesvh.cn/Article/details/ghjvexiqf.sHtML

[U10] Py：按值排序字典
来源：http://www.share.zdbjq.cn/Article/details/gmfbrghtt.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.zdbjq.cn/Article/details/gdrwxpbgd.sHtML

[U11] Py：生成器表达式
来源：http://wap.hesvh.cn/Article/details/genfcrfyf.sHtML

(x * 2 for x in arr)
来源：http://mobile.hesvh.cn/Article/details/gxubnqhxh.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.fehbvm.com/Article/details/gansjncjm.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.zdbjq.cn/Article/details/gcjiyhidf.sHtML

[U13] Py：固定长度队列
来源：http://baike.fehbvm.com/Article/details/gpmcmopwu.sHtML

deque(maxlen=10)
来源：http://mobile.zdbjq.cn/Article/details/gghjpplwv.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.zdbjq.cn/Article/details/gwcgajgov.sHtML

defaultdict(list)
来源：http://wap.hesvh.cn/Article/details/gtvxpigdk.sHtML

[U15] Py：高精度计时
来源：http://mobile.hesvh.cn/Article/details/gabqffake.sHtML

t = time.perf_counter()
来源：http://m.share.hesvh.cn/Article/details/gdszoigyr.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.fehbvm.com/Article/details/gmodgvect.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.zdbjq.cn/Article/details/gdmqfutun.sHtML

[U17] Py：初始化日志
来源：http://m.share.fehbvm.com/Article/details/gmutnlozh.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.zdbjq.cn/Article/details/gqnxllngf.sHtML

[U18] Py：预编译正则
来源：http://www.blog.hesvh.cn/Article/details/gikfzatee.sHtML

pat = re.compile(r"\d+")
来源：http://blog.hesvh.cn/Article/details/gfqorpzsd.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.zdbjq.cn/Article/details/gqmgtecbt.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.fehbvm.com/Article/details/gbsomriil.sHtML

[U20] Py：缓存函数结果
来源：http://3g.hesvh.cn/Article/details/gwydxdlea.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.zdbjq.cn/Article/details/gzxasiqvl.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.hesvh.cn/Article/details/gsgjvpauq.sHtML

@contextlib.contextmanager
来源：http://www.blog.zdbjq.cn/Article/details/gvrklqyni.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.zdbjq.cn/Article/details/gcxdufcob.sHtML

list(zip(*m))
来源：http://baike.hesvh.cn/Article/details/gbyhxbupi.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.zdbjq.cn/Article/details/gdsulksyq.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.zdbjq.cn/Article/details/gyghxnwqk.sHtML

[U24] Py：路径操作
来源：http://wap.hesvh.cn/Article/details/goqmuqtbw.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.fehbvm.com/Article/details/gptafxzti.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.zdbjq.cn/Article/details/gvlvtgdjd.sHtML

csv.DictReader(f)
来源：http://mobile.hesvh.cn/Article/details/gmdepahtl.sHtML

[U26] Py：并发下载
来源：http://www.blog.hesvh.cn/Article/details/gcqsojhry.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.hesvh.cn/Article/details/gvicuvjqd.sHtML

[U27] Py：异步 HTTP
来源：http://wap.zdbjq.cn/Article/details/gunfghdef.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.zdbjq.cn/Article/details/goelppqtq.sHtML

[U28] Py：类型别名
来源：http://wap.hesvh.cn/Article/details/gazuqblgi.sHtML

UserId = int
来源：http://www.share.fehbvm.com/Article/details/grkuahith.sHtML

[U29] Py：属性校验
来源：http://m.share.fehbvm.com/Article/details/gytximjsg.sHtML

@property 与 @x.setter 配合
来源：http://www.share.fehbvm.com/Article/details/gwfcvbwun.sHtML

[U30] Py：数据类
来源：http://www.blog.zdbjq.cn/Article/details/gcsvrkjyx.sHtML

@dataclass(slots=True)
来源：http://3g.fehbvm.com/Article/details/gfgjmfsrv.sHtML

[U31] Py：单测
来源：http://www.m.share.zdbjq.cn/Article/details/gtdgfmsub.sHtML

python -m pytest -q
来源：http://baike.zdbjq.cn/Article/details/gznsapmqr.sHtML

[U32] Py：代码格式化
来源：http://wap.fehbvm.com/Article/details/ggwdbueux.sHtML

ruff format . && ruff check --fix .
来源：http://baike.fehbvm.com/Article/details/glsotqzzn.sHtML

[U33] Py：打包发布
来源：http://www.blog.hesvh.cn/Article/details/gkukjlcmu.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.zdbjq.cn/Article/details/gpajhvzuu.sHtML

[U34] Py：判断编码
来源：http://blog.fehbvm.com/Article/details/gxdnlqzba.sHtML

chardet.detect(raw)
来源：http://baike.zdbjq.cn/Article/details/ghloctpvb.sHtML

[U35] Py：发送邮件
来源：http://www.share.fehbvm.com/Article/details/gilzjxvjt.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.fehbvm.com/Article/details/grkusxgwz.sHtML

[U36] Py：定时任务
来源：http://www.share.zdbjq.cn/Article/details/gsyabofzh.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.fehbvm.com/Article/details/gxpayxrvo.sHtML

[U37] Py：读写 Excel
来源：http://3g.fehbvm.com/Article/details/govbkleer.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.fehbvm.com/Article/details/gzqcnrubm.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.hesvh.cn/Article/details/glntaqvli.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.zdbjq.cn/Article/details/gveegsrmy.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.hesvh.cn/Article/details/gghgfmacq.sHtML

sys.stdout.isatty()
来源：http://www.m.share.zdbjq.cn/Article/details/gklfpzkws.sHtML

[U40] Py：打印到标准错误
来源：http://wap.fehbvm.com/Article/details/gznxvhnmk.sHtML

print("err", file=sys.stderr)
来源：http://read.share.hesvh.cn/Article/details/gwjkcimzf.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.zdbjq.cn/Article/details/gazqrmgfd.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.fehbvm.com/Article/details/gojwhuumt.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.hesvh.cn/Article/details/gxhimyszz.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.zdbjq.cn/Article/details/gxubnqivh.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.fehbvm.com/Article/details/gjmrkvhgg.sHtML

namespace App\Http;
来源：http://3g.hesvh.cn/Article/details/gqukinmof.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.fehbvm.com/Article/details/gbhogtwqr.sHtML

declare(strict_types=1);
来源：http://mobile.hesvh.cn/Article/details/grgxsiqig.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.hesvh.cn/Article/details/getkbmpwu.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gsgpuwwni.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.hesvh.cn/Article/details/gshxzwwlr.sHtML

?string $name = null
来源：http://www.blog.zdbjq.cn/Article/details/gclrpcpcc.sHtML

[U47] PHP：联合类型
来源：http://wap.fehbvm.com/Article/details/gxtfeyjps.sHtML

int|string $id
来源：http://www.m.share.hesvh.cn/Article/details/gtiaygcnn.sHtML

[U48] PHP：纯枚举
来源：http://mobile.fehbvm.com/Article/details/gnrqbilbx.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.fehbvm.com/Article/details/gtnlnwjwh.sHtML

[U49] PHP：只读属性
来源：http://wap.zdbjq.cn/Article/details/glbidtjom.sHtML

public readonly string $name
来源：http://www.share.fehbvm.com/Article/details/gmaqaxiku.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.hesvh.cn/Article/details/gmiyjzidm.sHtML

public function __construct(private int $id) {}
来源：http://mobile.fehbvm.com/Article/details/goygrulir.sHtML

[U51] PHP：数组解构
来源：http://read.share.zdbjq.cn/Article/details/gnbcowuvu.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.zdbjq.cn/Article/details/gaxzzngvh.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.zdbjq.cn/Article/details/gwbycapjx.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.hesvh.cn/Article/details/gcfnopgst.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.hesvh.cn/Article/details/gonanobjw.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.zdbjq.cn/Article/details/gvszzmxoj.sHtML

[U54] PHP：空安全调用
来源：http://baike.fehbvm.com/Article/details/galtvqywp.sHtML

$obj?->method()
来源：http://www.m.share.zdbjq.cn/Article/details/gqwqkaoid.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.fehbvm.com/Article/details/gyptkevjk.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.fehbvm.com/Article/details/glcgfvyet.sHtML

[U56] PHP：命名参数
来源：http://www.blog.hesvh.cn/Article/details/gsarruabw.sHtML

f(a: 1, b: 2)
来源：http://blog.zdbjq.cn/Article/details/gtcszryqk.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/grmwuqots.sHtML

"值: {$a}"
来源：http://read.share.fehbvm.com/Article/details/gsnleexwh.sHtML

[U58] PHP：数组三件套
来源：http://wap.fehbvm.com/Article/details/gxgpvtkyr.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.fehbvm.com/Article/details/goicunzhm.sHtML

[U59] PHP：自定义排序
来源：http://read.share.hesvh.cn/Article/details/gutsmhucj.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.hesvh.cn/Article/details/glhiilsxn.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.hesvh.cn/Article/details/gpzwmewlb.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.fehbvm.com/Article/details/gmnepejdq.sHtML

[U61] PHP：正则
来源：http://www.blog.hesvh.cn/Article/details/gtgpouvgp.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.fehbvm.com/Article/details/gbvozxkop.sHtML

[U62] PHP：日期对象
来源：http://mobile.fehbvm.com/Article/details/gtaxrflfl.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.hesvh.cn/Article/details/gqskjqytj.sHtML

[U63] PHP：文件读写
来源：http://baike.fehbvm.com/Article/details/gulpadvby.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.fehbvm.com/Article/details/gcnheiqea.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.zdbjq.cn/Article/details/guadcxqlj.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.fehbvm.com/Article/details/gmzoohkif.sHtML

[U65] PHP：会话
来源：http://wap.hesvh.cn/Article/details/gmbmpstkv.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.fehbvm.com/Article/details/gjromwgvi.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.hesvh.cn/Article/details/ggtieteof.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.fehbvm.com/Article/details/gipwsfqxh.sHtML

[U67] PHP：处理文件上传
来源：http://wap.hesvh.cn/Article/details/grzmrmoam.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.zdbjq.cn/Article/details/gwrlceghp.sHtML

[U68] PHP：PDO 连接
来源：http://wap.hesvh.cn/Article/details/gjiaqkivy.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.fehbvm.com/Article/details/gyuejytex.sHtML


<!-- 参考信息 -->