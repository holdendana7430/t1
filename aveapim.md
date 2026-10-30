代发 wailian999

[S35] C++：map
来源：http://www.blog.fehbvm.com/Article/details/gwxrfwdzz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fehbvm.com/Article/details/geepvtzxn.sHtML

[S36] C++：unordered_map
来源：http://www.share.zdbjq.cn/Article/details/gxfmmlvca.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gvqfdsssd.sHtML

[S37] C++：set
来源：http://wap.fehbvm.com/Article/details/gemehgkxd.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.zdbjq.cn/Article/details/gklodvcho.sHtML

[S38] C++：排序
来源：http://www.blog.zdbjq.cn/Article/details/gqgnosavw.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.zdbjq.cn/Article/details/gzauwitmu.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.hesvh.cn/Article/details/gcdabgdpf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fehbvm.com/Article/details/gmsbbpyui.sHtML

[S40] C++：查找元素
来源：http://blog.zdbjq.cn/Article/details/gavwvaecg.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.hesvh.cn/Article/details/ghxianpwi.sHtML

[S41] C++：类与构造函数
来源：http://m.share.hesvh.cn/Article/details/gxdmstznn.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fehbvm.com/Article/details/gkpcjtasy.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fehbvm.com/Article/details/goszkwycx.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.zdbjq.cn/Article/details/ghjgyawvm.sHtML

[S43] C++：智能指针
来源：http://3g.fehbvm.com/Article/details/gkunszfff.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fehbvm.com/Article/details/gqictxihl.sHtML

[S44] C++：引用传参
来源：http://www.share.zdbjq.cn/Article/details/gimyounfi.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fehbvm.com/Article/details/gcualmooi.sHtML

[S45] C++：lambda
来源：http://www.share.fehbvm.com/Article/details/gcccauvop.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.zdbjq.cn/Article/details/gcoxtwajw.sHtML

[S46] C++：函数模板
来源：http://www.blog.fehbvm.com/Article/details/gtsuirjdp.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.hesvh.cn/Article/details/gydsorarw.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.zdbjq.cn/Article/details/gytmolxcg.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fehbvm.com/Article/details/gsgqjvzlv.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gawgfahml.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.zdbjq.cn/Article/details/gvjwzolgv.sHtML

while (std::getline(in, line)) { }
来源：http://wap.hesvh.cn/Article/details/gbauzlstd.sHtML

[S49] C++：写文件
来源：http://mobile.hesvh.cn/Article/details/gqqtszkvo.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fehbvm.com/Article/details/gtwtuetnl.sHtML

[S50] C++：格式化数字
来源：http://mobile.hesvh.cn/Article/details/grmimmtis.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fehbvm.com/Article/details/glwfkwnvo.sHtML

[S51] C++：显式类型转换
来源：http://mobile.zdbjq.cn/Article/details/grpxagujq.sHtML

static_cast<double>(a) / b
来源：http://3g.fehbvm.com/Article/details/gatsulpha.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fehbvm.com/Article/details/gabawdsct.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fehbvm.com/Article/details/gwryakhbx.sHtML

[S53] C++：移动语义
来源：http://blog.hesvh.cn/Article/details/gnvyvxhlc.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fehbvm.com/Article/details/gwrjgunxc.sHtML

[S54] C++：异常处理
来源：http://baike.hesvh.cn/Article/details/gspjhvqxi.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.zdbjq.cn/Article/details/gecpmjelb.sHtML

[S55] C++：结构化绑定
来源：http://3g.fehbvm.com/Article/details/gopjridtj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.zdbjq.cn/Article/details/godoimqrl.sHtML

[S56] C++：optional
来源：http://www.share.hesvh.cn/Article/details/ghvrgwzwk.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.hesvh.cn/Article/details/glhuqqsgi.sHtML

[S57] C++：编译期常量
来源：http://read.share.fehbvm.com/Article/details/ghkqziclo.sHtML

constexpr int N = 10;
来源：http://baike.fehbvm.com/Article/details/gjkltjwue.sHtML

[S58] C++：命名空间
来源：http://wap.hesvh.cn/Article/details/gmieugbgj.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.zdbjq.cn/Article/details/gtlbggnst.sHtML

