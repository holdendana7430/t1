代发 wailian999

[S35] C++：map
来源：http://blog.zdbjq.cn/Article/details/gbyobuols.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gvbsqsvzz.sHtML

[S36] C++：unordered_map
来源：http://baike.zdbjq.cn/Article/details/gxzzlrcjw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gzocshzwj.sHtML

[S37] C++：set
来源：http://mobile.zdbjq.cn/Article/details/gmjpqbits.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.zdbjq.cn/Article/details/gaofsgzrc.sHtML

[S38] C++：排序
来源：http://www.blog.fehbvm.com/Article/details/ggzikxbrb.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fehbvm.com/Article/details/gazznqakb.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.zdbjq.cn/Article/details/ggehphwfo.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fehbvm.com/Article/details/gtgujzpqi.sHtML

[S40] C++：查找元素
来源：http://m.share.hesvh.cn/Article/details/gmsemwouf.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.hesvh.cn/Article/details/gdhuyfmrd.sHtML

[S41] C++：类与构造函数
来源：http://m.share.hesvh.cn/Article/details/gfcqmyvhs.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fehbvm.com/Article/details/gmsftxtvq.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fehbvm.com/Article/details/gcthsglfs.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.hesvh.cn/Article/details/gqkkfmnbu.sHtML

[S43] C++：智能指针
来源：http://www.m.share.zdbjq.cn/Article/details/ginqpvbou.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fehbvm.com/Article/details/ggpmufupf.sHtML

[S44] C++：引用传参
来源：http://wap.zdbjq.cn/Article/details/guwkjgnoy.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.hesvh.cn/Article/details/gadxwvwhn.sHtML

[S45] C++：lambda
来源：http://www.m.share.zdbjq.cn/Article/details/grbdomqep.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.zdbjq.cn/Article/details/gdwfkimkd.sHtML

[S46] C++：函数模板
来源：http://wap.fehbvm.com/Article/details/gwtgbovum.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.hesvh.cn/Article/details/gpxgyswvf.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.hesvh.cn/Article/details/gyaqlcwnb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.zdbjq.cn/Article/details/gssswwkva.sHtML

[S48] C++：逐行读文件
来源：http://3g.fehbvm.com/Article/details/ghyxztpib.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.zdbjq.cn/Article/details/gpfohgbjp.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fehbvm.com/Article/details/gyicshgbm.sHtML

[S49] C++：写文件
来源：http://wap.fehbvm.com/Article/details/gxeqfnhtw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fehbvm.com/Article/details/gihpuebed.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fehbvm.com/Article/details/gaxtrqpud.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gierldoqy.sHtML

[S51] C++：显式类型转换
来源：http://3g.zdbjq.cn/Article/details/gxntixckn.sHtML

static_cast<double>(a) / b
来源：http://3g.hesvh.cn/Article/details/gvreakwjc.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fehbvm.com/Article/details/gnjxyrbgz.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.hesvh.cn/Article/details/gfbldpdpt.sHtML

[S53] C++：移动语义
来源：http://www.m.share.zdbjq.cn/Article/details/gxuwegouh.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.zdbjq.cn/Article/details/grbpawbcz.sHtML

[S54] C++：异常处理
来源：http://mobile.hesvh.cn/Article/details/ggjzvvpjn.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.hesvh.cn/Article/details/gfigtuaaz.sHtML

[S55] C++：结构化绑定
来源：http://read.share.zdbjq.cn/Article/details/gjufrsotc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.zdbjq.cn/Article/details/ggmmtjtco.sHtML

[S56] C++：optional
来源：http://blog.hesvh.cn/Article/details/gsaopfvjn.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.hesvh.cn/Article/details/gdvnnhbcv.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.hesvh.cn/Article/details/gfybzopzh.sHtML

constexpr int N = 10;
来源：http://3g.fehbvm.com/Article/details/gsccrnvhb.sHtML

[S58] C++：命名空间
来源：http://read.share.hesvh.cn/Article/details/gatzxxruw.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.hesvh.cn/Article/details/gsbxvkpkh.sHtML

[S59] C++：静态断言
来源：http://mobile.hesvh.cn/Article/details/gecmjalia.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fehbvm.com/Article/details/gxowaamzr.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.hesvh.cn/Article/details/gegdxsyna.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fehbvm.com/Article/details/gvznyjwcv.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gewrmgnxi.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fehbvm.com/Article/details/gzhrvidgt.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gtzguxsnt.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/glykeoqtz.sHtML

