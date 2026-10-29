代发 wailian999

[S33] C++：vector 增删
来源：http://mobile.fehbvm.com/Article/details/gklcbrgcr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.zdbjq.cn/Article/details/ghgkfiyyq.sHtML

[S34] C++：遍历 vector
来源：http://wap.hesvh.cn/Article/details/gjbhhuetr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.zdbjq.cn/Article/details/gawalaulh.sHtML

[S35] C++：map
来源：http://www.share.fehbvm.com/Article/details/geskjlvfr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gsgsdttof.sHtML

[S36] C++：unordered_map
来源：http://blog.hesvh.cn/Article/details/gozvoweto.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gsxqjvlnb.sHtML

[S37] C++：set
来源：http://m.share.fehbvm.com/Article/details/gcmpvelga.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.zdbjq.cn/Article/details/gvfsrxkyc.sHtML

[S38] C++：排序
来源：http://m.share.hesvh.cn/Article/details/gtxkddapo.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.hesvh.cn/Article/details/gklububfn.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fehbvm.com/Article/details/guxsyjfts.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.hesvh.cn/Article/details/ggzfqqunv.sHtML

[S40] C++：查找元素
来源：http://read.share.hesvh.cn/Article/details/gllhjruou.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.zdbjq.cn/Article/details/giozyefdb.sHtML

[S41] C++：类与构造函数
来源：http://www.share.zdbjq.cn/Article/details/giowrkrcs.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fehbvm.com/Article/details/gwvcpauxw.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fehbvm.com/Article/details/gfxzpebzo.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fehbvm.com/Article/details/gbopkhjsa.sHtML

[S43] C++：智能指针
来源：http://wap.zdbjq.cn/Article/details/ghnxifsya.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.zdbjq.cn/Article/details/glecyowxi.sHtML

[S44] C++：引用传参
来源：http://baike.fehbvm.com/Article/details/gqrephonq.sHtML

void inc(int &x) { ++x; }
来源：http://blog.hesvh.cn/Article/details/gkcutdktj.sHtML

[S45] C++：lambda
来源：http://baike.fehbvm.com/Article/details/gqtkbevnj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fehbvm.com/Article/details/gskzsimvd.sHtML

[S46] C++：函数模板
来源：http://www.m.share.hesvh.cn/Article/details/gloxldmeo.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.hesvh.cn/Article/details/gtfzlifbo.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.zdbjq.cn/Article/details/gchxydthx.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fehbvm.com/Article/details/gpouqgwfy.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gksvlenmp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.zdbjq.cn/Article/details/gfwbilvkd.sHtML

while (std::getline(in, line)) { }
来源：http://blog.zdbjq.cn/Article/details/gqgjyexra.sHtML

[S49] C++：写文件
来源：http://wap.fehbvm.com/Article/details/ghcnxnxnz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.hesvh.cn/Article/details/geuskrndq.sHtML

[S50] C++：格式化数字
来源：http://3g.hesvh.cn/Article/details/gpoyvcikm.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gcpnlnbsg.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fehbvm.com/Article/details/gdiqfjztg.sHtML

static_cast<double>(a) / b
来源：http://www.blog.zdbjq.cn/Article/details/gqkdkddxp.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.hesvh.cn/Article/details/gucruwuic.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.hesvh.cn/Article/details/grbfaljhe.sHtML

[S53] C++：移动语义
来源：http://baike.fehbvm.com/Article/details/godhkgsbh.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fehbvm.com/Article/details/gpkyvkcjx.sHtML

[S54] C++：异常处理
来源：http://www.m.share.zdbjq.cn/Article/details/gvjhyowbe.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gxhpibkxz.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fehbvm.com/Article/details/gmzkbzrmr.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fehbvm.com/Article/details/girhdcxeo.sHtML

[S56] C++：optional
来源：http://m.share.hesvh.cn/Article/details/gyurmbncw.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fehbvm.com/Article/details/guxhuqdeh.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.hesvh.cn/Article/details/grkysondn.sHtML

constexpr int N = 10;
来源：http://read.share.hesvh.cn/Article/details/gtrhddxlc.sHtML

[S58] C++：命名空间
来源：http://www.share.fehbvm.com/Article/details/gajfqpvte.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fehbvm.com/Article/details/gbmlecnua.sHtML

