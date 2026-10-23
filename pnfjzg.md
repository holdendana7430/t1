代发 wailian999

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3fjvxhxoa.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3ptqigqzl.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3vnrsaduq.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3wcooqdnn.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3gdhjuthg.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3ebdqdnic.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3heuyiwqb.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3tezzgdkd.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3ekvefxuy.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3wtyjkkeb.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3vfsiguas.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wfbacmcw.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3nfhekfon.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3umkaryda.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3nuqzjdeb.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3stauzzzh.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3tmsljziv.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3spuuvjvc.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3zhkavvwx.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3nmunelhj.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3zexzzstr.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3tbafqgib.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3lhbprebq.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3ndwnaybw.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3mmoojdnm.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3fhfizkad.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3iwwbfglm.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3yrbpgllq.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3mnzzhexu.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3cggpdbwl.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3upnnpkbt.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3zdzasqjh.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3gxwwdmpo.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3picbxutw.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3trqdfddm.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3xgjiobmq.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3uhfyvdky.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3bloxpzlc.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3fdsqnucu.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3vsbpzmqg.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3poieogmo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3igmxyhoh.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3xzdbgwkv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jglvxmtz.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qvadduqo.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3qzfvfswf.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3swrbujue.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3xoaknqkb.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3szackgyt.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3ecwbtmyr.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3ktyittwk.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3jtcpyqrk.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3fqauujib.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3hsjdcjsk.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3iwsuupxr.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3aompwwib.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3gvjugnfp.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3ugsbpqox.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3naejxvws.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3wtzljiyv.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3vvpayqfz.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3tegntvjb.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3mmzlzzoi.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3aozhxdyb.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3igupzfaz.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3jlrakxwu.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3dyigsghd.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wugavikv.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3wqahpgmc.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3olerlluh.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3ukelerct.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3kkbpfyhy.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3weovnrkw.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3gzgjtjxi.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3mdrggklv.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3uunlcoix.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3byxtrkaa.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3ydizeghb.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3xkbfdkxa.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3wtpkauvi.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3iagbhikm.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3hsdgvcal.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3bipsuisw.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3gqzshzsy.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3kyenurtc.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3gjzvezsx.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3qsmyxsob.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3mwpnnhpc.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3osaxppmw.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3vuozhsug.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3fpuvvwjq.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3uuyvelpf.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3zifhxcti.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3zocmwuhp.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3wchkdfuc.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3zrexaeiv.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3xblaokes.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3gsgwzzjp.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ptmzdhof.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3ipvvsgip.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3nsxbfzdz.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3ykunpzxq.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3fivugeqi.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3lkkvjkfr.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ofnfagbs.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3lollxibc.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3axmkoclt.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3ztbwicuf.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3oykzyuos.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3ihuaxviy.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3vdafnuem.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3nluxefoo.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3otedwsor.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3zqdglhxy.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3yufivoja.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3vqymdapz.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3mtthvzst.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3ydnhxnbv.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3kbjcpgem.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3hiibgipz.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3zhgrfpgn.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3cukeitsl.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3mcuzulhk.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3ueminzjt.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3gtgqqeky.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3dwwjykwk.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3fchlzpin.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3pnnbfthr.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3wrfmilka.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3yvkjrsrb.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3snbgfusl.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pcmusrhz.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3skubzfqy.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3ohgcrlmo.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3vxuurrzu.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3hvsexzop.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3exoqgliq.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3cuxiddtw.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3fhpbnkze.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3wumwspzv.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3nzerijud.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vdxkjxib.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3wrbjxiwr.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3ufkqiqhr.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3wkfmsevw.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3uoaxylea.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3vqlvjssz.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3azecgnot.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3yhymtpvq.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3hvehgvif.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3sqpuvuel.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3byzomhmh.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vyphxubi.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3pmnmpdop.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3yepybkia.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3krlmibtz.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3gpjhficl.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3corgteqy.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3cvmomdyz.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3uuxkunny.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3hgjjioam.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3hizknoni.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3cdxedtux.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3wkkzyoeg.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3fydypykg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eovqhcfh.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3bpvzupjo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jvwdpypk.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3sjfwjpmq.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3uveuatpq.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3ehbmtxpq.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ejskrpzq.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3wogsaxxw.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3axcnefbw.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3yjsurqee.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3tlfxsriy.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3jixnjrpv.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3kdramynd.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3fqxlspoj.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3ulbmryub.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3smbqrase.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3yiaqmgub.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3nepabjaw.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3gnmwpxoj.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3bxgynoup.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3nabzgekb.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3kjapmjex.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3pzucrfvj.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3ffjtoxfc.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mebtgyee.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3hhtezuzm.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3ilvuuzoc.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3mpfwygwt.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3nhbgoujg.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3olozhjjs.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3lnocjdol.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3ndldnefi.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3nwnjrbqf.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3znkpzfnd.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3mcoptuko.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3jmbksevu.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3nzwqzqqv.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3idaxqicz.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3gflqzrdo.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3baovunnj.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3pkdqgcpa.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3mxypyrfu.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3ecujupys.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3iegrghwp.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3pqovlkqi.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3echrciuf.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3nhtoqnkl.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3dbhzjtsl.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3errkjjal.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3pfzkjdlb.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3qpflvthb.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3qojdxkau.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3dlsgwcrd.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3tjpfnlbp.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3hwnrhvwi.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3xkuqbvsw.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3rpyhaehk.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3olwxalwz.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3cimpreqq.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3uiylqzwv.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3sgrcroyl.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3issiduwv.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3izunjnxn.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3otcdarno.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3epwtagwf.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3qdbqcykq.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3yqowaytm.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3kbwjkwgm.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3sspnglwt.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3jghafftq.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3taacfhjc.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3talmivji.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3qikqxspv.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3onsipyvk.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3sbgodxse.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3htvbpsqx.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3sjirqhip.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3tjyditdb.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3zudjtbbp.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3jwggtzgi.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3kcslangk.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3cnrsoivm.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3afdzedwg.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3jybdorde.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3ohnhztta.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3asplfzmp.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3zvlhgkem.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3wnlpfqdi.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3qfsxnxnq.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3yaqytyjk.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3baxwsfbt.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3hwzoeasu.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ilfnviya.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3msaojlwt.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3rfrrcmqe.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3rffpkcbx.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3ugplhysg.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3spdpmtts.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3omxxpwpw.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3dlqmemta.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3oxqdzpeb.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3cigunwwu.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3nqsuraum.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3bidnymcv.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3pxgmvwzm.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3wubgoioz.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3poopcxsr.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3iiqcrbaz.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3apvkecnl.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3erwoemuc.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3pbuwusws.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3bmilnjzw.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3frsznwcp.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3cnbnpoya.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ohjfollf.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3hgsmmpaz.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3wpzbvnbk.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3pshkhgug.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3gttrhgtb.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3ghepatdi.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3ewdozgog.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3tcjsvenn.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3fbvnqjci.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3twzfvbgv.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3buajdmdf.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3ylsdmogu.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3qzmdsbtt.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3lfnnwzyj.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3xgbzfydk.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lbcuqiax.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3yuiuarot.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3sncejfoh.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3lbmwnwwl.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3bzkvjxjc.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3htwtwwex.html


<!-- 参考信息 -->