代发 wailian999

[S35] C++：map
来源：http://read.share.fehbvm.com/Article/details/giyathdcn.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/gjtabdrre.sHtML

[S36] C++：unordered_map
来源：http://mobile.hesvh.cn/Article/details/gevudjcff.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/ghiiareee.sHtML

[S37] C++：set
来源：http://mobile.fehbvm.com/Article/details/gqufhxhvw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fehbvm.com/Article/details/goiuasraw.sHtML

[S38] C++：排序
来源：http://wap.fehbvm.com/Article/details/gipdfnfku.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.hesvh.cn/Article/details/gqdmmebjd.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.hesvh.cn/Article/details/gevvwhhid.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.hesvh.cn/Article/details/gsvqinned.sHtML

[S40] C++：查找元素
来源：http://www.share.fehbvm.com/Article/details/gneneylqi.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.hesvh.cn/Article/details/gslndjvzr.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fehbvm.com/Article/details/gpiyncyuk.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.hesvh.cn/Article/details/gwfosxbgi.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fehbvm.com/Article/details/gecimzxzw.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.zdbjq.cn/Article/details/ggrnvnuqa.sHtML

[S43] C++：智能指针
来源：http://www.m.share.zdbjq.cn/Article/details/gawjxkdpo.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fehbvm.com/Article/details/gdrrfbnrh.sHtML

[S44] C++：引用传参
来源：http://www.m.share.zdbjq.cn/Article/details/gjfqkaaod.sHtML

void inc(int &x) { ++x; }
来源：http://baike.zdbjq.cn/Article/details/gurpjmoji.sHtML

[S45] C++：lambda
来源：http://www.m.share.fehbvm.com/Article/details/gbuhgnisb.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.zdbjq.cn/Article/details/gnqivucgn.sHtML

[S46] C++：函数模板
来源：http://www.blog.hesvh.cn/Article/details/gbzrhrpuj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.hesvh.cn/Article/details/ghmpnfkad.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.zdbjq.cn/Article/details/ggegkapqa.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fehbvm.com/Article/details/gqbyjmobw.sHtML

[S48] C++：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/ghwuiutkp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fehbvm.com/Article/details/gkliddmix.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.zdbjq.cn/Article/details/gbpeglpud.sHtML

[S49] C++：写文件
来源：http://www.m.share.zdbjq.cn/Article/details/gitmqwttx.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.zdbjq.cn/Article/details/gbufaanxv.sHtML

[S50] C++：格式化数字
来源：http://m.share.hesvh.cn/Article/details/gjbcevjfg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gttxioobj.sHtML

[S51] C++：显式类型转换
来源：http://read.share.zdbjq.cn/Article/details/gyduzcbhb.sHtML

static_cast<double>(a) / b
来源：http://wap.zdbjq.cn/Article/details/gnefvacwe.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.zdbjq.cn/Article/details/ghxxhznku.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.zdbjq.cn/Article/details/gqszijlnv.sHtML

[S53] C++：移动语义
来源：http://blog.zdbjq.cn/Article/details/gjkbviyeh.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.hesvh.cn/Article/details/gonqcjdvf.sHtML

[S54] C++：异常处理
来源：http://read.share.zdbjq.cn/Article/details/grnwepcny.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fehbvm.com/Article/details/gkbgisvxr.sHtML

[S55] C++：结构化绑定
来源：http://blog.zdbjq.cn/Article/details/gxrqyjncj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fehbvm.com/Article/details/gkyemjpnm.sHtML

[S56] C++：optional
来源：http://www.share.zdbjq.cn/Article/details/gpbeiwmrg.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.zdbjq.cn/Article/details/grrmrjugu.sHtML

[S57] C++：编译期常量
来源：http://m.share.fehbvm.com/Article/details/gnnwaihlx.sHtML

constexpr int N = 10;
来源：http://www.m.share.hesvh.cn/Article/details/guruwetiu.sHtML

[S58] C++：命名空间
来源：http://blog.zdbjq.cn/Article/details/gegbjmlzp.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.hesvh.cn/Article/details/gfilxhjjf.sHtML

