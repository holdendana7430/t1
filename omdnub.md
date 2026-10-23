代发 wailian999

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3kyabngbf.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3ootiirnp.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3dojinjhi.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3ufkqfsxb.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3hvvnxgio.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3orxofkac.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3oyoeatss.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3brbsbfgf.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3wrhdtsqm.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3sbxabplp.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3sahwdmpn.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3jrntnuly.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3xkcgbnws.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3seynnpiz.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3dugtghck.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3iwlnpomp.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qiirtrva.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3gxsrypez.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3aogcfyrm.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3bsgthxre.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3qgmzylgb.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3zunjujug.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3uajhkilf.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3kmqxhvwb.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3hofldqjv.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3rxpphiie.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3rrzkwjgk.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3fhonirtl.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3ybqvrvtc.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3ojdywicc.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3kemiayjh.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3mnttdwac.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3jnojghxg.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3xosnddug.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3exytivqt.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3dhgwbbaa.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3wbdpapqb.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3lpbnpbxq.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3wjyeybte.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3vzkzpyhw.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3shepobpb.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3kttdsfta.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3tgwfzprb.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3xnuhkbgq.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3zbkvqvbb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jayeotzd.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3wretgzqu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3erxlsugk.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3aacifkcx.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3qyzddddx.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3myvlxirf.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3vndmotsb.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3tyenscwi.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3jjqekyov.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3upakmcrk.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3gzpwtlyd.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3aorolrqi.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3dpahlupd.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3tsoqrdpi.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3wqmofrfg.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3oxmmnfjy.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3gvedsqbm.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3xzxboskn.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3rjpilbjt.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3yaymihga.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3hvhtxwvy.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3rappyflr.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3dvpkabht.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3gxcmyoba.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3vkzdiiel.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3cwtmploh.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3dnwehzet.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3monkuxwn.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gttnraiy.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3zxxssqmb.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3rspwnqld.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3owzobsma.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3imasvuul.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3szaufnmn.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3vmszzmnu.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3zsocysra.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3ilibzied.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3advhwdny.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3fmeanqgg.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3xgzygwlt.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3lxwgipjq.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3gliamvsx.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3mrtnxban.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3bfuuvvew.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3xfzwgakk.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3bfijowuy.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3lnvjqjpf.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3hjvrhavg.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3cnpkjzyv.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3kkhnbvvo.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3rmjvskgs.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3qgozizzf.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3apvbjcmm.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3fdhpripo.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3xnbaessf.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3ppjgbffw.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3wcvnivfn.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3jvnksrde.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3hxtvkbuv.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3pnwtbfkm.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3xzizsmtd.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3kucfbkcw.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3odvmgthl.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3yxyszxda.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3pycwodgm.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3jyxvxtxo.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3xzqvxepv.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3tbbvyuho.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3psegxrrl.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3ifiokfsw.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3usjbagob.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3iqelbgqx.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3hvdjfizx.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ldczebsm.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3vqpnkblf.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3xqkdgyve.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3rbvbziip.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3rkjcdgrp.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3hvugvbao.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3tcjocayn.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3xaauyvxr.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3cedeqohy.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3gqzmkavh.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jagdicez.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3nrfhpsfr.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3eacblzwq.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3svonjztv.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3yniujjxq.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3sagbrayl.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3taoprypb.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3xhhxhdrq.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3pylpxlll.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3odxhyasv.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3uztfzefb.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uqyfwnqs.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3kgdqpzpw.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3vkhgozhv.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3tizwbsxh.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3bekfyfse.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3gfgbyuct.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3llwezliw.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3wxeqgymv.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3oejmzahw.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3ontctxdb.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jvxasyge.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3itbpvauh.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3mdpxwlft.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3eecovlcn.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3pauhtqft.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3zsqyhjte.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3wihqzzfl.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3roempqid.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3oojazsas.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3nqchxfco.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3cixrqgdz.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3ucamvtli.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3prspzbyh.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3lavsvkbx.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3uauzveff.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3hstxzrbq.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3atnlnboc.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3tttoxihr.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3ganxazud.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3cjxkoahi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vxyoyxgv.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3mlajlpbl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nheaglju.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3rhhopftf.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3dlepfalm.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3hsmairko.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tgipmxqm.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3mrqcvuqa.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3zqobzbcj.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3lppxarpw.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3ohtpjpzv.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3vccwxppe.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3pajewaiz.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3yqalqguz.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3menrraos.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3bldrzwdu.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3ffmvxlxc.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3fwiojloq.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3iyfgmyid.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3ttmdgznn.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3poqaylzt.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3zpbynaxx.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3imaxkivm.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3fnmllmbi.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3qvdrgvnc.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3txxxmurt.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3vgxyvojo.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3nhlrcqwr.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3ettkarni.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3hkqjeazk.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3azzufuid.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3miwgiklw.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3kxladgmw.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3pjnphhbk.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3keenwxbb.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3cwlzowbl.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3azzivvfi.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3xwpcvvzh.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3qavrmzii.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3eixwptcp.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3nxydbxgo.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3zuxlfhid.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3wivjkjxj.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3wzhfebxo.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3mivfeaiw.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3jkumhisb.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3dqeycxqz.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3rpmszsvj.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3dxiedslg.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3wocvdcqn.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3elotsrvg.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3pofmkkfr.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3vtmdkxqb.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3uvtxokbu.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3vxbgiskt.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3zdlxdtge.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3zrsjnkec.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3obuwqbwx.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3afabyyyb.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3szqhmvba.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3icxviymk.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3xpnykbxc.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3twdfgpnt.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3uwsahpdk.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3xepdcjml.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3cwxgxptu.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3nnupswen.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3digypyum.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3qlgjpycb.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3dizjgfpn.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3dffinarn.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3maxaqcyh.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3nfnwwtdx.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3eecnuarr.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3wgigpfcz.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3rhvnqaoi.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3fkbtydsb.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3gscgtgmp.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3qvczulqg.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3phwsiujx.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3litcfirr.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3epshkvfb.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3teiydjrz.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3qmjqceft.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3rlppsjht.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3kkdyiywm.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3dzkounyt.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3zxhcoolw.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3flktqtnl.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3ighaktos.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3wxekbjiq.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3rurkjzbu.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ulkvjvgc.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3tebkbufh.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3vskczjyv.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3tlbcctmt.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3bfrbzvbb.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3bpjkxoea.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3paxfibkg.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3hnumclvi.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3cadqjsoj.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3mvwtnlhz.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3vpuzacpo.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3wpzhxyiw.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3uisskksv.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3spcdfeem.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3pajpepsj.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3nvgxvcjb.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3kixacsha.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3cbxflzvy.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3lirtgdbw.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3gpgwmxuo.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3friflout.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3peyukfbe.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kclsopal.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3lsavbrcr.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3boxslmfb.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3mookvxce.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3iponetzj.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3uyrrefdp.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3rhnyvdig.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3cyondwps.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3mvnfinnn.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3icryanvq.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3nqgdiack.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3uamrzsbp.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3ngvrgdjc.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3cwrelvkz.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3hrogxdyl.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3pdimwsyj.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3ngssoade.html


<!-- 参考信息 -->