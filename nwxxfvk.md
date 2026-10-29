代发 wailian999

[S37] C++：set
来源：http://baike.zdbjq.cn/Article/details/gvrywewfq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fehbvm.com/Article/details/ghaamuxgz.sHtML

[S38] C++：排序
来源：http://mobile.hesvh.cn/Article/details/gjthlpkms.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/gfzuqqhem.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.hesvh.cn/Article/details/girfbohew.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fehbvm.com/Article/details/gziujeahy.sHtML

[S40] C++：查找元素
来源：http://read.share.zdbjq.cn/Article/details/gvtqbcbkq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.zdbjq.cn/Article/details/gxuojsbyn.sHtML

[S41] C++：类与构造函数
来源：http://mobile.zdbjq.cn/Article/details/giferwylh.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.hesvh.cn/Article/details/gwsguoczj.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fehbvm.com/Article/details/gpzywyobs.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fehbvm.com/Article/details/gxbjhteez.sHtML

[S43] C++：智能指针
来源：http://www.blog.hesvh.cn/Article/details/gcxfcqwrc.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.zdbjq.cn/Article/details/gqxgfvfnt.sHtML

[S44] C++：引用传参
来源：http://m.share.hesvh.cn/Article/details/gxigxjhxo.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.hesvh.cn/Article/details/gickuwhie.sHtML

[S45] C++：lambda
来源：http://mobile.zdbjq.cn/Article/details/goqfzcevq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fehbvm.com/Article/details/giljmcejx.sHtML

[S46] C++：函数模板
来源：http://www.m.share.hesvh.cn/Article/details/gddgqeufn.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.hesvh.cn/Article/details/grliwdszt.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fehbvm.com/Article/details/gerjjfrst.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fehbvm.com/Article/details/gfdoqxess.sHtML

[S48] C++：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gsmnxkxdu.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.hesvh.cn/Article/details/gqxjojtmr.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fehbvm.com/Article/details/gpnydstqt.sHtML

[S49] C++：写文件
来源：http://baike.fehbvm.com/Article/details/gfbcnqniw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.hesvh.cn/Article/details/gzysnwlgm.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.zdbjq.cn/Article/details/gbzvcdjte.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fehbvm.com/Article/details/gusuhipei.sHtML

[S51] C++：显式类型转换
来源：http://www.share.hesvh.cn/Article/details/gujymzyqr.sHtML

static_cast<double>(a) / b
来源：http://read.share.hesvh.cn/Article/details/gunbgslst.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.hesvh.cn/Article/details/gcjkztiyn.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fehbvm.com/Article/details/gxenxicyg.sHtML

[S53] C++：移动语义
来源：http://mobile.zdbjq.cn/Article/details/gxfyzujyn.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fehbvm.com/Article/details/gnanslzxt.sHtML

[S54] C++：异常处理
来源：http://www.share.fehbvm.com/Article/details/gapmshkdw.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fehbvm.com/Article/details/gxjegsjys.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fehbvm.com/Article/details/gigkkkbjn.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.hesvh.cn/Article/details/gmeucuyln.sHtML

[S56] C++：optional
来源：http://3g.fehbvm.com/Article/details/gfhaqocwt.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.hesvh.cn/Article/details/gvqdidgzg.sHtML

[S57] C++：编译期常量
来源：http://blog.hesvh.cn/Article/details/gjtaurgob.sHtML

constexpr int N = 10;
来源：http://www.share.fehbvm.com/Article/details/grkfoualz.sHtML

[S58] C++：命名空间
来源：http://blog.hesvh.cn/Article/details/glaxrczii.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.zdbjq.cn/Article/details/gtymjyksi.sHtML

[S59] C++：静态断言
来源：http://m.share.fehbvm.com/Article/details/gcshevwuu.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fehbvm.com/Article/details/gocqvrcrg.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fehbvm.com/Article/details/gojgtmuqx.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/gyknrxspt.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gvgxuiezc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.hesvh.cn/Article/details/grvrrellp.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gfkrbjxkd.sHtML

[T01] Kotlin：Hello World
来源：http://wap.zdbjq.cn/Article/details/gyujafzds.sHtML

println("Hello")
来源：http://wap.zdbjq.cn/Article/details/gntezefer.sHtML

