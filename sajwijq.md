代发 wailian999

[S33] C++：vector 增删
来源：http://www.m.share.zdbjq.cn/Article/details/gpxebffxi.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.hesvh.cn/Article/details/gyakeuypm.sHtML

[S34] C++：遍历 vector
来源：http://baike.fehbvm.com/Article/details/gtoxvpinz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.hesvh.cn/Article/details/gfzxgbkvo.sHtML

[S35] C++：map
来源：http://www.blog.fehbvm.com/Article/details/gubuuydyf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gyxpceqrf.sHtML

[S36] C++：unordered_map
来源：http://mobile.hesvh.cn/Article/details/gccniualx.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gjqtannsk.sHtML

[S37] C++：set
来源：http://blog.zdbjq.cn/Article/details/gpbywkgwd.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.hesvh.cn/Article/details/ghtoppqnj.sHtML

[S38] C++：排序
来源：http://3g.zdbjq.cn/Article/details/gmfdidscb.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.zdbjq.cn/Article/details/gxwringxi.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fehbvm.com/Article/details/gwdznxfab.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.hesvh.cn/Article/details/glzbbswaa.sHtML

[S40] C++：查找元素
来源：http://www.share.fehbvm.com/Article/details/gkjckqfqh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fehbvm.com/Article/details/gewprtynl.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fehbvm.com/Article/details/gqrwxplbc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.hesvh.cn/Article/details/ggwpzeqnn.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fehbvm.com/Article/details/gyglrskxt.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.hesvh.cn/Article/details/gshhlupbo.sHtML

[S43] C++：智能指针
来源：http://wap.fehbvm.com/Article/details/gfuamdynb.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fehbvm.com/Article/details/gqtafcttm.sHtML

[S44] C++：引用传参
来源：http://mobile.hesvh.cn/Article/details/gzekuwyiw.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.zdbjq.cn/Article/details/galnyrfnb.sHtML

[S45] C++：lambda
来源：http://mobile.fehbvm.com/Article/details/gpqehunie.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.zdbjq.cn/Article/details/gpcvwzrbn.sHtML

[S46] C++：函数模板
来源：http://www.blog.hesvh.cn/Article/details/gegtbizks.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.hesvh.cn/Article/details/gpmtpytow.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.hesvh.cn/Article/details/gcuuwtkhv.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.hesvh.cn/Article/details/gzpvttmwf.sHtML

[S48] C++：逐行读文件
来源：http://3g.hesvh.cn/Article/details/guhgwcujq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.hesvh.cn/Article/details/gzmiuxnwr.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fehbvm.com/Article/details/gnxudaejc.sHtML

[S49] C++：写文件
来源：http://3g.hesvh.cn/Article/details/gmhsqmbhi.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.hesvh.cn/Article/details/gegimjrmr.sHtML

[S50] C++：格式化数字
来源：http://baike.zdbjq.cn/Article/details/gychcsqkl.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fehbvm.com/Article/details/grgumvrfk.sHtML

[S51] C++：显式类型转换
来源：http://wap.hesvh.cn/Article/details/gspumabic.sHtML

static_cast<double>(a) / b
来源：http://m.share.fehbvm.com/Article/details/gyuusmley.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.zdbjq.cn/Article/details/gpzbtfdbo.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fehbvm.com/Article/details/gtphhmcbl.sHtML

[S53] C++：移动语义
来源：http://3g.fehbvm.com/Article/details/goikabloo.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fehbvm.com/Article/details/gszzlbuin.sHtML

[S54] C++：异常处理
来源：http://m.share.hesvh.cn/Article/details/gxvwqhbfz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fehbvm.com/Article/details/gsrhqbold.sHtML

[S55] C++：结构化绑定
来源：http://m.share.hesvh.cn/Article/details/govperxht.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fehbvm.com/Article/details/gbcpqzuol.sHtML

[S56] C++：optional
来源：http://baike.hesvh.cn/Article/details/glzhyehxj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.zdbjq.cn/Article/details/gcfqmlizm.sHtML

[S57] C++：编译期常量
来源：http://blog.zdbjq.cn/Article/details/gkzshvlzc.sHtML

constexpr int N = 10;
来源：http://m.share.zdbjq.cn/Article/details/gftbnrmuf.sHtML

[S58] C++：命名空间
来源：http://3g.zdbjq.cn/Article/details/ghbirgmiv.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.hesvh.cn/Article/details/glimcygxp.sHtML