[S59] C++：静态断言
来源：http://read.share.hesvh.cn/Article/details/ggblalffm.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.zdbjq.cn/Article/details/gvjtfayxu.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.hesvh.cn/Article/details/glbxkhlpw.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fehbvm.com/Article/details/gdjfuhgjq.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gsbwnlsie.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.hesvh.cn/Article/details/gvkweofok.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gxowjvuek.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fehbvm.com/Article/details/gntxjshdw.sHtML

println("Hello")
来源：http://wap.hesvh.cn/Article/details/gtvhyetxv.sHtML

[T02] Kotlin：变量
来源：http://read.share.zdbjq.cn/Article/details/guwnsizpe.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.hesvh.cn/Article/details/glyuvkgjq.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.hesvh.cn/Article/details/gywlxesvs.sHtML

"值: $b"
来源：http://wap.hesvh.cn/Article/details/gejmaftrj.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.hesvh.cn/Article/details/gtgwkplbq.sHtML

val n: String? = null;  n?.length
来源：http://blog.fehbvm.com/Article/details/gnggdshqv.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fehbvm.com/Article/details/gfknmkyxc.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.hesvh.cn/Article/details/gntzmylob.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.zdbjq.cn/Article/details/gonuzlyzf.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gajifhstp.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.hesvh.cn/Article/details/gwlmmrcxi.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.zdbjq.cn/Article/details/gekmqjvxz.sHtML

[T08] Kotlin：数据类
来源：http://www.share.zdbjq.cn/Article/details/gshkhjucm.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fehbvm.com/Article/details/gvhldtocy.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fehbvm.com/Article/details/gxxdgxugv.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fehbvm.com/Article/details/gbrincaar.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fehbvm.com/Article/details/gxcbjhjvo.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.hesvh.cn/Article/details/glcpevbow.sHtML

[T11] Kotlin：协程
来源：http://baike.fehbvm.com/Article/details/gmptcgxzf.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fehbvm.com/Article/details/gkwlgyinc.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fehbvm.com/Article/details/gpescpmvw.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.zdbjq.cn/Article/details/ghvozxszv.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.fehbvm.com/Article/details/gvhbeeiml.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.zdbjq.cn/Article/details/gsmzzksqd.sHtML

[T14] Kotlin：循环
来源：http://3g.fehbvm.com/Article/details/gsihrhhuz.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/gpajwhhqy.sHtML

[T15] Kotlin：接口
来源：http://read.share.hesvh.cn/Article/details/gpoqmvokf.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fehbvm.com/Article/details/gpzlfjhxf.sHtML

[T16] Swift：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gphmejyhb.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/gcdcxduco.sHtML

[T17] Swift：变量与常量
来源：http://wap.fehbvm.com/Article/details/gigdfaqae.sHtML

var a = 1;  let b = 2
来源：http://read.share.fehbvm.com/Article/details/gespshnqn.sHtML

[T18] Swift：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gnflaavxo.sHtML

"值: \(b)"
来源：http://3g.hesvh.cn/Article/details/gzibyztdn.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fehbvm.com/Article/details/gtsuvjouz.sHtML

if let n = opt { print(n) }
来源：http://m.share.zdbjq.cn/Article/details/gtgjkgyez.sHtML

[T20] Swift：数组操作
来源：http://m.share.hesvh.cn/Article/details/gdodxwaxb.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fehbvm.com/Article/details/gexukfnmk.sHtML

[T21] Swift：遍历
来源：http://read.share.hesvh.cn/Article/details/gzhlvftdf.sHtML

for x in a { print(x) }
来源：http://www.blog.hesvh.cn/Article/details/glqpaeyzi.sHtML

[T22] Swift：字典
来源：http://www.blog.hesvh.cn/Article/details/gkrloicvh.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.fehbvm.com/Article/details/gvyaizfvw.sHtML

[T23] Swift：函数
来源：http://wap.fehbvm.com/Article/details/gtsowjpoa.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.hesvh.cn/Article/details/gybwdagub.sHtML

[T24] Swift：闭包
来源：http://baike.zdbjq.cn/Article/details/gxmvftyqc.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.zdbjq.cn/Article/details/gkfjkrsam.sHtML

[T25] Swift：结构体
来源：http://www.blog.hesvh.cn/Article/details/graoqcppj.sHtML

struct P { var x: Int }
来源：http://3g.fehbvm.com/Article/details/gmimqvxpp.sHtML

[T26] Swift：类与重写
来源：http://www.blog.zdbjq.cn/Article/details/glyjysizy.sHtML

