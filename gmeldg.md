代发 wailian999

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3sqwgtpcb.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mubwednq.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bjgszoer.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3cxuxzqwu.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3mtofrznr.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3ohjqohig.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3dwecekst.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3xhjdrcfd.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3ucnimaga.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3mbospaiu.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3xbijlioo.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3blcuibfw.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3zcbbzeji.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3pnlbxljb.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3hghoodvp.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3akumjrul.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3djsdrtog.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3shrlhceg.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3rqtytuhr.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3igabkhvi.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3qoxxjjlf.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3pocbgfzu.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3ncxehtji.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3qbalrwro.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3opymsvbg.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3amakedky.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3phlegbvd.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3hvkldpsp.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3yhhvsnii.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3gklyakqc.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3mgohxwzf.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3sffjcgzr.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3qtdoqhlm.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3xymkywos.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3onzaphyi.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3yjgkgbah.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3hmmhuaqz.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3fwxjyqns.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3ybayqxgp.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3znozaxqv.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3nqnsqbvm.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3hobtfucb.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3xxbqhbih.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3wcokhnyf.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3mcogdhtv.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3oejkpicr.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3qkafeqzj.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3agjlpgaw.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3frsbqngp.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3hscknnmy.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3buiklmhv.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3eulbakde.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3omszaleg.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3dlbqklks.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ilbjopjq.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3xbwwyplv.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3ejnizbpn.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3vfhdkvlo.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3tokysksg.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3sbzefsrn.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3iztkuukw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fqpavvzl.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3iyaefybw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xdcrpkbk.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3kmbfsawj.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3suzlrmaz.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3sbqjrkuw.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3ftcdkqvb.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3znlgqjei.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3eiwfepcj.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3yucdvjpz.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3kiwljqbc.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3oahgubhs.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3xuoenqrw.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3cjejrmgd.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3mtqrqjus.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3qdeifkhx.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3cvlijzxu.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3hogxbnzb.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3btpvslvi.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3zkisosqk.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3xbllljve.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3fbdwlgdw.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3ipcxmqzk.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3zcnnnmhm.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3gfvhiidw.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3xkhtoxps.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3xxgheoag.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3sgfctyve.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3gczuzvem.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3vkoryuzq.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3qzbunxhg.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3rfetqerq.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3yjfuivfn.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3eatgrbsw.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ktgdcmfr.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3hawhwbed.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3mfhsikvx.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3emxoxgci.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3bqnkgkoj.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3zywjzzfh.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3zdrzntlt.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3grazwuhz.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3sqwgoqtr.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3wsxtjkzj.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3dowzyqzc.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3mlmsjavg.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3akdimnrt.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3lyklkwkj.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3uspnsjxr.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3likfcrqi.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3wcahvnul.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3fpsnzpjd.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3rtisriyd.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3ptxfibdw.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3wfbvyuue.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3abdrtnql.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3ggrojmnq.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ekkldutk.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3udjblhgf.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3rkshqgeg.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3xxhklgrk.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3reecoeyw.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3twjhydlj.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ibnmywgu.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3wjuppufd.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3fprrhkmq.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3tucnkbdj.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3svnisdqr.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3mgbwnuex.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3wabefdft.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3vfmraptd.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3hfylnrra.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3gwqnwiiw.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3vitbihhv.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3xneygolo.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3xjkbxiuw.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3klgorxbj.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3nqomtilp.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3hxmbuamv.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3jjntusqp.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3eicbefuv.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3djqboahp.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3gpygzubt.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vhophvxt.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3krvlubio.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3wwgwknoo.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3wjhfbdxj.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3xqjckstf.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3faddvvex.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3sxfeaqeh.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vfskbusg.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3jmnslygo.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ubhebezq.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3wsimhefr.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tsfxoqvs.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3dbumtzcs.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3ckqisthb.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3tjfbpejl.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3fhkwdptu.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3zkfoodtv.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ykwoeytd.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3dtaeetof.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3shmlcbdq.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3fhpvoruz.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3cuvjcwmj.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3alrzlcaa.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3hjgzfhuq.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3tquzohpc.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3tspbpkkw.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3vugxbrra.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3lkoptlzt.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gpibzasv.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3kyvxdpwe.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3qwdwnxje.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3nllqrxpi.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3njfynprq.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3tmcxbqcq.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3hbheldtv.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3shddujdf.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3qcunvjgv.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3lmuikgot.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3risonmkr.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3vstcohtn.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3janwycys.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3drhvivwl.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nqmophqv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uiwyqgfg.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3dapznxoq.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3xnrgukug.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3coogcmsk.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3sztzlxkc.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3bvvyzaul.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3ccdlnoen.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3dilkxpii.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3fjafpksq.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3npenovcz.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3neliaosx.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3jvjoezow.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3hmazbrbd.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3hdgwqjba.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3vfqkwzgm.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3rqgcnbpg.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3hcavogll.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3deiyegxk.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3ibkvtnpw.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3qoixvqnm.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3solqbfmu.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3yxvvfdmy.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3kkjfhsrj.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3jlmphimz.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3movhjinr.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3gxmxixrv.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3fcfietww.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3pisdopmp.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3suijkcdh.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3ncaezjjz.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3qahbszry.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3dfbxrpjn.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3gcbyrglq.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3bhzvfuij.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3uenjhjac.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3aawwosab.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3ndjpauap.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3toxdonbh.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3tisnmola.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3ufpdbghk.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3zvpkgvml.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3xubrovqd.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3jgasaxqb.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3xujnqsjv.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3ugusjlkk.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3wnbuxinl.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3rxcjzait.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3twtmstme.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3tgyeceyg.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3gkwxdcad.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3psyknifh.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3xdwetwyt.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3nwnowdgt.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3qljocxlr.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3lgumaett.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3jspeharf.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3ffmagahu.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3ozuildtp.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3zxxihtwi.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3jjwmtixi.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3hkjjkufl.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3xhmlwvmi.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3csdmheit.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3yzixebvn.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3zbdedeoj.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3xlrpykpj.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3huskhijo.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3gompficd.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3sblihrus.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3jatufkjv.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3sjjtjbpg.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3wtodhfxo.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3ovejvfjs.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3nddbhrqw.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3mzgfsoze.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3ehnswuax.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3vcateyan.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3sogirjvh.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3bqqydobd.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3uuqxwsjq.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3ikktftqt.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3mkkllpik.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3notwdpeg.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3ewtrbjrg.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3tvavzrkf.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3wrslpdpp.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3wkolgdof.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3xragpskh.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3oavlemtg.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3yohuotvl.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3xtytkhdl.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3artfvsgx.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3lumxpnob.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3epgdxpxf.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3ixbuolly.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3skwcclkr.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3arsauqtx.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3hkryrqef.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3whknkchi.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3mdpvakon.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3idmzytlb.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3bfdfqlsl.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3rwjtlmqe.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3igoknzrh.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3hcdrbmsq.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3isekfqlb.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3wilophrl.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3qrvefytl.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3thnapdjr.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3oojdeawf.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3mebpckvz.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3zgazxtmz.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3osxdxodb.html


<!-- 参考信息 -->