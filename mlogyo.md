代发 wailian999

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2lhopftwy.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2zteupmoj.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2uzzxxhdg.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qulhqihw.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2dwudjqlt.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2brceeogu.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2jcggqjnf.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2esxbextk.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2llisiyqi.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2kpblibpf.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2efafacdw.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2takqxbsp.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2tomwbovs.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2isaeywkc.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2hcapjoev.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2lirkbnru.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2spgcqjrr.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2pcygrxtl.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2sllzjala.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2hpzooccb.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2zdbffnbu.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2lvzzgpqd.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2nhytbrev.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2ixjwighq.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2cpfgvdob.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2qmxskqwi.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2gstphtfi.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2yzjpfixy.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2zktfzelq.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2ikhlbjtu.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2ombnirsh.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2zgqedqtk.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2fpyxxpqx.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2naqtoini.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2lcpvspao.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2cqyojgde.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2cvnqxksh.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2iqsaurrj.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2pixgmmrg.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2mnosgozi.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2hwzhcyxv.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2ayorfvyh.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2uvdobzkn.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2abttngjt.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2vwrekwep.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rrppimvq.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2iaizpntz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cxqodvig.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2cwrciawy.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2loimfbjs.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2ykngjyod.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2byuukpnh.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2vxrzkwbh.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2wezrhggi.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2awbbmvwg.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2rhfuavob.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2mtbgdetj.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2iphlqros.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2vrnehijb.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2jnskzetd.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2hnhiclyg.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2biwnepre.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2ltgmfdtg.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2yqbrsmim.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2kzxiohcc.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2azomfyma.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2piviftzk.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2htaxrsyx.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2whrtuohw.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2fvibqkpz.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2owmnurrw.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2bmocdnks.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2fsfzkczm.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2obefcaag.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2fjqfaaal.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2vdemgqks.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2qcwsopse.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2xzmfkwyl.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2szjigfbd.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2rglbtppd.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2pprltoob.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2iessckyc.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2zxnsbjry.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2zopmfthe.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2juzqezje.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2kgxexjha.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2npxtxvvw.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2okriwcqs.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2ujbkeqpr.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2evjkkcsu.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2almdnqri.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2stlsmeux.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2anhhneyt.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2uwfxsnba.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2zwxhdpmy.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2pblomcrz.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2wmaimydo.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2hddyuwkx.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2nuyukmkf.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2mmogyrtn.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2ntiylmzl.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2rvfzjzce.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2ildtfbqp.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2dagdonuk.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2srlieizj.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2ddeepnuu.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2zpzgfkat.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2kdcghqov.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2lfkwniyq.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2vfrtmscm.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2tkgogcnz.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2uqocodzu.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2ubvhhiyn.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2cphtauwh.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2vwcogbqv.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2rwwrihuv.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2hqwpgsje.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2ioerlczc.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2knaivxgm.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2ghwdnlmn.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2rsyhpldl.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2fjvcgqjq.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2avcfvdcs.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2spnjbblb.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2wzuntppd.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2iadywwkk.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2edubkttn.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2eywmtmme.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2yyjiteds.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2ehvxhzrb.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2replmzis.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2cjfyiirz.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2nozieozx.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2bmqeybga.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2xlnmxglf.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2yowatdrz.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2egwknpjf.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2dehoitfe.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2wjqgmpsj.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nsgdiykp.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2razecmsa.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2uyyzcjlm.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2yzprslay.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2yenqkufu.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2cwptwots.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pzszjuui.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2jnwmvqci.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2wnekldiz.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2hdkegdpg.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wzarxmnx.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2juusmgnt.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2fqoojmqf.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2qvhirovh.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2upvlavpo.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2mouxgekc.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2bjdpiywq.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2szgazitm.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2vdvubbdu.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2yqekmllb.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2viribbhm.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2ducwfcdw.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2epeqoknn.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2epetgffe.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2lnoyqnnq.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2bzgevujo.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2bjpnotvk.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2nmwxfkvp.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2phbubzzs.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2qieavbtk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xeukkepj.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2zsifojvz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uahfgapr.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2oqyjhain.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2euhxxxke.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2ywtlwlex.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2gypfwxhp.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2yqpskkyv.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2nwjwonaj.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2vytvvkna.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2wvblcaro.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2fskgvptw.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2mkgfiffc.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2ptxmxtnk.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2okjffnfq.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2qtqbbsqr.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2xhfmjbvu.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2kkidheik.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2fjxckhcy.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2pydihgio.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2aaqvbpru.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2xfzdkhom.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2aiidufeg.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2ozjdhnnz.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2hoaaurtd.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2jiidxxqc.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2dnwnlybe.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2mupnzxzm.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2tcmkfpgr.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2ohecmgae.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2gungfhdw.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2wfyiioge.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2znbtngts.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2goudhoch.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2tiaagxdw.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2bnrlkhvy.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2krzrsxfh.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2tckrwpfr.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2heeaeqmh.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2jgwshwos.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2djwrxlib.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2pqimmuns.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2nbabdqjt.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2afcjzksv.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2tzkqoffk.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2wqmjbkdb.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2tjzoydpw.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2ooichfuh.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2vesafbvl.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2gyfwpjbb.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2idimduoj.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2mpayljyz.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2kdmnnaje.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2zgknxpam.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2wpwmgmnk.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2nbgztglh.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2sbqympfx.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2thoifzye.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2pjyhotii.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2cliimnpl.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2uaobszfe.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2nvojpcvl.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2qhiihagy.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2blbsbgxw.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2sylurgju.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2vnxbsyft.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2wqnpzmcc.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2nqkainhm.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2aempzffv.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2wdkkmqjx.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2pealjjio.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2djxdopcb.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2pvczvcna.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2hqfqcvtp.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2bxwhoutb.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2hcgacmzn.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2orgglmwo.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2ttwwmrgp.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2drkhvffv.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2dwlpnogj.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2lqeukccc.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2gemddewx.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2loaqmkwj.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2pyozwsky.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2dzgynpdk.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2pdbrsdqc.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2xbykzlpc.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2xtpsrgqk.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2tcoromed.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2ozaezxkg.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2ncqvojpd.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2urcaccba.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2eojovgqj.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2twbtbcme.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2toyhwmro.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2lhrgstur.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2isflakvd.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2pooysgmv.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2iyganycv.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2awtysbyo.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2yqwgovyg.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2ebppwurt.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2rtwprgvu.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2fqfkwcip.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2ufgumhls.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2hqnyglyw.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2hzmbxlhy.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2nekacupi.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2fkmajwro.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2iltyllxh.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2algkpeyi.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2dihhtmwh.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2eijnkyqk.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2buhchkad.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ppxmlkzp.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2sfqnvzxr.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2ffqokjoj.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2sqphuhln.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2etujvxvf.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2gpnascej.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2ztyxhxrx.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2tmxryhlv.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2hvbdxsje.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2gefjijra.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2hdbfuzjc.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2pbcafxwu.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2sdfalvzm.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2fcipjamd.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2qxrokbbc.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zdgurepi.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2osshuati.html


<!-- 参考信息 -->