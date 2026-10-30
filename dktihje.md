代发 wailian999

[S37] C++：set
来源：http://blog.zdbjq.cn/Article/details/gouforezi.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.zdbjq.cn/Article/details/guhyhkmpf.sHtML

[S38] C++：排序
来源：http://baike.fehbvm.com/Article/details/grhimpvva.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/gmyuxfgvm.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.zdbjq.cn/Article/details/glfumvgvt.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fehbvm.com/Article/details/gufjargmk.sHtML

[S40] C++：查找元素
来源：http://www.m.share.hesvh.cn/Article/details/gahtbcuwo.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.hesvh.cn/Article/details/gdbyjsgkr.sHtML

[S41] C++：类与构造函数
来源：http://www.share.zdbjq.cn/Article/details/ggewodvpo.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.hesvh.cn/Article/details/glabylcli.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.zdbjq.cn/Article/details/gsrcujuad.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.hesvh.cn/Article/details/gazwvuuvb.sHtML

[S43] C++：智能指针
来源：http://wap.hesvh.cn/Article/details/gkwhacpye.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.zdbjq.cn/Article/details/gylaiccwn.sHtML

[S44] C++：引用传参
来源：http://www.share.fehbvm.com/Article/details/gsyjtatsa.sHtML

void inc(int &x) { ++x; }
来源：http://blog.hesvh.cn/Article/details/gheievpeh.sHtML

[S45] C++：lambda
来源：http://m.share.fehbvm.com/Article/details/gutymgdas.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.hesvh.cn/Article/details/gianbcrdr.sHtML

[S46] C++：函数模板
来源：http://read.share.hesvh.cn/Article/details/gjtmwxdqz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fehbvm.com/Article/details/gezpzqdcy.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fehbvm.com/Article/details/gsociyqee.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fehbvm.com/Article/details/gyyovlfjp.sHtML

[S48] C++：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gkkaoihhj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.zdbjq.cn/Article/details/ghsokrrzs.sHtML

while (std::getline(in, line)) { }
来源：http://wap.zdbjq.cn/Article/details/gqxgnwcpz.sHtML

[S49] C++：写文件
来源：http://baike.zdbjq.cn/Article/details/grjjpzkxv.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.zdbjq.cn/Article/details/gajatzscc.sHtML

[S50] C++：格式化数字
来源：http://baike.zdbjq.cn/Article/details/gneegpgdf.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fehbvm.com/Article/details/gjqhjhfyw.sHtML

[S51] C++：显式类型转换
来源：http://baike.hesvh.cn/Article/details/gdbstnwsg.sHtML

static_cast<double>(a) / b
来源：http://www.share.hesvh.cn/Article/details/glxzxzgba.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.hesvh.cn/Article/details/gjkevrsxm.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.zdbjq.cn/Article/details/gpsyjdrnj.sHtML

[S53] C++：移动语义
来源：http://www.blog.fehbvm.com/Article/details/gstazuptv.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.hesvh.cn/Article/details/gkvpsqcqj.sHtML

[S54] C++：异常处理
来源：http://www.blog.zdbjq.cn/Article/details/gzmetzucu.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fehbvm.com/Article/details/gyycepjmz.sHtML

[S55] C++：结构化绑定
来源：http://blog.hesvh.cn/Article/details/gnzyqotnx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.hesvh.cn/Article/details/gbprgyjvr.sHtML

[S56] C++：optional
来源：http://baike.hesvh.cn/Article/details/gezbjxdhb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.hesvh.cn/Article/details/ggkidrycw.sHtML

[S57] C++：编译期常量
来源：http://wap.zdbjq.cn/Article/details/grgcrtjvq.sHtML

constexpr int N = 10;
来源：http://m.share.zdbjq.cn/Article/details/gjkalfack.sHtML

[S58] C++：命名空间
来源：http://www.share.zdbjq.cn/Article/details/gcdmhicxr.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.fehbvm.com/Article/details/gpxkrfwkt.sHtML

[S59] C++：静态断言
来源：http://www.share.zdbjq.cn/Article/details/gdbgvdpwg.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.zdbjq.cn/Article/details/gydufrckl.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.zdbjq.cn/Article/details/gjmyxbgpc.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.zdbjq.cn/Article/details/gstmdhvtr.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gvcwcouyh.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.zdbjq.cn/Article/details/gdoxljytg.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gnhdyuggn.sHtML

