代发 wailian999

[S39] C++：自定义比较器排序
来源：http://blog.fehbvm.com/Article/details/ghadbvekj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.hesvh.cn/Article/details/grjwumhfw.sHtML

[S40] C++：查找元素
来源：http://read.share.fehbvm.com/Article/details/guswmphil.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fehbvm.com/Article/details/gagnjxmql.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fehbvm.com/Article/details/gixctdteg.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.zdbjq.cn/Article/details/gehpobcyw.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fehbvm.com/Article/details/gtztpabtn.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.hesvh.cn/Article/details/gipgcyira.sHtML

[S43] C++：智能指针
来源：http://www.blog.zdbjq.cn/Article/details/gssbtmltn.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fehbvm.com/Article/details/giptxnvkl.sHtML

[S44] C++：引用传参
来源：http://read.share.hesvh.cn/Article/details/gadizounf.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fehbvm.com/Article/details/gmcntpylr.sHtML

[S45] C++：lambda
来源：http://3g.hesvh.cn/Article/details/gxvfuntdy.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.zdbjq.cn/Article/details/gswcgdppb.sHtML

[S46] C++：函数模板
来源：http://www.m.share.hesvh.cn/Article/details/gbpavihhk.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fehbvm.com/Article/details/gyvtmhaiu.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fehbvm.com/Article/details/geqsyshgp.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fehbvm.com/Article/details/gsrwuwlnu.sHtML

[S48] C++：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gveajknlt.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.hesvh.cn/Article/details/gsshvbhpq.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fehbvm.com/Article/details/grhqgywfu.sHtML

[S49] C++：写文件
来源：http://baike.fehbvm.com/Article/details/gmruspzek.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fehbvm.com/Article/details/gmydggkot.sHtML

[S50] C++：格式化数字
来源：http://wap.zdbjq.cn/Article/details/gfwswzmqr.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gotylacte.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.hesvh.cn/Article/details/gxablhtez.sHtML

static_cast<double>(a) / b
来源：http://www.share.hesvh.cn/Article/details/gxxcnxgvw.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.hesvh.cn/Article/details/gxtjwaiml.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fehbvm.com/Article/details/glofxrywp.sHtML

[S53] C++：移动语义
来源：http://mobile.hesvh.cn/Article/details/gnprafeqz.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fehbvm.com/Article/details/ghezvpahz.sHtML

[S54] C++：异常处理
来源：http://m.share.hesvh.cn/Article/details/gsgdnmcsd.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.hesvh.cn/Article/details/ggvbcxfky.sHtML

[S55] C++：结构化绑定
来源：http://baike.hesvh.cn/Article/details/gmqokqkaa.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fehbvm.com/Article/details/gsafhlymp.sHtML

[S56] C++：optional
来源：http://baike.zdbjq.cn/Article/details/gxumuvvtg.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.zdbjq.cn/Article/details/glhplfxbg.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fehbvm.com/Article/details/gmypntbod.sHtML

constexpr int N = 10;
来源：http://www.blog.fehbvm.com/Article/details/gpwqwcahz.sHtML

[S58] C++：命名空间
来源：http://read.share.zdbjq.cn/Article/details/guxtsimkq.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.zdbjq.cn/Article/details/gyhxuwafh.sHtML

[S59] C++：静态断言
来源：http://www.share.zdbjq.cn/Article/details/goayzewgv.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fehbvm.com/Article/details/gzliwmuxf.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.zdbjq.cn/Article/details/gtnzxuqyt.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fehbvm.com/Article/details/gijbtnzzc.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/goywswqni.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.zdbjq.cn/Article/details/gnqwtouoa.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gtnpmxmsy.sHtML

[T01] Kotlin：Hello World
来源：http://blog.zdbjq.cn/Article/details/gbhtsainx.sHtML

println("Hello")
来源：http://3g.hesvh.cn/Article/details/gcelaaqyo.sHtML

[T02] Kotlin：变量
来源：http://read.share.hesvh.cn/Article/details/grotioqlw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.hesvh.cn/Article/details/gxemysmia.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.hesvh.cn/Article/details/gnxadxrpb.sHtML

"值: $b"
来源：http://read.share.hesvh.cn/Article/details/gdvzmyonl.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fehbvm.com/Article/details/gnofgfbjf.sHtML

