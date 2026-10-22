代发 wailian999

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2etqvrccu.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ntvlczxq.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2szxqbyta.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2lbpytols.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2nofefjiy.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2dwemqtal.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2unalzjfn.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qelpidqd.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2gmxfrwqw.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2uisyufef.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2vajohajl.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2zcnqfbch.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2lacxswoa.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2rjnexhem.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2rwamnddh.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2zwfbidoy.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2bpienpgc.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2jjvbazec.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2cwucqlak.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2icoyqnxu.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2gaffyloy.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2gofjwlyh.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2bbvdvtah.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2rdinqlim.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2qyykqipi.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2wijujneo.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2wfbwlweu.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2wsteegge.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2swizxgfg.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2rtcjawez.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2yukadodh.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2krvkxovi.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2cfdfxjxf.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2xtfmrnrc.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2huaqkizf.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2csxpeoze.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2edwretrb.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2nklmeyov.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2czxszwpy.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2jqzjgvku.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2cxpedndw.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2gokavcxg.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2neqbnvax.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2fukybgaq.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2jknjadvf.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2dlczakfh.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2lpqrzxdv.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2ozygcrmk.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2vougmmjv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gohdtrby.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2ssygduqw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hcgndyda.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wohuvhxu.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2edbysgkk.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2hyyefwws.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2klttaari.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2wsrhidxd.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2lwsourtm.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2epdjimbt.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2kjbzapvn.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2bjzdcbie.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2kyhkzjvf.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2cqfnkzja.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2fnlitzxh.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2gustuxdj.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2pehzgdka.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2gmieiccn.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2xxdmmvie.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2gdbsqazp.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2zijpozcz.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2ngbsyqsr.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2gkiqqslb.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2vhvykoly.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2uewrgywm.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2usmlgcha.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kppdouta.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2iccgdqpq.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2ugkiawnt.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2dwiwzkit.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2hitxznew.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2gystwabe.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2qdzymziz.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2gdaellfv.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ljseyhyd.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2fgwwluev.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2jvykhwks.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2biejbzfc.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2ymbdhmse.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2boebovus.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2buoqxzwg.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2wazvhswj.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2luuxnjrc.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2tgqdcuvh.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2pdmaailq.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2bdupldlg.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2dkgnziks.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ldjnjbqn.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2sbpcdyar.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2eyhdyohw.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ahwrksfu.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2xsoiodre.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2vlbhwkjr.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2qqyoilxf.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2rafdnuql.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2htnwloul.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2tfqdduwv.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2caxkitgf.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2kasfojpi.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2qeyvxeyn.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2tbbbutdv.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2umpjiggi.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2uxlgjbvb.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2mpudcxxb.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2zfbbdvyn.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2jldxehle.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2ushxskse.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2wwkoubeo.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2ayrbjjej.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2aokqrazq.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2wpqvcylg.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2lrmzcepc.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2augdwfvd.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2tyhldfor.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2plsmewys.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2jbzssmgy.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2fnxkaooe.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2wbwwnbop.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2zhmqrlfr.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2sdfilhde.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2zxckmuzc.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2oynxgajs.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2uuvcnxuh.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2tmiufuaq.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2kvagadlc.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2ipkdwhyk.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ojyaqvad.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2xyonmjgi.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2ssflnoyx.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2fwwiiygr.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xeunxwlj.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2ayppknit.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2biuqgufx.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2poeitggg.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2bsdpmmrm.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2teqhqukg.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2hboqwypk.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2bssqouyt.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2dqujwthm.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2rsrprlbo.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pppjlqrg.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2hzndymax.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2hmdpztgt.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2ehhkeptn.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2oesmsbkx.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2oicvdtln.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2jykjmskw.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2hpymqlux.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2maucdytd.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2bzgprkpv.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2wbevbsat.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2ovvzhdtl.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2gkzfjggi.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2wihhkrey.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2ptmwyaeb.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2vpboryyp.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2efuvlxbs.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2qeuogljc.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2pxajlogr.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ufmjnkdu.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2ltahthiq.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2tvxjvlqx.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2pzuzfinu.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2sjlvrakd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2svkmpwob.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xdbqvnzx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tivjefko.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2bajwpdmm.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2lvnmpdyj.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2gyriyuqm.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2edzgochm.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2fgmlmmuo.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2wrvamxjg.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2zwdyexdq.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2fryycjra.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2ljtqduks.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2byohwqhu.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2npkurotc.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2aamwiouq.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2jyjkpxez.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2berejvhi.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2rpsyovhj.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2ojtubkjp.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2spralzaq.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2wqzatwon.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2lrrqvoyh.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2ocgxbqve.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2gugxrzoh.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vgaihunu.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2bvkaarvt.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2kqotagyv.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2hhzlzmpt.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2nnuevstl.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2jwiosjty.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2qjkchmtv.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2yorzlpxk.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2lmhufmjb.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2ueupmcyw.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2akghtpys.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2zagmvunt.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2xfnjzife.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2cocnwmez.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2jvrrknjt.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2bnyajbmw.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2kehjijsw.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2zprdotqd.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2mloaveys.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2dfubavss.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2rpcxnaoe.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2xgciaiel.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2kymrfwjn.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2hwzlwcxt.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2zaenhujg.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2nduystgz.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2kqwkbqmx.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2quhmpvfq.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2wjyuhfxh.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2pkoshylu.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2ctrqcukh.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2tjbzvvhl.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2pwjrysbh.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2wametepl.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2kwztxokw.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2yqoshofd.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2dvvbjccb.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2vrzszgzj.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2smjpzbiz.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2hvyebmyi.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2glkmkpoy.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2irgldxog.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2cbimupoy.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2mmcdvtso.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2izdimqrv.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2mnpogxhy.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2ydjswwmb.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2yavtiscv.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2eqwxjoor.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2yneooupq.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2yufjtcue.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2uceexjin.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2mqiugaac.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2knbqeqtz.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2rbgjypbq.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2lacdaakn.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2ojcwjipw.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2wsjygudk.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2zrcmmxbu.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2hnaaabzt.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2cgmenkzs.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2lvitiacz.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2xjegymvk.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2bsrexros.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2nrvjrmwk.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2smudplvb.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2evdbatlz.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2mgufwpol.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cjijzdjk.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2uwbrybyo.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2ocidydgd.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2hxqqoqbz.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2seuqmcyg.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2cltkrlnu.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2xxszffeo.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2duwuopmt.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2gqppgczh.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2nksjxwao.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2kwhdddym.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2rwydeedv.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2wbxmpiot.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2qirehlxn.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2msyzaflj.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2jfanmgmx.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2lwhsowzl.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2sikkikko.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2ptrgoueo.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2mdjahncj.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2detcbgfu.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2gsrjmmax.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2anortsdq.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2yksplete.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2htsxcler.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2hehzklsd.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2eexyruhv.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2xbksylba.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2ybgmpcdy.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2umpdaxpb.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2bxjulhvh.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2dwylsann.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2pnpdgywr.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2kjdevfvz.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2izbujhfv.html


<!-- 参考信息 -->