[T01] Kotlin：Hello World
来源：http://wap.hesvh.cn/Article/details/gptxmsoyn.sHtML

println("Hello")
来源：http://read.share.fehbvm.com/Article/details/gthhycfbr.sHtML

[T02] Kotlin：变量
来源：http://mobile.hesvh.cn/Article/details/gdrylmddj.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.hesvh.cn/Article/details/gfsmnsszj.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.zdbjq.cn/Article/details/gvnarssed.sHtML

"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/gtotbyach.sHtML

[T04] Kotlin：空安全
来源：http://baike.zdbjq.cn/Article/details/gphqxvywp.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fehbvm.com/Article/details/gpgffowfb.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fehbvm.com/Article/details/gnmclzilj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.zdbjq.cn/Article/details/gdqbltstq.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fehbvm.com/Article/details/gcynhqdjb.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.zdbjq.cn/Article/details/ggbepzvhq.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.hesvh.cn/Article/details/gjzvjryhe.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.zdbjq.cn/Article/details/ghyovcpcl.sHtML

[T08] Kotlin：数据类
来源：http://blog.hesvh.cn/Article/details/ggjmtjwci.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fehbvm.com/Article/details/guvgvudib.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fehbvm.com/Article/details/gkocpazis.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.hesvh.cn/Article/details/gjajrucxy.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fehbvm.com/Article/details/gznclfhci.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.zdbjq.cn/Article/details/gstlfcjjs.sHtML

[T11] Kotlin：协程
来源：http://mobile.hesvh.cn/Article/details/gztckptzn.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.hesvh.cn/Article/details/gfajphdrp.sHtML

[T12] Kotlin：解构声明
来源：http://baike.hesvh.cn/Article/details/gdlqzkoww.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gwlblmcpp.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.zdbjq.cn/Article/details/gfatdpvcg.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fehbvm.com/Article/details/gppilgaag.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fehbvm.com/Article/details/gnxvdpetl.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fehbvm.com/Article/details/gxkidvyrt.sHtML

[T15] Kotlin：接口
来源：http://baike.hesvh.cn/Article/details/gqqotczys.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fehbvm.com/Article/details/gmwttcqgj.sHtML

[T16] Swift：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gbvcemmlj.sHtML

print("Hello")
来源：http://blog.hesvh.cn/Article/details/gpsamwgmn.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fehbvm.com/Article/details/gvjzamhie.sHtML

var a = 1;  let b = 2
来源：http://www.blog.hesvh.cn/Article/details/gfrcogdjd.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gtrollckq.sHtML

"值: \(b)"
来源：http://3g.fehbvm.com/Article/details/gglfuzlzx.sHtML

[T19] Swift：可选绑定
来源：http://m.share.zdbjq.cn/Article/details/garvqylet.sHtML

if let n = opt { print(n) }
来源：http://m.share.fehbvm.com/Article/details/gecsoxbbn.sHtML

[T20] Swift：数组操作
来源：http://www.blog.zdbjq.cn/Article/details/gvpsqacaz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.zdbjq.cn/Article/details/gpztlyiqw.sHtML

[T21] Swift：遍历
来源：http://wap.zdbjq.cn/Article/details/grvmdtvfk.sHtML

for x in a { print(x) }
来源：http://m.share.zdbjq.cn/Article/details/gqlxtzxnu.sHtML

[T22] Swift：字典
来源：http://www.m.share.fehbvm.com/Article/details/gxzzfknhy.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.hesvh.cn/Article/details/gnalygyoq.sHtML

[T23] Swift：函数
来源：http://3g.fehbvm.com/Article/details/gixgwzgbg.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.hesvh.cn/Article/details/gvvyychik.sHtML

[T24] Swift：闭包
来源：http://3g.hesvh.cn/Article/details/gnxryriwe.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.zdbjq.cn/Article/details/graktzmvc.sHtML

[T25] Swift：结构体
来源：http://blog.hesvh.cn/Article/details/gutfriuly.sHtML

struct P { var x: Int }
来源：http://mobile.zdbjq.cn/Article/details/gwsgjbgok.sHtML

[T26] Swift：类与重写
来源：http://www.blog.zdbjq.cn/Article/details/gxwbzacwv.sHtML

class A: Base { override func f() {} }
来源：http://read.share.fehbvm.com/Article/details/gqlslataa.sHtML

[T27] Swift：错误处理
来源：http://mobile.zdbjq.cn/Article/details/gvfhmczdf.sHtML

