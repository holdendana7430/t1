代发 wailian999

[S39] C++：自定义比较器排序
来源：http://3g.zdbjq.cn/Article/details/gifvpcphz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.hesvh.cn/Article/details/geshosmqt.sHtML

[S40] C++：查找元素
来源：http://wap.hesvh.cn/Article/details/gljnuukbx.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fehbvm.com/Article/details/guayntsls.sHtML

[S41] C++：类与构造函数
来源：http://m.share.hesvh.cn/Article/details/gbqacegqt.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.zdbjq.cn/Article/details/gofetxusl.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.hesvh.cn/Article/details/gifwyitpi.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.zdbjq.cn/Article/details/guykhnhdi.sHtML

[S43] C++：智能指针
来源：http://m.share.zdbjq.cn/Article/details/gkfkbkqwb.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fehbvm.com/Article/details/gxwfdxpyz.sHtML

[S44] C++：引用传参
来源：http://read.share.hesvh.cn/Article/details/gsrzhughh.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.zdbjq.cn/Article/details/gtpenvrte.sHtML

[S45] C++：lambda
来源：http://mobile.fehbvm.com/Article/details/gdfnssjsv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fehbvm.com/Article/details/gfpycxwcl.sHtML

[S46] C++：函数模板
来源：http://m.share.fehbvm.com/Article/details/grkuyvxoe.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.zdbjq.cn/Article/details/gtvqwhllc.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.zdbjq.cn/Article/details/gsxszhqry.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.hesvh.cn/Article/details/gnwnixhtv.sHtML

[S48] C++：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gabbwrhjc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.zdbjq.cn/Article/details/grzpklcyv.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.hesvh.cn/Article/details/gwwblptii.sHtML

[S49] C++：写文件
来源：http://www.m.share.fehbvm.com/Article/details/guqgrzfpt.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.zdbjq.cn/Article/details/grpfoblvb.sHtML

[S50] C++：格式化数字
来源：http://mobile.hesvh.cn/Article/details/gztgnhepk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fehbvm.com/Article/details/gzqcsyldl.sHtML

[S51] C++：显式类型转换
来源：http://wap.fehbvm.com/Article/details/gpdalnavb.sHtML

static_cast<double>(a) / b
来源：http://mobile.zdbjq.cn/Article/details/gusnnvohs.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fehbvm.com/Article/details/gnjzvhvci.sHtML

int size() const noexcept { return n_; }
来源：http://baike.hesvh.cn/Article/details/ghcoryoxj.sHtML

[S53] C++：移动语义
来源：http://3g.fehbvm.com/Article/details/gowzdjxob.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.zdbjq.cn/Article/details/gmnklqaoe.sHtML

[S54] C++：异常处理
来源：http://mobile.hesvh.cn/Article/details/gbppvqyyp.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.zdbjq.cn/Article/details/gnwhvsxzt.sHtML

[S55] C++：结构化绑定
来源：http://www.share.hesvh.cn/Article/details/gcgknxifh.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.zdbjq.cn/Article/details/ggqbfmusu.sHtML

[S56] C++：optional
来源：http://wap.hesvh.cn/Article/details/gkrrchspi.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.hesvh.cn/Article/details/gweqdebhp.sHtML

[S57] C++：编译期常量
来源：http://m.share.hesvh.cn/Article/details/gpznrqmgn.sHtML

constexpr int N = 10;
来源：http://www.share.hesvh.cn/Article/details/gjyaxbnwk.sHtML

[S58] C++：命名空间
来源：http://wap.zdbjq.cn/Article/details/gmnomxhzo.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.hesvh.cn/Article/details/gkhrodgqt.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fehbvm.com/Article/details/gznftzmvd.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.zdbjq.cn/Article/details/gbzktsxre.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fehbvm.com/Article/details/gpjbfpoyf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.hesvh.cn/Article/details/gpyxzejky.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gkosrapfc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.hesvh.cn/Article/details/gphzjdovw.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/guuqmuzlk.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fehbvm.com/Article/details/gmnlihxgs.sHtML

