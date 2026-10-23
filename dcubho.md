代发 wailian999

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3slwxfxrw.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3aabpwfbd.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3luehlegz.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3fgkrjfye.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3mpwsyvsd.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3vjeikfvl.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3jwgjytel.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3yjgzemet.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3flbqtufu.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3mouyvbqn.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3nhjyjqsv.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zkvrmuni.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3ppwebzot.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3yhlyvjuo.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3fcjqpbug.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3udihodkm.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3seazegmc.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3ppfmbvbv.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3wjxbxyxc.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3lkuoyolz.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3glmrytqn.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3divimmai.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3rtecwvsb.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3dggezgpv.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3flkppfzr.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3smjlmgwq.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3ooimjtdv.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3yxkzjata.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3ksfqpjrm.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3cxcjwjno.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3oimzinet.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3ctnpgheh.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3kxriuklc.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3rxdapwvd.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3kkmweodh.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3zciblzjw.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3txtiaaho.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3ychludho.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3qofkhtqp.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3bhuheyar.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3bknplkaq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fcijedtw.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3fkdkjzbi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mdhqkqrf.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3szelfnkv.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3vklsdmzl.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3kasezzfm.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3lcgciqph.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3zsmsflzj.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3wwnepbfa.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3gsecjyid.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3gamxwfzo.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3kwpxjuwu.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3tvkoqswp.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3hsdgvxvk.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3akckhklm.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3xboxrgrx.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3kqxxkfvq.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3vjtzvanq.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3ybrwinnz.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3kpmvxafp.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3spcsmrgk.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3hyixbrcz.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3eknhgnzr.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3sipysbhm.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3cqrazrbz.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3txjikgaf.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nyyswiid.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3temasgbc.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kwttqdpz.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3jpcfmlqn.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3kxzqhuvs.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3ueaupkio.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3rlrrlolo.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3saqdszlu.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3tuhhokmw.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3clznmrap.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3yrdevixg.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3pgoxrdtk.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3mzxdkqzl.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3yfqgbxpl.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3tozsdyfx.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3iheaonkr.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3zlmdmrrb.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3gpgjhhec.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3zyaohcdy.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3vzeuqlwb.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3uzauqtff.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3jxtfwsud.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3kromrejl.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3ukqffibb.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3mspxaazx.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3sygpneru.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3hhdcnsqw.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3tqbornwd.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3leokhhdh.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3hbihnlav.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3zuscaoze.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3phjdfkon.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3ynyfhtds.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3elxvdsto.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3winvahup.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3jwgntgre.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3ssuzywvb.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tcbffxgz.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3mpvnrzqg.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3oxdgnrsg.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3cxukxqsn.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3zqawyzde.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3zedhktid.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3bvtvtdtn.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3tmmbaztl.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3xuuqmwpo.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3mgbjgqrk.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3xczjsuaq.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3lxleqzkx.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3hebgelmb.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3fpldqpet.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3woxwsuxq.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3naqqrxnl.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3myellyuk.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3xwafnowm.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3zkbpfldh.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3nfnefjig.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3fowupahl.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3jhvhdbgz.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3amytkxkp.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3byfmbwbn.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3hmhhqgki.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3kppsfadc.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3vazyeogl.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yxuvbbvi.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3hcdtjkav.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3hhlqsrbh.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3erktsriv.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3sczjrrmg.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3zxrrhktb.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3mpchjbhl.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3bcpxfxnh.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3fpehhdsg.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3tlnidjmg.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wkumqdly.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3fhqfhhsy.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3xqamkecu.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3dqpkmmhf.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ieqjjpnb.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3tsiblktu.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3jliubmjh.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3vqlznnqn.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3nlxlcnab.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3ucfuccvm.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3tmcqxmlp.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3hhfvtycz.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3vbibyvqb.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3pflxwmzr.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3gubznqjl.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3jdndbgoh.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3facdwfog.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3dpuudpwn.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3phqbeoei.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3jktbnwed.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3axgpqnfn.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3yqkuztui.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3tllomwkl.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3zlhybsgw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3htcseogx.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3wvdqoxkm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jnqfkncu.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3elwtsqis.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3uaartxac.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3nncakyql.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3pteyvqcq.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3okdrcwrp.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3gloypzqb.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3riqkuuua.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3uxgnpnxg.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3uuxopywq.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ordiwumu.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3hvctvsxs.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3nslkeevx.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3xixaiapq.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3acpetcjv.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3dedsboiz.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3rdixyhln.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3wgtskdtf.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3bpjlswjl.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3urmygdir.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3dpsjtbns.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3qyoztysm.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3edytmtsy.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3rjoqxvod.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3niduzyoz.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3ixfjphrd.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3jfcpimor.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3brpglinl.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3oaahdxre.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3vsvjwwtv.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3zesjxqxf.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3xniaxfle.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3zkbmxclr.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3xeagnexk.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3jbpnxeir.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3rxcexfce.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3ateuxsil.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3vplmghgx.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3mbceyvrj.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3whqpfaqj.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3wzzejwlw.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3sdxwifrb.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3uhhbqcst.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3zlugguvi.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3ccqigewl.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3harkjorn.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3wblgbycg.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3zkvpnbvc.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3symchwio.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3tewvufha.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3enxuvxuz.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3mdlddkzj.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3gxhveqgq.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3qqzjwjgz.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3wbnoewyp.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3pjisjcyj.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3drlrobbs.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3fxnndvfj.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3cplpcmdy.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3ubgbdggi.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3xurmcdck.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3kazfqxnj.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3upqbizfs.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3auraeijv.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3nvwomzfj.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3lfyuvnfi.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3teklevgc.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3jpyuoqjo.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3dpffsiwz.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3nftldvzb.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3vvvjatys.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3fdjztqqr.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3jcicgrfg.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3nsmttnhh.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3xgopkknn.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3tnzpbypb.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3alfebbwk.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3dsubjgyy.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3kkdxfywx.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3klgsdmpk.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3wdxiwbeb.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3vqdgucal.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3kcfgpazy.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3vsvkpoqp.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3uvhfnfim.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3xqwbrhcl.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3wkaqiwvm.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3wuevsnyd.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3dsrqksjw.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3qvbblzca.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pskmhmor.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3kyuhsuvn.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3tdsicens.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3wlbwinkb.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3ifqsqlbv.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3jmwbmvxl.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jtwdlilu.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3wqjcoous.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3sskwoqkm.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3uhynyqut.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jfcragnv.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3nfyupham.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3vzvgsomd.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3sntjfjwd.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3terrejha.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3xikixlwu.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3lzpjgmqo.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3asdbersq.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3vlxvnnwl.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3zcwzxmxe.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3flqyidzn.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3vskxbqlz.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3sehggowq.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3demeohiz.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3kdidmzcg.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3jfqitoik.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3kgriuiji.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3mwwcldbu.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3beliqqfh.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3ditnojuv.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3nyzxyxuy.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3ofjrmnqt.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3berwoafo.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3fojyalrm.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3cboezfxo.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3wanllcyw.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3tqbztnvl.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3hlinpmur.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3zlawcegv.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3gizqpfzu.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3phzkvtqd.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3muicjsdo.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3jgcfcqfi.html


<!-- 参考信息 -->