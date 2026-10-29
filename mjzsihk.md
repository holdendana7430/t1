代发 wailian999

[S35] C++：map
来源：http://3g.fehbvm.com/Article/details/ggwfrhhkk.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/glgmadhvx.sHtML

[S36] C++：unordered_map
来源：http://www.blog.zdbjq.cn/Article/details/ggxjsjyxf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/glcczwrka.sHtML

[S37] C++：set
来源：http://baike.hesvh.cn/Article/details/gkmolpnfw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.zdbjq.cn/Article/details/gmqwnlkrq.sHtML

[S38] C++：排序
来源：http://www.m.share.fehbvm.com/Article/details/gekhrxwrr.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.zdbjq.cn/Article/details/glnogjsty.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.zdbjq.cn/Article/details/ggqwnjcun.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.zdbjq.cn/Article/details/gxxibjcrt.sHtML

[S40] C++：查找元素
来源：http://wap.zdbjq.cn/Article/details/gcxvhmhlj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.zdbjq.cn/Article/details/gprurixwe.sHtML

[S41] C++：类与构造函数
来源：http://m.share.hesvh.cn/Article/details/gmzbweswj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fehbvm.com/Article/details/girakovbw.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fehbvm.com/Article/details/gaajegvtp.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.zdbjq.cn/Article/details/guwdejpui.sHtML

[S43] C++：智能指针
来源：http://mobile.fehbvm.com/Article/details/gnrcderde.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fehbvm.com/Article/details/gebsdlpeg.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fehbvm.com/Article/details/gzkaklrnz.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.zdbjq.cn/Article/details/gfjhfowbt.sHtML

[S45] C++：lambda
来源：http://www.blog.hesvh.cn/Article/details/gkrrcyluz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fehbvm.com/Article/details/glelcsttu.sHtML

[S46] C++：函数模板
来源：http://blog.hesvh.cn/Article/details/gjxejctrs.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fehbvm.com/Article/details/gwlkdkbgo.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.hesvh.cn/Article/details/gamgeklhm.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fehbvm.com/Article/details/giecluzgw.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gksmajwno.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.hesvh.cn/Article/details/gpawpmlfd.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.hesvh.cn/Article/details/gzzrvjqbp.sHtML

[S49] C++：写文件
来源：http://baike.fehbvm.com/Article/details/gsqbabvdh.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.hesvh.cn/Article/details/gjsevymgl.sHtML

[S50] C++：格式化数字
来源：http://mobile.hesvh.cn/Article/details/gykfwghhe.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.hesvh.cn/Article/details/glafkteyz.sHtML

[S51] C++：显式类型转换
来源：http://baike.hesvh.cn/Article/details/gxrmgpbyc.sHtML

static_cast<double>(a) / b
来源：http://wap.fehbvm.com/Article/details/gnxmicbbx.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.hesvh.cn/Article/details/gitzotgay.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fehbvm.com/Article/details/gluregwjy.sHtML

[S53] C++：移动语义
来源：http://m.share.fehbvm.com/Article/details/gelrafctt.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fehbvm.com/Article/details/ggmpqbiqu.sHtML

[S54] C++：异常处理
来源：http://www.m.share.hesvh.cn/Article/details/gjkmhcubt.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.hesvh.cn/Article/details/ggxdtchlx.sHtML

[S55] C++：结构化绑定
来源：http://blog.zdbjq.cn/Article/details/grzookxhp.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.zdbjq.cn/Article/details/grbqbyxve.sHtML

[S56] C++：optional
来源：http://wap.hesvh.cn/Article/details/giopjegsn.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fehbvm.com/Article/details/gewwfwblr.sHtML

[S57] C++：编译期常量
来源：http://mobile.hesvh.cn/Article/details/gabsbqtob.sHtML

constexpr int N = 10;
来源：http://mobile.hesvh.cn/Article/details/gvwgbrlzq.sHtML

[S58] C++：命名空间
来源：http://baike.zdbjq.cn/Article/details/ghoeglafk.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fehbvm.com/Article/details/grrrujxiv.sHtML

[S59] C++：静态断言
来源：http://baike.fehbvm.com/Article/details/gvtbfittr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.hesvh.cn/Article/details/gjprdnehh.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fehbvm.com/Article/details/genovcdyn.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.zdbjq.cn/Article/details/gyosyhinx.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gwsavwjku.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fehbvm.com/Article/details/golbmhzqw.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gvpkiortd.sHtML