println("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gzrbofkkm.sHtML

[T02] Kotlin：变量
来源：http://wap.hesvh.cn/Article/details/gtjulokwv.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fehbvm.com/Article/details/gnofvqiym.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.zdbjq.cn/Article/details/gttgpompj.sHtML

"值: $b"
来源：http://www.m.share.fehbvm.com/Article/details/gypebkfoh.sHtML

[T04] Kotlin：空安全
来源：http://read.share.zdbjq.cn/Article/details/glayzubko.sHtML

val n: String? = null;  n?.length
来源：http://wap.fehbvm.com/Article/details/gthgzihni.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fehbvm.com/Article/details/gqeuzncoh.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.zdbjq.cn/Article/details/gajfxtbri.sHtML

[T06] Kotlin：集合映射
来源：http://baike.hesvh.cn/Article/details/geflhdbqq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.hesvh.cn/Article/details/gfrwcqxfb.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.zdbjq.cn/Article/details/gcsbajkwh.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fehbvm.com/Article/details/giipivchp.sHtML

[T08] Kotlin：数据类
来源：http://mobile.hesvh.cn/Article/details/ggmtfxccs.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.zdbjq.cn/Article/details/gdecxlxmf.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fehbvm.com/Article/details/gwnavxtoo.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fehbvm.com/Article/details/gqjkywcbs.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.zdbjq.cn/Article/details/gvhqhznqt.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.hesvh.cn/Article/details/gtjqtwvjq.sHtML

[T11] Kotlin：协程
来源：http://www.share.fehbvm.com/Article/details/gtfislggp.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.zdbjq.cn/Article/details/gaucpwlsf.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fehbvm.com/Article/details/gtwfftfan.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gwdcfqsdd.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.hesvh.cn/Article/details/gzhooqvyp.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fehbvm.com/Article/details/gzgiubzdp.sHtML

[T14] Kotlin：循环
来源：http://baike.hesvh.cn/Article/details/gzcyqogyz.sHtML

for (i in 1..10) println(i)
来源：http://baike.hesvh.cn/Article/details/gdvwstztz.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.hesvh.cn/Article/details/gelsvfqmm.sHtML

interface Shape { fun area(): Double }
来源：http://3g.hesvh.cn/Article/details/glxqmjiha.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/glgztgkgx.sHtML

print("Hello")
来源：http://blog.zdbjq.cn/Article/details/gzbbigbed.sHtML

[T17] Swift：变量与常量
来源：http://blog.hesvh.cn/Article/details/gucgpskau.sHtML

var a = 1;  let b = 2
来源：http://wap.fehbvm.com/Article/details/grkkoyyln.sHtML

[T18] Swift：字符串插值
来源：http://baike.hesvh.cn/Article/details/ghztmjvfh.sHtML

"值: \(b)"
来源：http://mobile.fehbvm.com/Article/details/ghmgqpdms.sHtML

[T19] Swift：可选绑定
来源：http://baike.zdbjq.cn/Article/details/gelponihb.sHtML

if let n = opt { print(n) }
来源：http://m.share.zdbjq.cn/Article/details/gjoxosrtv.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fehbvm.com/Article/details/glfjmejni.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.zdbjq.cn/Article/details/gbsesaoio.sHtML

[T21] Swift：遍历
来源：http://wap.zdbjq.cn/Article/details/gsyrqghyn.sHtML

for x in a { print(x) }
来源：http://wap.hesvh.cn/Article/details/gyxudytte.sHtML

[T22] Swift：字典
来源：http://3g.fehbvm.com/Article/details/grsbepzzk.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.hesvh.cn/Article/details/ghlckeyel.sHtML

[T23] Swift：函数
来源：http://mobile.fehbvm.com/Article/details/glicbacoe.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.zdbjq.cn/Article/details/gkfjudyox.sHtML

[T24] Swift：闭包
来源：http://mobile.fehbvm.com/Article/details/gqdidsnns.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fehbvm.com/Article/details/gjpmrrywj.sHtML

[T25] Swift：结构体
来源：http://wap.fehbvm.com/Article/details/gpebjuknx.sHtML

struct P { var x: Int }
来源：http://blog.fehbvm.com/Article/details/gvcrwftne.sHtML

[T26] Swift：类与重写
来源：http://www.blog.zdbjq.cn/Article/details/ghwigkzkl.sHtML

class A: Base { override func f() {} }
来源：http://m.share.zdbjq.cn/Article/details/gafyxuhgs.sHtML

[T27] Swift：错误处理
来源：http://www.blog.fehbvm.com/Article/details/gwskjdtsz.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.zdbjq.cn/Article/details/ghzedbfsq.sHtML

[T28] Swift：枚举
来源：http://mobile.hesvh.cn/Article/details/gwmfqzlwi.sHtML

enum Color { case red, green }
来源：http://wap.fehbvm.com/Article/details/gutjbiwtt.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.zdbjq.cn/Article/details/gwjmomwsf.sHtML

guard let x = opt else { return }
来源：http://mobile.zdbjq.cn/Article/details/ghlntwpvu.sHtML

[T30] Swift：协议
来源：http://3g.zdbjq.cn/Article/details/gufhnozwj.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fehbvm.com/Article/details/gumeltpgg.sHtML

[T31] Lua：Hello World
来源：http://read.share.hesvh.cn/Article/details/gtqutdopb.sHtML

print("Hello")
来源：http://www.share.fehbvm.com/Article/details/gshmnhxoc.sHtML

[T32] Lua：局部变量
来源：http://wap.zdbjq.cn/Article/details/ggvgawdpx.sHtML

local a = 1
来源：http://www.blog.fehbvm.com/Article/details/gptgduajl.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fehbvm.com/Article/details/gepahppcf.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.zdbjq.cn/Article/details/gtgexygam.sHtML

[T34] Lua：遍历表
来源：http://mobile.hesvh.cn/Article/details/gvpougtex.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.zdbjq.cn/Article/details/gdptybvpb.sHtML

[T35] Lua：字典表
来源：http://blog.hesvh.cn/Article/details/guumowbuh.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gnwgavqbw.sHtML

[T36] Lua：函数
来源：http://baike.zdbjq.cn/Article/details/ghaczlxzb.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.zdbjq.cn/Article/details/gwpjuspyz.sHtML

[T37] Lua：字符串拼接
来源：http://blog.hesvh.cn/Article/details/gkdhqqbuq.sHtML

"a" .. "b"
来源：http://baike.hesvh.cn/Article/details/gvbmbozed.sHtML

[T38] Lua：条件
来源：http://www.blog.fehbvm.com/Article/details/gxuoodmtc.sHtML

if x > 0 then print("正") end
来源：http://www.blog.hesvh.cn/Article/details/gwxhtpqsj.sHtML

[T39] Lua：模式匹配
来源：http://3g.fehbvm.com/Article/details/gksctlqav.sHtML

string.find(s, "%d+")
来源：http://m.share.hesvh.cn/Article/details/gcubkpuik.sHtML

[T40] Lua：元表
来源：http://3g.fehbvm.com/Article/details/gnwqqpbrh.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.hesvh.cn/Article/details/gtbpmbusx.sHtML

[T41] Perl：Hello World
来源：http://blog.hesvh.cn/Article/details/gpxkvcavc.sHtML

print "Hello\n";
来源：http://blog.zdbjq.cn/Article/details/gcyqflcoj.sHtML

[T42] Perl：变量类型
来源：http://www.blog.zdbjq.cn/Article/details/gmcufngzo.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.hesvh.cn/Article/details/gdkjfjwky.sHtML

[T43] Perl：字符串插值
来源：http://3g.fehbvm.com/Article/details/guctztqld.sHtML

"值: $a"
来源：http://www.share.zdbjq.cn/Article/details/gywldjshz.sHtML

[T44] Perl：条件
来源：http://www.blog.fehbvm.com/Article/details/gocdpuccp.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.zdbjq.cn/Article/details/gruqtaoil.sHtML

[T45] Perl：数组遍历
来源：http://3g.zdbjq.cn/Article/details/gpqxclyad.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.fehbvm.com/Article/details/ghcemvjgv.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fehbvm.com/Article/details/gpkedloep.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.fehbvm.com/Article/details/gdmtutpij.sHtML

[T47] Perl：正则捕获
来源：http://baike.fehbvm.com/Article/details/gyfehkjrs.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.zdbjq.cn/Article/details/guwvqazml.sHtML

[T48] Perl：正则替换
来源：http://wap.zdbjq.cn/Article/details/gigtijeao.sHtML

$s =~ s/old/new/g;
来源：http://m.share.hesvh.cn/Article/details/glmhxmyru.sHtML

[T49] Perl：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gwoccxbds.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/ghgmgjrrs.sHtML

[T50] Perl：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gakmreotq.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.zdbjq.cn/Article/details/gjnlsufgk.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.fehbvm.com/Article/details/gvsmbnbiu.sHtML

[T51] Scala：Hello World
来源：http://mobile.hesvh.cn/Article/details/gekxxrbbl.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/ginorcgsv.sHtML

[T52] Scala：变量
来源：http://m.share.fehbvm.com/Article/details/gapjsbxjb.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gctxxwdrn.sHtML

[T53] Scala：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gswtkkzmd.sHtML

s"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/guvpaosfa.sHtML

[T54] Scala：集合映射
来源：http://baike.zdbjq.cn/Article/details/ggmhfswew.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.zdbjq.cn/Article/details/gatyhuygk.sHtML

[T55] Scala：集合过滤
来源：http://baike.hesvh.cn/Article/details/gtotkmvmg.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.hesvh.cn/Article/details/grjvshrwi.sHtML

[T56] Scala：样例类
来源：http://baike.fehbvm.com/Article/details/gwysmxjzj.sHtML

case class User(name: String, age: Int)
来源：http://mobile.hesvh.cn/Article/details/gndvkvgfa.sHtML

[T57] Scala：模式匹配
来源：http://m.share.hesvh.cn/Article/details/gloaylgri.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.fehbvm.com/Article/details/gxgtyulhy.sHtML

[T58] Scala：函数定义
来源：http://www.share.fehbvm.com/Article/details/gqaytrwps.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.fehbvm.com/Article/details/girbivpxb.sHtML

[T59] Scala：循环
来源：http://baike.hesvh.cn/Article/details/gdxjhneie.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.hesvh.cn/Article/details/gkamdsocc.sHtML

[T60] Scala：折叠
来源：http://read.share.hesvh.cn/Article/details/golfkdgqo.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.hesvh.cn/Article/details/gwmajlpjv.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gojxgouqc.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.zdbjq.cn/Article/details/gtjjeqfkq.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gbktixuen.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.fehbvm.com/Article/details/gtsbzsodh.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.hesvh.cn/Article/details/gzgtcwyke.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.fehbvm.com/Article/details/gwvfccjnc.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.zdbjq.cn/Article/details/gfaogtgbo.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.fehbvm.com/Article/details/gdwmkfcxi.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.hesvh.cn/Article/details/gtsmqcyml.sHtML

[U04] Py：变量调试打印
来源：http://m.share.zdbjq.cn/Article/details/gldzycdjm.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.fehbvm.com/Article/details/glwhghweu.sHtML

[U05] Py：列表去重且保序
来源：http://baike.zdbjq.cn/Article/details/gjdwuzaip.sHtML

list(dict.fromkeys(arr))
来源：http://baike.hesvh.cn/Article/details/ghchcqyyk.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.hesvh.cn/Article/details/gqdmzzrwr.sHtML

{**a, **b}
来源：http://wap.hesvh.cn/Article/details/gsttcfczr.sHtML

[U07] Py：反转字典键值
来源：http://wap.zdbjq.cn/Article/details/giqhewvqb.sHtML

{v: k for k, v in d.items()}
来源：http://wap.fehbvm.com/Article/details/gqyiullym.sHtML

[U08] Py：展平二维列表
来源：http://www.share.fehbvm.com/Article/details/gkvgzhhyj.sHtML

[y for x in nested for y in x]
来源：http://blog.hesvh.cn/Article/details/gklvtpaob.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.fehbvm.com/Article/details/grjwlhsff.sHtML

max(d, key=d.get)
来源：http://read.share.hesvh.cn/Article/details/geutzbpzr.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.hesvh.cn/Article/details/gtqvuxxbx.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.zdbjq.cn/Article/details/gcmpjcdar.sHtML

[U11] Py：生成器表达式
来源：http://mobile.fehbvm.com/Article/details/gyyvjpaga.sHtML

(x * 2 for x in arr)
来源：http://m.share.hesvh.cn/Article/details/gvhllffnp.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.zdbjq.cn/Article/details/gwjstdwbu.sHtML

Counter(arr).most_common(3)
来源：http://blog.hesvh.cn/Article/details/gbkjxgtdn.sHtML

[U13] Py：固定长度队列
来源：http://m.share.fehbvm.com/Article/details/gzkbzicsm.sHtML

deque(maxlen=10)
来源：http://mobile.zdbjq.cn/Article/details/gssmenrdf.sHtML

[U14] Py：分组收集到列表
来源：http://wap.hesvh.cn/Article/details/gdpcjzpbg.sHtML

defaultdict(list)
来源：http://blog.hesvh.cn/Article/details/ggagylevx.sHtML

[U15] Py：高精度计时
来源：http://mobile.zdbjq.cn/Article/details/gufqfxzwg.sHtML

t = time.perf_counter()
来源：http://read.share.fehbvm.com/Article/details/gvzejuxmu.sHtML

[U16] Py：命令行参数解析
来源：http://baike.zdbjq.cn/Article/details/gcsezfqvb.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.zdbjq.cn/Article/details/gzhkbokof.sHtML

[U17] Py：初始化日志
来源：http://www.share.fehbvm.com/Article/details/gowuwmlgu.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.zdbjq.cn/Article/details/gjnwbaaro.sHtML

[U18] Py：预编译正则
来源：http://wap.zdbjq.cn/Article/details/gwgkeebye.sHtML

pat = re.compile(r"\d+")
来源：http://blog.fehbvm.com/Article/details/gmczirzgt.sHtML

[U19] Py：正则替换带回调
来源：http://wap.zdbjq.cn/Article/details/gqlvjlhti.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.fehbvm.com/Article/details/gfztxkzyl.sHtML

[U20] Py：缓存函数结果
来源：http://3g.hesvh.cn/Article/details/gexdniwgt.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.hesvh.cn/Article/details/gloqmeqaz.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.fehbvm.com/Article/details/gxpoxpvcx.sHtML

@contextlib.contextmanager
来源：http://www.share.fehbvm.com/Article/details/gumtlnzbb.sHtML

[U22] Py：矩阵转置
来源：http://baike.hesvh.cn/Article/details/gwkvtzedm.sHtML

list(zip(*m))
来源：http://blog.zdbjq.cn/Article/details/glxghhazr.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.fehbvm.com/Article/details/gttgzvwzx.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.zdbjq.cn/Article/details/gffyvghqc.sHtML

[U24] Py：路径操作
来源：http://3g.fehbvm.com/Article/details/grhubdvuk.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.zdbjq.cn/Article/details/ghyrvwjxx.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.fehbvm.com/Article/details/gfyaopkzc.sHtML

csv.DictReader(f)
来源：http://www.blog.zdbjq.cn/Article/details/glijpianf.sHtML

[U26] Py：并发下载
来源：http://blog.zdbjq.cn/Article/details/gmftivywz.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.hesvh.cn/Article/details/gojhqkmdp.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.hesvh.cn/Article/details/gdtshlglf.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.fehbvm.com/Article/details/gkecwskng.sHtML

[U28] Py：类型别名
来源：http://wap.zdbjq.cn/Article/details/gjajgdimi.sHtML

UserId = int
来源：http://mobile.hesvh.cn/Article/details/gwxtwqhbk.sHtML

[U29] Py：属性校验
来源：http://mobile.fehbvm.com/Article/details/gxwldmtho.sHtML

@property 与 @x.setter 配合
来源：http://mobile.hesvh.cn/Article/details/gmyduoqeo.sHtML

[U30] Py：数据类
来源：http://read.share.zdbjq.cn/Article/details/guswvnihp.sHtML

@dataclass(slots=True)
来源：http://www.share.fehbvm.com/Article/details/gbhwyhddm.sHtML

[U31] Py：单测
来源：http://www.m.share.hesvh.cn/Article/details/gxzzjqnmw.sHtML

python -m pytest -q
来源：http://www.m.share.fehbvm.com/Article/details/gfvspgvnt.sHtML

[U32] Py：代码格式化
来源：http://www.blog.zdbjq.cn/Article/details/ggdzphhpl.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.hesvh.cn/Article/details/gcvcksznf.sHtML

[U33] Py：打包发布
来源：http://baike.hesvh.cn/Article/details/gjxroejsu.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.fehbvm.com/Article/details/gnorybkgp.sHtML

[U34] Py：判断编码
来源：http://mobile.zdbjq.cn/Article/details/gkelsnsie.sHtML

chardet.detect(raw)
来源：http://3g.hesvh.cn/Article/details/gbzoqyjqd.sHtML

[U35] Py：发送邮件
来源：http://blog.zdbjq.cn/Article/details/gfvqmvznk.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.hesvh.cn/Article/details/glsujvfla.sHtML

[U36] Py：定时任务
来源：http://blog.zdbjq.cn/Article/details/gmvjxmoyf.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.zdbjq.cn/Article/details/ggcyawmwm.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.fehbvm.com/Article/details/gpdnuhlyq.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.fehbvm.com/Article/details/gikmjflmw.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.zdbjq.cn/Article/details/gztlgdtwc.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.zdbjq.cn/Article/details/gdplbnfds.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.hesvh.cn/Article/details/gqkxmafls.sHtML

sys.stdout.isatty()
来源：http://blog.zdbjq.cn/Article/details/gubvxwwzd.sHtML

[U40] Py：打印到标准错误
来源：http://baike.zdbjq.cn/Article/details/gvfortecu.sHtML

print("err", file=sys.stderr)
来源：http://read.share.fehbvm.com/Article/details/gajuyvfhj.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.zdbjq.cn/Article/details/gowdxdfdk.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.fehbvm.com/Article/details/gdsdcwrke.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.zdbjq.cn/Article/details/geeutilnb.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.fehbvm.com/Article/details/gpkxagadz.sHtML

[U43] PHP：声明命名空间
来源：http://3g.hesvh.cn/Article/details/gcgkbikoi.sHtML

namespace App\Http;
来源：http://www.blog.hesvh.cn/Article/details/gudoczuhp.sHtML

[U44] PHP：开启严格类型
来源：http://blog.hesvh.cn/Article/details/gqluevpce.sHtML

declare(strict_types=1);
来源：http://blog.fehbvm.com/Article/details/gvuhshslo.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.hesvh.cn/Article/details/gtalxinax.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/ghgkhnjjp.sHtML

[U46] PHP：可空类型
来源：http://baike.hesvh.cn/Article/details/gilchzljb.sHtML

?string $name = null
来源：http://blog.zdbjq.cn/Article/details/gyjoftnmv.sHtML

[U47] PHP：联合类型
来源：http://3g.zdbjq.cn/Article/details/gorooxsok.sHtML

int|string $id
来源：http://www.share.fehbvm.com/Article/details/gkdyfuzak.sHtML

[U48] PHP：纯枚举
来源：http://blog.fehbvm.com/Article/details/glapbwcgv.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.hesvh.cn/Article/details/gysxuapey.sHtML

[U49] PHP：只读属性
来源：http://www.share.zdbjq.cn/Article/details/glyxnznup.sHtML

public readonly string $name
来源：http://read.share.fehbvm.com/Article/details/gpohodbjn.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.zdbjq.cn/Article/details/gswvaxgzl.sHtML

public function __construct(private int $id) {}
来源：http://read.share.hesvh.cn/Article/details/gogtriphn.sHtML

[U51] PHP：数组解构
来源：http://read.share.hesvh.cn/Article/details/gkzjmaxuk.sHtML

[$a, $b] = $arr;
来源：http://www.share.hesvh.cn/Article/details/gpmwtzqei.sHtML

[U52] PHP：箭头函数
来源：http://baike.hesvh.cn/Article/details/geqneikqo.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.hesvh.cn/Article/details/gkluwazcn.sHtML

[U53] PHP：空合并运算符
来源：http://blog.hesvh.cn/Article/details/glzwwhokh.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.hesvh.cn/Article/details/gfzwfifxf.sHtML

[U54] PHP：空安全调用
来源：http://wap.zdbjq.cn/Article/details/ghvsalceq.sHtML

$obj?->method()
来源：http://baike.fehbvm.com/Article/details/gusnztvvt.sHtML

[U55] PHP：match 表达式
来源：http://www.share.zdbjq.cn/Article/details/gmzwzmbek.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.zdbjq.cn/Article/details/gvfjrdqin.sHtML

[U56] PHP：命名参数
来源：http://mobile.zdbjq.cn/Article/details/gakeqkinz.sHtML

f(a: 1, b: 2)
来源：http://mobile.hesvh.cn/Article/details/gogyrxgpa.sHtML

[U57] PHP：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gnbtlnzqs.sHtML

"值: {$a}"
来源：http://mobile.zdbjq.cn/Article/details/gtijehmjy.sHtML

[U58] PHP：数组三件套
来源：http://read.share.hesvh.cn/Article/details/gjlgwoogv.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.hesvh.cn/Article/details/gvbmzmlae.sHtML

[U59] PHP：自定义排序
来源：http://read.share.fehbvm.com/Article/details/gjxgygqxw.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gbcaiqypi.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.zdbjq.cn/Article/details/gglptgpxt.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.zdbjq.cn/Article/details/ggawjfpdk.sHtML

[U61] PHP：正则
来源：http://3g.zdbjq.cn/Article/details/ggjpdbqle.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gtjzeutzx.sHtML

[U62] PHP：日期对象
来源：http://3g.fehbvm.com/Article/details/gjyfiiulk.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.hesvh.cn/Article/details/gutrsknce.sHtML

[U63] PHP：文件读写
来源：http://baike.fehbvm.com/Article/details/gnaeioxno.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.zdbjq.cn/Article/details/gcgghetjy.sHtML

[U64] PHP：目录遍历
来源：http://www.share.zdbjq.cn/Article/details/gkryfluno.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.hesvh.cn/Article/details/gwvfrgcum.sHtML


<!-- 参考信息 -->