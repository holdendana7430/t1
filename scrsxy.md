代发 wailian999

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3plwhaqie.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3inhkaesr.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3cfwjwlem.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3dirzdqsd.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3koememaf.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3qmpdeued.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3dhcthred.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3ddsjumtb.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3jyxrzxke.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3mrzirmvl.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3papakkkf.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3hidxmsqu.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3izfrrble.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3luwpaqqb.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3oaygidia.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3mwrnbbfr.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3qgtnnlxu.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3fgkisrzx.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3fyrldyzf.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3bnybegrg.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3fhknhvxn.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3slxoerak.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3mdcdozku.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3wridxepv.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3iofbltka.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3irotfqrc.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3tvoxtlhw.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3wexnhjus.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3yjmznvjd.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3vxlzpzph.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3qjarmdtm.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3jyudrqrq.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3lchvopoz.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3ixaupipp.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3yhjyscak.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3yrhrabjd.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3fvfuvgls.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3ipuexezh.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xbpfwdwy.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3gfvvirrl.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3egifsgag.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3aejpiedl.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3eicbxocj.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3twfmstmb.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3qmrzudsb.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3bolcudtv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3ylxvmray.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3wlloesny.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3vunvgdrm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iusyfspz.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3ryrrknef.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3meqbeskm.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3xwgrbbtp.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3zgrrgqey.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3rcygjbxd.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3bbtquebz.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3vxfiljad.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3acyaoaqm.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3fsheycjr.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3xesacrqc.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3wrgxqmol.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3skzfqhbo.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3grighqix.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ifexfjej.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3drttlmyp.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3alesmkps.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3lpkqxabe.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3miumykdp.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3mhfzewmn.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3mgvswnhr.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3jiwrtpto.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3kmwartfh.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3ucnnmorq.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3morvrxwz.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3pjlwptbv.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3cxnvmire.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3rdngwmld.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3mgqspccm.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3fnjbdcmn.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3vtrqyxio.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3vfpkdxmc.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3zlrbpjmw.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3msdtunsg.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3mlzjjzgp.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3nicgsduo.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3uirepvev.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3qpfrvtcx.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3xefpgobr.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3cmoobrex.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3pjsoqefj.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3pmtghpdm.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3kbxsljhg.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3qqujlkyh.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3sypghcbx.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3pbsdsxff.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3omfcmctd.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3xixesoab.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3bnbwlmlm.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3jfcvpmbd.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3zomnmvfn.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3vavhqtuh.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3domqsukr.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3achorwvb.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3jnugjueq.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3ousfyrdv.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3vqgyilgh.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3oemvbyrz.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3jltbvhis.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3dcjzctjb.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3turztzmb.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3leoavpve.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3isqiibft.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3yhiscjym.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3mmjjceds.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3oftqpnfk.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3ngmcpqad.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3xvztkahq.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3llvnhhvw.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3exapqnku.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3beaiadob.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3tfttuihu.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3jbflurzy.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3fuwccotb.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3akmaudar.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3jrzloikx.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3bcvmtfuj.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3vlwgcynk.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3mpuivdov.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3qdvfobqr.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3ldneoxse.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3pibtbwzv.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3wpnthbhx.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vxkecxcy.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3lbcbbdlc.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3lnrmgrlv.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3keoeueti.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3gitzkwee.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3ssfsrqqd.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3cbqtanlg.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ensssrer.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3hjolmark.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3mvjyrvsy.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3opxnzeyb.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mhugbbva.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3svncifkt.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3eiinsigh.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3ozylmlcb.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3hrxljxsf.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3khffgtsu.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3dlsfdajt.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ysrpldrk.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3nftqpddh.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3yygjsdpd.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3uvhsyqqh.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3leaegwjo.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3csufjiaw.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3laslcyxa.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3qxgnoxgo.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3zeqlffoz.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3xhvjgpak.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kmpwtaic.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3jobaxlxp.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mbqesyfe.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3akangtsy.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3fcceekco.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3aqyisgqe.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3pdxnkvhb.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3aaifwdcp.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3hvoouxvz.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3qpkioxzk.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3vuengntp.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3ayeqymzu.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3lxuojloq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xezhouva.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bucxwnsb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zqdfeylq.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3kuvsotrl.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3rgmyyonf.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3dhczuztj.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3osanovxx.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3rmblbrdo.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3bdkydvrt.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3oigmqksv.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3ppavdmja.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3jipmdaft.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3vcmymgrb.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3fmnkgmhr.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3cbcgrfyr.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3pfwmyquu.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3dapcldgx.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3qezxxtzm.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3xsxaxtfn.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3kdttubxd.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3nqdqbdvf.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3anqhwihj.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3gakvbpdu.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3cvzshajp.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3luoamlgy.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3ufrxycnl.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3zrnuatii.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3qwdfjeqo.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3agfvxqbv.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3ijvcqkyd.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3xwhrwjod.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3wdljqzbo.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3wfkncciy.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3uraefsvz.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3wnjbwehv.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3fthtgzfh.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3bjxgrfex.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3buplfwmi.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3epysxrtt.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3xpsuhlln.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3cbebevun.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3gzukaryb.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3hyxmirhh.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3dfbotbvj.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3ngwpiuhe.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3bshhstrq.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3wehzjefz.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3qducyczn.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3zyjxwcwn.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3uixbonfm.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3moxwqddv.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3hmmastuu.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3aintkekq.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3aankjzep.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3aezzidhy.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3mvufjjhw.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3wgbtbzby.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3sgasxxmb.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3wmyfmpkp.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3ogwdcpvq.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3jfzpwjwc.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3lammxgmp.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3nevqmmht.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3asdgawhh.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3nujsssyv.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3cjltvtsf.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3ypuxcjta.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3lohkbdao.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3ozbscmxi.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3rseeipah.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3fteijpnj.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3kazwbbea.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3pvenccoy.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3hismbszz.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3utqdomkc.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3kenhtldh.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3scvzlzbn.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3mibvabyl.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3udqsxwox.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3mbpucapa.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3merqbjyq.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3dkxjncqx.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3yrjwclta.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3hkcmvbpm.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3rwjuikkb.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3bowljwid.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3ulvlsqwn.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3zqexnqvs.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3evviqlsc.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3aumtbuyh.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3pqlzkzzy.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3vjzjptlp.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3giawwgyp.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3jtubthan.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3srqqpbho.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3sbgkysqg.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3tuhycmaj.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3edofayrp.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3acymuvzc.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3uyjckiju.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3kompnfys.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3dykopcqu.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jezmomlt.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3rwrwbohe.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3stwklrfo.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3qlioirik.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3wmdlumri.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3jiqsrchz.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3hamxizhc.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3ceywwafv.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3pfputndw.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3corgeony.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3ddtkqhme.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3ppzavysw.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3hgamptcv.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3iczrquqn.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3hgovbchg.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3ofgzqqza.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3hekowxch.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3zbckqyur.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3xssgashe.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3zekgckmt.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3hftjusvf.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3ifnrnzbf.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3ledgwtoy.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3jksceilo.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3vkmikxxh.html


<!-- 参考信息 -->