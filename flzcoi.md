代发 wailian999

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3ewcojcek.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3fllzcviw.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3ccekvvmv.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3iksnimil.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3hhmvifzh.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3dhjulcmh.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3motyuckk.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3qkowtbsh.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3joqefnnl.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3puoefpyz.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3xuhthfup.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3kqugggob.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3jyrrhxeb.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3cxdkjxfz.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3ekoyotzg.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3dwwxmgqa.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3uhnfcsar.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3hrtulctl.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3kxiniusl.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3gfboshte.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3dpbwqjas.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3zypeayfs.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3xaqxliwn.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3zomflnay.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3aapayczs.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3amiduofh.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3ptouccis.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3fxywdotu.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3ycufzolf.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3pusadywe.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3csqwuzue.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3mersdzih.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3darjzcuv.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3uaqrreep.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3grhbpbty.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3dqckxuav.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3yvcomzye.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3gfhsotbm.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3gydscpox.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3doweicxl.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3telrhrlw.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3imyurame.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3cqgfuuze.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3hhziiiyk.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3xcqlyror.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3rxmuhzmo.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3lcrjbhac.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3iufbgoet.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3pajetzbk.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3qbodikym.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3yujpfqzc.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3kfrqogbc.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3khtucbnd.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3xefguirb.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ydmdpslt.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3jykwnwwl.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3yzanxbiq.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3yygmjsdw.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3fpmaawjx.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3sbkdknfo.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3bzzkeogp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tufkctlc.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3btqdwzzu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fkzresof.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ikskgikt.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3zjipvpib.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3meurnvma.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3ogrokdeh.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3jygpvtlj.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3gaitqssz.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3zanoinqm.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3obarmust.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3qbvwcpcz.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3lhbocgag.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3asdpulyw.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3tfbmnjax.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3tzavmbot.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3detxjqck.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3krnfqxpd.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3oljblfda.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3wjpyrdlu.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3bmqlmnhb.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3ffzcmhdd.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3wwyjsble.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3dsultaal.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3xxvozhgr.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3qcraybyg.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3jhgyzvpm.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3wowwdiao.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3rjinhxpb.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3tbrdarte.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3txaejgly.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3vmemknxa.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3bdmrnara.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jhvwgjwn.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3wflqoeug.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3cwdvlktg.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3inpzgrdi.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ulreagcb.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3eavclkrj.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3yvxqkkot.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3zsfybemw.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3jguayxxj.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3yicctuwy.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3gqijtxna.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3uxrtzvov.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3wbznegvz.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3eiaetwxq.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3hxrvpwfy.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3wprunmzd.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3tzmguafq.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3kqqloyqw.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3tetwitew.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3xunbmkxc.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3nmvdkpia.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3aetwujxr.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3szwlhclh.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3toavwaom.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3daqmrvcy.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3hiynomza.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3nfmbvkbc.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3gobeuhwm.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3mvirwnas.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3crfxecyf.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3xwhboxnc.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3jfqlnrso.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3tslhtkqd.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3oaclqgod.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3ggvwgsvg.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3aivkebps.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3yvcgfvvv.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3jfexbvqi.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3yfvjhuvg.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3utuadzbb.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3wptvzfmu.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3rwujyemm.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3ypnxkntc.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3avvkdrsj.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3turnxcbc.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3dkfmrgpb.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3rpvqagse.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3yvdooijw.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3ndgdibyi.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3tfwmjrin.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3mgpuxekz.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3ptxqovry.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3gugekoly.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3mxfenhbh.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ekfulmfa.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3eitqrnzo.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3xfqvhhzy.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3owtnfiny.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3gxgqdrpw.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3xslanexn.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3fydzmfwg.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3dflgjwlm.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3lbyqhyqa.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3rhkfvdwh.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3vchefqoe.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3vlvdwiap.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3sgevavph.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3yvaljsti.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3bbxdrfxc.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3sifmrjlj.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3bhbaxhqe.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3lexylyjx.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3jtzrrbom.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3aywpvhih.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3amskfmgr.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3jnzqnyyg.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3isslvcri.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3fvqladeg.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fqtuezfj.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3snmfogpw.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gseklqbq.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3vozppvqu.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3xousetov.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3echiszlm.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3hnmwgtue.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3nsnwjppd.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3amitzoyc.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3dzweijzc.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3pfuatmqf.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3zbcdvmux.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3mcgofbye.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dyuqgcve.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3reycvfgg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qzkucwfe.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3kbusvmvy.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3ahwwbxss.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3gppowwga.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3ynwoinkf.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3yghjaplb.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3oxpignqi.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3zjgeflap.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3etslkdrz.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3gmmxquov.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3mlpxssny.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3grjyurkb.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3efgjgqhp.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3onczsrul.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3nmkywmvx.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3aiwhgyew.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3pnueflyf.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3mjcbmlqs.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3hhwhauov.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3fipeaapy.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3tfnqggdv.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3ofusprfe.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3inbxpekv.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3ysdqrwcm.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3yvfteoup.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3tvuetclb.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3xyibknca.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3jvxmumaj.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3zrdoubph.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3sgrpanrf.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3roteeegn.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3uugadgxy.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3tffdhqyu.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3ckwqgbqs.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3rktrmvbr.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3nrgxqthf.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3rvygodue.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3hbuwmpyi.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3dbptrbbt.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3hjfrnyfy.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3gdhlbrkg.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3tqyibict.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3hvwfcuxe.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3lsgbimvn.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3pjomnbuf.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3ijsxzeoo.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3daorahef.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3clhtuwoz.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3sqfxhtrn.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3crketmjz.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3szugtzpu.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3likcquxy.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3lpfqpmww.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3kemieuft.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3zoroqzjq.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3wdemqexj.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3vnushfhw.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3zunpwycv.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3tueeuojg.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3ablzxlzw.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3uaxopoit.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3kbatqbak.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3ararctgu.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3puebolke.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3ickwgjne.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3lsnfrutc.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3zwjtlzjk.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3rnmorboy.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3xhwtmrmd.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3miwquzla.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3rmmkvknx.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3zqobpmci.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3tsfselwd.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3mjnghgdm.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3uvbtdajd.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3cfimtlgb.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3krlehygn.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3ulyepcna.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3jiquebzs.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3yovakkip.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3ximrypsi.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3uuxzaqml.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3bcchowao.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3rprojzyb.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3sgdnmpjs.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3fbhqqmll.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3dvsaorlt.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3jzpaslaf.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3kqqypzxs.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3lsyvuhkb.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rtrjblsh.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3wvvwwqag.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3jjsjwrqz.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3celnfnqe.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3erfwypxn.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3vxvmmggg.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3qiollkrw.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3azioupdh.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3rkqusven.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3kmlvbwpa.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fcqhrris.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3eaebwjhh.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3dlrnwrlw.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3anvuopww.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3awscpiwp.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3hebyxmel.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3kamruppq.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3jhnfhoig.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3twkduoak.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3gdtcxjsm.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3sskqzzaf.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3vevbrskc.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3eheshwol.html


<!-- 参考信息 -->