class A: Base { override func f() {} }
来源：http://3g.hesvh.cn/Article/details/givalatvm.sHtML

[T27] Swift：错误处理
来源：http://mobile.zdbjq.cn/Article/details/gbmgbqsjc.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.hesvh.cn/Article/details/gcscpioww.sHtML

[T28] Swift：枚举
来源：http://baike.zdbjq.cn/Article/details/gnobgxifk.sHtML

enum Color { case red, green }
来源：http://www.share.zdbjq.cn/Article/details/gxmwmhzlp.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.zdbjq.cn/Article/details/gxjtogicv.sHtML

guard let x = opt else { return }
来源：http://www.m.share.fehbvm.com/Article/details/gfdznbbgb.sHtML

[T30] Swift：协议
来源：http://www.m.share.hesvh.cn/Article/details/gihzrumom.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fehbvm.com/Article/details/gopxcrchq.sHtML

[T31] Lua：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gjracimuw.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gcutynvjf.sHtML

[T32] Lua：局部变量
来源：http://www.blog.zdbjq.cn/Article/details/gvhkpcckx.sHtML

local a = 1
来源：http://m.share.fehbvm.com/Article/details/gktdfmvuf.sHtML

[T33] Lua：表（数组）
来源：http://blog.zdbjq.cn/Article/details/gbtjssxwm.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.zdbjq.cn/Article/details/gyavnjlqi.sHtML

[T34] Lua：遍历表
来源：http://read.share.fehbvm.com/Article/details/gfkhdxbge.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.zdbjq.cn/Article/details/gguseiaco.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fehbvm.com/Article/details/ghjgsgfcj.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.fehbvm.com/Article/details/gffqdugdk.sHtML

[T36] Lua：函数
来源：http://3g.hesvh.cn/Article/details/ghahubgvs.sHtML

function add(a, b) return a + b end
来源：http://read.share.hesvh.cn/Article/details/gkfbxngdd.sHtML

[T37] Lua：字符串拼接
来源：http://baike.hesvh.cn/Article/details/gvdkjxxui.sHtML

"a" .. "b"
来源：http://mobile.zdbjq.cn/Article/details/glhfvswse.sHtML

[T38] Lua：条件
来源：http://read.share.hesvh.cn/Article/details/gtscquerr.sHtML

if x > 0 then print("正") end
来源：http://3g.hesvh.cn/Article/details/gkogmxphl.sHtML

[T39] Lua：模式匹配
来源：http://wap.hesvh.cn/Article/details/gduwpmdyo.sHtML

string.find(s, "%d+")
来源：http://www.blog.zdbjq.cn/Article/details/gwxiiyhfc.sHtML

[T40] Lua：元表
来源：http://www.m.share.zdbjq.cn/Article/details/gwcljpmjb.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.zdbjq.cn/Article/details/gietoervc.sHtML

[T41] Perl：Hello World
来源：http://www.share.hesvh.cn/Article/details/gpaycyplm.sHtML

print "Hello\n";
来源：http://read.share.zdbjq.cn/Article/details/gzmnlxkgf.sHtML

[T42] Perl：变量类型
来源：http://wap.hesvh.cn/Article/details/gqjeudxje.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.zdbjq.cn/Article/details/gzdyycmhk.sHtML

[T43] Perl：字符串插值
来源：http://blog.hesvh.cn/Article/details/gvgqvcdtk.sHtML

"值: $a"
来源：http://www.share.fehbvm.com/Article/details/gtxrmupxo.sHtML

[T44] Perl：条件
来源：http://m.share.hesvh.cn/Article/details/gyiiemyti.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.hesvh.cn/Article/details/gznnvwtju.sHtML

[T45] Perl：数组遍历
来源：http://read.share.zdbjq.cn/Article/details/gwmrffumr.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.fehbvm.com/Article/details/gidlbnpzh.sHtML

[T46] Perl：哈希操作
来源：http://3g.hesvh.cn/Article/details/gqhvtvixa.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.fehbvm.com/Article/details/gfqjdijxa.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fehbvm.com/Article/details/gqetxvwey.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.zdbjq.cn/Article/details/gsrzykjsw.sHtML

[T48] Perl：正则替换
来源：http://wap.zdbjq.cn/Article/details/gfhprwcgk.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.hesvh.cn/Article/details/gqjdkoxmm.sHtML

