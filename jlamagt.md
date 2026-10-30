代发 wailian999

[S37] C++：set
来源：http://wap.fanxiaobao.xyz/Article/details/gyoidyinm.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gjiijerku.sHtML

[S38] C++：排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gijgcadlk.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/ggxcnhpxe.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gldyjarvd.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fanxiaobao.xyz/Article/details/gujhlktke.sHtML

[S40] C++：查找元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gqjbrhotd.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gkovstxxy.sHtML

[S41] C++：类与构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/gzqhkmayp.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gfjyfktpb.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gdicmjtvf.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfguytzzk.sHtML

[S43] C++：智能指针
来源：http://wap.fanxiaobao.xyz/Article/details/gzttrtvko.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fanxiaobao.xyz/Article/details/gybgwpgpt.sHtML

[S44] C++：引用传参
来源：http://baike.fanxiaobao.xyz/Article/details/gxykzigkh.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtneqvzba.sHtML

[S45] C++：lambda
来源：http://baike.fanxiaobao.xyz/Article/details/gitkfqdfo.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gacgcmqox.sHtML

[S46] C++：函数模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfkqowxlt.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grnetdmgz.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gknkkdqks.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fanxiaobao.xyz/Article/details/gshhetigm.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geqcjfytn.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fanxiaobao.xyz/Article/details/gxepuberi.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gmcigebyh.sHtML

[S49] C++：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gfkrbphge.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaiulriif.sHtML

[S50] C++：格式化数字
来源：http://m.share.fanxiaobao.xyz/Article/details/glgssfkkz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/glcbqrvmq.sHtML

[S51] C++：显式类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/ggustsmrf.sHtML

static_cast<double>(a) / b
来源：http://baike.fanxiaobao.xyz/Article/details/gpcpuwalv.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fanxiaobao.xyz/Article/details/gbxhgiuzw.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbspghjcu.sHtML

[S53] C++：移动语义
来源：http://3g.fanxiaobao.xyz/Article/details/guqwtyuml.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmpzcmkap.sHtML

[S54] C++：异常处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gzrgmzjyq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvdwuwzlc.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gjuufbrsd.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fanxiaobao.xyz/Article/details/gjrucaqxx.sHtML

[S56] C++：optional
来源：http://m.share.fanxiaobao.xyz/Article/details/gxxiztruj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbuqdigfp.sHtML

[S57] C++：编译期常量
来源：http://3g.fanxiaobao.xyz/Article/details/gilsghsiq.sHtML

constexpr int N = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gjskbrvdp.sHtML

[S58] C++：命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/ghbfoyusp.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.fanxiaobao.xyz/Article/details/gpgzbgkxx.sHtML

[S59] C++：静态断言
来源：http://m.share.fanxiaobao.xyz/Article/details/gkiieqhpd.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fanxiaobao.xyz/Article/details/guewltskq.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fanxiaobao.xyz/Article/details/ghfwnqnme.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gccttbbyn.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gjiobdoky.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fanxiaobao.xyz/Article/details/gdhfwytul.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gofnnqvat.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfndlurej.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gesubnqid.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdkfkdzwk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbaleijlt.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fanxiaobao.xyz/Article/details/gwdwqbtow.sHtML

"值: $b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnpqrgtkw.sHtML

[T04] Kotlin：空安全
来源：http://blog.fanxiaobao.xyz/Article/details/gmxykfeor.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fanxiaobao.xyz/Article/details/gwisttnkz.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gubtuauhp.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fanxiaobao.xyz/Article/details/gmlsimdbp.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fanxiaobao.xyz/Article/details/gkercbzfb.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/gcrmraixp.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/grsyobjrc.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwfmdwacb.sHtML

[T08] Kotlin：数据类
来源：http://blog.fanxiaobao.xyz/Article/details/gavsrzgcm.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpiscuhfv.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fanxiaobao.xyz/Article/details/gbsyhazrn.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfoojavdv.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gxksznqyd.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fanxiaobao.xyz/Article/details/gcoufzhuq.sHtML

[T11] Kotlin：协程
来源：http://read.share.fanxiaobao.xyz/Article/details/goofaosmf.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcqmzujdi.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fanxiaobao.xyz/Article/details/gdwsimsyo.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtaxtzzrt.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fanxiaobao.xyz/Article/details/gxvbnipbf.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gkkblnvto.sHtML

