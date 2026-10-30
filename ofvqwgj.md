代发 wailian999

[S39] C++：自定义比较器排序
来源：http://3g.zdbjq.cn/Article/details/gfykzkslz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fehbvm.com/Article/details/gzwbxcvql.sHtML

[S40] C++：查找元素
来源：http://read.share.hesvh.cn/Article/details/gqgvvqqoc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.hesvh.cn/Article/details/gokwytsmf.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gzeicslxu.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.zdbjq.cn/Article/details/gcrfbzqol.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.hesvh.cn/Article/details/guxtocsdz.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.zdbjq.cn/Article/details/gepyldksr.sHtML

[S43] C++：智能指针
来源：http://m.share.fehbvm.com/Article/details/gezmszclm.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fehbvm.com/Article/details/gbyabrcei.sHtML

[S44] C++：引用传参
来源：http://wap.zdbjq.cn/Article/details/gopkjoxvs.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.hesvh.cn/Article/details/gsslwltrt.sHtML

[S45] C++：lambda
来源：http://baike.zdbjq.cn/Article/details/gkfuopsgh.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.zdbjq.cn/Article/details/gpfhwggnj.sHtML

[S46] C++：函数模板
来源：http://www.m.share.hesvh.cn/Article/details/gebegtrxa.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.zdbjq.cn/Article/details/gsysbqxud.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.hesvh.cn/Article/details/gyumnhyys.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.hesvh.cn/Article/details/gsxgvujgm.sHtML

[S48] C++：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gqxukvoig.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fehbvm.com/Article/details/gbkqltspb.sHtML

while (std::getline(in, line)) { }
来源：http://3g.zdbjq.cn/Article/details/gugdvfvoe.sHtML

[S49] C++：写文件
来源：http://3g.fehbvm.com/Article/details/gpibqpull.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fehbvm.com/Article/details/gfctdlzmz.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.zdbjq.cn/Article/details/gsrocdnva.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gpsfyjchv.sHtML

[S51] C++：显式类型转换
来源：http://wap.fehbvm.com/Article/details/gaxhcddiu.sHtML

static_cast<double>(a) / b
来源：http://blog.fehbvm.com/Article/details/gxojzjlmy.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fehbvm.com/Article/details/gzlbvgeyk.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.hesvh.cn/Article/details/gnnapnglu.sHtML

[S53] C++：移动语义
来源：http://blog.fehbvm.com/Article/details/guelxgiwn.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.hesvh.cn/Article/details/gxmonfmcn.sHtML

[S54] C++：异常处理
来源：http://mobile.zdbjq.cn/Article/details/ggszzkjlu.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.zdbjq.cn/Article/details/glglpdcom.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.zdbjq.cn/Article/details/gcyutvdfa.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.hesvh.cn/Article/details/gbnjnwxwn.sHtML

[S56] C++：optional
来源：http://blog.fehbvm.com/Article/details/gvmwvxwcf.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.hesvh.cn/Article/details/gtwlmvwsa.sHtML

[S57] C++：编译期常量
来源：http://baike.fehbvm.com/Article/details/gbbxqvlvf.sHtML

constexpr int N = 10;
来源：http://m.share.zdbjq.cn/Article/details/gxbwoksmm.sHtML

[S58] C++：命名空间
来源：http://baike.fehbvm.com/Article/details/gjxkkcxtg.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fehbvm.com/Article/details/gvklrusjk.sHtML

[S59] C++：静态断言
来源：http://m.share.hesvh.cn/Article/details/gfdyugggd.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.zdbjq.cn/Article/details/gtxkqwvdc.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.hesvh.cn/Article/details/gwbkockhg.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.hesvh.cn/Article/details/gniwqtxrz.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gtsmrwxrc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fehbvm.com/Article/details/grrjnvavi.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gsdxzmqeo.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.zdbjq.cn/Article/details/grnenrour.sHtML

