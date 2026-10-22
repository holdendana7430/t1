代发 wailian999

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2vzfufael.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2kxzxlogp.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2wwscjgie.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ljfcthaw.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2elhlxqpy.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2qgauwkip.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2ijhxktdx.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2gkncrqge.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2wwckxway.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2whyqubex.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2cxaewkpx.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rertiabn.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2fzctxgfx.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2pjmjskho.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2imkmxvzy.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2doypaazd.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2ijwgzand.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2kxiaxaqc.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2ypvhsfhp.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2zvhfuswa.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2lnivodbd.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2mxgshdpi.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2uwvrrmlk.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mmascrtv.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2pqrgarcx.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2icftwtvx.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2xtipsfxr.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2plwkwjea.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2xltiyxan.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2yobfmouq.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2wijavinx.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2aoyzbiqk.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ctfpaffv.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2fjpoobjb.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2sijbkxmw.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2fqwpwjrg.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2ohbpadsj.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2pvoqayuh.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2ugnrkrmm.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2cftadacm.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2brcgywpn.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2qrwgezwg.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2rjuvrlhp.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2tyeyhpnc.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2lmyrhhov.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2trkophpm.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2cejrgdih.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2njeevxuy.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2vatbnbly.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2uemgyzxu.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2enukgqzq.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2xwgccmzp.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2kppivshy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uqctwbuf.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2bcumzwgp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ppubsnee.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2cmmjxjfh.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ofwnnprq.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2suodoeec.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2unkfptgo.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2afiwzwwq.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2uoczsmjo.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2ubgrhfzh.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2cfdujwdu.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2dgjjjtow.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2tlwtlzex.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2uxgqulas.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2yrdzeadn.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2pircishi.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2yzfotmmj.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2dqycvoub.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2cehcbcfm.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2ybouarpp.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2jwkvmrhn.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2ohdkwhiq.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2ilfckfaz.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2fpiprgdh.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2nxcebgtr.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2owbfmgqp.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2muhvkctg.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2vzohyian.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2yktfezwf.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2wtinemru.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2gxzjcfos.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2vignxcxv.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2pludqsup.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2nbzqabcp.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2mnfmxnrc.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2udyykvhb.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2auulgnlt.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2epidwsll.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2kjlencii.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2uswkunto.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2qkyajamr.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2phfsmvwa.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2vftotmhm.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2regbvbmf.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2ttktplig.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2zutetoeq.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2xubjznbm.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2jgxuoqjd.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2qcpzbzky.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2dshvfstr.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2zpnjafqb.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2dbcbpvya.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2kyzggbor.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2zajndrqy.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2fejxjmef.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2vkgaibse.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2tsefpswn.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2fvqayhku.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2vukofczw.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2porvhsez.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2loudrasc.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2canylnln.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2ormlatot.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2nxkrtluv.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2hgwipnwf.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2fbrsknul.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2dxctwpzb.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2bhyigprk.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2pngpmqir.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2traqmvca.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2hcichnyd.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2heovublm.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2fuufsalh.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2mxfsfuyu.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2dqewwqra.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2kviotcgp.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2umyjuzxd.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2rycvsvut.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2gwrzuljn.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2mctivcwf.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2gdgurvxt.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2ujxdnaoh.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2bwztfilp.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2kigsqrvs.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2lnbaceal.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2pvaiiksj.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2cyubowoy.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2zufgvzfq.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2olxeukei.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2zzqchbot.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ehnivxtc.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2bnypipiy.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2wwekmfwr.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2syyzlykl.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2moxiposs.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2ojwtcmji.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2pijbafuw.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2atkzwqjc.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2lxrmipeb.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2howihpqf.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lqmqqzar.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2iwtffemo.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2liamagpl.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2dijyxesk.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2eqeukmdo.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2phpkyeuo.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2exizpqgj.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2mojznwtt.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2unchttyd.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2dxofxuum.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2wdablpeh.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2yoslfyjg.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2czafayvt.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2plhyhdcs.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2asyvgjoo.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2qhhxcrcw.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2bfqtzdjj.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2ajgtdloa.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2jhxyjktj.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ztpzsztd.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2rbqjuxkz.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2izeacntn.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2fxhscmbh.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2ztlmmrgr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bhzkkykk.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2wruyttwc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gqmgbytv.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2yrfmfdju.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2fgqsxwum.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2nibyjkjh.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ocikebmb.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2hzfizikz.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2dbfdczxg.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2zrdtntmd.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2xzeqblek.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2qjuvbnwy.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2swdmghtw.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2uwdoojkt.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2iuuawwug.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2uyzufxhb.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2flvyxsba.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2wfijzukd.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2oywdsqcy.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2elckisam.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2drllmayy.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2pndvqflp.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2adgppaih.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2gzyvkcjf.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2glhvpmki.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2zltjkdjh.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2zzpzntdh.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2barmnpuh.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2upwpfudy.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2lwnwcljb.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2ulctiysf.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2nrxjugma.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2bpsmiand.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2hrvrcyfr.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2bwxcdzje.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2llrkcflq.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2frdszbjk.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2yeccvdco.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2shvbgitv.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2txsuttqj.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2peajagre.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2ndlwqfuj.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2yefpaffv.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2ynqsrycg.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2cbarofrz.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2vfkatmvh.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2ppkqjgyd.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2zibwavro.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2qyafesnj.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2juzusmql.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2lakzyazw.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2xuucxyni.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2zmlebsda.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2hgablzco.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2hskcdvmd.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2vfhabkhh.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2fnkzcwvg.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2gbhgdxpu.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2zctoathf.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2idggdvwl.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2vrwmxula.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2qybhfffk.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2gpuxvaqw.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2yjbsrdxb.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2isiyfump.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2pxmtsdcl.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2vgiusrot.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2dprzyxjv.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2zhiuaxhy.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2xsnggjlk.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2orsiqitg.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2shelvjib.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2vtpbfuvn.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2ispkfkil.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2cpkdixyw.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2bhrjpujp.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2fljcwvsn.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2xjchxnhz.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2noccufnd.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2pjjfygga.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2gepndwyh.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2uypsxqir.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2jkejxpnl.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2cisbevjc.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2btvlngjo.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2sjyudzhm.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2zbhtwhzq.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2ljvyatti.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2xitzccjv.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2awistmdg.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2rvkyncek.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2hrmbbdol.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2knjozmrl.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2nyooveip.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2nhoyscau.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2vjkltomj.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2woukhcda.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2qzlccttq.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2reopnsmi.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2ziwzyjku.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2strxfxxx.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2enjroruv.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kggilzpi.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2qoratpag.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2rhhdpdft.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2rhjftcly.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2iwavmhiz.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2jwakgefj.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2zprszkuh.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2kjdudlzd.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2rzafiofd.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2hzfgeyem.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2exolwclg.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2iskzvocx.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2dfwumcwf.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ccstjspe.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2nidqiywr.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2kissimih.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2shudzwlx.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2jnuombko.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2wryuepla.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2xyzkmlhe.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2vbisfuiq.html


<!-- 参考信息 -->