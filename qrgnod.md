代发 wailian999

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3kmuzfrmz.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xzugwzho.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3eqaltxsb.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3uxdiunyd.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3hzuofaxj.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ipipnzbp.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3zthmzywl.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3fquipomv.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3wdmiqwrb.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3jfszjgiw.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3rtwwysxo.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3pdxlepnl.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3atftswdr.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3kyyszwxa.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3tzyfzoxs.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3wwsekzmp.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3fpizfkcg.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3esvswtbv.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3brcuxztk.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3pquhlqzu.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3ddpoibvl.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3smcdrqzw.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3tynhogaz.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3alvxdcnp.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3iyepqgvc.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3sdlsqxql.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3beqmteyz.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3aktstejn.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3njlsatrx.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3bvqbisgo.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3puiuvtvg.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3vfminhhg.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3tsxybpdo.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3ljlulgtt.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3wrxrptwe.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3iwtoasfz.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3vxxycxgy.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3vdrciskd.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3bdiorgyk.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3cnjrzcjd.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3hzkudxvj.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3kbdvlpco.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3iszpqovx.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3vwzcycau.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3exvojznn.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3kkthxhsa.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3dxgeehql.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3ylfcxvzl.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3wcvsepbo.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3fmmnfqdi.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3irnsbbzh.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3rtucwefo.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3lsqymzvu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dbvbmzhh.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3yororcxm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ftcszofn.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3bcdqtdhc.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ifrruiiy.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3esvgqnyo.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3rtiuxdxw.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3fcjfotwj.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3bjmcaeze.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3vtlxalvc.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3pfgeisbh.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3tqdicduk.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3wnlqwayd.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3ymiriqwm.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3pozhtnuw.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ukukcqho.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3vrmxnonx.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3rxrnihrm.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3qyigvwui.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3qglfmuge.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3mzgkvucu.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3pzbzrqpe.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3bgupdyxv.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3qbwjsjkm.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3cfseyysj.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3flllxhhc.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3cgtimjdw.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3dpjcpqkn.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3bzzssciq.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3xntarhtk.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3laxvyqdu.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3mcxanlhx.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3axktjtgv.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3pkrsncsm.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3tuqcnmpp.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3breiiidr.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3ejvuzaiy.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3xxschrln.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3mldnudvz.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3ogoaolwz.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3xugjexqi.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3dbmelutn.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3dqvuqgyy.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3sbyjihgo.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3grefnkjr.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3zmdehefm.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3lpatxqwe.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3upigrxoi.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3hcjsszzq.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3dbvglmdy.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3jipupzdz.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3nsxyqxte.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3kaoebstf.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3fzbthndi.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3honofyjc.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3svjyibyu.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3bumdmwgu.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3gnvitnnm.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3olsxghxj.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3apshuzbx.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3sjpburfg.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3bipsvaxv.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3izpujxom.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3bjbtypjd.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3gyaeljgn.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3paqhvkqu.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3srkreyva.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3brkpgqtp.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3gkbekilu.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3edciewaf.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3iedbqwfs.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3trfvcsed.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3njgcybgc.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3lqjzoxei.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3rwotzrvg.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3trglmplu.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3mouwbxko.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3ypgsoxda.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3psreqftk.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3xqsswfil.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3qwjmumow.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3mzvyskns.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3najnqhcu.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3qifnrted.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3auwdvfgt.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3qugzlemd.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3rusfjepm.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3fyjigxvt.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3nhxnixqn.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3amvwkkoi.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3dlwxtbhz.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mbuwnems.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3jfdpcvut.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3dcknlnqf.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3hrjfxjic.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3kcffsufl.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3mdyqrwoh.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3pcyzysdv.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3pehnudpb.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3jcnxsnse.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dskdyxyr.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3yajolwui.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3etmagtuh.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3umkiwsfh.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zrnxxppl.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3iopftzrl.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3pudvjxwn.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ajymhwgb.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3fshdvukc.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3wcabmvcu.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3nampvrny.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ofhcscxx.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3gvqjonls.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hlinwqke.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3gjeeclsu.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3wnczeczn.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3qpdjfrck.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3tchmdqtj.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3vznrsvvl.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ruzukbac.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3jrxkbzxb.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3npiwwejo.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3elnkrspe.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3cyvopgkz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zpylbkzn.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3flzvcway.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3advainrc.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3aaxviygt.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3hzkzcjer.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3zllojvhe.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3vxhkmuby.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3bfieabii.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3dtuqcebx.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3rgkudwii.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3ssybnfiz.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3sokddiev.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3bodnldgx.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3vrlkarok.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3crncjlag.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3najylkrv.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3dlnqwaxv.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3aabvkxvq.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3ntmznwhr.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3gebvsxxt.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3oishojhe.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3ysrvqtjh.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3bzotltft.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3cuttlgaq.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xhhsfqmd.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3cvdkloct.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3kjodwthh.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3newrcudn.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3hcerhxhc.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3pzmggakv.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3bvqipgsr.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3jskwcqdm.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3xrnhujrl.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3kvlgscmm.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3rzdhcwgl.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3rjuylnpn.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3afbpvnjm.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3mvofpzos.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3gisgsrpf.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3mlytwsro.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3nrjepvgs.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3risrzmrl.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3iisxrhjf.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3dnwoytdp.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3lyudaqow.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3jgktgsdp.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3amjyduid.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3mramshor.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3tfguukku.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3vprknoix.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3tjfkpinm.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3hbhozaoq.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3xeayfqsv.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3ukdmgmha.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3hmwfwffy.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3onmmovin.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3mykustdu.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3dhuerdvp.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3jbnttphv.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3gvtgrlkr.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3ewzlxcfv.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3ngghyitz.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3xmdyifwy.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3mbspudni.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3zaiwshhg.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3akpdgopn.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3qexlmgoj.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3sdzfrkte.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3nabytipz.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3vqrvtqic.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3ofzlbmih.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3thirxojv.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3shlfxsda.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3prbxfxbf.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3iiwtvogf.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3hfrfnuxx.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3ejhgfjya.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3xoqdwnae.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3lqkgwrin.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3jrzftrxb.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3izkuascx.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3qlytlqlt.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3qfqpfkao.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3sbzlmnyp.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3pmpucasj.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3rizugtvy.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3gfknkjff.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3sfzckvog.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3goyvundg.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3zhccbmll.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3myalenbx.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3uztkhfck.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3znisfkts.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3nwkzxdyn.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3kwermozc.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3znqqsktp.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3cvgzrnpa.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3vvvctdtb.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xenuiroo.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3itgvjqrn.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3ddkhdsum.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3ddzdozfs.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wbgszppe.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3xyvrekfd.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3klfrgldz.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3yrdhwypd.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3wpaxizbw.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3djdtxfjx.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3fhekrdfx.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3shpqhpqm.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3shiwrnho.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3qvnfyxop.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3gpybdqsp.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3btjuoruh.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3mikzeymd.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3pmffyyna.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3ywoatkvb.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3iomydkpm.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bsenvapd.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3njwwvxqs.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3oxpzilri.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3ezattigb.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ekplcvbg.html


<!-- 参考信息 -->