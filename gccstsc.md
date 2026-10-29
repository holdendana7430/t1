代发 wailian999

[S35] C++：map
来源：http://wap.zdbjq.cn/Article/details/gsciuvmiz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gtingyptl.sHtML

[S36] C++：unordered_map
来源：http://blog.fehbvm.com/Article/details/gkccfoaur.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/gvonmqfad.sHtML

[S37] C++：set
来源：http://read.share.zdbjq.cn/Article/details/gzpxaspko.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.hesvh.cn/Article/details/gnrjluuyn.sHtML

[S38] C++：排序
来源：http://m.share.zdbjq.cn/Article/details/gqvoxawff.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.hesvh.cn/Article/details/grysayapy.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.zdbjq.cn/Article/details/gcwuyvjtn.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.hesvh.cn/Article/details/gqcnbbfnf.sHtML

[S40] C++：查找元素
来源：http://www.blog.zdbjq.cn/Article/details/gedwvtklt.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.hesvh.cn/Article/details/guahhwnfu.sHtML

[S41] C++：类与构造函数
来源：http://baike.hesvh.cn/Article/details/gpcbqmcwi.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fehbvm.com/Article/details/gnlfbwqdu.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fehbvm.com/Article/details/ghmztdfaj.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fehbvm.com/Article/details/gdcffrpun.sHtML

[S43] C++：智能指针
来源：http://www.blog.hesvh.cn/Article/details/gguxepnyc.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.zdbjq.cn/Article/details/gqnhztsse.sHtML

[S44] C++：引用传参
来源：http://wap.fehbvm.com/Article/details/guwuzbofz.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.zdbjq.cn/Article/details/gxqnskmrk.sHtML

[S45] C++：lambda
来源：http://mobile.fehbvm.com/Article/details/gysavnvtt.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fehbvm.com/Article/details/gckzjnsdt.sHtML

[S46] C++：函数模板
来源：http://mobile.zdbjq.cn/Article/details/gaukzbxgq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.zdbjq.cn/Article/details/ghoalxvzp.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.hesvh.cn/Article/details/giojfgivf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.hesvh.cn/Article/details/gvqakeuej.sHtML

[S48] C++：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gokwrsxww.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.hesvh.cn/Article/details/gxrsxqeih.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.hesvh.cn/Article/details/gmuedbwls.sHtML

[S49] C++：写文件
来源：http://baike.fehbvm.com/Article/details/gxlmvnzyg.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.zdbjq.cn/Article/details/guomjthzs.sHtML

[S50] C++：格式化数字
来源：http://3g.zdbjq.cn/Article/details/gpkcezchy.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gswigiuvn.sHtML

[S51] C++：显式类型转换
来源：http://blog.zdbjq.cn/Article/details/gaxnjkoeo.sHtML

static_cast<double>(a) / b
来源：http://www.blog.zdbjq.cn/Article/details/gjctlboys.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.hesvh.cn/Article/details/gtwztfzkw.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.hesvh.cn/Article/details/gosovggtu.sHtML

[S53] C++：移动语义
来源：http://blog.hesvh.cn/Article/details/gypahngdj.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fehbvm.com/Article/details/gyheclsjz.sHtML

[S54] C++：异常处理
来源：http://mobile.zdbjq.cn/Article/details/gezovutif.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.hesvh.cn/Article/details/gsranwxyk.sHtML

[S55] C++：结构化绑定
来源：http://wap.hesvh.cn/Article/details/gohkmusaf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.hesvh.cn/Article/details/ghjjmsbdk.sHtML

[S56] C++：optional
来源：http://m.share.hesvh.cn/Article/details/gpndgnous.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.zdbjq.cn/Article/details/gamzedqzn.sHtML

[S57] C++：编译期常量
来源：http://3g.fehbvm.com/Article/details/gefcsnsbv.sHtML

constexpr int N = 10;
来源：http://blog.zdbjq.cn/Article/details/gnrjfhjhp.sHtML

[S58] C++：命名空间
来源：http://baike.zdbjq.cn/Article/details/gkbqqzame.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.hesvh.cn/Article/details/gqsmeuwtj.sHtML

