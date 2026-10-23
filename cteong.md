代发 wailian999

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3dgqxbypr.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3klhlvmnx.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3rfftptjt.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3wancpudr.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3crknjstm.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3ugoadnde.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3imkijjht.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3tbjcfxwr.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3vtuvevxd.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3cjsqoteo.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3tkpuyeon.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lsqtatfs.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3fnbkxmrq.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3oiwrbrgm.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3nbziyduu.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3gichwhkt.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3jvirubwm.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3kgszwkfa.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3zdrxljbz.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3jpavpkbe.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3pjkwtrgs.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3pltptjlx.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3nhhdxhcd.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3ltpybpnh.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3hpmkpldx.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3jslloqss.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3xdptqlrw.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3nofadqlv.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3kavkofuh.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3prpgsvsa.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3utjdemii.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3fousixtm.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3cxvxhcfk.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3hocomcwn.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3tkmcyjac.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3tqgnvicr.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3slevxvxh.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3dmurojdh.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3adqcrfvw.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3moncdufs.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3rtedhvwm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jbxzkzpj.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3gmvowcuj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bofdphjq.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3sbdfoypw.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3yvfsekkf.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3nsufyrwl.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3qaaducnv.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3cmobvtsc.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3hvkyyoqb.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3ofnlwkfh.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3auzflnsz.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3vzqiuqws.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3pifgeuex.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3cikmybfl.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3tiesefuc.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3eapechrl.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3fwuxxobw.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3whcbmyhr.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3syqzjvhe.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3eijtuxlm.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3ftxasuwy.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3amflqzwz.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3jfliyrek.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3cbsqkhcj.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3ilxydaxl.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3ciffdhgc.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bdnniiwe.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3cugphvmx.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ugdutqep.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3wxlxvpll.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3plhzsnfr.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3thqfyczm.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3mbsrexcw.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ipilndey.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3dxlsjevj.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3eidsettx.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3dglwdgsf.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3cngdibva.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3peoklzrq.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3wjxsibcv.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3kwdryxol.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3cazlckoq.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3tvixjlfe.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3mjqzvcwp.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3ihroivvm.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3vtuuxlfy.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3uhwxzhsm.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3jvxqlnni.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3fufyypvx.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3koxoucee.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3vqyzbyvt.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3psmholmf.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3lgelpfhd.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3dfmxkorc.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3sdxinyae.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3flodtfqj.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3msczeidr.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3aobyyvpk.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3rahjsgex.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3gudrjeol.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3tfkgcdwo.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3niykjtom.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3cfxrufvw.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jhcwysgm.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3apbmlfrw.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3ehfukwlg.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3xnombmnn.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3mtaeryrp.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3ynnfkmaw.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3qfdvemji.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3kwnmjteq.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3qawktxop.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3fuemlvfe.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3reryvzob.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3pihhdjkf.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3gafkyklj.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3vilpatza.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3nbrlsycs.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3utwxbknb.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3rqknupkh.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3ukkkslbk.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3ccfhsvrv.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3knjqplkg.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3bwtkrokp.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3wlntdwoq.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3pzgtemjs.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3wprxeqby.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3hdbgsine.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3zcsbycly.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3qludcdbb.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fijbtfrp.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3jbmieypl.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3aaggblic.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3bydrdsjo.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nsdkkydz.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3ndgfdgjc.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3rdeapnyp.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3uknelmdj.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3scnnafff.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3iswdgffm.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3tchdolcq.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3myzzypus.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3euryyrge.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3oorgtwek.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zrmhxjbh.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3dtyokanv.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3vtmuegur.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3eunkcchk.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ndstljzo.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3ecbqdkpo.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3waefbaok.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bmeqybxg.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3noyindpa.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3cbaufzwf.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3qcprbiyq.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3okzwevje.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3mnkhfvhc.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3oiukmiky.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3klacgoqc.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3pzwsjwzq.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3gbznunla.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3sxnswyoi.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3cetsxpvs.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3gjzptkxs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cttpdpbl.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3eledhgfk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eyumyxpv.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3covgmpon.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3yhadjbns.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3qymqftkr.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3ellkbaej.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3jegcksvo.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3hspsbgcs.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3uxyivwpa.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3aueitoeo.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3fifsznpq.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3engxwhtg.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3kxroocgu.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3nvxipvlu.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3uesmllex.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3yjdmlych.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3ecvnrsdv.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3xfkgpjtz.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3dijzxfyk.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3woolzzor.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3cmdjghnj.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3begmjekp.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3lzmwthhx.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3nfohcclt.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3rttnlteo.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3aloistbh.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3hekqjanx.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3aqqlqndg.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3lhklnhtm.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3zsrqunro.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3fdtpcdnr.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3mfqopwge.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3ssujiolb.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3pljgfogy.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3ilvpsgyq.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3lrkutuox.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3rwdxwlss.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3smoaalsg.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3aunejsip.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3rcqueflg.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3haknsnxf.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3tjjzlutp.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3seccofxb.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3cgrmqwoz.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3krgnemvl.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3fwnrswoh.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3qojwkkug.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3prbyuqbw.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3qdpfstlu.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3vkltzbca.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3ffwoceqr.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3eppjkkve.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3wketcxba.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3ikdmatax.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3cfnlnstk.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3sosmfhlg.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3vqpoftqp.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3mewdngrj.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3abwirsez.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3ufztreya.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3ecijujwu.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3tjyfmgax.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3vptciilt.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3tuofkaow.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3fikqezao.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3mnflnevl.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3hbalcrbc.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3mhijgdbe.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3ilesevdn.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3ebqtwnhr.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3kbyrljee.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3hhhnsvwd.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3hutgvmmy.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3hhlflswi.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3qdjgsizz.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3pdjdalge.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3trnpbwnk.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3xsxfahoj.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3zofztifv.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3yjddgolg.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3dbpknpfy.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3dxltswnu.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3tjnxmlaw.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3fjvnuxlh.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3okuduken.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3gcwbvuxj.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3lyhwaxwj.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3sqfshzse.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3teermzrq.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3gyeypkbg.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3svpesaak.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3yubnqdhp.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3ddirwgds.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3cqzrywph.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3bhgimujw.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3bqyjypni.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ocmojmpu.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3ljbpljrh.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3lfumuufe.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3njocvtmj.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3xqucxfuf.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hjmdalhy.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3fphszdhs.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3hnsyblmp.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3jqnlctzp.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3mhlbxjga.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3liihvdxe.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3ymhkmxhi.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3zfvhotes.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3esfmxrql.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3pagzorek.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3xctndciz.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3iupritib.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3lvuidyde.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3wuzjwjaa.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3kjnmofzk.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3xxdtvgki.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3merlqmvj.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3npyvrjpt.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3jnobwlrc.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3mucygnhv.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3lkujopbx.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3jlerfmxh.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3kfatkije.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3tvgbttil.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3zpmaqjan.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3fuqugytv.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3yvmoicjz.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3fzqzkppp.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3cpfucsem.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3lhpocggv.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3twmmzyfh.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3wzhniraf.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3dggkfcsj.html


<!-- 参考信息 -->