[T02] Kotlin：变量
来源：http://read.share.zdbjq.cn/Article/details/gfltrmxes.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.zdbjq.cn/Article/details/gvlwbfzrc.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.hesvh.cn/Article/details/gomydyvmf.sHtML

"值: $b"
来源：http://mobile.fehbvm.com/Article/details/gqdcmlbwc.sHtML

[T04] Kotlin：空安全
来源：http://wap.zdbjq.cn/Article/details/gqjhpovvh.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fehbvm.com/Article/details/ghjtwrlqj.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fehbvm.com/Article/details/gbcmrxjhk.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.zdbjq.cn/Article/details/gukvtqfwq.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.zdbjq.cn/Article/details/ghfsfpack.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.hesvh.cn/Article/details/gayvejful.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fehbvm.com/Article/details/gzzmuppps.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.hesvh.cn/Article/details/gghsamvlf.sHtML

[T08] Kotlin：数据类
来源：http://baike.zdbjq.cn/Article/details/gcdeaglkg.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.hesvh.cn/Article/details/giowmmzfm.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.zdbjq.cn/Article/details/gfcbyqihq.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.hesvh.cn/Article/details/gimmkmkof.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fehbvm.com/Article/details/gdnolueei.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.hesvh.cn/Article/details/guevnhayd.sHtML

[T11] Kotlin：协程
来源：http://3g.fehbvm.com/Article/details/gzutqngmw.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fehbvm.com/Article/details/gfsdopjme.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.zdbjq.cn/Article/details/gcigllvxs.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/gglxqbohe.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fehbvm.com/Article/details/ghyukgosg.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fehbvm.com/Article/details/ggbmpjrtm.sHtML

[T14] Kotlin：循环
来源：http://baike.zdbjq.cn/Article/details/gpgfprjvw.sHtML

for (i in 1..10) println(i)
来源：http://wap.fehbvm.com/Article/details/gaklwnxiy.sHtML

[T15] Kotlin：接口
来源：http://blog.fehbvm.com/Article/details/ghvlrkyoy.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fehbvm.com/Article/details/ghmoujina.sHtML

[T16] Swift：Hello World
来源：http://www.blog.hesvh.cn/Article/details/giynfsxbc.sHtML

print("Hello")
来源：http://3g.zdbjq.cn/Article/details/gmsozmaqm.sHtML

[T17] Swift：变量与常量
来源：http://wap.hesvh.cn/Article/details/gljhxyvhz.sHtML

var a = 1;  let b = 2
来源：http://baike.fehbvm.com/Article/details/gwakjrefq.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gttgeaivt.sHtML

"值: \(b)"
来源：http://read.share.hesvh.cn/Article/details/gpvyvgdda.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fehbvm.com/Article/details/gibyldrmw.sHtML

if let n = opt { print(n) }
来源：http://baike.fehbvm.com/Article/details/gppewmgyg.sHtML

[T20] Swift：数组操作
来源：http://wap.zdbjq.cn/Article/details/gsewnbgci.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.hesvh.cn/Article/details/gkcqybyeh.sHtML

[T21] Swift：遍历
来源：http://m.share.zdbjq.cn/Article/details/gsdrmdtvu.sHtML

for x in a { print(x) }
来源：http://baike.fehbvm.com/Article/details/galtkawxw.sHtML

[T22] Swift：字典
来源：http://read.share.fehbvm.com/Article/details/ghzmomhkt.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.zdbjq.cn/Article/details/gexoxptpi.sHtML

[T23] Swift：函数
来源：http://3g.fehbvm.com/Article/details/glfguwydk.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.hesvh.cn/Article/details/gubvkvfiu.sHtML

[T24] Swift：闭包
来源：http://mobile.fehbvm.com/Article/details/guohklmus.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/giqhxhqka.sHtML

[T25] Swift：结构体
来源：http://baike.zdbjq.cn/Article/details/gpznadbhj.sHtML

struct P { var x: Int }
来源：http://m.share.hesvh.cn/Article/details/goivhegfr.sHtML

[T26] Swift：类与重写
来源：http://3g.hesvh.cn/Article/details/goqhzofrr.sHtML

class A: Base { override func f() {} }
来源：http://baike.hesvh.cn/Article/details/goleunpok.sHtML

[T27] Swift：错误处理
来源：http://blog.hesvh.cn/Article/details/giptlrkcs.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.hesvh.cn/Article/details/grmqekgjg.sHtML