[S59] C++：静态断言
来源：http://mobile.hesvh.cn/Article/details/gqjzkniwu.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.zdbjq.cn/Article/details/gtvgosuon.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.hesvh.cn/Article/details/gslnvokls.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.hesvh.cn/Article/details/gcuokgffo.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gytjewgwq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fehbvm.com/Article/details/gzoxkqojm.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gyxmsbtfm.sHtML

[T01] Kotlin：Hello World
来源：http://blog.zdbjq.cn/Article/details/gorxpqvds.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/gcdkcaicq.sHtML

[T02] Kotlin：变量
来源：http://read.share.fehbvm.com/Article/details/gkixydebu.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.zdbjq.cn/Article/details/gmflciiem.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fehbvm.com/Article/details/goscmimar.sHtML

"值: $b"
来源：http://blog.zdbjq.cn/Article/details/gxmfvvruu.sHtML

[T04] Kotlin：空安全
来源：http://3g.hesvh.cn/Article/details/gmzsfdyba.sHtML

val n: String? = null;  n?.length
来源：http://3g.zdbjq.cn/Article/details/gmwkwbjik.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.zdbjq.cn/Article/details/ggjowfwkq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.zdbjq.cn/Article/details/gaujnokhz.sHtML

[T06] Kotlin：集合映射
来源：http://baike.zdbjq.cn/Article/details/gbasfembp.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.hesvh.cn/Article/details/gjnkgunij.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.zdbjq.cn/Article/details/guhwlglnx.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.hesvh.cn/Article/details/grzcwslxw.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.zdbjq.cn/Article/details/gedcusgbn.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fehbvm.com/Article/details/gmekzsmgj.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.zdbjq.cn/Article/details/gnqoogevu.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.hesvh.cn/Article/details/gbzicftdx.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fehbvm.com/Article/details/ggyeqkkby.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fehbvm.com/Article/details/gvcuqznif.sHtML

[T11] Kotlin：协程
来源：http://wap.fehbvm.com/Article/details/gqqtgajik.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.hesvh.cn/Article/details/gcxdnvyfm.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fehbvm.com/Article/details/gaowfxrgq.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gwvfyshbc.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fehbvm.com/Article/details/gvxcuulnw.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fehbvm.com/Article/details/glzflrrrd.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.zdbjq.cn/Article/details/gvtuhlmek.sHtML

for (i in 1..10) println(i)
来源：http://blog.hesvh.cn/Article/details/guocsfhzt.sHtML

[T15] Kotlin：接口
来源：http://3g.zdbjq.cn/Article/details/gcsgnckvh.sHtML

interface Shape { fun area(): Double }
来源：http://blog.hesvh.cn/Article/details/grvvxnqtf.sHtML

[T16] Swift：Hello World
来源：http://read.share.hesvh.cn/Article/details/gfcgztugu.sHtML

print("Hello")
来源：http://www.share.fehbvm.com/Article/details/grkjiwyse.sHtML

[T17] Swift：变量与常量
来源：http://mobile.hesvh.cn/Article/details/guomujxit.sHtML

var a = 1;  let b = 2
来源：http://www.blog.hesvh.cn/Article/details/gpebbdmuw.sHtML

[T18] Swift：字符串插值
来源：http://wap.fehbvm.com/Article/details/ghjezgmkd.sHtML

"值: \(b)"
来源：http://mobile.fehbvm.com/Article/details/gdxogabaj.sHtML

[T19] Swift：可选绑定
来源：http://read.share.zdbjq.cn/Article/details/gvnyurvmb.sHtML

if let n = opt { print(n) }
来源：http://read.share.zdbjq.cn/Article/details/gbeoeofks.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.zdbjq.cn/Article/details/glwqfyyil.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fehbvm.com/Article/details/gwpurcecn.sHtML

[T21] Swift：遍历
来源：http://m.share.zdbjq.cn/Article/details/gluklonyk.sHtML

for x in a { print(x) }
来源：http://mobile.fehbvm.com/Article/details/ggribpccf.sHtML

[T22] Swift：字典
来源：http://3g.fehbvm.com/Article/details/gbpplhciq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.zdbjq.cn/Article/details/gkodhotjv.sHtML

[T23] Swift：函数
来源：http://read.share.zdbjq.cn/Article/details/gxczwzess.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.zdbjq.cn/Article/details/gjfkjxzxj.sHtML

