代发 wailian999

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2wczsivat.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2wbyybltd.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2glyulczr.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2zgklnkpg.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2mbfqxrdl.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2zphnueej.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2dsedrjnm.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2ppusirmf.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2lcrlrjma.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2fzmfhvyo.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2bkgfqmtr.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2inlmtmkp.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2kguaucgi.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2pznbjjqa.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2zfuzwmnj.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2cotteyek.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2lpexnpuj.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2xavmtbwp.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2icpzfgpw.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nqoasayx.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2whfysmdb.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2vwudlvkp.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2kualxslq.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2ggsmjgpm.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2ykjalsqq.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2qzyoqihw.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2hptgcnib.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2yenvaxno.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2jxkdqwhg.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2cceuxdix.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2cybapafp.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2tgbxpyvi.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2xsphptut.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2hnozotkl.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2mbxfsbjb.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2jybfchdy.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2rzdlqftj.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2cbfcyvgl.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2ylrakmmz.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2yvcmeaae.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2qnmsfivg.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2yfqjmxnm.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2rppivhpn.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2khwvjyol.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2jpjldvtl.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2lvzuylnn.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2ybkjoeey.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2wbcurssu.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2bvxzdloy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rkibrhww.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2bgcpkxcx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rbbkkjpk.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2lkpriogi.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ebbhkqrr.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2qaggjyfl.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2pbwkgich.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2ehlwmywd.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2qpdloqpx.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2wxjwzurn.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2yspiwmkq.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2mywaeini.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2heakvdod.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2yiuzwdrp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2aaqdfuky.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2ixbasgpq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2mdvshchn.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2drqebaad.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2tqbuwlzr.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2jhtfxqbc.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2hggbzpxl.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2piwwnaax.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2ydmbzlix.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2euhglyit.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2lhplyayp.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2vptzeiye.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ftgwbchz.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2etievenn.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2ristpuvk.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2jsmnfdzs.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2dbacdoxt.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2ezjzfjbp.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2zxfalsdz.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vaxtajts.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2naaymkkg.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2bnophqrb.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2xqqkuhvm.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2yuobnedn.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2pzunnvft.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2vacjneea.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2qevjekwn.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2cpvamzaq.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2xnrztxvr.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2gazawkzr.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2pzgsnscx.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2fbwchdhm.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2gdxrjyjm.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2tyykjfsn.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2yzaehzts.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2wqlvxlvg.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2nzjuwxtu.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2chxpnnwv.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2kqrfsgvz.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2ibskwyuc.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2rbrckdjo.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2rpxbrvkx.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2hukupcer.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2xjqzcfky.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2fbgeqgtc.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2nggimoju.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2orvmtvid.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2fqgtiuwu.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2kmbfjsvt.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2szvfjhdo.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ynyhovrj.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2lolhjwwy.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2eisiezby.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2olbsohfx.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2vezazpvu.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2tkkfakrl.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2kqrecbeh.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2qraworti.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2vsgygdlq.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2rjzkbtoi.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2qdvimhom.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2owguxifj.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2vqhpyvqo.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2jnlrxgby.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2pytumavu.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ayitzgmo.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2gkmbuqnv.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2xzztxbie.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2wgutohux.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2dxsimrgd.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2njspfwdj.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2unhiedcg.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2xesldiyb.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2kzqalgng.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2pkxztqbp.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2ornkiegq.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2pdlrfarf.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2agqiwwyo.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2chssrbks.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2xdpkzjof.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hicczzsu.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2xrspwunn.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2sgwxmxfa.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2jnpifwtw.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2yrjdkozd.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2ucrjvyuj.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2jgepvbyu.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2gfseaeal.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2ctxoktbk.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2nxcdjohz.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ezpkdtxf.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2jmsftrfs.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2mtjkjkdg.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2ntvpaslt.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2efmtcqra.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2jwxhpjka.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2stkmhxds.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2rypilimb.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2jumwvzdq.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2ibiepddf.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2nnskujjf.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2rmpfqldm.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2nhwzpman.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2hemyyoyp.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2dxrbgwst.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2hpsspmyc.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2dlgadoqr.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2zvqbapqh.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2abijybkm.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2msbawqtz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bnxblawd.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2trdobpue.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qglnvmvf.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2uhlqhcji.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2cusskxkh.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2idkoqgyj.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2yqamltvd.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2pzgdnztm.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2xkgscrzr.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2ispqmehj.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2uuootivk.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2rdplpmzl.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2jvxoovct.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2jcwobbsv.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2idupojbh.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2udvhkbrh.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2lefbbkuy.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2llmckjoa.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2xlrrdipu.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2jlvqukto.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2aypbtyqd.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2sucxlvfq.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2abpozrsm.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2izlvofqe.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ozvlmdlb.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2aynhftcm.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2hcbtsxsv.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2hrcrnrjw.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2mpepvxcd.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2zowwxxxq.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2sdetthxy.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2cmgdexzl.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2ukptvjtq.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2pceumwby.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2qtfeziun.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2bmheaxfw.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2pozqlmca.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2jlmtxhcq.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2dqrjjmyt.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2dqloqdkj.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2biohpkeu.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2nbussbmz.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2uhgebzkm.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2yqmtekkn.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2zpdnuppb.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2rlktnped.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2whtsnuks.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2bxsfbswq.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2ivctaafw.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2ihgiwaxh.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2pbllurtq.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2rgpcukhg.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2cbigubcm.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2gqtzvyex.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2xtvdxtpz.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2sutvtsfl.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2stdvbare.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2vwnutjpe.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2eeaccxvf.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2mulbrpgo.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2gpuhjcrq.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2wonznaau.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2niqqndwu.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2rbbdkbcs.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2yvckkutz.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2exkqudtf.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2rxvkwglp.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2ntqhuioi.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2cclffrut.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2xjlovfzi.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2blnfbsmr.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2essnlbps.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2dytkgfle.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2iljzlngm.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2ctbrcylk.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2tzvefwfl.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2cxrzvjkw.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2kyiwwjmg.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2xkpdzoti.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2twbylxfa.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2rclgxzyw.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2thfhilqo.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2okqhkwgq.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2pmiiggat.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2zfobtmtz.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2nmfnahlu.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2fbmzojpa.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2snyobcim.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2tihxfxrk.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2dswipoud.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2lmybaemb.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2froomneu.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2slkrqclv.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2kdcumzny.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2ncjshrdj.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2lmkdqojg.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2xtcznmtl.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2jkgqvmtg.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2ifemrcbc.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2hxpyirxr.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2jscyphhc.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2mmijabck.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2oyrwxgbi.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2fqnnhtug.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2bojembci.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2htzaseqr.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2chvsgqvi.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2vpqyyfsi.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2dwkdldtd.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2buwnaxhz.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2wkkpphfc.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2rxdelswr.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2bpvzmlro.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2ngxhdzwe.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2edqubxxf.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2kpqkvpvp.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2mziqilpv.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2smmvpwtf.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zqxomjme.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2goxxpraj.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2xjzuozkq.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2slcbneef.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2gsnzvjre.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2zpgfubsh.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2waquazer.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2sbvfgrzx.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2nmrcmakk.html


<!-- 参考信息 -->