[S59] C++：静态断言
来源：http://blog.hesvh.cn/Article/details/gpqvxmzce.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.hesvh.cn/Article/details/gmnwcdrgu.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fehbvm.com/Article/details/gqtumxrea.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fehbvm.com/Article/details/gwortjgmy.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ghjjfxpto.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fehbvm.com/Article/details/gurdxhuob.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ghwqthuqk.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fehbvm.com/Article/details/gizkzctzd.sHtML

println("Hello")
来源：http://mobile.hesvh.cn/Article/details/gvoxoetfo.sHtML

[T02] Kotlin：变量
来源：http://m.share.fehbvm.com/Article/details/ghpjeedpa.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.zdbjq.cn/Article/details/gzurqajtj.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.hesvh.cn/Article/details/gkmkelnru.sHtML

"值: $b"
来源：http://www.blog.hesvh.cn/Article/details/gvvcfypyb.sHtML

[T04] Kotlin：空安全
来源：http://mobile.hesvh.cn/Article/details/govbdkubg.sHtML

val n: String? = null;  n?.length
来源：http://wap.hesvh.cn/Article/details/gnigmooqd.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fehbvm.com/Article/details/gscdqiflv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.hesvh.cn/Article/details/gknwlxhnr.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.hesvh.cn/Article/details/ghdclzqez.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.hesvh.cn/Article/details/gftwobvlj.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/gjalbzdmj.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/gxcchkdlm.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fehbvm.com/Article/details/gfpxvwdcl.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fehbvm.com/Article/details/gouinvzjl.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.hesvh.cn/Article/details/gfdhrsqcp.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fehbvm.com/Article/details/gnjamrhnh.sHtML

[T10] Kotlin：默认参数
来源：http://blog.hesvh.cn/Article/details/gqqjphwpj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fehbvm.com/Article/details/gnerxnlnj.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fehbvm.com/Article/details/glrvofyxz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.zdbjq.cn/Article/details/gfvqadvds.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fehbvm.com/Article/details/grqllmlck.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.fehbvm.com/Article/details/gjditsxrx.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.zdbjq.cn/Article/details/gspwqpkmt.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.hesvh.cn/Article/details/giyobvfsh.sHtML

[T14] Kotlin：循环
来源：http://baike.hesvh.cn/Article/details/genukbngw.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fehbvm.com/Article/details/gpthxswvz.sHtML

[T15] Kotlin：接口
来源：http://wap.hesvh.cn/Article/details/gancbnygr.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.zdbjq.cn/Article/details/gbxqrmoof.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/guwommqgg.sHtML

print("Hello")
来源：http://www.share.hesvh.cn/Article/details/guczyiesh.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fehbvm.com/Article/details/gnvbwqjcy.sHtML

var a = 1;  let b = 2
来源：http://www.share.fehbvm.com/Article/details/gqfyrqaqw.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gckhppqnm.sHtML

"值: \(b)"
来源：http://www.m.share.hesvh.cn/Article/details/gdytzicbm.sHtML

[T19] Swift：可选绑定
来源：http://wap.hesvh.cn/Article/details/geqhvvdma.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.hesvh.cn/Article/details/gfbznnwud.sHtML

[T20] Swift：数组操作
来源：http://m.share.hesvh.cn/Article/details/godkuawbv.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.zdbjq.cn/Article/details/gorewbapi.sHtML

[T21] Swift：遍历
来源：http://m.share.hesvh.cn/Article/details/gclgpflbm.sHtML

for x in a { print(x) }
来源：http://read.share.hesvh.cn/Article/details/gnscygvkp.sHtML

[T22] Swift：字典
来源：http://www.m.share.zdbjq.cn/Article/details/ghnpbejkv.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.zdbjq.cn/Article/details/gnqbigqqo.sHtML

[T23] Swift：函数
来源：http://baike.hesvh.cn/Article/details/gmbceohkc.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fehbvm.com/Article/details/gilcvapdw.sHtML

[T24] Swift：闭包
来源：http://www.blog.fehbvm.com/Article/details/gpjmzqnxk.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fehbvm.com/Article/details/gpvapacwr.sHtML

[T25] Swift：结构体
来源：http://read.share.hesvh.cn/Article/details/gekalaqhb.sHtML

struct P { var x: Int }
来源：http://blog.zdbjq.cn/Article/details/gyafaoenj.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.fehbvm.com/Article/details/gqvyaippq.sHtML