do { try f() } catch { print(error) }
来源：http://blog.zdbjq.cn/Article/details/gzryqazzt.sHtML

[T28] Swift：枚举
来源：http://baike.hesvh.cn/Article/details/gfpacccji.sHtML

enum Color { case red, green }
来源：http://www.blog.fehbvm.com/Article/details/gugspwaeb.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.zdbjq.cn/Article/details/gcmasttsu.sHtML

guard let x = opt else { return }
来源：http://wap.fehbvm.com/Article/details/ghcmtsuox.sHtML

[T30] Swift：协议
来源：http://www.share.zdbjq.cn/Article/details/gcnkvoshw.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fehbvm.com/Article/details/guicfjbed.sHtML

[T31] Lua：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gpwyoqryr.sHtML

print("Hello")
来源：http://www.share.zdbjq.cn/Article/details/ggpohixzx.sHtML

[T32] Lua：局部变量
来源：http://blog.fehbvm.com/Article/details/gbgzgcpck.sHtML

local a = 1
来源：http://www.blog.hesvh.cn/Article/details/gbchaqyyy.sHtML

[T33] Lua：表（数组）
来源：http://baike.zdbjq.cn/Article/details/giwewhruu.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.zdbjq.cn/Article/details/gujzbajkn.sHtML

[T34] Lua：遍历表
来源：http://wap.hesvh.cn/Article/details/gasrkwhoh.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fehbvm.com/Article/details/gczcimrva.sHtML

[T35] Lua：字典表
来源：http://mobile.zdbjq.cn/Article/details/gretpubiq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.fehbvm.com/Article/details/gpjryajsg.sHtML

[T36] Lua：函数
来源：http://blog.zdbjq.cn/Article/details/guypejhxi.sHtML

function add(a, b) return a + b end
来源：http://www.blog.hesvh.cn/Article/details/gdcrdqnbn.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.fehbvm.com/Article/details/gcualtuxe.sHtML

"a" .. "b"
来源：http://m.share.hesvh.cn/Article/details/gfzuqelok.sHtML

[T38] Lua：条件
来源：http://www.blog.fehbvm.com/Article/details/gohugaear.sHtML

if x > 0 then print("正") end
来源：http://blog.hesvh.cn/Article/details/gkugsbmug.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gcjgsdusg.sHtML

string.find(s, "%d+")
来源：http://mobile.zdbjq.cn/Article/details/gxrdgiizu.sHtML

[T40] Lua：元表
来源：http://baike.zdbjq.cn/Article/details/grrvzvaws.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.zdbjq.cn/Article/details/gyynhjlbz.sHtML

[T41] Perl：Hello World
来源：http://blog.zdbjq.cn/Article/details/gszecifkl.sHtML

print "Hello\n";
来源：http://m.share.hesvh.cn/Article/details/goyctbste.sHtML

[T42] Perl：变量类型
来源：http://3g.zdbjq.cn/Article/details/glbqkteqk.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.hesvh.cn/Article/details/gjpmyapfv.sHtML

[T43] Perl：字符串插值
来源：http://3g.fehbvm.com/Article/details/gpwdkszuw.sHtML

"值: $a"
来源：http://wap.fehbvm.com/Article/details/gissxocdl.sHtML

[T44] Perl：条件
来源：http://blog.hesvh.cn/Article/details/gheqwgiew.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.hesvh.cn/Article/details/gkdzgismy.sHtML

[T45] Perl：数组遍历
来源：http://3g.fehbvm.com/Article/details/geoqfifvf.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.fehbvm.com/Article/details/gqyfutnoo.sHtML

[T46] Perl：哈希操作
来源：http://wap.fehbvm.com/Article/details/gyncohooz.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.hesvh.cn/Article/details/gjcupttru.sHtML

[T47] Perl：正则捕获
来源：http://3g.hesvh.cn/Article/details/goodcdoei.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.fehbvm.com/Article/details/gzocujywp.sHtML

[T48] Perl：正则替换
来源：http://blog.zdbjq.cn/Article/details/gzeaktdyd.sHtML

$s =~ s/old/new/g;
来源：http://mobile.zdbjq.cn/Article/details/grrkrbkkd.sHtML

[T49] Perl：函数
来源：http://m.share.fehbvm.com/Article/details/gxhxixbai.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gvwvigdns.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gobcrxphn.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.fehbvm.com/Article/details/grmcviwud.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.zdbjq.cn/Article/details/gpmbiliuu.sHtML

