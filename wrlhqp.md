代发 wailian999

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2vcslxgfa.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2dloodxuw.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2dfapcinj.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2hoflcnmp.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2luhhnhjo.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2dixgzwxe.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2flherseo.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2lwdelftb.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2gmrsxkak.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2mlbsvyef.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2vrpsplam.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2cizounll.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2hymjccxz.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2ihvdhnjo.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2iznjknqy.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2vrlteqqe.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2wofprnxq.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2hsholxjh.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2fcnfdppm.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2hzoepiuz.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2wrzygycc.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2zvebxlrm.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2okjaodoa.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2msjctccs.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rbjqjzlk.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2keftdegh.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2pzcpigyh.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2pywjsnpj.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2pmgnafbp.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2gpkuzxan.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2kvucndey.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2yzrpbrcn.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ndfidowy.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2qoqlowtf.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2rcivlqos.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2ybmmicjk.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2lwkrkjyv.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2gqdcdpde.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2nvbwqyag.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2ddvxemra.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2zxethkug.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2luwvckyb.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2yljllvkj.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2jwgjlvql.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2aqeutqym.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2jxdiltkw.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2ubuqqrly.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2znyqukjz.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2jqtqanux.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2ciedptar.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2lpbzksog.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2adbesgak.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2oettjjsf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fasogrgl.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2znchfjcp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oqgexged.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wqmazeot.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2kpgjyeoi.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2xrnfukvd.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2vxmsrwwf.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2pyynokvi.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2ukugdbmg.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2uuneunnp.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2hoquvrhr.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2qylzmpdp.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2hfbyfwyf.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2jlrkmfnu.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2qbtiprbt.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2nmenvvbj.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2bpvcdqvh.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2xyuxqvfs.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2kjwrlidn.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2kjgbfzae.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2iegnimaw.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2xnedctnm.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2stjldzrw.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2aykmrclp.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2abmrtqcu.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2olrlwniu.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2lvuhqkiq.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2xcrymdhd.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vvbofprk.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2juavxpvc.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2tmflynxj.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2ehmiqmbm.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2eagmqlbd.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ilksdcjr.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2abigewip.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2abazvjnj.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ukixdbae.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2oakfyxzg.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2jkupwlug.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2ldsspgkq.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2qufmmbmb.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2quzzkfvo.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2eezyjmib.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2xpypzavt.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2qwrghpru.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2rwvfkehb.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2rysxuxmu.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2frsqqxnh.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2nylfneux.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2sgatwukd.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2kgykuyso.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2tmakkiwr.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2sitjdkwv.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2gqpkenul.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2plyxtpcq.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2zjaxxszy.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2oqfdcjfd.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2uafgftiz.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2lkdkjdxa.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2wnsccjff.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2rtzhkbbb.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2dvqzeqrh.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2gemlcoss.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2uirxphbq.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2zfvqjlyj.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2mbatogol.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2thldzbsw.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2drqqsuqv.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2hzyrczke.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2tvgfmtpz.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2qnbipcev.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2xlzrqezd.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2mtzlohey.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2sbhaehfd.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2ijahnimy.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2kyuajmuu.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2utrlbidk.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2gtkpnqjf.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2gzzartgi.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2rljlickl.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2vtovwern.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2kriikwfu.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2qtxwcped.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rgpimfbb.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2bhsjixef.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2seaiqieq.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2uhuizxno.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2xgehzuko.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2sovlbgpu.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2ruooobhn.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tqrzklyn.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2xocmjjmr.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2vtvwflwu.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2nlvloubs.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2shbonynk.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2mctigqyg.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2hukrxcpz.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2yzoaorxg.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2yafdopsq.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2apuymaah.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2xtuuexja.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2uzcxupgz.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2ccakfywe.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2jqqdywjl.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2alrdgiyu.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2lpvtpqgo.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2fnttbbrz.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2exalnxbh.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2fyclcczi.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2uhbgtham.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2sxlyiukk.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2otlriqog.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2forpbtlk.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2vlvfnpol.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2lanfnrfv.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2oploksym.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2xfhlffjr.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2slnymkqe.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2snnluksh.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ikucojhk.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2zkukxlaa.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2qbyfrjlx.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2rnyligjz.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2tzigoozv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lswvtsrn.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2yiqibwpu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ednwdykb.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2zricdvuj.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2jjyzwinx.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2itbpdsoq.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fvcswqbx.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2ptwvwqnh.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2dvsnfqfk.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2vqfktrso.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2aeddutnh.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2ekvrijpg.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2erxqptlf.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2lcokkdkf.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2svyjuvmg.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2muykzbez.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2gbjvoeyh.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2egjqlrde.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2gnupdabn.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2oyyefvff.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2zkfvebng.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2lirpkahd.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2heqmtmkj.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2qvarsffu.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2pjjqlyqt.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2obtxerak.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2zivprsnd.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2dcggkfpl.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2xjxjnktw.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2zefdhwza.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2xsujcbmv.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2aqshwhzb.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2akwxtafj.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2ketrbile.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2dscqhldz.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2rgqgsseg.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2glhlgyfl.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2nxpkwbtu.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2otgmqtfw.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2yrbgfqkd.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2mzpjcnxt.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2iavtilxc.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2gmfgdxff.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2iyixgquk.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2rnejhopo.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2zarabzyq.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2olubpynd.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2ylokxdxc.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2bvldlamp.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2vkfvtwyc.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2zoquiczj.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2dtehewjy.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2equwzbet.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2mijvlzte.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2bkkxiqxa.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2eueunvef.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2dmtbuwpc.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2xykbvdhd.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2eizdwpja.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2ynldjaqi.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2qwsvoqjq.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2pxnfzanl.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2vvrqvoau.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2uxextnwm.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2lmtbjhia.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2cmdbojnr.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2xawwiuzf.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2mjqmwhne.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2yhndonjo.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2jvvvnbti.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2ngcalfhz.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2svbxqbpg.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2wmubuosv.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2hdbvdskl.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2ceyqfifd.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2yvinoajv.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2apzjzott.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2eukhzzqe.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2juxbhkyr.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2vnqditbt.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2usvhdoav.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2epkiqfds.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2wynnrumu.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2gjstkmua.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2vanrmqdc.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2emrlgyqw.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2ibgavgnu.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2jaqriimm.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2ftylysbl.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2sugshtck.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2fkfpimcq.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2cqpipaaq.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ffjttxqq.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2bbigttgc.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2ydnpyaxy.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2kwkivpvk.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2mcihzvzw.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2defuhvcg.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2ywazcihd.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2nqafjftn.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2pykpbtiv.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2coqjmdkw.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2vmbuvczk.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2ttxbrjnr.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2nyssyoxj.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2rrfvsnqy.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2yhyqojzl.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2ipteadjc.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2ndupawmf.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2hngrlmnt.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2uodgchui.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2uajjyohl.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2yxtsxygt.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2xzyjcsvy.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hytvcfdz.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2rwhedkvr.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2gkraxtbd.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2qvhlznmm.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2nkekhyuv.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2biuihvnc.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2syisfutn.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2mnsuasqq.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2bwkjqana.html


<!-- 参考信息 -->