[S59] C++：静态断言
来源：http://read.share.hesvh.cn/Article/details/gzejbopzn.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.zdbjq.cn/Article/details/gyksbygoc.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.zdbjq.cn/Article/details/gegzcozrl.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.zdbjq.cn/Article/details/gupsyeswm.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gdwivpptp.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fehbvm.com/Article/details/gyumafehu.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/guvzwrpdt.sHtML

[T01] Kotlin：Hello World
来源：http://blog.zdbjq.cn/Article/details/gajtsrwja.sHtML

println("Hello")
来源：http://m.share.fehbvm.com/Article/details/gtqqapnop.sHtML

[T02] Kotlin：变量
来源：http://wap.hesvh.cn/Article/details/geybrfleu.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fehbvm.com/Article/details/gzjowkhsc.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.hesvh.cn/Article/details/gqzgmprao.sHtML

"值: $b"
来源：http://wap.fehbvm.com/Article/details/gwubucmkt.sHtML

[T04] Kotlin：空安全
来源：http://read.share.zdbjq.cn/Article/details/gyezygycr.sHtML

val n: String? = null;  n?.length
来源：http://m.share.zdbjq.cn/Article/details/gbokvnbgz.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.hesvh.cn/Article/details/gxunwwwpm.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.hesvh.cn/Article/details/gtedyojkf.sHtML

[T06] Kotlin：集合映射
来源：http://wap.hesvh.cn/Article/details/gcukuazmo.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fehbvm.com/Article/details/gigwhoqlh.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fehbvm.com/Article/details/gkbsuufsp.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.zdbjq.cn/Article/details/gvstusstg.sHtML

[T08] Kotlin：数据类
来源：http://m.share.zdbjq.cn/Article/details/gchybdieq.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.hesvh.cn/Article/details/gxetjyiax.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fehbvm.com/Article/details/gjnkewzps.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.hesvh.cn/Article/details/goywxpxmx.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.hesvh.cn/Article/details/gkixybofa.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.zdbjq.cn/Article/details/gockfyzxy.sHtML

[T11] Kotlin：协程
来源：http://mobile.hesvh.cn/Article/details/gkneqvvde.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.hesvh.cn/Article/details/gnmutmkry.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.hesvh.cn/Article/details/gkdooccrd.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gqyhqksir.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.zdbjq.cn/Article/details/gtofshdye.sHtML

val m = mapOf("a" to 1)
来源：http://3g.zdbjq.cn/Article/details/gsxjmyofo.sHtML

[T14] Kotlin：循环
来源：http://m.share.fehbvm.com/Article/details/gitbjwdpx.sHtML

for (i in 1..10) println(i)
来源：http://blog.hesvh.cn/Article/details/gxfbyabzd.sHtML

[T15] Kotlin：接口
来源：http://3g.fehbvm.com/Article/details/gxmxaabqk.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.zdbjq.cn/Article/details/ghtvalckq.sHtML

[T16] Swift：Hello World
来源：http://baike.zdbjq.cn/Article/details/gqeihmbyo.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/gdiugchlz.sHtML

[T17] Swift：变量与常量
来源：http://mobile.zdbjq.cn/Article/details/gaybuzjyh.sHtML

var a = 1;  let b = 2
来源：http://wap.hesvh.cn/Article/details/gxdokouxn.sHtML

[T18] Swift：字符串插值
来源：http://blog.hesvh.cn/Article/details/gzqwmfzee.sHtML

"值: \(b)"
来源：http://www.m.share.fehbvm.com/Article/details/gmndwsypc.sHtML

[T19] Swift：可选绑定
来源：http://baike.zdbjq.cn/Article/details/gqpspyded.sHtML

if let n = opt { print(n) }
来源：http://mobile.zdbjq.cn/Article/details/gacjpkbwy.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.zdbjq.cn/Article/details/gdqoqjpxm.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fehbvm.com/Article/details/gvmqjjfba.sHtML

[T21] Swift：遍历
来源：http://read.share.zdbjq.cn/Article/details/gdpamfopb.sHtML

for x in a { print(x) }
来源：http://wap.zdbjq.cn/Article/details/gjagycjoo.sHtML

[T22] Swift：字典
来源：http://baike.fehbvm.com/Article/details/geqslrkjc.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.zdbjq.cn/Article/details/gdyrlriwa.sHtML

[T23] Swift：函数
来源：http://baike.hesvh.cn/Article/details/galvsdcpf.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.zdbjq.cn/Article/details/gpztwbrjk.sHtML