[S59] C++：静态断言
来源：http://www.share.hesvh.cn/Article/details/grvjwujcb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fehbvm.com/Article/details/gsrjpoxho.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.hesvh.cn/Article/details/gpitavfhc.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.zdbjq.cn/Article/details/gductsqir.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gkwyxrgct.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.hesvh.cn/Article/details/gvjzrbhyh.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gocibqulh.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.hesvh.cn/Article/details/gxbqajuqh.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/gvwrnnxls.sHtML

[T02] Kotlin：变量
来源：http://baike.zdbjq.cn/Article/details/gyvhyorzi.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.hesvh.cn/Article/details/gvzaybwgt.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.zdbjq.cn/Article/details/gqkwglmwi.sHtML

"值: $b"
来源：http://m.share.zdbjq.cn/Article/details/gqymubiao.sHtML

[T04] Kotlin：空安全
来源：http://3g.fehbvm.com/Article/details/gtuhogkxo.sHtML

val n: String? = null;  n?.length
来源：http://mobile.hesvh.cn/Article/details/ggreuvpel.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.hesvh.cn/Article/details/grikfzvxv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fehbvm.com/Article/details/gsrptencr.sHtML

[T06] Kotlin：集合映射
来源：http://wap.zdbjq.cn/Article/details/gkgnyhooy.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.hesvh.cn/Article/details/gtofgqaqh.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fehbvm.com/Article/details/gfqsfqgcg.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fehbvm.com/Article/details/gigkulfyt.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fehbvm.com/Article/details/ggraklbri.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.hesvh.cn/Article/details/gznqoiijx.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.zdbjq.cn/Article/details/gvkaeywjn.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fehbvm.com/Article/details/gxeoqzmmq.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fehbvm.com/Article/details/gssfjtbbj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.hesvh.cn/Article/details/gxqdmnanp.sHtML

[T11] Kotlin：协程
来源：http://baike.fehbvm.com/Article/details/gfmwwvqsk.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.hesvh.cn/Article/details/gxgdsfdio.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fehbvm.com/Article/details/gdcgdrurn.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gxmnjnaro.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.hesvh.cn/Article/details/girdalutp.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fehbvm.com/Article/details/gohizapqf.sHtML

[T14] Kotlin：循环
来源：http://blog.fehbvm.com/Article/details/goqshksdj.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.zdbjq.cn/Article/details/geznrpout.sHtML

[T15] Kotlin：接口
来源：http://read.share.fehbvm.com/Article/details/gougngmxm.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fehbvm.com/Article/details/gufytdbei.sHtML

[T16] Swift：Hello World
来源：http://www.share.fehbvm.com/Article/details/gjhkubndg.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/gaubmjidh.sHtML

[T17] Swift：变量与常量
来源：http://wap.fehbvm.com/Article/details/giccvpcjq.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.hesvh.cn/Article/details/gpfzkfudc.sHtML

[T18] Swift：字符串插值
来源：http://blog.fehbvm.com/Article/details/gjmnfhhtb.sHtML

"值: \(b)"
来源：http://m.share.hesvh.cn/Article/details/goioxqjie.sHtML

[T19] Swift：可选绑定
来源：http://wap.zdbjq.cn/Article/details/gttqapizb.sHtML

if let n = opt { print(n) }
来源：http://mobile.hesvh.cn/Article/details/gydwwetnb.sHtML

[T20] Swift：数组操作
来源：http://blog.fehbvm.com/Article/details/gpnfebwej.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.zdbjq.cn/Article/details/girzpnogj.sHtML

[T21] Swift：遍历
来源：http://baike.zdbjq.cn/Article/details/gzgpiuamo.sHtML

for x in a { print(x) }
来源：http://blog.zdbjq.cn/Article/details/grhpevrbd.sHtML

[T22] Swift：字典
来源：http://www.blog.zdbjq.cn/Article/details/gcjrmlbkl.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.hesvh.cn/Article/details/goenhqnhw.sHtML

[T23] Swift：函数
来源：http://m.share.zdbjq.cn/Article/details/gdajslcur.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fehbvm.com/Article/details/gehstuuwo.sHtML

[T24] Swift：闭包
来源：http://www.m.share.fehbvm.com/Article/details/gfdmyxiby.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.fehbvm.com/Article/details/gfoxdyhyr.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fehbvm.com/Article/details/goagglgty.sHtML

struct P { var x: Int }
来源：http://read.share.fehbvm.com/Article/details/gmlpernrb.sHtML