[T24] Swift：闭包
来源：http://baike.hesvh.cn/Article/details/gupkpgswx.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fehbvm.com/Article/details/gtfspvlhh.sHtML

[T25] Swift：结构体
来源：http://mobile.hesvh.cn/Article/details/geqmvxbzt.sHtML

struct P { var x: Int }
来源：http://www.share.zdbjq.cn/Article/details/gvgpizglf.sHtML

[T26] Swift：类与重写
来源：http://blog.hesvh.cn/Article/details/gfrpwrarl.sHtML

class A: Base { override func f() {} }
来源：http://www.share.hesvh.cn/Article/details/gjlsqbpjg.sHtML

[T27] Swift：错误处理
来源：http://wap.fehbvm.com/Article/details/gcnuzkhvb.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.hesvh.cn/Article/details/gnvdtavuk.sHtML

[T28] Swift：枚举
来源：http://www.m.share.hesvh.cn/Article/details/gdhhahazr.sHtML

enum Color { case red, green }
来源：http://wap.hesvh.cn/Article/details/gievmatei.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.zdbjq.cn/Article/details/gferycaxo.sHtML

guard let x = opt else { return }
来源：http://www.m.share.hesvh.cn/Article/details/gewlwaavt.sHtML

[T30] Swift：协议
来源：http://wap.hesvh.cn/Article/details/gklhojpvb.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fehbvm.com/Article/details/gyoublebg.sHtML

[T31] Lua：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gyziedtqa.sHtML

print("Hello")
来源：http://read.share.fehbvm.com/Article/details/gluiyrtrh.sHtML

[T32] Lua：局部变量
来源：http://read.share.zdbjq.cn/Article/details/gcweyidxr.sHtML

local a = 1
来源：http://blog.hesvh.cn/Article/details/gidjrdmkg.sHtML

[T33] Lua：表（数组）
来源：http://3g.hesvh.cn/Article/details/gaynigurz.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fehbvm.com/Article/details/gcilekulv.sHtML

[T34] Lua：遍历表
来源：http://www.share.fehbvm.com/Article/details/gxpuirtap.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.hesvh.cn/Article/details/gnftaazit.sHtML

[T35] Lua：字典表
来源：http://m.share.hesvh.cn/Article/details/geveobdlu.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.fehbvm.com/Article/details/gekawgswv.sHtML

[T36] Lua：函数
来源：http://www.m.share.fehbvm.com/Article/details/gfwqazxvs.sHtML

function add(a, b) return a + b end
来源：http://blog.fehbvm.com/Article/details/gycvqopze.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.hesvh.cn/Article/details/gempjgdzc.sHtML

"a" .. "b"
来源：http://www.share.zdbjq.cn/Article/details/ghgjuctno.sHtML

[T38] Lua：条件
来源：http://www.m.share.fehbvm.com/Article/details/gsthpsslc.sHtML

if x > 0 then print("正") end
来源：http://3g.zdbjq.cn/Article/details/gneeubgou.sHtML

[T39] Lua：模式匹配
来源：http://m.share.zdbjq.cn/Article/details/gytuvqmsv.sHtML

string.find(s, "%d+")
来源：http://mobile.zdbjq.cn/Article/details/giinidnut.sHtML

[T40] Lua：元表
来源：http://www.m.share.fehbvm.com/Article/details/gvfdlllht.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.hesvh.cn/Article/details/gctmpdrnt.sHtML

[T41] Perl：Hello World
来源：http://m.share.hesvh.cn/Article/details/gncfwhute.sHtML

print "Hello\n";
来源：http://blog.fehbvm.com/Article/details/gdglpwmzv.sHtML

[T42] Perl：变量类型
来源：http://blog.zdbjq.cn/Article/details/gwlosqzqn.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.zdbjq.cn/Article/details/gicwzsuqh.sHtML

[T43] Perl：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gwvtexyfx.sHtML

"值: $a"
来源：http://3g.fehbvm.com/Article/details/gvtbndvva.sHtML

[T44] Perl：条件
来源：http://www.share.hesvh.cn/Article/details/gygzshjcf.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.hesvh.cn/Article/details/gezhhxjpg.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.zdbjq.cn/Article/details/gpfqlxkyv.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.zdbjq.cn/Article/details/grgaoepnp.sHtML

