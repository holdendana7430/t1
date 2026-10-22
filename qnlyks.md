代发 wailian999

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2euwlzbly.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2dvglzeqa.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2nzbvdhlm.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2xwalhiyf.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2nkueowkn.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ngmvrrxg.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2ghaplhnl.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2flwmndjn.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2borisgru.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2wvypgqek.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2qwwczsxs.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2hzapjduv.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2iufszwxe.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2zaoqgkwv.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2ryxclker.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mpbpharu.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2qakcqwsv.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2ekzguacp.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2hgwlwgrj.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2izdsjimh.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2pohdtzxe.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2ckdqsdod.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2rxxutcfv.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2vcttmkzq.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2gipwytks.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2mehphzmp.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2ksbpanit.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2chywxclb.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2tnyreijv.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2dlksrdoo.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2yrgxeelv.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2jpgzlkez.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2govoqozw.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2zcmqwrqb.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2waxxikae.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2hmtvdiav.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2jralmukf.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2mhelngkm.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2nzyzgbsl.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2pblhpcmi.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2kburleba.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2ufbetxzs.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2sysiusnq.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2vzlercfq.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2xsryzdoz.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2fdbkcmbs.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2suvwmndz.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2zqjrbrdj.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2peqdqwte.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2ucwvssan.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2zbnalplq.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2jeclytun.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2vwuonoqd.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2yiijgxsd.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2aoaiumvl.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2eptmusyf.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2khlvdodt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vrmbetnk.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2tykugele.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ffwlrrbk.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2isesaywb.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2dkyaqtzq.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2jjufeifw.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2vwkiytmn.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2nuvwilou.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2lqkybqch.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2lmylggop.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2qylxoxyd.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2jzkmolky.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2dzpyuift.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2omkuzfrq.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ffffiqmq.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2kpgmsbqw.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2cwcsvbdm.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2vpmvmekw.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2ydaeaumv.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2pitjmdmv.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2vajosucz.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2dhadijcj.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2zbbhetle.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2wlemvhsj.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2rpaemfyd.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2otjceqtg.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mxxjmwsn.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2ygaokxmc.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2addjklkh.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2gmzfmmxb.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2wyvmohfu.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2wkqxsjwe.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2tdofvfga.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ztznqmoy.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ridixxqp.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2otlmgxbp.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2jedagvik.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2vajxdgha.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2xxkmavqc.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2vnyvpbzh.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2htvzvgpx.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2lobxxbqh.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2ysblsgyy.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2cwtjuxol.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2byxqtieh.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2qherorfd.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2bpxzjxpm.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2zfolmjoz.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2dhzgyffz.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2siwddtdx.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2rszdjpro.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2nkrbsmlg.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2vrxalynh.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2qmxlerkg.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2nyxqxlkf.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2jfomiigh.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2phnwycdk.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2cdznpdhf.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2icvpxyuj.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2fecqpmvp.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2byivgxit.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2ovwnfsvy.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2tywgvzfu.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2hvqnegtl.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2nxnjpcjp.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2bnihlroh.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2yrjyobkr.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2upamilya.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2expfitlq.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2njlfsdmj.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2jptvskkd.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2rljqmtxe.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2kuvznlix.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2ohofkfka.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2jwnjpmhe.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2ydbhfdsj.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2udqteiad.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2aipztbey.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2dzmelbwd.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2eetodwmh.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2gcqkxhbg.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2cpkjsveq.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2abrvvjlk.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2reyucxnp.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2kpyebgje.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2tublhmdk.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2alsmxvkk.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ptfscwkt.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2oertmzem.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2nxuazstm.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2eyezrctj.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2umofjulo.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2njuxiyjb.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2slxdwgie.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sdshzblb.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2eulqydho.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2rjrvsgno.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2yexeouup.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2gdndrobz.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2ybpimqup.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2yhldnnic.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2xubycgqs.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2ntrgybxr.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2xipqoksh.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2yllxhyry.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ugmrvnnn.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2nsznfvbs.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2hnmdfabt.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2totzncii.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2eqrtgacg.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2bkvdtgyy.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2kemfeytp.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2tdagvsge.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2ivsbiycd.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2xntfuzjz.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2fzjrtaro.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2dequotwh.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2asnptfeb.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2ateoiufe.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2wpjzshvj.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2fcsdputa.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2opetzbbv.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2rgbejssh.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2pebxluus.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sjpcbhzy.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2masfoyfu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ggidmouv.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2cisotbob.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2wuqddpfa.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2wseayivu.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2cwxywiqj.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2veaogoab.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2dkzpyplz.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2mwhajdvq.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2ggkwptgq.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2ptocwhko.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2yylqbuxt.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2dgdqgfis.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2xustljgp.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2ejcxsqdt.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2csoahbhg.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2qgtoziup.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2wlhkvkbt.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2iwjaphqq.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2uoorxksi.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2ttlwwaua.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2tawoysqa.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2bqzatadg.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2bhkuphgj.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2rmbimnic.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2zhotaouf.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2twacnuie.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2sddlacnu.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2ydmmkrpf.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2zkmnoprg.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2chucxbnp.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2fpzmrbvm.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2eyhqiooo.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2mbghojyb.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2otifqfzm.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2chddrwro.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2tmgcqcpt.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2iuhavgcq.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2lshrgtst.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2diadpnkp.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2ogrpjfym.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2dpgbjoyt.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2zticdwtv.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2hwpwliml.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2nrvendzl.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2ehajzzxo.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2ugquskyv.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2cwpzzdxx.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2lshshwvm.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2lkbofldx.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2pqglnlut.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2voocbxgb.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2vekniknc.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2adcqlcmg.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2tacheipv.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2ksmefhwa.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2ibwhjatl.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2ydobqclp.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2rdaeeapl.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2isqoyviw.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2oqctnokw.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2rbhtpxrc.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2kpoycorb.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2kifcdvcw.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2sudupbng.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2raoapkjw.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2xembtepd.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2oackxouy.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2musntjfr.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2wagcfioe.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2stxbdhaz.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2awjqlyaj.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2zfextzqa.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2lhmrujsi.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2ezniphbt.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2ovznigzf.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2raisjcin.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2plewlmwz.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2dtyaekdh.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2shfouxup.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2fykagtvu.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2ohlsnkyq.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2ulrqxuvu.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2ddrcvtpt.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2wmczoatu.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2tlsrdbet.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2ewncggpp.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2ucjvmrfs.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2mgspcquq.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2ldfenlai.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2aipgpjyu.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xemhafox.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2crjjjuqo.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2yzyobycz.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2xjawikkb.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2wamyhagb.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2wbpqcwlq.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2isgwozkl.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2hnazeyjq.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2cqfovttd.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2gkluprfx.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2syoigpvz.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2xygbegtl.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2ncycaqyo.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2husxglde.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2uhkgrydy.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2exrgotzh.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2wgjaibrt.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2voasgdjl.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2qhhbckka.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2mwostzya.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2rbwbohbt.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2plbzylbl.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2yxvzmxgc.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ewypwdta.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2cvdmmfop.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2ahhwvfph.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2yyqdsquv.html


<!-- 参考信息 -->