[T01] Kotlin：Hello World
来源：http://baike.zdbjq.cn/Article/details/ggpljaprz.sHtML

println("Hello")
来源：http://read.share.hesvh.cn/Article/details/gbmzmnjqi.sHtML

[T02] Kotlin：变量
来源：http://m.share.zdbjq.cn/Article/details/grhhvjlax.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.zdbjq.cn/Article/details/gzdsmtflc.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.zdbjq.cn/Article/details/gnkpacvhk.sHtML

"值: $b"
来源：http://wap.fehbvm.com/Article/details/gbvtxzwdc.sHtML

[T04] Kotlin：空安全
来源：http://wap.fehbvm.com/Article/details/gbcyntzqg.sHtML

val n: String? = null;  n?.length
来源：http://read.share.hesvh.cn/Article/details/grkyrtcok.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fehbvm.com/Article/details/gbhkbjefw.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.hesvh.cn/Article/details/gixwathgp.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.zdbjq.cn/Article/details/gwxltyqrt.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.zdbjq.cn/Article/details/gzwpxjmhu.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/gjelgbldl.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fehbvm.com/Article/details/gjohvvuhd.sHtML

[T08] Kotlin：数据类
来源：http://www.share.zdbjq.cn/Article/details/gajkwcvid.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.zdbjq.cn/Article/details/gdmrcfmse.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.hesvh.cn/Article/details/gudhpxisg.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fehbvm.com/Article/details/gbzmycfqo.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.hesvh.cn/Article/details/ggkxqichu.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fehbvm.com/Article/details/gtzhirxgm.sHtML

[T11] Kotlin：协程
来源：http://3g.fehbvm.com/Article/details/gepjzevjs.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.zdbjq.cn/Article/details/gqbloxuek.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fehbvm.com/Article/details/gdiwtswlk.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gcrrdguzb.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.zdbjq.cn/Article/details/gnposwzmc.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.zdbjq.cn/Article/details/gniqlkbxz.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fehbvm.com/Article/details/gsyfwxdvt.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.zdbjq.cn/Article/details/gaptiffzi.sHtML

[T15] Kotlin：接口
来源：http://www.blog.hesvh.cn/Article/details/glsgstpry.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fehbvm.com/Article/details/gjgrdgpvd.sHtML

[T16] Swift：Hello World
来源：http://m.share.zdbjq.cn/Article/details/ghayuycga.sHtML

print("Hello")
来源：http://3g.zdbjq.cn/Article/details/gahxcnlym.sHtML

[T17] Swift：变量与常量
来源：http://blog.fehbvm.com/Article/details/grjlyxdop.sHtML

var a = 1;  let b = 2
来源：http://wap.zdbjq.cn/Article/details/glirenykt.sHtML

[T18] Swift：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gpssksmrv.sHtML

"值: \(b)"
来源：http://read.share.fehbvm.com/Article/details/gdpzmbmwb.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.hesvh.cn/Article/details/gqspxacjr.sHtML

if let n = opt { print(n) }
来源：http://mobile.hesvh.cn/Article/details/gyvpyrfew.sHtML

[T20] Swift：数组操作
来源：http://m.share.hesvh.cn/Article/details/gixbckvri.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fehbvm.com/Article/details/goxjxpoqa.sHtML

[T21] Swift：遍历
来源：http://baike.fehbvm.com/Article/details/grfpxeqhb.sHtML

for x in a { print(x) }
来源：http://3g.hesvh.cn/Article/details/gjtebreyj.sHtML

[T22] Swift：字典
来源：http://mobile.hesvh.cn/Article/details/gxytrqrxn.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.hesvh.cn/Article/details/gaqbelbpy.sHtML

[T23] Swift：函数
来源：http://www.m.share.hesvh.cn/Article/details/geskpfjln.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.zdbjq.cn/Article/details/guheqfdeq.sHtML

[T24] Swift：闭包
来源：http://www.m.share.hesvh.cn/Article/details/gbdveakwc.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gbwmsdhul.sHtML

[T25] Swift：结构体
来源：http://mobile.zdbjq.cn/Article/details/gcwtfbjkq.sHtML

struct P { var x: Int }
来源：http://www.share.zdbjq.cn/Article/details/gqdqesmdj.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.zdbjq.cn/Article/details/gpvgyrmjk.sHtML