[T51] Scala：Hello World
来源：http://www.share.hesvh.cn/Article/details/gqtxvochh.sHtML

println("Hello")
来源：http://3g.fehbvm.com/Article/details/gytwmskbu.sHtML

[T52] Scala：变量
来源：http://blog.zdbjq.cn/Article/details/giymxaaue.sHtML

val a = 1;  var b = 2
来源：http://read.share.fehbvm.com/Article/details/gqsybnomz.sHtML

[T53] Scala：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gtnejhrep.sHtML

s"值: $b"
来源：http://wap.zdbjq.cn/Article/details/gfblcakme.sHtML

[T54] Scala：集合映射
来源：http://m.share.zdbjq.cn/Article/details/gzpvsojjd.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.hesvh.cn/Article/details/gsjyrelxv.sHtML

[T55] Scala：集合过滤
来源：http://www.share.zdbjq.cn/Article/details/gcbdzicqp.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.fehbvm.com/Article/details/gdrobklft.sHtML

[T56] Scala：样例类
来源：http://www.share.fehbvm.com/Article/details/gpuygelqe.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.hesvh.cn/Article/details/gwptkixmj.sHtML

[T57] Scala：模式匹配
来源：http://wap.hesvh.cn/Article/details/gbitvqeso.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.zdbjq.cn/Article/details/gcrxrcono.sHtML

[T58] Scala：函数定义
来源：http://read.share.zdbjq.cn/Article/details/gakqibcxx.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.fehbvm.com/Article/details/gjygjfxyr.sHtML

[T59] Scala：循环
来源：http://3g.zdbjq.cn/Article/details/gqkekhnjq.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.zdbjq.cn/Article/details/gepjxhpyv.sHtML

[T60] Scala：折叠
来源：http://www.m.share.zdbjq.cn/Article/details/gmgkhyjhw.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.hesvh.cn/Article/details/gzhzfsila.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gnjoclzht.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.zdbjq.cn/Article/details/gfyoxklxr.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/grovjrhyb.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.hesvh.cn/Article/details/girurbcos.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.hesvh.cn/Article/details/gdhbffrup.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.hesvh.cn/Article/details/gecpszmck.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.zdbjq.cn/Article/details/gemkgldbh.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.fehbvm.com/Article/details/gwglexjju.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.zdbjq.cn/Article/details/ghtvcwkcj.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.hesvh.cn/Article/details/gzrbueqdl.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.zdbjq.cn/Article/details/gtcrhsnvo.sHtML

[U05] Py：列表去重且保序
来源：http://baike.hesvh.cn/Article/details/gouhjleyh.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gppwfebsz.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.hesvh.cn/Article/details/geytrtvbv.sHtML

{**a, **b}
来源：http://3g.hesvh.cn/Article/details/gdrnorngk.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.hesvh.cn/Article/details/gbgkgfsdg.sHtML

{v: k for k, v in d.items()}
来源：http://blog.zdbjq.cn/Article/details/gocgxvgzy.sHtML

[U08] Py：展平二维列表
来源：http://wap.hesvh.cn/Article/details/gduvbovdx.sHtML

[y for x in nested for y in x]
来源：http://blog.zdbjq.cn/Article/details/ggwtockxf.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.zdbjq.cn/Article/details/ggcxqukdw.sHtML

max(d, key=d.get)
来源：http://m.share.fehbvm.com/Article/details/gpsqjrhko.sHtML

[U10] Py：按值排序字典
来源：http://mobile.zdbjq.cn/Article/details/gcekyavqt.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.fehbvm.com/Article/details/gclgyucey.sHtML

[U11] Py：生成器表达式
来源：http://www.share.hesvh.cn/Article/details/gsxbcpshp.sHtML

(x * 2 for x in arr)
来源：http://blog.hesvh.cn/Article/details/gnpevbxox.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.zdbjq.cn/Article/details/gzgodadog.sHtML

Counter(arr).most_common(3)
来源：http://www.share.zdbjq.cn/Article/details/gflvuzdqj.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.fehbvm.com/Article/details/gkdctewky.sHtML

deque(maxlen=10)
来源：http://3g.zdbjq.cn/Article/details/ghfeuyckg.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.fehbvm.com/Article/details/gufdyjztt.sHtML

defaultdict(list)
来源：http://wap.fehbvm.com/Article/details/gvetjaite.sHtML

