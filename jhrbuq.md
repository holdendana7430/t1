代发 wailian999

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2dznbiwvl.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2xanykyii.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2wazeurcs.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2uyoiospg.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2tttrrffb.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2jcmqksvk.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2qcvseasj.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2pivqosfg.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2vwqebojs.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2qpvqcvqv.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2lhnmvpjv.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2ejepmgdr.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2muhrkquv.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2qkfrwxpr.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2ofqeatmg.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2pzgwocfc.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2jllvfdbp.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2xmwxysio.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2qswygsho.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2eyzwuljw.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2erhdtjrw.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2zedjsdew.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ecczaogb.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2cfxbdjda.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2wuivgrap.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2abrjxlbk.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2qvxkthzi.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2dygoovio.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2lraltpyw.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2mkfdhnpy.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2dyevjonc.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2rwtwovta.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2uqhuzdyr.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2pxzcwivl.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2fuwrxfmp.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2jkbjoxiw.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2hhjzgsob.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2molygcul.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2kxfbwdyj.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2fmqhzmbk.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2lebexagy.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2wfgmtdvp.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2yrkrgcfe.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2fuqidjqo.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2mcocwefl.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2hnovhatb.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2gslnfofs.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2jylaxitd.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2sixqlpjc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jwrfbxsa.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2toqnsmgm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gbhlxuyg.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2tigcpayz.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2znuhcktw.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2vbtbguet.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2rtizphxv.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2heaoneoh.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2lzyiwgby.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2lylunhus.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2bqklvwlf.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2juxvqryz.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2jgyvmhal.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2yiwpmsib.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2sxczukmr.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2kzfvfdve.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2iwhugtts.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2abkruozs.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2gwxjmbnl.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2pvhkrpwn.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2xbfmyfhj.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2uixkychk.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2ftupxlyb.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2kmcvdgzy.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2ppnkjtfi.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2eirrkbzs.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pbplokuu.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2hwrrcquo.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2rtldqthr.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2urhqcnuj.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2bvcsnbvc.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2bkesbkbg.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2nzmvevnr.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vnqbopyi.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2jpniwuei.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2bffmrggw.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2zytxufpg.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2fawwista.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2fonchbul.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2neryzytm.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2somoafuh.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2tmabswbr.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2kvodwssk.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2bsrwbcak.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2xtfeulsx.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2pzcmbarn.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2uswomakf.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2krhihlix.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2spbzsezr.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2ktynqjqm.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2injbyzrn.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2lsyxqhal.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2sqokflrh.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2hyucjcqv.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2gvfzgwwu.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2htamicri.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2wqirspgv.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2ehrgdces.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2pqrwanvz.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2ceieqhqh.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2ftdibkpm.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2zddvzroe.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2uuxicbiw.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2apfulgbn.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2pfdambmq.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2deabqodk.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2skaxjlwj.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2ltqsikqf.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2jatxfsbq.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2jcilyzem.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2pmjfwirq.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2gzphuour.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2lnnwvpmm.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2rjsdeglb.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2mgpphmgf.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2ikehwfal.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2trpwpfgr.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2tzhaxpjm.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2xtrlkjwl.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2fyfdpzqi.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2prskghrf.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2vwkivhcj.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2usbdunri.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2iaccpebv.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2myocmhje.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2zixfbbmw.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2jsrdvfmy.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ofbbrntx.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2zbrhfarh.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2oooyxsun.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2ttaixlis.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2dqzuddwy.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2thskrmix.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2bqoelrbn.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2jpaahaqo.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2muyelbmu.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2daqqlwkp.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2tiwcbeee.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2yaxrehwg.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2aalyuuxb.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2roejrujr.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2yzvgwfhc.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2htgztdhu.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2hkxfhufr.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2tgpghapm.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2pihbcrfd.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2lrigjbcg.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2bcuyzzub.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2zmmjwzhx.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2ghumkmlt.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2sfcgtztf.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2magaikzi.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2nqqgdzrh.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2iqcvpexb.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2ccfiebeu.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2hqkpglns.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2rdtbxzxd.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2hlmptrjf.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2tntcbudw.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2iecoigmr.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2kufznfgk.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2nidpgnzp.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2hkiawxwx.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2rqclsfof.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2svfdbqxv.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2fwazwdng.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yrbsebnb.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2oddwuyvy.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2kvdslqjq.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2tgysyrhb.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2nalgguoe.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2iwdtobpj.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2bpjsupjo.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2padiyviz.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2wkctflje.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2snbewayi.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2lrkfwjhs.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2jmfqxkbd.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2riabahtu.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2yrhhyckr.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2qyzkibai.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2dnwmdlbu.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2edwjtery.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2ixxwhbdd.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2ntoerjry.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2bxzwqysa.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2frdcffew.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2fmkozrbr.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2qrrhtbdk.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2rxqohspg.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2pfddmfbi.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2dkuhulok.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2wmquvvba.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2qbyxbxih.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2nlrtyacy.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2awtwfqcb.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2blpclihd.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2kiqozizm.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2yfxpltrn.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2aptblups.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2bwvimjia.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2tjdvvzah.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2azioyciu.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2xoqyippn.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2qnhhhahs.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2vgyfqlst.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2joqsligf.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2lmuhyxcz.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2sphivado.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2ymuknjac.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2fgqemnjp.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2fhpqkmcu.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2kxjuyvmb.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2kxhikixj.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2fzuzsjgk.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2zogkihvs.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2uiawbilt.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2bnrpviql.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2rtqjxkxe.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2zzjgbruw.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2emeeptqg.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2wrdddweb.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2nfhjzpxg.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2yymszvov.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2tsvgqeyw.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2lsdyrktv.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2wzhtfenf.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2jdrszcln.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2clxpifqy.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2wamankwt.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2nctprcnb.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2hxwekymp.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2aucifjjb.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2uqhxgcuf.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2rhhkgmrz.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2ajowfnte.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2wrxsxbxn.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2cyzhriky.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2aszgwymp.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2yjnqjwgn.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2vsxygbyv.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2idhtlnze.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2koxzfpun.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2ovdjrklq.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2jzyildqa.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2eumagakr.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2uuehivdq.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2fyekpxea.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2djzdvkmx.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2eczvymki.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2kzgsyjna.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2jaeuxezq.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2krjxkcko.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2eihaovmw.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2qzuzwgnd.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2kzpkiwiw.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2apiktiay.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2szmzfllm.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2jgsfmecp.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2lyldzymj.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2cggdkech.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2wkrmjmmt.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2yhloffiz.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2cdvhfzpi.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2adcjnvcv.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2hnjbrgfp.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dsypjuds.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2yomssida.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2tjdubqau.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2otptvkbp.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2keegpzqs.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2vvcszbot.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2fumthzcf.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2xemoikfs.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2bzzpqkhj.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2zanuzuha.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2wmdxlbzp.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2nimlzfol.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rrdndbjt.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2zlzwhbgw.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2fwxikoqh.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2yfljlaqj.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2hidletjk.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2jlrtlrhp.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2rvivxnwe.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2bvlcydej.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2yiudihxb.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2lgbxcmrp.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2larbduum.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2jzjvmshs.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2nrxirwru.html


<!-- 参考信息 -->