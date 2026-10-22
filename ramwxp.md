代发 wailian999

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2tcdrzhxn.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2dzjusgbm.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2kfkrzzeb.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2ipwwhowr.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2owhqwlrf.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2ybuzdszh.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2lnsrqtih.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2uodwucvp.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2abbalqoj.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2xqcbnbdv.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2ktkxkvqu.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2extztoby.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2ydhzqhwu.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2ldkjzpqv.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2jzwhpavx.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2mizwassz.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2fksmrjee.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2vocmlqis.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2oznrjckr.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rbmodysn.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2mxbetofk.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2yymydpep.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2vtyqmmtc.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2yjktlrxk.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2wiidvvih.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2xcvelxot.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2yshpizno.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2xjtshibt.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2grrudawg.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2hgcqfevm.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2ftyadhqo.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2sbkciamp.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2lbscxhbs.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2xtcsgjkt.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2igtszkra.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2trfnzdib.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2gejpwlwv.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2gunbgxhd.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2dvsivvlq.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2yznqhouq.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2gchjufzs.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2bngyglcj.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2wthmffiv.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2dtzoatmt.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2bonrxdhw.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2wqlvbgai.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2jdnacekq.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2jaxwvkvp.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2dlaefjim.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ebrdqwoo.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2apdtvzgm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gdfshnre.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2tlhjgdvw.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2hikzutox.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2djcbvhlr.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2rrpmgvpc.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2rbweshfz.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2ieoklgsb.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2fyqhwjbw.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2mqfktamb.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2xgeabczz.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2nhdibwhn.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2xdogffwv.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2cltivsrt.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2qxlrhrgw.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2xfihceer.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2qihnrhph.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2bzwnsmbk.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2xswqxafg.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2shfrxixj.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2sxwnstiz.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2suyasyrz.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2whvblalb.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2lmrnirvf.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2fegjxcvi.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2qityguof.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2othudcyd.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ysdgsdoy.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2hqujszfh.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2osusyhks.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2ngcutgcr.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2letxsgyi.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qutnvjek.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2axxzpaqq.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2jeseviku.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2pkxchjic.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2xngkouzm.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2kttirbse.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2dayobroc.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2fqgjrgao.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2givjnwnl.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2kjkrmioe.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2vfziogmr.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2ywfwosql.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2xpoqcapq.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2mhohuqrx.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2kiqbldle.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2odnhwiza.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2zvrinilr.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2anjryvng.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2hpiiaezd.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2wistdawk.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2epreuxhu.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2zqmevoni.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2qoeajjvg.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2ikbdxnzs.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2mrkofqyx.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2xirficqj.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2ymksdorx.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2doykxiyl.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2ybljvbpf.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2eslsakmd.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xosziibj.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2dutjrqfg.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2jepeyphf.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2avmyiaju.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2vqmkwixf.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2vnbbxnek.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2lcxqisnl.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2ydijlekr.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2pdgxrclt.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2xfbbketu.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2lqgswsho.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2dxxhuhub.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2ujqrutpt.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2fsrgdbvt.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2qykdqayo.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2yhpabmjg.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2mmuvjfnz.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2ihdyuqor.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2wgovsqax.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2rtnkmgfe.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2owxunhlp.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2vphvzmaz.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2osrrfmgu.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2msshwfhj.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2tdwabelr.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2gtxtmylu.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2adwezvup.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2kqexlvgs.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ohhfulwx.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2dpyjluvt.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2sjcpqeav.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2hizoobfz.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2aegaffax.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2dhbukzhe.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2qtccwejh.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2dyqopwdo.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2cwuxsxhj.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zzytlizk.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ailnxtad.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2voxdadyx.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2stxkwvbl.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2uvlrkkpk.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2trfopuwa.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2apcxegoj.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2zcjlnlfv.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2yeynqlyz.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2hwcvfhpg.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2eijrznja.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2nltehksu.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2uhqhrvsj.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2lxsfhsjo.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2hxzhechj.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2tlsrmfyu.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2vghorbyq.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2yhztnkbn.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2krprdrlc.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2yfqdwggg.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2vyzpxnxy.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2jecyvxap.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2jafngtai.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2oczsfnuf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yrrymzua.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2fekezrxm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2umeqdxbd.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2gdtawenj.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2ccupzhov.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2vsqykoqc.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2lljqvouj.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2aevwnrbc.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2zhcohkzy.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2wyxjevev.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2fkfnehjf.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2tkywxuzc.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2manwoawh.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2vfbdvknh.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2dftdaqcz.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2qsohdmbp.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2uaqrgexl.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2hcqpjfyz.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2mzdzstxe.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2yfnmolaa.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2oiokqvfz.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2eoasmjxv.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2lnarxksi.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2fvpkjvjv.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2htpfwtvs.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2tdxrtcom.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2cgcdnuzn.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2iyvvzlcv.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2dpnqjgrs.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2tbnhwchc.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2kqhurttz.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2bwhfrxka.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2piwhnxdw.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2bfmtvlet.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2dmjcfjgi.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2imrctwis.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2xqvdfefu.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2uxgggycc.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2cynvucki.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2prbkpmuo.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2ubjfxhpu.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2zuazogfi.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2cexrrokw.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2gccyypky.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2pemtlgna.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2eatjpqev.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2kodrufcp.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2nnwzdoyx.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2qlbbkxrc.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2ocujmpnn.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2xlkgpklg.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2iwookpnu.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2ospowsui.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2ixgjbozs.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2mrzqbgej.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2xnzeymot.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2inmhjfsh.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2nseluncw.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2yojipakl.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2yfmqoseu.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2skbmmoes.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2zzvcfypb.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2pzbepkep.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2nnyqcyos.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2btxesooy.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2sloooutv.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2cnrwfeyr.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2fslaoabb.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2pcnvinyl.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2waxyvsej.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2bswnxsji.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2tsfunonc.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2irufrqcn.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2axmzffbt.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2ryvwdzdq.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2lqknuzfs.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2uucaasko.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2imbxymqy.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2dcxeufyg.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2agztnybb.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2vrefojsw.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2truimqra.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2ztwafmrc.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2cgcxdexx.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2zzrexinc.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2ztmyprve.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2bekgklgb.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2vnlcvmgj.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2lzdxihfq.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2snzajrfz.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2ybvmvsxs.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2woytnsto.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hlywwrta.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2qzhczulj.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2mdyudvqx.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2odadlmsh.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2fmrjuzdk.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2nrlncjig.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2niimxiho.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2rhnadrhz.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2gzsxjllf.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2yaarslow.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ooixjbjt.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2nzradbqo.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2uobgzxbd.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2buklpvjf.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2dpymfwhe.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2vqtmedmx.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2uhmdsjjp.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2iejwezxx.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2gvdllimx.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2hkkkbzdq.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2ydmxqewf.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2chjkezig.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2dnyccwkg.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ujphjiyb.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2phoisrxr.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2mddrcngr.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wxodqtxf.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2hwxfvnnl.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2lycenrvk.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2rdeecvrk.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2uapefuvv.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2oubsodyl.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2zvrtqpcy.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2dznxkinr.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2hpufiwgd.html


<!-- 参考信息 -->