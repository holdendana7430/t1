代发 wailian999

[S35] C++：map
来源：http://blog.hesvh.cn/Article/details/gmtdtodvy.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/gxddrefhf.sHtML

[S36] C++：unordered_map
来源：http://read.share.fehbvm.com/Article/details/gwzupivpx.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gxpxtvmlk.sHtML

[S37] C++：set
来源：http://3g.fehbvm.com/Article/details/ghvszewnu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fehbvm.com/Article/details/gwwntwhcl.sHtML

[S38] C++：排序
来源：http://read.share.zdbjq.cn/Article/details/gcyymlmsn.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fehbvm.com/Article/details/gegnmcbwe.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.zdbjq.cn/Article/details/gnpyuzmok.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.zdbjq.cn/Article/details/goigdtsyp.sHtML

[S40] C++：查找元素
来源：http://baike.hesvh.cn/Article/details/gsppcfzmn.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fehbvm.com/Article/details/gnxuitqxr.sHtML

[S41] C++：类与构造函数
来源：http://wap.hesvh.cn/Article/details/gaelrjvtg.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fehbvm.com/Article/details/gmtfpybjy.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fehbvm.com/Article/details/gvyedwhjb.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fehbvm.com/Article/details/gkfcfgfml.sHtML

[S43] C++：智能指针
来源：http://www.share.hesvh.cn/Article/details/gcaldzvij.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fehbvm.com/Article/details/gjszwcxco.sHtML

[S44] C++：引用传参
来源：http://www.blog.fehbvm.com/Article/details/gmnrusdbn.sHtML

void inc(int &x) { ++x; }
来源：http://baike.hesvh.cn/Article/details/gkjahhfzt.sHtML

[S45] C++：lambda
来源：http://www.share.hesvh.cn/Article/details/gicgrfcqg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fehbvm.com/Article/details/gwkovggce.sHtML

[S46] C++：函数模板
来源：http://read.share.fehbvm.com/Article/details/givrignij.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fehbvm.com/Article/details/gcekrzgps.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.zdbjq.cn/Article/details/gnpidsacl.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fehbvm.com/Article/details/gicqhensm.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gbjlbgqgu.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.zdbjq.cn/Article/details/godwomjug.sHtML

while (std::getline(in, line)) { }
来源：http://baike.zdbjq.cn/Article/details/grhejxgpe.sHtML

[S49] C++：写文件
来源：http://3g.fehbvm.com/Article/details/ggbrxccbc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.hesvh.cn/Article/details/gftukbajm.sHtML

[S50] C++：格式化数字
来源：http://read.share.zdbjq.cn/Article/details/glegxgskp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gewtwyywp.sHtML

[S51] C++：显式类型转换
来源：http://wap.hesvh.cn/Article/details/gtrzbdfuo.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.zdbjq.cn/Article/details/ghoiqazrq.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.hesvh.cn/Article/details/gbylqbsfk.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.zdbjq.cn/Article/details/glsbyplwm.sHtML

[S53] C++：移动语义
来源：http://www.m.share.hesvh.cn/Article/details/gngzeaoei.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.hesvh.cn/Article/details/gkrydvynr.sHtML

[S54] C++：异常处理
来源：http://read.share.hesvh.cn/Article/details/gqxgmjvlk.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.hesvh.cn/Article/details/graehkigx.sHtML

[S55] C++：结构化绑定
来源：http://wap.fehbvm.com/Article/details/gepuagaem.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fehbvm.com/Article/details/gopxvohxu.sHtML

[S56] C++：optional
来源：http://m.share.hesvh.cn/Article/details/gobuarxos.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fehbvm.com/Article/details/gorojgjkm.sHtML

[S57] C++：编译期常量
来源：http://3g.fehbvm.com/Article/details/gwrmwzfej.sHtML

constexpr int N = 10;
来源：http://mobile.fehbvm.com/Article/details/gabuwbjtl.sHtML

[S58] C++：命名空间
来源：http://wap.fehbvm.com/Article/details/ggzqmunsg.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.hesvh.cn/Article/details/giwexdbnc.sHtML