val n: String? = null;  n?.length
来源：http://3g.zdbjq.cn/Article/details/gbgahnaea.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fehbvm.com/Article/details/gnbmbvmdu.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.zdbjq.cn/Article/details/gdpylgirc.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.zdbjq.cn/Article/details/gvcccyfng.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fehbvm.com/Article/details/ghimheijj.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.hesvh.cn/Article/details/gcqpvtocg.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/gyysyuien.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fehbvm.com/Article/details/gnjivftei.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.hesvh.cn/Article/details/gtcwmkgcz.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.zdbjq.cn/Article/details/gksciabti.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fehbvm.com/Article/details/gtftfbokn.sHtML

[T10] Kotlin：默认参数
来源：http://blog.hesvh.cn/Article/details/gsmnhayts.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fehbvm.com/Article/details/gmvucoged.sHtML

[T11] Kotlin：协程
来源：http://baike.fehbvm.com/Article/details/gvflkdliw.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.hesvh.cn/Article/details/gujzfnniy.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fehbvm.com/Article/details/gemzfzxvx.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gldfaxahw.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.hesvh.cn/Article/details/girfgfgcl.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.zdbjq.cn/Article/details/gqaqgqxlk.sHtML

[T14] Kotlin：循环
来源：http://www.blog.zdbjq.cn/Article/details/gibighmgt.sHtML

for (i in 1..10) println(i)
来源：http://wap.zdbjq.cn/Article/details/gvfksdawu.sHtML

[T15] Kotlin：接口
来源：http://blog.fehbvm.com/Article/details/gfwzipsij.sHtML

interface Shape { fun area(): Double }
来源：http://baike.zdbjq.cn/Article/details/gsbodibwb.sHtML

[T16] Swift：Hello World
来源：http://m.share.fehbvm.com/Article/details/gxrtikvke.sHtML

print("Hello")
来源：http://www.share.zdbjq.cn/Article/details/glndwddpm.sHtML

[T17] Swift：变量与常量
来源：http://baike.hesvh.cn/Article/details/gettuprbg.sHtML

var a = 1;  let b = 2
来源：http://read.share.zdbjq.cn/Article/details/gfxaibuim.sHtML

[T18] Swift：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gszegecmx.sHtML

"值: \(b)"
来源：http://m.share.hesvh.cn/Article/details/guxmnhahj.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.hesvh.cn/Article/details/gjaliviqp.sHtML

if let n = opt { print(n) }
来源：http://read.share.fehbvm.com/Article/details/ghbtwiyzb.sHtML

[T20] Swift：数组操作
来源：http://wap.zdbjq.cn/Article/details/gatvvohqz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.hesvh.cn/Article/details/gmxaigaep.sHtML

[T21] Swift：遍历
来源：http://read.share.zdbjq.cn/Article/details/gexvhfsxy.sHtML

for x in a { print(x) }
来源：http://blog.zdbjq.cn/Article/details/gahvscwth.sHtML

[T22] Swift：字典
来源：http://www.m.share.fehbvm.com/Article/details/gxdzmhyis.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.hesvh.cn/Article/details/gqnnvdqel.sHtML

[T23] Swift：函数
来源：http://www.blog.fehbvm.com/Article/details/gakuhvphe.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.hesvh.cn/Article/details/gneepbhwb.sHtML

[T24] Swift：闭包
来源：http://3g.hesvh.cn/Article/details/gvtawyakh.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.hesvh.cn/Article/details/gcfbpedsf.sHtML

[T25] Swift：结构体
来源：http://www.share.hesvh.cn/Article/details/geeblrndv.sHtML

struct P { var x: Int }
来源：http://www.blog.zdbjq.cn/Article/details/gpkiojfpq.sHtML

[T26] Swift：类与重写
来源：http://www.share.hesvh.cn/Article/details/gfanfeyjp.sHtML

class A: Base { override func f() {} }
来源：http://mobile.zdbjq.cn/Article/details/gjpkbqcni.sHtML

[T27] Swift：错误处理
来源：http://blog.hesvh.cn/Article/details/grhanaarj.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.zdbjq.cn/Article/details/gunfdwrpp.sHtML

[T28] Swift：枚举
来源：http://www.share.zdbjq.cn/Article/details/ghkpshqmd.sHtML

enum Color { case red, green }
来源：http://www.m.share.hesvh.cn/Article/details/garafaaii.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.hesvh.cn/Article/details/grmdqeeoo.sHtML