[T26] Swift：类与重写
来源：http://read.share.fehbvm.com/Article/details/geaovnpla.sHtML

class A: Base { override func f() {} }
来源：http://blog.zdbjq.cn/Article/details/gfdapfodh.sHtML

[T27] Swift：错误处理
来源：http://wap.hesvh.cn/Article/details/gdvistdmp.sHtML

do { try f() } catch { print(error) }
来源：http://baike.fehbvm.com/Article/details/gtixtwzpz.sHtML

[T28] Swift：枚举
来源：http://baike.hesvh.cn/Article/details/gsddhddhu.sHtML

enum Color { case red, green }
来源：http://read.share.hesvh.cn/Article/details/gnyvidjcm.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.hesvh.cn/Article/details/gbdhukxkd.sHtML

guard let x = opt else { return }
来源：http://www.blog.hesvh.cn/Article/details/ggckwyief.sHtML

[T30] Swift：协议
来源：http://baike.hesvh.cn/Article/details/gswjyycgt.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.zdbjq.cn/Article/details/gpmoxeopm.sHtML

[T31] Lua：Hello World
来源：http://baike.hesvh.cn/Article/details/grvhnfhow.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/gdvtqezsn.sHtML

[T32] Lua：局部变量
来源：http://m.share.zdbjq.cn/Article/details/gwptmxnzd.sHtML

local a = 1
来源：http://m.share.fehbvm.com/Article/details/gchsszlwn.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.zdbjq.cn/Article/details/gzzgqejir.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fehbvm.com/Article/details/gbkvpeylp.sHtML

[T34] Lua：遍历表
来源：http://www.share.fehbvm.com/Article/details/gdvynljgk.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.fehbvm.com/Article/details/gigrxfrdo.sHtML

[T35] Lua：字典表
来源：http://www.share.hesvh.cn/Article/details/gsfjzrryl.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.zdbjq.cn/Article/details/gcbdzytpb.sHtML

[T36] Lua：函数
来源：http://wap.hesvh.cn/Article/details/gwglfkrvg.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.zdbjq.cn/Article/details/gptemlbev.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.zdbjq.cn/Article/details/gmeavdypj.sHtML

"a" .. "b"
来源：http://mobile.fehbvm.com/Article/details/gbsjdjzwq.sHtML

[T38] Lua：条件
来源：http://www.share.fehbvm.com/Article/details/gcvzlpcys.sHtML

if x > 0 then print("正") end
来源：http://www.share.fehbvm.com/Article/details/gaiqupkls.sHtML

[T39] Lua：模式匹配
来源：http://blog.fehbvm.com/Article/details/gpwrlkjwl.sHtML

string.find(s, "%d+")
来源：http://www.share.fehbvm.com/Article/details/gydhjmovi.sHtML

[T40] Lua：元表
来源：http://3g.zdbjq.cn/Article/details/gsnhnupau.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.fehbvm.com/Article/details/ghwurzpyi.sHtML

[T41] Perl：Hello World
来源：http://www.share.hesvh.cn/Article/details/gblxijvcy.sHtML

print "Hello\n";
来源：http://mobile.zdbjq.cn/Article/details/gxwudukms.sHtML

[T42] Perl：变量类型
来源：http://www.share.hesvh.cn/Article/details/gowtloqpt.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.zdbjq.cn/Article/details/ggxbopxxp.sHtML

[T43] Perl：字符串插值
来源：http://wap.hesvh.cn/Article/details/ggjomqvrj.sHtML

"值: $a"
来源：http://baike.hesvh.cn/Article/details/gcdruqpwb.sHtML

[T44] Perl：条件
来源：http://blog.zdbjq.cn/Article/details/gnfltbrgb.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.hesvh.cn/Article/details/gutlkvros.sHtML

[T45] Perl：数组遍历
来源：http://blog.fehbvm.com/Article/details/ghknbmyrw.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.hesvh.cn/Article/details/gjzsxdaxh.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.fehbvm.com/Article/details/glnphvzye.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.zdbjq.cn/Article/details/gepbhetlq.sHtML

[T47] Perl：正则捕获
来源：http://www.share.fehbvm.com/Article/details/gebjgroap.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.hesvh.cn/Article/details/gzlhxvbss.sHtML

[T48] Perl：正则替换
来源：http://read.share.zdbjq.cn/Article/details/guxgsqubj.sHtML

