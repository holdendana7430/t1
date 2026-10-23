代发 wailian999

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3tcxtmfdg.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3lsjrehcj.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3pnhtoenp.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3jlgghjtm.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3avizhetu.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3fbutyxgf.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3lqhfqgav.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3zbhjmsms.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3xtodguus.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3ebbykqot.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3iokdrhhs.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3urzktbld.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3xwizmrng.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3wcffzatm.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3ymomgngb.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3slkgibnl.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bdxbvikk.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3zrvztixp.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3nfxpqtlp.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3xsyugfqi.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3gfzaoshj.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3tdhqbnlo.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3yypkzzel.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3cmwialqk.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3fkghovbd.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3rshjtfas.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3bpnzsxdk.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3ezghidbu.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3sgpnadyk.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3xbfqrwwf.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3ptmbuigt.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3djzvsuul.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3wqwqewsx.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3wxnyxpvv.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qneoczmm.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3vyzvxgfr.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3atnqhnvc.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3qqweywpe.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3girnqkfk.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3kqtlhrzp.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3unbjcdsf.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3exrzityc.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3ahwbyylt.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3ulehfpdu.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3gfkloeyb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uuxfjpka.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3qhkekchj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cxvwjcau.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3xdmtkosx.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ywbjgnez.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3nvzvvaav.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3uyryaqwf.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3jdhgwazd.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3lvmbvanh.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3aqeiiggv.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3cxazwdax.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3gcnceoek.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3xtglwtxn.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3qivtinve.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3qxtmindm.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3tsmgecth.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3shrqjnfc.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3hebyzkqs.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3omwymtdf.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3ekyjdidq.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3vozuavom.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3xhsaiwtk.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3vuldtuhu.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3eratiqbp.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3rspozqyk.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3pfmstcgq.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zylbdcwi.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3xwsehqjc.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3fjppyfrs.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3lgkqjuor.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3udtzfctd.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3yooxcinp.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ipyuodkm.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ldgaznmb.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3sylkedlf.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3azkqzolv.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3gbiomqdh.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3lykbkrjh.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3rmnzdfyp.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3ttsudvrk.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3rhdmejtx.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3nkjaylqh.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3dugohilf.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bbdyyfzi.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3uztjypko.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3twsakvmy.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3vermtkfc.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3xlctneir.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3hmfkagdm.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3iddkwlpu.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3bcwgxvbz.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3ylvlxflk.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3igzqooti.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3ikinsuun.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3njdckoaq.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3zvqxjvem.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3gictowsj.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3xpsxuaph.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3gvijybuw.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3uwtxuely.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3dixnsaux.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3elprkgpo.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3zihyoqdt.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3klsyyjda.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3bxcgribz.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3artoftkk.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3lfxoumwc.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3savahvmh.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3khfnspzo.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3hxewuivq.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3uslavyhj.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3sfbhdljz.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3pieccxfe.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3uqzukkzx.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3ewaejydk.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3xbnrvads.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3iremwvbe.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3dlshgnbn.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3dvkckiku.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3sibivkxt.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3sxcmlfmx.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3tldquzpj.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3irxtthmc.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3mknotulg.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3xthtvklg.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3afsiwrhz.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ocmdwwci.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3zsrwttwh.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3wnbkvpoa.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3yafcnaqn.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3tuniswqr.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3pnolsyqe.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3vvxfrynt.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3rvulkpzp.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xpfdhlal.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3pwmtstzs.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3wybbjljk.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3izgxubyw.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3ksoqjaqg.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3zmleqiws.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3yhgyatwh.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3eyzbqxex.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3gonsskei.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3wdezqgpq.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ebezabzo.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3iciohdcb.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3spbvvytx.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3wuapndjg.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3uszmamiq.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3wiqbnkha.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3lbaxzqtk.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bhtmzhyi.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3eomfeupg.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xmmvexoq.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3nqyalcwg.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3gaullwtx.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3ithcsoxk.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3crbbcbge.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3vmophtky.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3vjqjgdxr.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3zgdmawjh.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3hanppdwg.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3vufauzll.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3usbwulds.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3odxkezic.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3tecbutbw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xyqxeavb.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3myfsaifg.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3zwzxaegn.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3noodaaoe.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3znnadrwv.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3mlkurwny.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3tuqgqlzp.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3zxlpquzf.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3pppdxzmh.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3dmirflol.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3sjiqcbmu.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3onvwsixk.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3qdgchdtr.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3uabovmua.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3vfixqkur.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3mqevezyk.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3owoaiulw.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3jvsppind.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3yeyasxkv.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3zzhvaixy.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3cpvellzg.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ovdrybmf.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3dktasevn.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3bfmjbqcp.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3lhhbtvps.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3wxpxwyia.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3lrosoizl.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3zhihptyq.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3dqezjjsg.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3fnbbbmks.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3bmvcmxvl.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3gomrybir.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3nbxzqcsh.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3jnyuehby.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3looutvsq.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3eixrqrfz.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3kfoxvmzn.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3ambblodv.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3yrxbhwhq.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3owxsgkzm.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3hzedzrzj.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3meoitjbi.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3xwvqfwlr.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3bvlyzhvx.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3feiqmhmw.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3cbgycqhd.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3xsivxrka.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3kvllnhjr.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3drxjlqnp.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3hhjkszyg.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3qrqoayjk.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3uhclrnmq.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3hwylqtnr.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3ufjdphuo.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3mcjzawkw.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3pmmrtjlm.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3hrljpqln.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3baofarqs.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3xeppnjvz.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3njpjsrte.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3anxudslt.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3hxbevoyl.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3kddirnxr.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3khlsixbm.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3htytmpnd.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3oivoqtmx.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3wnncqvoa.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3vffwclro.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3tnwcoztx.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3wjtyfxln.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3xnjjmmxi.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3bozqhaiu.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3udrddjee.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3ddivomba.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3nnuxantz.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3gcgvyfnd.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3rqttstgy.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3ismxhitj.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3rrcxasza.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3bnumiblq.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3usrxmfny.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3fdwinxur.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3ytsvtqvq.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3qlrvpqyt.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3tgbcehaf.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3vtnybtsy.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3phetzeui.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3nbuaoyzb.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3awlpoxci.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3erxfgjza.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3htbbmqyc.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3xreajvhr.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3balaxaaj.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3mrrffnqe.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3emmnmegl.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3vuxzntsf.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3vlugqadz.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3ihgynivo.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3vpqvnmvx.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3dgsxxzvl.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3avwxopta.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3aguovmli.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3nqgnafnr.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3tcysspqb.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3twtzxmcc.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3qmwmwwpx.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3zpfjcglq.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3pmlaryod.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3xebbymlc.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3oguoufcc.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3ybbxtunz.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3ovmyuojj.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gwtwauhk.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3nbcxxcmr.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3axaifsds.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3suptvhxp.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3vgkectht.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3reaqfhdh.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3hacehonb.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3bgqrvdok.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3piyatrfg.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3veahngna.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vbxgubna.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3bpevadni.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3wifoduqm.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3hpoefyfg.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3ioccqohx.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3vfqtvoex.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3mjgheumy.html


<!-- 参考信息 -->