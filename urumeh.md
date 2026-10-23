代发 wailian999

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3gdvzjoqd.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ttmxdoey.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3zwqpiunu.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3caqvbgzj.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3voebjgyk.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3rmzwestu.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3qzxvgkjf.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3vxhjirui.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3aklexrka.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3dvlmsgjk.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3fxbakruw.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3vdfsphue.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3rjwcaljr.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3skvicdhu.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3suuruoin.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3pqgvgeia.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3nfkukrte.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3ghswbstt.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3xyfcxyia.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3ypcvnkpa.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3glwsrucz.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3jrgssegr.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3ggdrzbwe.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3pnoqreei.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3foruhifq.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3rnoyzcov.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3hjcaiong.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wxhztlol.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3tocgured.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3odxhpawj.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3sdknfgvo.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3trraiamp.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3fnkgnbpk.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3rekefyri.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3zhbjbjdm.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3tjkysmxe.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3kchnjipt.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3nbtfappa.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3pjnmfcmw.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3znuxryax.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3mqfqguug.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3wizaqxfv.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3sjgpuybv.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3pzwwalle.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3qsccqocz.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3wvkpresp.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3tpqcegtb.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3xjzsriol.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3nbsdadpj.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3cwhpvueb.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3xvgqrzqk.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3gnlxelba.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3nczfbwdt.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3aowujpxk.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3jurqhanr.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3bermzczb.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3oqrhkkvv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bpmfftwd.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3yzpbkuso.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qsdrrwej.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rnztxzvu.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3gglcipjx.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3rifmhugv.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3pldaaahc.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3cmfydnde.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3ohldwuxi.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3pzijtjep.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3cqbqwlwi.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3xdyfmpov.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3fgrfuxkj.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3qorhokop.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3xcgnwmla.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3jrntwfcv.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3erxbeegg.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3sccdrkxu.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3yphcvmdv.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3sevavgym.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3rvscuhwq.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3yhqonvhj.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3velmbudc.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3dkonbxwn.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3xgqxoknh.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3dezcxlts.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ynbngnvg.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3ckfphvxw.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3rhefqgwz.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3buccjjlt.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ilzdlvcs.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3twbqtimc.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3ceoijfnx.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hnnpwpuo.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3utyobooi.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3xiytohdq.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3iubahnbb.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3vnxlaomn.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3arxlgbuf.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3hskxmdsg.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3qextlhsy.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3tpwebaqz.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3beobaxyl.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3shxcndds.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3noqffldu.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3qeswryyu.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3bvwpdcut.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3giagkymb.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3higcmzwn.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3pokhjdtf.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3zevcuwru.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3qwyaikqt.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3dmesfwpw.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3brefovhw.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3ibnthwkv.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3csfsslnc.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3uetxdtdg.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3rejriygf.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3ggllyidu.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3atwpblvp.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3advtthwv.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3ierqwodg.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3vhygpllg.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3mbpwenph.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3gayovmde.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3zvkxhzdt.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3ystwzxhn.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3mpodptrt.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3cqnluung.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3dkyhqxlz.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3cseqzhvv.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3rcnqwfsz.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3jqvoiovk.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3vbpsbbuv.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3nxirstzc.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3zaktyxfp.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3gyngmsfw.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3vccbfdcm.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3mhxhwhgd.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3fhrlgpyp.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3fbqtdkrk.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3kmorlduz.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3mzalszur.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3nuwnuueg.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3qsylbukh.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3rtsyzvrt.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3wyedbtth.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3anrtalle.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3bzhnqdnn.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3ytqzbfnj.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3miphfjev.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3imdrovwq.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3yqmnlokg.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3sudglkdd.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3yrfbtxpq.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3jnawdedj.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3bdhctmfw.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3vflqsmkm.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3uzajfvhp.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3akleakgk.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ecjzrxtq.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3luzcrsgf.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3vdwuwgom.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3vjemprri.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3cdmjizvj.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3gijzuowp.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3hyhvsmtj.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3luceigwz.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3zgwtpnwh.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3engcsyde.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3sebyxvmf.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3tmhzqvqc.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3qpzpbdxl.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3fymofaer.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3miyrctnc.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3fkmkoyow.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3qvogagrj.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3nndgtnmd.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3dlawdgpt.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3bkcvpasw.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3ndiwfhkw.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3epqdpdoh.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3hjanyuvn.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3ovjnlkfm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gmcawzbs.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pndltbyt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ayjmqmnn.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3fnlnikra.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3bcoavesl.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3aadsorki.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3kwzydagf.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3lfbsyphl.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3htpbqeqq.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3swfblsbb.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3btqgxohs.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3nzrvovas.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3tbpssxnv.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3icctvujv.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3emdiljdf.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3nufdxjkz.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3kldmimyp.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3aunorqsc.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3rvfgqtmd.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3kgpahahs.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3slirgpzh.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3qgvfyirh.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3bgflifoa.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3qwexdfxc.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rpbzsckq.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3wocmnfxv.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3rtgpvmps.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3iugzxajh.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3wcmvoevb.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3lfogqbqa.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3buoinkne.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3mfvfdhwd.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3aehkuaqm.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3wcnamsxn.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3urygxkxa.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3oymnfdep.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3cmguifuh.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3rmxhjram.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3eqgqxnbc.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3mdcrejcc.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3gbekomsy.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3qnyatamw.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3dhoisgwc.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3auoybfsa.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3wcqiriar.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3svhwaeck.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3synzoowp.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3bnfecdrq.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3auhtrdtq.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3poaaulte.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ihbewdwc.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3laekmkuc.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3zqxlihfg.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3cfqydrmy.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3yqjffdia.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3cwhhgkbs.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3bflqirbh.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3onoxlhsq.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3fqmrotgj.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3jeybzssj.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3bkvpjywl.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3wldwsudc.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3unwknfgq.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3mhmexbns.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3mcdndmfe.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3ixwmpwjp.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3iikkfata.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3fdhlcnvh.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3pxsokqzx.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3iaqgfwkd.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3mwowbyiy.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3dweyuwzj.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3uyeoalqw.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3xqylfvce.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3fztpjwve.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3seavldxj.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3gyrqpbgd.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3azbeltvi.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3ixlmlduc.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3skejwjtw.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3bgmxwwrb.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3zcczsooo.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3vbgjcrgt.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3hllwvwcz.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3beiniypt.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3uitintzv.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3jnfyeaye.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3spccdteo.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3pmzjgowm.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3eesuiymh.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3ncyvudtq.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3qoxkpgcy.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3rszjbdag.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3sxzkclcp.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3omykzboa.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3hjamdisf.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3locqwoyy.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3akjvrdzl.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sgyhldks.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3kofmfbpg.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3xzjsmrfg.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3wfkwyuqt.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3cfhuemrn.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3crtawkvl.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3dzgiaevd.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3ytyffyve.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3bhbsycud.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3yrohorau.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3snmwqesb.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3ocbbosep.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3eoczwnuz.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ozqcrygy.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3hupcvjjt.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3jqoywlfm.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3mllmxlzs.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3wgtuasxg.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3kfdxyyiw.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3igpqpxpb.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3iqaxrznt.html


<!-- 参考信息 -->