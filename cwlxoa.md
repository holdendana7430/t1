代发 wailian999

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3gdczovbz.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3ubckhlhg.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3hslzwlge.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3eltmpcwq.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3hfmmtsmh.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3hrscgdgv.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3uopbflsa.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3sujhxdzl.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3bqngqygx.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3ziqhissc.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3tlfftkgo.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3rnaipmgc.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3tddjvlgj.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3doexhpvq.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3iflpiocy.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vjvjwvfl.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hgdzrigl.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3mqqsrgut.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3oojbsfwp.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3ylbufszf.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3tolfwgoq.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3wjivcyah.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3ubhslusv.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3wxqvylpv.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3fggspnyy.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3owugtmin.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3gjximbmx.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3bnaaighf.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3aqevdtrs.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3yyjxsoue.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3kntrjxdi.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3flzgeaql.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3zqahiezx.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3oompaidx.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3qmqcwinb.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3shsurmlo.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3rlhzgojz.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3kgcgfxcb.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3tqbpmyer.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3xhkqmorv.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3cunggptq.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3cbftqrtb.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3amjblnou.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3wncapyfz.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3birpahml.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rguuiogd.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3afouccwd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hzahmfqm.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3qcazghew.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3pheuirta.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3lzzfhwih.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3yrypurae.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3chxvcolw.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3osmdajno.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3xleevjks.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3ndgumzro.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3fsunkcmr.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3skelrifd.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3ybgwytfl.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3rwaensvv.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3tcbiuwwa.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3mrqayleh.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3zjbmqxdb.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3maxezgxi.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3oyxnuxri.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3moxdyhki.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3mduhvtiw.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3lydilbkf.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3wcrttrtd.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3uxwysyyi.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3iwynzdcm.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3eqwtxyxg.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3zcwzoihl.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3uacxiqqg.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3nhyyvvpp.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3pokkmjwt.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3clxzhvth.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3dvknpfrx.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3adfbzrhu.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3aruallep.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3oucpqief.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3faxqcgzu.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ldptfwgx.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3hoodiwdx.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3mipenalz.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3rpiewgtk.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3vgarzuvb.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3bimgzqrp.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3wtwzortu.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3ntfvicyp.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3elfrgsuk.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ojhikdcu.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ufaytbjq.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3pvuolxst.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3ledxapje.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3tgmydwzf.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3bkgzgvyg.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3epxymhpg.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3ptntcszm.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3bbaewped.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3videfudy.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3zhlfnmaw.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3xqfuvkfz.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3qzktxpzv.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3mxmzucea.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3mjckbsii.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3woprxnwr.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3ksoemzbf.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3bjovrjwa.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3umkmcicv.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3iedzrtfn.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3xatfeoxv.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3dwzlgein.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3gqlguesf.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3fkdmoons.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3fbbadnlp.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3jxalfwhn.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3ithpwbha.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3llhizkvf.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3neyibdlr.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3vnwuzqsk.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3regcmwus.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3wmqlyzon.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3tncwukjp.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3gljifzub.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3blvwlnqq.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3bmovdyqw.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3jjdofsrn.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xnyjnaav.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3wgsndyjg.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3zaflwfuz.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3bbzoxsnn.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ipviduin.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3lhywnzvu.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3mupsjoyf.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3cjldbita.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3uebqomhc.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3wilswgcy.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3ygjzarex.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3ermtwyuj.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3oopducmp.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3ivhrujwp.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3tvschuar.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3ntpipunj.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3pylqfcls.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bivpeyct.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3syiftewu.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3gvaxkgyl.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3mtsoxswc.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3nzheiabo.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3nklgxeml.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3uabdbkau.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3jeguoezs.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3mqhazmay.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3aufhfvvt.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3gfobbbja.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3tpglpsrd.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3vrkqidso.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qfrfhsdf.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3xipxstpj.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3yvyssgcu.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3hqqdqoxm.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3hrjrdtoh.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3qpsdqpdg.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3uzeaszvt.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3sznifhpr.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3kdgrwszy.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3fonimfyy.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3lhwqqiux.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lvlhvmqq.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3qsukqmmw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zlvkbzlp.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3clwvxiak.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3qjcyjdta.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3bsfekkci.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3laameeah.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3pafpfxev.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3ijghazze.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3pfgqahhs.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3yahwhhgv.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3grqbsivn.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3echxhfhz.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3ahflevfo.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3fvptobda.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3vqsdfevb.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3gspfrhyv.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3huuavmad.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3susezqgq.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3dklrrdfe.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3mhccxinn.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3oilrbivp.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3efaeigky.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ezaiolpt.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wjaecngu.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3qsdkhcxm.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3qqapsbff.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3zstorwdk.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3kbgiuevm.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3vlwdywrr.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3ivpdaytc.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3uceckioj.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3hvlonwmv.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3dvgyqtfs.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3rbshuoav.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3vahhjvst.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3tpunjpmy.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3umehecjw.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3znewmzeh.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3rwdtrsgz.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3lyzoliqu.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3osqxxrob.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3xgawnnsk.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3aouikvau.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3uainmmmi.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3hgtffjic.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3fqgubfxu.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3newtwgop.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3pvokqviq.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3tqrqmrdy.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3wrfiarsu.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3yvdechob.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3ecmisdat.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3pogjxldd.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3irpqdnvk.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3chggbsju.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3pijqowom.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3vpmqswlk.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3okzlfxlg.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3gghmreau.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3ghfynnsd.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3vnpmoeca.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3nqvgkqts.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3tctwbwam.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3ccoxocff.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3niihsrie.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3gnalrzwh.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3rawtjurx.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3rmvlhluz.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3kixijcjr.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3lqjqdfrl.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3omeoctsr.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3pzqbhpfs.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3rtmsngli.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3mspzidmw.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3acrfijoh.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3gxiqqxbi.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3tbsppmjo.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3cwpstkkv.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3tkfetuhu.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3vfubbaok.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3qdjjhtzt.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3kpjlrygc.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3sgbtgkww.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3brxqprrg.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3mccekhml.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3szzvculj.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3bcedqupn.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3wrayatxt.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3rxnspzlz.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3hoahfwba.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3utolbbov.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3efoegpmi.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3bfrpsqaw.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3nhztkebc.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3pmgvscih.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3iehyqopi.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3vbheldwz.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3efvcpfih.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3dtvjauzj.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3ipmnekew.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3gadoswga.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3dgglenyo.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3mebiwxdn.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3wjunsbkd.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3rackcesf.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3tcnbtimm.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3motsfjcw.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3gtctynta.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3rxeshofn.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3spmiguxz.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3imgmmhrf.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3ojbjmxeb.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3wnguqvvv.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3elvqaido.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3wqkoxivm.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3fqmxubvx.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3pmauoxbf.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3svhtwzjf.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3szymimcb.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3mrvswrgm.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3rvxtpped.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3kdahwtxv.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3ridtolyn.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3eodrstdb.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3tmafcatt.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3trxcppgq.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3cozgoncf.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3jrxkahoe.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3jvfefqfg.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3eznrprdc.html


<!-- 参考信息 -->