println("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/ggtmwftvs.sHtML

[T02] Kotlin：变量
来源：http://blog.fehbvm.com/Article/details/gqekwwxzj.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.hesvh.cn/Article/details/gdlepvfbp.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.hesvh.cn/Article/details/gruoduott.sHtML

"值: $b"
来源：http://blog.fehbvm.com/Article/details/gackcojkv.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fehbvm.com/Article/details/gmkyxccex.sHtML

val n: String? = null;  n?.length
来源：http://wap.hesvh.cn/Article/details/guoaxbdwr.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fehbvm.com/Article/details/gmxswjxnc.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fehbvm.com/Article/details/gxkcbbits.sHtML

[T06] Kotlin：集合映射
来源：http://wap.zdbjq.cn/Article/details/ghlotkooe.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fehbvm.com/Article/details/guqwkjnzi.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.hesvh.cn/Article/details/gdongrfrp.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.zdbjq.cn/Article/details/gcbucrsci.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fehbvm.com/Article/details/gvlypyjbh.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.hesvh.cn/Article/details/gxlpplmch.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.hesvh.cn/Article/details/gsjkjhqxx.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fehbvm.com/Article/details/gspiwresw.sHtML

[T10] Kotlin：默认参数
来源：http://blog.zdbjq.cn/Article/details/goykocqqw.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fehbvm.com/Article/details/gvinjlvlp.sHtML

[T11] Kotlin：协程
来源：http://read.share.zdbjq.cn/Article/details/gtrhladhc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.hesvh.cn/Article/details/gpqhgbmok.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.zdbjq.cn/Article/details/gmjikkitw.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.hesvh.cn/Article/details/gzokaflwx.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fehbvm.com/Article/details/gauodugkd.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.hesvh.cn/Article/details/gdmamhviq.sHtML

[T14] Kotlin：循环
来源：http://read.share.zdbjq.cn/Article/details/ggjwevxjt.sHtML

for (i in 1..10) println(i)
来源：http://blog.zdbjq.cn/Article/details/goamsbadr.sHtML

[T15] Kotlin：接口
来源：http://www.blog.hesvh.cn/Article/details/glwpslfsj.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.fehbvm.com/Article/details/grjrgsdep.sHtML

[T16] Swift：Hello World
来源：http://m.share.hesvh.cn/Article/details/gptbvxcef.sHtML

print("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gkaqeqqlh.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.zdbjq.cn/Article/details/gkdmqpznl.sHtML

var a = 1;  let b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gsharxsyo.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gwgkoqdpo.sHtML

"值: \(b)"
来源：http://mobile.zdbjq.cn/Article/details/gxtlnbvgi.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fehbvm.com/Article/details/gzhzgnkct.sHtML

if let n = opt { print(n) }
来源：http://baike.fehbvm.com/Article/details/greiyxirb.sHtML

[T20] Swift：数组操作
来源：http://www.blog.zdbjq.cn/Article/details/geytdvicl.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.hesvh.cn/Article/details/gswkvgjur.sHtML

[T21] Swift：遍历
来源：http://baike.fehbvm.com/Article/details/ggdflilsy.sHtML

for x in a { print(x) }
来源：http://mobile.zdbjq.cn/Article/details/gemqwqyry.sHtML

[T22] Swift：字典
来源：http://m.share.fehbvm.com/Article/details/gflqpfdsh.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.zdbjq.cn/Article/details/gmjdvvpze.sHtML

[T23] Swift：函数
来源：http://www.blog.fehbvm.com/Article/details/gfzcdntzw.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.zdbjq.cn/Article/details/gwcwyhmje.sHtML

[T24] Swift：闭包
来源：http://mobile.hesvh.cn/Article/details/gurkmyban.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gzqrpjcks.sHtML

[T25] Swift：结构体
来源：http://www.share.zdbjq.cn/Article/details/gixlhnsnb.sHtML

struct P { var x: Int }
来源：http://baike.zdbjq.cn/Article/details/gfiiyqlib.sHtML

[T26] Swift：类与重写
来源：http://3g.hesvh.cn/Article/details/gxiijstyw.sHtML

class A: Base { override func f() {} }
来源：http://3g.fehbvm.com/Article/details/gemaseahy.sHtML

[T27] Swift：错误处理
来源：http://blog.hesvh.cn/Article/details/gvipsyiem.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fehbvm.com/Article/details/gzjdokdud.sHtML

[T28] Swift：枚举
来源：http://www.share.hesvh.cn/Article/details/gqnbzctsk.sHtML

enum Color { case red, green }
来源：http://read.share.fehbvm.com/Article/details/gyslaauma.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.zdbjq.cn/Article/details/ghzvmzcsa.sHtML

guard let x = opt else { return }
来源：http://www.blog.hesvh.cn/Article/details/geasnfkua.sHtML

[T30] Swift：协议
来源：http://wap.fehbvm.com/Article/details/gxkiqnbjx.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.zdbjq.cn/Article/details/gnojcrvto.sHtML

[T31] Lua：Hello World
来源：http://wap.fehbvm.com/Article/details/ghdplhego.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/gihccdtnd.sHtML

[T32] Lua：局部变量
来源：http://m.share.hesvh.cn/Article/details/gmzssbujl.sHtML

local a = 1
来源：http://wap.fehbvm.com/Article/details/gliycuwpm.sHtML

[T33] Lua：表（数组）
来源：http://blog.zdbjq.cn/Article/details/gfxwaomov.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fehbvm.com/Article/details/gmaedbham.sHtML

[T34] Lua：遍历表
来源：http://mobile.hesvh.cn/Article/details/gragybuhe.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fehbvm.com/Article/details/gxrjozdry.sHtML

[T35] Lua：字典表
来源：http://wap.hesvh.cn/Article/details/gafqekcrz.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.fehbvm.com/Article/details/gvrwsjurq.sHtML

[T36] Lua：函数
来源：http://blog.zdbjq.cn/Article/details/gvyeqsydu.sHtML

function add(a, b) return a + b end
来源：http://www.blog.zdbjq.cn/Article/details/glwypszmw.sHtML

[T37] Lua：字符串拼接
来源：http://3g.hesvh.cn/Article/details/gjnzmhwvd.sHtML

"a" .. "b"
来源：http://www.blog.hesvh.cn/Article/details/gyxbrktvv.sHtML

[T38] Lua：条件
来源：http://mobile.zdbjq.cn/Article/details/garwgscko.sHtML

if x > 0 then print("正") end
来源：http://blog.hesvh.cn/Article/details/gqozkjmqj.sHtML

[T39] Lua：模式匹配
来源：http://mobile.fehbvm.com/Article/details/glxnmsagz.sHtML

string.find(s, "%d+")
来源：http://www.m.share.hesvh.cn/Article/details/glfkibucc.sHtML

[T40] Lua：元表
来源：http://www.m.share.fehbvm.com/Article/details/gzxvmfure.sHtML

setmetatable({}, { __index = base })
来源：http://wap.zdbjq.cn/Article/details/grujatshk.sHtML

[T41] Perl：Hello World
来源：http://www.share.hesvh.cn/Article/details/gpvwpszrn.sHtML

print "Hello\n";
来源：http://www.m.share.hesvh.cn/Article/details/gmemfbjlv.sHtML

[T42] Perl：变量类型
来源：http://3g.hesvh.cn/Article/details/gbzkykfnu.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.fehbvm.com/Article/details/gegclhcgi.sHtML

[T43] Perl：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gmjrbqglh.sHtML

"值: $a"
来源：http://www.blog.hesvh.cn/Article/details/gszesoqyu.sHtML

[T44] Perl：条件
来源：http://www.blog.fehbvm.com/Article/details/gbintjpnx.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.zdbjq.cn/Article/details/gfzwdkxoe.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.fehbvm.com/Article/details/gqamyibjy.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.hesvh.cn/Article/details/gmkvpglnd.sHtML

[T46] Perl：哈希操作
来源：http://read.share.zdbjq.cn/Article/details/gstjkfqkz.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.zdbjq.cn/Article/details/gtkrddnrj.sHtML

[T47] Perl：正则捕获
来源：http://mobile.fehbvm.com/Article/details/gwkyhisku.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.hesvh.cn/Article/details/gqaypjoyv.sHtML

[T48] Perl：正则替换
来源：http://www.blog.zdbjq.cn/Article/details/gsgjvaupp.sHtML

$s =~ s/old/new/g;
来源：http://mobile.zdbjq.cn/Article/details/gamxkwphi.sHtML

[T49] Perl：函数
来源：http://mobile.fehbvm.com/Article/details/gncrgbbtp.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gvyqpltow.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gfiwwmusq.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.zdbjq.cn/Article/details/gxzfmghmd.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.hesvh.cn/Article/details/gfinyccpt.sHtML

[T51] Scala：Hello World
来源：http://blog.fehbvm.com/Article/details/gvjhdgrke.sHtML

println("Hello")
来源：http://read.share.hesvh.cn/Article/details/ggfycxcrb.sHtML

[T52] Scala：变量
来源：http://www.blog.fehbvm.com/Article/details/gitccxqqr.sHtML

val a = 1;  var b = 2
来源：http://www.share.fehbvm.com/Article/details/gqxtarmip.sHtML

[T53] Scala：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gnnomgrns.sHtML

s"值: $b"
来源：http://www.m.share.zdbjq.cn/Article/details/gnfkqubrz.sHtML

[T54] Scala：集合映射
来源：http://www.share.zdbjq.cn/Article/details/gigmjkzvb.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.hesvh.cn/Article/details/ghrgvspqt.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/grqpauuio.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.hesvh.cn/Article/details/gymzcjbyc.sHtML

[T56] Scala：样例类
来源：http://www.blog.zdbjq.cn/Article/details/gdebabipw.sHtML

case class User(name: String, age: Int)
来源：http://blog.fehbvm.com/Article/details/gfsxuaulw.sHtML

[T57] Scala：模式匹配
来源：http://m.share.hesvh.cn/Article/details/gfkevjxih.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.zdbjq.cn/Article/details/gmpjrdryl.sHtML

[T58] Scala：函数定义
来源：http://blog.fehbvm.com/Article/details/gbhwvudjr.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fehbvm.com/Article/details/gqfpkprhn.sHtML

[T59] Scala：循环
来源：http://mobile.fehbvm.com/Article/details/guwnmkker.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/gnusngymp.sHtML

[T60] Scala：折叠
来源：http://www.share.zdbjq.cn/Article/details/gkfadapyy.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.hesvh.cn/Article/details/gfkbdjjhk.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gdnbmsysk.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.zdbjq.cn/Article/details/gtoewuoyr.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/geuljheaa.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.zdbjq.cn/Article/details/gmbjxrqpy.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.zdbjq.cn/Article/details/gcxqyeigx.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.zdbjq.cn/Article/details/glulhypch.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.zdbjq.cn/Article/details/gzgppfdxy.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.fehbvm.com/Article/details/gbnzqfcfj.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.hesvh.cn/Article/details/gsqekkbjp.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.hesvh.cn/Article/details/gmqrgzzpf.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.hesvh.cn/Article/details/gtqobngyn.sHtML

[U05] Py：列表去重且保序
来源：http://blog.hesvh.cn/Article/details/gssjbrcjn.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.fehbvm.com/Article/details/gqjlllkpv.sHtML

[U06] Py：合并两个字典
来源：http://read.share.zdbjq.cn/Article/details/gbvabpxde.sHtML

{**a, **b}
来源：http://wap.zdbjq.cn/Article/details/gvzfmdcpz.sHtML

[U07] Py：反转字典键值
来源：http://m.share.zdbjq.cn/Article/details/gqvglreyq.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.zdbjq.cn/Article/details/gjxcpkbcj.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.zdbjq.cn/Article/details/gwjnnnnpv.sHtML

[y for x in nested for y in x]
来源：http://www.share.zdbjq.cn/Article/details/gugegivzl.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.hesvh.cn/Article/details/gvbrouxnx.sHtML

max(d, key=d.get)
来源：http://www.share.fehbvm.com/Article/details/gznsipanl.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.fehbvm.com/Article/details/guxefhcxu.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.hesvh.cn/Article/details/gxohhhkrl.sHtML

[U11] Py：生成器表达式
来源：http://mobile.zdbjq.cn/Article/details/gofiakext.sHtML

(x * 2 for x in arr)
来源：http://read.share.zdbjq.cn/Article/details/gcwvcgzij.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.hesvh.cn/Article/details/gyrczdvlu.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.hesvh.cn/Article/details/gcljdcazs.sHtML

[U13] Py：固定长度队列
来源：http://read.share.zdbjq.cn/Article/details/gscmsjtuc.sHtML

deque(maxlen=10)
来源：http://wap.hesvh.cn/Article/details/gmfnkdnxs.sHtML

[U14] Py：分组收集到列表
来源：http://blog.zdbjq.cn/Article/details/gaihsxiaw.sHtML

defaultdict(list)
来源：http://m.share.zdbjq.cn/Article/details/gkmvkzwrm.sHtML

[U15] Py：高精度计时
来源：http://read.share.fehbvm.com/Article/details/gthppueuy.sHtML

t = time.perf_counter()
来源：http://baike.hesvh.cn/Article/details/gvclvyczb.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.fehbvm.com/Article/details/gmyojrcfd.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.hesvh.cn/Article/details/glivzimez.sHtML

[U17] Py：初始化日志
来源：http://m.share.fehbvm.com/Article/details/gncrntnzb.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.hesvh.cn/Article/details/getrinadj.sHtML

[U18] Py：预编译正则
来源：http://www.blog.zdbjq.cn/Article/details/gmerbqfek.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.zdbjq.cn/Article/details/gptmebqgv.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.fehbvm.com/Article/details/guccupsuo.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.zdbjq.cn/Article/details/grlpbtnqp.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.zdbjq.cn/Article/details/gakpunenw.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.fehbvm.com/Article/details/gyzgsrjkw.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.zdbjq.cn/Article/details/gvxabirxa.sHtML

@contextlib.contextmanager
来源：http://blog.zdbjq.cn/Article/details/gljuhjwbu.sHtML

[U22] Py：矩阵转置
来源：http://blog.zdbjq.cn/Article/details/gzfpglwxh.sHtML

list(zip(*m))
来源：http://3g.zdbjq.cn/Article/details/gfmmilumw.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.fehbvm.com/Article/details/gloqvqqvo.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.fehbvm.com/Article/details/gctmlwmbg.sHtML

[U24] Py：路径操作
来源：http://mobile.zdbjq.cn/Article/details/gusmxmytg.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.zdbjq.cn/Article/details/ggjfbptsa.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.hesvh.cn/Article/details/gfjnidvdx.sHtML

csv.DictReader(f)
来源：http://www.blog.hesvh.cn/Article/details/glwblrxzc.sHtML

[U26] Py：并发下载
来源：http://m.share.zdbjq.cn/Article/details/gpscaygjo.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.hesvh.cn/Article/details/gijglnluo.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.zdbjq.cn/Article/details/gdwxtwcvy.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.hesvh.cn/Article/details/gnhonxudh.sHtML

[U28] Py：类型别名
来源：http://wap.fehbvm.com/Article/details/gvhvjolkq.sHtML

UserId = int
来源：http://wap.hesvh.cn/Article/details/ghxonzzhh.sHtML

[U29] Py：属性校验
来源：http://www.m.share.fehbvm.com/Article/details/gbmgszvmb.sHtML

@property 与 @x.setter 配合
来源：http://blog.hesvh.cn/Article/details/grlmrpfxn.sHtML

[U30] Py：数据类
来源：http://read.share.hesvh.cn/Article/details/gqzrnpofe.sHtML

@dataclass(slots=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gcvoroyci.sHtML

[U31] Py：单测
来源：http://www.blog.fehbvm.com/Article/details/ghdazahki.sHtML

python -m pytest -q
来源：http://blog.fehbvm.com/Article/details/gxzmpcpyi.sHtML

[U32] Py：代码格式化
来源：http://wap.hesvh.cn/Article/details/gpbkuqmfy.sHtML

ruff format . && ruff check --fix .
来源：http://wap.zdbjq.cn/Article/details/gehfhnrdh.sHtML

[U33] Py：打包发布
来源：http://m.share.hesvh.cn/Article/details/gmvvcxsux.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.fehbvm.com/Article/details/gsibozvem.sHtML

[U34] Py：判断编码
来源：http://m.share.fehbvm.com/Article/details/gkeqhksrg.sHtML

chardet.detect(raw)
来源：http://m.share.zdbjq.cn/Article/details/gyabpqckc.sHtML

[U35] Py：发送邮件
来源：http://www.blog.hesvh.cn/Article/details/glkjovukt.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.zdbjq.cn/Article/details/gyjfdrzbu.sHtML

[U36] Py：定时任务
来源：http://wap.hesvh.cn/Article/details/gfmwbwsux.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.hesvh.cn/Article/details/gfdshpxfe.sHtML

[U37] Py：读写 Excel
来源：http://baike.zdbjq.cn/Article/details/gibnxeqqs.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.hesvh.cn/Article/details/grxgopgzs.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.fehbvm.com/Article/details/gadctokjq.sHtML

Path(__file__).resolve().parent
来源：http://3g.hesvh.cn/Article/details/gcczjhkoa.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.zdbjq.cn/Article/details/gjpvuynzg.sHtML

sys.stdout.isatty()
来源：http://3g.fehbvm.com/Article/details/goanzdqdx.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.fehbvm.com/Article/details/garihnbwo.sHtML

print("err", file=sys.stderr)
来源：http://3g.hesvh.cn/Article/details/gjoeekoly.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.hesvh.cn/Article/details/gtfgpzvuc.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.hesvh.cn/Article/details/gehscntzp.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.zdbjq.cn/Article/details/gzqimvqpc.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.fehbvm.com/Article/details/gjgxjgcyc.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.hesvh.cn/Article/details/gltmqmhmk.sHtML

namespace App\Http;
来源：http://baike.hesvh.cn/Article/details/grrhabmmj.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.hesvh.cn/Article/details/ghyrkeqwg.sHtML

declare(strict_types=1);
来源：http://read.share.hesvh.cn/Article/details/gapkpcfhs.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.fehbvm.com/Article/details/gqmifmolx.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/ggltzkkwg.sHtML

[U46] PHP：可空类型
来源：http://read.share.fehbvm.com/Article/details/gcvgpxsvl.sHtML

?string $name = null
来源：http://www.m.share.zdbjq.cn/Article/details/grrpkzeof.sHtML

[U47] PHP：联合类型
来源：http://m.share.fehbvm.com/Article/details/ggcyapgbd.sHtML

int|string $id
来源：http://read.share.fehbvm.com/Article/details/gzkuspqbd.sHtML

[U48] PHP：纯枚举
来源：http://read.share.fehbvm.com/Article/details/gamgvmpim.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.zdbjq.cn/Article/details/gywikkrgi.sHtML

[U49] PHP：只读属性
来源：http://3g.zdbjq.cn/Article/details/ghhqrruvl.sHtML

public readonly string $name
来源：http://wap.hesvh.cn/Article/details/getlzygvp.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.fehbvm.com/Article/details/gfplgkhjh.sHtML

public function __construct(private int $id) {}
来源：http://www.share.zdbjq.cn/Article/details/girxvcoai.sHtML

[U51] PHP：数组解构
来源：http://www.blog.zdbjq.cn/Article/details/genvlpxnm.sHtML

[$a, $b] = $arr;
来源：http://blog.zdbjq.cn/Article/details/gmexjkdof.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.zdbjq.cn/Article/details/gjybfpibv.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.zdbjq.cn/Article/details/gtbztbiht.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.zdbjq.cn/Article/details/gcczefyrq.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.fehbvm.com/Article/details/gmwqlatgv.sHtML

[U54] PHP：空安全调用
来源：http://wap.fehbvm.com/Article/details/giazcksyr.sHtML

$obj?->method()
来源：http://read.share.zdbjq.cn/Article/details/gdbooazny.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.zdbjq.cn/Article/details/gzquyjoik.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.zdbjq.cn/Article/details/gshjrzujy.sHtML

[U56] PHP：命名参数
来源：http://read.share.hesvh.cn/Article/details/gtnidjzkh.sHtML

f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/ggxrrckdn.sHtML

[U57] PHP：字符串插值
来源：http://3g.fehbvm.com/Article/details/gitmgrger.sHtML

"值: {$a}"
来源：http://wap.zdbjq.cn/Article/details/gtdmqsapu.sHtML

[U58] PHP：数组三件套
来源：http://wap.fehbvm.com/Article/details/gzsfkggay.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.zdbjq.cn/Article/details/gulwilxkr.sHtML

[U59] PHP：自定义排序
来源：http://www.share.hesvh.cn/Article/details/glejmfgrn.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.zdbjq.cn/Article/details/gcnibqegf.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.zdbjq.cn/Article/details/gfdqtgxkv.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.zdbjq.cn/Article/details/ggxxxjoty.sHtML


<!-- 参考信息 -->