[T28] Swift：枚举
来源：http://read.share.fehbvm.com/Article/details/gjwmlfkgv.sHtML

enum Color { case red, green }
来源：http://blog.fehbvm.com/Article/details/gyriaylhs.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fehbvm.com/Article/details/gyahukpme.sHtML

guard let x = opt else { return }
来源：http://read.share.zdbjq.cn/Article/details/gzovxmugt.sHtML

[T30] Swift：协议
来源：http://www.m.share.hesvh.cn/Article/details/gdzlmhfao.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fehbvm.com/Article/details/gmwzlxxcj.sHtML

[T31] Lua：Hello World
来源：http://m.share.fehbvm.com/Article/details/gkcaxfqnd.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/ggfkgtfvt.sHtML

[T32] Lua：局部变量
来源：http://baike.zdbjq.cn/Article/details/gbftpdujf.sHtML

local a = 1
来源：http://mobile.fehbvm.com/Article/details/gpmxzjzxl.sHtML

[T33] Lua：表（数组）
来源：http://www.share.hesvh.cn/Article/details/grbxvqgsb.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.zdbjq.cn/Article/details/gapvuajhc.sHtML

[T34] Lua：遍历表
来源：http://baike.hesvh.cn/Article/details/ggbiscsyt.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fehbvm.com/Article/details/gwrakunbj.sHtML

[T35] Lua：字典表
来源：http://www.share.hesvh.cn/Article/details/gjvcgrynn.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.hesvh.cn/Article/details/gmebatuqj.sHtML

[T36] Lua：函数
来源：http://3g.fehbvm.com/Article/details/ghczqteez.sHtML

function add(a, b) return a + b end
来源：http://3g.zdbjq.cn/Article/details/gjgcgsfml.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.fehbvm.com/Article/details/giomhdsbe.sHtML

"a" .. "b"
来源：http://baike.zdbjq.cn/Article/details/gojfgmszc.sHtML

[T38] Lua：条件
来源：http://blog.zdbjq.cn/Article/details/gukigyvqk.sHtML

if x > 0 then print("正") end
来源：http://m.share.hesvh.cn/Article/details/gmfmgtpvg.sHtML

[T39] Lua：模式匹配
来源：http://read.share.zdbjq.cn/Article/details/gddkmeeyo.sHtML

string.find(s, "%d+")
来源：http://www.blog.hesvh.cn/Article/details/gbzbyvued.sHtML

[T40] Lua：元表
来源：http://wap.zdbjq.cn/Article/details/gewbsxymj.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.zdbjq.cn/Article/details/gzvyhllud.sHtML

[T41] Perl：Hello World
来源：http://blog.fehbvm.com/Article/details/guvaujayq.sHtML

print "Hello\n";
来源：http://blog.fehbvm.com/Article/details/gilvaqjhc.sHtML

[T42] Perl：变量类型
来源：http://baike.hesvh.cn/Article/details/gkprqqdvf.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.fehbvm.com/Article/details/gmpzviylm.sHtML

[T43] Perl：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gddeygaew.sHtML

"值: $a"
来源：http://www.m.share.hesvh.cn/Article/details/gnnepetfj.sHtML

[T44] Perl：条件
来源：http://m.share.hesvh.cn/Article/details/gleracnll.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.hesvh.cn/Article/details/glzeacuok.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.hesvh.cn/Article/details/ggmcrxcrd.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.hesvh.cn/Article/details/gxpszxxsu.sHtML

[T46] Perl：哈希操作
来源：http://wap.zdbjq.cn/Article/details/gyzsglwqb.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.fehbvm.com/Article/details/gikgcpisc.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.zdbjq.cn/Article/details/gcsteicqr.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.hesvh.cn/Article/details/gvgvcbqme.sHtML

[T48] Perl：正则替换
来源：http://baike.fehbvm.com/Article/details/gfbwzkoot.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.fehbvm.com/Article/details/gsnekpvvs.sHtML

[T49] Perl：函数
来源：http://blog.zdbjq.cn/Article/details/gututbknn.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/guvuhject.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gtcepnfsn.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.hesvh.cn/Article/details/gftebyevx.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.hesvh.cn/Article/details/gzfexoqad.sHtML

