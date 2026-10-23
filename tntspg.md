代发 wailian999

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3ajuqinit.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3bvchgeiw.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3nnccmcfd.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3izdjsqos.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3dszflpgv.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3scyfeguq.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3wqvjwvvr.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3hqjaqqik.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3vffmekyb.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3qffbylch.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3gmirlqzm.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3zgstjwix.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3ivqmioss.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3wyblgqfo.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3giisykbi.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3hsgsblwz.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3puhlthtm.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3kjuvcqqw.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3zpwgxbzj.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3etamithu.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3tjmqacue.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3qrradysi.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3rtdmbbyf.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3ahgyfvrc.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3guubtnil.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3krzshfik.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3xfjtypai.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3beffkjem.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3tejmaopf.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3qhsgciqg.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3qrhamltc.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3svwjksdy.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3intqiorb.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3fhdlcrdg.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3qaixvimu.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3tdmkkhch.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3xepvmikq.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3mdfcvwbm.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3utuxqbhu.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3uyrhhxfj.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3jcvgjyda.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3fnjdivze.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3dmnqoyrg.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3akqcrsct.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3nagzyfde.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gpyhycbv.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3jguupava.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3husodfro.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ccnlcjct.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3udixecbn.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3qsarzqdz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3ractaoey.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3wazfrswp.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3cjqnahlc.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3vqnafshm.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3goidbgyu.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3wbkuyykh.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3jplhdpue.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3jlicnjtd.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3qzzgampj.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3dgfpphvy.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3mthvhkgw.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3zkytpfvc.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3utdqfzzd.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3wjcudpxj.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3qqohrido.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3ybqydevs.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3icxpzffe.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3jhjiseyz.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3ndgozexr.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3gpnzkbmi.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3tshuoebj.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3ukhxkxhb.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3rurerwxa.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3gljcxozp.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3guxcaxad.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3gcuiaopc.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ybkbviju.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3fiuxtmbc.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3cgbvreko.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3evhneymc.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3lajaemxn.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3fpcyopxg.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3irmumciy.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3xpxrzult.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3caxogzxg.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3eymgowlx.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3vszyhgnk.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bkpdfhdp.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3evrwtqoy.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3uckjiwtn.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3ilbklmac.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3kbuyeloz.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3hdcujrgt.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3comhzhuw.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3wxwgwjyu.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3sndunilg.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3clzzzveq.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3vkugwdmz.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3yxqhflet.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3kpnhykda.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3skumnoic.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3etxmnlwp.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3yrmqhube.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3gmkiwllx.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3sprqzsyy.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3coarpohj.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3zzuxsblh.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3kdizyjju.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3wplphfbk.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3quvsfkkq.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3fvhmgzov.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3cesaairi.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3mkxyfjoc.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3ahlynyhl.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3rlgdtefo.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3kywmlaoq.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3onjmwkuz.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3vklcmyzl.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3rsioodgq.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3jwixxzpa.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3wfjirxsw.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3twbmneka.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3vrtvyfxa.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3cpvhhilv.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3zymmwpei.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3hjqktzrn.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3wvoeqjnc.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ikwtgtsy.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3wlovrxys.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3wdofmuoo.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3fntlitbl.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3fgxcajbe.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3qoguxrwn.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3sqzazusu.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rtytzhyw.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3ljwvyqdt.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3owvnkfro.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3amtvupvj.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3oepftckm.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3zptmbgls.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ztuexncp.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3vxkkupbu.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3udzmsyfl.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3twtqvbdi.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ealusupt.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3hxufcwwn.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3tsloqpai.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3uxzdngzc.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3crpqiphv.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3dpfhkcyi.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3rsawcwew.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ogjepohh.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3vnbcpzzk.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3vbqussek.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3ztfnpwqt.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lokppcjh.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3neawdwtb.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3fbpqfhbh.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3dwqwvzbb.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3dwxdudis.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3swjcmvya.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3nkkvhyae.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3dtnmtjzj.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3wfdgmlfj.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3wjdpgwle.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3bndeqchz.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3kkzczbrz.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3bwuguttk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vtrrbomb.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3laapkgqx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wulzicrp.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3vohadatm.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3faydnmeh.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3joxpwrlg.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qderbefb.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3xtaalrkc.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3nqxebqvh.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3esbzvyqb.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3pnjouwdr.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3cwabvcmq.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3hxzizpxw.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3syrbqdax.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3qnozghlr.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3mupolvlu.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3lpmevfne.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3fsozvzok.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3sofdiyrv.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3crwwhxet.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3kwhzgmwh.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3fkrdwmbq.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3iygncljm.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3evleqyyw.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pzimdsda.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3zdqrdowg.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3vdcvrzdj.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3kwumgueh.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3ocepsrrz.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3gzlvuacv.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3eeappheg.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3vrytlvvc.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3zlpbkmry.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3uabzdokk.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3txfeqgfs.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3hlzmvcuu.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3yxulvbqx.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3kplfqfer.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3fsnwwjnv.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3rguvxupj.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3jnwhafrf.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3xbykojjb.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3ynptwthi.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3qmybunqf.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3trtufrts.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3dxugvgiq.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3goxytrud.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3wpmqdhms.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3yyaoipqc.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3ypkcsubg.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3ikstvssj.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3ejwudqtj.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3vkzrakla.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3qsbxiatq.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3kgexvsbo.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3semvnhbh.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3glcclxsn.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3crfgihpe.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3enasatdk.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3igjzmviu.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3zqttztcm.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3usdwpbsa.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3ovskpboj.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3qdenoabi.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3vzhnthgh.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3gymvrhwk.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3nxpltwso.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3craaerad.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3ybsiulsr.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3fhisqiju.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3peebbxza.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3dnvpnzfp.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3yydayjxa.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3cjctlnyf.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3ohhzudwg.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3nfhizqew.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3gqxrtgsb.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3uxccuqeo.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3tystbxjc.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3fiehpszr.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3vgulqdzr.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3eoeuoize.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3cbilxwyu.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3sndeyjcq.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3czmsfvzf.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3jnfpfpur.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3lvmzcjxl.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3ezfwsqxw.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3laypwzny.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3owqicbtp.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3kbsknhnt.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3wgqkumjp.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3hnxhdwex.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3sqknvowa.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3erujhthn.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3eiktznid.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3wdcwfejm.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3bbjjejyr.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3mkpnmvmu.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3zczpoudh.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3mvbpimgc.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3vxuyibwv.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lurndbgn.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3ettbmuxq.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3iydtkuii.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3hsktacrm.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3buuwoees.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3qxfcgpac.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3cygfhlrm.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3hjzusrqq.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3wteblrsm.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3eafasxcs.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3uocovgnv.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3uzeoxpon.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3nmdsassf.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3tiyafqyd.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3ijetzrke.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3cybvdnru.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3mulpencw.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3nkkjykfy.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3giwyqxqc.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3ilyqhkpp.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3gpjoedpu.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3ntzociet.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3vxwsshvs.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3oultaysq.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3bblbbkhm.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3qyvrcpqj.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3znmeuhfm.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3rayewegk.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3yvxsgeqg.html


<!-- 参考信息 -->