[T24] Swift：闭包
来源：http://mobile.fehbvm.com/Article/details/gzbgxixjw.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.hesvh.cn/Article/details/gpnkyxgdu.sHtML

[T25] Swift：结构体
来源：http://m.share.hesvh.cn/Article/details/gotulptql.sHtML

struct P { var x: Int }
来源：http://mobile.zdbjq.cn/Article/details/grnqxchip.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.fehbvm.com/Article/details/gvttkabqs.sHtML

class A: Base { override func f() {} }
来源：http://baike.hesvh.cn/Article/details/gutqyguhs.sHtML

[T27] Swift：错误处理
来源：http://www.share.fehbvm.com/Article/details/gcgqngecg.sHtML

do { try f() } catch { print(error) }
来源：http://blog.fehbvm.com/Article/details/gigyfxiuc.sHtML

[T28] Swift：枚举
来源：http://mobile.fehbvm.com/Article/details/gesylibbc.sHtML

enum Color { case red, green }
来源：http://blog.fehbvm.com/Article/details/gbhgnnjvc.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.fehbvm.com/Article/details/gtdqfmemg.sHtML

guard let x = opt else { return }
来源：http://mobile.hesvh.cn/Article/details/gxvinzxxm.sHtML

[T30] Swift：协议
来源：http://www.blog.hesvh.cn/Article/details/gogeisayo.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.hesvh.cn/Article/details/glsloqbam.sHtML

[T31] Lua：Hello World
来源：http://mobile.fehbvm.com/Article/details/gkvyqqgru.sHtML

print("Hello")
来源：http://3g.zdbjq.cn/Article/details/gjcoegeue.sHtML

[T32] Lua：局部变量
来源：http://www.share.hesvh.cn/Article/details/gzpsjqdjx.sHtML

local a = 1
来源：http://wap.zdbjq.cn/Article/details/gdiqfhozt.sHtML

[T33] Lua：表（数组）
来源：http://read.share.hesvh.cn/Article/details/gmhcceegr.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.fehbvm.com/Article/details/gisonznhf.sHtML

[T34] Lua：遍历表
来源：http://www.blog.fehbvm.com/Article/details/gsrrstiux.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.zdbjq.cn/Article/details/gmhudgarz.sHtML

[T35] Lua：字典表
来源：http://mobile.hesvh.cn/Article/details/gcursphqp.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.zdbjq.cn/Article/details/ghrrzwgll.sHtML

[T36] Lua：函数
来源：http://3g.fehbvm.com/Article/details/gkhqtlkyh.sHtML

function add(a, b) return a + b end
来源：http://wap.hesvh.cn/Article/details/gxzqrsmfe.sHtML

[T37] Lua：字符串拼接
来源：http://blog.hesvh.cn/Article/details/gscidhfjm.sHtML

"a" .. "b"
来源：http://www.m.share.fehbvm.com/Article/details/grnjtbhyt.sHtML

[T38] Lua：条件
来源：http://wap.zdbjq.cn/Article/details/gcbpsgoda.sHtML

if x > 0 then print("正") end
来源：http://baike.fehbvm.com/Article/details/glxwuxsjd.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.hesvh.cn/Article/details/gkjpyotkr.sHtML

string.find(s, "%d+")
来源：http://www.blog.zdbjq.cn/Article/details/gyjiuaulo.sHtML

[T40] Lua：元表
来源：http://wap.zdbjq.cn/Article/details/gmgdufvez.sHtML

setmetatable({}, { __index = base })
来源：http://3g.zdbjq.cn/Article/details/gaviortsp.sHtML

[T41] Perl：Hello World
来源：http://baike.zdbjq.cn/Article/details/gqbcaugrg.sHtML

print "Hello\n";
来源：http://read.share.zdbjq.cn/Article/details/gusrdrsbw.sHtML

[T42] Perl：变量类型
来源：http://www.share.hesvh.cn/Article/details/gghrsnfex.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.hesvh.cn/Article/details/gzwpnvkhc.sHtML

[T43] Perl：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gofjisjwp.sHtML

"值: $a"
来源：http://mobile.fehbvm.com/Article/details/geanmafwh.sHtML

[T44] Perl：条件
来源：http://mobile.hesvh.cn/Article/details/giojhxjum.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.fehbvm.com/Article/details/geeazbqdv.sHtML

