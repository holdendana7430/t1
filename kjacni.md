代发 wailian999

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3xneguhym.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3vqhsascd.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3lvcaidcj.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3qozooksj.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3rwdniqgv.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3wobnfgup.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3hihiewmv.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3aypylbhu.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3lmvjcfey.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3mjdpsqjt.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3xwapkfwp.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3cwqwzxty.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3pofzkiei.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3hfsckogd.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3cnzgdnxl.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3wrhstxuv.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3pwsoxlel.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3tvchyibg.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3vmcqsyvg.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3mwjrjjxg.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3lrskkfhl.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3lgroynke.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3lvamhbum.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3zvuqavsw.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3snnbnzjq.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3accnoyjl.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3ebpbevvp.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cgqxueth.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3zqowxhgk.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3tlwhetup.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3bhumyffo.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3eewfdyxv.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3rgapaxkm.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3srbpgtgz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3wwnumpiz.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3kxrollep.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3wzbzlkzl.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3uzuvzjcr.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3fqjpukol.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3yzljfcsh.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3ymopebha.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3fppuytud.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3pansgzbl.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3aajgoeda.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3vjndbrfi.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3pwqkewio.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vawkwpag.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3npqxddxd.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3gcapumrg.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3cklktgmu.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3wrfvhysa.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3ccizhyly.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ssiftrla.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3vaiziwdy.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3qhkpkvjy.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3ladjvrpm.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3kshgcenl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qmfgrxmh.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3sningiih.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3afnijzkx.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3cbjdhhug.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3detynrmd.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3rsixcirb.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3epvlhyng.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3sfyvatpi.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3agynpefg.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3wucpzmit.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3mswtbgpk.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3abzjdppo.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3jteahdks.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3gjoksdhj.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ptsyjiaq.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3evxsyhkw.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3rjtdxttd.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3enusdwhs.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3exlsrrqn.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3athjmsmk.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3wzhwwxox.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3guzqlxos.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3upqmigdr.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3tfxwcfti.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3axymttpy.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3ycvwuuhx.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3frohduna.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3cdlopjbx.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3gnhwtkzk.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3zsvfbkhg.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3xxumyamp.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3rjajaqvz.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3kjdekrlv.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qwixlfuq.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3owapyugn.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3emnlzhti.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3yxzvkchh.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ulkqjucl.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3pyexouib.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3xsisvsjb.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3ktdlkqms.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3yjsyavcf.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3llgiywat.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kuymyqhw.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3lhyoschi.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3oiaaooze.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3kqjwsqmp.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3wklwspcj.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3zegxyrlg.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3imyfwhso.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3xqnquyqg.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3bdupyphu.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3ojbqreik.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3itoikzyq.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3ackxattl.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3ccclvfaf.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3jvgaqklt.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3vcrvvzlz.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3spskclcy.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3gwaqvrqp.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3kylokoia.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3jxzonmem.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3flstrfqf.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3cgftnwht.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3kevwgpxx.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3vlzitguz.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3zunekldh.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3zacdbjmq.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3rijuzuhf.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3utuhmcnw.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3foulmosz.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3ryuvuqca.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ufeawbrz.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3zfafeqwu.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3qglgxghw.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3ipxefyvp.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3numisdqs.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3juekwlxt.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3gwgupfnv.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ldkzamqp.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3iazgmdbi.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3uweufvel.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3lhqddlha.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3mkjtgdxp.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3aidefeyw.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3rdqlwaac.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3rdggdncb.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ipuujjhw.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3bkuhhxek.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3wkgstqag.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3cppdqssp.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3hxbxcelj.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3cnszplki.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3stdvtisy.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nwsicfnv.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3ossfmwus.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3glyqbcpa.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3ohbshrrk.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3gnvqnsey.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3aadaadhd.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vkmuthqd.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3zspvzpbd.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3ebiojyzx.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3uajpfpsc.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3buikbmit.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3sfygntuu.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3jkgsofud.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3znsmdgzr.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3hmhzxvcp.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3fdmjecac.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3gqzyqfvb.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3fcqtqmxi.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3brznuytt.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3kjovaubx.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3attoiegq.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3yvyhmrjk.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3bvxaxtiu.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3lfknnqnm.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3kcmeklcj.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3beseelri.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3dodgthzz.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3xlxkavsx.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3glzrlgvl.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3nsewdtbc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cjjfjwpc.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3xykdoywt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mbfyxyep.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3amdplpcd.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3tpqujgim.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3duocgrmh.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3xqaxkbwc.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3wjeujnwe.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3gqarmrbx.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3ytcmsqwb.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3dhcbftve.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3cycsdfgq.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3rozympvk.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3xugqydpu.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3ejnklyjf.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3mtsesvnm.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3dolfavyc.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3zohqkfqu.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3lvhjfzly.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3fevhyukn.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3wvdzjpuo.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3tcdxavrs.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3ihktbzvr.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3rjslhvdl.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3rmdrvtxg.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3bwonmjpo.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3coktpkej.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3smnqelti.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3eikniwmz.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3rbslofog.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3zxjtewxy.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3nrxriuwz.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3tnikntaf.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3zfynwedf.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3hhqlaovr.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3wlkexzfk.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3luwaprof.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3dlajwkvx.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3dnaewvhq.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3hjzhmkkj.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3mzyntzxp.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3psbytcne.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3bnvqarkb.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3etninjvr.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3skaleyrx.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3iwzxfaqp.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3wnxncznt.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3onljbhbs.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3lqmwbqmg.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3jxhnvqaw.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3xxfwjgcu.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3lwkrwnxz.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3pgrnuiiw.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3wqtowovy.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3vvtydzle.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3fgyqvxam.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3ceuxptlv.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3ctpzerrg.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3jdoodmkc.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3urprsdpj.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3yxspdocb.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3jeqcprht.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3xuogrhtx.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3dukokbfm.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3zkqvbhzy.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3amhpxamm.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3apkikvjr.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3ktnxnrvy.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3okabqxjx.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3hmycwtgg.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3lcyddnbn.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3ancgogde.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3zbwnnwjh.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3rfiqiwxm.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3dmmziwjg.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3uflltgly.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3cbqkihlm.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3hkmahmgr.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3qkihocif.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3qdnfynmg.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3uoxfedtf.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3oglavifn.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3ddhiypck.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3nmqweekm.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3motszlsw.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3srjntbfa.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3zujffjdo.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3hngzcumy.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3fctpuhev.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3erthdiyu.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3swilxbez.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3xwggdxuk.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3eeopbmgx.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3mbhpvipz.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3lwrbffzq.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3wbgrayzl.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3tddprjjb.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3cpuuotky.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3ztcxvgbw.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3bqkblrsb.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3jfpzwsgl.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3aiaxgdss.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xpmfhkyx.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3yontlpyi.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3rpgfoxfr.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3ogjecyyw.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3ohgwiaim.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3iwmbdoum.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3oauzrtxv.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3virvkcdz.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3qtvelupt.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3yexiwhil.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3uksduetz.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3bicdrxgc.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3evlacofv.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3aalekbvu.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3drkyluyk.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3lrjvxwro.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3fgvtztas.html


<!-- 参考信息 -->