class A: Base { override func f() {} }
来源：http://baike.fehbvm.com/Article/details/gjcgrvrsq.sHtML

[T27] Swift：错误处理
来源：http://www.share.fehbvm.com/Article/details/getonrlpw.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fehbvm.com/Article/details/gqsyuxhvu.sHtML

[T28] Swift：枚举
来源：http://baike.hesvh.cn/Article/details/gvncnzbvd.sHtML

enum Color { case red, green }
来源：http://www.share.hesvh.cn/Article/details/gbrletguu.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.fehbvm.com/Article/details/gwcuatzgw.sHtML

guard let x = opt else { return }
来源：http://3g.hesvh.cn/Article/details/gtfddpsly.sHtML

[T30] Swift：协议
来源：http://www.blog.zdbjq.cn/Article/details/gnyhjqovm.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.zdbjq.cn/Article/details/gtpgwanol.sHtML

[T31] Lua：Hello World
来源：http://blog.fehbvm.com/Article/details/gttoivmyg.sHtML

print("Hello")
来源：http://wap.fehbvm.com/Article/details/gdeeeveak.sHtML

[T32] Lua：局部变量
来源：http://baike.zdbjq.cn/Article/details/gqvtwiatn.sHtML

local a = 1
来源：http://baike.hesvh.cn/Article/details/grsbxtnsk.sHtML

[T33] Lua：表（数组）
来源：http://www.share.fehbvm.com/Article/details/gogpbjkxu.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.fehbvm.com/Article/details/gosoqwlne.sHtML

[T34] Lua：遍历表
来源：http://baike.fehbvm.com/Article/details/gvlrxdmqk.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.zdbjq.cn/Article/details/gsvbesxtj.sHtML

[T35] Lua：字典表
来源：http://www.m.share.hesvh.cn/Article/details/gyttqviwc.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.fehbvm.com/Article/details/gachlrcxm.sHtML

[T36] Lua：函数
来源：http://www.blog.hesvh.cn/Article/details/gdkhibfax.sHtML

function add(a, b) return a + b end
来源：http://www.blog.fehbvm.com/Article/details/ggnonbulg.sHtML

[T37] Lua：字符串拼接
来源：http://wap.zdbjq.cn/Article/details/gkkqckytw.sHtML

"a" .. "b"
来源：http://read.share.fehbvm.com/Article/details/gehepbpfu.sHtML

[T38] Lua：条件
来源：http://m.share.fehbvm.com/Article/details/gkdykwkeo.sHtML

if x > 0 then print("正") end
来源：http://3g.zdbjq.cn/Article/details/gqgqeclrq.sHtML

[T39] Lua：模式匹配
来源：http://blog.hesvh.cn/Article/details/gcwuiefoh.sHtML

string.find(s, "%d+")
来源：http://www.blog.fehbvm.com/Article/details/gbfdnpdxv.sHtML

[T40] Lua：元表
来源：http://read.share.hesvh.cn/Article/details/ggfuslqnm.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.fehbvm.com/Article/details/gslrpibsi.sHtML

[T41] Perl：Hello World
来源：http://read.share.fehbvm.com/Article/details/gcfspmosy.sHtML

print "Hello\n";
来源：http://blog.hesvh.cn/Article/details/gmrvfffdv.sHtML

[T42] Perl：变量类型
来源：http://mobile.fehbvm.com/Article/details/geesjlpkl.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.zdbjq.cn/Article/details/goobidspi.sHtML

[T43] Perl：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gjlxfcysk.sHtML

"值: $a"
来源：http://baike.zdbjq.cn/Article/details/gcpqjydkk.sHtML

[T44] Perl：条件
来源：http://baike.zdbjq.cn/Article/details/gdvnsmhcg.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.zdbjq.cn/Article/details/gkwgwbvob.sHtML

[T45] Perl：数组遍历
来源：http://read.share.hesvh.cn/Article/details/gwvanpvve.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.hesvh.cn/Article/details/guxplmryl.sHtML

[T46] Perl：哈希操作
来源：http://wap.hesvh.cn/Article/details/giprplcic.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.zdbjq.cn/Article/details/gaimsuofw.sHtML

[T47] Perl：正则捕获
来源：http://read.share.hesvh.cn/Article/details/gykhktapx.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.zdbjq.cn/Article/details/gvlsyhvcp.sHtML

[T48] Perl：正则替换
来源：http://www.blog.hesvh.cn/Article/details/gjevamerz.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.zdbjq.cn/Article/details/gqappodrl.sHtML