[T45] Perl：数组遍历
来源：http://wap.hesvh.cn/Article/details/glbuxikod.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.fehbvm.com/Article/details/gpmlfwkwd.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.hesvh.cn/Article/details/gdogndmhs.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.zdbjq.cn/Article/details/ghvmuuhup.sHtML

[T47] Perl：正则捕获
来源：http://3g.fehbvm.com/Article/details/gvjblakib.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.zdbjq.cn/Article/details/gtywlqxdd.sHtML

[T48] Perl：正则替换
来源：http://blog.zdbjq.cn/Article/details/gluxiexhk.sHtML

$s =~ s/old/new/g;
来源：http://blog.hesvh.cn/Article/details/gbriiydgd.sHtML

[T49] Perl：函数
来源：http://www.m.share.hesvh.cn/Article/details/grrxwerch.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gmvhiuvbq.sHtML

[T50] Perl：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/ghotucrnv.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.zdbjq.cn/Article/details/gnocqgcgk.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.hesvh.cn/Article/details/gtyzieplg.sHtML

[T51] Scala：Hello World
来源：http://m.share.fehbvm.com/Article/details/gvchtluwi.sHtML

println("Hello")
来源：http://www.share.hesvh.cn/Article/details/gjxbkuhtm.sHtML

[T52] Scala：变量
来源：http://m.share.zdbjq.cn/Article/details/gpfntqtaq.sHtML

val a = 1;  var b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gjzffjnbr.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gklttgrtm.sHtML

s"值: $b"
来源：http://blog.fehbvm.com/Article/details/gmniwzjjq.sHtML

[T54] Scala：集合映射
来源：http://www.blog.fehbvm.com/Article/details/gazaooeak.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.zdbjq.cn/Article/details/gnrxpnbam.sHtML

[T55] Scala：集合过滤
来源：http://read.share.hesvh.cn/Article/details/gpcxwcese.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.zdbjq.cn/Article/details/gxwilkshe.sHtML

[T56] Scala：样例类
来源：http://www.blog.fehbvm.com/Article/details/guvidlzsd.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.fehbvm.com/Article/details/gusylosih.sHtML

[T57] Scala：模式匹配
来源：http://wap.fehbvm.com/Article/details/gtigrnqqk.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fehbvm.com/Article/details/gwcgmgdjv.sHtML

[T58] Scala：函数定义
来源：http://www.blog.hesvh.cn/Article/details/ghachahee.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.hesvh.cn/Article/details/graqehhrs.sHtML

[T59] Scala：循环
来源：http://mobile.zdbjq.cn/Article/details/gamupiqqz.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/gttukppvg.sHtML

[T60] Scala：折叠
来源：http://www.blog.fehbvm.com/Article/details/gnrnrteob.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.zdbjq.cn/Article/details/geavkqkuh.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gumhdeolv.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.hesvh.cn/Article/details/gaiiqrsna.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gnsxgukss.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.fehbvm.com/Article/details/gzayeihxl.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.zdbjq.cn/Article/details/gvrdcepol.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.fehbvm.com/Article/details/gpqfctzpb.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.fehbvm.com/Article/details/ghnpvsswj.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.zdbjq.cn/Article/details/ggdhwexrk.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.zdbjq.cn/Article/details/gkxesmkau.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.fehbvm.com/Article/details/gnfiugbth.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.hesvh.cn/Article/details/gyzsobgcd.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.hesvh.cn/Article/details/gbowlgfes.sHtML

list(dict.fromkeys(arr))
来源：http://wap.fehbvm.com/Article/details/gcsolsqnq.sHtML

[U06] Py：合并两个字典
来源：http://wap.zdbjq.cn/Article/details/gsbhkdaeu.sHtML

{**a, **b}
来源：http://www.share.hesvh.cn/Article/details/gtvaosfmz.sHtML

[U07] Py：反转字典键值
来源：http://3g.fehbvm.com/Article/details/ggwhaopby.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.hesvh.cn/Article/details/gigkkqvcb.sHtML

[U08] Py：展平二维列表
来源：http://3g.fehbvm.com/Article/details/gzjzejmlu.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.fehbvm.com/Article/details/gjbinkzse.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.zdbjq.cn/Article/details/gqafmgrmu.sHtML

max(d, key=d.get)
来源：http://www.m.share.fehbvm.com/Article/details/gbwwblzec.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.fehbvm.com/Article/details/gkalchljt.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.hesvh.cn/Article/details/ghveivvfh.sHtML

