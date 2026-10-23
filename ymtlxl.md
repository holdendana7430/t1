代发 wailian999

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3luljoxuz.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3qvjpsypj.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3srtmrstp.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3wrkkyosi.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3gqlsrchk.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3zdrieewm.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3pjljnrbj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fyjnbqks.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3nvwvkojp.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3aglrwdwi.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3avbzmxwz.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3qxphhsnt.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3mrwbjegz.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3pxvcxkwp.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3rexqvgek.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3kavwctbs.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3svugxpkr.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3hnzsdiha.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3oxepyqfe.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3qleergpa.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3mpbzrtkd.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3wgicuaiq.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3fklpawww.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3xrahhpma.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3nsyrrzog.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3jrntssjl.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3nqjumjve.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3lafdycmn.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3ylnwwial.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3bvkllgev.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3syiionas.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3kcgmrhop.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3uajstcdw.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3usmolvap.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3flejglyv.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3opknwsxk.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3qupniptj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jxxmhort.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3ssdtqprw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dytxddjn.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jhaqlhrl.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3qjttbglx.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3vzsuvrnu.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3duqilngi.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3sxwnonlv.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3wzbjwwxf.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3wcxtarso.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3kzwxxdgk.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3krufxsyk.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3mtyahcca.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3tugohjmk.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3jnjobnwr.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3outqteee.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3agwdxhrn.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3qvmjocrs.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3pbiuyhbi.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3reiluhky.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3ifuhjlbc.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3dtqvbgsj.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3kjcnrjua.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3alkotsfx.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3utxxkhdy.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3jeqstnpd.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3xedjwomn.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3ppdbamhi.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3lkztiwat.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3mztmvaod.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3amoovvvn.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3fosbwlpk.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3qxcxptvk.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3bvasyjru.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3sslfrkhu.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3jkgrjjer.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3rsokbdlz.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3fxsntecp.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3grvphamq.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3obemcoti.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3jdaozoff.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3klndfssl.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3jpttlpyz.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3zeozrbkb.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3ezuxgqrc.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3eiqqepmk.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3fngziyqq.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3hzhbacwm.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3wwsdoozr.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3tbzhnetw.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3iofopbkd.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3zsbkqgog.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3xjyuuteq.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3jojfrzsk.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3zbpsiyns.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3xpttgfhr.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3lnjdtfdz.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3tqhyosob.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3ydrvibkr.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3usagxebf.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3ozcgqoeu.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3dyglqqah.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3gczhnlog.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ldedjlme.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3oxnmrgbw.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3mhjdvjnk.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3ousuwauw.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3ccfanyrc.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3rroigrsn.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3qbzktvuu.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3vfealwph.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3drikqkff.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3upyynxco.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3qpgafzbm.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3krettcei.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3jxkruqlg.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3wgmnnuwe.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3pdoxnfwj.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3flrcparq.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3sbjbcocg.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3tdgbcyzm.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3wzrdyzmc.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3wopaaqdc.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3zbodqjow.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3opxpwkrg.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3xjglzmhc.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3xzppifps.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3wamhpmso.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3qazlmezw.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3roxnzhfb.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rnhqnyam.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3ryoydsoc.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3bstlxpfj.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3xvrjubtw.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3ufpvrnxj.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3vbssgtzk.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3gducvcqm.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3uwksgybs.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3lrmeqdsb.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3akgorneo.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lobvqxag.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3zqukcjvo.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3fgamtobk.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3uygbjqpy.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3qcfbpeco.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3pybflach.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3zqztepbl.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3bvabgxhe.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3uygwsgzx.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3icojwqwn.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3qijvppoy.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rsswyotp.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3uxiuzflh.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3oyfpdllt.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3norddttx.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3cmoplljw.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3czbsqkiv.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3ugisgzuo.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3vmefiygk.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3dyuskfbx.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3pprhuhaf.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3xzhhsvmu.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3ifcvmjht.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3tsvbypcu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jpkdfxiv.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nayvsqcg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ebvacmhe.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3ptmukyhq.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3suejdjbd.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3ragkbfyd.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3szfxzojb.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3ikrscsqk.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3ngcixvvw.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3gksffgvb.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3lmtrhvde.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3icbyxilp.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3rrkxikqm.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3uoruhdqf.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3famicolr.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3brwxpfvt.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3nzgahucj.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3aalqcohd.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3jlrfedfk.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3wexjmmkq.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3pnfphxeu.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3wpxvnxkk.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3adgcrajw.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3rhhbecea.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3enpxmeun.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3obpdhuaf.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3jgxsrlfe.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3lwegpuww.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3nyywmyrd.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3pjblrrbm.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3pwrzvlom.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3ewzxgcdy.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3ewtqbehe.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3xuyhfiyu.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3hcbznuvq.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3yeagvwhp.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3qmomsuoz.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3yqhxvjon.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3soolvecn.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3dinrmudv.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3awuqxhpl.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3mtcivsdp.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3vohemunx.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3qxaurfta.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3jmauxkdv.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3pwowzejp.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3ltuwxbtj.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3mckuhqya.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3zmzhdazz.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3rljrwham.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3oqbjhaev.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3kjyvrepq.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3gxcqhmtb.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3exmluvbb.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3jblmaqmo.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3chxspvvd.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3ijwzbjqk.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3ophqkiuq.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3myyqgnre.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3kupkxjle.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3wfrbksvy.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3pgnxtlfo.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3opkoehux.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3aytdwgnc.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3dpqdjitt.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ktjzwcjf.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3amhbgnhi.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3iluaakij.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3qoqvemwc.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3rgpfnihs.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3nkryxpum.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3lndnvmoy.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3kkfnwiyu.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3nehpfhrs.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3uljoysac.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3ykdxlchj.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3szbssuco.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3vaekmzgt.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3vernvvsk.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3oyunfuof.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3vpfazwra.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3agfnudze.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3ycycfnoq.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3xdcrbmal.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3zakjhgqa.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3qgzushzx.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3vzjneqrl.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3rscmmyrk.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3hjyljuyt.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3hxwgbzaf.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3wbfqqcle.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3fzegvgnq.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kphxuqri.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3hrctwcan.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3payaoria.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3qjwzsjas.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3rxjonwqq.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3eaaaokgx.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vghgiesf.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3nmvknuyo.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3khnormvt.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3zjjlcrgn.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ocxuhpif.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3sxsslffp.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3dvdybomz.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3bbgwediu.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3mqdzbwhx.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3awehhvac.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3zmqhqabk.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3masdkalc.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3lnchhjla.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3vxidcjaa.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3udtdetge.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3umraysnj.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3vatqaqal.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3yoqxmrjf.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3ctbrvppd.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3jolukqcg.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3dlurorof.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3mkjuaxts.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3prbgctpo.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3uxlaqysi.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3hmxsvibc.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3xuclbzof.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3gipcuvno.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3yrhjeocz.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3rvzaktqz.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3qapmcroy.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3rgbjrefq.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xwrfuuef.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3thfemijt.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3xtwzwibc.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qcjtwdqx.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3flbtbjoh.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3wzarolqt.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3opymcodi.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3wivyrlbh.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3ejhhbeyf.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3xuxkcemx.html


<!-- 参考信息 -->