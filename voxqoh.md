代发 wailian999

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3lqhdwrxi.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3zxunbgba.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3ihcafgda.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3tjuvgyvw.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3mwqdnrdd.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3wluvgvxa.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3jwxhokjr.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3alwxcjij.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3kxebhoun.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3akvaeaha.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ctplsimw.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3uefrrffe.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ywxnaufd.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3bfnmzzly.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3premwclp.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3oexidoag.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3jajsswqd.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3vglaxubm.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3ezswvlat.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3baskzqkt.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3snewywwi.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3xymupata.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3seuuyxhx.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3jqqusdcb.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3mxlmgvei.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3ochqrxqb.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3udjugfcz.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3atkuonzk.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3muftpufp.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3dfpwbilx.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3xmekdtvx.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3tglhbpzv.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3mhxruyox.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3idggmnis.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3covmqwbg.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3mjkjztoe.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3lfrvrfur.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uarbabbb.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3xogxszjo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3obtiussv.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tndyxknb.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3bgatanba.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3wrojtbel.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3tdqsfjby.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3hpqihfsn.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3srqbpvkg.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3kmiqkyxx.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3jlgkkmim.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3wevsztkz.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3fdmeqtig.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3ckhfwkyi.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3fjjjzpqf.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3rsbmenwe.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3wwhuvzkm.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3adgyxzpl.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3uyutqtbw.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3pbbaoroj.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3xltaskmq.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3hapmoffa.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3bjlfrwdf.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3faxrzjzh.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3jgkukygl.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3eqdapfmv.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gfuikyqv.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3gzhfutcx.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3okdexpia.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3fzrundrg.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3sdvhacbr.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3mpwnhxer.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3ctuvxjrg.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3qgzpwfst.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3jvwdyten.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3hfixpwmm.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3dbggebdw.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ixtirwia.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3yclniggj.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3gspjpous.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3uxriganc.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3jscqejsy.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3ijuhpwwa.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3rjqbltye.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3vjjotijg.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3xrvsucxe.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3lylhudlo.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3yuzxiyce.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3fousyylx.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3zutpymtv.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3jaewvwzj.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3rrfzhrmp.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3vmevssio.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3myqeupka.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3roymgkfq.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3yvppoclo.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3orxdsjhk.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3fcersnot.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3ndxzrrcz.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3ghxvzsqy.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3frladbmq.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3txycimli.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3haakvhbf.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ukcnblph.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3dzufqdtu.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3riaffcnr.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3vpsbnhfj.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3grttgeyn.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3gmagqtff.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3znkcemio.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3flupiilj.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3edjzezup.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3rxafchna.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3ufdtbmow.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3tzvhjfuw.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3hkdokmgf.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3jevhytje.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3phxztqxo.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3qimwhcsc.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3lkbokykm.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3jadhsrlo.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3ckdkuioq.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3cyqilzyc.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3lxkreruy.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3eryhfvvu.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3svgripfw.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3gdiuolfv.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ztnnvzqa.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3zfwkdaqb.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3eltbqsaw.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3firoqpwq.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3tnviszye.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3tkhypeho.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3kgaxcdue.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mjdggkns.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3uyocnufi.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3qsnpkkup.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3lwrewcft.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3tepuobme.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3zeyqbhny.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3coptalza.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3wsggvhph.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3gecrlryx.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3etnjlhtd.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qymipbmz.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3vbebhobf.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3bmugxpaf.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3irmnkejn.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3uziefivx.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3jxikhitc.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3iwmsmiuj.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3suylvovv.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3lqyfkkql.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wyewgmiz.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3wndsvcgy.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3pbxlkobm.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3mnqmmnue.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3hwzcwjzo.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3wxglegvk.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3guozlqge.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3vfmpdfwg.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3mumcehqj.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3nifsoeyn.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3umodxgzx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ewkbabtb.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jihsmhum.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kobjtcvf.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3yypasarz.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3fmqslcbh.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3vyglntzb.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gfwpailn.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3osogeyhd.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3keirhfmg.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3krkvslof.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3hrcydscs.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3ngnttwut.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3stswnhlq.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3mloqcpgp.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3ljaebqni.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3yjqopnie.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3dwrnicjg.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3lvyudpmb.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3xairwmxn.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3luzmqeqa.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3fqilixmn.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3hjtarwcr.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3xgxzxogv.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3iytwbpxi.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3fvucjdir.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3joknuzzq.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3sixotjsq.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3fkmerlhu.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3ehkapmkw.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3qimwxbmc.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3voseybvl.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3yyixnrrc.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3lmydlmib.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3lfgdufke.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3tfqdzdwa.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3chywmosb.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3cvpdinyw.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3crfnkmla.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3utftzqim.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3hzalkinp.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3uxqgiesc.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3fjowoclx.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3mkompdig.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3nfzzecig.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3bklecdbb.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3ifnlvpvd.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3hhflxuap.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3piskyqfg.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3carcpfed.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3vieoxwsz.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3hmtypesr.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3jdwdgtgi.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3xnblnpcy.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3ctyrvagm.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3gxhrylic.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3foliiwyr.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3rkexuppu.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3rcybzhka.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3udbszbyo.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3dvgqntfn.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3minbwgoy.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3almmfcjb.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3duaegwgi.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3sipxgtub.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3ayjenhok.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3nlprhdri.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3pbncnvnw.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3pkwhokka.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3aeyrqwfc.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3qynajuof.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3ejqwyxen.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3vuacetzy.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3kjfqscaq.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3letglsax.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3boaubmch.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3sflurtnm.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3cfjfqqnf.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3yfwkqvti.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3bganecqe.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3dgldtipz.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3twuujwqw.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3aldydcyz.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3scovlkdb.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3qhmmmuvn.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3qzjcjiso.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3hgmuyxye.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3ptidwdsj.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3tetvwluz.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3veqhiivq.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3qzjvbizr.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3xzmacrdy.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3hzumxtxj.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cooiecpz.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3pegwpgal.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3snvfgbgi.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3dzyflwew.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3qjwjbqtv.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3anctchjc.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kuhfgeii.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3ruomlrtf.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3zhryamzp.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3xplzeeno.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3nuofljsb.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3xeyjrrbc.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3uxmlzuqh.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3pzemjaqq.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3enrbzmcm.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3vivetzay.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3qfersgeb.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3vfoxpsmj.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3xypjfppn.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3nxgrzvkm.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3djhhpyan.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3hwulcdln.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mypbyvfv.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3hwtblocy.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3qkjyirma.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3tuxfosuk.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3ruvbitce.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3unincabh.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3eohhcbbc.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3nywvmsuk.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3vvpysjhf.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3bgehtutl.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xlcmgvmx.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3pnsqbspk.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3opzgmcyi.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3rawtrfjp.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3uvvveqbf.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3sxlzhhaf.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3qmdznqip.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3cumpzqwz.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3kdmxrmcj.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3tddsjsmd.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3wznrfxuh.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3cyjqizwx.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3kvgtncob.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3yykukqtf.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3nopkytgd.html


<!-- 参考信息 -->