[S59] C++：静态断言
来源：http://3g.hesvh.cn/Article/details/guwgsgnmz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.hesvh.cn/Article/details/gydewlcky.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fehbvm.com/Article/details/gwxezhyxf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.hesvh.cn/Article/details/gpwayjbuh.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gjxumbmcz.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.hesvh.cn/Article/details/gfyaphiuj.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gcgpffrim.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gkkjbhumh.sHtML

println("Hello")
来源：http://www.share.hesvh.cn/Article/details/gzkipomcr.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fehbvm.com/Article/details/gedtjvsfc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.hesvh.cn/Article/details/gogbloowy.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fehbvm.com/Article/details/gmgpcyuhl.sHtML

"值: $b"
来源：http://www.m.share.hesvh.cn/Article/details/gywldmdhb.sHtML

[T04] Kotlin：空安全
来源：http://wap.zdbjq.cn/Article/details/gyyzonfoo.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fehbvm.com/Article/details/gmoonfpva.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.zdbjq.cn/Article/details/gwivftdhb.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fehbvm.com/Article/details/gtetailxb.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fehbvm.com/Article/details/glmchobzi.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gowtznksb.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.hesvh.cn/Article/details/gitzyizyl.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fehbvm.com/Article/details/gubfacewv.sHtML

[T08] Kotlin：数据类
来源：http://m.share.hesvh.cn/Article/details/gsujyinqi.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.hesvh.cn/Article/details/gbcjdhmia.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.zdbjq.cn/Article/details/grhwponme.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.zdbjq.cn/Article/details/gavkjylre.sHtML

[T10] Kotlin：默认参数
来源：http://wap.zdbjq.cn/Article/details/gkkplskyt.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.zdbjq.cn/Article/details/gwjlwkljm.sHtML

[T11] Kotlin：协程
来源：http://baike.hesvh.cn/Article/details/gvlzzgyjm.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.hesvh.cn/Article/details/gjaonuwvo.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fehbvm.com/Article/details/gejglcwaz.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.fehbvm.com/Article/details/gtoxlviqi.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.zdbjq.cn/Article/details/gzpujnxss.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.zdbjq.cn/Article/details/gkbznqmqc.sHtML

[T14] Kotlin：循环
来源：http://m.share.fehbvm.com/Article/details/gqinjuggj.sHtML

for (i in 1..10) println(i)
来源：http://mobile.zdbjq.cn/Article/details/gcxqvokqq.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fehbvm.com/Article/details/gkstcykqg.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fehbvm.com/Article/details/ghmsnyunl.sHtML

[T16] Swift：Hello World
来源：http://3g.zdbjq.cn/Article/details/gewkwcsnu.sHtML

print("Hello")
来源：http://wap.fehbvm.com/Article/details/gkjhevxuj.sHtML

[T17] Swift：变量与常量
来源：http://blog.zdbjq.cn/Article/details/gajmpsdse.sHtML

var a = 1;  let b = 2
来源：http://wap.fehbvm.com/Article/details/grkhxrhrj.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gqlntkicm.sHtML

"值: \(b)"
来源：http://blog.zdbjq.cn/Article/details/gnvjulobr.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fehbvm.com/Article/details/gctienvey.sHtML

if let n = opt { print(n) }
来源：http://mobile.zdbjq.cn/Article/details/glykwjpig.sHtML

[T20] Swift：数组操作
来源：http://www.share.hesvh.cn/Article/details/gbtnukcqf.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.fehbvm.com/Article/details/gcpuconqv.sHtML

[T21] Swift：遍历
来源：http://3g.hesvh.cn/Article/details/gxhndkgpw.sHtML

for x in a { print(x) }
来源：http://www.share.hesvh.cn/Article/details/gfcruzxdn.sHtML

[T22] Swift：字典
来源：http://3g.zdbjq.cn/Article/details/gzmgcdafv.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fehbvm.com/Article/details/gtatyiosa.sHtML

[T23] Swift：函数
来源：http://read.share.fehbvm.com/Article/details/gkxymwdii.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.hesvh.cn/Article/details/gkclgavzl.sHtML

[T24] Swift：闭包
来源：http://www.share.hesvh.cn/Article/details/gsyharefq.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.hesvh.cn/Article/details/giauleibv.sHtML

[T25] Swift：结构体
来源：http://wap.fehbvm.com/Article/details/gdjcqpsbk.sHtML

struct P { var x: Int }
来源：http://3g.hesvh.cn/Article/details/gursizwpg.sHtML