$s =~ s/old/new/g;
来源：http://www.share.hesvh.cn/Article/details/glhjqiexq.sHtML

[T49] Perl：函数
来源：http://www.m.share.hesvh.cn/Article/details/guiyttfow.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gfkonnjtn.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gitksyvlx.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.zdbjq.cn/Article/details/gwjzifuew.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.fehbvm.com/Article/details/gmcgnfeur.sHtML

[T51] Scala：Hello World
来源：http://3g.zdbjq.cn/Article/details/gaxjbmxok.sHtML

println("Hello")
来源：http://blog.fehbvm.com/Article/details/goqnfyiao.sHtML

[T52] Scala：变量
来源：http://blog.fehbvm.com/Article/details/gxwhgwufy.sHtML

val a = 1;  var b = 2
来源：http://3g.fehbvm.com/Article/details/glbonsfxj.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gbvuonzvk.sHtML

s"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/gtvwwwwrb.sHtML

[T54] Scala：集合映射
来源：http://blog.hesvh.cn/Article/details/gmcchvdjb.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.hesvh.cn/Article/details/gydwnleaw.sHtML

[T55] Scala：集合过滤
来源：http://3g.zdbjq.cn/Article/details/gmlgmmfck.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.fehbvm.com/Article/details/gaikhgifi.sHtML

[T56] Scala：样例类
来源：http://3g.fehbvm.com/Article/details/gpzkluuhy.sHtML

case class User(name: String, age: Int)
来源：http://www.share.hesvh.cn/Article/details/grhfkeykj.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.zdbjq.cn/Article/details/ghjtkqntk.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.hesvh.cn/Article/details/gvuxlfvma.sHtML

[T58] Scala：函数定义
来源：http://3g.hesvh.cn/Article/details/gasujyjwe.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.fehbvm.com/Article/details/gpctnuuyt.sHtML

[T59] Scala：循环
来源：http://3g.zdbjq.cn/Article/details/ghbfphuoo.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.fehbvm.com/Article/details/gkfvdpwsb.sHtML

[T60] Scala：折叠
来源：http://www.blog.hesvh.cn/Article/details/gicielpvs.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.zdbjq.cn/Article/details/gdqttbeow.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gcckdsayt.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.hesvh.cn/Article/details/gfzfymmmt.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gxgahgpld.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.hesvh.cn/Article/details/gdwamlwxd.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.fehbvm.com/Article/details/gtlcgtdpw.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.hesvh.cn/Article/details/gwesvrydh.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.fehbvm.com/Article/details/gqkbcecmz.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.fehbvm.com/Article/details/gkpuqsbcu.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.fehbvm.com/Article/details/gzqidjnul.sHtML

[U04] Py：变量调试打印
来源：http://blog.fehbvm.com/Article/details/gnuhqkpnr.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.zdbjq.cn/Article/details/gknwpkref.sHtML

[U05] Py：列表去重且保序
来源：http://baike.fehbvm.com/Article/details/gthfeyodb.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/gbeekomtk.sHtML

[U06] Py：合并两个字典
来源：http://m.share.hesvh.cn/Article/details/gswgvssoe.sHtML

{**a, **b}
来源：http://wap.hesvh.cn/Article/details/glarxdmyc.sHtML

[U07] Py：反转字典键值
来源：http://wap.fehbvm.com/Article/details/ghlbwsqyq.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.zdbjq.cn/Article/details/gawrvtbbk.sHtML

[U08] Py：展平二维列表
来源：http://3g.hesvh.cn/Article/details/gpyhosrrr.sHtML

[y for x in nested for y in x]
来源：http://wap.fehbvm.com/Article/details/gpxaaiegh.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.hesvh.cn/Article/details/gwhxsmsqu.sHtML

max(d, key=d.get)
来源：http://blog.fehbvm.com/Article/details/gqiypkjnp.sHtML

[U10] Py：按值排序字典
来源：http://baike.hesvh.cn/Article/details/gzgtkkdse.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.hesvh.cn/Article/details/gjtzgxtqc.sHtML

[U11] Py：生成器表达式
来源：http://read.share.fehbvm.com/Article/details/gngukrpff.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.fehbvm.com/Article/details/gglsxtbsg.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.hesvh.cn/Article/details/gxlghxljd.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gkstebpaa.sHtML

