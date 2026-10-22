代发 wailian999

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2raidblqc.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xaanzmyb.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2osyqqbdz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2xyvbkjhb.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2torsksye.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2uvpzafxw.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2pwgbsrlt.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2wgwzbhvg.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2huugsknl.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2erbzwgja.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2qepzcudy.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kceytglj.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2aypmrywt.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2qqdhreap.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2ilmdotxc.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2xkqqtlog.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2ytwxvqrt.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2jlgdctdn.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2xapwquwt.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2zrtgocqm.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2zgmgxpkd.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2btdbqkae.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2rvttpzck.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2agkckbry.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2bkheaueo.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2flurbahz.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2gqduzuvs.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2jydfacxs.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2eplbtxfb.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2reziokgp.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2vkdiblgo.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2ceuiavwv.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2tamldjeo.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2izdgwnay.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2prnysrtq.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2lmamhppf.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2olezglgl.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2mpdpxtjp.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2gercotsp.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2zadytkfr.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2sakjkyxe.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2kmljzked.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rkbcnxqy.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2pitdlffg.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2sbbpwljy.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2kkzhygtq.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2fumrtvne.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2ertlhdvf.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2tmrjagby.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2spwafmom.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2tgiubsiy.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2plimpqzp.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2fypiedax.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uscsydtl.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2irgslyrj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oshqglga.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2onipbcdh.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ynskvjjo.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2nbktzara.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2hjbubrrs.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2wgsefgts.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2vhyqmate.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2fekvkurm.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2xxecmavx.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2fuemjvui.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2kbdtkcpr.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2tnwmbmtb.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2duimnnwg.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2yzhzaaok.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2cbawscic.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2lehhmxrg.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2ljchslwr.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2lfgoevpo.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2hxmhtysi.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2elzjimwh.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2doolnkjn.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2jtjapjrj.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2ewpzzdjy.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2glfjnrjg.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fderznji.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2vdaixioo.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2pbojcbhs.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2bxpwqwke.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2djiblodw.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2kweytgus.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2sohsmnkb.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2eaxumgyt.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2xseisiyc.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2vgccplwi.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2qalyisvk.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2eboaopkd.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2uxfvmjmh.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2nbtekbeu.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2kwzhbfms.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2ipzgjnqu.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2lcngtsyk.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2finmhjvj.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2fvpiwlwk.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2aijpjpfk.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2jboaopdd.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2xywphvog.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2xdrelrpk.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2njucmzub.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2tzgjtero.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2knqammpq.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2jjxcptes.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2ozgyztum.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2pjwmauqp.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2sudeejjp.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2stutpmek.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2fxxdbmbe.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2jublnbho.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2lebsjjtt.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2ivfztdvn.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2boxaryov.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2figzcfgr.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ciznswvg.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2lskerbbn.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2ncjzrsrk.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2ukfptufc.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2zakdbdxb.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2wrbtkhjz.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2uaokvans.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2qxxzzsws.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2dmphhwef.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2ldgxnncs.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2mjcwqzsq.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2rcjlegkx.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2txnasgxw.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2fiomrjde.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2ltgdcbdy.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2edwmpbko.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2hxouhggj.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2pkukioxg.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2wbunzreq.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2vxysbyfe.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rdnrwaas.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2uihhwzuv.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2duqbwxgy.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2uvlxscky.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2pcfpbjlv.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2rwrnqzwd.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2tcdakdzu.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2stwfgriu.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2svzyhdqu.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2wpizbwdd.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2zplmrhwt.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vnoduret.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2wihhzrwm.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2mxgeabtb.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2scrocmmw.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2opmhhtjk.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2osxzgzno.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rezcwrnp.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2xqoukykx.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2gdrjkbpk.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2lwnlidia.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2bfwioxbw.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2zmoigskr.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2bbzrhbaf.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2exlblzwn.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2revwvkja.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2frbtbiay.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2uaspgjuq.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ntaglfqo.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2ygucrbzs.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2wuszcojk.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2lngpjyjf.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2efwuzlwg.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2sjhrqgjo.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2alznvlgy.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2cbhoptqb.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2phsrydwu.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2nzbysebo.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2rhbiugzf.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2pbxptpfb.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2pxirebgh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mowvusfh.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2znmzngyb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jvodmylu.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2taveobha.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2tiietwbb.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2rmibyjju.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2hdhpzjzo.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2fnrcszjw.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2squijnzz.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2wtbvxmcy.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2dydpsmle.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2tkzdslfm.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2qsugmewf.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2mazlbscu.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2lkuuowgj.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2peuevgbx.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2lwwfkssw.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2uorpzwdm.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2uioyhxqk.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2qupdrgey.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2ssxjzzxn.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2yytyrprr.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2qbgkleiu.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2zqzuhjif.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2puzxvyks.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2dvpkbtaz.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2fkraceay.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2ajasbbsr.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2avnwgalf.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2pydmhjjd.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2dblsfoou.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2nhpzjrox.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2hybswvgv.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2irdtfewk.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2umjjxtza.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2djzcupih.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2hjfqczhz.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2cwmlpjey.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2wzrqngxp.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2qktobncj.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2izrmvasi.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2sqgblfvo.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2wofpfqeh.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2wgydyqqb.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2dgxdrylb.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2cqyiiftv.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2ciifmwno.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2yzqyukrf.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2bokmbmci.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2vhxwmmdd.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2ukizapvg.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2mqgikpfe.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2rxdneizk.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2igduradl.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2tkrwwaiw.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2gzkzxtwf.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2khwkbsdd.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2wiehyzay.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2bbzsnqgf.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2gcqlfcnl.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2kpsouutq.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2wzcczpic.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2bwfajqxv.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2pnibmlhy.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2rxyfunwm.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2wihhrffl.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2lzqebhwk.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2tywmnsqo.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2dcehtkql.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2fgxbhumq.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2qckppvpt.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2jcjzddem.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2hwrsdacg.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2ydfbffdp.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2xmqsempe.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2wroozaae.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2nitunwuk.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2bjocytuv.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2acvdwuss.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2byiceyxu.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2rzdqaieq.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2oudswlju.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2aazfzpoz.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2nstnexiu.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2eqxprkij.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2mocrjzpq.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2yrhlsqnf.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2tceuisjn.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2uvuhgmrz.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2ikesywwa.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2tfnnrzzc.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2cyiilygw.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gyjbelke.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2qgflrrvr.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2dylolyva.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2shxzmhzv.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2waqfakak.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2gjopkuaz.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2mnbnxrah.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2otvmzubu.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2pmfrriba.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2ixwumpaw.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2reehpeta.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2ibdyeyqd.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2jztzxqnm.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2nugkqaxa.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2slfnrjxy.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2soqnazml.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2avnkvigj.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2pyvsybbb.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2leowztoj.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2ktgcggmd.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2xfclasnx.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2iqwnqgfk.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kaixasen.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2jgzvfauz.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2csljgnbf.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2mjfnxqss.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2xydjzmzv.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2bnrywykk.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2xzkcvddc.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2ewguadgw.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2dzdomdkq.html


<!-- 参考信息 -->