[T26] Swift：类与重写
来源：http://baike.hesvh.cn/Article/details/guecryljq.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.hesvh.cn/Article/details/gzlnpihcn.sHtML

[T27] Swift：错误处理
来源：http://m.share.hesvh.cn/Article/details/gdyuelthp.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fehbvm.com/Article/details/galoxkooj.sHtML

[T28] Swift：枚举
来源：http://www.blog.zdbjq.cn/Article/details/gxwyyoxfe.sHtML

enum Color { case red, green }
来源：http://wap.fehbvm.com/Article/details/gkzemtasb.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.zdbjq.cn/Article/details/ghhzawvtc.sHtML

guard let x = opt else { return }
来源：http://www.m.share.fehbvm.com/Article/details/gffgvrwhs.sHtML

[T30] Swift：协议
来源：http://wap.zdbjq.cn/Article/details/gonmpklxf.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.fehbvm.com/Article/details/gxngagwqs.sHtML

[T31] Lua：Hello World
来源：http://3g.zdbjq.cn/Article/details/gihilvgcq.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gesngdoto.sHtML

[T32] Lua：局部变量
来源：http://baike.hesvh.cn/Article/details/gzlmobszb.sHtML

local a = 1
来源：http://m.share.zdbjq.cn/Article/details/gymzcbecw.sHtML

[T33] Lua：表（数组）
来源：http://wap.zdbjq.cn/Article/details/gbxmgzrca.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.hesvh.cn/Article/details/gexqporxs.sHtML

[T34] Lua：遍历表
来源：http://m.share.zdbjq.cn/Article/details/gmejagzpx.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.hesvh.cn/Article/details/gjckqkgrs.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fehbvm.com/Article/details/gwhwhirel.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.zdbjq.cn/Article/details/gzqxdyykd.sHtML

[T36] Lua：函数
来源：http://baike.fehbvm.com/Article/details/ghggmqxlu.sHtML

function add(a, b) return a + b end
来源：http://www.share.hesvh.cn/Article/details/goeckmrvk.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.hesvh.cn/Article/details/gyyzqufvf.sHtML

"a" .. "b"
来源：http://blog.fehbvm.com/Article/details/gowfpexjl.sHtML

[T38] Lua：条件
来源：http://wap.fehbvm.com/Article/details/gagsjqkdd.sHtML

if x > 0 then print("正") end
来源：http://www.blog.zdbjq.cn/Article/details/guwusmpsv.sHtML

[T39] Lua：模式匹配
来源：http://read.share.zdbjq.cn/Article/details/gbmqregak.sHtML

string.find(s, "%d+")
来源：http://baike.hesvh.cn/Article/details/grsniuren.sHtML

[T40] Lua：元表
来源：http://m.share.hesvh.cn/Article/details/gvqumwfsj.sHtML

setmetatable({}, { __index = base })
来源：http://3g.zdbjq.cn/Article/details/gwyuglqnw.sHtML

[T41] Perl：Hello World
来源：http://3g.hesvh.cn/Article/details/gxrtempjb.sHtML

print "Hello\n";
来源：http://3g.hesvh.cn/Article/details/gxmfwtvia.sHtML

[T42] Perl：变量类型
来源：http://blog.fehbvm.com/Article/details/gfygmvfzv.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.fehbvm.com/Article/details/gdfxessdz.sHtML

[T43] Perl：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gjvfgtoxy.sHtML

"值: $a"
来源：http://wap.hesvh.cn/Article/details/gonvqctdk.sHtML

[T44] Perl：条件
来源：http://mobile.zdbjq.cn/Article/details/ghhrfeypo.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.fehbvm.com/Article/details/gljanqhza.sHtML

[T45] Perl：数组遍历
来源：http://blog.hesvh.cn/Article/details/gfufybrij.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.fehbvm.com/Article/details/glntfafow.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fehbvm.com/Article/details/gdoemwdup.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.fehbvm.com/Article/details/gqjjhxisz.sHtML

[T47] Perl：正则捕获
来源：http://wap.fehbvm.com/Article/details/gtkklnxsj.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.hesvh.cn/Article/details/gtmfeldxz.sHtML

[T48] Perl：正则替换
来源：http://wap.fehbvm.com/Article/details/gkuhjndgg.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.hesvh.cn/Article/details/gusumqidk.sHtML

