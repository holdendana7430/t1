代发 wailian999

[S37] C++：set
来源：http://mobile.fehbvm.com/Article/details/gcfjqkowv.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.zdbjq.cn/Article/details/gcajsrxkv.sHtML

[S38] C++：排序
来源：http://m.share.zdbjq.cn/Article/details/gjxqliycg.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/gfdwkoifi.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fehbvm.com/Article/details/gdbqtgjhz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fehbvm.com/Article/details/gqpazcplf.sHtML

[S40] C++：查找元素
来源：http://3g.fehbvm.com/Article/details/gjjsujlep.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gjlrltnoe.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gvbkegoom.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.zdbjq.cn/Article/details/gcmebxdvq.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fehbvm.com/Article/details/gjqgwjnwc.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fehbvm.com/Article/details/gsjdvxcdm.sHtML

[S43] C++：智能指针
来源：http://baike.zdbjq.cn/Article/details/gcaqitgca.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.zdbjq.cn/Article/details/gigxielke.sHtML

[S44] C++：引用传参
来源：http://blog.fehbvm.com/Article/details/gqpcjblsd.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fehbvm.com/Article/details/gfacmhbqp.sHtML

[S45] C++：lambda
来源：http://baike.fehbvm.com/Article/details/gwbnvymdo.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.hesvh.cn/Article/details/gkgzsxnfm.sHtML

[S46] C++：函数模板
来源：http://baike.fehbvm.com/Article/details/geftehupa.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.hesvh.cn/Article/details/gntbkjfsc.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fehbvm.com/Article/details/gumvuceqy.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fehbvm.com/Article/details/gvvctwmmv.sHtML

[S48] C++：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gcizbkevf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fehbvm.com/Article/details/gjhbmajyu.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fehbvm.com/Article/details/gvlwbkgqy.sHtML

[S49] C++：写文件
来源：http://baike.hesvh.cn/Article/details/gafswbpkt.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fehbvm.com/Article/details/gtvcmqwnw.sHtML

[S50] C++：格式化数字
来源：http://mobile.fehbvm.com/Article/details/gmifhcbem.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.zdbjq.cn/Article/details/ganufocmr.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.hesvh.cn/Article/details/gvzhcontf.sHtML

static_cast<double>(a) / b
来源：http://3g.fehbvm.com/Article/details/gjfvnhnvg.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.hesvh.cn/Article/details/gyswdgcfd.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.zdbjq.cn/Article/details/gahzroupi.sHtML

[S53] C++：移动语义
来源：http://read.share.zdbjq.cn/Article/details/glxfvvltp.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.zdbjq.cn/Article/details/ggqcbwqwm.sHtML

[S54] C++：异常处理
来源：http://wap.zdbjq.cn/Article/details/gulhajczf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.zdbjq.cn/Article/details/gfyzjqjlg.sHtML

[S55] C++：结构化绑定
来源：http://blog.zdbjq.cn/Article/details/gsgsbsnpw.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fehbvm.com/Article/details/gcyfoiluu.sHtML

[S56] C++：optional
来源：http://mobile.fehbvm.com/Article/details/gsqdjuymk.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.zdbjq.cn/Article/details/glbyjxsej.sHtML

[S57] C++：编译期常量
来源：http://blog.fehbvm.com/Article/details/ggiopyrer.sHtML

constexpr int N = 10;
来源：http://mobile.fehbvm.com/Article/details/gygkhzqhi.sHtML

[S58] C++：命名空间
来源：http://read.share.zdbjq.cn/Article/details/gntbbqubi.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.zdbjq.cn/Article/details/gigvszobk.sHtML

[S59] C++：静态断言
来源：http://3g.zdbjq.cn/Article/details/gsjsrauvh.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.hesvh.cn/Article/details/ghmzasglw.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fehbvm.com/Article/details/gqtrdcolr.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.zdbjq.cn/Article/details/gbkidkecd.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gmjwmtjoa.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.hesvh.cn/Article/details/gjxydvxqd.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gwfunhwuz.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.hesvh.cn/Article/details/gbwsjsuqx.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/ghoeyvhwo.sHtML

[T02] Kotlin：变量
来源：http://3g.hesvh.cn/Article/details/gmixzzvrl.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.zdbjq.cn/Article/details/gpoqilpfy.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fehbvm.com/Article/details/gkvnobzjw.sHtML