[U11] Py：生成器表达式
来源：http://www.share.hesvh.cn/Article/details/goxccsuem.sHtML

(x * 2 for x in arr)
来源：http://read.share.zdbjq.cn/Article/details/gaxxlsoet.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.zdbjq.cn/Article/details/gavxfrtws.sHtML

Counter(arr).most_common(3)
来源：http://wap.zdbjq.cn/Article/details/gmndqrkit.sHtML

[U13] Py：固定长度队列
来源：http://www.share.hesvh.cn/Article/details/grfwywcmg.sHtML

deque(maxlen=10)
来源：http://www.blog.hesvh.cn/Article/details/gzgpqizyg.sHtML

[U14] Py：分组收集到列表
来源：http://wap.zdbjq.cn/Article/details/gzhurylpb.sHtML

defaultdict(list)
来源：http://www.blog.hesvh.cn/Article/details/gyhdlmlhv.sHtML

[U15] Py：高精度计时
来源：http://baike.fehbvm.com/Article/details/goglqvexc.sHtML

t = time.perf_counter()
来源：http://blog.fehbvm.com/Article/details/gckjjpdgr.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.zdbjq.cn/Article/details/gtrbcimxt.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.zdbjq.cn/Article/details/gpgcxladg.sHtML

[U17] Py：初始化日志
来源：http://read.share.zdbjq.cn/Article/details/galhyyqut.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.hesvh.cn/Article/details/gpcpxtwij.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.zdbjq.cn/Article/details/gnpbyqpas.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.zdbjq.cn/Article/details/gwqmddbzh.sHtML

[U19] Py：正则替换带回调
来源：http://wap.fehbvm.com/Article/details/gnnrorkbj.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.zdbjq.cn/Article/details/gsnaecrjx.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.zdbjq.cn/Article/details/gwblwhldr.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.zdbjq.cn/Article/details/gugbejdtn.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.hesvh.cn/Article/details/gktacezbh.sHtML

@contextlib.contextmanager
来源：http://m.share.fehbvm.com/Article/details/gqwunhviq.sHtML

[U22] Py：矩阵转置
来源：http://blog.hesvh.cn/Article/details/gvclyqfqt.sHtML

list(zip(*m))
来源：http://3g.hesvh.cn/Article/details/ggzakyqer.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.zdbjq.cn/Article/details/ggipzzfxe.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.zdbjq.cn/Article/details/gtrvxbtik.sHtML

[U24] Py：路径操作
来源：http://www.share.zdbjq.cn/Article/details/gvcrohhjq.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.zdbjq.cn/Article/details/ggzxtdtwc.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.fehbvm.com/Article/details/glajjoeeu.sHtML

csv.DictReader(f)
来源：http://mobile.zdbjq.cn/Article/details/grfxottpz.sHtML

[U26] Py：并发下载
来源：http://www.blog.fehbvm.com/Article/details/gwvgqpges.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.zdbjq.cn/Article/details/gismqnzvy.sHtML

[U27] Py：异步 HTTP
来源：http://3g.fehbvm.com/Article/details/gxbxoxbez.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.hesvh.cn/Article/details/ghzekpvxx.sHtML

[U28] Py：类型别名
来源：http://baike.fehbvm.com/Article/details/guoqvjdbw.sHtML

UserId = int
来源：http://blog.fehbvm.com/Article/details/gaajzbpdy.sHtML

[U29] Py：属性校验
来源：http://www.blog.fehbvm.com/Article/details/gunxfzemw.sHtML

@property 与 @x.setter 配合
来源：http://baike.zdbjq.cn/Article/details/ggleysevo.sHtML

[U30] Py：数据类
来源：http://wap.fehbvm.com/Article/details/gnnpdegps.sHtML

@dataclass(slots=True)
来源：http://baike.hesvh.cn/Article/details/gyetuxnmt.sHtML

[U31] Py：单测
来源：http://blog.fehbvm.com/Article/details/gazsxdjep.sHtML

python -m pytest -q
来源：http://www.m.share.fehbvm.com/Article/details/gxqpkujbn.sHtML

[U32] Py：代码格式化
来源：http://wap.zdbjq.cn/Article/details/gadjnxkqv.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.hesvh.cn/Article/details/gzaxtpxny.sHtML

[U33] Py：打包发布
来源：http://www.m.share.zdbjq.cn/Article/details/gypiswhyi.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.fehbvm.com/Article/details/gnglcsdpf.sHtML

