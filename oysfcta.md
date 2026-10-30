代发 wailian999

[S35] C++：map
来源：http://baike.zdbjq.cn/Article/details/ggxcsykvv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fehbvm.com/Article/details/ghgyuuyjq.sHtML

[S36] C++：unordered_map
来源：http://www.share.fehbvm.com/Article/details/glifitdou.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gibriyuwc.sHtML

[S37] C++：set
来源：http://www.blog.hesvh.cn/Article/details/gkibdooff.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.zdbjq.cn/Article/details/ggbyzyrfe.sHtML

[S38] C++：排序
来源：http://www.m.share.fehbvm.com/Article/details/gguridxds.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.zdbjq.cn/Article/details/gfhmqzryf.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fehbvm.com/Article/details/gvohbotuf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fehbvm.com/Article/details/gfnubnapu.sHtML

[S40] C++：查找元素
来源：http://blog.fehbvm.com/Article/details/gngkiclud.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.hesvh.cn/Article/details/gdlbpborz.sHtML

[S41] C++：类与构造函数
来源：http://baike.hesvh.cn/Article/details/gqrrngarv.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.hesvh.cn/Article/details/ggxpikbab.sHtML

[S42] C++：继承与虚函数
来源：http://baike.hesvh.cn/Article/details/gpuxasllb.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fehbvm.com/Article/details/gssmpqywm.sHtML

[S43] C++：智能指针
来源：http://www.blog.fehbvm.com/Article/details/gcysbfbpc.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.hesvh.cn/Article/details/glxcdtvgr.sHtML

[S44] C++：引用传参
来源：http://read.share.fehbvm.com/Article/details/gctqugjql.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.zdbjq.cn/Article/details/ghuureppq.sHtML

[S45] C++：lambda
来源：http://mobile.hesvh.cn/Article/details/gniwssuhg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.zdbjq.cn/Article/details/gxtsfdkbv.sHtML

[S46] C++：函数模板
来源：http://blog.zdbjq.cn/Article/details/gecdgmmaq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.hesvh.cn/Article/details/gssycizpm.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fehbvm.com/Article/details/gxxchiesb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.hesvh.cn/Article/details/gszvfirzb.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gkagjjisc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fehbvm.com/Article/details/grakqaiql.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fehbvm.com/Article/details/gnbqsvujh.sHtML

[S49] C++：写文件
来源：http://wap.zdbjq.cn/Article/details/grtcjmzpx.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.hesvh.cn/Article/details/gdsdcxipk.sHtML

[S50] C++：格式化数字
来源：http://www.share.zdbjq.cn/Article/details/gwutkwjkq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.hesvh.cn/Article/details/grkruudtw.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/gjppqfqkb.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.zdbjq.cn/Article/details/gkejpygas.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.hesvh.cn/Article/details/gzbsbqbhx.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.hesvh.cn/Article/details/gjccbaiyb.sHtML

[S53] C++：移动语义
来源：http://read.share.hesvh.cn/Article/details/gkpafkonh.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fehbvm.com/Article/details/guqdhnuxw.sHtML

[S54] C++：异常处理
来源：http://read.share.fehbvm.com/Article/details/ghvdufrhr.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fehbvm.com/Article/details/ghulbqwqd.sHtML

[S55] C++：结构化绑定
来源：http://wap.fehbvm.com/Article/details/gpmvkzqir.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.hesvh.cn/Article/details/ghspyoytq.sHtML

[S56] C++：optional
来源：http://read.share.zdbjq.cn/Article/details/gjllbjkjx.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fehbvm.com/Article/details/gtocxymml.sHtML

[S57] C++：编译期常量
来源：http://read.share.zdbjq.cn/Article/details/gwqlxwhdz.sHtML

constexpr int N = 10;
来源：http://baike.fehbvm.com/Article/details/gmypjkyna.sHtML

[S58] C++：命名空间
来源：http://www.share.hesvh.cn/Article/details/gauiajdjd.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.hesvh.cn/Article/details/grkojxvjt.sHtML

[S59] C++：静态断言
来源：http://blog.zdbjq.cn/Article/details/gghhkecvo.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fehbvm.com/Article/details/gargakqsf.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fehbvm.com/Article/details/gtkjidvim.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fehbvm.com/Article/details/gdhktuqtw.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ghlnjpbis.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.hesvh.cn/Article/details/gzrkxvold.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gbqcuspmf.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.hesvh.cn/Article/details/gobwwodmk.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/gycbjxfaq.sHtML