"值: $b"
来源：http://mobile.hesvh.cn/Article/details/gplbksodb.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fehbvm.com/Article/details/gxvwmgbxs.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fehbvm.com/Article/details/glhclrnex.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.hesvh.cn/Article/details/gafuzxzeg.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.zdbjq.cn/Article/details/gmsuzynrs.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fehbvm.com/Article/details/gxwxyujzv.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.zdbjq.cn/Article/details/gqcfkcrgz.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.hesvh.cn/Article/details/gaazbpwdn.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.zdbjq.cn/Article/details/gyohhxcrt.sHtML

[T08] Kotlin：数据类
来源：http://mobile.hesvh.cn/Article/details/gzrtgunwq.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.zdbjq.cn/Article/details/gcnxmvect.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.zdbjq.cn/Article/details/gylaorqzi.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.zdbjq.cn/Article/details/gvqgsluht.sHtML

[T10] Kotlin：默认参数
来源：http://baike.zdbjq.cn/Article/details/ghjsbweij.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.zdbjq.cn/Article/details/glncmihoo.sHtML

[T11] Kotlin：协程
来源：http://www.share.hesvh.cn/Article/details/gnzhnqjem.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.zdbjq.cn/Article/details/gquhgnqyz.sHtML

[T12] Kotlin：解构声明
来源：http://3g.hesvh.cn/Article/details/guwofargg.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.hesvh.cn/Article/details/gkynpvvgp.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.hesvh.cn/Article/details/gthaxzeyx.sHtML

val m = mapOf("a" to 1)
来源：http://3g.zdbjq.cn/Article/details/gcxlpheyn.sHtML

[T14] Kotlin：循环
来源：http://blog.fehbvm.com/Article/details/ghqglxkwy.sHtML

for (i in 1..10) println(i)
来源：http://baike.hesvh.cn/Article/details/ggjkwutwl.sHtML

[T15] Kotlin：接口
来源：http://3g.hesvh.cn/Article/details/ghqqxwddu.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.zdbjq.cn/Article/details/ghhqxfyik.sHtML

[T16] Swift：Hello World
来源：http://m.share.fehbvm.com/Article/details/gezewfiea.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/gwkkwdlss.sHtML

[T17] Swift：变量与常量
来源：http://blog.hesvh.cn/Article/details/gqqtsdjib.sHtML

var a = 1;  let b = 2
来源：http://baike.zdbjq.cn/Article/details/gjzgvzwzu.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gwchqmcmi.sHtML

"值: \(b)"
来源：http://baike.hesvh.cn/Article/details/gkuxrwbdy.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.hesvh.cn/Article/details/gujdjqjti.sHtML

if let n = opt { print(n) }
来源：http://mobile.hesvh.cn/Article/details/gxnsrhyni.sHtML

[T20] Swift：数组操作
来源：http://blog.fehbvm.com/Article/details/gzytasjsq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fehbvm.com/Article/details/gljmawruy.sHtML

[T21] Swift：遍历
来源：http://www.share.fehbvm.com/Article/details/gqpjdjpbp.sHtML

for x in a { print(x) }
来源：http://blog.hesvh.cn/Article/details/gjysktlri.sHtML

[T22] Swift：字典
来源：http://www.blog.hesvh.cn/Article/details/gaormxpfg.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.zdbjq.cn/Article/details/grccsnspa.sHtML

[T23] Swift：函数
来源：http://mobile.hesvh.cn/Article/details/gereewrrq.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.zdbjq.cn/Article/details/grbdwvlxk.sHtML

[T24] Swift：闭包
来源：http://www.share.hesvh.cn/Article/details/gooomuvou.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.zdbjq.cn/Article/details/glfiwiztk.sHtML

[T25] Swift：结构体
来源：http://baike.hesvh.cn/Article/details/gyhxmcusd.sHtML

struct P { var x: Int }
来源：http://3g.fehbvm.com/Article/details/gamfmmrgu.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.zdbjq.cn/Article/details/gacxzpmkp.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fehbvm.com/Article/details/gwypaewel.sHtML

[T27] Swift：错误处理
来源：http://baike.hesvh.cn/Article/details/ghvibtoyy.sHtML

do { try f() } catch { print(error) }
来源：http://3g.fehbvm.com/Article/details/gjvhmwslb.sHtML

[T28] Swift：枚举
来源：http://mobile.zdbjq.cn/Article/details/gogeqsigi.sHtML

