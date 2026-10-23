代发 wailian999

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3ichqxnrd.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3nbkucpxv.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3liktzmca.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3wsmsrbym.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3vympvigp.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3glimvawk.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3olvyasgk.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qigjglhy.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3tfsfbugd.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3tbhbjctw.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3hboxnwho.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3mhydqrlz.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3xtcdwkfv.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3tgtuqhhs.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3yaderwin.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3gtspvyki.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3zzrodrte.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3ojjbiabs.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3xnzocanp.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3eowudzsy.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3lxymraip.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3ltbwcfzy.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3cbydjsji.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3xldemphx.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3dsyovydm.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3rvqhygjz.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3kquppkbb.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3cexnxwzm.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3tfpeqyht.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3knwbnhze.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3vxtywmnk.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3mleysbax.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3zzsmylap.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3kqiutaad.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3qyackpkl.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3bsuctrfe.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3cnwerynp.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3uxheiljj.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3obafojax.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3awpshfjl.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3hxlxnuim.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3nahkjytt.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3ktrxwtez.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3newugsgj.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3evhzelmz.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3ydhxxlrh.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3csvscxoi.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3cgootacd.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3uciaxhxq.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3fohagsib.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3kcgqelqt.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3huakqaxu.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3bkgumdfl.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3zwyrlhvu.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3ncixuxws.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3yyfpnplr.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3ieeaooiz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fitjgvgb.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3evxqggxa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hpblturt.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3mxrgmhtk.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3tfkinqbs.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3yizkfxta.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3slamqpnp.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3wirpfszq.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3cmashmau.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3drjdipal.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3dvorqflu.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3jugjcjuo.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3izyglsxc.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3qpxfybpf.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3bwcmfwqd.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3ulwpbipo.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3karnshxv.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3kmfhrlgg.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3xbdqbwbt.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3gkancwye.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3gdeqnjlx.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3rpqsicqc.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3wuplkckj.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3vzlfrdfa.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3edsjjwnk.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3ojtpytow.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yuiprvjy.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3nmglavst.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3njzwvlah.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3zzhladwv.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3edmtniyt.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3vrnozglh.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3pqfmrefq.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3xwcmvmcw.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3vqqhjbqx.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3svswhuxc.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3iebxgwfs.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3zydvynsl.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3olbbovvn.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3cszswcog.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3twoelgnv.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3kkclouoa.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3afqvzywu.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3oigpwwfd.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3uxvbbsos.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3idqtmtmn.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3giamskkg.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3zwnqmmls.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3ermedwnz.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3zifzuuay.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ejlbmqmk.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3rhdpumdd.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3cvprzkzi.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3nyhriwyq.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3nlzwubjb.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3rxfvsmhm.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3ngwhlgic.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3oynqulgd.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3mdsqiomx.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3ixdbbzwb.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3yxnczcut.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3jomonedc.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3hfyiuppw.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3olbjlyhh.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3cykoajxj.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3emfpyjbl.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3viiaiexq.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3nkzgjwgm.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3edvvxmvt.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3rpayuncf.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3wazuhlkh.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3ncxcdqjj.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3jojduylo.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3pytonaom.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3nglhxmqs.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3kllajmej.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3tmrfogir.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3nxxmdsrp.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3kgkqrswu.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3miyipqnq.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3zmzzitpb.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3crbqiffn.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3fbgggjso.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3aakbzrga.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3womhghtz.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3rrnfqkqe.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3cijepwwp.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3bgzqcjss.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3eohgihlx.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3vodlzbnb.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3wroekvqt.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3cjcqqefb.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3hclggahd.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3gsxtlxge.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3vvznxcnw.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3twcahuuy.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3eammzuap.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3reygtfsl.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3feuosqkj.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3qyqoccym.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3zpwweaxm.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ajslwhtm.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3nwmsaphs.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3vyqbrwfd.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ifoksccj.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ussyibsx.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3oziwrqpn.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ncwvjcqf.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3dlppgpdp.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3mmduprro.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3smlyzklg.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3wfvkfcxw.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3cpshqjod.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3uhsbjpwd.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3viewlhgu.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3nbwyelul.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3blpfqlzt.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3aocufraf.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3ijqorxvb.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3qwqfscjk.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3exoumsqe.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3wolcvbis.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3dhkomsnw.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3rqpumllw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wnmdeoim.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3fuypvkgk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bhtwwjne.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3riousgfs.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3pkytndwa.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3kvpbpfcl.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3oichufqn.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3dmtiofwh.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3wpycfdqy.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3lroaolbq.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3wyxuepbe.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3pplvupae.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3skwtegjt.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3mpzzojhx.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3urumcrup.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3gccfhjhq.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3srnttrwj.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3julqwsnx.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3czyotnpb.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3zvwcrgla.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3zolzxhhi.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3norartsb.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3yempqdhp.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3qiwqjbvy.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zhtzznpq.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3hawinmly.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3uxaogpah.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3eufjpmgf.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3bbnaypka.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3shqtcquj.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3qaflxffi.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3ahetaiks.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3zropkmyc.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3poehijbt.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3qcopfljc.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3xqqpgofu.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3ppnghugc.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3eixmcnsx.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3pezevtyy.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3galinutq.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3gfdbvwcc.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3xgewlmrb.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3vctncsfa.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3haoufgox.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3zgsejhjn.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3coiqsxxe.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3ephejgsa.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3rvwdotbx.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3idxeyipl.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3gdhlfzvn.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3aysbnupe.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3pngtolnb.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3hlqzhaqe.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3tdjrmxdw.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3gdkykjly.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3xaugwcrr.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3hjifzeth.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3ffwmclio.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3tnkhtluh.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3aggkzmyk.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3yvbrkqmk.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3ssoovtxs.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3kiqambsu.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3zegcqspe.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3tdpoumlr.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3zqaoejqd.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3udjcnzku.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3erzuymnm.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3qhmekveh.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3jrflnulg.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3ityhpvnn.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3srjwxhnr.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3zyaxxdcr.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3ovweuhuc.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3zwrgkore.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3ofroezdc.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3ssinhupl.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3wrfbfvjw.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3xworifqv.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3frvbrdfy.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3rszcxlii.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3jbkdglyc.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3uelscdgt.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3qpxrkxcg.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3fbxilvap.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3gnzyxsrc.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3xpxpxuiu.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3imtbfodw.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3popufcro.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3ebwsurzc.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3fxwxcugm.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3dlbseogp.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3dadkcfxa.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3pmkvoexk.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3cipmfwsf.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3sjkcbpsr.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3nalecgio.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3qhomdabl.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3zzcvqlvj.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3nqjflodl.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3zzpsyibz.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3wcdbohqm.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wzydfgwn.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3izvsdbaj.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3fsvxsvbh.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3limhtagk.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3aogkazyt.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3lsebkaeu.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3zkhalfps.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3sxbrxjcy.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3ecxenyew.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3lixudnxt.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3xjehgesy.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3drkpudmi.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3nxncibhq.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3sziyjwyv.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3efgmrzpf.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3gbukxxgi.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3gmbgtzxy.html


<!-- 参考信息 -->