[T14] Kotlin：循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gostbugaf.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghznpnvuu.sHtML

[T15] Kotlin：接口
来源：http://read.share.fanxiaobao.xyz/Article/details/gkawlnabl.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnjtpcddr.sHtML

[T16] Swift：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gcueapqua.sHtML

print("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/glfdelukr.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/grrbgtuvf.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghubqjaec.sHtML

[T18] Swift：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/ggjpwwebb.sHtML

"值: \(b)"
来源：http://3g.fanxiaobao.xyz/Article/details/gswvyfplu.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/grzpliywl.sHtML

if let n = opt { print(n) }
来源：http://blog.fanxiaobao.xyz/Article/details/gfsporjmq.sHtML

[T20] Swift：数组操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gdqdzjrnn.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fanxiaobao.xyz/Article/details/gakrhvcak.sHtML

[T21] Swift：遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gvjkcqndz.sHtML

for x in a { print(x) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnoyiycgb.sHtML

[T22] Swift：字典
来源：http://m.share.fanxiaobao.xyz/Article/details/gpycgusme.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gqvlvisst.sHtML

[T23] Swift：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gvrxoglme.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbhorejab.sHtML

[T24] Swift：闭包
来源：http://read.share.fanxiaobao.xyz/Article/details/gxkryroto.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gripafyxt.sHtML

[T25] Swift：结构体
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjuartbrx.sHtML

struct P { var x: Int }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggqphuyox.sHtML

[T26] Swift：类与重写
来源：http://www.share.fanxiaobao.xyz/Article/details/gsyfhpsgi.sHtML

class A: Base { override func f() {} }
来源：http://read.share.fanxiaobao.xyz/Article/details/grqgnwydc.sHtML

[T27] Swift：错误处理
来源：http://3g.fanxiaobao.xyz/Article/details/gnyyvcebn.sHtML

do { try f() } catch { print(error) }
来源：http://3g.fanxiaobao.xyz/Article/details/gkkvhjmnc.sHtML

[T28] Swift：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gfhvljqni.sHtML

enum Color { case red, green }
来源：http://m.share.fanxiaobao.xyz/Article/details/guzhgqwkz.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.fanxiaobao.xyz/Article/details/gxnjoleqk.sHtML

guard let x = opt else { return }
来源：http://read.share.fanxiaobao.xyz/Article/details/gybxqqdkm.sHtML

[T30] Swift：协议
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gofdxeong.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.fanxiaobao.xyz/Article/details/gdpcxquys.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggqrnlpcj.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/grayhucth.sHtML

[T32] Lua：局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghmnezeyk.sHtML

local a = 1
来源：http://wap.fanxiaobao.xyz/Article/details/gznioluqv.sHtML

[T33] Lua：表（数组）
来源：http://m.share.fanxiaobao.xyz/Article/details/gjqbjhebb.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fanxiaobao.xyz/Article/details/gdqogtbee.sHtML

[T34] Lua：遍历表
来源：http://wap.fanxiaobao.xyz/Article/details/gvgogtpws.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtpwrhgjh.sHtML

[T35] Lua：字典表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmmsztgwp.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gumzsgldu.sHtML

[T36] Lua：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gzasxneam.sHtML

function add(a, b) return a + b end
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghyguneos.sHtML

[T37] Lua：字符串拼接
来源：http://blog.fanxiaobao.xyz/Article/details/gsmwjhgoh.sHtML

"a" .. "b"
来源：http://blog.fanxiaobao.xyz/Article/details/gwivjkxaj.sHtML

[T38] Lua：条件
来源：http://3g.fanxiaobao.xyz/Article/details/gczwbeyhc.sHtML

if x > 0 then print("正") end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxvrwoqpp.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpzbotkxm.sHtML

string.find(s, "%d+")
来源：http://blog.fanxiaobao.xyz/Article/details/gctlhpvyx.sHtML

[T40] Lua：元表
来源：http://mobile.fanxiaobao.xyz/Article/details/gdejjyhkf.sHtML

setmetatable({}, { __index = base })
来源：http://wap.fanxiaobao.xyz/Article/details/gkdzkenco.sHtML

[T41] Perl：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/grszbfflo.sHtML

print "Hello\n";
来源：http://baike.fanxiaobao.xyz/Article/details/gaocendnw.sHtML

[T42] Perl：变量类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gkqrjijtg.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gykyurrao.sHtML

[T43] Perl：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/ggtukerfb.sHtML

"值: $a"
来源：http://3g.fanxiaobao.xyz/Article/details/gtbbfwoah.sHtML

[T44] Perl：条件
来源：http://wap.fanxiaobao.xyz/Article/details/gwrabsigu.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/geysowajh.sHtML

[T45] Perl：数组遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwhxcotf.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjrjtrrtc.sHtML

[T46] Perl：哈希操作
来源：http://3g.fanxiaobao.xyz/Article/details/guedbsoal.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gxnfsnrcw.sHtML

[T47] Perl：正则捕获
来源：http://read.share.fanxiaobao.xyz/Article/details/gpnylnjxg.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gkyrwhlsg.sHtML

[T48] Perl：正则替换
来源：http://blog.fanxiaobao.xyz/Article/details/gytqjjivo.sHtML

$s =~ s/old/new/g;
来源：http://mobile.fanxiaobao.xyz/Article/details/gcpsktzrd.sHtML

[T49] Perl：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjanahaju.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnyyhbtbo.sHtML

[T50] Perl：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/ghzouzntd.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqghefxli.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.fanxiaobao.xyz/Article/details/guifmeqqz.sHtML

[T51] Scala：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gizyzjqqn.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gdcslvfvs.sHtML

[T52] Scala：变量
来源：http://3g.fanxiaobao.xyz/Article/details/gdhakawtt.sHtML

val a = 1;  var b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/glqpsnbld.sHtML

[T53] Scala：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gpqmrzkmh.sHtML

s"值: $b"
来源：http://3g.fanxiaobao.xyz/Article/details/gjurwduyk.sHtML

[T54] Scala：集合映射
来源：http://baike.fanxiaobao.xyz/Article/details/gviejveni.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gogghzkme.sHtML

[T55] Scala：集合过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gpvxpldxk.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gccwnctmj.sHtML

[T56] Scala：样例类
来源：http://read.share.fanxiaobao.xyz/Article/details/gwjtsgweu.sHtML

case class User(name: String, age: Int)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvnkzxnpy.sHtML

[T57] Scala：模式匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gxxmgdxqx.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghsejmoxg.sHtML

[T58] Scala：函数定义
来源：http://blog.fanxiaobao.xyz/Article/details/gsgptgplf.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fanxiaobao.xyz/Article/details/gdhzcuthi.sHtML

[T59] Scala：循环
来源：http://baike.fanxiaobao.xyz/Article/details/gpsugohrp.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.fanxiaobao.xyz/Article/details/giwnfeoxi.sHtML

[T60] Scala：折叠
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdbyoalvy.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyckkjrcg.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gjernldwi.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gbuadadyf.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gnaezwiih.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.fanxiaobao.xyz/Article/details/ghddgvnmc.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.fanxiaobao.xyz/Article/details/gtcginomy.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwajwytod.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvnddneib.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.fanxiaobao.xyz/Article/details/givcrguqb.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.fanxiaobao.xyz/Article/details/ghhlmmtbm.sHtML

[U04] Py：变量调试打印
来源：http://read.share.fanxiaobao.xyz/Article/details/gjjqkuukc.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.fanxiaobao.xyz/Article/details/gnvblevze.sHtML

[U05] Py：列表去重且保序
来源：http://wap.fanxiaobao.xyz/Article/details/gkwyuttif.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.fanxiaobao.xyz/Article/details/gohqugfnn.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fanxiaobao.xyz/Article/details/glfdkqilu.sHtML

{**a, **b}
来源：http://blog.fanxiaobao.xyz/Article/details/ghcfodbmu.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcpgncrvw.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.fanxiaobao.xyz/Article/details/ghbdzzdyw.sHtML

[U08] Py：展平二维列表
来源：http://mobile.fanxiaobao.xyz/Article/details/gowroogic.sHtML

[y for x in nested for y in x]
来源：http://baike.fanxiaobao.xyz/Article/details/gbajheuwr.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.fanxiaobao.xyz/Article/details/gdcqwgqev.sHtML

max(d, key=d.get)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbtfmdvdp.sHtML

[U10] Py：按值排序字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gdhwuahip.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.fanxiaobao.xyz/Article/details/gatrgxmau.sHtML

[U11] Py：生成器表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gecnnffnm.sHtML

(x * 2 for x in arr)
来源：http://wap.fanxiaobao.xyz/Article/details/gfdnsowry.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.fanxiaobao.xyz/Article/details/gcfhbeehp.sHtML

Counter(arr).most_common(3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyikyglhy.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmljdbanp.sHtML

deque(maxlen=10)
来源：http://mobile.fanxiaobao.xyz/Article/details/gokmipuzf.sHtML

[U14] Py：分组收集到列表
来源：http://blog.fanxiaobao.xyz/Article/details/ginabuenq.sHtML

defaultdict(list)
来源：http://3g.fanxiaobao.xyz/Article/details/gkrnpxfdy.sHtML

[U15] Py：高精度计时
来源：http://3g.fanxiaobao.xyz/Article/details/gpbheraso.sHtML

t = time.perf_counter()
来源：http://read.share.fanxiaobao.xyz/Article/details/ghozscqvm.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdnytaemj.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaebyvszb.sHtML

[U17] Py：初始化日志
来源：http://3g.fanxiaobao.xyz/Article/details/gvbuolzhq.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.fanxiaobao.xyz/Article/details/gewxziche.sHtML

[U18] Py：预编译正则
来源：http://3g.fanxiaobao.xyz/Article/details/gtplwocsg.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/gzpfuanux.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gprrgynkv.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghicxgtpt.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcqjtmjlz.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkzqyykkg.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.fanxiaobao.xyz/Article/details/gnmnevcvl.sHtML

@contextlib.contextmanager
来源：http://www.share.fanxiaobao.xyz/Article/details/giqwynslp.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjyzrxfrk.sHtML

list(zip(*m))
来源：http://mobile.fanxiaobao.xyz/Article/details/gtdfeuihy.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gclcctzhc.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.fanxiaobao.xyz/Article/details/ghsoeuwpe.sHtML

[U24] Py：路径操作
来源：http://3g.fanxiaobao.xyz/Article/details/ghewipwlr.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.fanxiaobao.xyz/Article/details/ggabjzgfj.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.fanxiaobao.xyz/Article/details/gdwartmfm.sHtML

csv.DictReader(f)
来源：http://read.share.fanxiaobao.xyz/Article/details/golzrnaln.sHtML

[U26] Py：并发下载
来源：http://baike.fanxiaobao.xyz/Article/details/gqiujmigr.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.fanxiaobao.xyz/Article/details/ghqchuduv.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfguwfwmv.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.fanxiaobao.xyz/Article/details/gmtnhfulv.sHtML

[U28] Py：类型别名
来源：http://www.blog.fanxiaobao.xyz/Article/details/gposhjomy.sHtML

UserId = int
来源：http://baike.fanxiaobao.xyz/Article/details/gmuslrgwl.sHtML

[U29] Py：属性校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmoqsswha.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtrgkyklw.sHtML

[U30] Py：数据类
来源：http://mobile.fanxiaobao.xyz/Article/details/gfuaulogt.sHtML

@dataclass(slots=True)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gscqvimdr.sHtML

[U31] Py：单测
来源：http://m.share.fanxiaobao.xyz/Article/details/gwzrivyul.sHtML

python -m pytest -q
来源：http://blog.fanxiaobao.xyz/Article/details/gatmojacf.sHtML

[U32] Py：代码格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/geonknmoe.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.fanxiaobao.xyz/Article/details/gknztkxae.sHtML

[U33] Py：打包发布
来源：http://www.share.fanxiaobao.xyz/Article/details/gtketjnmh.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqyonqwlz.sHtML

[U34] Py：判断编码
来源：http://read.share.fanxiaobao.xyz/Article/details/gyrtiucnu.sHtML

chardet.detect(raw)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpiquqzzd.sHtML

[U35] Py：发送邮件
来源：http://wap.fanxiaobao.xyz/Article/details/giogotlvw.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjtahdugs.sHtML

[U36] Py：定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/gdeluhsil.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdmcpvcox.sHtML

[U37] Py：读写 Excel
来源：http://m.share.fanxiaobao.xyz/Article/details/gifulbtog.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.fanxiaobao.xyz/Article/details/glqnbyjgs.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.fanxiaobao.xyz/Article/details/gmklszfsu.sHtML

Path(__file__).resolve().parent
来源：http://baike.fanxiaobao.xyz/Article/details/gtbyjakbl.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.fanxiaobao.xyz/Article/details/ggjlosatp.sHtML

sys.stdout.isatty()
来源：http://www.share.fanxiaobao.xyz/Article/details/grakvjezl.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.fanxiaobao.xyz/Article/details/gdqpolnkw.sHtML

print("err", file=sys.stderr)
来源：http://baike.fanxiaobao.xyz/Article/details/gocrycoxf.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.fanxiaobao.xyz/Article/details/gnuajjsgv.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.fanxiaobao.xyz/Article/details/gjzcejvwn.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.fanxiaobao.xyz/Article/details/gialcmydd.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gztpfcbfo.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/grzykkqmy.sHtML

namespace App\Http;
来源：http://baike.fanxiaobao.xyz/Article/details/gymutjjfk.sHtML

[U44] PHP：开启严格类型
来源：http://baike.fanxiaobao.xyz/Article/details/gqpfpqthr.sHtML

declare(strict_types=1);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gizetujuz.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.fanxiaobao.xyz/Article/details/ggazddkrx.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxjbcqpzy.sHtML

[U46] PHP：可空类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gmmkqykmh.sHtML

?string $name = null
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gerjlcsga.sHtML

[U47] PHP：联合类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gfealhdws.sHtML

int|string $id
来源：http://3g.fanxiaobao.xyz/Article/details/gmxczytce.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggnqawyux.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gkzdgztvn.sHtML

[U49] PHP：只读属性
来源：http://m.share.fanxiaobao.xyz/Article/details/gcqgjrdwt.sHtML

public readonly string $name
来源：http://blog.fanxiaobao.xyz/Article/details/grkrwxiqo.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjymdgcda.sHtML

public function __construct(private int $id) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gxbehqtiw.sHtML

[U51] PHP：数组解构
来源：http://mobile.fanxiaobao.xyz/Article/details/gheyzxamw.sHtML

[$a, $b] = $arr;
来源：http://3g.fanxiaobao.xyz/Article/details/gtspvqvcn.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzczdlxsr.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyosyzhhh.sHtML

[U53] PHP：空合并运算符
来源：http://wap.fanxiaobao.xyz/Article/details/gyulsrnwy.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.fanxiaobao.xyz/Article/details/giwdrayhu.sHtML

[U54] PHP：空安全调用
来源：http://wap.fanxiaobao.xyz/Article/details/ggzexampj.sHtML

$obj?->method()
来源：http://blog.fanxiaobao.xyz/Article/details/goeptksnf.sHtML

[U55] PHP：match 表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gwzarcila.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geipwfgum.sHtML

[U56] PHP：命名参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqzpguux.sHtML

f(a: 1, b: 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghpotrvgd.sHtML

[U57] PHP：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gedjjctgo.sHtML

"值: {$a}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvvxwabjj.sHtML

[U58] PHP：数组三件套
来源：http://wap.fanxiaobao.xyz/Article/details/glgusvspc.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtogbhnsx.sHtML

[U59] PHP：自定义排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gcvefkazc.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzpwpagqr.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.fanxiaobao.xyz/Article/details/ghefihdho.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.fanxiaobao.xyz/Article/details/gyfllgoip.sHtML

[U61] PHP：正则
来源：http://wap.fanxiaobao.xyz/Article/details/gwcilbzoe.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqfzgygat.sHtML

[U62] PHP：日期对象
来源：http://www.share.fanxiaobao.xyz/Article/details/gtiicnerr.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.fanxiaobao.xyz/Article/details/ggfhvjyie.sHtML


<!-- 参考信息 -->