[T51] Scala：Hello World
来源：http://baike.fehbvm.com/Article/details/gkgujaesm.sHtML

println("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gjroccuky.sHtML

[T52] Scala：变量
来源：http://www.blog.hesvh.cn/Article/details/gfltlupce.sHtML

val a = 1;  var b = 2
来源：http://mobile.hesvh.cn/Article/details/gaaihurqg.sHtML

[T53] Scala：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gqktfyqza.sHtML

s"值: $b"
来源：http://m.share.fehbvm.com/Article/details/grilystnh.sHtML

[T54] Scala：集合映射
来源：http://baike.zdbjq.cn/Article/details/gaeejdolg.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gwqwajtgn.sHtML

[T55] Scala：集合过滤
来源：http://read.share.zdbjq.cn/Article/details/givmcwrub.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.zdbjq.cn/Article/details/gmznceglk.sHtML

[T56] Scala：样例类
来源：http://read.share.fehbvm.com/Article/details/gpfdiskna.sHtML

case class User(name: String, age: Int)
来源：http://m.share.hesvh.cn/Article/details/giwshwgyt.sHtML

[T57] Scala：模式匹配
来源：http://3g.fehbvm.com/Article/details/gfcgjktob.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.zdbjq.cn/Article/details/gkrlwzddf.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.hesvh.cn/Article/details/givciiugo.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.hesvh.cn/Article/details/gjgdxvcct.sHtML

[T59] Scala：循环
来源：http://blog.zdbjq.cn/Article/details/gjaljsviw.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.hesvh.cn/Article/details/gpvtnfhay.sHtML

[T60] Scala：折叠
来源：http://3g.fehbvm.com/Article/details/gxpavtsdj.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.hesvh.cn/Article/details/gvtyvaxjx.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gijkcfbco.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.zdbjq.cn/Article/details/ggregkzgr.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gsintprnt.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.zdbjq.cn/Article/details/gjskawccq.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.hesvh.cn/Article/details/gcmhggdks.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.hesvh.cn/Article/details/gkmmlrofx.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.fehbvm.com/Article/details/gesroulwq.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.hesvh.cn/Article/details/gqsgyovah.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.hesvh.cn/Article/details/gduswyljy.sHtML

[U04] Py：变量调试打印
来源：http://read.share.zdbjq.cn/Article/details/gxldmuquu.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.fehbvm.com/Article/details/gktlitgrz.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.hesvh.cn/Article/details/gygzywgfc.sHtML

list(dict.fromkeys(arr))
来源：http://3g.fehbvm.com/Article/details/gbsboaucd.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.zdbjq.cn/Article/details/gxobjtrsb.sHtML

{**a, **b}
来源：http://www.share.zdbjq.cn/Article/details/gqtjcpuno.sHtML

[U07] Py：反转字典键值
来源：http://baike.zdbjq.cn/Article/details/ggsrgoufp.sHtML

{v: k for k, v in d.items()}
来源：http://blog.zdbjq.cn/Article/details/gsimswvsr.sHtML

[U08] Py：展平二维列表
来源：http://wap.hesvh.cn/Article/details/gcwkariee.sHtML

[y for x in nested for y in x]
来源：http://www.share.zdbjq.cn/Article/details/gsnjncdlk.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.zdbjq.cn/Article/details/gqneeebyd.sHtML

max(d, key=d.get)
来源：http://www.m.share.zdbjq.cn/Article/details/geyjgurzh.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.fehbvm.com/Article/details/gtmjzpuny.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.zdbjq.cn/Article/details/gqvmsaprv.sHtML

[U11] Py：生成器表达式
来源：http://3g.hesvh.cn/Article/details/gexgnlwtt.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gvfgdrnry.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.fehbvm.com/Article/details/gbhunybgz.sHtML

Counter(arr).most_common(3)
来源：http://mobile.zdbjq.cn/Article/details/gyytwyqcm.sHtML

[U13] Py：固定长度队列
来源：http://baike.hesvh.cn/Article/details/glccpqxgf.sHtML

deque(maxlen=10)
来源：http://m.share.fehbvm.com/Article/details/gvzizomjc.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.hesvh.cn/Article/details/ggspvqnwr.sHtML

defaultdict(list)
来源：http://blog.hesvh.cn/Article/details/guurtxkhp.sHtML

[U15] Py：高精度计时
来源：http://3g.fehbvm.com/Article/details/gwajzvxla.sHtML

t = time.perf_counter()
来源：http://www.share.fehbvm.com/Article/details/gkpdqzcbf.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.fehbvm.com/Article/details/glwcazcqx.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.zdbjq.cn/Article/details/gjrxnfikp.sHtML

[U17] Py：初始化日志
来源：http://3g.zdbjq.cn/Article/details/glsepoyrf.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.zdbjq.cn/Article/details/gfdsodblz.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.hesvh.cn/Article/details/gdpchrsid.sHtML

pat = re.compile(r"\d+")
来源：http://baike.zdbjq.cn/Article/details/gxagfhalp.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.fehbvm.com/Article/details/gdmuxvzvj.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.fehbvm.com/Article/details/gvwemayir.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.zdbjq.cn/Article/details/gmdcvabql.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.zdbjq.cn/Article/details/gglhkrzxv.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.hesvh.cn/Article/details/gloujmqlm.sHtML

@contextlib.contextmanager
来源：http://read.share.fehbvm.com/Article/details/ghurxjnwm.sHtML

[U22] Py：矩阵转置
来源：http://read.share.zdbjq.cn/Article/details/gbbcgzjoz.sHtML

list(zip(*m))
来源：http://www.share.hesvh.cn/Article/details/gcqepbget.sHtML

[U23] Py：分块读取大文件
来源：http://3g.hesvh.cn/Article/details/gucofqiva.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.hesvh.cn/Article/details/gtspjemdk.sHtML

[U24] Py：路径操作
来源：http://www.share.hesvh.cn/Article/details/gudyrgmzv.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.zdbjq.cn/Article/details/gtrshqojs.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.hesvh.cn/Article/details/gqfcfeqfl.sHtML

csv.DictReader(f)
来源：http://baike.fehbvm.com/Article/details/gybvpgfep.sHtML

[U26] Py：并发下载
来源：http://mobile.fehbvm.com/Article/details/gqcewbnfz.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.fehbvm.com/Article/details/gdkjfqybg.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.fehbvm.com/Article/details/gdhhfsxmg.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.hesvh.cn/Article/details/gxkvnzpwz.sHtML

[U28] Py：类型别名
来源：http://wap.hesvh.cn/Article/details/gxahkwyrp.sHtML

UserId = int
来源：http://baike.zdbjq.cn/Article/details/gdqupqncs.sHtML

[U29] Py：属性校验
来源：http://mobile.fehbvm.com/Article/details/gewistuwt.sHtML

@property 与 @x.setter 配合
来源：http://www.share.fehbvm.com/Article/details/giqlhodmd.sHtML

[U30] Py：数据类
来源：http://blog.zdbjq.cn/Article/details/gukrhzfcu.sHtML

@dataclass(slots=True)
来源：http://mobile.hesvh.cn/Article/details/gofimyoah.sHtML

[U31] Py：单测
来源：http://blog.zdbjq.cn/Article/details/gsogyikmh.sHtML

python -m pytest -q
来源：http://3g.fehbvm.com/Article/details/gzcsmrtec.sHtML

[U32] Py：代码格式化
来源：http://m.share.hesvh.cn/Article/details/gwcsuvahf.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.fehbvm.com/Article/details/gkinrrhfz.sHtML

[U33] Py：打包发布
来源：http://mobile.hesvh.cn/Article/details/gezfisolb.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.hesvh.cn/Article/details/grsubtxui.sHtML

[U34] Py：判断编码
来源：http://read.share.fehbvm.com/Article/details/gauxblbxi.sHtML

chardet.detect(raw)
来源：http://3g.fehbvm.com/Article/details/gixwxzdix.sHtML

[U35] Py：发送邮件
来源：http://www.share.hesvh.cn/Article/details/gykuwrpgo.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.zdbjq.cn/Article/details/gvtlpvmps.sHtML

[U36] Py：定时任务
来源：http://www.blog.hesvh.cn/Article/details/gfeebscoc.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.hesvh.cn/Article/details/gezvzttlo.sHtML

[U37] Py：读写 Excel
来源：http://read.share.fehbvm.com/Article/details/gyvlxvrfo.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.zdbjq.cn/Article/details/gfuqyiobk.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.zdbjq.cn/Article/details/gtrinhhjt.sHtML

Path(__file__).resolve().parent
来源：http://3g.zdbjq.cn/Article/details/gguyejazd.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.fehbvm.com/Article/details/gdwagpvnw.sHtML

sys.stdout.isatty()
来源：http://www.share.hesvh.cn/Article/details/guyojduci.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.hesvh.cn/Article/details/ghkoptmmc.sHtML

print("err", file=sys.stderr)
来源：http://www.share.fehbvm.com/Article/details/gjuiiblwq.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.fehbvm.com/Article/details/gsgdpiwxx.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.fehbvm.com/Article/details/gmezivmrv.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.hesvh.cn/Article/details/gbeqemydj.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.zdbjq.cn/Article/details/glfghreml.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.fehbvm.com/Article/details/gsvbuqmdv.sHtML

namespace App\Http;
来源：http://www.blog.hesvh.cn/Article/details/gdlqlgbuk.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.zdbjq.cn/Article/details/gsccpztbi.sHtML

declare(strict_types=1);
来源：http://3g.fehbvm.com/Article/details/ghzrtzlmr.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.fehbvm.com/Article/details/geujlfrha.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/giavcfgvz.sHtML

[U46] PHP：可空类型
来源：http://wap.zdbjq.cn/Article/details/gidymugfp.sHtML

?string $name = null
来源：http://www.blog.zdbjq.cn/Article/details/gqxkamawv.sHtML

[U47] PHP：联合类型
来源：http://read.share.zdbjq.cn/Article/details/gyjaafohy.sHtML

int|string $id
来源：http://wap.fehbvm.com/Article/details/gnfksvebw.sHtML

[U48] PHP：纯枚举
来源：http://m.share.hesvh.cn/Article/details/gwkdvcuwo.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.hesvh.cn/Article/details/gjtdncljy.sHtML

[U49] PHP：只读属性
来源：http://www.blog.fehbvm.com/Article/details/grsogwavq.sHtML

public readonly string $name
来源：http://mobile.hesvh.cn/Article/details/ghkpgolis.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.hesvh.cn/Article/details/gubmwbbnv.sHtML

public function __construct(private int $id) {}
来源：http://blog.zdbjq.cn/Article/details/gyyxrdbgu.sHtML

[U51] PHP：数组解构
来源：http://www.blog.zdbjq.cn/Article/details/gqsctjtkq.sHtML

[$a, $b] = $arr;
来源：http://mobile.zdbjq.cn/Article/details/gaylwtark.sHtML

[U52] PHP：箭头函数
来源：http://blog.zdbjq.cn/Article/details/glzhxhjje.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.zdbjq.cn/Article/details/ganfcillf.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.zdbjq.cn/Article/details/gtxchokkf.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.zdbjq.cn/Article/details/gzpqnbcad.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.hesvh.cn/Article/details/gmeltgjeh.sHtML

$obj?->method()
来源：http://3g.hesvh.cn/Article/details/gbbornslb.sHtML

[U55] PHP：match 表达式
来源：http://www.share.zdbjq.cn/Article/details/gacenuhli.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.zdbjq.cn/Article/details/grlmrvyqh.sHtML

[U56] PHP：命名参数
来源：http://mobile.hesvh.cn/Article/details/gkgxwyedy.sHtML

f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/gnbmwbcat.sHtML

[U57] PHP：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gcskemgwf.sHtML

"值: {$a}"
来源：http://www.m.share.fehbvm.com/Article/details/gtmhiwrtf.sHtML

[U58] PHP：数组三件套
来源：http://blog.fehbvm.com/Article/details/gnbqpcwul.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gcpksvvmh.sHtML

[U59] PHP：自定义排序
来源：http://www.share.zdbjq.cn/Article/details/gqzgunhto.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.zdbjq.cn/Article/details/ghwlmrbys.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.hesvh.cn/Article/details/gfftdmsds.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.hesvh.cn/Article/details/gfircpsal.sHtML

[U61] PHP：正则
来源：http://mobile.zdbjq.cn/Article/details/gjpalkkxb.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fehbvm.com/Article/details/gejvbcagf.sHtML

[U62] PHP：日期对象
来源：http://3g.fehbvm.com/Article/details/gdnppqgms.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.zdbjq.cn/Article/details/gwugsqtnc.sHtML


<!-- 参考信息 -->