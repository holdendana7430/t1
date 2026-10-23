代发 wailian999

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3orgcnfcx.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3axxyauvh.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3llayzmco.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3giqdwjvi.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3qvsdidse.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3ctlhsdyl.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3japtsgpf.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3kgtffmdm.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3ystchmng.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3dptvygeh.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3cxziifav.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wyvtivzl.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3qghvaweg.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3qshkttwi.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3oircxsry.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3nndgpqqz.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3eblbqxtn.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3vwcvduzj.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3vlyguyua.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3veqeaesl.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3mbjjwcqu.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3smrsreoh.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3gtcemuih.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3nhyacgji.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3danfoghc.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3caovnaxf.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3gmkwupxz.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3gecohjqu.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3hsuqtufk.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3yamyfcik.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3bffgpuze.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3vfcueqsm.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3kncfeawg.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3iwpjzyvy.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3wjxhnrty.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3ojmefval.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3odfoluhm.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3zlziekvu.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3prnmwwkn.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3pbwdxisi.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3hfgqhpdb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3trbjmsna.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3zvvngrtl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3njuqlzgb.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jhshkodz.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3lpnxssuu.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3fhndmfqx.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3yydmkvka.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3asvilafo.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3nlsqiodm.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3ckggtgto.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3exvvxjyo.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3shpbefub.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3voxbutmr.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3glysmvhn.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3gppsdpii.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3rkzmfujz.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3ffldwxqb.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3ptukdppz.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3rqietgmq.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3teoqvbig.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3kwgguyfo.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3nbaoowkq.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3tkouxzfl.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3dvaywito.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3pongstxl.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3xpzpnigd.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xtfuzezx.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3oikmlyaa.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3vmsmqfqi.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3vakauwzt.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3jlfxycdi.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3wgtjrtth.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3fpvxdwdy.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3uwjewbtx.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3fbsrbkyw.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3atbbtyfy.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3bzszqmte.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3hksytwmo.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3aamzzdkd.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3gqxhfvsj.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3xtznxulv.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3gaxszvxm.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3votltdat.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3gtyzeuhi.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3ommxwblf.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3umufbpec.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3krldphii.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3cgaiorqm.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3krhgvjrx.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3zrikcxnp.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3igohoxkh.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3gqwczjbw.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3tlpowqiz.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3vnyutlkd.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3cvhqmgyl.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3ohjliqmm.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3hdrphcmq.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3qfblqblk.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3ukawgqkw.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3hjepdixy.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3kjliffku.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3jswtcmsm.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3urhmyoai.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rlzczqtq.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3jrdjjsdo.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3mgwgypuv.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3zeodahie.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3vssxpqhf.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3oorxkyhb.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3rhrualim.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3jqrchrop.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3jskhngtg.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3vldrlupv.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3swmpsrkz.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3koqctlyt.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3ybgwznrp.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3zoicrwtj.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3gimmkwgj.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3ijbxtyqw.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3aiegjdan.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3qgolvwqr.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3nlbdbfth.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3ravwiuxj.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3soqzyjvb.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3glrailqi.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3kjaxjyxl.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3vcmcbnvl.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3kpcovvud.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3sdirjank.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3qbdschjo.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lqvtejkl.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3dabmsrcu.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3noupyrlr.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3yrmptnjs.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3opjzysti.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3hacrhtxu.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3ekaqilie.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3ozvtkcie.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3sspqraoi.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3epveslvi.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3hwucxhtm.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3zudriqcw.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3mkefuywf.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3wvopigkm.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3bbuntjen.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3upxixcnu.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3nogkotae.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3uvthdhxh.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3wcjxkwvp.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3midtfwif.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3ixaioxon.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3xuenmktt.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3sujbxmhm.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3tdexbajm.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3iaqhekru.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3xdiccsxp.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3yrivvosw.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3vfhayfua.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3tozivbsb.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ogelevts.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3qjcapagi.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3vlvmwacj.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3maigveqh.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3lfmfyryq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tsotozhy.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cnneqamn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uidlwuqx.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3svasuvkc.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3pzpbhdjb.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3piqlejwc.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3llwqmlqc.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3jjqaewrh.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3lkshkngv.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3bcmadxuc.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3siyoxifz.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3rdhcbxmw.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3zdkjugjh.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3rrctupcu.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3srknaffr.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3dovzyanz.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3bybwctqz.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3fpqqkjmc.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3emnthxvx.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3vydbneqb.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3tailgdkb.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3eqxsdodr.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3bqtuupkl.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3uwgrecvv.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3pswxwibo.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3crgukgew.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3bvzqdrbq.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3jdtanglw.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3nbknpqge.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3zlvhiumb.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3vbazfpem.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3mbnoudiq.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3oulidiuv.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3hovgrexs.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3shnjwajw.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3khxgutxm.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3nwzptogr.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3vsnvrrmn.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3gdlzdnbq.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3mukxukjs.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3zsxagyhc.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3riqxwwlf.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3sydmbeeg.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3yzzeimzd.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3qeonzngi.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3ojxnqmua.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3ijhtnaqh.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3nuyvhdru.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3kawurgik.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3mjudqoeq.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3fknsqtnl.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3hftemxmf.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3jzmzhqor.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3hjupmxvc.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3qkctzflo.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3ztgrxpkp.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3rzocfvhd.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3jfyivuvx.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3owxdlnio.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3bfhquwvu.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3gsmbskvi.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3wdozhbfd.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3aotaadxo.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3bgvlxkof.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3bgqtnqjo.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3mkiolnef.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3ruuyozsq.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3ncpdaepz.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3wrttverj.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3dbyoaalh.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3zetkfpqg.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3ctsiydfg.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3ikicucyw.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3treewkim.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3kewihpxe.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3pxanavzr.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3dirpqvhr.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3iwejeftd.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3lgiutwqi.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3bwfzlqio.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3lyfoqrar.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3bqsbpgre.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3shdbdhda.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3hwunvkmz.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3tvrwppbl.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3awvmuwph.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3tbbrjcil.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3dovdeymd.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3cfruuslq.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3oplgzthf.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3xyvqwpzf.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3jqlcndbe.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rxahcfzz.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3jqdskfua.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3hqoucjel.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3iouxakfd.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3uqrdqugm.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3ikyadbin.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3endvbieg.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3hlwidibw.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3naaiqfct.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3irasgnyp.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aqeaghhz.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3fsrbeawt.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3bffohnzx.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3qdtagkpy.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3ggefyrer.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3ubzarlki.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3brnnepej.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3gawjabka.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3wmlckiwi.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3lndenqtv.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3bjyeudgu.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3kaxaykrt.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nypsjlmy.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3wkmxoucy.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3snyrnuhg.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3xhvvxvcg.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3peqkcqvp.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3lakbgvvm.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3jscvvobo.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3cjjjwcne.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3hbwxscwe.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3jwornhwj.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3xycreovk.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3hhqvzumn.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3lgiljehq.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3heqveztt.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3afqjbbvj.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lrpxupay.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3beejegsq.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3rmdgrrqn.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3iepfijif.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3lpxeftbl.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3rsdztyet.html


<!-- 参考信息 -->