guard let x = opt else { return }
来源：http://www.blog.zdbjq.cn/Article/details/gasgkrbvo.sHtML

[T30] Swift：协议
来源：http://3g.zdbjq.cn/Article/details/gnbmukmig.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.hesvh.cn/Article/details/gymksxfbs.sHtML

[T31] Lua：Hello World
来源：http://read.share.fehbvm.com/Article/details/gxjalqfnw.sHtML

print("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/goouppmkh.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.zdbjq.cn/Article/details/gbpwqjgly.sHtML

local a = 1
来源：http://blog.hesvh.cn/Article/details/gvqtmllim.sHtML

[T33] Lua：表（数组）
来源：http://m.share.zdbjq.cn/Article/details/gveoxpslr.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.hesvh.cn/Article/details/gdsmmacro.sHtML

[T34] Lua：遍历表
来源：http://blog.hesvh.cn/Article/details/glfauwroi.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.fehbvm.com/Article/details/girchkstm.sHtML

[T35] Lua：字典表
来源：http://www.share.zdbjq.cn/Article/details/gjdjrnkow.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.zdbjq.cn/Article/details/gtscamyax.sHtML

[T36] Lua：函数
来源：http://read.share.zdbjq.cn/Article/details/gzturoqrf.sHtML

function add(a, b) return a + b end
来源：http://m.share.fehbvm.com/Article/details/gkkwxrmkd.sHtML

[T37] Lua：字符串拼接
来源：http://wap.zdbjq.cn/Article/details/gaedpeqdj.sHtML

"a" .. "b"
来源：http://mobile.hesvh.cn/Article/details/gosqqlcha.sHtML

[T38] Lua：条件
来源：http://baike.hesvh.cn/Article/details/geacosisj.sHtML

if x > 0 then print("正") end
来源：http://mobile.zdbjq.cn/Article/details/gaarivgxi.sHtML

[T39] Lua：模式匹配
来源：http://blog.hesvh.cn/Article/details/gsulcrjkl.sHtML

string.find(s, "%d+")
来源：http://www.m.share.zdbjq.cn/Article/details/gxbgkggar.sHtML

[T40] Lua：元表
来源：http://mobile.zdbjq.cn/Article/details/gsxedkrlq.sHtML

setmetatable({}, { __index = base })
来源：http://baike.hesvh.cn/Article/details/gschzwyig.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gjqzewgjr.sHtML

print "Hello\n";
来源：http://m.share.fehbvm.com/Article/details/gbsqrycem.sHtML

[T42] Perl：变量类型
来源：http://www.share.zdbjq.cn/Article/details/gxwrlkaio.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.fehbvm.com/Article/details/gfjtozivk.sHtML

[T43] Perl：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gynoveaaj.sHtML

"值: $a"
来源：http://m.share.hesvh.cn/Article/details/guecsesgg.sHtML

[T44] Perl：条件
来源：http://baike.zdbjq.cn/Article/details/gvuyyanyl.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.hesvh.cn/Article/details/gipccbvcf.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.hesvh.cn/Article/details/gdugmxlxf.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.fehbvm.com/Article/details/gvlqjodux.sHtML

[T46] Perl：哈希操作
来源：http://baike.zdbjq.cn/Article/details/gtyqdsqkw.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.hesvh.cn/Article/details/gswzmcpum.sHtML

[T47] Perl：正则捕获
来源：http://3g.hesvh.cn/Article/details/gioztosvn.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.zdbjq.cn/Article/details/gxirnynxh.sHtML

[T48] Perl：正则替换
来源：http://www.blog.hesvh.cn/Article/details/gmahrcyco.sHtML

$s =~ s/old/new/g;
来源：http://wap.zdbjq.cn/Article/details/ghjjzuvgg.sHtML

[T49] Perl：函数
来源：http://www.blog.fehbvm.com/Article/details/gyltxsfbw.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gnjbtjzzx.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gifoqspdm.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.fehbvm.com/Article/details/gpewfsjxm.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.zdbjq.cn/Article/details/gjlbrpgud.sHtML

[T51] Scala：Hello World
来源：http://www.share.fehbvm.com/Article/details/gsqicqenn.sHtML

println("Hello")
来源：http://wap.hesvh.cn/Article/details/gxhyynpha.sHtML

[T52] Scala：变量
来源：http://3g.fehbvm.com/Article/details/gycbvctjk.sHtML

val a = 1;  var b = 2
来源：http://blog.zdbjq.cn/Article/details/gztwrnequ.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gwfzqpnxt.sHtML

s"值: $b"
来源：http://3g.hesvh.cn/Article/details/gbxiqfyxa.sHtML

[T54] Scala：集合映射
来源：http://wap.zdbjq.cn/Article/details/ghwltzajn.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.fehbvm.com/Article/details/gykoieoac.sHtML

[T55] Scala：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/gqahktadz.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.fehbvm.com/Article/details/gkywxewml.sHtML

[T56] Scala：样例类
来源：http://www.m.share.zdbjq.cn/Article/details/grvovqiku.sHtML

case class User(name: String, age: Int)
来源：http://www.share.hesvh.cn/Article/details/gdxpbjlzi.sHtML

[T57] Scala：模式匹配
来源：http://www.share.hesvh.cn/Article/details/gkgkfzwjx.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.fehbvm.com/Article/details/gjziiagah.sHtML

[T58] Scala：函数定义
来源：http://read.share.fehbvm.com/Article/details/gdujdetjv.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.hesvh.cn/Article/details/gtquqtpia.sHtML

[T59] Scala：循环
来源：http://wap.zdbjq.cn/Article/details/gpobumxkn.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.fehbvm.com/Article/details/gjwxmzzgx.sHtML

[T60] Scala：折叠
来源：http://www.blog.zdbjq.cn/Article/details/gcdxlyesc.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.fehbvm.com/Article/details/gqiuuzerd.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gjucbqsao.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.hesvh.cn/Article/details/gidlvuxsg.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gqlplmxzg.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.zdbjq.cn/Article/details/gesbqikyi.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.zdbjq.cn/Article/details/gqfasaqws.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.hesvh.cn/Article/details/gutexyvza.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.zdbjq.cn/Article/details/gqgxkpngc.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.hesvh.cn/Article/details/gtpptpkun.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.hesvh.cn/Article/details/gcqxofyjz.sHtML

[U04] Py：变量调试打印
来源：http://3g.fehbvm.com/Article/details/gakjajkzv.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.zdbjq.cn/Article/details/gjdvirvrf.sHtML

[U05] Py：列表去重且保序
来源：http://wap.fehbvm.com/Article/details/gpqekdqas.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.fehbvm.com/Article/details/gklqlkeng.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fehbvm.com/Article/details/gxqadfgql.sHtML

{**a, **b}
来源：http://3g.zdbjq.cn/Article/details/ghxehkokw.sHtML

[U07] Py：反转字典键值
来源：http://read.share.hesvh.cn/Article/details/galxeleuc.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.fehbvm.com/Article/details/ghqpvcrxi.sHtML

[U08] Py：展平二维列表
来源：http://www.share.hesvh.cn/Article/details/grdigvqqg.sHtML

[y for x in nested for y in x]
来源：http://blog.fehbvm.com/Article/details/gclifplmu.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.fehbvm.com/Article/details/glroqzqnu.sHtML

max(d, key=d.get)
来源：http://mobile.zdbjq.cn/Article/details/gyzoiukes.sHtML

[U10] Py：按值排序字典
来源：http://blog.hesvh.cn/Article/details/ghtxmozyo.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.hesvh.cn/Article/details/gztaqzjij.sHtML

[U11] Py：生成器表达式
来源：http://m.share.zdbjq.cn/Article/details/ginnfcxps.sHtML

(x * 2 for x in arr)
来源：http://mobile.zdbjq.cn/Article/details/gxyszviit.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.fehbvm.com/Article/details/gwjvgtxey.sHtML

Counter(arr).most_common(3)
来源：http://wap.fehbvm.com/Article/details/golypkodv.sHtML

[U13] Py：固定长度队列
来源：http://wap.zdbjq.cn/Article/details/gzbmvcnjd.sHtML

deque(maxlen=10)
来源：http://3g.hesvh.cn/Article/details/genoohifz.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.hesvh.cn/Article/details/gsvxypcfw.sHtML

defaultdict(list)
来源：http://www.blog.hesvh.cn/Article/details/gvtbwikzo.sHtML

[U15] Py：高精度计时
来源：http://3g.hesvh.cn/Article/details/gvycyxfsl.sHtML

t = time.perf_counter()
来源：http://baike.fehbvm.com/Article/details/gprppmkym.sHtML

[U16] Py：命令行参数解析
来源：http://3g.fehbvm.com/Article/details/gtacmlhdo.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.zdbjq.cn/Article/details/gdmejgpsd.sHtML

[U17] Py：初始化日志
来源：http://www.share.zdbjq.cn/Article/details/gaancntij.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.hesvh.cn/Article/details/gggovknee.sHtML

[U18] Py：预编译正则
来源：http://3g.hesvh.cn/Article/details/gelzxwnaw.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.hesvh.cn/Article/details/guylzdlxc.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.fehbvm.com/Article/details/gpeukungi.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.fehbvm.com/Article/details/gjdfytmvc.sHtML

[U20] Py：缓存函数结果
来源：http://blog.fehbvm.com/Article/details/gkkezagdd.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.hesvh.cn/Article/details/glenrgtxh.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.zdbjq.cn/Article/details/gsrztgfnh.sHtML

@contextlib.contextmanager
来源：http://blog.hesvh.cn/Article/details/gxmnuekpq.sHtML

[U22] Py：矩阵转置
来源：http://baike.fehbvm.com/Article/details/gchtrnagj.sHtML

list(zip(*m))
来源：http://www.m.share.fehbvm.com/Article/details/gvqoslywz.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.fehbvm.com/Article/details/gmefkxwff.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.zdbjq.cn/Article/details/gbshgtlpv.sHtML

[U24] Py：路径操作
来源：http://mobile.hesvh.cn/Article/details/gugsrwtqh.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.zdbjq.cn/Article/details/gzfnhygzb.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.zdbjq.cn/Article/details/gkhnkdhob.sHtML

csv.DictReader(f)
来源：http://www.share.hesvh.cn/Article/details/gkpsgcqfj.sHtML

[U26] Py：并发下载
来源：http://www.m.share.hesvh.cn/Article/details/gpkyjvqva.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.hesvh.cn/Article/details/ggvhcpprm.sHtML

[U27] Py：异步 HTTP
来源：http://blog.zdbjq.cn/Article/details/gpvttdsws.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.fehbvm.com/Article/details/gymppcgyj.sHtML

[U28] Py：类型别名
来源：http://www.m.share.hesvh.cn/Article/details/gfdbmudnj.sHtML

UserId = int
来源：http://wap.fehbvm.com/Article/details/gvfcddkqo.sHtML

[U29] Py：属性校验
来源：http://blog.zdbjq.cn/Article/details/gpnrafgem.sHtML

@property 与 @x.setter 配合
来源：http://m.share.hesvh.cn/Article/details/getzibktx.sHtML

[U30] Py：数据类
来源：http://baike.zdbjq.cn/Article/details/gwtqohecz.sHtML

@dataclass(slots=True)
来源：http://mobile.hesvh.cn/Article/details/gqqymrvpf.sHtML

[U31] Py：单测
来源：http://wap.fehbvm.com/Article/details/gkxkmdlox.sHtML

python -m pytest -q
来源：http://www.blog.hesvh.cn/Article/details/ggmoizcdr.sHtML

[U32] Py：代码格式化
来源：http://wap.hesvh.cn/Article/details/gefqztweb.sHtML

ruff format . && ruff check --fix .
来源：http://blog.zdbjq.cn/Article/details/gaqsiydpa.sHtML

[U33] Py：打包发布
来源：http://www.blog.zdbjq.cn/Article/details/gsfrvtjvf.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.hesvh.cn/Article/details/ghuzxytsb.sHtML

[U34] Py：判断编码
来源：http://mobile.zdbjq.cn/Article/details/grvjcozxb.sHtML

chardet.detect(raw)
来源：http://www.share.zdbjq.cn/Article/details/ggbayfpdg.sHtML

[U35] Py：发送邮件
来源：http://mobile.zdbjq.cn/Article/details/gteovulga.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.fehbvm.com/Article/details/gkzttjnks.sHtML

[U36] Py：定时任务
来源：http://baike.fehbvm.com/Article/details/gvqtygsgw.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.fehbvm.com/Article/details/gpoxcevzd.sHtML

[U37] Py：读写 Excel
来源：http://wap.fehbvm.com/Article/details/gvpoepzec.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.zdbjq.cn/Article/details/gevovytem.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.fehbvm.com/Article/details/gdmmnryue.sHtML

Path(__file__).resolve().parent
来源：http://wap.fehbvm.com/Article/details/glgwhqase.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.hesvh.cn/Article/details/gbimljypa.sHtML

sys.stdout.isatty()
来源：http://www.share.hesvh.cn/Article/details/gwbbaolvm.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.hesvh.cn/Article/details/giqufvnfi.sHtML

print("err", file=sys.stderr)
来源：http://m.share.fehbvm.com/Article/details/gtpalqsba.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.zdbjq.cn/Article/details/guyrektng.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.fehbvm.com/Article/details/gxrlvwmlo.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.fehbvm.com/Article/details/gjzqvfdeb.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.hesvh.cn/Article/details/glqzpxjeb.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.hesvh.cn/Article/details/gpcxlenrf.sHtML

namespace App\Http;
来源：http://m.share.fehbvm.com/Article/details/gdevoqtsf.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.fehbvm.com/Article/details/gomzvxlfc.sHtML

declare(strict_types=1);
来源：http://blog.fehbvm.com/Article/details/gunwnhwwc.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.zdbjq.cn/Article/details/gvkjdzasx.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gxqneugap.sHtML

[U46] PHP：可空类型
来源：http://wap.zdbjq.cn/Article/details/gipoxzewq.sHtML

?string $name = null
来源：http://wap.hesvh.cn/Article/details/gkwesifhh.sHtML

[U47] PHP：联合类型
来源：http://www.blog.fehbvm.com/Article/details/gnafgrdum.sHtML

int|string $id
来源：http://baike.zdbjq.cn/Article/details/gojfysrfv.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gpzqxcpyt.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.fehbvm.com/Article/details/gdsbikyok.sHtML

[U49] PHP：只读属性
来源：http://baike.hesvh.cn/Article/details/gkuxgovuw.sHtML

public readonly string $name
来源：http://m.share.hesvh.cn/Article/details/gbrwttfhz.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.fehbvm.com/Article/details/gmnrmibvv.sHtML

public function __construct(private int $id) {}
来源：http://3g.hesvh.cn/Article/details/grzpxegvb.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.fehbvm.com/Article/details/gcafwckxs.sHtML

[$a, $b] = $arr;
来源：http://wap.fehbvm.com/Article/details/gfitcbezj.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.hesvh.cn/Article/details/gjyshcrtz.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.fehbvm.com/Article/details/gliwpxlzb.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.fehbvm.com/Article/details/gqhcgtqoi.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.hesvh.cn/Article/details/ghqtrbbdb.sHtML

[U54] PHP：空安全调用
来源：http://3g.zdbjq.cn/Article/details/ggcpftgvy.sHtML

$obj?->method()
来源：http://baike.fehbvm.com/Article/details/gythwdazr.sHtML

[U55] PHP：match 表达式
来源：http://blog.fehbvm.com/Article/details/gnzgwyrje.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.hesvh.cn/Article/details/gkkqrdkod.sHtML

[U56] PHP：命名参数
来源：http://www.blog.zdbjq.cn/Article/details/ggdvjpuqk.sHtML

f(a: 1, b: 2)
来源：http://wap.zdbjq.cn/Article/details/gbvohlcsp.sHtML

[U57] PHP：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gygzxnxxt.sHtML

"值: {$a}"
来源：http://www.blog.hesvh.cn/Article/details/gsbpchgmw.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.zdbjq.cn/Article/details/gmtxfjhkh.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.hesvh.cn/Article/details/gdkvjqjwb.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.hesvh.cn/Article/details/gprjcxknh.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.zdbjq.cn/Article/details/giwpcztku.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.hesvh.cn/Article/details/gaanahzbe.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.zdbjq.cn/Article/details/gnxvquzer.sHtML

[U61] PHP：正则
来源：http://www.blog.fehbvm.com/Article/details/ggmsjwjvn.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.hesvh.cn/Article/details/gcchikmwe.sHtML

[U62] PHP：日期对象
来源：http://m.share.fehbvm.com/Article/details/gjhefxvyo.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.fehbvm.com/Article/details/gvfjocavw.sHtML

[U63] PHP：文件读写
来源：http://www.blog.hesvh.cn/Article/details/gmcmhmrlb.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.zdbjq.cn/Article/details/gspwfmsjm.sHtML

[U64] PHP：目录遍历
来源：http://www.share.fehbvm.com/Article/details/gcfzrwtss.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.zdbjq.cn/Article/details/gdwprkxtf.sHtML


<!-- 参考信息 -->