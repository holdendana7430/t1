代发 wailian999

[S33] C++：vector 增删
来源：http://www.share.fehbvm.com/Article/details/gsbpwgbdw.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fehbvm.com/Article/details/gvilacrxc.sHtML

[S34] C++：遍历 vector
来源：http://mobile.zdbjq.cn/Article/details/gducccdln.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.zdbjq.cn/Article/details/gxxsumuxl.sHtML

[S35] C++：map
来源：http://www.m.share.hesvh.cn/Article/details/grxnfegav.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/gpkzjvcdc.sHtML

[S36] C++：unordered_map
来源：http://baike.hesvh.cn/Article/details/gcroblvtt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gwmkrpkzo.sHtML

[S37] C++：set
来源：http://baike.fehbvm.com/Article/details/gihvwxavh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fehbvm.com/Article/details/gromwioxk.sHtML

[S38] C++：排序
来源：http://mobile.fehbvm.com/Article/details/gpsvyrgbq.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fehbvm.com/Article/details/gfraarhtd.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.zdbjq.cn/Article/details/gwcqxbanh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.hesvh.cn/Article/details/gakkhznjh.sHtML

[S40] C++：查找元素
来源：http://3g.hesvh.cn/Article/details/gngytktkm.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.zdbjq.cn/Article/details/gjtdvvjly.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gnyqtzzcy.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.hesvh.cn/Article/details/gqzbtthnk.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.hesvh.cn/Article/details/gbdpssgxx.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.zdbjq.cn/Article/details/gjxsakdrp.sHtML

[S43] C++：智能指针
来源：http://wap.fehbvm.com/Article/details/ghsewgybe.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fehbvm.com/Article/details/gyopsqxol.sHtML

[S44] C++：引用传参
来源：http://www.blog.zdbjq.cn/Article/details/gyzflzoro.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.hesvh.cn/Article/details/gajmjvugs.sHtML

[S45] C++：lambda
来源：http://read.share.zdbjq.cn/Article/details/grxvzfcit.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.hesvh.cn/Article/details/gvgnricxl.sHtML

[S46] C++：函数模板
来源：http://www.share.hesvh.cn/Article/details/gorzoguux.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.zdbjq.cn/Article/details/gerrqnaug.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.zdbjq.cn/Article/details/gwgfhrzae.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fehbvm.com/Article/details/gixvdlwub.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/grpxkmkgb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fehbvm.com/Article/details/gkuqjfgoq.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.hesvh.cn/Article/details/gxejxcwgc.sHtML

[S49] C++：写文件
来源：http://www.share.fehbvm.com/Article/details/gllkvfotr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.zdbjq.cn/Article/details/gvrzosefs.sHtML

[S50] C++：格式化数字
来源：http://blog.hesvh.cn/Article/details/gxpnvfglz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gdxnvikrl.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fehbvm.com/Article/details/gosvtwrgl.sHtML

static_cast<double>(a) / b
来源：http://mobile.hesvh.cn/Article/details/gssikqyoc.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.hesvh.cn/Article/details/gpevjokih.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fehbvm.com/Article/details/gixldqdnc.sHtML

[S53] C++：移动语义
来源：http://3g.zdbjq.cn/Article/details/gftodqxyf.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.hesvh.cn/Article/details/gjinqpqlz.sHtML

[S54] C++：异常处理
来源：http://www.m.share.hesvh.cn/Article/details/gqumwbgdu.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.zdbjq.cn/Article/details/gymzyjeli.sHtML

[S55] C++：结构化绑定
来源：http://blog.hesvh.cn/Article/details/guonnenlf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.zdbjq.cn/Article/details/gaakeysfj.sHtML

[S56] C++：optional
来源：http://wap.fehbvm.com/Article/details/gefqbmhbg.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fehbvm.com/Article/details/gzhfyddbk.sHtML

[S57] C++：编译期常量
来源：http://baike.hesvh.cn/Article/details/gzvxfbglv.sHtML

constexpr int N = 10;
来源：http://read.share.zdbjq.cn/Article/details/gvhfkzhfe.sHtML

[S58] C++：命名空间
来源：http://3g.hesvh.cn/Article/details/gnfdgyess.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.zdbjq.cn/Article/details/gxvikuunc.sHtML