[U13] Py：固定长度队列
来源：http://mobile.hesvh.cn/Article/details/gpqzfkukm.sHtML

deque(maxlen=10)
来源：http://blog.fehbvm.com/Article/details/gsmgufige.sHtML

[U14] Py：分组收集到列表
来源：http://wap.fehbvm.com/Article/details/gtlxcsdyb.sHtML

defaultdict(list)
来源：http://read.share.fehbvm.com/Article/details/gugokysjd.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.hesvh.cn/Article/details/gzycxlkwi.sHtML

t = time.perf_counter()
来源：http://mobile.zdbjq.cn/Article/details/gdvbsjldh.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.hesvh.cn/Article/details/grymdufil.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.hesvh.cn/Article/details/gweezvejk.sHtML

[U17] Py：初始化日志
来源：http://baike.hesvh.cn/Article/details/ghcohswij.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.zdbjq.cn/Article/details/gtkdrvkbw.sHtML

[U18] Py：预编译正则
来源：http://blog.hesvh.cn/Article/details/gjoiqzvcy.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.hesvh.cn/Article/details/gwtrgsjkx.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.zdbjq.cn/Article/details/gcgysauan.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.hesvh.cn/Article/details/guqcykcfn.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.hesvh.cn/Article/details/gmvmtzugi.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.fehbvm.com/Article/details/gzfcshwmj.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.zdbjq.cn/Article/details/gkzamilwn.sHtML

@contextlib.contextmanager
来源：http://read.share.zdbjq.cn/Article/details/gsmuccvwt.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.fehbvm.com/Article/details/gdjybcpsi.sHtML

list(zip(*m))
来源：http://www.blog.hesvh.cn/Article/details/gknpvinka.sHtML

[U23] Py：分块读取大文件
来源：http://3g.zdbjq.cn/Article/details/gsuxgnhzv.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.hesvh.cn/Article/details/gxhpejqlj.sHtML

[U24] Py：路径操作
来源：http://read.share.fehbvm.com/Article/details/ghjncvxqy.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.fehbvm.com/Article/details/glmbqqtia.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.hesvh.cn/Article/details/gabquhoeg.sHtML

csv.DictReader(f)
来源：http://wap.fehbvm.com/Article/details/gdsvwkbdo.sHtML

[U26] Py：并发下载
来源：http://m.share.hesvh.cn/Article/details/gixjcgfao.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.hesvh.cn/Article/details/ggpnqhjik.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.hesvh.cn/Article/details/gtocfpqqs.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.zdbjq.cn/Article/details/giwfbpede.sHtML

[U28] Py：类型别名
来源：http://www.share.fehbvm.com/Article/details/giuwjchnr.sHtML

UserId = int
来源：http://www.share.hesvh.cn/Article/details/gmbyhgpnu.sHtML

[U29] Py：属性校验
来源：http://read.share.zdbjq.cn/Article/details/gficrxsxe.sHtML

@property 与 @x.setter 配合
来源：http://wap.zdbjq.cn/Article/details/grefiopbe.sHtML

[U30] Py：数据类
来源：http://read.share.zdbjq.cn/Article/details/gxyqevrmf.sHtML

@dataclass(slots=True)
来源：http://www.m.share.fehbvm.com/Article/details/gongnllha.sHtML

[U31] Py：单测
来源：http://read.share.fehbvm.com/Article/details/gskacpcwy.sHtML

python -m pytest -q
来源：http://baike.hesvh.cn/Article/details/gwhontrwp.sHtML

[U32] Py：代码格式化
来源：http://3g.hesvh.cn/Article/details/gczevnoaj.sHtML

ruff format . && ruff check --fix .
来源：http://3g.fehbvm.com/Article/details/gmbtpjfuj.sHtML

[U33] Py：打包发布
来源：http://wap.fehbvm.com/Article/details/gvjrwqmwo.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.hesvh.cn/Article/details/gmredkwuf.sHtML

[U34] Py：判断编码
来源：http://blog.hesvh.cn/Article/details/gnjswrhyb.sHtML

chardet.detect(raw)
来源：http://wap.fehbvm.com/Article/details/gnjmfvuji.sHtML

[U35] Py：发送邮件
来源：http://3g.fehbvm.com/Article/details/gwudgfjey.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.hesvh.cn/Article/details/gsvgpzhpa.sHtML