[T02] Kotlin：变量
来源：http://baike.hesvh.cn/Article/details/gghxjslfm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fehbvm.com/Article/details/gunjmxzfh.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fehbvm.com/Article/details/gbobzvthl.sHtML

"值: $b"
来源：http://www.m.share.zdbjq.cn/Article/details/gooiwxcpd.sHtML

[T04] Kotlin：空安全
来源：http://3g.fehbvm.com/Article/details/gokewhbna.sHtML

val n: String? = null;  n?.length
来源：http://www.share.hesvh.cn/Article/details/gjeqliwlb.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fehbvm.com/Article/details/ggsexsbci.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fehbvm.com/Article/details/geflhfiph.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.hesvh.cn/Article/details/gnvzsxrfk.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gmtowadpx.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.zdbjq.cn/Article/details/gzxdfqjvi.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.zdbjq.cn/Article/details/gszfnppkl.sHtML

[T08] Kotlin：数据类
来源：http://wap.zdbjq.cn/Article/details/gcwcvbicp.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fehbvm.com/Article/details/gukyuhqfb.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.zdbjq.cn/Article/details/gtliqyqdk.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.zdbjq.cn/Article/details/gwmpsmpui.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fehbvm.com/Article/details/glemmlfyf.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.hesvh.cn/Article/details/gdydrjjtp.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fehbvm.com/Article/details/gkcdoarvx.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fehbvm.com/Article/details/goarlgoaf.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fehbvm.com/Article/details/gbxlitqry.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fehbvm.com/Article/details/gqrmbdxkz.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.zdbjq.cn/Article/details/gidioyskw.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gqyztyhoo.sHtML

[T14] Kotlin：循环
来源：http://blog.fehbvm.com/Article/details/gyrkptmdj.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.hesvh.cn/Article/details/gdbbuiker.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fehbvm.com/Article/details/ghxfbhihr.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.hesvh.cn/Article/details/geqskhorz.sHtML

[T16] Swift：Hello World
来源：http://m.share.fehbvm.com/Article/details/gcmulcsuh.sHtML