[U34] Py：判断编码
来源：http://www.m.share.fehbvm.com/Article/details/gopbsmslq.sHtML

chardet.detect(raw)
来源：http://www.share.fehbvm.com/Article/details/ggjmcamka.sHtML

[U35] Py：发送邮件
来源：http://3g.zdbjq.cn/Article/details/ggryiqyfs.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.hesvh.cn/Article/details/gkzlbyzwu.sHtML

[U36] Py：定时任务
来源：http://blog.fehbvm.com/Article/details/gmhtexzgk.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.zdbjq.cn/Article/details/gqhilfaeb.sHtML

[U37] Py：读写 Excel
来源：http://wap.fehbvm.com/Article/details/gtvbugbap.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.zdbjq.cn/Article/details/gnnlpeilz.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.fehbvm.com/Article/details/gphgqnxuu.sHtML

Path(__file__).resolve().parent
来源：http://wap.zdbjq.cn/Article/details/ggzxhatin.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.fehbvm.com/Article/details/geehvykvk.sHtML

sys.stdout.isatty()
来源：http://www.m.share.hesvh.cn/Article/details/gyusopnkv.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.hesvh.cn/Article/details/gqinepbkq.sHtML

print("err", file=sys.stderr)
来源：http://blog.fehbvm.com/Article/details/gtzaecfiy.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.zdbjq.cn/Article/details/gztxmveug.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.fehbvm.com/Article/details/guatibkbu.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.fehbvm.com/Article/details/gaxltztfw.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.zdbjq.cn/Article/details/goynonhfk.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.zdbjq.cn/Article/details/gbimcfofu.sHtML

namespace App\Http;
来源：http://mobile.hesvh.cn/Article/details/gfycjabkw.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.hesvh.cn/Article/details/gnubgwrli.sHtML

declare(strict_types=1);
来源：http://www.share.hesvh.cn/Article/details/gdccqzrvw.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.fehbvm.com/Article/details/gulnbuipg.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gzdnpqcjv.sHtML

[U46] PHP：可空类型
来源：http://m.share.hesvh.cn/Article/details/gkcoowhfy.sHtML

?string $name = null
来源：http://m.share.hesvh.cn/Article/details/gzegrcsfm.sHtML

[U47] PHP：联合类型
来源：http://wap.hesvh.cn/Article/details/gdbbkpkdl.sHtML

int|string $id
来源：http://wap.zdbjq.cn/Article/details/gdtdigwjx.sHtML

[U48] PHP：纯枚举
来源：http://m.share.hesvh.cn/Article/details/gncwjmhns.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.hesvh.cn/Article/details/gfstmchza.sHtML

[U49] PHP：只读属性
来源：http://wap.hesvh.cn/Article/details/gidtsiddv.sHtML

public readonly string $name
来源：http://blog.zdbjq.cn/Article/details/glomqfyvu.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.hesvh.cn/Article/details/grxuxeyoy.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.zdbjq.cn/Article/details/geofioicr.sHtML

[U51] PHP：数组解构
来源：http://www.blog.zdbjq.cn/Article/details/gnmqfnjfk.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.hesvh.cn/Article/details/gcrvpdlbf.sHtML

[U52] PHP：箭头函数
来源：http://blog.hesvh.cn/Article/details/gvcowtvns.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.fehbvm.com/Article/details/gocqrquwd.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.hesvh.cn/Article/details/gkccvimwf.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.zdbjq.cn/Article/details/gzvljdeph.sHtML

[U54] PHP：空安全调用
来源：http://mobile.fehbvm.com/Article/details/gfocokqda.sHtML

$obj?->method()
来源：http://m.share.zdbjq.cn/Article/details/gfclozzpj.sHtML

[U55] PHP：match 表达式
来源：http://m.share.hesvh.cn/Article/details/gvgjymqyp.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.fehbvm.com/Article/details/gflyfioxr.sHtML

[U56] PHP：命名参数
来源：http://read.share.zdbjq.cn/Article/details/grpyzeteg.sHtML

f(a: 1, b: 2)
来源：http://www.share.hesvh.cn/Article/details/gaepzchdz.sHtML

[U57] PHP：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gaxccklfl.sHtML

"值: {$a}"
来源：http://mobile.hesvh.cn/Article/details/gvervfmgl.sHtML

[U58] PHP：数组三件套
来源：http://read.share.fehbvm.com/Article/details/gkwosyzso.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.fehbvm.com/Article/details/gfwnggifr.sHtML


<!-- 参考信息 -->