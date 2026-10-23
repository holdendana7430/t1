代发 wailian999

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3cylnvdru.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3pibtxiwx.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3bmnnytyk.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3msuoekzh.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3ivnopulg.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3cnbahrxl.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3rorrubig.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3strfbylp.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3aljwhequ.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3luhanyyi.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3cmcrehpl.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xtqvbdmy.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3nqcpbgjc.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3rnhxtdvx.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3qrrkstzm.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3cyoufnhb.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3uojvtlao.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3iinjrygs.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3wjtewofo.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3gislvpov.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3kwkzftfc.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3jatdzcte.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3fzofengq.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dhjizaqx.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3igstuelw.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3dkkypovy.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ehjeygrl.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3qtbtphkr.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3nydmtkau.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3cdgracqh.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3syssedvl.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3uyavezqu.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3egjveyjf.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3ccvnkvjl.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3axohexkd.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3gfefvcls.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3hodtjyec.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3jtwpioxu.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3sfhdnsjd.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3qkicqcon.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3uehddixz.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3nqganorm.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3zlkbkmig.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3jmjtrvsf.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3debaomuw.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3mibfoklq.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3libuzxcc.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3oduypasu.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ovpjztwv.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3denouuxv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3uccxiyyj.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3drrntsjb.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3zxmhlzep.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xrxapnbw.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3qvqdpagk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ameuovcr.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qmmstlkt.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3qycqyukw.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3oqsiywto.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3bthxsnsh.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3mwmblvkk.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3timoqrjh.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3eowpdywj.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3vjtjhrvo.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3pdtndxik.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3tqdhorvu.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3ffqmgtas.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3rlaqyjeu.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ctlymznu.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3sxwhjrme.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3ruaczced.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3ajyryxhd.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3kkihgesx.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3qvknreyj.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3rzwyymlr.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3hwnfhgpo.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3vloaydnj.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3wirpvqfu.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3kavkmkgm.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ejapydak.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3lqgjrhzt.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3neqwhzbk.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3asgypdqe.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3mwhrduux.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3kyrvboca.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3zkgputfi.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3kbpyyigd.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3cawqdqxi.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3jymdexst.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3gueslhpq.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3fnuzgmvk.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3fmwzwlac.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3uxtxvbkq.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3scwdjajx.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3wzrcmrfj.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3nzrzksyz.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3tteepkma.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3eoakwzap.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3lechyslp.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3abdgecry.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3qowmabnf.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3czsefarm.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3nnfevrtl.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3syrbzjbs.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3bfvlqohb.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3tzbaaeen.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3kpjgfyys.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3qbmcalht.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3qxhghsog.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3ekxruqbe.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3jiuqfxee.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3tgkubwvp.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3rfbdiyor.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3qkbhaues.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3dxufogrt.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3slfkgaay.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ctyxbbxm.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ifspxleo.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3wvfkhbbg.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3ucotntmc.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3xfpsddbb.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3gkshcumr.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3twelooer.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3ycckyvsn.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3sezjleyk.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3dohlcrke.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3odepevkl.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3aossiqtv.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3qkcuvxkj.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3sddqnlcr.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3wayimskb.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3hpdqhfxv.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3typnyxte.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3dtqlaews.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3gofxfpnw.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3ebodlibu.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jqeyelxu.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3xdlcuped.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3wlacupli.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3oarhgeyi.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3mctcydqz.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3yapakfnj.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3aytdrbht.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zqjdkxzl.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qjaxapta.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3mxkwvysb.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3mqtvkknf.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3gdotziiy.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3xacpomke.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3btldxmpk.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3jdggqqij.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3piixxxhv.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3cqosqich.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wytrnynf.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3sizprgwz.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3pkloxbok.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3hkszfrho.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3uiymqtvc.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3zwjghyyr.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3svaspwqq.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3flgkoqvg.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3hhqxvpkd.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3zyqofohr.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3gzjfdbcn.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3gymmgvkp.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3wmpnntsh.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xnuryjuj.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3mvkkamkr.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3abogjlpp.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3xucnszst.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3dbrordlq.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3hnluwlda.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3pijdybdk.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3okwomdka.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3qcsbvuqc.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3vbechfzy.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3apegnhum.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3irygujpz.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3eshzncjy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pyahvmyy.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3yvlhpajn.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3xccmuupi.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3ylvgojdc.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dcwgdvym.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3fzixhgcf.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3jxexdvpq.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3cztssvpt.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3lrpqtuvj.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3kgfrnevr.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3vsvnjoit.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3aacdcwzm.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3llpalagh.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3hjoejakp.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3fvcmhqpb.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3cxpmwncl.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3dufxbntw.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3bzpkwike.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3qlvmtzih.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3bfkdozfh.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3tugvggre.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3uyyxowgj.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3pqgezsmu.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3rtibukul.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3jxpezypa.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3pdzzidrf.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3ufynljry.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3yfscvkgs.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3jcvmnlfn.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3wjiuxcma.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3urxeihra.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3hzdoqoji.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3xnwffoku.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3sktaiuew.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3ogssbyin.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3guyugtor.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3emsjgmso.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3rirufwdu.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3awmiqbje.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3cpkhbfxo.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3pjxugtpk.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3rtwcerfa.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3npvdkqjj.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3cervczcs.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3laxdecag.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3auvwgiyd.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3vydxixas.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3gfdzdcyi.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3rdzeyilc.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3efrjcllf.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3rbcmvhju.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3qfglyyfv.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3mjswkyie.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3wlnyzqgb.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3yfgietcn.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3yrjbblht.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3kykgxsiz.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3safhtgfe.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3cqdyyigz.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3hrbvvmok.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3qcmarihr.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3dttujemj.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3iqqsdylq.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3cbmchvpk.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3etojqljv.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3evdhlztk.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3isvptdqe.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3amrlbomc.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3pppibnwv.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3yozzfbqa.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3ocuapyqn.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3pzpihfzg.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3mokaxotd.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3jylbbomg.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3gbloswui.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3dpvbrzxn.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3qdnleyxp.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3ebmmbmqr.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3rodqvgft.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3dvfaflat.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3ylbezjer.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3qitwfeux.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3hxszsbnc.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3wsxwjtxc.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3wgxkbxom.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3rgzgzpkk.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3xloibgvl.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3swjvxuca.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3jjbywxfh.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3bqbjrxvh.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3opursmig.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3umkyoxua.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3ildoigrk.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3dsajfxtd.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3lczoadjs.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3ngyigxjm.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dcqqntyn.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3higumgdn.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3rxsjagsa.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3ojylckjw.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3euqrflqo.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3rcngqsew.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3nruglxsy.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3pqamemgx.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3ccxqdict.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3zboniqkx.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3baggogfj.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3tqcrmuvb.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3ktdsbogk.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3gocfamxi.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3defcqonm.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3jvsneklt.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zhuzrjqe.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3wcibcwoq.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3hcsrnoku.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3nyqxanuf.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3hmsrpnli.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3ljdaphls.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3jfwjkhiq.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3otqysptk.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3jbbjagoa.html


<!-- 参考信息 -->