[T49] Perl：函数
来源：http://www.blog.zdbjq.cn/Article/details/gkhxnvlzu.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gnrxceobl.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gldatgico.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.fehbvm.com/Article/details/gkrvxkvil.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.zdbjq.cn/Article/details/gepcsyzqt.sHtML

[T51] Scala：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gsivtlxdu.sHtML

println("Hello")
来源：http://3g.fehbvm.com/Article/details/gpwgenzbf.sHtML

[T52] Scala：变量
来源：http://www.blog.hesvh.cn/Article/details/gbuvdjazy.sHtML

val a = 1;  var b = 2
来源：http://baike.zdbjq.cn/Article/details/garnaqdxq.sHtML

[T53] Scala：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gjbgecbou.sHtML

s"值: $b"
来源：http://www.blog.hesvh.cn/Article/details/ggvinygsa.sHtML

[T54] Scala：集合映射
来源：http://blog.fehbvm.com/Article/details/gzsexkvte.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.fehbvm.com/Article/details/gmepcytkm.sHtML

[T55] Scala：集合过滤
来源：http://mobile.hesvh.cn/Article/details/gsnytbaoi.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.hesvh.cn/Article/details/gblnwprep.sHtML

[T56] Scala：样例类
来源：http://www.m.share.zdbjq.cn/Article/details/gxjedwbdz.sHtML

case class User(name: String, age: Int)
来源：http://read.share.fehbvm.com/Article/details/gdhtfkzom.sHtML

[T57] Scala：模式匹配
来源：http://read.share.fehbvm.com/Article/details/geouhnxzr.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.fehbvm.com/Article/details/gvbjskvop.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.fehbvm.com/Article/details/godntebvt.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.fehbvm.com/Article/details/gfxmfclvq.sHtML

[T59] Scala：循环
来源：http://m.share.fehbvm.com/Article/details/gfepqlpuk.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.hesvh.cn/Article/details/ghjjegisi.sHtML

[T60] Scala：折叠
来源：http://3g.fehbvm.com/Article/details/gcdtyipek.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fehbvm.com/Article/details/gwxzdzlnk.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gtffnayxq.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fehbvm.com/Article/details/geigzfluz.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gbisjncks.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.zdbjq.cn/Article/details/gfnikayhu.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.fehbvm.com/Article/details/gxltmxjtb.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.hesvh.cn/Article/details/gxuwpfpjs.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.zdbjq.cn/Article/details/gtdzfmikn.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.hesvh.cn/Article/details/gdmmnkjzy.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.fehbvm.com/Article/details/gwkpyhrcd.sHtML

[U04] Py：变量调试打印
来源：http://wap.hesvh.cn/Article/details/gntultdvv.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.zdbjq.cn/Article/details/guzenemog.sHtML

[U05] Py：列表去重且保序
来源：http://baike.hesvh.cn/Article/details/gshftktsu.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.fehbvm.com/Article/details/gvjyepmve.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.zdbjq.cn/Article/details/ghzetifse.sHtML

{**a, **b}
来源：http://3g.hesvh.cn/Article/details/gujknbxtj.sHtML

[U07] Py：反转字典键值
来源：http://m.share.fehbvm.com/Article/details/gkpwikwih.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.zdbjq.cn/Article/details/ggeoupuon.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.zdbjq.cn/Article/details/grfnwkbfo.sHtML

[y for x in nested for y in x]
来源：http://wap.fehbvm.com/Article/details/gqhzngpfv.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.fehbvm.com/Article/details/giowamtow.sHtML

max(d, key=d.get)
来源：http://read.share.hesvh.cn/Article/details/gqpcbxtmu.sHtML

[U10] Py：按值排序字典
来源：http://wap.zdbjq.cn/Article/details/gypimwzse.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.zdbjq.cn/Article/details/gixajoyrh.sHtML

[U11] Py：生成器表达式
来源：http://3g.fehbvm.com/Article/details/gdsdqugop.sHtML

(x * 2 for x in arr)
来源：http://wap.zdbjq.cn/Article/details/ggnhmjjtn.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.hesvh.cn/Article/details/gpsnshdqz.sHtML

Counter(arr).most_common(3)
来源：http://m.share.zdbjq.cn/Article/details/gfmewnnee.sHtML

[U13] Py：固定长度队列
来源：http://baike.zdbjq.cn/Article/details/gktxxmryo.sHtML

