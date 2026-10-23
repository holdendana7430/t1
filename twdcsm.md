代发 wailian999

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3cvvqnrim.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3kcgxyiaq.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3vigzrhgw.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3xupwcncw.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3qsxpolhs.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3sahmennm.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3phtqwzrx.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3jomkwssf.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3jgoxgsqw.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3bdbmdrrh.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3onxzztbe.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3rrybhxsz.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ytnluhtf.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3jeaaqude.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3nfkzwhjj.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3lecskfjm.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3clrxybcn.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3xrhepouy.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3wwtmwemn.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3dunsdvwv.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3mhaaufvy.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3hlbkikbz.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3rwhqdrxo.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3wpdyhemi.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3sbgfoemm.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3xfusyfxs.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3mzjxrrdh.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3modyouor.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3wtwyftpj.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3hlkyejeq.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3mvkrxdbk.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3rpgclnjf.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3aekrpwgb.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3lzkrtjhb.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3xxdkcjhp.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3nrxgbhny.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3wvajemhr.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3berhhlla.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3mnnnwddx.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3rywssslg.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3nzsteypt.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3ckoozuqo.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3nlntuwpi.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3mcezwihj.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3odoyzmav.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3vtlpdubq.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3uikjtapq.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3jodmazhf.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3sxojmnim.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3rfinfrmf.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3bozstmzt.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3zdzudnhf.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3ivqnmwpj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fgwxaigt.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3pefzequj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3byetdczs.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3myvkeawm.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3thhycvze.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3cgkzmqdi.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3wrdmjdbz.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3bisxafft.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3qlfcitxg.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3jtxfvfbi.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3nfqysnzb.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3iswmzyna.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3lqscbxeq.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3kruozdoo.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3aihejdcn.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3pmituace.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3ylyosgal.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3asautxlx.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3nzoqioew.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3zqvoajll.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3ctuwjpqj.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3xrwhxwlo.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3hxpjmsof.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3rzizyiij.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3ixtzfnlm.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3zpgpwzdi.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3sbgxnkwr.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3hjjfyhmj.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xbiyojnn.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3hgtacczq.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3ikfwhrkz.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3wulgtrcp.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3gdsmvqrz.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3zstfviwi.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3amkshhnx.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3yuofcrsv.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3mlwtiqkf.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3dzhranpt.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3nmrhnfru.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3qnrygryn.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3xprtwkqf.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3rrwgpcsb.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3bwqgrkuu.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ghgzpxdg.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3dsfujmin.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3bqispugy.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3hrykkdzg.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3lcbfeyrv.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3nbxeuyfr.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3vjgpdnzx.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3aubuxrtn.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3jplzkpne.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3bxluczxi.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3oegogupz.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3dpetzree.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3dqmgrlqp.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3xoowftvw.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3geqnnvbt.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3haglgabm.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3smbjyzxu.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3bttbdjix.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3uesfkwiq.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3rpljegcw.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3cvtucqhn.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3zcouyfcd.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3evhxgngy.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3tzslziiy.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3gtlymxni.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3kosbstud.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3xvfygauq.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3awtfdaps.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3dfjqvumi.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3kmfrcxlz.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3dkzqklvt.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3jnwtejyk.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3opuokdto.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3zgdmtfgy.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3almpnwug.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3zlcwpbll.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3jjfobbpk.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3nxvdzkrt.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3uejmymgu.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3mgqogxdt.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3nazprrjg.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3lnntjpta.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3jfnzqqes.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3dpanpjca.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3sqxqwdrt.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3djvcwjyk.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3agmfrjrp.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jijyrkof.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3fssskcyw.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3yithcxer.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3mqorrbss.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tqnizqmm.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3siffftsk.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3qvsjugzq.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3ddjxbmia.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3ucfqotjx.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3eeehjgiq.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3pfbbdmyx.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3fezlavjh.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3qxrprdfk.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3wsuwhjzy.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ymcvfgsb.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3eyqaffye.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3bygrtyzr.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3wryzlntl.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3mcepqcre.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3kelawobv.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3fkprmndm.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3jdixuocv.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3nnwkrare.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3alwfmcje.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3ujobiqwq.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3teukzarw.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3zoeyounn.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3eakrcfyp.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3xjmvqkmx.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3xbiswwvr.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3ajyqtjpb.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3ztgkuoko.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3akumkaox.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3dabcijcd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xymdnkpq.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ryfxefrw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vtjdbipy.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3yvynwbon.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3bfijctgl.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3gvwdwwbp.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fdspeflx.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3nifcaqma.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3regotfxz.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3hsmzmuit.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3ciismevb.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3yiblrsam.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3bjuwivom.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3hqjhwgvw.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3lfioavyt.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3weliposd.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3bqupmzuf.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3kfokvicx.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3deraipxx.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3recyfovg.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3grynwnwj.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3hpaqsyun.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3nwohpuux.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3kcrskbjl.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3ennxwzdy.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3xkglrbhy.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3easlljrs.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3eqxshhbn.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3vkqogbhx.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3rqblwpbw.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3wumyqyrl.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3jorhamab.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3sfifwkqu.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3lpaogogs.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3enslstjg.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3ocdxaztu.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3jgkdrxrw.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3rwvjzvps.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3yfvmmlcg.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3gsvtfgld.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3ykqdgoee.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3gwvkzdaw.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3manaabnx.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3xpuplice.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3sfhzadyk.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3xemrriax.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3xuyyqmek.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3qoerxgjq.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3dytdbekd.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3shpjzfgi.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3rtumoght.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3lpjfpzeb.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3hndjxlyo.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3tpfjnfbz.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3owuelgtf.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3bwvqycan.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3djsrllzy.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3fwphsglq.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3yonrhlim.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3zmkqcigv.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3hazbjdpp.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3arrlyghk.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3hijixump.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3owkrxpfi.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3juuwvwms.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3jrqjxwnp.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3znshabqz.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3mduukkim.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3mylkoufq.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3wbuubqfm.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3qfqozjkm.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3jektmenu.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3wajdxsbs.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3uresouje.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3aekxkpag.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3mnqdpnqm.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3pmvmihja.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3oxqgdlbh.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3wqbwebnn.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3pleqwdxp.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3lfxlkiqk.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3gszsahac.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3lwmdjeze.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3ucaxratr.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3smbxjjcs.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3izkxvadc.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3cvxltrqk.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3otewidrn.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3nbbqpftt.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3latkfsib.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3cbohzlfs.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3krcrikqk.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3apxfonja.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3kzpgxezu.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3strshqtq.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3vjkyeqoo.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3ojpwpsgy.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3boiaqzxb.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3ciadoxyn.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3kyljdxic.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3adezexmn.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3oxmlcgwa.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cwbqksbl.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3pcbhhqup.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3iphuzztg.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3wkisnznl.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3nxtmtwsp.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3jljuuyxj.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3gevowvhb.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3zdrdjktc.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3nxaislfo.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3xrvuvpov.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3tqfpmgrp.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3frkanjjh.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3orqbscnq.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3tmoqadhh.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3zxjtjrgw.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3krbdbyad.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bkfynkdt.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3pgubwkil.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3onzxpfpp.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3szarxnbc.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3dxsrcyot.html


<!-- 参考信息 -->