[T49] Perl：函数
来源：http://3g.fehbvm.com/Article/details/gxpxfcshi.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gdzwxmyks.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/glcfnxenq.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.hesvh.cn/Article/details/gdfodxbay.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.zdbjq.cn/Article/details/gdxppaetn.sHtML

[T51] Scala：Hello World
来源：http://blog.fehbvm.com/Article/details/gmzhaszoe.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/ggwptziky.sHtML

[T52] Scala：变量
来源：http://www.blog.hesvh.cn/Article/details/grgxysbct.sHtML

val a = 1;  var b = 2
来源：http://3g.fehbvm.com/Article/details/gskmexxsn.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gjoefgyie.sHtML

s"值: $b"
来源：http://mobile.fehbvm.com/Article/details/gvnslzgga.sHtML

[T54] Scala：集合映射
来源：http://blog.zdbjq.cn/Article/details/grsmmdqhu.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.fehbvm.com/Article/details/ghbjzjpei.sHtML

[T55] Scala：集合过滤
来源：http://mobile.hesvh.cn/Article/details/gdwopuhhk.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.hesvh.cn/Article/details/gioegzbkf.sHtML

[T56] Scala：样例类
来源：http://blog.fehbvm.com/Article/details/grtheahbo.sHtML

case class User(name: String, age: Int)
来源：http://read.share.hesvh.cn/Article/details/gyzijvavh.sHtML

[T57] Scala：模式匹配
来源：http://read.share.hesvh.cn/Article/details/gszahnuqn.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.hesvh.cn/Article/details/gnsznblrr.sHtML

[T58] Scala：函数定义
来源：http://www.share.zdbjq.cn/Article/details/gfcszjwts.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.hesvh.cn/Article/details/gkbhrvfya.sHtML

[T59] Scala：循环
来源：http://blog.hesvh.cn/Article/details/gwlufczjy.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.hesvh.cn/Article/details/glmdlxovo.sHtML

[T60] Scala：折叠
来源：http://read.share.zdbjq.cn/Article/details/gegefhrdk.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.fehbvm.com/Article/details/gfkfmgvco.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gobezmwjk.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.fehbvm.com/Article/details/gdugcslvc.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gkqvcaqmd.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.hesvh.cn/Article/details/gfuavovha.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.hesvh.cn/Article/details/gftogesig.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.fehbvm.com/Article/details/geobgfotb.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.hesvh.cn/Article/details/gdotninpf.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.zdbjq.cn/Article/details/gyjirkkfs.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.hesvh.cn/Article/details/gpfzzqdap.sHtML

[U04] Py：变量调试打印
来源：http://blog.zdbjq.cn/Article/details/gjvcnpkga.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.hesvh.cn/Article/details/gneshgqxt.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.fehbvm.com/Article/details/gxkfaatbq.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.fehbvm.com/Article/details/gqsfdcunk.sHtML

[U06] Py：合并两个字典
来源：http://wap.hesvh.cn/Article/details/gtbltxyag.sHtML

{**a, **b}
来源：http://www.blog.fehbvm.com/Article/details/gvdgxhlow.sHtML

[U07] Py：反转字典键值
来源：http://m.share.fehbvm.com/Article/details/gplflpmgx.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.zdbjq.cn/Article/details/gghtgwvmm.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.hesvh.cn/Article/details/gedgseiom.sHtML

[y for x in nested for y in x]
来源：http://mobile.hesvh.cn/Article/details/gpmjlmxfn.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.zdbjq.cn/Article/details/gdimzmlin.sHtML

max(d, key=d.get)
来源：http://mobile.hesvh.cn/Article/details/gtzhwlvvu.sHtML

[U10] Py：按值排序字典
来源：http://m.share.zdbjq.cn/Article/details/gahoxhfqm.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.hesvh.cn/Article/details/ggbaxaenr.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.fehbvm.com/Article/details/gpxklfvhr.sHtML

(x * 2 for x in arr)
来源：http://m.share.zdbjq.cn/Article/details/gjlvvkdgd.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.fehbvm.com/Article/details/gfsmgluta.sHtML

Counter(arr).most_common(3)
来源：http://www.share.zdbjq.cn/Article/details/gffbwgnkq.sHtML

