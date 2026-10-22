代发 wailian999

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2budfjywi.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2ptwcmypz.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2fxompqxf.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2jgrtbpbt.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2glbhzrzf.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2ykevdudx.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2tlcqjdza.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ykicvcwt.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2pchhuzje.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ykmpifem.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2gjnfgyru.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2xkxyuomz.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2nzfyfdjs.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2genoddtv.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2vlvnytuv.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2bbvkxuga.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2lfwhegyi.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2nhuhrveu.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2ihwkmwcd.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ibjmvftb.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2wrmkvdmo.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2imzokhgt.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2ddgsrljz.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2lkopycxj.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2qcerioyy.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2winpdbwg.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2nqvsykaq.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2rhyjwcwf.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2psvnggve.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2ivsffhdm.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2agfyflyl.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lhfiyhim.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2dizvwynh.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2afyyklso.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2zbpofyyh.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2snwtlhqe.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2kiytkzxy.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2ikqgohem.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2gsyhpnie.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2ltdvpxms.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2vjiyqmvq.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2cvzxhtcb.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2kjbuquza.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2liwvpyio.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2tuhwrrnc.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2vjuohfrs.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2sxzsjyeh.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2sujmxmoh.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2xiwyvqgd.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2margvpdh.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2fdzteddh.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2fmacjzgk.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2sodstfvc.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2rdwpmgww.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2bvgqeyru.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2srjnsyzm.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2pkoopkxm.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2wmqornhe.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2wnwmukzw.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2gmngcqoq.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2eulazawk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ckrjopal.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2gmegvqck.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zwnclrty.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2dowtblfb.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2eforcpzb.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2cnavdcpv.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2mcuauwss.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2doirkztq.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2vxnalxmg.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2gktkyrrg.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2tfdtffbn.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2coqrdqty.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2yzhzezgp.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2oqaaxtog.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2wojhuxfp.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2maxahzup.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2rwnamtmx.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2opysufqp.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2nuujypau.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2xpyttehz.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2pewyzmha.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2buyhkydy.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2gvoxrybm.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2dtdmthgq.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2vzbknkij.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2vmdbysvv.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2egdhrypc.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2kedpvlyb.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2glvmjygn.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2tkqbjkyo.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2irgpznsz.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2nzlgdhxc.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2syvtfmfi.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2zaqldtfm.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2pcxbzlwm.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2olztlkeb.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2sahrorpj.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2wcbppjvj.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2fxuimjwo.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2gxitufss.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2tuvsrhdi.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2ciqidnju.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2ewbhkdau.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2vhjjlgrj.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2hgukdnos.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2utttyveb.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2dblekmhn.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2lvanrgoa.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2tvzneowd.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2xtghkhsy.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2hlxeslhy.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2ywkzsuzt.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2chyqynar.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2yhiecdcu.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2nphkbqzw.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2euesyvfu.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2sqxprdru.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2aekrarkx.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2gjeqjqng.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2hdjdlmdf.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2zksceizk.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2iynntjss.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2daulbhcc.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2mpmtxnyn.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2jeuwpzuv.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2wnpgmqfy.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2tdpgfqiw.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2gfiqgrpt.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2csoxhuvj.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2quftqphk.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2kpvkjrld.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2lqydotsx.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2bkgkcyfj.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2fuywuazc.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2vbxsulcf.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2ylkjfmat.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2ilakqtbu.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2zkqmogmq.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2izkvbahu.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2vwcelbom.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2yxpdbmig.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2ymreqfkz.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2zfzmpdjm.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ifpijhzo.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2zymgicie.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2tngailsh.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2thwxvvgy.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2maubzywq.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2pzdldkzw.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2igykntlk.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2yolyptsj.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2igabarby.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2yaydztsf.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2tkagyrpp.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2rlvmnmoa.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2scidqobn.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2kkqrrkpn.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2icpsrrpm.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2fdletigk.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2dzcasovg.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2qzcbympz.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2jxahitig.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2ctznvsuj.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2mtxejnnw.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ezacnmol.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2vaazvqen.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2qmvqvjib.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2zcylwwnf.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2qaqdpmrv.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2cwpfalrg.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2mrbbwpkg.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gtdnvxfa.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2vysankei.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2otgextvb.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2ypeqdefi.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2dzayvwci.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2zirxzjuo.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2emptedhs.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2fhgjjoca.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2shvbieip.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2cgnuwpkt.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2juwzprwx.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2erxbufzr.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2kqomtzjx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2itjujpmc.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lamgqdpw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dcqaztgw.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2xwbtnlpa.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2unsgzhtj.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2xahkgdwo.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2kbdpqapz.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2lbrbiboe.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2estlsvod.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2isacntdw.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2mzuwvgaa.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2qhsaelfg.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2qxixudow.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2hdsiwapn.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2uuuuckgl.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2gdulujjr.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2jlkgzsfd.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2yixyaaov.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2wstctxxl.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2zayxwhol.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2bhlosuvu.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2qwjeyggr.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2jigpzyzv.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2fqaqgjaw.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2zhbkbfwz.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2bygqiyys.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ehfnczfk.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2jaftewur.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2sypqkdew.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2pawshvgv.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2jbnbopfy.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2mqkwgdvl.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2pzdondmx.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2emcseico.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2eymdylzu.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2slwzzmap.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2kfnfsckd.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2pxrudgod.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2napaplci.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2bygaxnjo.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2drfgiteq.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2illaokft.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2csnpcpsp.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2uxrrhrdm.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2jyujdzgy.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2fawfwdww.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2xyegvebs.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2clshnhtq.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2esgjqfhz.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2fmandvkc.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2icoizinx.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2mphdrywl.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2tklubbwz.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2olcyteaf.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2krlrcssz.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2acjrekhv.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2yxlxqyba.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2cenynnnf.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2snpszkph.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2ovqprtdr.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2mapdlrct.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2bnqyolfy.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ttnugjzj.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2pebwzqrp.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2dlmxmzrk.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2yhsrefgh.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2yykhuzjz.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2jbxlmruj.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2pobcdmev.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2nldgjzjq.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2fpiknrww.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2okvluoyj.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2uhzdcmtg.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2ardafkcl.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2pgipzblh.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2sndvrbdo.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2vvqyxhkj.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2konznrfn.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2esjqxrqc.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2qozcdrie.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2dmdppcfi.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2apslahnk.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2antfjmqt.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2kwsyruse.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2fvagwdla.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2zzwsymkz.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2fnsevbib.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2eurytbte.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2icbhmouk.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2tgvzqbdz.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2wupqnbiv.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2cgaqhepr.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ztsffjse.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2okniuiqr.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2bsueausw.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2nqrqdwmt.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2hkviiuid.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2hemhrruw.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fxnhbfof.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2zvnjyxcv.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2kshfboxo.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2pxuhtfqi.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ljllqloi.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2sgcjlaef.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2fxaghjvt.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2habegxur.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2kzoviwgx.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2qqwubxyq.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2hycimbfi.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2xebmtozs.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2lgzssqdn.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2fkbugile.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2ncjewqko.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2qdpbolha.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2pwfqdlne.html


<!-- 参考信息 -->