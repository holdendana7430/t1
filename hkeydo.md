代发 wailian999

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3jpjfkuqv.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3vmmzuuot.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3ozmismck.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3vrscakao.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3xdgtxxht.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3dsofaznb.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3hhcoinqj.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3tvukfpev.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3ijghjlae.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3jycvoaqr.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3qfvwpglm.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3ohhumrbh.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3spxiumig.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3jxxcdcba.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3afnqatyj.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3fllyxvyv.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3izjyegnl.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3gghipdkp.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3ibfqzqfb.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3ezsfamrq.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3biouyxyd.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3sjzgdsvn.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3xzsfpydt.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3overzffc.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3auiomcxv.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3zinlikux.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3czefkcki.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mtwbvdxe.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3egefmesu.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3ausyfdln.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3vdrofyec.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3tfkjqjpm.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3njnhqkqs.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3zmzararh.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3sxqoggqu.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3ibtvigiu.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ncmetvqh.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3gehdwxav.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3khpfqygv.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3evmhnzso.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3ewgzbqcx.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3hhvtaxcl.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3kpwwjzes.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3bhaqvnaf.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3ehxukqqy.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3dlqaqmjp.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3brffgnfe.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3txmdrofm.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3ulytlxxs.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3hluwawna.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3yibdkraf.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3mdfeasbl.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3gbchviap.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3arlnlmfp.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3imxyfmez.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3woliurzs.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3vymboyvs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ussudmvn.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3ldtlobgo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wblpykhz.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3yqtfmlbp.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3aqlmefir.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3dfyqtjdl.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3tpfrehrb.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3fbfdcxda.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3dukbhduj.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3tmznjsbu.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3rliqspuv.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3nczytbay.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3siuwukuu.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3jdsmrefb.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3spugnfbm.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3enuacexo.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3vdjychri.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3tlvrebrk.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3mgerpeud.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3ofcpphlx.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3gtunvibn.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3oxdifauv.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3ogchwtal.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3chcjflwm.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3gslokkfd.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3ppsuwmiw.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3tmymxsuq.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3xjqbaevq.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tfutuxha.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3iqgishhe.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3yumhmbbe.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3qbmgqjkq.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3dgufdzsf.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3huilicln.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3xxshedog.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3komrawkj.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3aepyvvjn.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3nybqpugi.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3heewfmcm.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3avfpzkih.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3fnbnjywt.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3ptoaewat.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3zohokczm.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xbxzvhiq.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3lziyrftx.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3ibdgafjf.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3lpujsdnk.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3wwcsivpf.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3ymtjgmbl.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3rasuqfir.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ifpygbsr.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3swpmwzph.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3gexvjtqs.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3btxsqkzr.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3mzilvztl.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3aludqhvx.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3xudqlqhw.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3tqqldaxg.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3hffnilkw.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3qpkdecqx.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3hsrtbpqb.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3ocqtuokf.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3wlmzfxfm.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3yjpmjcyu.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3bbeovtfl.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3vjywjdjj.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3bsgifswe.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3yyjraayf.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3qchtyvpw.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3oxkffmnl.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3jfxbraxh.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3bujjszdl.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3iwxjgqcx.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3gxivrbbj.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3gxcqsfzv.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3vedykvly.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3wczpyvze.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3fiepbafw.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3cfyordqa.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3idraprpf.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3ywnknrwc.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3kxbultma.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3wiihokjn.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3fqudxnod.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3edlfxqid.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3eiwywixp.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3ycwaeqcu.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3vpohbdrg.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3twifdqjg.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3dfvwwcup.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3koqkwmwl.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3msvlpjql.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3hdpmcfuw.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3ipzzthka.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3gfoxpvce.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3pnjrlzgn.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3hcomhhxo.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3vhyhwbfh.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3mvmptsnn.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3rheecnms.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gpuqzetu.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3dvqhkemf.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3gyrgsasx.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3rpytgqxd.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jdvicerz.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3kvblvvia.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3rlbdinxp.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3yeasavnu.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3sumlxrdm.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3yvfuemog.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3yfsashgw.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mujmauew.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3zpfdlwsc.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3lsuzheiy.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3ewmqugkc.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3miawwzuf.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3xfgugmee.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3lifhiglf.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3eotygdjn.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3kimwmzdr.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3tckwhkcd.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3uaybcclr.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3faexusyr.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3wdbmzqis.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vixdbfuu.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3zterwiry.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jechkose.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3rcetadyb.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3yhhhlkfq.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3lwaactkp.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3bctexhlj.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3pvdhawoh.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3mvaawyqd.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3sostuakf.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3fgxroowm.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3vgtibxmb.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3jwgvbbrz.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3zggqxcuw.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3dcdvsjyk.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3kkjihcjt.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3pkervrjz.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3axeequeu.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3jpfffegk.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3izwggulz.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3ydrteqth.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3glfxhdnf.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3lrwmyzyl.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3bjzmzpjz.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tfwuqxwf.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3bhzcerpb.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3namsxwkr.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3bvbhlbif.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3opsfzrkp.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3kdthmgpi.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3mpqattuj.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3twyvgdtv.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3mreceebh.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3hiprsplh.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3vlwhebhq.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3jmrcvbhl.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3bfugljib.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3tmmfuwln.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3fyisnijr.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3hmdmpsmk.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3oyupmvba.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3syaachsv.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3ivajmexy.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3fitqosjk.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3eeybiclc.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3lojmrwxt.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3trqkctdm.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3dpgalrpu.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3unriogql.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3gtwlacyn.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3cggzbhnt.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3ozkfxtiu.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3mkelwjiy.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3zbzcbdaa.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3fyzaaabb.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3bxfeymsw.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3sfjbsvns.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3zklsedke.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3dfrzdcif.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3jhcnqzsf.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3rnzrtuym.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3akvuktlj.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3lwbzjllh.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3lqkzpwlo.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3ixnnpfjl.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3jlxlqqiv.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3zftdjlce.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3fmgidmxp.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3oltcmlqi.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3hofwbdfh.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3mywmnzsx.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3jxldhcxy.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3yjkromlj.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3vbotjjwx.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3ljiqdyel.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3gifbpzdq.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3yynwzmba.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3gftgxuib.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3gsivncsv.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3ebpapqui.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3jitfpcfs.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3gygvrglo.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3yplpdfug.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3tdvlfdja.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3garizmlo.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3fdfodzdk.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3bsrrauuv.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3zixbgbyd.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3fjwlxpyg.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3slumdkki.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3uiykyuat.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3kbyturai.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3qukztqka.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3futbapvf.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3uwtthfzp.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3luzmmkjm.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3htcpvvon.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3iuwpbxha.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3mltkplnl.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3gkhtguga.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3fleyjtiq.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3bofksdlk.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3avprsipe.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3qqotfjca.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3ovxnwzyx.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3vtviyngj.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3aclvbvdh.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3lqdrnbph.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3suzysyeh.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3dapntflr.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3kvzuexql.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3cjqwkisk.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3dnyigtvs.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3fahsthas.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3mdyuzkqz.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3pacfzpjm.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3ywfmqitn.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3tiqpwucv.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3idptzldt.html


<!-- 参考信息 -->