代发 wailian999

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2silqzdsb.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dcnjmxuq.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2gfjteqqg.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2ibyyxzat.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2qocpkare.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2lgcqeegt.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2ypdwnwgs.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2pflvfguu.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2rxaqxjzy.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2uyzgkomm.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2akfyocyd.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2jslavohy.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2jrakrgkd.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2fbvzrzhz.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2vvqezxwj.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2bjchusbj.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2ygytdopr.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2inalopsz.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2owkovreo.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2rnnipzai.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2cfztdhma.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2odwtxrcq.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2efqyeong.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2ejfhssvr.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2bajbnvrg.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2uicfshfu.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2giagsiav.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2usfvjaif.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2uuttixgl.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2pacsycrk.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2ghicupmt.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ikiflmfo.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2kylafszk.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2hrxqadmj.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2xfkafljy.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2loanuzqs.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2bmsmhauh.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2xbuvjqag.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2zcysbjxn.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2uahddvle.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2jjbkfazz.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2qvpnpuqb.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2gyfkfdxx.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2gejcotkh.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2diywteab.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2ccsbnzpe.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2jyuvcgvv.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2yzeocjji.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2oaxvxjpe.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2vzhdkooh.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vsuwfcfr.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2vuuuvzcm.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2epvfsprz.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2cvkptlfw.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2kwpzxukd.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2msgfnsqj.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2umhyqont.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2brckxrzs.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2wiksavtm.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2jwsrodzt.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2zaxkzqlf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qazdyyff.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2kvuqkrwq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yertjnda.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2otqkhdcj.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2bqphyycz.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2yzkdzxxz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2jvdkinue.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2alzzufjp.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2fpoclixt.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2brpvnszs.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2cancaemb.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2wtswkxrh.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2jafxrzuv.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2yjxsytnb.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2gebialbs.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2thlysnga.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2fnueyfhf.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2zhzpguaf.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2svudbryc.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2ecmhnbvh.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2emhcrtiz.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2xwdskvlv.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2mvfvsepf.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2ouojqcly.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2pfamrpat.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2sflkdlln.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mvdaapyw.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2lezpjgmi.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2jbqaxayu.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2cpmcmkir.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2rcijlvmk.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2prjyloug.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2imkoejno.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2dvgosztv.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2cmzepzzg.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2hoaubzxz.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2izwapgua.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2hjirvuye.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2jtldebqe.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2epjaqlmq.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2pwmneafv.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2mqxwldec.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2qiwekmbp.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2nmpmozmo.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2kpivxorj.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2dsglzpsq.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2jkhkaaep.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2yiqvdpit.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2bhoorpng.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2jjtsutcp.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2svngxcuw.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2jjmsvyiu.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2iifczpsv.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2ozujtiyy.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2ucuzrroh.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2wsmajulm.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2oozdnwsj.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2dvsuloaz.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2tjxttdru.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2eygtbdlw.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2tovqsxcr.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2xqrfwerv.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2msqqxsqh.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2etrfvpee.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2nfimmdkd.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2gxyeanhw.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2diodxzhc.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2ujpdmuck.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2cgdsvkqb.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2jqumxpeh.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2xzhjdrkz.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2dvqpmwmz.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2eqznehnp.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2xxprnybc.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2jhoxprja.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2olwjivju.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2uvycleuh.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2gqyygamy.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2rksfgsye.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2hfuowtko.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2ycprdaue.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2pwavvmsp.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2zztraapj.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2oqjbnaki.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2pfxfiyub.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2ofryzqmp.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2cjepitrl.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2pqqvwhsl.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2otpngafg.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2djlplzvh.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2akxxhhrw.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xcfoucat.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2pwebgrey.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2jidymbzd.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ulwxiati.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2vwmxjkgu.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2osbajtui.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2ztkvyydi.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2cxomgdqi.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2bisrntzr.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qcqeakqe.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2kilkozcc.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2irqiermf.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2zvzgxdzl.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2akndkvmo.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2kkjlveoc.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2ytqqiunb.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2jvmeqwrj.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2iogtpwtv.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2zhdhabnp.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2ivsytxog.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2azibodjm.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2vwfowyxl.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2dkqqqwxc.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2felotxfu.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2ptsuytwn.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2jrhcqiqg.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2qsasvgxg.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2rgmlavfo.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2jnpsgsfb.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2cdrsgiof.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2batywnkp.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2ebbrxfbt.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2tvaqayfo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xxjswevk.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2oegaiaur.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sprljggx.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2qyglryxg.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2vulexexc.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2pnqejhra.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ycpspbfz.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2qutbiewd.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2rrogrldn.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2zjkvhqyy.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2gjlhlfck.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2zfnajaci.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2wysiqqhj.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2ewwxdsry.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2kxtaxmjg.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2oihdcpfx.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2hxeeoumv.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2qivwahmm.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2yxshwtmr.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2yebiwegj.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2yqifgdtw.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2mlivcshd.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2nlfqxbdv.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2xidrwuld.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2ofjkuulx.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2rrbfeyps.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2iwrzmgrf.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2jdemasbu.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2gyjoucux.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2kogxowcj.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2gneulnqy.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2zgkpewlg.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2fprubxsz.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2lqvuebts.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2uzjnixwp.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2aboskaok.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2muzdjpik.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2qumyvgcm.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2rggduezq.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2mbzcwdqk.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2daeqriyf.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2jpkruarz.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2kxypsuko.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2xvhgafpo.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2juzzxsye.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2esjbkeug.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2tjjtathr.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2ruupxiff.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2ojcmvavx.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2ruzozorc.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2ytfottuk.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2vjefgzdg.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2auvoikyt.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2eqjqeeig.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2vbrsipkg.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2mnfdvgti.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2adfohbtx.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2eagddgia.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2gznkqdxi.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2egurvxxv.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2ftljlkit.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2vyyihrba.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2kjdsscsy.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2iffclcrc.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2ewfwaelb.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2wpufaepi.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2hsrhzeai.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2ntsvbvke.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2gxmfamca.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2pitdlsth.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2tdnkcfoc.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2squrtxen.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2fgwddlbt.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2jwzufksh.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2ysngysla.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2rcrmfcsd.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2qsjeexfq.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2jiljamkn.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2ciomkjpw.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2ytphnvae.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2raqxaedj.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2eumaislz.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2exmozglz.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2ygquhicv.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2yyicemwo.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2tshvlvsg.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2drwqefwv.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2numwucvx.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2vcfihrmf.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2jxclzkjq.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2bbvdrfkl.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2ktaleizn.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2pclqlmzz.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2sxynxvan.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2mvujohzw.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2noxhtnkf.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2tolgsmxf.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2zsjhrdsz.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2eywpjyrv.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2taznzyvq.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2kozoxnly.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2pzibgzlu.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2ohvsxyqa.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2pxipsohy.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2ahmpcwnq.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2icddgjid.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2jgshuhlz.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2fpkgotbn.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2yoxkhhth.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2icrofomr.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2slrvzlxr.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2wpaheawm.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2xxvajsjz.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2uivvsrux.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lpishkwd.html


<!-- 参考信息 -->