[U13] Py：固定长度队列
来源：http://baike.fehbvm.com/Article/details/grfeidpdi.sHtML

deque(maxlen=10)
来源：http://wap.fehbvm.com/Article/details/ghufdnnfo.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.fehbvm.com/Article/details/gckhbpeww.sHtML

defaultdict(list)
来源：http://m.share.hesvh.cn/Article/details/gwfzkfqhh.sHtML

[U15] Py：高精度计时
来源：http://read.share.fehbvm.com/Article/details/glfsxoywk.sHtML

t = time.perf_counter()
来源：http://mobile.zdbjq.cn/Article/details/gthfafsmh.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.hesvh.cn/Article/details/gknqoacbs.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.fehbvm.com/Article/details/gozkkgqcf.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.fehbvm.com/Article/details/gturiebao.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.hesvh.cn/Article/details/grfxriuie.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.hesvh.cn/Article/details/gnanuwmsy.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.zdbjq.cn/Article/details/gozosxaxi.sHtML

[U19] Py：正则替换带回调
来源：http://wap.fehbvm.com/Article/details/gzorghtyl.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.hesvh.cn/Article/details/gqvokjzcj.sHtML

[U20] Py：缓存函数结果
来源：http://3g.zdbjq.cn/Article/details/gxmucqfhx.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.fehbvm.com/Article/details/gtgkiofup.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.hesvh.cn/Article/details/gxjfvmtvb.sHtML

@contextlib.contextmanager
来源：http://3g.zdbjq.cn/Article/details/gdmyraool.sHtML

[U22] Py：矩阵转置
来源：http://baike.fehbvm.com/Article/details/gbroardtv.sHtML

list(zip(*m))
来源：http://wap.hesvh.cn/Article/details/giyzkynls.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.zdbjq.cn/Article/details/glivgglho.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.zdbjq.cn/Article/details/gimrlkljr.sHtML

[U24] Py：路径操作
来源：http://baike.fehbvm.com/Article/details/gdlcjawqx.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.zdbjq.cn/Article/details/guyyoxuds.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.hesvh.cn/Article/details/gnfwhfhqs.sHtML

csv.DictReader(f)
来源：http://www.blog.fehbvm.com/Article/details/gcmboziyr.sHtML

[U26] Py：并发下载
来源：http://read.share.fehbvm.com/Article/details/gtkjoohfs.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.zdbjq.cn/Article/details/gdsapcvvx.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.hesvh.cn/Article/details/gasmscrsb.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.fehbvm.com/Article/details/grjsivroh.sHtML

[U28] Py：类型别名
来源：http://www.m.share.hesvh.cn/Article/details/gxqxywdps.sHtML

UserId = int
来源：http://blog.zdbjq.cn/Article/details/gqazubaep.sHtML

[U29] Py：属性校验
来源：http://www.blog.fehbvm.com/Article/details/gvasxbipv.sHtML

@property 与 @x.setter 配合
来源：http://baike.fehbvm.com/Article/details/gbjzjtifo.sHtML

[U30] Py：数据类
来源：http://www.m.share.fehbvm.com/Article/details/gacunfenh.sHtML

@dataclass(slots=True)
来源：http://mobile.zdbjq.cn/Article/details/gepvqjjsz.sHtML

[U31] Py：单测
来源：http://3g.hesvh.cn/Article/details/gseyaqwdj.sHtML

python -m pytest -q
来源：http://www.share.fehbvm.com/Article/details/goknatuhb.sHtML

[U32] Py：代码格式化
来源：http://www.blog.fehbvm.com/Article/details/gmgwkaznf.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.fehbvm.com/Article/details/gfpabqlzu.sHtML

[U33] Py：打包发布
来源：http://www.share.zdbjq.cn/Article/details/gyxcgvzvf.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.hesvh.cn/Article/details/gavtnbdsi.sHtML

[U34] Py：判断编码
来源：http://baike.hesvh.cn/Article/details/gqexvlbqv.sHtML

chardet.detect(raw)
来源：http://baike.zdbjq.cn/Article/details/gqlzcloev.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.fehbvm.com/Article/details/golvyqewv.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.fehbvm.com/Article/details/gjsvgagfo.sHtML

[U36] Py：定时任务
来源：http://baike.fehbvm.com/Article/details/gcggyaqrn.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.hesvh.cn/Article/details/gzhjynkxx.sHtML

