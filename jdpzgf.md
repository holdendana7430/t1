代发 wailian999

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3xhiomkav.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3udmdfvuu.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3opxgopon.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3xlypzmjm.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3qqhzsyif.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3zmtgcimk.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3hneoygdb.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ligtfhxb.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3yagrhznc.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3enbqeptz.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3engdotjv.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3ckjhqgfe.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3danczhoh.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3pthhtgjt.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ekbrowwe.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3exknfwzt.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3egpexokv.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3emvnhbgl.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3rwumyrrq.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3fugzrohd.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3dyqhliyx.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3pklztojr.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3ceeptrqi.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3tyfunzbx.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3ppwaijzd.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3xamicjed.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3yvnhibot.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3bxszheqx.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3uulhunta.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3lqxysuso.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3bnhsyogo.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3waejixsz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3fjvxmbla.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3bykriyvd.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3brteqkku.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3iqdhngor.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3gwafynzd.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3uxcgwisb.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3dyquxtte.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3rdiamsus.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3nxiqzjll.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dybkwguc.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3keacjjkt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ymakzrui.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3nfcjaclz.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3cidazjfy.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3iyapgnjc.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3moxwjhzc.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3wyhorkfg.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3hvdfdwao.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3elejqwnj.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3odcmzwsb.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3twmujbxf.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3kbemrihx.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3nabbmizi.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3bhicjngk.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3panhbwyk.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3ecdlepah.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3boxdjccx.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3wdhzrmar.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3jrqrhuqa.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3ukjnomvv.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3cawmsvza.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3zaosyaak.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3jvrjqhzd.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3awphcprc.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3rgfmsnvl.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ztabcmpo.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3lpiquype.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3znannsti.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3pwnwzgoa.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3mkxjncvy.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3rmcvanjg.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3ccaljxjt.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ivhabrkg.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3pjyeutuq.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3kvskdytg.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3jnnvctbf.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3mhsqpbba.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3izfdgyij.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3vojcxujc.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3yvwhlvhg.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3xucnuigg.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3sjqtyfmw.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3wzhkwqnr.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3ivldgcat.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3dyvwletr.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3zipinjeh.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3cdpdakov.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ucbibljo.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3fhaychlb.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3lpwnslfa.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3rbtvvuos.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3vmsohuru.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3nwscprjv.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3xlkaktuc.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3gfklbwsr.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3iexrijyg.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3czqfsjbg.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3nanpsqnp.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3cbschhkd.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3wkebmvgv.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3eqxvnikz.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3zfegjobd.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vrhoazyq.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3fxngoczi.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3ywqtosrs.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3vfxdsssz.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3kfbmqrxk.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3tzbegncp.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3ddgeereh.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3dbpjejsa.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3kghjsezz.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3lsljpzbi.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3qzwdhctf.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3etcdqnzv.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3igqvcvwh.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3owqavwyj.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3wzpndnuy.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3ntwmvdcn.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3qmtvqthx.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3bnqovnmk.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3afmulnpb.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3vezrlfhr.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3apefxzkz.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3ltvtinxn.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3krhuirpu.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3xfetfzmq.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3fzxehwwc.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3fdafzbpn.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3mjwwqwrk.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wpydjkyc.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3znqkdwhw.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3frdpzblq.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3uzpjlhcb.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jxxelqme.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3ejretxrb.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3zghtumgb.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3dekqnppz.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3ixmclopz.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3ocaxrcqp.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rsgvkney.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3lejkxzlf.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3hcqhtukh.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3zblzntds.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3azhozdcm.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3jzsulrhe.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3qcaikovl.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3jsldelpq.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3xesrrfxe.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3egocifbk.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3aiqhqorc.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3tepougmx.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3bjtdbshq.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wlegeqqz.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3samwnalk.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3bloshuff.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3gpnpxtpm.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3franvrjw.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3baowzwiz.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ofkwjcid.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3tkdzkhcn.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3zgevskmh.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3dfmpuaxs.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3hxeamfrx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yfjrmphe.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rfcfifkv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xcgcycxj.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3mekblkbv.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3sfulrhxl.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3ztjknfwf.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3yrhwtzri.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3niiwdkym.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3roztoukk.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3sewxwqyw.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3xtcnixol.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3lczlszuh.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ctwsaamw.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3xlfyygxl.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3mvwvgfup.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3lhdotamc.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3tallyktc.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3borbkxer.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3dqdmrpsd.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3wcdlntps.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3eisagyib.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3kwtjucuj.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3slcsnuav.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3fkjgedzr.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3mfkinuqm.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3mfzvbbve.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3zqujrtqk.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3qgitvuub.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3iuhyibyl.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3kiasagtq.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3nstuzbgd.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3iykaqxwh.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3zoicwfws.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3japcpqlc.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3logydyef.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3jiftjekk.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3wmnqcukt.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3ylgvdzko.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3fgwvbrnu.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3rmyxrblg.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3iitgpqjh.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3bezrhuvr.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3rmxozngp.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3zxxbcnwt.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3gpviqltg.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3trctzvin.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3ieoyaetl.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3dpvbfytr.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3mcsnpwid.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3ssmomgxg.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3alxdoiah.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3ljwtwesl.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3mvjntauv.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3xjtbixtb.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3aiqcdmpm.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3odpadhyu.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3dsxsyjxb.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3dftzuoqw.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3fknyfnja.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3hqahxszv.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3rfsfsoys.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3eqdphwjc.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3eemkdkiy.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3jcxgsueg.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3pqpnfqza.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3blwcxumw.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3wqfwgdku.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3hopgddee.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3gseinnsl.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3pkhckxvc.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3ahynxtuu.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3qawhqzcr.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3ybrxzhah.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3swalytye.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3plfydqih.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3aiegjpdp.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3vzwefecg.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3oicgrzbd.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3kjqvffkd.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3cbhbvzes.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3veluyugc.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3leeqjlcn.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3bshsypjy.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3otpbxfvy.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3wwlfyjfd.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3qmnbiboi.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3nmxvgwrl.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3kzxlubwa.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3qjvqznhh.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3hsgcbzrf.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3qdclzjbz.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3tipcsdly.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lmpxqzvs.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3rbncscvx.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3hndtjpki.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3ddbesncd.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3koogmxie.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3gmstgujt.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3rlraixic.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3xqhpviqf.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3jhbothrz.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3ezsaogzc.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oiuylgmp.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3ezgqifzk.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3saktyysh.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3qofxvorg.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3culsitbk.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3bdnrisnz.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3kzmrevue.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3oewndncx.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3vzfvipla.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3rpuhiiyf.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3rmqblmyt.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3hqkijrbm.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3iugyusww.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ytlpkddj.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3tusjivrc.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3siwsubvp.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3sncvoxsq.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3urocccat.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3cbhlhlql.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3fzijnhog.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3atalyemr.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3yirsbzhe.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3wpxadbjb.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3gnlndlwb.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3llplalbx.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3ujgbynom.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3wqfarumz.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3vlzsgkta.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3gmefsjfq.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3fpwcrdtt.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3kcngwwjg.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3yqunffde.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3loyjwvba.html


<!-- 参考信息 -->