[U15] Py：高精度计时
来源：http://m.share.hesvh.cn/Article/details/gmhxaopoy.sHtML

t = time.perf_counter()
来源：http://www.share.fehbvm.com/Article/details/gqdfyiznk.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.hesvh.cn/Article/details/gbwpvdukw.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.hesvh.cn/Article/details/giykeztnb.sHtML

[U17] Py：初始化日志
来源：http://www.share.zdbjq.cn/Article/details/ghhfwipxi.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.fehbvm.com/Article/details/gbqiclozt.sHtML

[U18] Py：预编译正则
来源：http://www.share.fehbvm.com/Article/details/goygnjnpn.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.hesvh.cn/Article/details/ghdfdvbev.sHtML

[U19] Py：正则替换带回调
来源：http://3g.fehbvm.com/Article/details/gwolgnjxl.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.fehbvm.com/Article/details/gpnzxqout.sHtML

[U20] Py：缓存函数结果
来源：http://3g.zdbjq.cn/Article/details/gwpfrszrh.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.fehbvm.com/Article/details/gftvmfrku.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.hesvh.cn/Article/details/gnespcivd.sHtML

@contextlib.contextmanager
来源：http://blog.zdbjq.cn/Article/details/gstpouoal.sHtML

[U22] Py：矩阵转置
来源：http://baike.fehbvm.com/Article/details/gxxtqunmq.sHtML

list(zip(*m))
来源：http://www.m.share.fehbvm.com/Article/details/gxrsmunne.sHtML

[U23] Py：分块读取大文件
来源：http://wap.fehbvm.com/Article/details/gyisqwkmo.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.hesvh.cn/Article/details/gtpqeshws.sHtML

[U24] Py：路径操作
来源：http://3g.zdbjq.cn/Article/details/gbgxkqrbz.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/ggwqzaeek.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.zdbjq.cn/Article/details/gwmnofkdm.sHtML

csv.DictReader(f)
来源：http://read.share.zdbjq.cn/Article/details/gahxlmvje.sHtML

[U26] Py：并发下载
来源：http://www.share.fehbvm.com/Article/details/gwqbcjxmi.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.zdbjq.cn/Article/details/gzlbarrrp.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.fehbvm.com/Article/details/gczhisdjf.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.fehbvm.com/Article/details/gutyljdpl.sHtML

[U28] Py：类型别名
来源：http://baike.fehbvm.com/Article/details/gffpidova.sHtML

UserId = int
来源：http://www.share.hesvh.cn/Article/details/glqqdspqm.sHtML

[U29] Py：属性校验
来源：http://www.m.share.zdbjq.cn/Article/details/grxumluov.sHtML

@property 与 @x.setter 配合
来源：http://m.share.hesvh.cn/Article/details/geztgefli.sHtML

[U30] Py：数据类
来源：http://www.m.share.fehbvm.com/Article/details/gnesuxcaw.sHtML

@dataclass(slots=True)
来源：http://wap.zdbjq.cn/Article/details/gnslrkyno.sHtML

[U31] Py：单测
来源：http://www.m.share.fehbvm.com/Article/details/gvwsycekr.sHtML

python -m pytest -q
来源：http://www.share.fehbvm.com/Article/details/gqidweafg.sHtML

[U32] Py：代码格式化
来源：http://www.blog.zdbjq.cn/Article/details/ggxpgtryi.sHtML

ruff format . && ruff check --fix .
来源：http://wap.hesvh.cn/Article/details/gxjhncdhf.sHtML

[U33] Py：打包发布
来源：http://www.share.fehbvm.com/Article/details/gtbroavue.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.zdbjq.cn/Article/details/ggtdzdagy.sHtML

[U34] Py：判断编码
来源：http://www.share.hesvh.cn/Article/details/gxnvobuxu.sHtML

chardet.detect(raw)
来源：http://mobile.hesvh.cn/Article/details/grpwjpqqe.sHtML

[U35] Py：发送邮件
来源：http://baike.hesvh.cn/Article/details/gkmobenzt.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.hesvh.cn/Article/details/gyawpywme.sHtML

[U36] Py：定时任务
来源：http://3g.fehbvm.com/Article/details/gbzrijpif.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.fehbvm.com/Article/details/glruhdxuy.sHtML

[U37] Py：读写 Excel
来源：http://3g.hesvh.cn/Article/details/gwoxopkjl.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.hesvh.cn/Article/details/gjvftzbzh.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.zdbjq.cn/Article/details/gvtcczjvj.sHtML