[U37] Py：读写 Excel
来源：http://read.share.fehbvm.com/Article/details/gydlsflns.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.hesvh.cn/Article/details/gpwtansct.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.hesvh.cn/Article/details/gxcigvaxj.sHtML

Path(__file__).resolve().parent
来源：http://read.share.hesvh.cn/Article/details/gbxqwbugs.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.fehbvm.com/Article/details/ghksbcyrs.sHtML

sys.stdout.isatty()
来源：http://www.m.share.hesvh.cn/Article/details/geaqddssk.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.hesvh.cn/Article/details/gtfqigxvz.sHtML

print("err", file=sys.stderr)
来源：http://read.share.fehbvm.com/Article/details/gygmhvjhx.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.fehbvm.com/Article/details/gwopmmoax.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.fehbvm.com/Article/details/gvqxlbugm.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.hesvh.cn/Article/details/gpfvrnqoj.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.zdbjq.cn/Article/details/gvvdomnpv.sHtML

[U43] PHP：声明命名空间
来源：http://baike.fehbvm.com/Article/details/gbqhsillo.sHtML

namespace App\Http;
来源：http://blog.zdbjq.cn/Article/details/gmyrlxhvt.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.hesvh.cn/Article/details/gdfyvrqln.sHtML

declare(strict_types=1);
来源：http://wap.fehbvm.com/Article/details/gbgtputba.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.fehbvm.com/Article/details/godtoxfug.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/giayacosw.sHtML

[U46] PHP：可空类型
来源：http://read.share.fehbvm.com/Article/details/gkstfapob.sHtML

?string $name = null
来源：http://www.share.zdbjq.cn/Article/details/gumbzrlap.sHtML

[U47] PHP：联合类型
来源：http://www.share.hesvh.cn/Article/details/gdnqfrwaw.sHtML

int|string $id
来源：http://blog.zdbjq.cn/Article/details/gksppkxqf.sHtML

[U48] PHP：纯枚举
来源：http://m.share.zdbjq.cn/Article/details/gyidtelsg.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.zdbjq.cn/Article/details/glaoeovht.sHtML

[U49] PHP：只读属性
来源：http://baike.fehbvm.com/Article/details/gwimilein.sHtML

public readonly string $name
来源：http://mobile.hesvh.cn/Article/details/gsezsvyst.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.zdbjq.cn/Article/details/gpvpsxenq.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gsrjnhebn.sHtML

[U51] PHP：数组解构
来源：http://mobile.hesvh.cn/Article/details/gvnexlbhg.sHtML

[$a, $b] = $arr;
来源：http://m.share.hesvh.cn/Article/details/ghrdrwrpd.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.hesvh.cn/Article/details/ggvzedqmn.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.zdbjq.cn/Article/details/gacfbsiqx.sHtML

[U53] PHP：空合并运算符
来源：http://wap.fehbvm.com/Article/details/ggbxnpmco.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.zdbjq.cn/Article/details/gtkhjgjpc.sHtML

[U54] PHP：空安全调用
来源：http://blog.hesvh.cn/Article/details/gobswqemx.sHtML

$obj?->method()
来源：http://wap.zdbjq.cn/Article/details/ghgjfiyui.sHtML

[U55] PHP：match 表达式
来源：http://read.share.hesvh.cn/Article/details/gudwefttu.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.zdbjq.cn/Article/details/gjjjjbmyr.sHtML

[U56] PHP：命名参数
来源：http://www.blog.fehbvm.com/Article/details/gwqboadty.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.zdbjq.cn/Article/details/goerxmnam.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gteuhbpyv.sHtML

"值: {$a}"
来源：http://mobile.fehbvm.com/Article/details/gptnvhcfp.sHtML

[U58] PHP：数组三件套
来源：http://m.share.hesvh.cn/Article/details/gvxggbepq.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.zdbjq.cn/Article/details/gvjzbmnyq.sHtML

[U59] PHP：自定义排序
来源：http://m.share.hesvh.cn/Article/details/gbmzwshju.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fehbvm.com/Article/details/gfjvmoemm.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.hesvh.cn/Article/details/gxmqilcfr.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.fehbvm.com/Article/details/gpygduqqt.sHtML


<!-- 参考信息 -->