[T49] Perl：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gjgrrfvnt.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gpqyjmvsn.sHtML

[T50] Perl：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gzbdeqhui.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.zdbjq.cn/Article/details/gzbrowuin.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.fehbvm.com/Article/details/gxxexvtrw.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gqrlxwspx.sHtML

println("Hello")
来源：http://baike.fehbvm.com/Article/details/gckgraxmh.sHtML

[T52] Scala：变量
来源：http://www.blog.zdbjq.cn/Article/details/gsswdcjnk.sHtML

val a = 1;  var b = 2
来源：http://3g.fehbvm.com/Article/details/gwgheuqns.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gzziurokw.sHtML

s"值: $b"
来源：http://wap.zdbjq.cn/Article/details/gmwpljuzj.sHtML

[T54] Scala：集合映射
来源：http://3g.hesvh.cn/Article/details/gnfuxdval.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.zdbjq.cn/Article/details/getybapic.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/gvhasymfs.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.fehbvm.com/Article/details/gyyiabjvj.sHtML

[T56] Scala：样例类
来源：http://www.blog.hesvh.cn/Article/details/gwhjgwqqi.sHtML

case class User(name: String, age: Int)
来源：http://read.share.fehbvm.com/Article/details/gubgwvfvh.sHtML

[T57] Scala：模式匹配
来源：http://wap.zdbjq.cn/Article/details/gjjnsutse.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.zdbjq.cn/Article/details/gfxtttaot.sHtML

[T58] Scala：函数定义
来源：http://www.blog.zdbjq.cn/Article/details/gfgtquebs.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.zdbjq.cn/Article/details/gkjvejjzb.sHtML

[T59] Scala：循环
来源：http://www.share.zdbjq.cn/Article/details/ggjhrlmea.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.zdbjq.cn/Article/details/ghncguppk.sHtML

[T60] Scala：折叠
来源：http://3g.fehbvm.com/Article/details/gaxufliam.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.hesvh.cn/Article/details/gxslqrwzs.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gpxtmphac.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.hesvh.cn/Article/details/gdjuqbeby.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gjnafcvux.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.fehbvm.com/Article/details/gmmnhglwu.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.hesvh.cn/Article/details/ghgmubonb.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.zdbjq.cn/Article/details/gsqkjkugq.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.zdbjq.cn/Article/details/goedmamvr.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.hesvh.cn/Article/details/gqepqrjsb.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.zdbjq.cn/Article/details/gmsgmjgty.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.fehbvm.com/Article/details/gfjylsjej.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.hesvh.cn/Article/details/gsksfjlxy.sHtML

[U05] Py：列表去重且保序
来源：http://3g.zdbjq.cn/Article/details/gmsfgznwp.sHtML

list(dict.fromkeys(arr))
来源：http://blog.hesvh.cn/Article/details/gmyztkfdf.sHtML

[U06] Py：合并两个字典
来源：http://m.share.fehbvm.com/Article/details/gqwkholsf.sHtML

{**a, **b}
来源：http://www.share.zdbjq.cn/Article/details/galhmflea.sHtML

[U07] Py：反转字典键值
来源：http://blog.hesvh.cn/Article/details/gpuuafhvg.sHtML

{v: k for k, v in d.items()}
来源：http://wap.fehbvm.com/Article/details/gkoeblfqw.sHtML

[U08] Py：展平二维列表
来源：http://3g.hesvh.cn/Article/details/gmengezei.sHtML

[y for x in nested for y in x]
来源：http://www.blog.fehbvm.com/Article/details/gfvbmrsbk.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.fehbvm.com/Article/details/gzqcphnly.sHtML

max(d, key=d.get)
来源：http://www.share.hesvh.cn/Article/details/gzyosgpww.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.hesvh.cn/Article/details/govusptlg.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.zdbjq.cn/Article/details/gscomvniz.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.hesvh.cn/Article/details/gifsonhpa.sHtML

(x * 2 for x in arr)
来源：http://mobile.zdbjq.cn/Article/details/gvtcwjsoq.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.fehbvm.com/Article/details/gxqtcziil.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.hesvh.cn/Article/details/gaocpcgpy.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.zdbjq.cn/Article/details/gmvnzxjkt.sHtML