[S59] C++：静态断言
来源：http://3g.zdbjq.cn/Article/details/ggeiuepkr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.zdbjq.cn/Article/details/gttlqoemm.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.zdbjq.cn/Article/details/glefkxdfq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fehbvm.com/Article/details/gmsdxkjul.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gtyohrmbc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fehbvm.com/Article/details/gidebfhji.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ggjffvstc.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/ggqccidrr.sHtML

println("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/giormdhmv.sHtML

[T02] Kotlin：变量
来源：http://3g.zdbjq.cn/Article/details/gxnlzeavn.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.hesvh.cn/Article/details/gtuuxcgeo.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fehbvm.com/Article/details/gluacmkuu.sHtML

"值: $b"
来源：http://m.share.fehbvm.com/Article/details/gbylqshva.sHtML

[T04] Kotlin：空安全
来源：http://baike.zdbjq.cn/Article/details/goecfutta.sHtML

val n: String? = null;  n?.length
来源：http://blog.fehbvm.com/Article/details/gvehavlnk.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.zdbjq.cn/Article/details/gcoffdsav.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.zdbjq.cn/Article/details/gomijiaxb.sHtML

[T06] Kotlin：集合映射
来源：http://3g.zdbjq.cn/Article/details/gwaebkpck.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.hesvh.cn/Article/details/gotxssfsd.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.hesvh.cn/Article/details/gpajmmxzt.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.zdbjq.cn/Article/details/grdqaiava.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fehbvm.com/Article/details/gifyfgrdd.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.zdbjq.cn/Article/details/gvuoqtgid.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.hesvh.cn/Article/details/gjzrpssau.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.zdbjq.cn/Article/details/gpgwzrqmy.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fehbvm.com/Article/details/gdtjdccet.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.hesvh.cn/Article/details/gsoezfsbj.sHtML

[T11] Kotlin：协程
来源：http://baike.fehbvm.com/Article/details/ghncclqzl.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.hesvh.cn/Article/details/gvxuuvceg.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fehbvm.com/Article/details/gwkzbpevy.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.fehbvm.com/Article/details/gaholrvsn.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.hesvh.cn/Article/details/gflrbepsd.sHtML

val m = mapOf("a" to 1)
来源：http://3g.zdbjq.cn/Article/details/gixxausmf.sHtML

[T14] Kotlin：循环
来源：http://read.share.hesvh.cn/Article/details/gpcswxmfz.sHtML

for (i in 1..10) println(i)
来源：http://m.share.zdbjq.cn/Article/details/gorhzewbr.sHtML

[T15] Kotlin：接口
来源：http://m.share.hesvh.cn/Article/details/gwfjhebch.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.fehbvm.com/Article/details/gbiocdckp.sHtML

[T16] Swift：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gtwmamstq.sHtML

print("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gpiajhpxi.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.zdbjq.cn/Article/details/gczvvodpg.sHtML

var a = 1;  let b = 2
来源：http://3g.hesvh.cn/Article/details/ghaebneza.sHtML

[T18] Swift：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gyemupjvu.sHtML

"值: \(b)"
来源：http://blog.fehbvm.com/Article/details/gmwybjwmt.sHtML

[T19] Swift：可选绑定
来源：http://www.share.zdbjq.cn/Article/details/gzhsbtoot.sHtML

if let n = opt { print(n) }
来源：http://baike.fehbvm.com/Article/details/ggqmlszgj.sHtML

[T20] Swift：数组操作
来源：http://m.share.zdbjq.cn/Article/details/gtbcemxbw.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fehbvm.com/Article/details/gamwgbzpn.sHtML

[T21] Swift：遍历
来源：http://m.share.hesvh.cn/Article/details/goygjdoyg.sHtML

for x in a { print(x) }
来源：http://mobile.fehbvm.com/Article/details/gbuywpjbs.sHtML

[T22] Swift：字典
来源：http://3g.hesvh.cn/Article/details/gbjevqavj.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fehbvm.com/Article/details/gkaklyjhm.sHtML

[T23] Swift：函数
来源：http://wap.hesvh.cn/Article/details/gfrdzjscy.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.zdbjq.cn/Article/details/ghppsxnlw.sHtML

[T24] Swift：闭包
来源：http://mobile.fehbvm.com/Article/details/gbtaxocne.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gszvjhmka.sHtML

[T25] Swift：结构体
来源：http://www.share.hesvh.cn/Article/details/gayddvvrs.sHtML

struct P { var x: Int }
来源：http://www.share.hesvh.cn/Article/details/ghbigscwy.sHtML

[T26] Swift：类与重写
来源：http://baike.zdbjq.cn/Article/details/gsufuzzsc.sHtML

class A: Base { override func f() {} }
来源：http://mobile.zdbjq.cn/Article/details/gpcfxdoqp.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.zdbjq.cn/Article/details/guhsohbjt.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.zdbjq.cn/Article/details/gdsdznfml.sHtML

[T28] Swift：枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gsmitgcuc.sHtML

enum Color { case red, green }
来源：http://3g.hesvh.cn/Article/details/gefgedadh.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.hesvh.cn/Article/details/ghmftawqc.sHtML

guard let x = opt else { return }
来源：http://www.m.share.zdbjq.cn/Article/details/gnlqgwgjs.sHtML

[T30] Swift：协议
来源：http://mobile.hesvh.cn/Article/details/gnvdxxlet.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.hesvh.cn/Article/details/gqvxzbjuf.sHtML

[T31] Lua：Hello World
来源：http://wap.hesvh.cn/Article/details/gjbrjsdax.sHtML

print("Hello")
来源：http://baike.fehbvm.com/Article/details/gedtzrcsq.sHtML

[T32] Lua：局部变量
来源：http://blog.zdbjq.cn/Article/details/gffmpucss.sHtML

local a = 1
来源：http://blog.zdbjq.cn/Article/details/gepfmyffk.sHtML

[T33] Lua：表（数组）
来源：http://baike.fehbvm.com/Article/details/gyvqkonuk.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.hesvh.cn/Article/details/gklpcbemb.sHtML

[T34] Lua：遍历表
来源：http://read.share.hesvh.cn/Article/details/gkmtvhxyk.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.hesvh.cn/Article/details/gtkrinibz.sHtML

[T35] Lua：字典表
来源：http://mobile.fehbvm.com/Article/details/gkctcqlce.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.hesvh.cn/Article/details/gihhfonwz.sHtML

[T36] Lua：函数
来源：http://blog.hesvh.cn/Article/details/gpinalrjw.sHtML

function add(a, b) return a + b end
来源：http://3g.hesvh.cn/Article/details/gotxwrgse.sHtML

[T37] Lua：字符串拼接
来源：http://wap.hesvh.cn/Article/details/gfjvzvgxn.sHtML

"a" .. "b"
来源：http://baike.zdbjq.cn/Article/details/gqwcnalke.sHtML

[T38] Lua：条件
来源：http://www.share.zdbjq.cn/Article/details/gwpnhevbg.sHtML

if x > 0 then print("正") end
来源：http://m.share.fehbvm.com/Article/details/geuwqjvdo.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.zdbjq.cn/Article/details/ggetegolv.sHtML

string.find(s, "%d+")
来源：http://www.m.share.zdbjq.cn/Article/details/guvutmwno.sHtML

[T40] Lua：元表
来源：http://wap.zdbjq.cn/Article/details/gtofotmhc.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.fehbvm.com/Article/details/gjelwddip.sHtML

[T41] Perl：Hello World
来源：http://3g.fehbvm.com/Article/details/gfbrbysdh.sHtML

print "Hello\n";
来源：http://www.m.share.fehbvm.com/Article/details/gxvbzhhjt.sHtML

[T42] Perl：变量类型
来源：http://read.share.zdbjq.cn/Article/details/gbuaitmqf.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.fehbvm.com/Article/details/gbqgvolna.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gujdpuyaj.sHtML

"值: $a"
来源：http://www.blog.fehbvm.com/Article/details/gewbqqfrz.sHtML

[T44] Perl：条件
来源：http://www.share.zdbjq.cn/Article/details/geonxmzms.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.fehbvm.com/Article/details/gagpufkau.sHtML

[T45] Perl：数组遍历
来源：http://baike.fehbvm.com/Article/details/grjwmybmw.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.fehbvm.com/Article/details/gkkjbxpta.sHtML

[T46] Perl：哈希操作
来源：http://mobile.fehbvm.com/Article/details/ghtfrpora.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggxxakoch.sHtML

[T47] Perl：正则捕获
来源：http://read.share.fehbvm.com/Article/details/gehljngjo.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.fehbvm.com/Article/details/gftpzmnpb.sHtML

[T48] Perl：正则替换
来源：http://www.blog.fehbvm.com/Article/details/gywutwgyd.sHtML

$s =~ s/old/new/g;
来源：http://wap.zdbjq.cn/Article/details/gqcfxwehl.sHtML

[T49] Perl：函数
来源：http://www.blog.hesvh.cn/Article/details/gnxmsjzea.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gjqtybvcp.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gkrpwagym.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.fehbvm.com/Article/details/gpwczbvyo.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.fehbvm.com/Article/details/gondyeuju.sHtML

[T51] Scala：Hello World
来源：http://wap.zdbjq.cn/Article/details/gfabzqczt.sHtML

println("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gmqmupsoh.sHtML

[T52] Scala：变量
来源：http://www.m.share.hesvh.cn/Article/details/grlamsubx.sHtML

val a = 1;  var b = 2
来源：http://wap.fehbvm.com/Article/details/gimiayafn.sHtML

[T53] Scala：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gnlgerdok.sHtML

s"值: $b"
来源：http://www.m.share.zdbjq.cn/Article/details/gnfqextkk.sHtML

[T54] Scala：集合映射
来源：http://3g.zdbjq.cn/Article/details/gtgbfunzp.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.fehbvm.com/Article/details/gywblnpin.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.hesvh.cn/Article/details/gzwyvupde.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.fehbvm.com/Article/details/gvupmyguw.sHtML

[T56] Scala：样例类
来源：http://3g.fehbvm.com/Article/details/gcrlxfhsc.sHtML

case class User(name: String, age: Int)
来源：http://wap.fehbvm.com/Article/details/gfejjibuk.sHtML

[T57] Scala：模式匹配
来源：http://blog.hesvh.cn/Article/details/gpnygmfyr.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.fehbvm.com/Article/details/gfejgnbak.sHtML

[T58] Scala：函数定义
来源：http://baike.zdbjq.cn/Article/details/gxtjukjxg.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.fehbvm.com/Article/details/gktpviggg.sHtML

[T59] Scala：循环
来源：http://3g.zdbjq.cn/Article/details/gozboqirf.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.zdbjq.cn/Article/details/gauivabye.sHtML

[T60] Scala：折叠
来源：http://m.share.fehbvm.com/Article/details/gvfrbjyqh.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.hesvh.cn/Article/details/gyrmngahi.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ggekjrmcy.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fehbvm.com/Article/details/gcwtbvsrl.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gxpvfqcai.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.fehbvm.com/Article/details/gooiglqxw.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.fehbvm.com/Article/details/gmwpzdgky.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.hesvh.cn/Article/details/gjxvnzyne.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.hesvh.cn/Article/details/getwwxusw.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.zdbjq.cn/Article/details/givfnfpve.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.fehbvm.com/Article/details/gqxceykte.sHtML

[U04] Py：变量调试打印
来源：http://read.share.fehbvm.com/Article/details/gdsersvcc.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.hesvh.cn/Article/details/gbbgtolab.sHtML

[U05] Py：列表去重且保序
来源：http://wap.zdbjq.cn/Article/details/gyvceijgz.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.hesvh.cn/Article/details/gpurzvzjd.sHtML

[U06] Py：合并两个字典
来源：http://mobile.fehbvm.com/Article/details/gzjkejswx.sHtML

{**a, **b}
来源：http://www.m.share.zdbjq.cn/Article/details/gkkqydkes.sHtML

[U07] Py：反转字典键值
来源：http://read.share.zdbjq.cn/Article/details/gqeugrdgs.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.fehbvm.com/Article/details/gzdgkefjz.sHtML

[U08] Py：展平二维列表
来源：http://wap.hesvh.cn/Article/details/gqgayfwql.sHtML

[y for x in nested for y in x]
来源：http://www.blog.fehbvm.com/Article/details/gkogniqmm.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.fehbvm.com/Article/details/gbkfxarep.sHtML

max(d, key=d.get)
来源：http://www.m.share.fehbvm.com/Article/details/gxjkypyrd.sHtML

[U10] Py：按值排序字典
来源：http://wap.zdbjq.cn/Article/details/gapcszxln.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.fehbvm.com/Article/details/glbxrrxpz.sHtML

[U11] Py：生成器表达式
来源：http://3g.fehbvm.com/Article/details/gbgntvscg.sHtML

(x * 2 for x in arr)
来源：http://wap.zdbjq.cn/Article/details/gaupvvrxa.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.hesvh.cn/Article/details/gyyeebbgh.sHtML

Counter(arr).most_common(3)
来源：http://www.share.hesvh.cn/Article/details/gzqttzlow.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.fehbvm.com/Article/details/gbxrkzfht.sHtML

deque(maxlen=10)
来源：http://www.m.share.fehbvm.com/Article/details/guqhzoyxi.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.fehbvm.com/Article/details/gvmxlnuqw.sHtML

defaultdict(list)
来源：http://read.share.zdbjq.cn/Article/details/griuszbha.sHtML

[U15] Py：高精度计时
来源：http://baike.zdbjq.cn/Article/details/gbvvbgnzr.sHtML

t = time.perf_counter()
来源：http://m.share.hesvh.cn/Article/details/glrjfugbi.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.hesvh.cn/Article/details/gyrqhbkvy.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.fehbvm.com/Article/details/glwmljzmg.sHtML

[U17] Py：初始化日志
来源：http://baike.fehbvm.com/Article/details/guwbimyza.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.fehbvm.com/Article/details/gndfbunma.sHtML

[U18] Py：预编译正则
来源：http://m.share.zdbjq.cn/Article/details/graelbrnm.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.zdbjq.cn/Article/details/gbbqpiwxr.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.hesvh.cn/Article/details/gsiioqlqt.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.hesvh.cn/Article/details/ghukecjcj.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.fehbvm.com/Article/details/gvccwgezx.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.hesvh.cn/Article/details/gpxcngtsp.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.hesvh.cn/Article/details/grbtpcwkt.sHtML

@contextlib.contextmanager
来源：http://read.share.hesvh.cn/Article/details/gwrtbcbku.sHtML

[U22] Py：矩阵转置
来源：http://3g.hesvh.cn/Article/details/guzrxufba.sHtML

list(zip(*m))
来源：http://www.share.hesvh.cn/Article/details/gsrjsfgoo.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.hesvh.cn/Article/details/gjtigjwup.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.fehbvm.com/Article/details/glrssogys.sHtML

[U24] Py：路径操作
来源：http://mobile.zdbjq.cn/Article/details/ggtzxylar.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.zdbjq.cn/Article/details/gelcawqla.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.zdbjq.cn/Article/details/gqamcybpm.sHtML

csv.DictReader(f)
来源：http://read.share.hesvh.cn/Article/details/ganildfrm.sHtML

[U26] Py：并发下载
来源：http://read.share.fehbvm.com/Article/details/gweavvjhy.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.zdbjq.cn/Article/details/gcpgwsnvl.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.zdbjq.cn/Article/details/gapjjllhv.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.zdbjq.cn/Article/details/ggvvcslnv.sHtML

[U28] Py：类型别名
来源：http://baike.fehbvm.com/Article/details/gzeckyunt.sHtML

UserId = int
来源：http://mobile.hesvh.cn/Article/details/gckuywlgt.sHtML

[U29] Py：属性校验
来源：http://www.blog.zdbjq.cn/Article/details/galsruwla.sHtML

@property 与 @x.setter 配合
来源：http://mobile.zdbjq.cn/Article/details/ggephgvel.sHtML

[U30] Py：数据类
来源：http://www.share.zdbjq.cn/Article/details/gbefnicfn.sHtML

@dataclass(slots=True)
来源：http://3g.hesvh.cn/Article/details/gdpmbdnwb.sHtML

[U31] Py：单测
来源：http://blog.hesvh.cn/Article/details/gkdawbpsp.sHtML

python -m pytest -q
来源：http://m.share.fehbvm.com/Article/details/gsbufopzc.sHtML

[U32] Py：代码格式化
来源：http://3g.zdbjq.cn/Article/details/gfhotzimc.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.fehbvm.com/Article/details/ggcahbpxh.sHtML

[U33] Py：打包发布
来源：http://www.m.share.zdbjq.cn/Article/details/glxobcbux.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.fehbvm.com/Article/details/gtpvlrngv.sHtML

[U34] Py：判断编码
来源：http://read.share.hesvh.cn/Article/details/gvsoxginf.sHtML

chardet.detect(raw)
来源：http://blog.zdbjq.cn/Article/details/glxshsnbj.sHtML

[U35] Py：发送邮件
来源：http://read.share.fehbvm.com/Article/details/grjdmxvdj.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.fehbvm.com/Article/details/gqzweiyio.sHtML

[U36] Py：定时任务
来源：http://mobile.zdbjq.cn/Article/details/gsjcnfrsh.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.fehbvm.com/Article/details/gemlxizar.sHtML

[U37] Py：读写 Excel
来源：http://wap.zdbjq.cn/Article/details/gzulxpxsr.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.fehbvm.com/Article/details/gmjoftfwk.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.zdbjq.cn/Article/details/gmuvoaanf.sHtML

Path(__file__).resolve().parent
来源：http://blog.zdbjq.cn/Article/details/gtfsbftvo.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.fehbvm.com/Article/details/gkshemyxo.sHtML

sys.stdout.isatty()
来源：http://mobile.hesvh.cn/Article/details/gjrrmqxrr.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.hesvh.cn/Article/details/gkpqalswi.sHtML

print("err", file=sys.stderr)
来源：http://baike.fehbvm.com/Article/details/gybclijjd.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.fehbvm.com/Article/details/gecjkjyli.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.fehbvm.com/Article/details/gvufafwul.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.hesvh.cn/Article/details/gopgoytok.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.zdbjq.cn/Article/details/ghuxnufnc.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.fehbvm.com/Article/details/gxstidgve.sHtML

namespace App\Http;
来源：http://wap.hesvh.cn/Article/details/gihqcumoo.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.fehbvm.com/Article/details/gsziifmui.sHtML

declare(strict_types=1);
来源：http://www.m.share.fehbvm.com/Article/details/gntcaboje.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.zdbjq.cn/Article/details/ghndyklvy.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gfrgcnlhn.sHtML

[U46] PHP：可空类型
来源：http://3g.zdbjq.cn/Article/details/gcwyuthgf.sHtML

?string $name = null
来源：http://wap.hesvh.cn/Article/details/gtrivbsiw.sHtML

[U47] PHP：联合类型
来源：http://blog.fehbvm.com/Article/details/gibicasjt.sHtML

int|string $id
来源：http://baike.zdbjq.cn/Article/details/ghdkuttjz.sHtML

[U48] PHP：纯枚举
来源：http://blog.hesvh.cn/Article/details/gsbxufzak.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.fehbvm.com/Article/details/gsfhoommb.sHtML

[U49] PHP：只读属性
来源：http://www.share.hesvh.cn/Article/details/glpwzsrrt.sHtML

public readonly string $name
来源：http://blog.fehbvm.com/Article/details/goiopxgll.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.zdbjq.cn/Article/details/gzaftzdaf.sHtML

public function __construct(private int $id) {}
来源：http://blog.hesvh.cn/Article/details/gimqlanqp.sHtML

[U51] PHP：数组解构
来源：http://baike.zdbjq.cn/Article/details/gsnidiyni.sHtML

[$a, $b] = $arr;
来源：http://blog.zdbjq.cn/Article/details/gkcfonskf.sHtML

[U52] PHP：箭头函数
来源：http://read.share.hesvh.cn/Article/details/ggkiroswx.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.hesvh.cn/Article/details/goalvleux.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.zdbjq.cn/Article/details/gzpekzykb.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.zdbjq.cn/Article/details/gseqanpup.sHtML

[U54] PHP：空安全调用
来源：http://mobile.hesvh.cn/Article/details/gocxvlacp.sHtML

$obj?->method()
来源：http://3g.zdbjq.cn/Article/details/grxxharwj.sHtML

[U55] PHP：match 表达式
来源：http://www.share.fehbvm.com/Article/details/grdiedncj.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.fehbvm.com/Article/details/gedayhoeo.sHtML

[U56] PHP：命名参数
来源：http://mobile.fehbvm.com/Article/details/gaiojtjlo.sHtML

f(a: 1, b: 2)
来源：http://read.share.hesvh.cn/Article/details/gnzjifpxt.sHtML

[U57] PHP：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gjylxubmz.sHtML

"值: {$a}"
来源：http://read.share.fehbvm.com/Article/details/gsdhzbigx.sHtML

[U58] PHP：数组三件套
来源：http://3g.zdbjq.cn/Article/details/gylsbnxni.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.fehbvm.com/Article/details/gtxzhticl.sHtML


<!-- 参考信息 -->