deque(maxlen=10)
来源：http://baike.zdbjq.cn/Article/details/gnylaeunv.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.hesvh.cn/Article/details/gxkpcuual.sHtML

defaultdict(list)
来源：http://wap.zdbjq.cn/Article/details/gbfgvpygj.sHtML

[U15] Py：高精度计时
来源：http://blog.zdbjq.cn/Article/details/gpxsowkce.sHtML

t = time.perf_counter()
来源：http://www.m.share.hesvh.cn/Article/details/ggysqmvuo.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.fehbvm.com/Article/details/gzpblfyxm.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.zdbjq.cn/Article/details/gatnqaprx.sHtML

[U17] Py：初始化日志
来源：http://www.share.zdbjq.cn/Article/details/gjacokswo.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.fehbvm.com/Article/details/gtesdiiwh.sHtML

[U18] Py：预编译正则
来源：http://3g.hesvh.cn/Article/details/gohudixnh.sHtML

pat = re.compile(r"\d+")
来源：http://blog.hesvh.cn/Article/details/gkidsmqrj.sHtML

[U19] Py：正则替换带回调
来源：http://3g.zdbjq.cn/Article/details/gyjtmbfoy.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.fehbvm.com/Article/details/ggyagaglb.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.zdbjq.cn/Article/details/gzblfafxi.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.fehbvm.com/Article/details/gnigdiksj.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.zdbjq.cn/Article/details/gjuhzhpfk.sHtML

@contextlib.contextmanager
来源：http://mobile.hesvh.cn/Article/details/gvchomfte.sHtML

[U22] Py：矩阵转置
来源：http://www.share.fehbvm.com/Article/details/gbbozedbj.sHtML

list(zip(*m))
来源：http://wap.fehbvm.com/Article/details/gxoiauwge.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.fehbvm.com/Article/details/gqlzwsmwa.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.zdbjq.cn/Article/details/gbqasvpsn.sHtML

[U24] Py：路径操作
来源：http://www.blog.fehbvm.com/Article/details/guzzippgy.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gyxgwqfdm.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.zdbjq.cn/Article/details/gskepzalp.sHtML

csv.DictReader(f)
来源：http://mobile.fehbvm.com/Article/details/gyigwqner.sHtML

[U26] Py：并发下载
来源：http://www.blog.zdbjq.cn/Article/details/gjftqsakz.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.hesvh.cn/Article/details/ggeznztfq.sHtML

[U27] Py：异步 HTTP
来源：http://blog.zdbjq.cn/Article/details/gbekyvszb.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.hesvh.cn/Article/details/gzxazyecw.sHtML

[U28] Py：类型别名
来源：http://mobile.hesvh.cn/Article/details/gwxfobspr.sHtML

UserId = int
来源：http://3g.fehbvm.com/Article/details/gerlsjdvv.sHtML

[U29] Py：属性校验
来源：http://read.share.hesvh.cn/Article/details/gxywhbsqx.sHtML

@property 与 @x.setter 配合
来源：http://3g.hesvh.cn/Article/details/gymrtxcuk.sHtML

[U30] Py：数据类
来源：http://mobile.zdbjq.cn/Article/details/gmhytnjql.sHtML

@dataclass(slots=True)
来源：http://mobile.zdbjq.cn/Article/details/geloceycf.sHtML

[U31] Py：单测
来源：http://3g.zdbjq.cn/Article/details/gbxsqmauy.sHtML

python -m pytest -q
来源：http://www.share.hesvh.cn/Article/details/gkuoojutl.sHtML

[U32] Py：代码格式化
来源：http://wap.hesvh.cn/Article/details/gqmeluhww.sHtML

ruff format . && ruff check --fix .
来源：http://3g.zdbjq.cn/Article/details/gjexhkdbq.sHtML

[U33] Py：打包发布
来源：http://baike.zdbjq.cn/Article/details/gbqrnmfbf.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.hesvh.cn/Article/details/gaahfjado.sHtML

[U34] Py：判断编码
来源：http://mobile.hesvh.cn/Article/details/gqdjalouh.sHtML

chardet.detect(raw)
来源：http://mobile.hesvh.cn/Article/details/gxhybvuxc.sHtML

[U35] Py：发送邮件
来源：http://wap.hesvh.cn/Article/details/gzucfxbwx.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.zdbjq.cn/Article/details/ggrzeymlx.sHtML