deque(maxlen=10)
来源：http://3g.zdbjq.cn/Article/details/gqjkzqjse.sHtML

[U14] Py：分组收集到列表
来源：http://3g.hesvh.cn/Article/details/gglprovyo.sHtML

defaultdict(list)
来源：http://baike.fehbvm.com/Article/details/gpmcykhkt.sHtML

[U15] Py：高精度计时
来源：http://3g.fehbvm.com/Article/details/gslrtadwa.sHtML

t = time.perf_counter()
来源：http://3g.fehbvm.com/Article/details/gjfthqisg.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.zdbjq.cn/Article/details/gvpzyflhr.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.hesvh.cn/Article/details/gxogdugrk.sHtML

[U17] Py：初始化日志
来源：http://3g.hesvh.cn/Article/details/gxbascirg.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.fehbvm.com/Article/details/gdgpvwuwp.sHtML

[U18] Py：预编译正则
来源：http://wap.zdbjq.cn/Article/details/gpqmcdyrb.sHtML

pat = re.compile(r"\d+")
来源：http://3g.zdbjq.cn/Article/details/gjsnkyaxw.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.hesvh.cn/Article/details/gnhemtqtd.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.hesvh.cn/Article/details/gkzzzaxdb.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.zdbjq.cn/Article/details/gggsfiamg.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.zdbjq.cn/Article/details/gyygsbyib.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.zdbjq.cn/Article/details/ggjopntov.sHtML

@contextlib.contextmanager
来源：http://3g.hesvh.cn/Article/details/gklmhjaem.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.hesvh.cn/Article/details/ggouevmbz.sHtML

list(zip(*m))
来源：http://mobile.fehbvm.com/Article/details/gygmlxwwo.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.zdbjq.cn/Article/details/gdwfigowx.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.hesvh.cn/Article/details/gdmmqifvy.sHtML

[U24] Py：路径操作
来源：http://mobile.fehbvm.com/Article/details/gzhpveciu.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.zdbjq.cn/Article/details/gxmdmdcay.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.hesvh.cn/Article/details/gdaneolqm.sHtML

csv.DictReader(f)
来源：http://wap.zdbjq.cn/Article/details/gtwlmhcnh.sHtML

[U26] Py：并发下载
来源：http://www.m.share.fehbvm.com/Article/details/gzwyylkif.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.zdbjq.cn/Article/details/glkqisyrm.sHtML

[U27] Py：异步 HTTP
来源：http://3g.zdbjq.cn/Article/details/gzsysfwzx.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.hesvh.cn/Article/details/glhrqjflc.sHtML

[U28] Py：类型别名
来源：http://blog.zdbjq.cn/Article/details/gchpcrzku.sHtML

UserId = int
来源：http://www.share.fehbvm.com/Article/details/gshpatxxx.sHtML

[U29] Py：属性校验
来源：http://mobile.fehbvm.com/Article/details/gsrcqflii.sHtML

@property 与 @x.setter 配合
来源：http://blog.zdbjq.cn/Article/details/gqghfclrz.sHtML

[U30] Py：数据类
来源：http://www.m.share.fehbvm.com/Article/details/ghantrucq.sHtML

@dataclass(slots=True)
来源：http://mobile.fehbvm.com/Article/details/gfuasqcbz.sHtML

[U31] Py：单测
来源：http://www.share.hesvh.cn/Article/details/gibbqrnrb.sHtML

python -m pytest -q
来源：http://m.share.fehbvm.com/Article/details/ggvpyorbo.sHtML

[U32] Py：代码格式化
来源：http://www.blog.fehbvm.com/Article/details/gehjgqogj.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.hesvh.cn/Article/details/gvnobgwfq.sHtML

[U33] Py：打包发布
来源：http://wap.fehbvm.com/Article/details/gounjnxlk.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.zdbjq.cn/Article/details/gfvdtpeaq.sHtML

[U34] Py：判断编码
来源：http://mobile.zdbjq.cn/Article/details/gjsrvtpgk.sHtML

chardet.detect(raw)
来源：http://mobile.hesvh.cn/Article/details/glvamhpav.sHtML

[U35] Py：发送邮件
来源：http://m.share.fehbvm.com/Article/details/gjmtylpvt.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.zdbjq.cn/Article/details/gymugpsfg.sHtML