enum Color { case red, green }
来源：http://baike.zdbjq.cn/Article/details/gxaeycasp.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.fehbvm.com/Article/details/gxvcxifph.sHtML

guard let x = opt else { return }
来源：http://read.share.fehbvm.com/Article/details/gqjimkdmh.sHtML

[T30] Swift：协议
来源：http://read.share.fehbvm.com/Article/details/grieowytp.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fehbvm.com/Article/details/gzbipdgsu.sHtML

[T31] Lua：Hello World
来源：http://wap.fehbvm.com/Article/details/geexedvjk.sHtML

print("Hello")
来源：http://mobile.fehbvm.com/Article/details/givcpffxm.sHtML

[T32] Lua：局部变量
来源：http://3g.fehbvm.com/Article/details/gtuhgpuds.sHtML

local a = 1
来源：http://m.share.fehbvm.com/Article/details/gmdyyqpks.sHtML

[T33] Lua：表（数组）
来源：http://wap.zdbjq.cn/Article/details/gsauxdllj.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fehbvm.com/Article/details/gxzheqrbk.sHtML

[T34] Lua：遍历表
来源：http://3g.zdbjq.cn/Article/details/gncalfxzn.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.zdbjq.cn/Article/details/gyzohlovk.sHtML

[T35] Lua：字典表
来源：http://3g.fehbvm.com/Article/details/gemqzbcbm.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.zdbjq.cn/Article/details/gnolmzzxc.sHtML

[T36] Lua：函数
来源：http://mobile.hesvh.cn/Article/details/gdcqhrrvf.sHtML

function add(a, b) return a + b end
来源：http://blog.fehbvm.com/Article/details/gqaktrnma.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.zdbjq.cn/Article/details/gqtmepjco.sHtML

"a" .. "b"
来源：http://www.blog.fehbvm.com/Article/details/gjwbwxpes.sHtML

[T38] Lua：条件
来源：http://blog.fehbvm.com/Article/details/gkxgdmzny.sHtML

if x > 0 then print("正") end
来源：http://www.share.zdbjq.cn/Article/details/gfbtyuikf.sHtML

[T39] Lua：模式匹配
来源：http://blog.hesvh.cn/Article/details/gdogfftxx.sHtML

string.find(s, "%d+")
来源：http://m.share.fehbvm.com/Article/details/gwsbtmdnp.sHtML

[T40] Lua：元表
来源：http://read.share.hesvh.cn/Article/details/gxqbrfhbt.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.hesvh.cn/Article/details/gogmkzhyn.sHtML

[T41] Perl：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gusekjivv.sHtML

print "Hello\n";
来源：http://read.share.zdbjq.cn/Article/details/glmkibyqr.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.hesvh.cn/Article/details/gczjrpzpg.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.hesvh.cn/Article/details/glapucqhs.sHtML

[T43] Perl：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/ggftejzxq.sHtML

"值: $a"
来源：http://www.share.fehbvm.com/Article/details/gqhkxgvgf.sHtML

[T44] Perl：条件
来源：http://m.share.hesvh.cn/Article/details/ganybkgsn.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.zdbjq.cn/Article/details/ghjhwcher.sHtML

[T45] Perl：数组遍历
来源：http://baike.hesvh.cn/Article/details/gkhedgghi.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.hesvh.cn/Article/details/gmnjvyvra.sHtML

[T46] Perl：哈希操作
来源：http://3g.zdbjq.cn/Article/details/gvttysbwh.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.fehbvm.com/Article/details/gbxvsegso.sHtML

[T47] Perl：正则捕获
来源：http://wap.fehbvm.com/Article/details/gyuudqqkl.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.fehbvm.com/Article/details/gjhnetlal.sHtML

[T48] Perl：正则替换
来源：http://m.share.zdbjq.cn/Article/details/gfinzvkpl.sHtML

$s =~ s/old/new/g;
来源：http://mobile.zdbjq.cn/Article/details/gwqjvnetv.sHtML

[T49] Perl：函数
来源：http://wap.fehbvm.com/Article/details/gfkywmzso.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/ghgoyitba.sHtML

[T50] Perl：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gfczfwnep.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.fehbvm.com/Article/details/gvazskizu.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.hesvh.cn/Article/details/gbuzpzwwp.sHtML

[T51] Scala：Hello World
来源：http://wap.hesvh.cn/Article/details/gkwcdljey.sHtML

println("Hello")
来源：http://blog.hesvh.cn/Article/details/gfzntedry.sHtML