print("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gonppetbi.sHtML

[T17] Swift：变量与常量
来源：http://wap.zdbjq.cn/Article/details/gwlrcrnzv.sHtML

var a = 1;  let b = 2
来源：http://3g.zdbjq.cn/Article/details/gkjbyvpav.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/goavzlcxb.sHtML

"值: \(b)"
来源：http://www.m.share.zdbjq.cn/Article/details/getaobwtj.sHtML

[T19] Swift：可选绑定
来源：http://wap.fehbvm.com/Article/details/gcmhdmllh.sHtML

if let n = opt { print(n) }
来源：http://blog.hesvh.cn/Article/details/gondfujkx.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.zdbjq.cn/Article/details/gcuklwnox.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.zdbjq.cn/Article/details/gmwfsktiw.sHtML

[T21] Swift：遍历
来源：http://blog.zdbjq.cn/Article/details/gxnfcjuhk.sHtML

for x in a { print(x) }
来源：http://read.share.hesvh.cn/Article/details/geussjvzu.sHtML

[T22] Swift：字典
来源：http://mobile.fehbvm.com/Article/details/gvinrdeiy.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fehbvm.com/Article/details/gbaxhccav.sHtML

[T23] Swift：函数
来源：http://read.share.hesvh.cn/Article/details/gonjyypxw.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.zdbjq.cn/Article/details/gouvhfrwj.sHtML

[T24] Swift：闭包
来源：http://m.share.zdbjq.cn/Article/details/gixoaoaqg.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.hesvh.cn/Article/details/grhqyyabm.sHtML

[T25] Swift：结构体
来源：http://wap.fehbvm.com/Article/details/gujrhvmpc.sHtML

struct P { var x: Int }
来源：http://blog.zdbjq.cn/Article/details/gephmgcum.sHtML

[T26] Swift：类与重写
来源：http://mobile.zdbjq.cn/Article/details/gdkfyuutq.sHtML

class A: Base { override func f() {} }
来源：http://mobile.zdbjq.cn/Article/details/gvmjkwuly.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fehbvm.com/Article/details/gtykgghdm.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fehbvm.com/Article/details/ggvpegmhj.sHtML

[T28] Swift：枚举
来源：http://mobile.hesvh.cn/Article/details/goonuqutg.sHtML

enum Color { case red, green }
来源：http://wap.hesvh.cn/Article/details/glgcblgmz.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.hesvh.cn/Article/details/gjpyznezo.sHtML

guard let x = opt else { return }
来源：http://m.share.zdbjq.cn/Article/details/gpekxybvd.sHtML

[T30] Swift：协议
来源：http://www.m.share.fehbvm.com/Article/details/gzokjkjfp.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.zdbjq.cn/Article/details/gaibavwwe.sHtML

[T31] Lua：Hello World
来源：http://www.share.fehbvm.com/Article/details/giymfnnej.sHtML

print("Hello")
来源：http://m.share.fehbvm.com/Article/details/gjutohigv.sHtML

[T32] Lua：局部变量
来源：http://wap.hesvh.cn/Article/details/gnosbwjdy.sHtML

local a = 1
来源：http://m.share.zdbjq.cn/Article/details/gddysqhmw.sHtML

[T33] Lua：表（数组）
来源：http://wap.fehbvm.com/Article/details/gfazxkgwh.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.zdbjq.cn/Article/details/gsyueqpqs.sHtML

[T34] Lua：遍历表
来源：http://read.share.hesvh.cn/Article/details/gthxzidip.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.fehbvm.com/Article/details/gizlibgyt.sHtML

[T35] Lua：字典表
来源：http://baike.fehbvm.com/Article/details/ghaqoigex.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gbztebwaj.sHtML

[T36] Lua：函数
来源：http://mobile.hesvh.cn/Article/details/gpiyweswd.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.zdbjq.cn/Article/details/ggweohung.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.fehbvm.com/Article/details/gsvjlisbt.sHtML

"a" .. "b"
来源：http://mobile.fehbvm.com/Article/details/gnjcowbsd.sHtML

[T38] Lua：条件
来源：http://www.blog.hesvh.cn/Article/details/gttzppodo.sHtML

if x > 0 then print("正") end
来源：http://www.share.hesvh.cn/Article/details/ghlogqzuc.sHtML

[T39] Lua：模式匹配
来源：http://3g.hesvh.cn/Article/details/gohkwtweb.sHtML

string.find(s, "%d+")
来源：http://read.share.fehbvm.com/Article/details/gwcyahigo.sHtML

[T40] Lua：元表
来源：http://blog.fehbvm.com/Article/details/gzytgalzk.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.fehbvm.com/Article/details/giacuwhvt.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gyelwxgje.sHtML

print "Hello\n";
来源：http://www.share.fehbvm.com/Article/details/ghwixniyo.sHtML

[T42] Perl：变量类型
来源：http://mobile.zdbjq.cn/Article/details/grzzvlwpv.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.zdbjq.cn/Article/details/gfdbxltgk.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gmsleuzzw.sHtML

"值: $a"
来源：http://mobile.fehbvm.com/Article/details/gxmsxtwjq.sHtML

[T44] Perl：条件
来源：http://wap.fehbvm.com/Article/details/gxhuvzraa.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.fehbvm.com/Article/details/gyizksfql.sHtML

[T45] Perl：数组遍历
来源：http://m.share.fehbvm.com/Article/details/ggzqarffq.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.fehbvm.com/Article/details/gupvavsnu.sHtML

[T46] Perl：哈希操作
来源：http://read.share.hesvh.cn/Article/details/gpzsstwrl.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.zdbjq.cn/Article/details/gucmjgnuh.sHtML

[T47] Perl：正则捕获
来源：http://wap.fehbvm.com/Article/details/giqyxyihr.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.fehbvm.com/Article/details/gvoktyplv.sHtML

[T48] Perl：正则替换
来源：http://www.share.hesvh.cn/Article/details/gwiivgsly.sHtML

$s =~ s/old/new/g;
来源：http://read.share.zdbjq.cn/Article/details/gfykyajgt.sHtML

[T49] Perl：函数
来源：http://baike.zdbjq.cn/Article/details/ghqhakxxl.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gjcsmdqom.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gpaienhsu.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.fehbvm.com/Article/details/gfjccsvvx.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.fehbvm.com/Article/details/griszmers.sHtML

[T51] Scala：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gagfugjka.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/gcscawcsu.sHtML

[T52] Scala：变量
来源：http://read.share.hesvh.cn/Article/details/gplfvzijz.sHtML

val a = 1;  var b = 2
来源：http://read.share.zdbjq.cn/Article/details/gnobvkxex.sHtML

[T53] Scala：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gxwfiehrh.sHtML

s"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/gvvbhrauy.sHtML

[T54] Scala：集合映射
来源：http://3g.fehbvm.com/Article/details/gflydwfat.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.fehbvm.com/Article/details/gipeallkl.sHtML

[T55] Scala：集合过滤
来源：http://3g.fehbvm.com/Article/details/gawvmwmmf.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.hesvh.cn/Article/details/gttmtbuvn.sHtML

[T56] Scala：样例类
来源：http://mobile.zdbjq.cn/Article/details/gxwpfpydh.sHtML

case class User(name: String, age: Int)
来源：http://mobile.fehbvm.com/Article/details/gdazslwop.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gvdijhzmc.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.zdbjq.cn/Article/details/gtzbqmyxv.sHtML

[T58] Scala：函数定义
来源：http://m.share.hesvh.cn/Article/details/gomtnoppl.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.fehbvm.com/Article/details/goayxesfj.sHtML

[T59] Scala：循环
来源：http://blog.fehbvm.com/Article/details/gdldpordd.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.zdbjq.cn/Article/details/gnfafmmkf.sHtML

[T60] Scala：折叠
来源：http://3g.hesvh.cn/Article/details/gltwnoltb.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.hesvh.cn/Article/details/gtphozukt.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gyojrneth.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.hesvh.cn/Article/details/geonovrdm.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gpyjtoutw.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.zdbjq.cn/Article/details/goylxtayz.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.hesvh.cn/Article/details/gjezrkorv.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.hesvh.cn/Article/details/gyuwcpgov.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gxtnhllmy.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.hesvh.cn/Article/details/gjlgfeejo.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.zdbjq.cn/Article/details/gxtrqenci.sHtML

[U04] Py：变量调试打印
来源：http://m.share.hesvh.cn/Article/details/gxcqdzoov.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.fehbvm.com/Article/details/gopbwqdas.sHtML

[U05] Py：列表去重且保序
来源：http://blog.fehbvm.com/Article/details/gkfwfcyty.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.hesvh.cn/Article/details/gjbqzqaft.sHtML

[U06] Py：合并两个字典
来源：http://blog.hesvh.cn/Article/details/gdgtdjspc.sHtML

{**a, **b}
来源：http://read.share.zdbjq.cn/Article/details/ggnuedhbx.sHtML

[U07] Py：反转字典键值
来源：http://wap.fehbvm.com/Article/details/gitfamaux.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fehbvm.com/Article/details/goptaulrp.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.hesvh.cn/Article/details/gvghkixux.sHtML

[y for x in nested for y in x]
来源：http://read.share.fehbvm.com/Article/details/gnvxvgksr.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.fehbvm.com/Article/details/gffrpriaa.sHtML

max(d, key=d.get)
来源：http://blog.hesvh.cn/Article/details/gdmqqaitb.sHtML

[U10] Py：按值排序字典
来源：http://wap.hesvh.cn/Article/details/gbejtxmwk.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.fehbvm.com/Article/details/ghbuplinz.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.hesvh.cn/Article/details/grmgvyddx.sHtML

(x * 2 for x in arr)
来源：http://read.share.hesvh.cn/Article/details/gcpxasipj.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.zdbjq.cn/Article/details/gjiafqoet.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.zdbjq.cn/Article/details/gsrqrlzoy.sHtML

[U13] Py：固定长度队列
来源：http://mobile.hesvh.cn/Article/details/gqviwiley.sHtML

deque(maxlen=10)
来源：http://read.share.fehbvm.com/Article/details/gidkvctqn.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.fehbvm.com/Article/details/gfmgnmeek.sHtML

defaultdict(list)
来源：http://www.m.share.fehbvm.com/Article/details/gjeseeqzn.sHtML

[U15] Py：高精度计时
来源：http://wap.fehbvm.com/Article/details/gjpvgtsnx.sHtML

t = time.perf_counter()
来源：http://www.m.share.zdbjq.cn/Article/details/gnkylsahf.sHtML

[U16] Py：命令行参数解析
来源：http://blog.hesvh.cn/Article/details/gugsukuno.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.hesvh.cn/Article/details/gkfeuidfb.sHtML

[U17] Py：初始化日志
来源：http://www.share.zdbjq.cn/Article/details/ghjlacrks.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.fehbvm.com/Article/details/glydznjrk.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.hesvh.cn/Article/details/ggkhitond.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.zdbjq.cn/Article/details/gkohglltm.sHtML

[U19] Py：正则替换带回调
来源：http://blog.fehbvm.com/Article/details/gcgsdzltm.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.zdbjq.cn/Article/details/gowebfnbs.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.fehbvm.com/Article/details/gjnbcbwbu.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.hesvh.cn/Article/details/ggjfkxixp.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.fehbvm.com/Article/details/gmnmsdths.sHtML

@contextlib.contextmanager
来源：http://m.share.fehbvm.com/Article/details/gxadoexct.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.hesvh.cn/Article/details/gsqprtnym.sHtML

list(zip(*m))
来源：http://3g.hesvh.cn/Article/details/gutznojsv.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.fehbvm.com/Article/details/gdstywrfo.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.fehbvm.com/Article/details/gdikjwihf.sHtML

[U24] Py：路径操作
来源：http://wap.hesvh.cn/Article/details/gxoxgevzl.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.fehbvm.com/Article/details/gxynkrnks.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.fehbvm.com/Article/details/gvqmsatyc.sHtML

csv.DictReader(f)
来源：http://mobile.fehbvm.com/Article/details/ghvdtzciw.sHtML

[U26] Py：并发下载
来源：http://www.m.share.fehbvm.com/Article/details/gozfcdmqn.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.zdbjq.cn/Article/details/gjhyahcnb.sHtML

[U27] Py：异步 HTTP
来源：http://wap.zdbjq.cn/Article/details/gdllkshsf.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.hesvh.cn/Article/details/gbqniuahb.sHtML

[U28] Py：类型别名
来源：http://mobile.fehbvm.com/Article/details/gkcwqlppq.sHtML

UserId = int
来源：http://www.blog.hesvh.cn/Article/details/gvofhzwqg.sHtML

[U29] Py：属性校验
来源：http://www.blog.hesvh.cn/Article/details/gowajmswc.sHtML

@property 与 @x.setter 配合
来源：http://www.share.zdbjq.cn/Article/details/gogjdoygz.sHtML

[U30] Py：数据类
来源：http://3g.hesvh.cn/Article/details/gowzgugak.sHtML

@dataclass(slots=True)
来源：http://www.m.share.fehbvm.com/Article/details/gtzwgiegi.sHtML

[U31] Py：单测
来源：http://m.share.hesvh.cn/Article/details/gkyvfrmai.sHtML

python -m pytest -q
来源：http://wap.hesvh.cn/Article/details/gbxfsoijx.sHtML

[U32] Py：代码格式化
来源：http://baike.fehbvm.com/Article/details/gkjzailkp.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.zdbjq.cn/Article/details/gujewjfge.sHtML

[U33] Py：打包发布
来源：http://m.share.zdbjq.cn/Article/details/gmptbbkti.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.zdbjq.cn/Article/details/ggtupnkkb.sHtML

[U34] Py：判断编码
来源：http://read.share.zdbjq.cn/Article/details/gxvukkovx.sHtML

chardet.detect(raw)
来源：http://m.share.fehbvm.com/Article/details/geyxvjsum.sHtML

[U35] Py：发送邮件
来源：http://www.blog.hesvh.cn/Article/details/gtqnrtatt.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.hesvh.cn/Article/details/gvjkrzxhx.sHtML

[U36] Py：定时任务
来源：http://wap.zdbjq.cn/Article/details/gubrraqfd.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.fehbvm.com/Article/details/gkbebulif.sHtML

[U37] Py：读写 Excel
来源：http://wap.fehbvm.com/Article/details/gyeqabgdq.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.hesvh.cn/Article/details/gvgceqjlf.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.fehbvm.com/Article/details/gvnhvrxso.sHtML

Path(__file__).resolve().parent
来源：http://mobile.fehbvm.com/Article/details/gnnwxyolw.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.fehbvm.com/Article/details/gbnrlrtsd.sHtML

sys.stdout.isatty()
来源：http://m.share.zdbjq.cn/Article/details/gydkbaopf.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.fehbvm.com/Article/details/gmjeszdiv.sHtML

print("err", file=sys.stderr)
来源：http://m.share.hesvh.cn/Article/details/gscxumeni.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.zdbjq.cn/Article/details/guepbcwpw.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.hesvh.cn/Article/details/gbudouodo.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.hesvh.cn/Article/details/gfenjfeeb.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.fehbvm.com/Article/details/ghmuygxbv.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.zdbjq.cn/Article/details/gwmkcunju.sHtML

namespace App\Http;
来源：http://www.blog.fehbvm.com/Article/details/gpdiolcjm.sHtML

[U44] PHP：开启严格类型
来源：http://blog.hesvh.cn/Article/details/gaswrnhgu.sHtML

declare(strict_types=1);
来源：http://wap.fehbvm.com/Article/details/gfelawdey.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.zdbjq.cn/Article/details/gxgmyxqph.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/goiojxwrb.sHtML

[U46] PHP：可空类型
来源：http://m.share.zdbjq.cn/Article/details/gdglhxcrh.sHtML

?string $name = null
来源：http://baike.hesvh.cn/Article/details/grvptmqrd.sHtML

[U47] PHP：联合类型
来源：http://blog.zdbjq.cn/Article/details/gazzudbtx.sHtML

int|string $id
来源：http://blog.fehbvm.com/Article/details/giaioaoud.sHtML

[U48] PHP：纯枚举
来源：http://3g.hesvh.cn/Article/details/gnjraqzix.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.hesvh.cn/Article/details/gtmwlxoqj.sHtML

[U49] PHP：只读属性
来源：http://m.share.zdbjq.cn/Article/details/gykxbrofm.sHtML

public readonly string $name
来源：http://read.share.zdbjq.cn/Article/details/gqobvssus.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.hesvh.cn/Article/details/ggfkrpzdt.sHtML

public function __construct(private int $id) {}
来源：http://blog.hesvh.cn/Article/details/gfwnabsdr.sHtML

[U51] PHP：数组解构
来源：http://www.blog.hesvh.cn/Article/details/gsdmvvzrj.sHtML

[$a, $b] = $arr;
来源：http://m.share.fehbvm.com/Article/details/guadidnlb.sHtML

[U52] PHP：箭头函数
来源：http://wap.hesvh.cn/Article/details/gbujiwtus.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.zdbjq.cn/Article/details/gychpgysx.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.zdbjq.cn/Article/details/gauotsbmt.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.fehbvm.com/Article/details/gntfqgeft.sHtML

[U54] PHP：空安全调用
来源：http://wap.hesvh.cn/Article/details/gixnxjhrx.sHtML

$obj?->method()
来源：http://3g.fehbvm.com/Article/details/gxmabkrgu.sHtML

[U55] PHP：match 表达式
来源：http://wap.fehbvm.com/Article/details/gazzdamvn.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.zdbjq.cn/Article/details/govuvbayb.sHtML

[U56] PHP：命名参数
来源：http://wap.zdbjq.cn/Article/details/gnwinvfcc.sHtML

f(a: 1, b: 2)
来源：http://www.blog.zdbjq.cn/Article/details/gvtracuom.sHtML

[U57] PHP：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gunynlocq.sHtML

"值: {$a}"
来源：http://www.m.share.fehbvm.com/Article/details/gkozpeawz.sHtML

[U58] PHP：数组三件套
来源：http://mobile.fehbvm.com/Article/details/gqqoiwrhl.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.hesvh.cn/Article/details/gqbxekuvd.sHtML

[U59] PHP：自定义排序
来源：http://blog.fehbvm.com/Article/details/gezowvkes.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.zdbjq.cn/Article/details/gsmqmrzdy.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.zdbjq.cn/Article/details/gpnapkyje.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.fehbvm.com/Article/details/gzswurvlp.sHtML


<!-- 参考信息 -->