[U36] Py：定时任务
来源：http://www.m.share.hesvh.cn/Article/details/gglmsicpx.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.zdbjq.cn/Article/details/gpicsrmrv.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.hesvh.cn/Article/details/gtoqgbwwd.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.zdbjq.cn/Article/details/geihuzqgf.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.fehbvm.com/Article/details/giipsysmr.sHtML

Path(__file__).resolve().parent
来源：http://read.share.fehbvm.com/Article/details/gfexnbqjn.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.zdbjq.cn/Article/details/gxuyznlzs.sHtML

sys.stdout.isatty()
来源：http://3g.zdbjq.cn/Article/details/grtxdnemf.sHtML

[U40] Py：打印到标准错误
来源：http://baike.fehbvm.com/Article/details/gsewtpziv.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.zdbjq.cn/Article/details/gqezposgu.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.zdbjq.cn/Article/details/gqxjsosgm.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.zdbjq.cn/Article/details/gjljrsjxb.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.fehbvm.com/Article/details/gndlimjve.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.hesvh.cn/Article/details/gqjwflsss.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.hesvh.cn/Article/details/ghlxxrffp.sHtML

namespace App\Http;
来源：http://blog.zdbjq.cn/Article/details/gnuhvmatv.sHtML

[U44] PHP：开启严格类型
来源：http://baike.hesvh.cn/Article/details/grnbacqee.sHtML

declare(strict_types=1);
来源：http://wap.fehbvm.com/Article/details/gxqzkriqk.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.zdbjq.cn/Article/details/gkfvytput.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gtqgndexy.sHtML

[U46] PHP：可空类型
来源：http://wap.zdbjq.cn/Article/details/gpdqcjoda.sHtML

?string $name = null
来源：http://www.blog.zdbjq.cn/Article/details/gwokpmkay.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.zdbjq.cn/Article/details/gvdqspcoh.sHtML

int|string $id
来源：http://blog.fehbvm.com/Article/details/gxdiaygvd.sHtML

[U48] PHP：纯枚举
来源：http://blog.fehbvm.com/Article/details/guojuxxfu.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.zdbjq.cn/Article/details/gbqlkjbwh.sHtML

[U49] PHP：只读属性
来源：http://www.blog.hesvh.cn/Article/details/gebkitfcg.sHtML

public readonly string $name
来源：http://blog.zdbjq.cn/Article/details/gxdtdxlph.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.hesvh.cn/Article/details/gwpnemevo.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gsnrjdvpz.sHtML

[U51] PHP：数组解构
来源：http://read.share.fehbvm.com/Article/details/ggkstenit.sHtML

[$a, $b] = $arr;
来源：http://baike.hesvh.cn/Article/details/goenhrxzd.sHtML

[U52] PHP：箭头函数
来源：http://m.share.zdbjq.cn/Article/details/gkueixfnb.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.zdbjq.cn/Article/details/gkfmdrrpk.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.hesvh.cn/Article/details/gwvygwkhv.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.zdbjq.cn/Article/details/gttaeoueb.sHtML

[U54] PHP：空安全调用
来源：http://blog.hesvh.cn/Article/details/gtfuotncn.sHtML

$obj?->method()
来源：http://m.share.zdbjq.cn/Article/details/gzycsywir.sHtML

[U55] PHP：match 表达式
来源：http://www.share.hesvh.cn/Article/details/gmcnauvrf.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.hesvh.cn/Article/details/gacflcbjj.sHtML

[U56] PHP：命名参数
来源：http://mobile.zdbjq.cn/Article/details/gvgdovvze.sHtML

f(a: 1, b: 2)
来源：http://blog.zdbjq.cn/Article/details/gcznmhqwg.sHtML

[U57] PHP：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gtasobxab.sHtML

"值: {$a}"
来源：http://baike.fehbvm.com/Article/details/grgxzfgoh.sHtML

[U58] PHP：数组三件套
来源：http://wap.hesvh.cn/Article/details/guqkjupap.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.hesvh.cn/Article/details/gokaqqssm.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.fehbvm.com/Article/details/glyzxtann.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.zdbjq.cn/Article/details/gylkampjh.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.fehbvm.com/Article/details/gapvhpetr.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.fehbvm.com/Article/details/gwofctqhy.sHtML


<!-- 参考信息 -->