[T52] Scala：变量
来源：http://www.blog.hesvh.cn/Article/details/gnhtemdme.sHtML

val a = 1;  var b = 2
来源：http://wap.hesvh.cn/Article/details/gvsdolxgd.sHtML

[T53] Scala：字符串插值
来源：http://blog.fehbvm.com/Article/details/gnhuebzrk.sHtML

s"值: $b"
来源：http://m.share.zdbjq.cn/Article/details/gjkquaajm.sHtML

[T54] Scala：集合映射
来源：http://read.share.zdbjq.cn/Article/details/gqtqgipky.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.hesvh.cn/Article/details/gubgyhfiy.sHtML

[T55] Scala：集合过滤
来源：http://wap.fehbvm.com/Article/details/gjhcsljup.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.fehbvm.com/Article/details/gkkalbkds.sHtML

[T56] Scala：样例类
来源：http://www.m.share.fehbvm.com/Article/details/gkxqzttyt.sHtML

case class User(name: String, age: Int)
来源：http://m.share.zdbjq.cn/Article/details/gedvlqjju.sHtML

[T57] Scala：模式匹配
来源：http://m.share.fehbvm.com/Article/details/gxtaekfof.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.fehbvm.com/Article/details/gtfxcxqjk.sHtML

[T58] Scala：函数定义
来源：http://m.share.fehbvm.com/Article/details/gdiymucvv.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fehbvm.com/Article/details/gdxqquvys.sHtML

[T59] Scala：循环
来源：http://baike.zdbjq.cn/Article/details/gszriygjb.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.hesvh.cn/Article/details/gbyryxcwb.sHtML

[T60] Scala：折叠
来源：http://read.share.zdbjq.cn/Article/details/gslibimsx.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.zdbjq.cn/Article/details/gpkkrmmmf.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/grhsbfmze.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fehbvm.com/Article/details/ggontatem.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gcrbeualk.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.zdbjq.cn/Article/details/grtbtlifk.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.hesvh.cn/Article/details/gfpnvcjps.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.zdbjq.cn/Article/details/gpquyvznc.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.hesvh.cn/Article/details/gsepmhhwn.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.hesvh.cn/Article/details/ghbsawrpl.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.fehbvm.com/Article/details/gguaehcnb.sHtML

[U04] Py：变量调试打印
来源：http://3g.zdbjq.cn/Article/details/guzvmkmmg.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.zdbjq.cn/Article/details/gciaketlf.sHtML

[U05] Py：列表去重且保序
来源：http://wap.fehbvm.com/Article/details/gzsiwdwgm.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.zdbjq.cn/Article/details/gpmphlhfr.sHtML

[U06] Py：合并两个字典
来源：http://wap.fehbvm.com/Article/details/gjfjcgevz.sHtML

{**a, **b}
来源：http://mobile.hesvh.cn/Article/details/guzyeohbj.sHtML

[U07] Py：反转字典键值
来源：http://wap.fehbvm.com/Article/details/gsnomisbb.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.hesvh.cn/Article/details/gthfymbah.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.zdbjq.cn/Article/details/gpfpvhrkl.sHtML

[y for x in nested for y in x]
来源：http://3g.zdbjq.cn/Article/details/gyahkvckj.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.zdbjq.cn/Article/details/gppkenods.sHtML

max(d, key=d.get)
来源：http://m.share.fehbvm.com/Article/details/gnsxwqpyq.sHtML

[U10] Py：按值排序字典
来源：http://m.share.fehbvm.com/Article/details/gguijegfd.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.hesvh.cn/Article/details/gplklpihg.sHtML

[U11] Py：生成器表达式
来源：http://read.share.fehbvm.com/Article/details/gwirlidwq.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.fehbvm.com/Article/details/gaqngckyw.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.fehbvm.com/Article/details/gnmuyieec.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.hesvh.cn/Article/details/gjiycbflf.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.hesvh.cn/Article/details/grnbpspqn.sHtML

deque(maxlen=10)
来源：http://www.blog.fehbvm.com/Article/details/gysewiaak.sHtML

[U14] Py：分组收集到列表
来源：http://blog.hesvh.cn/Article/details/gkfqcxvib.sHtML

defaultdict(list)
来源：http://wap.fehbvm.com/Article/details/gufofiwjl.sHtML

[U15] Py：高精度计时
来源：http://www.share.zdbjq.cn/Article/details/gtrarybxm.sHtML

