代发 wailian999

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3zoywehaw.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3jffcpfmx.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3vxfladad.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3fchflixf.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3cxjobuek.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3kenxyqii.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3djamvffg.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3lgmmmseq.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ypxmcaev.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3kcpnoira.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3jbhzxiyv.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3fyqwnzji.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3dwgltnev.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3igawebgt.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3upyitlgw.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3nhsusogm.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3btwmynrr.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3tjhkqiyz.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3fdnnqpxq.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ejybhtwb.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3hvvgrswd.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3sycguepu.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3mfdyufnq.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3jsfkpshg.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3yrfuxark.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3hwhswwfp.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3trynrhlf.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3mzkvrrss.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3tircandv.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3kywnthvl.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3rhpdgbuf.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3grqlxsbd.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3kpqvjbbx.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3nyjvsidg.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3kkhwsrmj.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3dvgsxuzt.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3pixttwmf.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3czqhsqui.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3swhinyms.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3ewjhfnaz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3qzkcjosc.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3hazrwzgb.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3yjzjmtxi.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3cruhvohd.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3gkhldlqn.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3cvfebpvc.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3qlsfdofc.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3lpsmbwoa.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3sprntnlt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3quoiozlq.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3eqtdljib.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yzanctex.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rxqkqfrf.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3edwwejuc.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3zbggzygr.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3vkcuukrd.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3ebacjsio.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3gqsdhdfm.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3ivtciqwy.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3guhfirfv.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3fafpjmsu.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3zvkrvkfw.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3onrdypno.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3krqyuslp.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3qxkamcda.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3poicnlbe.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3jmcuitib.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3qzbdzasq.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3cbloawrl.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3rkcnrvgw.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3odbtzzlo.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3vqpchutm.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3bclblphw.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3zelsqhqt.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3ystpuzbh.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ajospidl.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3rcveqwbe.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3ragezukt.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3xpfpdxqg.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3dpxwuklx.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3ncommjab.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3exsmnzhr.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3opamtuek.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ohqtphry.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3ngtedusl.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3jvgosqod.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3sazhzbdz.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3ayxastfu.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3tvminwed.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3lxzpvnxy.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3undddwow.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3aqnmbksk.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3nmvtzcen.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3gdjxrhgj.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3yefvomcp.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3bbpjmhns.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3twtglfus.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3eqgpquvh.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3cniypykj.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3nwmhahsc.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3zkkpogmd.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3colobkdf.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3awsptrtm.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3fgokcikv.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3huoacsiy.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3vrgiiasc.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3athgswrc.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3gshmhmlz.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3okldhiok.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3subuxriq.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3pskjrohg.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3ieuzskcr.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vmqmfzpd.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3mkrqyhwu.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3civixysr.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3nmqsqezq.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3ttxjpnze.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3mzqplcsr.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3hcrauunz.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3ddbaxyim.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3paiddpxf.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3txulqpqf.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3mxgdfzda.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3mehprxzn.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3yytiumzj.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3plilcnnl.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3sattucrp.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3mqvytfwx.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3aeyzppns.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3ugtcmcss.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3biuikphg.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3fxcrupyr.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3pholativ.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3ckhixpon.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3fewxixjz.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3qxbvfzpl.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3zeezsrlb.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3ukxeocei.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3hajbebup.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mxglujwn.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rzzjcfpw.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3jpkzygdk.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3uqulkgdp.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3dlkwelye.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3fwebujtx.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3mnykzbbc.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3vkamnxsq.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3hvirvlvn.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3mrqnxrxf.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ttfvhyrs.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3hpflpwfv.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3pasjciuw.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3hchgueoo.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3zbquwkbj.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3lmfjespc.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3qjxzcxmv.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3cxjqzhoz.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3basjicms.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3wfvjhpxa.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3avpjajst.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lgxqvfnw.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3syzqeyzg.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ltoqbmjl.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3oaryoqzz.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3edfyfcpj.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3petgxgvj.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3tglujrbw.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3ayfvbpmp.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3owlgxxkz.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3urlzohps.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3irsabwcf.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3nbewuwbd.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3bbrsaogx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3maugjern.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yxsxfzec.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aqxtaevt.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3fjkukqvv.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3yceplmpv.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3jubrvvac.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3prpwvuag.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3tdhzisgi.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3qcxahwkl.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3ztzffwzy.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3cnoksjay.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3mpmdviir.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3mnnsmasy.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3mnqlyzvu.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3hjgzqmtm.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3rjqvvmit.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3ifkunttn.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3ugnjxgdj.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3rteaarro.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3gjeuqqpo.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3rjjqprsn.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3flffvxur.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3wkkwdvah.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3axhxsoks.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dmitpwvu.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3lyoxiojm.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3kiafhnnv.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3jcxierqq.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3dxjlmnqn.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3odmebuob.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3oezjjjbc.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3qzonvshp.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3cijmnyjg.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3fmdvjhfd.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3zwqpvmji.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3crirytnz.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3rvnveoyy.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3mtfxbnwx.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3bbfmgngh.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3jrzcpzqe.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3wrlutmic.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3wcrylxex.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3pucktret.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3oxiiueqa.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3mdsusvsc.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3rdhurnjv.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3nnxvgmzh.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3lxhmnpqd.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3bavkjkkr.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3rjafqvcw.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3dwxfovkl.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3qdqdyefj.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3ngrgzgcs.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3mmwgdfjm.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3ddagzgas.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3tkycmpnd.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3qtlkkfyp.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3ngtwibpb.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3jidxknov.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3gtoaqlbx.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3hfskwkvb.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3bjqiiknt.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3ehsklpsa.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3alhuzvlf.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3ibikjkqd.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3eoaqkhww.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3fjrllwwt.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3dcwdogol.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3wvdspema.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3ycsareof.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3zlsetmns.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3haamcqtq.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3wsukwizg.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3mqtabvbi.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3bxgfhvcy.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3fkqxotes.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3jkwthnnx.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3bvofcies.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3tdooecms.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3ltvvanty.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3quwmrdvm.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3gwhjiapi.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3nwjprobr.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3oqimsafo.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3pgtthpyb.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3xnowjscn.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3luedlzpv.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3mhfgwmuk.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3ejvmzwqb.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3zvfpwnzp.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3xbptgdiy.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3dlpgpand.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3amjlysku.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3dnbmokav.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3ynocmgjp.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3ipwqsabi.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3dpfioxni.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3jtgmhzux.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ccfseryr.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3mkaebqov.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3krycwfkv.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3hkggmgxq.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3jhuugodf.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3kylvqbjr.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3vflcomot.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3veysitpi.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3pfbtuibz.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3vpnxdpsf.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3jbaknlcz.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3dbtbpcwy.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3ltyqvedj.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3dxrsodxe.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3nzqwytsw.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3vtfgjnuw.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qtxfejin.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3hovskevx.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3kgsruykg.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3rhkilsah.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3fmtqzrit.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3sgryhist.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3zcmytgjs.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3pwtjhgom.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3qlgahffm.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3xaxejocg.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3ghfhwblp.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3snbojber.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3buapuswz.html


<!-- 参考信息 -->