println("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gxlddyryx.sHtML

[T02] Kotlin：变量
来源：http://wap.fehbvm.com/Article/details/gstupljwg.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.zdbjq.cn/Article/details/ggerwjkcn.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.hesvh.cn/Article/details/gktjdztej.sHtML

"值: $b"
来源：http://www.share.fehbvm.com/Article/details/gpjpaqcvq.sHtML

[T04] Kotlin：空安全
来源：http://3g.hesvh.cn/Article/details/gqsmhlred.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fehbvm.com/Article/details/gwxfnstdv.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.hesvh.cn/Article/details/grpkqsdqr.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fehbvm.com/Article/details/giozpjzcz.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.hesvh.cn/Article/details/guzbaynhm.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.hesvh.cn/Article/details/gwnnnvgtx.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.zdbjq.cn/Article/details/gfjmnhvwu.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fehbvm.com/Article/details/gtkavlxkm.sHtML

[T08] Kotlin：数据类
来源：http://wap.hesvh.cn/Article/details/gdpibknwb.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.hesvh.cn/Article/details/gvxeaownz.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.hesvh.cn/Article/details/gjdtrtvhl.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.hesvh.cn/Article/details/gqrgbdbrz.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.hesvh.cn/Article/details/gvvoybgvk.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.hesvh.cn/Article/details/gebfufhnf.sHtML

[T11] Kotlin：协程
来源：http://read.share.fehbvm.com/Article/details/gbxqptpmn.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.zdbjq.cn/Article/details/ggzomruee.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.hesvh.cn/Article/details/gcoqnrpew.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gexgzsina.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fehbvm.com/Article/details/gstgslgfx.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.zdbjq.cn/Article/details/gmxaezhws.sHtML

[T14] Kotlin：循环
来源：http://www.blog.zdbjq.cn/Article/details/gsgslzlsd.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.zdbjq.cn/Article/details/ggfuhconf.sHtML

[T15] Kotlin：接口
来源：http://3g.zdbjq.cn/Article/details/gscbfmoec.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.zdbjq.cn/Article/details/gixchsudm.sHtML

[T16] Swift：Hello World
来源：http://m.share.fehbvm.com/Article/details/ggbwdepsz.sHtML

print("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gybnuoaya.sHtML

[T17] Swift：变量与常量
来源：http://baike.fehbvm.com/Article/details/gcerzynmi.sHtML

var a = 1;  let b = 2
来源：http://mobile.hesvh.cn/Article/details/gosbbpznj.sHtML

[T18] Swift：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gkuowhqbe.sHtML

"值: \(b)"
来源：http://3g.zdbjq.cn/Article/details/gchxsytqt.sHtML

[T19] Swift：可选绑定
来源：http://www.share.zdbjq.cn/Article/details/grigiqevi.sHtML

if let n = opt { print(n) }
来源：http://wap.zdbjq.cn/Article/details/gwwlfbrfk.sHtML

[T20] Swift：数组操作
来源：http://wap.zdbjq.cn/Article/details/gmhnzrcuo.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.hesvh.cn/Article/details/gvpaboxjs.sHtML

[T21] Swift：遍历
来源：http://baike.zdbjq.cn/Article/details/gdzpfyjns.sHtML

for x in a { print(x) }
来源：http://www.blog.hesvh.cn/Article/details/glztpnjmu.sHtML

[T22] Swift：字典
来源：http://m.share.zdbjq.cn/Article/details/gugfkmyas.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fehbvm.com/Article/details/gtnnnseqw.sHtML

[T23] Swift：函数
来源：http://m.share.hesvh.cn/Article/details/gqdyespuy.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.zdbjq.cn/Article/details/glqfrxmmc.sHtML

[T24] Swift：闭包
来源：http://3g.zdbjq.cn/Article/details/geieekijf.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gvhhoyqxq.sHtML

[T25] Swift：结构体
来源：http://blog.zdbjq.cn/Article/details/grzrpgmzo.sHtML

struct P { var x: Int }
来源：http://mobile.zdbjq.cn/Article/details/gsabqebfq.sHtML

[T26] Swift：类与重写
来源：http://m.share.zdbjq.cn/Article/details/gdlcetsbv.sHtML

class A: Base { override func f() {} }
来源：http://m.share.zdbjq.cn/Article/details/gqozloueu.sHtML

[T27] Swift：错误处理
来源：http://wap.fehbvm.com/Article/details/geizqurax.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.zdbjq.cn/Article/details/gpdvxsfkn.sHtML

[T28] Swift：枚举
来源：http://baike.hesvh.cn/Article/details/ggqjxlevp.sHtML

enum Color { case red, green }
来源：http://read.share.fehbvm.com/Article/details/glnipddex.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.fehbvm.com/Article/details/girqzrlao.sHtML

guard let x = opt else { return }
来源：http://www.blog.zdbjq.cn/Article/details/gtxunmrqs.sHtML

[T30] Swift：协议
来源：http://www.blog.hesvh.cn/Article/details/gvneyhkwy.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.zdbjq.cn/Article/details/glqtjprgt.sHtML

[T31] Lua：Hello World
来源：http://baike.zdbjq.cn/Article/details/gmqmlssbh.sHtML

print("Hello")
来源：http://www.share.fehbvm.com/Article/details/gfjcroqtf.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.hesvh.cn/Article/details/gofizlrcx.sHtML

local a = 1
来源：http://wap.hesvh.cn/Article/details/golurdzrx.sHtML

[T33] Lua：表（数组）
来源：http://baike.fehbvm.com/Article/details/gvzdricsh.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.hesvh.cn/Article/details/gwfnwtzsj.sHtML

[T34] Lua：遍历表
来源：http://blog.zdbjq.cn/Article/details/gzyouxspt.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.zdbjq.cn/Article/details/gfhancncf.sHtML

[T35] Lua：字典表
来源：http://www.blog.fehbvm.com/Article/details/gimwqlpty.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.fehbvm.com/Article/details/gkskgfocu.sHtML

[T36] Lua：函数
来源：http://baike.hesvh.cn/Article/details/gffrlcbnm.sHtML

function add(a, b) return a + b end
来源：http://blog.fehbvm.com/Article/details/gzuvrmakv.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.hesvh.cn/Article/details/gnkrotnrn.sHtML

"a" .. "b"
来源：http://read.share.hesvh.cn/Article/details/gywymtqpk.sHtML

[T38] Lua：条件
来源：http://www.share.hesvh.cn/Article/details/gydidslpy.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.fehbvm.com/Article/details/gnccisqqh.sHtML

[T39] Lua：模式匹配
来源：http://3g.fehbvm.com/Article/details/glbjfbuwy.sHtML

string.find(s, "%d+")
来源：http://wap.zdbjq.cn/Article/details/gxlmcmwrb.sHtML

[T40] Lua：元表
来源：http://wap.fehbvm.com/Article/details/gfsiduybw.sHtML

setmetatable({}, { __index = base })
来源：http://3g.zdbjq.cn/Article/details/gorwcuhud.sHtML

[T41] Perl：Hello World
来源：http://wap.zdbjq.cn/Article/details/gyokacqpc.sHtML

print "Hello\n";
来源：http://m.share.fehbvm.com/Article/details/gzntipcgc.sHtML

[T42] Perl：变量类型
来源：http://m.share.zdbjq.cn/Article/details/gzkgybduv.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.hesvh.cn/Article/details/glodmwksz.sHtML

[T43] Perl：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gujpxenyp.sHtML

"值: $a"
来源：http://www.blog.zdbjq.cn/Article/details/gpkfymgzj.sHtML

[T44] Perl：条件
来源：http://www.blog.hesvh.cn/Article/details/gwccuuzle.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.hesvh.cn/Article/details/gdrxafinb.sHtML

[T45] Perl：数组遍历
来源：http://baike.hesvh.cn/Article/details/gvndpdxir.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.fehbvm.com/Article/details/gbevimtin.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fehbvm.com/Article/details/gcoyhvzsj.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.fehbvm.com/Article/details/gubsflguc.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.hesvh.cn/Article/details/gxpfwyxuc.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.zdbjq.cn/Article/details/glvcntbsa.sHtML

[T48] Perl：正则替换
来源：http://www.share.hesvh.cn/Article/details/glwdvbmdw.sHtML

$s =~ s/old/new/g;
来源：http://wap.fehbvm.com/Article/details/glcbshffj.sHtML

[T49] Perl：函数
来源：http://baike.zdbjq.cn/Article/details/ghvjwwkbf.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gmbpozakb.sHtML

[T50] Perl：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gktjoybwu.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.hesvh.cn/Article/details/gxdghrqdk.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.zdbjq.cn/Article/details/ggwkgstwq.sHtML

[T51] Scala：Hello World
来源：http://wap.fehbvm.com/Article/details/gvkramqbv.sHtML

println("Hello")
来源：http://blog.zdbjq.cn/Article/details/ggsefxgdp.sHtML

[T52] Scala：变量
来源：http://baike.zdbjq.cn/Article/details/gvhcygvja.sHtML

val a = 1;  var b = 2
来源：http://blog.zdbjq.cn/Article/details/gxhxzjzcn.sHtML

[T53] Scala：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gzrdmqjfr.sHtML

s"值: $b"
来源：http://www.m.share.hesvh.cn/Article/details/gcmcxaaqy.sHtML

[T54] Scala：集合映射
来源：http://baike.fehbvm.com/Article/details/gzqggllvr.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.hesvh.cn/Article/details/ggcaqxupv.sHtML

[T55] Scala：集合过滤
来源：http://3g.hesvh.cn/Article/details/gjmgnfkmf.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.hesvh.cn/Article/details/gimkpytba.sHtML

[T56] Scala：样例类
来源：http://m.share.fehbvm.com/Article/details/gxcojefys.sHtML

case class User(name: String, age: Int)
来源：http://www.share.hesvh.cn/Article/details/gvhgmhajb.sHtML

[T57] Scala：模式匹配
来源：http://m.share.hesvh.cn/Article/details/gttfspeko.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.zdbjq.cn/Article/details/gitrhketb.sHtML

[T58] Scala：函数定义
来源：http://baike.fehbvm.com/Article/details/gpznfjiyc.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.zdbjq.cn/Article/details/gygujpdcg.sHtML

[T59] Scala：循环
来源：http://www.m.share.fehbvm.com/Article/details/gwpzjsgot.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.hesvh.cn/Article/details/gakpsrbfp.sHtML

[T60] Scala：折叠
来源：http://www.blog.hesvh.cn/Article/details/glemcizra.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.fehbvm.com/Article/details/gldvxakoo.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gqzphorek.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.zdbjq.cn/Article/details/gnqjuvyyl.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gbvtbcfmf.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.zdbjq.cn/Article/details/gqbszculv.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.fehbvm.com/Article/details/ggdqryuck.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.zdbjq.cn/Article/details/gxetoolbw.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.zdbjq.cn/Article/details/gquttdcqr.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.fehbvm.com/Article/details/gmbkughwc.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.zdbjq.cn/Article/details/gusuozubb.sHtML

[U04] Py：变量调试打印
来源：http://m.share.hesvh.cn/Article/details/gzhjersiq.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.zdbjq.cn/Article/details/gpnydqvty.sHtML

[U05] Py：列表去重且保序
来源：http://blog.fehbvm.com/Article/details/gqhvbbyyu.sHtML

list(dict.fromkeys(arr))
来源：http://3g.zdbjq.cn/Article/details/gvgkrrpqu.sHtML

[U06] Py：合并两个字典
来源：http://3g.fehbvm.com/Article/details/gongibzqv.sHtML

{**a, **b}
来源：http://blog.fehbvm.com/Article/details/glznhkzco.sHtML

[U07] Py：反转字典键值
来源：http://baike.fehbvm.com/Article/details/gdrfqfwzw.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fehbvm.com/Article/details/gdhgkmqfs.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.zdbjq.cn/Article/details/gjswmoifh.sHtML

[y for x in nested for y in x]
来源：http://m.share.fehbvm.com/Article/details/gxtavyhma.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.hesvh.cn/Article/details/gvpmswumh.sHtML

max(d, key=d.get)
来源：http://wap.hesvh.cn/Article/details/gxgwqkbix.sHtML

[U10] Py：按值排序字典
来源：http://wap.hesvh.cn/Article/details/gtvacmaia.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.fehbvm.com/Article/details/gbnhcehnw.sHtML

[U11] Py：生成器表达式
来源：http://3g.hesvh.cn/Article/details/gmvnhlybz.sHtML

(x * 2 for x in arr)
来源：http://www.blog.zdbjq.cn/Article/details/gxturglqs.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.zdbjq.cn/Article/details/gcpogfztf.sHtML

Counter(arr).most_common(3)
来源：http://baike.zdbjq.cn/Article/details/gjezltzry.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.zdbjq.cn/Article/details/ggylovhpk.sHtML

deque(maxlen=10)
来源：http://wap.zdbjq.cn/Article/details/gnrbyqrmo.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.hesvh.cn/Article/details/gxgisgxdr.sHtML

defaultdict(list)
来源：http://blog.zdbjq.cn/Article/details/gmggdwwwi.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.fehbvm.com/Article/details/gsgaiueih.sHtML

t = time.perf_counter()
来源：http://mobile.hesvh.cn/Article/details/guweajgpp.sHtML

[U16] Py：命令行参数解析
来源：http://wap.hesvh.cn/Article/details/gknqdxzkh.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.fehbvm.com/Article/details/gqnvavkgo.sHtML

[U17] Py：初始化日志
来源：http://3g.hesvh.cn/Article/details/gqouuxpya.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.fehbvm.com/Article/details/gdpiazpcx.sHtML

[U18] Py：预编译正则
来源：http://www.blog.fehbvm.com/Article/details/gxqpxlmav.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.zdbjq.cn/Article/details/gcgoskdio.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.hesvh.cn/Article/details/ghrcxhsmj.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.fehbvm.com/Article/details/geuptgbsy.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.fehbvm.com/Article/details/gpcjnkpcz.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.hesvh.cn/Article/details/glvmowhvy.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.zdbjq.cn/Article/details/gcecogbbj.sHtML

@contextlib.contextmanager
来源：http://wap.zdbjq.cn/Article/details/giabicjhg.sHtML

[U22] Py：矩阵转置
来源：http://mobile.zdbjq.cn/Article/details/gbecgvffm.sHtML

list(zip(*m))
来源：http://m.share.hesvh.cn/Article/details/gxolamwtx.sHtML

[U23] Py：分块读取大文件
来源：http://3g.zdbjq.cn/Article/details/gvdqzaxpl.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.zdbjq.cn/Article/details/gugpccumx.sHtML

[U24] Py：路径操作
来源：http://blog.hesvh.cn/Article/details/gxlrtmjoa.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.fehbvm.com/Article/details/gevprmpwe.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.zdbjq.cn/Article/details/gqxgtmtjk.sHtML

csv.DictReader(f)
来源：http://www.m.share.fehbvm.com/Article/details/gijtqpzxv.sHtML

[U26] Py：并发下载
来源：http://blog.fehbvm.com/Article/details/gpkzchbjy.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.zdbjq.cn/Article/details/gxuqwohjp.sHtML

[U27] Py：异步 HTTP
来源：http://blog.fehbvm.com/Article/details/gjyswvlbs.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.zdbjq.cn/Article/details/glclryyhy.sHtML

[U28] Py：类型别名
来源：http://baike.fehbvm.com/Article/details/glktsyrxk.sHtML

UserId = int
来源：http://www.blog.hesvh.cn/Article/details/gmxqguqkg.sHtML

[U29] Py：属性校验
来源：http://www.m.share.hesvh.cn/Article/details/gekywmfuj.sHtML

@property 与 @x.setter 配合
来源：http://3g.hesvh.cn/Article/details/gbgpjzjdj.sHtML

[U30] Py：数据类
来源：http://www.share.zdbjq.cn/Article/details/grincgges.sHtML

@dataclass(slots=True)
来源：http://3g.fehbvm.com/Article/details/gadoxdlbc.sHtML

[U31] Py：单测
来源：http://blog.hesvh.cn/Article/details/gljxbszdm.sHtML

python -m pytest -q
来源：http://m.share.zdbjq.cn/Article/details/goedvucmh.sHtML

[U32] Py：代码格式化
来源：http://www.blog.zdbjq.cn/Article/details/gqcrxspei.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.zdbjq.cn/Article/details/ggtkdskac.sHtML

[U33] Py：打包发布
来源：http://www.blog.hesvh.cn/Article/details/gzgdrlqfo.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.zdbjq.cn/Article/details/gvelbdrgo.sHtML

[U34] Py：判断编码
来源：http://m.share.fehbvm.com/Article/details/guhihssbm.sHtML

chardet.detect(raw)
来源：http://read.share.hesvh.cn/Article/details/gnlgykdde.sHtML

[U35] Py：发送邮件
来源：http://mobile.hesvh.cn/Article/details/geogsnhnf.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.fehbvm.com/Article/details/gwdibbmuz.sHtML

[U36] Py：定时任务
来源：http://www.blog.hesvh.cn/Article/details/gleckxafk.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.zdbjq.cn/Article/details/glzrdjrzl.sHtML

[U37] Py：读写 Excel
来源：http://blog.hesvh.cn/Article/details/guerxvizd.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.fehbvm.com/Article/details/gjronpczs.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.zdbjq.cn/Article/details/gcpkrefjf.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.zdbjq.cn/Article/details/gcxsgodzl.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.hesvh.cn/Article/details/gtpzkgqyr.sHtML

sys.stdout.isatty()
来源：http://www.m.share.zdbjq.cn/Article/details/gwnnbqdnb.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.zdbjq.cn/Article/details/grohdwyoe.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.hesvh.cn/Article/details/glixjgxvb.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.hesvh.cn/Article/details/gmcshwfse.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.hesvh.cn/Article/details/gmyuoeqpa.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.zdbjq.cn/Article/details/gcnjqsuuj.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.zdbjq.cn/Article/details/ggkcuktzo.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.zdbjq.cn/Article/details/geerbmrbi.sHtML

namespace App\Http;
来源：http://wap.hesvh.cn/Article/details/grubtigug.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.hesvh.cn/Article/details/gtheyzumk.sHtML

declare(strict_types=1);
来源：http://www.share.zdbjq.cn/Article/details/gbhuycfpq.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.zdbjq.cn/Article/details/gfiuflmdk.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gvawggdlf.sHtML

[U46] PHP：可空类型
来源：http://blog.fehbvm.com/Article/details/gdjygjkjx.sHtML

?string $name = null
来源：http://m.share.zdbjq.cn/Article/details/gexgbxyew.sHtML

[U47] PHP：联合类型
来源：http://www.blog.hesvh.cn/Article/details/gvhjtghad.sHtML

int|string $id
来源：http://read.share.fehbvm.com/Article/details/ghqxjbdhy.sHtML

[U48] PHP：纯枚举
来源：http://www.share.zdbjq.cn/Article/details/goalkwokk.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.fehbvm.com/Article/details/gdfrxwfjs.sHtML

[U49] PHP：只读属性
来源：http://3g.fehbvm.com/Article/details/gnxngtzuo.sHtML

public readonly string $name
来源：http://read.share.hesvh.cn/Article/details/gpxehyztd.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.hesvh.cn/Article/details/gdwlocjwi.sHtML

public function __construct(private int $id) {}
来源：http://www.share.zdbjq.cn/Article/details/gdoseptue.sHtML

[U51] PHP：数组解构
来源：http://m.share.hesvh.cn/Article/details/gzcftyaxa.sHtML

[$a, $b] = $arr;
来源：http://mobile.zdbjq.cn/Article/details/glgnzmtrv.sHtML

[U52] PHP：箭头函数
来源：http://read.share.hesvh.cn/Article/details/gemdgdzwa.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.hesvh.cn/Article/details/gukyagngy.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.zdbjq.cn/Article/details/guuvmamzj.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.zdbjq.cn/Article/details/gztkmuqhf.sHtML

[U54] PHP：空安全调用
来源：http://www.share.fehbvm.com/Article/details/gqfceubqf.sHtML

$obj?->method()
来源：http://wap.zdbjq.cn/Article/details/grenpvnyn.sHtML

[U55] PHP：match 表达式
来源：http://3g.zdbjq.cn/Article/details/gdxfydddg.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.fehbvm.com/Article/details/glneownhl.sHtML

[U56] PHP：命名参数
来源：http://m.share.zdbjq.cn/Article/details/ghhujekgp.sHtML

f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/gexpzifyw.sHtML

[U57] PHP：字符串插值
来源：http://3g.fehbvm.com/Article/details/glchihkzf.sHtML

"值: {$a}"
来源：http://www.blog.hesvh.cn/Article/details/grhpykygb.sHtML

[U58] PHP：数组三件套
来源：http://m.share.zdbjq.cn/Article/details/gtxgmhwfg.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.zdbjq.cn/Article/details/gmflifxjp.sHtML

[U59] PHP：自定义排序
来源：http://www.share.zdbjq.cn/Article/details/gizqcbney.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.hesvh.cn/Article/details/glefkzixx.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.zdbjq.cn/Article/details/gbpeuwwrm.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.zdbjq.cn/Article/details/gtfspnltw.sHtML

[U61] PHP：正则
来源：http://3g.fehbvm.com/Article/details/gszkhslsv.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.hesvh.cn/Article/details/gezjmxngf.sHtML

[U62] PHP：日期对象
来源：http://3g.zdbjq.cn/Article/details/gpivdewux.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.zdbjq.cn/Article/details/gbbteiiwh.sHtML

[U63] PHP：文件读写
来源：http://read.share.hesvh.cn/Article/details/gmzhhgxqd.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.fehbvm.com/Article/details/glccuzgxl.sHtML

[U64] PHP：目录遍历
来源：http://m.share.zdbjq.cn/Article/details/gjlowbzoo.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.fehbvm.com/Article/details/gqrdbpvyw.sHtML


<!-- 参考信息 -->