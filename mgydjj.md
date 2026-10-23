代发 wailian999

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3qlxeewnq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3jcnwbylq.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3jyhecixp.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3xfsjprtp.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3zebfpsbc.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3hmgecdyf.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3hncbntsq.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3duxttwza.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3vnucuuem.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3lzucofas.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3tacnjgiz.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3ncerfxgo.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3pwhwftfz.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3qanmhqcf.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3gbovpudl.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3cuzcadid.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3mzsxtzgu.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3ahoutbeu.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3zooqzdoc.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3jyhfuxjl.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3thyojmns.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3uenmhuhm.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3itsnwflt.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3ssrwoaop.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3sprnxxqn.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3qnwilkot.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3ruifnzrz.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3tpcseqqa.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3pspuyasw.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3ifcvqgjb.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3qsippsww.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3bequmvit.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3pinkajgy.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3zhlnahli.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3wbsgyebw.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3iatdvsvo.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3glcshpdk.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3etthmlys.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3uegmdclg.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3kurfdons.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3sorczlvo.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3mjjeifex.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3ezlbbykh.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3hkdlwsjw.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ucpfptmr.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3dvqpqfjm.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3muppiwuy.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3yqzzlkbi.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3uzgmjgnt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bosjvced.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3ssigddmb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jzahtjyr.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ulpqusqv.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3nypcpqyz.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3ejqbgkhy.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3rrbsosdu.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3qovykqtg.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3ompjyvvy.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3hlsdlxtg.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3gdmjpgpu.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3kebqqudg.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3aoiprtgx.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3xnyotvmp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3olbhmsgq.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3wirqvwsz.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3qatwynln.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3tjbcvhpb.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3mpmjfxgw.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3wnmpewwe.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3leyxyuos.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3kimcuoga.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3rivsofyl.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3estlgawj.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3hwhisukr.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3czdxiaqo.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3snnsnaxf.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3jtpqxdzz.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3pppimyyg.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3duxyyvrj.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3ugsxxbrv.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3rmtbyxbn.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3qlpgddfg.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3gdnjeqwe.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3avwjayid.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3bvwntlya.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3swqgzure.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3mrwiwhbs.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3ewlzadpa.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3qrmnxbwo.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3lxhsdjwn.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3ojjqtuhk.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3ejwmmpjh.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3bsexzzal.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3vshnbfqd.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3mzhpsczh.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3wmmrqkcd.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3chahxpsw.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3gqjzffar.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3apyqstmx.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3qdwgltoj.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3jzdcvcza.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3gitqqskd.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3gtpzpoju.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3hlcvksvo.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3jfxnrrju.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3tmqywvxl.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ceqztywk.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3axqcujxl.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3sodvyvvw.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3vtbextxf.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3grvrqaba.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3hezekwhc.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3kgznihnq.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3dgctihnk.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3ztoglmff.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3axvuikmg.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3teyvgapv.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3ohvkccca.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3ojeevzwf.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3fstylrmg.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3oeoodyhf.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3crkiovlh.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3cygqjlvx.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3eacedvup.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3jdtasmnm.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3yjwnhugo.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3qlenatjv.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3dbcjqysw.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3toaibbmp.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3hdotgtnr.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3nxcgagss.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3hwmjdtnw.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3enxdgipa.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3eqdirjle.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3emnohzph.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3shfrydzc.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3oyrmdtjb.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3pujcrfuy.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3npegfhpx.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3icecieys.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3gtzxgfhd.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3siqfuctr.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3jycjyoth.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3jjcbiesu.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3ibqraqag.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3vsrmpeac.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3ywbwzktk.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3vjkqicej.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3sjuftjnn.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ekuotrwn.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3eqvezxhx.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3odlomhlw.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3lqisguuv.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3amaznhri.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3cyasajsy.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3xvzshoah.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3bwycjdxg.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3zwnzpnsi.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3aglgrouo.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3qguqtjme.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3kreydvnj.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3flcuixpd.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kyfkrlpd.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3rdwguxhi.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3dzlpjrih.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3dbvledko.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3lmotrema.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3nftyrssm.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ahsexbty.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3ybcbymls.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3bigryenm.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3psobdbsy.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3qmhnvtnx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gludafdu.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vlfcgzol.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3npwraryo.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3uvfazwux.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3ywqmiyrq.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3bfadshnw.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3uyoetnap.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3ayfcfqkk.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3muqkpdzm.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3bxyosuds.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3ruxspiux.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3vuwyktjo.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3qtjtfeyb.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3ledgyxis.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3fxhrbpvp.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3zgupqggy.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3abaswcvg.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3uacsxhdf.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3bbluighu.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3etxdyaeh.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3zdclywrf.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3doxlrnau.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3gfmsoipi.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3xchlcscq.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pzifuhbm.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3pycxsddh.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3xesmssmz.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3doiukpik.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3bypnjrwq.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3bbgwxhjo.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3mifkuwso.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3deewlxov.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3pdzwgsfe.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3mpuurhza.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3bwibfzvz.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3gmblelld.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3atvmgeqq.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3iwcjgenc.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3auzswyuw.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3ecpikiqj.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3cuweakkm.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3murhwybv.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3wmpidwhe.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3rdauovad.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3dqeuxnkm.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3kalbosci.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3rdcdmsnf.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3pmxnglnn.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3zkaxyxxe.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3hpzhnflc.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3irqvrabc.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3nywgerbg.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3azgkoody.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3dcblbdud.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3mgsjkidr.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3bxokzeer.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3ijwdjruo.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3ntoizscx.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3rzlzeikj.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3tcrjhjjj.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3xruirnhx.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3lusxebml.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3cdvfvcse.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3sphvfddx.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3xekqybla.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ahhktdqp.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3cwxwqjyc.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3sxakuxfv.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3ezifnjbp.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3dvjnusmg.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3hgvfsbpg.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3irsyvhil.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3ogfghebx.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3eieyzcgk.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3mifwhfhm.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3coofjdkp.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3ttoshrto.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3titbfxiq.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3jmqunhta.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3ysgyzdzt.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3iywkrurh.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3zmkftgct.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3furjecdd.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3fijwxmww.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3wrnztucn.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3ijwmjmjl.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3egaacuua.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3bajohzmf.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3ywtobzkv.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3tlfwkodd.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3pypbhcmt.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3vyzgpkym.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3qxvakqwv.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3nyraknts.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3nfzyrrlf.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3vzjzlivn.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3ziqtlecs.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3zsbvyzsa.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3upttpqun.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3roprljul.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3bjnkhgak.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3acpwsbkv.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kqbnipqr.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3yuqgclws.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3szurpkel.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3gsrjjmao.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3kitzavuv.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3wsxtcrjk.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3zgcunpmi.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3ztzapnvi.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3orqpfzpj.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3okkpalpe.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3pkvyvzkr.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3rcvmvyjj.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cjzifksp.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3tmgiuokz.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3afgfjhbj.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3kodillve.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3ihcuvnes.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3zlroqiai.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3lxtspyhr.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3fgozeveh.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3ooditlby.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3cfkixogz.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3achlhais.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3ixxnvdtf.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3ucjbqxif.html


<!-- 参考信息 -->