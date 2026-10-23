代发 wailian999

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3fqzhskvu.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3tmpuyial.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3pqkckpya.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3xiiudvio.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3fszykyvh.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3bxzjupga.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3byxonufz.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3zbypjpma.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3pbsacwvs.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3mkpstuxp.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3rjatwuip.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3tqzrycox.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qpxnbfvo.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3xwxfnyzk.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3qflouria.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3dcxifapx.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3emujiufs.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3vvrjmuof.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3awbrazuu.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3jnfwdumy.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3tugegrsk.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3rilhzelm.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3ulhyusxe.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3iddohhow.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3ftkkdsye.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3fkoxdtll.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3rtejgdte.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3rvxqryls.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3fjwnpmuo.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3mroqbvuz.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ilmftpll.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3fmbbauxn.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3gqganqvy.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3ivjrrffa.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3xbghhqjz.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3dprwftql.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3eojwabzo.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3uiiqdiqn.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3svoddtbo.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3zlfhpddl.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3bzivfwyk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3btknigzv.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3pelvhcvx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3myonbavm.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3bpauzynl.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3snjuzkdx.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3bmyfcagb.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3dztgzxrq.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3ydgsganf.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3vpafokpg.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3tlnhnary.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3bghmacda.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3tdrvvhgb.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3yvqvttpy.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3aenmanbp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ipxykewc.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3xbcjeove.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3pvdykala.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3ythwcsuy.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3lyicaveb.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3luqzbkzo.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3jsmxcepz.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3wytxyzde.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3wcexmcmh.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3dkhkjnpm.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3rjikegzz.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3odycstsi.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tkpedtxy.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3uefutick.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3cevhxwjv.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3eqymkhoy.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3xxeloihp.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3tquujpvh.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3abhovidm.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3czodzukd.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3gyiacjza.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3oryxmccq.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3mxzuiicg.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3fbvgmokm.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3vucnvvlm.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3knrnpmds.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3livpwghz.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3ixwccask.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3vlexecqr.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3tyawntrn.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3agqibebf.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3pjeqcoge.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3thhzpemb.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3tpcnnejy.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3ifatgbde.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3qdpmylga.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3khcxsfof.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3vmbbhdfl.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3eguzvmhx.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3dakulnwi.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3klnxmrlj.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3drangrbd.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3bownlele.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ceplvbor.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3jrpgvhty.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3edbhyzbn.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3ouktthex.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3ppzaiisf.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3slwaydms.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3pvwlzhwz.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3tapuqote.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3hvuyvqvc.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3ybltbwuw.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3hpuulnhu.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3vzkbzxen.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3bnbgztpw.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3xlxbrgwk.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3grlatkbp.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3daabjazc.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3hlilqfkz.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3rxwdwtyb.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3kbzrivql.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3jftxtoum.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3elsjhkpc.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3brzrqhuq.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3tyjdotkh.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3jntuding.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3zmziwoxi.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3mqhbhwmo.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3oqazoikn.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3nnhcgkig.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3mtjphjvv.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3shcuwiws.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3sgquptoy.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3nrfvzvqj.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3bkxmkgdo.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3uookiiwl.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lubxthag.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3adfedacl.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3asxymcys.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yhmkxylk.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3rszoaejg.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ltswegbz.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3dflrbvat.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3vpgddrmo.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3iutocrss.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ojjzfqvw.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3zsuwgjzr.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3ijbazbwq.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3rusbijwn.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3txdidvob.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3amfkjkzm.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3kxkswjft.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3lflwzxzb.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3yyfmhjrm.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3nmnxtiuz.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3ifeywwdx.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3shohffao.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3rrapswxj.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3javgvvnp.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3mvjcrzbd.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3vlpopvmc.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3cjsrcvre.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3einkhjuv.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3kveqfpeg.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3mbuqivad.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3dinehvdf.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3kjyxsxlb.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3jitsvefn.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3pxeetrur.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3huoioziq.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gytdvmcj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uvvfkwlb.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3cfsixedp.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3qiahozne.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3xxugoqvm.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3iafmpqqy.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3uusqhlic.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3wfdiywvk.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3rkryzwig.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3abyaewcc.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3jprbfrbo.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3pwyzxmug.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3lzanizlf.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3cmalmzbg.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3jndqpusm.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3vhqeueyg.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3ffraogdw.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3vyldopyc.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3nicwwsme.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3llaqcobh.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3auqtjwnk.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3ewamdfzc.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3jigamlhi.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lndhenoq.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3axjuxnue.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3foauooky.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3wbismgxi.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3gtayshxy.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3ljmrxofv.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3locttntn.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3zsxetzme.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3dvpgkqtw.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3rxbrovuu.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3aetbiafc.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3ojafebsh.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3hnvjugqd.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3srdpthno.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3sgvlvatf.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3otelrmkn.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3mvdcrvax.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3guasxrho.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3frbdlzfw.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3jtsjknht.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3lkmgyprp.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3aipdbrdt.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3ofgqngec.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3odsnjrgn.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3qyzycyjl.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3kvnneqmz.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3dpefveoj.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3qyfatrzx.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3bwvtohis.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3zgsvmctn.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3dipgxjdl.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3jmuvawti.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3mhboxodd.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3lujpfbsy.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3cfjhedvr.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3jqzwwakq.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3maxuomsp.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3tyyhsvne.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ykfmcccu.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3eyfrgfzk.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3iahpclep.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3mytpbobw.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3tqyjggyb.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3hvqaebih.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3hitdtcsu.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3dmmeaufq.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3uvoavkkl.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3uxabprtx.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3tffdbhbf.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3sbuioyyg.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3qfzghqwm.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3cwavvarh.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3malbtsoe.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3idkvtbsm.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3icffbvtn.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3lcvncqsq.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3ogiqefkf.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3aylbfkkf.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3merkmpjr.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3ajsqvwgw.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3vrrncctq.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3owgcauui.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3dspacpml.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3zrxpvwoi.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3zrxoaqao.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3zvrmfidn.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3utekxsvk.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3jcosnuwc.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ixdcfbus.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3fccmtjus.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3pkaxitwm.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3gtgnkzlc.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3vnfdbxzy.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3ohtbsmrd.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3oykqdlii.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3yyohawuc.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3blempjwq.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3dusfstxj.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jpbrsdtv.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3qdkuftao.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3squmajqe.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3yjhcwdsq.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3uhfldeme.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3wnromirb.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3yyfyhlnb.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3fjavijrp.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3fumjbeec.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3spakgaab.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3qioubhda.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3mbdzurdx.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3klwmnmwt.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3czaeylxk.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3jmacjmxr.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3lfdsaitr.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3yhhvzowj.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3hjqwjfcc.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3qovcngqa.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3yqrwiztk.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3gvcpowkj.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3jtphtxxl.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3hpmqghpg.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3qqstijis.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3nccbqeqf.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3ciyavrkn.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3dylwrmmf.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3gwmfaucf.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3wdhaaghi.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3ruyjwpvg.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3sglycrco.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3kxvjdprb.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3cuwnbmto.html


<!-- 参考信息 -->