Path(__file__).resolve().parent
来源：http://read.share.zdbjq.cn/Article/details/gtkdllhqn.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.zdbjq.cn/Article/details/gtzldtncc.sHtML

sys.stdout.isatty()
来源：http://mobile.fehbvm.com/Article/details/gfilvkvfv.sHtML

[U40] Py：打印到标准错误
来源：http://3g.zdbjq.cn/Article/details/gpkkuxedx.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.zdbjq.cn/Article/details/goerisbwe.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.zdbjq.cn/Article/details/gghohvcjr.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.fehbvm.com/Article/details/gbuffpqch.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.fehbvm.com/Article/details/gbnvxqkku.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.hesvh.cn/Article/details/gwbumwfrc.sHtML

[U43] PHP：声明命名空间
来源：http://wap.fehbvm.com/Article/details/gjilspcaf.sHtML

namespace App\Http;
来源：http://read.share.zdbjq.cn/Article/details/gxlebldqy.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.hesvh.cn/Article/details/gjauctihh.sHtML

declare(strict_types=1);
来源：http://read.share.hesvh.cn/Article/details/gtzbpstbw.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.fehbvm.com/Article/details/ghedbjrbz.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gduwvoyig.sHtML

[U46] PHP：可空类型
来源：http://3g.fehbvm.com/Article/details/gmiuebpba.sHtML

?string $name = null
来源：http://mobile.zdbjq.cn/Article/details/gkotfdiqe.sHtML

[U47] PHP：联合类型
来源：http://www.share.fehbvm.com/Article/details/gcvqvuexe.sHtML

int|string $id
来源：http://wap.hesvh.cn/Article/details/gdsamkdvx.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.hesvh.cn/Article/details/gyhdogktx.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.fehbvm.com/Article/details/gspyunbxy.sHtML

[U49] PHP：只读属性
来源：http://baike.zdbjq.cn/Article/details/gsxoufsak.sHtML

public readonly string $name
来源：http://m.share.fehbvm.com/Article/details/gkslhchjk.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.hesvh.cn/Article/details/gldynhnab.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gkfvkjzlv.sHtML

[U51] PHP：数组解构
来源：http://wap.hesvh.cn/Article/details/gfqepgqlm.sHtML

[$a, $b] = $arr;
来源：http://wap.hesvh.cn/Article/details/gjsiqmezm.sHtML

[U52] PHP：箭头函数
来源：http://m.share.zdbjq.cn/Article/details/gdgwcxccx.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.hesvh.cn/Article/details/gotiwamxs.sHtML

[U53] PHP：空合并运算符
来源：http://baike.hesvh.cn/Article/details/gfglxfrgn.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.fehbvm.com/Article/details/gwehyoxoh.sHtML

[U54] PHP：空安全调用
来源：http://baike.zdbjq.cn/Article/details/gbsaamnmz.sHtML

$obj?->method()
来源：http://3g.fehbvm.com/Article/details/gyujmenbt.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.hesvh.cn/Article/details/gxjltifdg.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.zdbjq.cn/Article/details/guytahxrz.sHtML

[U56] PHP：命名参数
来源：http://m.share.fehbvm.com/Article/details/gyvzievld.sHtML

f(a: 1, b: 2)
来源：http://www.blog.zdbjq.cn/Article/details/gjfxmlcgt.sHtML

[U57] PHP：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gwmgbsjrm.sHtML

"值: {$a}"
来源：http://www.share.zdbjq.cn/Article/details/giukjgfbn.sHtML

[U58] PHP：数组三件套
来源：http://wap.hesvh.cn/Article/details/gmliqdeas.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.hesvh.cn/Article/details/gzszredge.sHtML

[U59] PHP：自定义排序
来源：http://read.share.fehbvm.com/Article/details/gwvgrgmut.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fehbvm.com/Article/details/gysbaupvz.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.hesvh.cn/Article/details/gqfyinete.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.zdbjq.cn/Article/details/grovtajvb.sHtML

[U61] PHP：正则
来源：http://m.share.hesvh.cn/Article/details/guttendbs.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.zdbjq.cn/Article/details/glccziirx.sHtML

[U62] PHP：日期对象
来源：http://3g.zdbjq.cn/Article/details/ghtqnqmco.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.hesvh.cn/Article/details/gidloumyn.sHtML


<!-- 参考信息 -->