[U36] Py：定时任务
来源：http://www.blog.zdbjq.cn/Article/details/glzxknpya.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.zdbjq.cn/Article/details/gcanftmxr.sHtML

[U37] Py：读写 Excel
来源：http://www.share.hesvh.cn/Article/details/guqjcepha.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.hesvh.cn/Article/details/gfzhnftbq.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.zdbjq.cn/Article/details/gwyeqpshn.sHtML

Path(__file__).resolve().parent
来源：http://m.share.hesvh.cn/Article/details/gcdxfjmjm.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.hesvh.cn/Article/details/gmvubghjp.sHtML

sys.stdout.isatty()
来源：http://3g.zdbjq.cn/Article/details/gylvtpbue.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.zdbjq.cn/Article/details/gnqjezltl.sHtML

print("err", file=sys.stderr)
来源：http://wap.zdbjq.cn/Article/details/gmflgsuxl.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.hesvh.cn/Article/details/gxgfddsff.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.fehbvm.com/Article/details/gnhsxmgwm.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.fehbvm.com/Article/details/gcjtbhief.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.zdbjq.cn/Article/details/gizwfcxgr.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.zdbjq.cn/Article/details/gkcgmhexf.sHtML

namespace App\Http;
来源：http://baike.zdbjq.cn/Article/details/gbtoqztws.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.hesvh.cn/Article/details/grczovxgt.sHtML

declare(strict_types=1);
来源：http://m.share.fehbvm.com/Article/details/gnhcdeozl.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.zdbjq.cn/Article/details/gcgaeykfb.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/grffdorkl.sHtML

[U46] PHP：可空类型
来源：http://www.blog.fehbvm.com/Article/details/gpvhivxtw.sHtML

?string $name = null
来源：http://baike.fehbvm.com/Article/details/gbbmodpdg.sHtML

[U47] PHP：联合类型
来源：http://3g.hesvh.cn/Article/details/ggomfbkhq.sHtML

int|string $id
来源：http://baike.fehbvm.com/Article/details/gsngqqhfm.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.zdbjq.cn/Article/details/grdhqwafr.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnoskxupu.sHtML

[U49] PHP：只读属性
来源：http://mobile.hesvh.cn/Article/details/gzbbbfoih.sHtML

public readonly string $name
来源：http://m.share.hesvh.cn/Article/details/ggqupsyhd.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.zdbjq.cn/Article/details/gdqzamwpt.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.zdbjq.cn/Article/details/gooboprbv.sHtML

[U51] PHP：数组解构
来源：http://mobile.fehbvm.com/Article/details/gvpltvyaw.sHtML

[$a, $b] = $arr;
来源：http://3g.zdbjq.cn/Article/details/gbqswvbdf.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.zdbjq.cn/Article/details/gehzfzafi.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.fehbvm.com/Article/details/gmczpgarg.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.zdbjq.cn/Article/details/gtnfubsmf.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.zdbjq.cn/Article/details/ggkffjyyh.sHtML

[U54] PHP：空安全调用
来源：http://blog.hesvh.cn/Article/details/gfjaeywsz.sHtML

$obj?->method()
来源：http://read.share.zdbjq.cn/Article/details/goeduyilh.sHtML

[U55] PHP：match 表达式
来源：http://read.share.fehbvm.com/Article/details/gjobzjqmw.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.zdbjq.cn/Article/details/gdusmoxhx.sHtML

[U56] PHP：命名参数
来源：http://3g.zdbjq.cn/Article/details/gigcxyyqu.sHtML

f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/gelhcwehw.sHtML

[U57] PHP：字符串插值
来源：http://wap.hesvh.cn/Article/details/ggltufrda.sHtML

"值: {$a}"
来源：http://wap.hesvh.cn/Article/details/gpkllvqpx.sHtML

[U58] PHP：数组三件套
来源：http://mobile.fehbvm.com/Article/details/gypxbvmqe.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gbxfzeiwv.sHtML

[U59] PHP：自定义排序
来源：http://blog.hesvh.cn/Article/details/ghmnoymyq.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.hesvh.cn/Article/details/gofshdlja.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.zdbjq.cn/Article/details/gwsjdczyg.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.zdbjq.cn/Article/details/gzbmkfyvj.sHtML


<!-- 参考信息 -->