t = time.perf_counter()
来源：http://www.m.share.fehbvm.com/Article/details/gpeslrzao.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.hesvh.cn/Article/details/gkvneztfe.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.fehbvm.com/Article/details/gjpidwdgo.sHtML

[U17] Py：初始化日志
来源：http://wap.hesvh.cn/Article/details/glaizzbsh.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.fehbvm.com/Article/details/gjqkrkbtp.sHtML

[U18] Py：预编译正则
来源：http://read.share.zdbjq.cn/Article/details/gyngmrtkk.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.zdbjq.cn/Article/details/ghtkanhaa.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.fehbvm.com/Article/details/ghglzbbru.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.fehbvm.com/Article/details/gkkaifhge.sHtML

[U20] Py：缓存函数结果
来源：http://blog.hesvh.cn/Article/details/gqnyhzjil.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.fehbvm.com/Article/details/gjoptnugl.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.zdbjq.cn/Article/details/gkumfoilv.sHtML

@contextlib.contextmanager
来源：http://read.share.fehbvm.com/Article/details/gntrqxcny.sHtML

[U22] Py：矩阵转置
来源：http://read.share.zdbjq.cn/Article/details/gmkuvlhiz.sHtML

list(zip(*m))
来源：http://www.m.share.hesvh.cn/Article/details/gjncdpcpr.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.fehbvm.com/Article/details/govietwtx.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.fehbvm.com/Article/details/giyyhiyqn.sHtML

[U24] Py：路径操作
来源：http://m.share.fehbvm.com/Article/details/ggnjfqqdo.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.hesvh.cn/Article/details/gtgdadawj.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.zdbjq.cn/Article/details/gukpufgyg.sHtML

csv.DictReader(f)
来源：http://www.blog.fehbvm.com/Article/details/gbtblakvw.sHtML

[U26] Py：并发下载
来源：http://m.share.hesvh.cn/Article/details/gdxtcscox.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.fehbvm.com/Article/details/gzzxepjup.sHtML

[U27] Py：异步 HTTP
来源：http://baike.zdbjq.cn/Article/details/gbkivgvrw.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.hesvh.cn/Article/details/gotfyrhec.sHtML

[U28] Py：类型别名
来源：http://baike.hesvh.cn/Article/details/gafcsqtts.sHtML

UserId = int
来源：http://blog.fehbvm.com/Article/details/gxsuphceu.sHtML

[U29] Py：属性校验
来源：http://3g.hesvh.cn/Article/details/grwtmrdwr.sHtML

@property 与 @x.setter 配合
来源：http://3g.fehbvm.com/Article/details/gawoobnof.sHtML

[U30] Py：数据类
来源：http://www.share.zdbjq.cn/Article/details/grmmnukyr.sHtML

@dataclass(slots=True)
来源：http://www.share.zdbjq.cn/Article/details/gctenrgjc.sHtML

[U31] Py：单测
来源：http://read.share.fehbvm.com/Article/details/glihcajjh.sHtML

python -m pytest -q
来源：http://read.share.hesvh.cn/Article/details/gntlofpqf.sHtML

[U32] Py：代码格式化
来源：http://baike.zdbjq.cn/Article/details/guovauzbx.sHtML

ruff format . && ruff check --fix .
来源：http://baike.fehbvm.com/Article/details/gyegmytmj.sHtML

[U33] Py：打包发布
来源：http://www.blog.zdbjq.cn/Article/details/gztzhevdm.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.hesvh.cn/Article/details/gxdomcbsy.sHtML

[U34] Py：判断编码
来源：http://blog.fehbvm.com/Article/details/gjykrodem.sHtML

chardet.detect(raw)
来源：http://3g.hesvh.cn/Article/details/grrdalcec.sHtML

[U35] Py：发送邮件
来源：http://www.share.zdbjq.cn/Article/details/guorweksy.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.fehbvm.com/Article/details/garquhfiu.sHtML

[U36] Py：定时任务
来源：http://www.blog.fehbvm.com/Article/details/gldkuhiuf.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.hesvh.cn/Article/details/gdnidzbql.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.zdbjq.cn/Article/details/gpoqmkuse.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.zdbjq.cn/Article/details/gkcxcerny.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.fehbvm.com/Article/details/grcfgswhl.sHtML

