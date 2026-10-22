代发 wailian999

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2optlaznr.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2kcoknfbp.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2kkcxfjbz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2viptnmjk.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2tmtpolla.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2pxmbcwxv.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2cuxkohis.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2dfgfvdbh.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2dhpnrrew.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2yjuhayci.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2bgbiybil.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2xhadcjcj.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2iyfrgqka.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2etojebae.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2bnuvahgz.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2tonvgmbx.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2kimanouf.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2aynkxefb.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2lsrgxoxu.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2zxcclhbg.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2niezrqow.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2jnmlzgcy.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2zsdtcuzh.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2eikiztvb.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2dldekuco.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2vejhpija.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2mxfxsvdl.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2mmggipdg.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2upauckvd.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2fwphaepp.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2hufzzxsk.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2mfntlmgb.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2byrubpxh.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2syvjiqui.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2vcrektjb.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2nviiftix.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2zyvkpjqk.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2trasrvel.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2cbmzbsyo.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2tdhiruib.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ejvbokkq.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2tsqydraz.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2lbvfedqs.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2mocevrtd.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2qwkvuewp.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2xawruilp.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2wtwlpplb.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2ezjcqglv.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ciwuevki.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2xrerwehc.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2vzgwgmsy.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2eegomqaf.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2llvgiauz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2olnicpca.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2kiksipzu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vutdscpf.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ypmjrtbb.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2bvsynsub.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2txvzwvkg.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2udvsepzq.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2csyuaeat.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2dovvaile.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2unymrlvc.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2japkhpgs.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2bzsbbnsd.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2mmsgepoe.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2pundufxm.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2spabavrf.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ypmunoqn.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2bzjbelqz.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2yfccsfqd.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2aqfndaqz.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2zzwdimxf.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2tczisywt.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2ekqjfimv.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2einbsazz.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2ytjosrnq.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2gcctyrue.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2yunlrold.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pntmxdei.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2jpuwjiew.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2uiitnxlh.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2lobrkpci.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2fbotxhrw.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2ppxqadqh.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2lecqaemd.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2cqiibjcp.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2bscwdkmd.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2unusnelr.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2lpwwyxsk.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2gnqelkbg.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2erkmcler.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2xogqfudu.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2svzobrlu.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2qzpgtqts.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2kswpjszb.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2hinxmwxd.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2zvkwjowa.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2dbrxxzlr.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2qtsigabk.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2tdldnemg.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2ibilzqle.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2cpuwjpus.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2swtlucrn.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2ceywivsa.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2wdfjcaat.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2zliezevf.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2xxlwnrcv.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2ibkcvxxu.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2krvmyzow.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2yoetmxyp.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2wxjipyxo.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2ibtctktb.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2ilocrtkk.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2gorjupgp.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2onhxrbgl.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ochezqlc.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ocnscxpc.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2tmfuvlez.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2yqgblxpq.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2lfnisghc.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2hlqtithq.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2wbcprjjj.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2hksmyont.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2hrypiygp.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2xcdmxrfv.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2qflwijmr.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2rfxekbep.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2pmjcdzjl.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2sgvwxjpc.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2zweckgbo.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2tqqqjumf.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2wnuphhtg.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2lxfouzeo.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2yvkvagwj.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2cyzvojza.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rwgevbnn.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2txuseadu.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2mxrrppqq.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2abautrhv.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2vdbeslmr.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2kuiuavms.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2oimhmnet.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uzofbjqj.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2owjdsrlw.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2tbdkpyuh.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2scmhtfvf.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2ijchosvl.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2pmvvrrnc.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ouaojkbb.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2zjuczyhe.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2rctyobfm.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2esdbykdi.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jfjqakiw.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2uuznkvzk.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2yknlvrvs.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2evdxdzyp.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2gtigdndr.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2qenjzlof.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2tkwiukrj.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2ypbjuphb.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2iikepshu.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2ruamwoyf.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2ybfhopcb.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ofjelulg.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2mmvhlmxd.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zxcuaejl.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2thsdbget.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2mnbukgpy.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2yfpwsfqp.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2dgsogbbg.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2swufflur.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2emivwcwh.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2shstwees.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2djfpszzu.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2qoyrcjvx.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2vgxhatvv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jwykwyyt.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2jfrccbyr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qbddvafd.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2cgblerxi.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2zunfqpfe.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2gkeojgzg.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gjocjyzc.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2aeumkqyu.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2irljurww.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2oldqvnov.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2zxyfwpfc.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2igkqgido.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2nsmbdfuh.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2gqhlylnw.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2sfmjvilo.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2hbgewrfw.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2hksapgsp.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2ruwfcpcy.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2mxlriygr.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2svypoyge.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2ldzjpfpe.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2wmukueks.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2nzzloexo.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2pvqojrlh.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2bprtdkwx.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2fmdvbbkk.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2cqclhmix.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2afpwjjyf.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2kqywoimo.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2yrhatzey.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2hofxyhky.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2bcggsnbh.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2fizeebau.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2ytjyjgxr.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2sepvlitt.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2gckxhvzv.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2emphummy.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2apisybby.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2vktznrym.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2fvauxusu.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2dnabazye.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2jgueggvt.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2thltseaq.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2ifquskuy.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2bwiuqfit.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2qmqoruxe.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2dtklhqme.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2nknrhuaj.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2rdgseocq.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2ddivzgmn.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2gfalmhcc.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2howyzuvq.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2ojoktqdp.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2eggixpmk.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2wuxgcwjc.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2arjozqpo.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2uqrtkila.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2peqicnoj.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2qwxjysdb.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2hogtfaec.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2opmnjfvr.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2gdmasnki.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2mpblmcoy.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2usvsivml.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2ubimutgu.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2mziavmpy.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2votofzda.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2gkhqvphz.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2ugjhiqpy.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2wzcdxgmx.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2mhcojbfj.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2pcljviej.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2kgdgicim.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2sayxvqdf.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2acaovaut.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2inergtlm.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2vggwdsjm.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2npssugcn.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2vheotfgb.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2jqhmclix.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2dwenxvtk.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2xyytaguu.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2nanaiabv.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2urgnvbbm.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2zgzslbrl.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2difcksjl.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2yfhiybpx.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2rgukhcst.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2hqhpycyv.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2xrreliwx.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2mjvvjnbx.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2kswmricy.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2mwaxoadt.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2whymxxld.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2pvqdcsec.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2eijumrhp.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2ypxclpvi.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2jwtntdvh.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2dslwzgzx.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2rjsmeonb.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2tegyykrg.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2dgfuyuwr.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dmixepex.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2udaxmlup.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2tfnnamok.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2ebkxbgkf.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2jytcztth.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2rjrkinrm.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2lbhdmiyr.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2kdzondzp.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2koqxlfkf.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2sdfroqnx.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2nfhtmkoc.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2pgyufuxc.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2dqqpppsm.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2nhtwtmhi.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2aimqhiuv.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2oixeauyo.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2woxbrgnx.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2vtkcodzj.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2xqxyhrap.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2pvvqnsfm.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2jnydgkjc.html


<!-- 参考信息 -->