class A: Base { override func f() {} }
来源：http://blog.zdbjq.cn/Article/details/gqwgovqbt.sHtML

[T27] Swift：错误处理
来源：http://3g.hesvh.cn/Article/details/gefpwylip.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.hesvh.cn/Article/details/gpeowoibd.sHtML

[T28] Swift：枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gsbgenzzy.sHtML

enum Color { case red, green }
来源：http://wap.zdbjq.cn/Article/details/ggcgeqmeh.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.hesvh.cn/Article/details/gxcocyzec.sHtML

guard let x = opt else { return }
来源：http://read.share.hesvh.cn/Article/details/gutqgnrno.sHtML

[T30] Swift：协议
来源：http://3g.zdbjq.cn/Article/details/gykblxudd.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.zdbjq.cn/Article/details/gvwfmuzug.sHtML

[T31] Lua：Hello World
来源：http://blog.hesvh.cn/Article/details/ggdryzaic.sHtML

print("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gjjxbnwde.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.zdbjq.cn/Article/details/glmhywlvg.sHtML

local a = 1
来源：http://mobile.zdbjq.cn/Article/details/gzwwuwqsc.sHtML

[T33] Lua：表（数组）
来源：http://blog.hesvh.cn/Article/details/goxwlflnp.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.hesvh.cn/Article/details/gjwoflpzx.sHtML

[T34] Lua：遍历表
来源：http://www.blog.hesvh.cn/Article/details/grmevkrqu.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.zdbjq.cn/Article/details/grvsqvlqg.sHtML

[T35] Lua：字典表
来源：http://baike.fehbvm.com/Article/details/gbwhilssz.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fehbvm.com/Article/details/guhnrpjxv.sHtML

[T36] Lua：函数
来源：http://m.share.hesvh.cn/Article/details/gauvaksjw.sHtML

function add(a, b) return a + b end
来源：http://read.share.zdbjq.cn/Article/details/gaynuyrcf.sHtML

[T37] Lua：字符串拼接
来源：http://3g.hesvh.cn/Article/details/gicartvwd.sHtML

"a" .. "b"
来源：http://www.share.fehbvm.com/Article/details/gwlpxorjq.sHtML

[T38] Lua：条件
来源：http://m.share.zdbjq.cn/Article/details/gzhzcxkbp.sHtML

if x > 0 then print("正") end
来源：http://baike.fehbvm.com/Article/details/guhuqfyjd.sHtML

[T39] Lua：模式匹配
来源：http://wap.fehbvm.com/Article/details/gzlxbxmke.sHtML

string.find(s, "%d+")
来源：http://read.share.zdbjq.cn/Article/details/gkucthune.sHtML

[T40] Lua：元表
来源：http://read.share.hesvh.cn/Article/details/gsmvtzels.sHtML

setmetatable({}, { __index = base })
来源：http://blog.zdbjq.cn/Article/details/gyzjinugw.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gcqwoofmt.sHtML

print "Hello\n";
来源：http://wap.hesvh.cn/Article/details/gscodojcs.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.hesvh.cn/Article/details/gukfgfhmy.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.zdbjq.cn/Article/details/giaariivy.sHtML

[T43] Perl：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gjgelltbp.sHtML

"值: $a"
来源：http://read.share.zdbjq.cn/Article/details/gfzeqzlxj.sHtML

[T44] Perl：条件
来源：http://www.share.fehbvm.com/Article/details/gmwzfzjyx.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.fehbvm.com/Article/details/gdfyerila.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.fehbvm.com/Article/details/guotofrff.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.fehbvm.com/Article/details/gvkwcbplr.sHtML

[T46] Perl：哈希操作
来源：http://wap.fehbvm.com/Article/details/gdsiygrvk.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.zdbjq.cn/Article/details/gakbkicag.sHtML

[T47] Perl：正则捕获
来源：http://www.share.fehbvm.com/Article/details/gmroyxbqf.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.fehbvm.com/Article/details/gaqxmdtim.sHtML

[T48] Perl：正则替换
来源：http://www.blog.zdbjq.cn/Article/details/gkdbrogee.sHtML

$s =~ s/old/new/g;
来源：http://read.share.hesvh.cn/Article/details/giiqcqdsq.sHtML

[T49] Perl：函数
来源：http://3g.zdbjq.cn/Article/details/grxvmhpnc.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gydhtfynd.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gzjjorxeh.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.fehbvm.com/Article/details/gflqysmrt.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.zdbjq.cn/Article/details/gazdarcwo.sHtML

[T51] Scala：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/ghcrfpyej.sHtML

println("Hello")
来源：http://3g.zdbjq.cn/Article/details/gzycixetw.sHtML

[T52] Scala：变量
来源：http://blog.fehbvm.com/Article/details/gyzlrtqqc.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.hesvh.cn/Article/details/guhhvotvn.sHtML

[T53] Scala：字符串插值
来源：http://wap.fehbvm.com/Article/details/gwxdcdkcy.sHtML

s"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/gcfzfguea.sHtML

[T54] Scala：集合映射
来源：http://m.share.zdbjq.cn/Article/details/gwnorvgrz.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.zdbjq.cn/Article/details/ghnvegyjk.sHtML

[T55] Scala：集合过滤
来源：http://m.share.zdbjq.cn/Article/details/guljawuym.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.zdbjq.cn/Article/details/gkcjvmbxv.sHtML

[T56] Scala：样例类
来源：http://www.blog.fehbvm.com/Article/details/gqrugqykh.sHtML

case class User(name: String, age: Int)
来源：http://www.share.zdbjq.cn/Article/details/gbkvobpew.sHtML

[T57] Scala：模式匹配
来源：http://www.share.hesvh.cn/Article/details/gqnicveii.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.hesvh.cn/Article/details/gfuduromy.sHtML

[T58] Scala：函数定义
来源：http://3g.zdbjq.cn/Article/details/gprjdngrm.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.fehbvm.com/Article/details/gpqijdvvn.sHtML

[T59] Scala：循环
来源：http://www.share.zdbjq.cn/Article/details/gaqmpejgr.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.fehbvm.com/Article/details/gibwzhndk.sHtML

[T60] Scala：折叠
来源：http://www.share.hesvh.cn/Article/details/gjklftcje.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.hesvh.cn/Article/details/gcrkpzuhh.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/geutrbzfr.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.zdbjq.cn/Article/details/gezsbekvy.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gefthzptl.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.fehbvm.com/Article/details/gbgcfiemu.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.hesvh.cn/Article/details/gjgsfxecn.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.zdbjq.cn/Article/details/gxrsovbbw.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.hesvh.cn/Article/details/gbvxjfmuz.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.fehbvm.com/Article/details/gnnnbtzei.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.hesvh.cn/Article/details/gxcnqysge.sHtML

[U04] Py：变量调试打印
来源：http://read.share.hesvh.cn/Article/details/gusguwezo.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.fehbvm.com/Article/details/gqkhzqkce.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.zdbjq.cn/Article/details/guzwnrewk.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.hesvh.cn/Article/details/gfehebeuz.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.zdbjq.cn/Article/details/gqoodfwxn.sHtML

{**a, **b}
来源：http://www.m.share.zdbjq.cn/Article/details/gqlkpqktg.sHtML

[U07] Py：反转字典键值
来源：http://blog.hesvh.cn/Article/details/ghxpyahms.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.hesvh.cn/Article/details/gnlumclve.sHtML

[U08] Py：展平二维列表
来源：http://read.share.fehbvm.com/Article/details/gcnlpsjcm.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.hesvh.cn/Article/details/gutrskipl.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.fehbvm.com/Article/details/gtdercibb.sHtML

max(d, key=d.get)
来源：http://baike.hesvh.cn/Article/details/gbspapugt.sHtML

[U10] Py：按值排序字典
来源：http://wap.zdbjq.cn/Article/details/gkxeuzwdu.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.zdbjq.cn/Article/details/gxqroivit.sHtML

[U11] Py：生成器表达式
来源：http://baike.fehbvm.com/Article/details/gxdvgkvwb.sHtML

(x * 2 for x in arr)
来源：http://wap.fehbvm.com/Article/details/ghcbrcqky.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.fehbvm.com/Article/details/gcxpytxbw.sHtML

Counter(arr).most_common(3)
来源：http://baike.fehbvm.com/Article/details/gcwuxwedx.sHtML

[U13] Py：固定长度队列
来源：http://m.share.zdbjq.cn/Article/details/gvxkmyzdk.sHtML

deque(maxlen=10)
来源：http://www.m.share.hesvh.cn/Article/details/glaobtcfj.sHtML

[U14] Py：分组收集到列表
来源：http://3g.fehbvm.com/Article/details/gnfujnrbe.sHtML

defaultdict(list)
来源：http://www.blog.fehbvm.com/Article/details/glmwazloo.sHtML

[U15] Py：高精度计时
来源：http://baike.fehbvm.com/Article/details/giamzgrib.sHtML

t = time.perf_counter()
来源：http://blog.fehbvm.com/Article/details/gokkasvtd.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.fehbvm.com/Article/details/gtvjonizs.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.hesvh.cn/Article/details/gyuowhzlr.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.hesvh.cn/Article/details/gtndgxvjb.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.zdbjq.cn/Article/details/glxcssjvf.sHtML

[U18] Py：预编译正则
来源：http://wap.fehbvm.com/Article/details/gyzrslieh.sHtML

pat = re.compile(r"\d+")
来源：http://blog.hesvh.cn/Article/details/gardciapr.sHtML

[U19] Py：正则替换带回调
来源：http://blog.hesvh.cn/Article/details/gcvobenha.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.zdbjq.cn/Article/details/gmdekzata.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.zdbjq.cn/Article/details/gxaldiqda.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.fehbvm.com/Article/details/guagdidwr.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.zdbjq.cn/Article/details/glwyrkoek.sHtML

@contextlib.contextmanager
来源：http://baike.fehbvm.com/Article/details/gzsxnpwil.sHtML

[U22] Py：矩阵转置
来源：http://mobile.hesvh.cn/Article/details/ggelfnkcx.sHtML

list(zip(*m))
来源：http://read.share.zdbjq.cn/Article/details/gdywhbctz.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.fehbvm.com/Article/details/givhgrdly.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.hesvh.cn/Article/details/gpiwwwuvc.sHtML

[U24] Py：路径操作
来源：http://www.m.share.zdbjq.cn/Article/details/gnupyzdop.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.fehbvm.com/Article/details/gkedjixit.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.hesvh.cn/Article/details/gqxmtfyxa.sHtML

csv.DictReader(f)
来源：http://mobile.hesvh.cn/Article/details/gtrxgtpdr.sHtML

[U26] Py：并发下载
来源：http://baike.fehbvm.com/Article/details/gynhaselh.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.fehbvm.com/Article/details/guupcjvtu.sHtML

[U27] Py：异步 HTTP
来源：http://blog.fehbvm.com/Article/details/gnrqzmhlt.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.fehbvm.com/Article/details/gxpryjcup.sHtML

[U28] Py：类型别名
来源：http://read.share.hesvh.cn/Article/details/gzxyhktjq.sHtML

UserId = int
来源：http://mobile.fehbvm.com/Article/details/goikbdwha.sHtML

[U29] Py：属性校验
来源：http://mobile.hesvh.cn/Article/details/gjmqruvvd.sHtML

@property 与 @x.setter 配合
来源：http://wap.hesvh.cn/Article/details/gudmhmlhx.sHtML

[U30] Py：数据类
来源：http://blog.zdbjq.cn/Article/details/glwdzmbxv.sHtML

@dataclass(slots=True)
来源：http://3g.fehbvm.com/Article/details/gzwfczwgg.sHtML

[U31] Py：单测
来源：http://wap.zdbjq.cn/Article/details/gkniiafed.sHtML

python -m pytest -q
来源：http://mobile.hesvh.cn/Article/details/goiqlqhge.sHtML

[U32] Py：代码格式化
来源：http://mobile.hesvh.cn/Article/details/gcdbrjxll.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.hesvh.cn/Article/details/gexprqiek.sHtML

[U33] Py：打包发布
来源：http://wap.hesvh.cn/Article/details/gmsazhosu.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.hesvh.cn/Article/details/gpqrycrgd.sHtML

[U34] Py：判断编码
来源：http://www.blog.fehbvm.com/Article/details/glwdrlzfm.sHtML

chardet.detect(raw)
来源：http://wap.fehbvm.com/Article/details/gdqdsrius.sHtML

[U35] Py：发送邮件
来源：http://blog.fehbvm.com/Article/details/guxqveoim.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.zdbjq.cn/Article/details/goueciukf.sHtML

[U36] Py：定时任务
来源：http://www.blog.fehbvm.com/Article/details/gihagxwpb.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.zdbjq.cn/Article/details/grwcanpyu.sHtML

[U37] Py：读写 Excel
来源：http://read.share.zdbjq.cn/Article/details/gulbrpuum.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.zdbjq.cn/Article/details/gcfwsmvva.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.zdbjq.cn/Article/details/gphqqlqqd.sHtML

Path(__file__).resolve().parent
来源：http://3g.zdbjq.cn/Article/details/gkqzhodoo.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.zdbjq.cn/Article/details/geccumvtu.sHtML

sys.stdout.isatty()
来源：http://baike.zdbjq.cn/Article/details/gcoeohhmu.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.fehbvm.com/Article/details/geeghtdqa.sHtML

print("err", file=sys.stderr)
来源：http://3g.fehbvm.com/Article/details/gqjusuygy.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.zdbjq.cn/Article/details/gcrbzsszt.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.hesvh.cn/Article/details/gkutglhck.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.zdbjq.cn/Article/details/guilfxpji.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.zdbjq.cn/Article/details/gjsmtyitc.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.zdbjq.cn/Article/details/gysevgoan.sHtML

namespace App\Http;
来源：http://wap.fehbvm.com/Article/details/gtqzmcljr.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.hesvh.cn/Article/details/gvazxyldj.sHtML

declare(strict_types=1);
来源：http://www.share.zdbjq.cn/Article/details/gwxqiyqqw.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.fehbvm.com/Article/details/gjgbcssmi.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gbhpjmciz.sHtML

[U46] PHP：可空类型
来源：http://blog.hesvh.cn/Article/details/grbjjqukt.sHtML

?string $name = null
来源：http://www.m.share.hesvh.cn/Article/details/gzilqgirx.sHtML

[U47] PHP：联合类型
来源：http://read.share.hesvh.cn/Article/details/gquifktfw.sHtML

int|string $id
来源：http://3g.fehbvm.com/Article/details/gakakbujb.sHtML

[U48] PHP：纯枚举
来源：http://baike.hesvh.cn/Article/details/ggmzyzhen.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.fehbvm.com/Article/details/grpsdjvld.sHtML

[U49] PHP：只读属性
来源：http://read.share.hesvh.cn/Article/details/gflokyhht.sHtML

public readonly string $name
来源：http://blog.zdbjq.cn/Article/details/gdhrxozuc.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.fehbvm.com/Article/details/gxgvnvsnv.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gfizihgnu.sHtML

[U51] PHP：数组解构
来源：http://read.share.fehbvm.com/Article/details/gzgrkdsut.sHtML

[$a, $b] = $arr;
来源：http://mobile.zdbjq.cn/Article/details/gzuxoeffp.sHtML

[U52] PHP：箭头函数
来源：http://blog.hesvh.cn/Article/details/gxuykyxrw.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.zdbjq.cn/Article/details/gligvadci.sHtML

[U53] PHP：空合并运算符
来源：http://3g.hesvh.cn/Article/details/gvxscbwgy.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.fehbvm.com/Article/details/gemzqcizo.sHtML

[U54] PHP：空安全调用
来源：http://m.share.zdbjq.cn/Article/details/gncxdqwod.sHtML

$obj?->method()
来源：http://read.share.hesvh.cn/Article/details/gcvqfrcfm.sHtML

[U55] PHP：match 表达式
来源：http://baike.hesvh.cn/Article/details/gmdueiiuz.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.fehbvm.com/Article/details/gosfmoimn.sHtML

[U56] PHP：命名参数
来源：http://3g.hesvh.cn/Article/details/gqyfaaeip.sHtML

f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/gcwfqvgpe.sHtML

[U57] PHP：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gchhdtgkv.sHtML

"值: {$a}"
来源：http://blog.hesvh.cn/Article/details/gurdiuxai.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.zdbjq.cn/Article/details/glqepxytr.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.hesvh.cn/Article/details/gugumvktt.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.fehbvm.com/Article/details/gpkaplwit.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.hesvh.cn/Article/details/gddpqtfht.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.fehbvm.com/Article/details/gqvajyedf.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.hesvh.cn/Article/details/ginhjvwsf.sHtML


<!-- 参考信息 -->