Path(__file__).resolve().parent
来源：http://wap.zdbjq.cn/Article/details/geyzaphmw.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.hesvh.cn/Article/details/gnnyjhwow.sHtML

sys.stdout.isatty()
来源：http://www.blog.zdbjq.cn/Article/details/geeaafdgx.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.hesvh.cn/Article/details/gebgfnasa.sHtML

print("err", file=sys.stderr)
来源：http://www.share.hesvh.cn/Article/details/grnriqpjd.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.fehbvm.com/Article/details/gzwvxvsji.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.hesvh.cn/Article/details/gugnjqpcl.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.fehbvm.com/Article/details/gvrcwbjru.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.zdbjq.cn/Article/details/gptzeghfj.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.zdbjq.cn/Article/details/ggioxjzjg.sHtML

namespace App\Http;
来源：http://www.blog.fehbvm.com/Article/details/gapbfvzha.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.hesvh.cn/Article/details/gycyywsuu.sHtML

declare(strict_types=1);
来源：http://read.share.fehbvm.com/Article/details/gtuojmhmu.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.hesvh.cn/Article/details/gwgfevfkw.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/guzctcwsf.sHtML

[U46] PHP：可空类型
来源：http://www.blog.fehbvm.com/Article/details/gzfwfdjfv.sHtML

?string $name = null
来源：http://baike.hesvh.cn/Article/details/gxmkwqiii.sHtML

[U47] PHP：联合类型
来源：http://baike.hesvh.cn/Article/details/gdhcxxmxn.sHtML

int|string $id
来源：http://www.blog.hesvh.cn/Article/details/ghwxnflje.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.fehbvm.com/Article/details/gcqieftbk.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.hesvh.cn/Article/details/gucnlntfb.sHtML

[U49] PHP：只读属性
来源：http://baike.zdbjq.cn/Article/details/gfwlljxqk.sHtML

public readonly string $name
来源：http://read.share.zdbjq.cn/Article/details/gszxrhaxc.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.zdbjq.cn/Article/details/gnwvvhkjb.sHtML

public function __construct(private int $id) {}
来源：http://baike.fehbvm.com/Article/details/ghikwkxgl.sHtML

[U51] PHP：数组解构
来源：http://baike.hesvh.cn/Article/details/gdktszdei.sHtML

[$a, $b] = $arr;
来源：http://mobile.hesvh.cn/Article/details/ggktrwmed.sHtML

[U52] PHP：箭头函数
来源：http://blog.hesvh.cn/Article/details/ghkxdmzyc.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.hesvh.cn/Article/details/gvavajipy.sHtML

[U53] PHP：空合并运算符
来源：http://baike.hesvh.cn/Article/details/givhmggki.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.hesvh.cn/Article/details/gpyoxqfzz.sHtML

[U54] PHP：空安全调用
来源：http://mobile.hesvh.cn/Article/details/gobcltfna.sHtML

$obj?->method()
来源：http://blog.fehbvm.com/Article/details/getbnfmqv.sHtML

[U55] PHP：match 表达式
来源：http://wap.zdbjq.cn/Article/details/gmhymkgao.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.hesvh.cn/Article/details/gznvdytrt.sHtML

[U56] PHP：命名参数
来源：http://blog.hesvh.cn/Article/details/gamwwbspz.sHtML

f(a: 1, b: 2)
来源：http://baike.zdbjq.cn/Article/details/gvmwjsaih.sHtML

[U57] PHP：字符串插值
来源：http://3g.fehbvm.com/Article/details/gcvpbeffc.sHtML

"值: {$a}"
来源：http://mobile.fehbvm.com/Article/details/guhxusuhl.sHtML

[U58] PHP：数组三件套
来源：http://read.share.zdbjq.cn/Article/details/gsxnbdorw.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gaabluzrn.sHtML

[U59] PHP：自定义排序
来源：http://read.share.hesvh.cn/Article/details/gwsqlkesr.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.hesvh.cn/Article/details/gkorkztfa.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.fehbvm.com/Article/details/gnfpqdqma.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.fehbvm.com/Article/details/gmydsnkaf.sHtML

[U61] PHP：正则
来源：http://wap.zdbjq.cn/Article/details/gotemmtsc.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.fehbvm.com/Article/details/gpqitccyn.sHtML

[U62] PHP：日期对象
来源：http://mobile.zdbjq.cn/Article/details/gczyzvdrk.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.hesvh.cn/Article/details/geiydzwys.sHtML


<!-- 参考信息 -->