[U36] Py：定时任务
来源：http://wap.fehbvm.com/Article/details/gabmyopgr.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.fehbvm.com/Article/details/grsmkmwto.sHtML

[U37] Py：读写 Excel
来源：http://baike.fehbvm.com/Article/details/grfzynlhm.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.zdbjq.cn/Article/details/glmwlimfe.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.fehbvm.com/Article/details/gmkeifauf.sHtML

Path(__file__).resolve().parent
来源：http://www.share.hesvh.cn/Article/details/gsdjwcelu.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.hesvh.cn/Article/details/gkkmfapan.sHtML

sys.stdout.isatty()
来源：http://read.share.hesvh.cn/Article/details/gcpjbkevt.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.hesvh.cn/Article/details/gdrjeufzo.sHtML

print("err", file=sys.stderr)
来源：http://3g.hesvh.cn/Article/details/gzhodxmme.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.hesvh.cn/Article/details/gbabhuxvb.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.hesvh.cn/Article/details/gxovxkzmx.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.zdbjq.cn/Article/details/gomuwvova.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.hesvh.cn/Article/details/ghquhnxwj.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.fehbvm.com/Article/details/gvratakyt.sHtML

namespace App\Http;
来源：http://wap.zdbjq.cn/Article/details/ggkjmeisp.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.hesvh.cn/Article/details/gslzfnmpx.sHtML

declare(strict_types=1);
来源：http://read.share.hesvh.cn/Article/details/gujrkssai.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.hesvh.cn/Article/details/gxvbyitot.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/gszhjnrvt.sHtML

[U46] PHP：可空类型
来源：http://blog.zdbjq.cn/Article/details/gpscrttvi.sHtML

?string $name = null
来源：http://wap.hesvh.cn/Article/details/gorqebutm.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.fehbvm.com/Article/details/gmgsfiaah.sHtML

int|string $id
来源：http://www.blog.hesvh.cn/Article/details/gzjdctthb.sHtML

[U48] PHP：纯枚举
来源：http://3g.fehbvm.com/Article/details/gaigxgnhf.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.hesvh.cn/Article/details/gwxijfjsr.sHtML

[U49] PHP：只读属性
来源：http://www.share.hesvh.cn/Article/details/gwwpxbeuy.sHtML

public readonly string $name
来源：http://m.share.hesvh.cn/Article/details/geixsioui.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.hesvh.cn/Article/details/glfsqnlkd.sHtML

public function __construct(private int $id) {}
来源：http://wap.zdbjq.cn/Article/details/gfxihpbwo.sHtML

[U51] PHP：数组解构
来源：http://blog.zdbjq.cn/Article/details/gfpwycoxy.sHtML

[$a, $b] = $arr;
来源：http://www.share.zdbjq.cn/Article/details/gcvgktsdd.sHtML

[U52] PHP：箭头函数
来源：http://m.share.fehbvm.com/Article/details/gvqlfefdj.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.fehbvm.com/Article/details/ganinstjt.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.fehbvm.com/Article/details/gvbgeojts.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.zdbjq.cn/Article/details/guczrbkwu.sHtML

[U54] PHP：空安全调用
来源：http://www.share.hesvh.cn/Article/details/gtjvpozif.sHtML

$obj?->method()
来源：http://baike.fehbvm.com/Article/details/gorolkjlt.sHtML

[U55] PHP：match 表达式
来源：http://www.share.hesvh.cn/Article/details/gzbwuxcsj.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.zdbjq.cn/Article/details/grarzpswf.sHtML

[U56] PHP：命名参数
来源：http://m.share.hesvh.cn/Article/details/gjkmmqsdy.sHtML

f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/ghasiqjme.sHtML

[U57] PHP：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gxpkoooyo.sHtML

"值: {$a}"
来源：http://m.share.zdbjq.cn/Article/details/gwiocmjsl.sHtML

[U58] PHP：数组三件套
来源：http://blog.zdbjq.cn/Article/details/gxceegyki.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.hesvh.cn/Article/details/gzczpjpvh.sHtML

[U59] PHP：自定义排序
来源：http://www.share.zdbjq.cn/Article/details/giwgfsbbf.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.hesvh.cn/Article/details/gofzjtljb.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.fehbvm.com/Article/details/gbrjbnvap.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.hesvh.cn/Article/details/gaqanobkx.sHtML


<!-- 参考信息 -->