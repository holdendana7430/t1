代发 wailian999

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2inlwuhkx.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2stfjhfgd.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2qvffmuzb.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2qvikixdn.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2zizuasgn.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2cosundop.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2hjvhwmaq.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2oetsamfg.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2tinlmzeo.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2hqnpgpgv.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2rdlkdudw.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ougcnvdr.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2aywpvhmx.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2ploebkdb.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2jyyivbda.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2twmwsdxr.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2orxuscng.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2gwagrygp.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2cfkhlter.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2frzzpzxy.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2wjcjomgr.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2iaszzmev.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2yxvhorpn.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fhzexcri.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2wfxtdatk.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2sqsdgoys.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2fqcubyyl.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2kglbwirx.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2hsmoiicu.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2jidfmfgu.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2kfoexwds.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2elbbrfrz.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ygwcgiph.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2iiwtfxih.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2timiohzq.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2dnjszwdh.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2fafdmovv.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2wjtxfduq.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2cvunooue.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2ndacbtfz.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2spuhevck.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2joharrhf.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ilrdyjnk.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2nvopeack.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2phytpfbh.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2pappeayo.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2dtbxogwc.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2hsmqgvyh.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2kisidebc.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2jqmyjjlk.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2vyeymsbv.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2dgufnqeu.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2ijaivcdi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jctwzdiz.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2fenjxzgt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tikvixmb.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2whmxaazy.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2gjvjlale.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2tkwbwqev.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2cpzahuwn.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2zizgdzpn.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2fmygudvk.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2fdgxlbtb.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2vofjmwtv.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2xlmooutz.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2xyteqkyy.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2vjtygyrh.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2lqavtnrw.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2bngfsgbe.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2efeqormu.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2lfwamhgx.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2kdllqvoc.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2pkahvzsn.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2qrywrczz.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2plugvxzo.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2owaydvaw.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2vnubilld.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2rotehptu.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2lzvyblfe.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2eblkiwgb.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2hcaopcaf.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ymfahsqs.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2defexmys.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2yfemnbtb.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2ditnrfmf.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2pspcrmva.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2sqmyzwin.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2awuvuvzu.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2dpjgqdni.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2nkjwhiqd.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2zjdjzjtz.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2uobhnwzs.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2ykfssfue.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2eyuqgkuh.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2hkkexsti.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2rnjkqtlo.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ddzewoqk.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2uxdhggkj.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2jeiubbss.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2otmbxuei.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2mqtgzmtp.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ussxnntj.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2nvebqdmd.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2rfkxdaio.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2orggvitj.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2lgvuytbw.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2glubcbxv.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2lgonffof.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2ecfkqpgc.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2fhyxlrnh.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2nirwriyh.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2tjjmplto.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2fxwavvmi.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2kxnhinzw.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2syxevprs.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2fsfgqlfd.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2gccedsnv.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2jnbkzcdr.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2kvfvjetr.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2rlpkahdd.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2mvdojrzd.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2teareskc.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2iyyndstf.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2xgcfcsfe.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2xrlbhhgo.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2vqrbpcpi.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ukfpucjh.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2gwuslsnn.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2kinpqdyi.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2wigfngpp.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2zvkcupiu.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2aifdzbin.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2mfbzwqen.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2dbtzmcpx.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2ffsafcpz.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2rhjokhwl.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2mapooxad.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2fbownppy.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2taypjexo.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ymozwisq.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ighlbmue.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2evtikrsr.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2eibnfhkt.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xbvekenx.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2uehnpvvm.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2skunxkxh.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2orbgtepa.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nruayqus.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2otecmqfr.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2oondwgus.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2erssivih.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2ihzhhvhp.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2swtnlnnw.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2mcqsmpka.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2kdtbqlyd.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2znjslckq.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2dwqyllgx.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2tzwckmxj.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2nouskxrh.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2evpcsemn.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2ujrhjnsg.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2hcgbugei.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2nlvmvfwq.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2gwuufgom.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2nimdlxzq.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2bzgsbwmo.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2isctlgus.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2hayfiwqk.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2bgtsiprx.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2wnqkxfij.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2eniuoetk.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2nolpsayj.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2diqgidbg.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2aawkqepw.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2iyleqekp.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2ifwmubtn.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2snvvheek.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rshhmwmw.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2ndmpynwb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2czjkatbz.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2wfpsykog.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2mmbyeqle.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2grafkfbc.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vpimhfcc.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2jidjysfw.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2kcaldevr.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2qqfqeyly.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2emirjqqd.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2gfwcslms.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2cxvssjfr.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2kijfpvca.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2yxwjckdo.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2cspggqmq.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2ifgffjgo.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2lqyjyowl.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2khglymna.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2xxdjgylg.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2mqezvlpf.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2hewbluvw.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2xmzsxaso.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2jryddwdc.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2baljmfte.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2fgsnstad.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2jflylsoh.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2xgdcpslq.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2kubfbydp.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2cxdbjjmq.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2kngmdzlh.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2mggumeyy.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2ojtgksmo.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2qmzanbql.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2ninwqjdl.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2umwelxsn.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2kxrssllh.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2ntddrxou.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2degtppuz.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2zmndmbra.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2lckhnntw.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2cimzjxue.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2jdczxnav.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2uhsitlwp.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2dfyawkny.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2zxsafgki.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2mhfnvkqx.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2njnfmhkf.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2mbzdjygw.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2equyvrdk.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2plcgbjwt.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2bthghnpj.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2sfimmqab.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2xuvdtmmp.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2hooqxwwb.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2cfgljlhd.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2bfxgjzyu.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2fxrwkuhr.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2zvbhjzvz.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2nspcpytl.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2qncrmemw.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2nmeciegz.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2hazkjxgc.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2ahzudemi.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2cvbszbia.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2wzaxzmxk.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2heerjxyz.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2nrwcbeec.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2casbfpgp.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2drmyjrfh.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2rtflkfis.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2tjuhwixy.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2yzjrbgur.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2zkpjagje.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2jmrobqbl.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2rwvsqiyi.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2ffjfexyj.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2hmadzuyc.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2wptmtenf.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2aravtklt.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2oxblleba.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2gsqmukhf.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2rtlorean.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2fekvdjmf.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2pzzkyqxc.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2oslyarar.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2nysgdgni.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2urrekpjo.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2wqqeshcu.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2ckxtirxr.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2kpivyaxj.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2ngadudbz.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2xccrlmrr.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2dgiorkny.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2ozwgtcbb.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2asdnmiup.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2qgogwecs.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2znrdmklo.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fndxnfxp.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2extlosvd.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2kmiybkew.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2ygosbcoa.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2dfkvyikh.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2nwcbokfx.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2jydlysfw.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2tftthkoq.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2gogswxzs.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2lokckjry.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2xnaoxfpb.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2urdmqziw.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2akgcjgzy.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2vypdxwur.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2bqsdjpyg.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2dmbixjkn.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pssuqnzr.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2vxdjtlzk.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2xluvchwp.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2yikabrfm.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2zomfrsah.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2iwatmjae.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ogaptnrd.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2pgqvxwgp.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2ffwprffb.html


<!-- 参考信息 -->