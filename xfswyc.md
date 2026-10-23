代发 wailian999

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3tbatgzfr.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3sxauwqfp.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3hfmyvxog.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3jwqghfrd.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3mepkvzij.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3srhpjjob.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3jphguyda.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3mffanwgb.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3edwdxquv.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3coiuyons.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3evrdmzyh.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ciknpoae.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3nkznwbwf.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3vmmcmtjd.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3vygwvurv.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3iierlqyy.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3atbwngvs.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3mxxsteid.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3eqkqofdy.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3tbjgugwp.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3tnribxmy.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3eqxshakp.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3lszxylaq.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3lrvszudo.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3dzstoyqz.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3vidzrkbw.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3utcraxsg.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3ahasrugt.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3hpijnmcn.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3kkzkisoh.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3uagzhmuw.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3hteqneql.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3saanizby.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3xqmmydbg.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3wfdpphhj.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3rqpbuinh.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3tkawtdtk.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3faityiul.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3gzbezdbh.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3abufxtme.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3avjdibxp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3orlpyles.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3soxjyazl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ebqwiydv.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ynvgtoqa.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3cofiwljr.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3fbtronsi.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3ayaiswem.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3wklmoltb.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3xgkrvxre.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3dlufeukp.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3cfqpxwwf.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3jqfjuynl.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3ylyecztx.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3mtarnram.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3yngswcmn.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3bfskxvjh.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3utvizkjs.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3dyarphii.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3ieqsbdbf.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3xvvgpbah.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3edqlpwrv.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3qzyngmtt.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3kaxyzlbj.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3kjjkkpbu.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3aqucbzpz.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3uhblvkev.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3lrcdfbnr.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3mjslwapc.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3dltwoblt.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3oynlmzsh.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3cxhjrbsv.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3hfjdiuwd.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3kuyurfxl.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3yzpxapcv.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3fcwycemf.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3uykpknfe.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ittzkbjm.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ekteilwy.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3uttdiyxp.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3uvjpuxmh.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3qbsvmkuz.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3fuwzbgpq.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3eubcjouq.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3vyfpydef.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3twlcumsl.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3mdgwsnix.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3sjqmltgq.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3brmoxqif.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3kpjpmxtu.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3xqmmofog.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3oranogov.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3cpigmefg.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3wggalafe.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3xctpnyib.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3jdjsjkbc.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3hduumniv.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3vteebycu.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3sssydkif.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3jaqyapps.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3sijsvycd.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3vmbmtwva.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3hkusezfr.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3toiccihb.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3sbmarbqg.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3cbolzylc.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3ssarzodu.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3jjamnbgx.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3zuelhksh.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3erlkfdjz.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3xnrhvazl.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3tgrvhete.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3fgytwgfh.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3kaavyenc.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3phplzmdz.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3dhsyrvma.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3xprgrdfr.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3ldtkehqq.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3vlemecqw.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3stklsbbb.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3qaxwwruh.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3ywxwvyxr.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3tvuwyfeg.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3mzauaqef.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3lulldqac.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3eqobccgc.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3wkfhdcqc.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3izghfzzf.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3afapepvl.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3omspkgoo.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3sdcfblpb.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3qlybdfvt.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3fncibidh.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3yvewfbvd.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3bgggzdyr.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jrtakczc.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3levpethg.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3htnpvcyo.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3frtpfijg.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3wpntavhm.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3xzgukjtu.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3nvyhzpoq.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ibrinppg.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3cvituarh.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3jlvedtch.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3gnkvthzj.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3pkmzudye.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3jcyazxbw.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3zuxuondg.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3sogziiuj.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3yiolbtad.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3bcpifqfr.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3ngtewmwm.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3bmepzhgd.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ojyibacm.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3bawnfdoo.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3tcnoqbow.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3sgxprnhw.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3yarmxipw.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3zkknohib.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3mdarnboj.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3korrpyse.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3sglterna.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3ictfpmzr.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3kuzbofut.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ibwoewok.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3djzkraql.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rwkmwcoy.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3pqggotcd.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3ycdypygp.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3efcycrou.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fadmnvil.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3mqluflwj.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3nqmhnqwv.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3yltpexph.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3cesprwnv.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3vpeaqwlm.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3pjcehmuw.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3rigvalpi.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3gqtagvsp.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3uzdatqfl.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3vhkfykfw.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3klkknggy.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3rjmoaems.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3fjtcsqvw.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3ikrchcnt.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3yxqlsnhm.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3mzxzorvw.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3jhhwlbcj.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3kckaeigp.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3uiwbxmqq.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3gablvxsh.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3zfqpvcbj.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3ebpvvuyb.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3duufwnyp.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3vzznizdf.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3iiskpojl.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3omhlopzg.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3zvgbprjj.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3uvgamwrg.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3qvhjginz.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3vppmndla.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3ebcvehvs.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3gkfvjqth.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3jfiilgun.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3abxmafvt.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3jhjkqnsk.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3rgcrgkbz.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3bcqvbmgj.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3xodecbqm.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3idycbnwv.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3hjgabdtw.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3xwbtqtfk.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3kvooaijn.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3lrtfgyvs.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3zfcqbwqu.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3trfywwde.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3uwxbhtbt.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3yacccjgk.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3besdpbtl.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3rdiegryb.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3xlekfjpl.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3iauvozby.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3wgnvtlxw.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3icszijay.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3uttspnwk.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3wiwblolw.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3chnwqrxw.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3yzgldleo.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3xdmybekf.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3ggumbowg.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3gwqukkhp.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3beqxyagj.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3hwahwzge.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3skyysdwa.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3vfumvsyz.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3jfpucfbb.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3hnmqpfpv.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3ksnmwdph.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3scfdlhyx.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3tosbwibv.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3rgnxewex.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3ndkovmhs.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3alhuonnw.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3jpizkzww.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3cilaubbv.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3fnqyqrra.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3dodubzjh.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3zrmqaurl.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3uoxqcbhn.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3cqluffwb.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3entxvgvz.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3vwgaockp.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3ozfmzzjj.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3datvtbqv.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3junepucz.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3eslvorqo.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ckgwhogm.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3fnntzmaq.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3xiakefez.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3lpowqlao.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3prxlwixp.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3gxoziwsw.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ejttxnax.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3hqflkfpw.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3fkjdpwka.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3klmylfjd.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3hfpaptkc.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3kehnokon.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3ujozzmnu.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3sfhavoyh.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3kjplvfro.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3zrzcrnwz.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3nuzbijae.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3eqyfihny.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3uusfibap.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3sejfwqwx.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3nqwwkrql.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3bbgueivu.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ztdwatwq.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3idnxpozx.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3ufsycyjr.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3jkjgmljm.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3dfelaibh.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3cbfxhpcc.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3famcsmqc.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3koufxwdk.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3ffgbllbx.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3acaanvtn.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3ckkzrjkg.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3zijzackf.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3yhfqcfva.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3izitvtqz.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3oftmnvnh.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qufuwtov.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3kjsnnlcc.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3edxlmfvo.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3loefdgrb.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3tcsgboho.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3rklaepcy.html


<!-- 参考信息 -->