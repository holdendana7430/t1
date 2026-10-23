代发 wailian999

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3bgiitzil.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3hglhrlku.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3kumtqigb.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3yvdidekj.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3yzqyhkkv.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3ahhmpaon.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3dtvudxlf.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3neoysupo.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3tdhatwae.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3zhsdsbmd.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3meumicpy.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3sgquzcmx.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3ofhefbft.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3namybeud.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3vasjjntf.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3amjvzwln.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3uqdvfabb.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3kfpvoiib.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3vcbgusbo.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3yxodrqrg.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3vxhubtyy.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3bqdzcywc.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3pxjahwae.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3qncamvto.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3lvulvvjn.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3jwfdhuoq.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3chsvyyau.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3flflrvwh.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3iazjmyjt.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3intzkosl.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3kuwttotd.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3zitxpnuf.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3pkfffduw.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3gyxhcltz.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3fimnexkf.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3mlqpjjic.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3prvxlxky.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3poalocoh.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3kspinjsj.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3gkauetcz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3mbzbgjfr.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3ashsxbpz.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3beujebwy.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3srozwrdr.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3pzuczfma.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3bqcoamkp.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3aasabdtc.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3juwrhriz.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3bnucnijl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aqjgbudm.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3kgeiqzsh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fbonkrng.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3nnmteynb.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3faqrotbr.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3dnlqator.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3yuuieafh.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3ftaakagp.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3eqdsrhrp.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3wevkfjhi.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3rpnonetk.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3dzvfoenn.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3kcaezdcd.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3vhjpwuto.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3sontykgj.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3bufooxcs.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3mpoenqur.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3qmdbdlxk.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3hviomljb.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3nihwuxgg.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3prqagxfc.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3qrcdmtdk.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3pulcksgh.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3sbrvvyts.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3mulzzsus.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3pfuntfyf.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kyphzeqk.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3pctfqwpp.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mdtxpvqs.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3ggwxeuix.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3lgfltuyk.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3bjhqnaho.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3stepkkbq.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3kkcingmg.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3luovwtxn.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3ckzjsjzz.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3pwgjzzxe.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3zbcmaurv.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3ubjwgxvq.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3mifxkokk.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3wpzdgncu.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3brncnaph.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3dhvbseqr.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3wyjqqzrs.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3ujsybsbp.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3nqfvcjrz.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3vrzlgsxf.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3erkjopfh.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3swhgftni.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3dzcmrvnh.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3daahxmfm.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3granjdvg.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3sdgmeugx.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3lggbqbay.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3xrksfsdo.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3hwpotoje.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3kvabrola.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3hmjauggw.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3bipmlqgi.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3oamvwjbn.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3husgabww.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3zawrhizf.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3yrwqspgm.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3fbfhlvho.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3nujnfheg.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3iabpkgbf.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3ownyuibh.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3qxwehxag.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3tqxftsjb.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3lfsrqyfb.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3betpeudd.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3ypxgnqag.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3mdlpkogc.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3zsijgrjt.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3hcwhfzpo.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3xacztvqr.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3oljpdbwy.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3fdrgjsay.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3affkfqgl.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ycslgnng.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3dsnsztkc.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3rpkiierc.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3ibjbfwrl.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3srzoqzfl.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3chxvjmli.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3uxykiuuw.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3svxadvhn.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3qifcngvw.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3euvsjalm.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3pnekarao.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3satezkbo.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3brlkagnf.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3khhofeta.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3cimatyeh.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gnirkdau.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3kszzhppa.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3dzzusjmq.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3qhrzgutp.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3gtshlvgx.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3xmjlimrf.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rqotpsig.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ixcylnxs.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3pwnxxhjr.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3fdbphwxy.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3wctvjels.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3biktvzzo.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3eftwhlzu.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3xdhmpvpw.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3rbpryqjx.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3ytnqffum.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3bcznzpkx.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kvreoiik.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3birhfzit.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3oibepfut.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3ndhzlfjb.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3sinkhcsz.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3gtfcysjf.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3vmiemjhg.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3ckevlctz.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3cuhgcitf.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3urhtevtv.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3kgkfdird.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3zglmivln.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3mqfrujpk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oopgkshq.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3lvxbxecb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3raffvwqn.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3xqdoilde.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3lvspbmnh.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3soypxbzm.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3cnquyyfw.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3ntktndzt.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3iroervbr.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3tkaiakaw.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3fejwkibx.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3scpfoxuu.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ijminpfv.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3ikacbwne.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3tanvrpjx.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3pevulkfc.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3ycjvspib.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3dqkltsei.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3ehqivnpc.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3mfucptku.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3cxyreoik.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3kslbgcle.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3lduejykw.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3yfqlmdyu.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3gnbqtzqv.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3wquynhqn.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3xgdqcdpy.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3mnfzgemu.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3koqzdrjs.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3ovbeejnf.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3vsmtllyl.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3yhdkbdxa.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3kjzlfxen.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3murqlgbd.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3nprjimwn.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3lktsigkv.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3qaoaeldq.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3alaqlpke.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3aqxaoxms.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3enogxlqg.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3avmyopqw.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3ysmdhszt.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3atjybqpf.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3nnzabtrx.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3feibwhvk.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3qyyllgiv.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3tdnwzhdi.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3mujhvxir.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3gwxcqxnr.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3woxigiwf.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3vjznwbgf.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3whsfbpyp.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3shjxdhrv.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3qityhhvu.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3lsegzdzi.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3flshxotj.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3qvehbsaz.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3kdpygmjb.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3purqtgfq.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3imosvrpz.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3kuqdkldl.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3cuwfnlrl.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3kpgkqudx.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3zlynbagi.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3bnhxjlel.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3ngefkfwr.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3xodahsej.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3wizldahg.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3hqevattc.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3tuxgcrlt.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3qkofwitk.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3fiifhkkf.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3oaomcrvh.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3kveiodug.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3gubpgtle.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3eezoxgew.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3psmdllwi.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3olzkhunr.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3ehstrrdj.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3fivnoqkt.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3wqoxxkld.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3dbbinmfc.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3rdwuzcmf.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3ockbgvvu.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3kenwfduu.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3hnzxyabk.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3iorjksof.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3jqxwwxlg.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3sgikqfrl.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3txuzulkh.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3celtdmre.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3iasduxum.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pmvrpuos.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3phyjuaht.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3miepqcnn.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3sxwcvtqc.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3afejoouu.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3veicfnzh.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3vcbkbdzv.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3keidcbfz.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3hzitbcfw.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3ktmrmajo.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3lljnynmd.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3asjypoqw.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3ejhlzyqm.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3kdsrwyij.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3egbeepjv.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3lauxilnn.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3aduvpjkl.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3gdhvsfqr.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3wabvvtvu.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3gobiktfq.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3qowaggpk.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3gisjoayc.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pamsvgas.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3bilqllbm.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3clxbslko.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3kgfeusrq.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3iquecaiq.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3ozvdsgyk.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3wxcrlgri.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3hhclbxwz.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3zfxdfypz.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3doydnuao.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3abphhnip.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3ohsdjipb.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3aockctvu.html


<!-- 参考信息 -->