[T46] Perl：哈希操作
来源：http://blog.zdbjq.cn/Article/details/gczcgqpoa.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.fehbvm.com/Article/details/ghruanhky.sHtML

[T47] Perl：正则捕获
来源：http://baike.fehbvm.com/Article/details/gefiihgeb.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.zdbjq.cn/Article/details/ghvwurlrj.sHtML

[T48] Perl：正则替换
来源：http://baike.fehbvm.com/Article/details/ggvllqmmx.sHtML

$s =~ s/old/new/g;
来源：http://3g.fehbvm.com/Article/details/gohkuwmnm.sHtML

[T49] Perl：函数
来源：http://blog.fehbvm.com/Article/details/gezzubokw.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gblndjmke.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gipufjmuy.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.zdbjq.cn/Article/details/gdhbrymel.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.fehbvm.com/Article/details/gykdmqjai.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gcmcyrdxx.sHtML

println("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gwxutnggp.sHtML

[T52] Scala：变量
来源：http://wap.hesvh.cn/Article/details/ghriftawm.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.hesvh.cn/Article/details/gbajixrjt.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/ggotxmmqw.sHtML

s"值: $b"
来源：http://baike.zdbjq.cn/Article/details/gbfnnttrs.sHtML

[T54] Scala：集合映射
来源：http://www.share.fehbvm.com/Article/details/ghhiphopt.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.hesvh.cn/Article/details/gkdvaqlfz.sHtML

[T55] Scala：集合过滤
来源：http://mobile.hesvh.cn/Article/details/geeovzzyj.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.fehbvm.com/Article/details/gnkthapnw.sHtML

[T56] Scala：样例类
来源：http://blog.zdbjq.cn/Article/details/gfdakgzxc.sHtML

case class User(name: String, age: Int)
来源：http://wap.zdbjq.cn/Article/details/gtlqloakl.sHtML

[T57] Scala：模式匹配
来源：http://m.share.hesvh.cn/Article/details/gdnjcthkf.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.hesvh.cn/Article/details/glzlvstax.sHtML

[T58] Scala：函数定义
来源：http://blog.fehbvm.com/Article/details/ginijxuuh.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.hesvh.cn/Article/details/gyqtxozxn.sHtML

[T59] Scala：循环
来源：http://baike.hesvh.cn/Article/details/gdultwioz.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/gpatipzzl.sHtML

[T60] Scala：折叠
来源：http://baike.fehbvm.com/Article/details/gntsvpsrm.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.hesvh.cn/Article/details/glgqplaks.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gjereynfo.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.fehbvm.com/Article/details/gwwpnragl.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/grviomtpt.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.zdbjq.cn/Article/details/gzxjefkey.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.zdbjq.cn/Article/details/gmeamrnlx.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.zdbjq.cn/Article/details/gelpicryx.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fehbvm.com/Article/details/gmwdnuhdo.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.fehbvm.com/Article/details/gsqlhftpa.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.hesvh.cn/Article/details/grsoobody.sHtML

[U04] Py：变量调试打印
来源：http://blog.fehbvm.com/Article/details/gyzgktveb.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.fehbvm.com/Article/details/gzsrxhxzj.sHtML

[U05] Py：列表去重且保序
来源：http://3g.hesvh.cn/Article/details/gilfwfijm.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.zdbjq.cn/Article/details/gkawwbnpa.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.zdbjq.cn/Article/details/gjrutyfst.sHtML

{**a, **b}
来源：http://read.share.zdbjq.cn/Article/details/gnsuhjmkk.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.zdbjq.cn/Article/details/gkadogwnl.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.fehbvm.com/Article/details/guwnhmffn.sHtML

[U08] Py：展平二维列表
来源：http://www.share.zdbjq.cn/Article/details/ghbesxrqw.sHtML

[y for x in nested for y in x]
来源：http://m.share.hesvh.cn/Article/details/gxtmtgsgh.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.fehbvm.com/Article/details/gilikpvxv.sHtML

max(d, key=d.get)
来源：http://m.share.fehbvm.com/Article/details/gzlyamdky.sHtML

[U10] Py：按值排序字典
来源：http://3g.hesvh.cn/Article/details/ghsepwywo.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.zdbjq.cn/Article/details/gczrvmbfr.sHtML

[U11] Py：生成器表达式
来源：http://baike.zdbjq.cn/Article/details/gdgtzkcng.sHtML

(x * 2 for x in arr)
来源：http://www.share.fehbvm.com/Article/details/gdclpacqc.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.fehbvm.com/Article/details/goqnphkat.sHtML

Counter(arr).most_common(3)
来源：http://read.share.zdbjq.cn/Article/details/gepgdfvpz.sHtML

[U13] Py：固定长度队列
来源：http://www.share.hesvh.cn/Article/details/gtwlyyzbv.sHtML

deque(maxlen=10)
来源：http://read.share.zdbjq.cn/Article/details/gjghqtekq.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.fehbvm.com/Article/details/gfsntygbr.sHtML

defaultdict(list)
来源：http://www.m.share.zdbjq.cn/Article/details/glbrktwfh.sHtML

[U15] Py：高精度计时
来源：http://www.blog.fehbvm.com/Article/details/gchedvqbc.sHtML

t = time.perf_counter()
来源：http://www.share.zdbjq.cn/Article/details/gapvretgs.sHtML

[U16] Py：命令行参数解析
来源：http://wap.hesvh.cn/Article/details/gmfxzzsot.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.fehbvm.com/Article/details/glfhkeqrd.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.hesvh.cn/Article/details/gevhkvlcp.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.zdbjq.cn/Article/details/gphrbwxbb.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fehbvm.com/Article/details/gkhdzilab.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.zdbjq.cn/Article/details/gcjekzkvm.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.fehbvm.com/Article/details/grpbssjbf.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.fehbvm.com/Article/details/gvfinodqd.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.hesvh.cn/Article/details/gnzazyzxm.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.hesvh.cn/Article/details/gtdeskeew.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.hesvh.cn/Article/details/gduhogzhn.sHtML

@contextlib.contextmanager
来源：http://blog.fehbvm.com/Article/details/gxqanpdip.sHtML

[U22] Py：矩阵转置
来源：http://mobile.zdbjq.cn/Article/details/gwclmbfqi.sHtML

list(zip(*m))
来源：http://3g.zdbjq.cn/Article/details/gdssaidnb.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.zdbjq.cn/Article/details/godjlxjxw.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.fehbvm.com/Article/details/gurpiuweq.sHtML

[U24] Py：路径操作
来源：http://www.m.share.hesvh.cn/Article/details/gjkcfpyfk.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.fehbvm.com/Article/details/gnkbnueuj.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.fehbvm.com/Article/details/gfyfkxcvy.sHtML

csv.DictReader(f)
来源：http://blog.zdbjq.cn/Article/details/gbktsacbh.sHtML

[U26] Py：并发下载
来源：http://www.share.fehbvm.com/Article/details/gwfhaszcy.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.fehbvm.com/Article/details/gnppsbymi.sHtML

[U27] Py：异步 HTTP
来源：http://baike.hesvh.cn/Article/details/gnrvvmdcb.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.zdbjq.cn/Article/details/gubntgdrl.sHtML

[U28] Py：类型别名
来源：http://read.share.zdbjq.cn/Article/details/gobnphrtk.sHtML

UserId = int
来源：http://mobile.hesvh.cn/Article/details/govjsvbls.sHtML

[U29] Py：属性校验
来源：http://www.m.share.fehbvm.com/Article/details/gamvkeham.sHtML

@property 与 @x.setter 配合
来源：http://baike.zdbjq.cn/Article/details/gzoymunef.sHtML

[U30] Py：数据类
来源：http://blog.zdbjq.cn/Article/details/gayzshlku.sHtML

@dataclass(slots=True)
来源：http://read.share.zdbjq.cn/Article/details/gtavmvdnn.sHtML

[U31] Py：单测
来源：http://baike.hesvh.cn/Article/details/gopuyhzji.sHtML

python -m pytest -q
来源：http://wap.fehbvm.com/Article/details/gropbyuht.sHtML

[U32] Py：代码格式化
来源：http://www.blog.zdbjq.cn/Article/details/gqedahvre.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.zdbjq.cn/Article/details/gnrbstohx.sHtML

[U33] Py：打包发布
来源：http://www.share.hesvh.cn/Article/details/gbxhrdxuk.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.zdbjq.cn/Article/details/goljmgqse.sHtML

[U34] Py：判断编码
来源：http://m.share.hesvh.cn/Article/details/gvxhngejf.sHtML

chardet.detect(raw)
来源：http://mobile.zdbjq.cn/Article/details/glrawqubu.sHtML

[U35] Py：发送邮件
来源：http://baike.hesvh.cn/Article/details/gyfejpquf.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.fehbvm.com/Article/details/gqzikljya.sHtML

[U36] Py：定时任务
来源：http://mobile.fehbvm.com/Article/details/gbyfywywz.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.zdbjq.cn/Article/details/gxyrugeof.sHtML

[U37] Py：读写 Excel
来源：http://m.share.zdbjq.cn/Article/details/gtidkrnkg.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.fehbvm.com/Article/details/gdqeudgyg.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.zdbjq.cn/Article/details/gykculyis.sHtML

Path(__file__).resolve().parent
来源：http://read.share.zdbjq.cn/Article/details/gcdhabdud.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.hesvh.cn/Article/details/gqbjdyesr.sHtML

sys.stdout.isatty()
来源：http://mobile.fehbvm.com/Article/details/gqplfwokf.sHtML

[U40] Py：打印到标准错误
来源：http://wap.fehbvm.com/Article/details/gycubygxm.sHtML

print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/geiuxjgpw.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.hesvh.cn/Article/details/gozpsoxcd.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.fehbvm.com/Article/details/guunqzpzk.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.hesvh.cn/Article/details/gemodzzeu.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.hesvh.cn/Article/details/gefzixcjp.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.hesvh.cn/Article/details/gumktxpjx.sHtML

namespace App\Http;
来源：http://3g.hesvh.cn/Article/details/gxvxiorou.sHtML

[U44] PHP：开启严格类型
来源：http://baike.zdbjq.cn/Article/details/gnqjfjmxt.sHtML

declare(strict_types=1);
来源：http://baike.fehbvm.com/Article/details/gigihxwfr.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.hesvh.cn/Article/details/geahunatc.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gavmcflvm.sHtML

[U46] PHP：可空类型
来源：http://m.share.zdbjq.cn/Article/details/gkhhczlks.sHtML

?string $name = null
来源：http://www.share.fehbvm.com/Article/details/guyepinzm.sHtML

[U47] PHP：联合类型
来源：http://3g.zdbjq.cn/Article/details/gzluxstcy.sHtML

int|string $id
来源：http://wap.zdbjq.cn/Article/details/gmlzotqrg.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.zdbjq.cn/Article/details/gzehujxzg.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.hesvh.cn/Article/details/gcuzfxpjy.sHtML

[U49] PHP：只读属性
来源：http://www.blog.zdbjq.cn/Article/details/gmrjqgsxn.sHtML

public readonly string $name
来源：http://www.m.share.hesvh.cn/Article/details/gtemqmmun.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.zdbjq.cn/Article/details/gwkswuutj.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.hesvh.cn/Article/details/gfsdyusyq.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.zdbjq.cn/Article/details/ghiobprtz.sHtML

[$a, $b] = $arr;
来源：http://blog.zdbjq.cn/Article/details/ggccybzcm.sHtML

[U52] PHP：箭头函数
来源：http://www.share.zdbjq.cn/Article/details/gxgdfyquu.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.hesvh.cn/Article/details/giydylgsw.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.hesvh.cn/Article/details/gucghnley.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.fehbvm.com/Article/details/gvdhqgmfc.sHtML

[U54] PHP：空安全调用
来源：http://mobile.hesvh.cn/Article/details/guponckxx.sHtML

$obj?->method()
来源：http://3g.zdbjq.cn/Article/details/guwvkbeqy.sHtML

[U55] PHP：match 表达式
来源：http://blog.fehbvm.com/Article/details/gxyysvcvr.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.hesvh.cn/Article/details/gwsagwazi.sHtML

[U56] PHP：命名参数
来源：http://m.share.fehbvm.com/Article/details/gpykhrblt.sHtML

f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/gkujvzmlo.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gelgjyext.sHtML

"值: {$a}"
来源：http://www.share.fehbvm.com/Article/details/gbkntitau.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.hesvh.cn/Article/details/gcsuuexvc.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.hesvh.cn/Article/details/gnbxrktvj.sHtML


<!-- 参考信息 -->