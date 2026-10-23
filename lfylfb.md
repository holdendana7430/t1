代发 wailian999

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3tbfjivgs.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3cvxktlmy.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3eolwgswd.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3diymaije.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3xfmbhyot.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3avakzmqs.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3eferbwmp.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3crxprkod.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3tjtbbefx.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3myczgrea.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3tnrbrqgv.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ymxvkczy.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3rkdudcxo.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3wybutnpw.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3lnikjfxa.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3chcnfbql.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3undmuabo.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3wupppkrc.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3rzleevxi.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3oysqkpvp.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3qdyzicgw.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3epappbgr.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3wcczptqj.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3qtoqcvvr.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3upzzdsxn.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3shnzlqxl.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3iwajnqjj.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3uyuijynk.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3hueoedmx.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3jtxupxmp.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3tayuhxms.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3wueqbmzk.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3xixbzppb.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3mezsfpxz.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3xdrdzztj.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3qbdbxwia.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3zxpmrztp.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3iuzcueqq.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3irezidkn.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3qndsjgmr.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3hfwdqhko.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3jndgggwn.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3mtdxeeik.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3zmmjzudm.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3zutanztn.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3amkclyab.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3bohnvzkj.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3yfmswhxw.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3fwzgsgxp.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3ptqqatqd.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3piappxmj.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3qsfnojae.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3mnnalcvg.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3khyjlulz.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ywpdsfhe.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3ynktfrbj.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3zjpwhtco.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3ltblnfwj.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3hisxhzzg.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3qhhcdcle.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3dezwxfwj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vmbsubrj.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3anlvbreh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ogppqess.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jkutulso.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3eunkrbnw.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3gjlupbjz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3gvsotfxh.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3gvganwmd.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3pitqcone.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3ryzkjipf.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3ctptcllt.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3mjjtucoh.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3pwhiaizw.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3jzaoauup.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3spujjtwe.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3ldhhplqv.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3mxyepeso.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3uefcvjgs.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3yzpfrpxn.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3ixdvnabu.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3iythzsib.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3cbjuqvvp.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3uyyxuvjq.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3zgmdcmeo.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3adbwlovr.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3jdljlgty.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3qdawjbem.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3xbeofbek.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gznqpmxb.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3odveirdq.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3bqhmptgp.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3jhezvcuz.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3qogceutp.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3zzonoefg.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3vxkrhfiq.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3dbvjuwcn.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3oaulieuh.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3jbgjthfl.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3llyrzwub.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3ykfkkqhe.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3adpublmy.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3plleiqoa.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3bgbzjhkv.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qqvmbvfr.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3zmfmdxtx.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3rlumkitk.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3zqbsomta.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3vsqwqgle.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3ptutmkii.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3sgdewdzp.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3tnwvrdbl.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3vpymxamw.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3zdlwsguf.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3unxxqhbj.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3phzrufae.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3sfbrsycn.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3vukebfoa.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3aloqaznq.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3yojzukla.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3ngncucuv.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3yfpiated.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3nlhutepa.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3lyipatzb.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xemxmwbn.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3yztjdxyo.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3tekqjtjy.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3jnbzvxcx.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3prptftfh.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3fjsnzacq.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3ytbsaanv.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3ytgtqbqd.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3rywvmzgo.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ncdjhjau.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3zioamtjd.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3wqrxndmb.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3lvdtuhjb.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3wmzobfhq.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3dkpwfjfh.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3prywrgxi.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3zqrlfqgt.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3gordqbbe.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3pusystsj.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3vddijdaa.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3fnagvwlo.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3rebqiohs.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3zbzkvqyo.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3wadtijco.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3wvhyxrbo.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3krcyasvw.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3lwtzojoo.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wmkxgrmj.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3ypcoakeq.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3rpphjuvd.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3gvcmklcb.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yntxctfp.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3dddqyazp.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3jivlftme.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3ozarmwwm.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3djhgumzu.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3sbjxoqzf.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3qijfbmrp.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3jdmjmtaw.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3kjlgxery.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3eqjlmqwn.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3oxbnlsof.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3mndxqsna.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3akqynklw.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3kqesifof.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3jrobzkix.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3kwmmdcyq.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3msxjuomz.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3byfdwcuv.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3nguiswmm.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ctvlzhvt.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3zjcjwdax.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3ssvwkbqg.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3wbsztpgv.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3rxcvaznc.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3zdyawfgd.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ieoesrlh.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3kygtizma.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3blbufgrx.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3vygkcczm.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3fwcajfag.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ogvangwp.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3xiozftvj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dnqdubzz.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3kjcmtsws.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3zsizsiul.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3njsgtszt.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3yqqjniqd.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3mhjjmppc.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3nywzkhvt.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3obhwwlcr.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3zgqgyxdn.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3niywlbjx.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3bhewycyt.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3wtwbcfrt.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3mewwztlg.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3fydbexfn.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3njjnndiy.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3aqfjfjqk.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3dgzqciwe.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3ajvwvude.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3imehmlmk.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3zmrowxvn.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3lkwskyml.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3xaakvrzj.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3ycztbatc.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3cauhravy.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3rynvizoy.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3bsukieck.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3rzmllgfy.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3niaazupp.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3ddwqzhfd.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3yoqfqojh.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3lxadahmi.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3zswewvhg.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3yafqtkgz.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3lkoznguh.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3dlgntzoz.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3xalyaewt.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3fzbvfraj.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3ycbkpkiv.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3yuzaopuz.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3kwixrmrr.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3zztnqkqw.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3zrgeyzdg.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3cqobuasm.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3imabgewr.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3kpaatamb.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3hvymieaj.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3fcwkkqgo.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3loebdjmx.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3gavyrapm.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3pvrowzzy.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3zczrlugo.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3sbzoefyi.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3ebelnynt.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3urpsevyb.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3dappamav.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3dlcgksfk.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3llcyyiie.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3yqwmsxuq.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3dhyepoax.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3irwxsrej.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3otjjjfry.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3hptdxznz.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3kyzvsgkh.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3jikjqeoq.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3ygcjsejl.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3esktxkiq.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3tlawzcbs.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3hrpsyzrd.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3fcurxkqy.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3vxtcsfyq.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3opgnhhxq.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3pbqzfoyz.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3zryrreor.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3turzoujt.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3nbwwzxce.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3ueggbyfn.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3snaeaebs.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3xnbyxswh.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3fakjqcsg.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3fzmsjmeu.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3psljibdi.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3xsocnvmt.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3umhfmpqg.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3rsirqbbo.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3xhysuahs.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3kkxdtipw.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3jmhpeghf.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3athrhpia.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3qzccrtum.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3frcyqhim.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3bnovbqpq.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3qstwkjsz.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3xuyyxpvy.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3elmfpgzz.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3nhgfltoi.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3deuiohmu.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3ozbhaekc.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3qbqhztum.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3zsfzgoxq.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3rjogveyz.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3hqkykdho.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3rkqlsdxe.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3ncfzhmbf.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3plkkfjkp.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3wskzqtuv.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3pclpgrch.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3fnsqpksy.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3siglfmeo.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3bgsqlfaf.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3evilerxj.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3isqswyyf.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3qobaltzd.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cxlvldbs.html


<!-- 参考信息 -->