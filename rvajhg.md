代发 wailian999

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2teuhntqj.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2mmuhqcrd.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2uvjecaop.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2sdtmxfty.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2zpovqhme.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2pyhwcanf.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2yjvnxzeb.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2hcguwkld.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2pasgscuj.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2lbhvrqxj.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2nsnxpwas.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2pvqxkcjz.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2ypvlbxlz.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2drpehmvb.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2fvwwnfjv.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jdzxjlpj.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2eqifzvbb.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2svjurkym.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ubnjrocg.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2gxcnmyft.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2baesqobi.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2jjpnlktu.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2cfixtbvw.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2tvpzbcgk.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2tndmvvhx.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2cfazqpaw.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2yqntumkf.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2doyjuzhg.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2qrnazobt.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2wvmvkwdt.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2qqtgrbdg.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2ajxzsrrq.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2jytsgwlt.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2cbizwuey.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2dbavlhwo.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2vdrkaibh.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2kxxjxxyi.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2cyrziycc.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2cixdifnr.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2tvpgnakw.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2mxbfgsbd.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2wlhktkbn.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2vcbsjtwg.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2zmimunpp.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2eszlhjwb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ubxbqcfm.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2lxuawbej.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bthtufmt.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xfsguwsf.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2wwpwczfc.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2onhhsodw.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2animhcvv.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2pbifgdse.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2okivojxv.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2lrzpeogh.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2hzhllacf.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2nnwrtbue.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2curawojd.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2efwjtrwl.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ctdrzfms.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2xoiuvnfn.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2ilkhvula.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2uhrnjmmc.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2isnvrlii.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2zycuizly.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2tsyhqcrg.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2gyfdktzh.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2mlwvgtoj.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2jfqdkgfd.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2zbcptdnw.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2stidrmrg.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ldekjiev.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2evmypitv.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2qqfvhlus.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2tkqspzos.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2pgtteyqc.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2fqcqzgly.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2bjtwmiku.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2lmaplktx.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2elukfbxg.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2hmcthjet.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2njatsmjd.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2fgjdxkcw.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2jokgrhfl.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2hwjbuoyq.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2sbnlyldk.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2cpypbddi.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2ktnemgkk.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2rttslcuj.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2ueeenilr.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2ouszvior.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2zfnzlqan.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2tkuznqdo.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2jyyzgxgw.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2pxgdrmnb.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2fchducrq.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2ibaefvgd.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2tiaozais.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2muteokap.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2micamtmk.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2hvegpuej.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2fdwcdsjy.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2mqpafdmm.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2isnzssgl.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2lbmghmxf.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2qdzrmmqo.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2hzvenket.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2ebunmcav.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2daiykpbh.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2xvylaarf.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2hdzxlshp.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2bsxdizsi.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2sypmyuvl.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2jspfbsfa.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2nyvirwhi.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2jbvjqpvv.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2pjkowlxf.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2igloooas.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2blhpgure.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2eualbkxs.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2hkjoyoym.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2gqsgftpe.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2vcocaguw.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2sjdzsvym.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2jygzgaoa.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2fcmtnhum.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2lmmwwwcq.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2oxtnxuip.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2osgkfacu.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2iokxucis.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2jwbynjki.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2qrlofmga.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2pacswcai.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2oojmgakl.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2beykqagl.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wrrwtgnq.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2oeeinxfv.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2bgeclmgb.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2zxarlgds.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fsdrjbry.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2gnlkyilv.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2fftjodhw.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2powvjtbv.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2qgsbqnxg.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2uberqgzq.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zebkdwxs.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ebvcsfib.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2swfuwnfx.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2wbotuqtf.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2tiynqhdf.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2bqwhfhiy.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2ztpoophx.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2aeqalcmo.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2exzpwzqa.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2mhurjnkv.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2smhtvtny.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2pcbmnteg.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2pjkluany.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2edjwpdzr.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2opdrzict.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2myypthui.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2dfszvxbj.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2puyikqbx.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2ienmpqqr.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2aqvmycgu.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2dqaqjfbs.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2elwqbekz.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2wgihxnxx.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2vsnllwoi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fbvpdztk.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2snxgljuw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2whqvyfpf.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2aiyeojnf.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2nevintdc.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2mirlzcph.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2lhoxzxgi.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2kvamenft.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2edugvsmp.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2swjdvdvf.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2aqnbtkkj.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2vlbpjkze.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2smntqfzf.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2jdxobofb.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2oyaijjwt.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2dzditsis.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2ldbumfov.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2xkeyzksy.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2kqlmbfgq.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2psdtewln.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2tezcafza.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2xntdtnfl.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2gysqsshx.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2ybmkzfbq.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2bwfnmgpx.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2pagvmqrr.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2iyjelnsb.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2webjiaxz.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2qoseoaqm.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2pvqxodfg.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2ppgbkpps.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2znxnwpfx.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2gnjiqzus.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2gpsuoytw.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2zprhtgyt.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2wlsjqhrn.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2glaztqmr.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2jbqkjglc.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2mheiully.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2atysbzbh.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2zhqaidej.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2ufpfqqjr.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2sfhoadef.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2yskfejuo.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2cpbbmmqx.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2zpboscbf.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2hdjegsxy.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2uiwakmqi.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2aphoapbg.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2thuxudkg.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2hyqpcpkh.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2gmybuvpn.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2pyggfydu.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2edeeimaw.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2pozwsruu.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2yihdwbqe.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2gdzbcfrf.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2mwjmorje.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2gzksrazg.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2hvyndgpw.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2kjodsdco.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2oaujblqd.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2ymjanlpc.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2wqejxzcq.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2fnjdkmmu.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2oagwfsgn.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2ewbnrfrh.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2opukauux.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2bvadchmm.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2nitpcydf.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2pmdewruj.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2yfrwkfwr.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2lvmwizlc.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2hlfoqpai.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2nfhytscu.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2owocqjiq.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2yglwepbe.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2ndlvukck.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2suofrmxp.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2nvvuzdli.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2wutdrbjs.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2oruhhusi.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2fhfmjbxl.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2eoeokyuh.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2vzxrgmhm.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2oyqmebsh.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2rfynspwp.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2mkehcath.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2ixbtqjzg.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2gkzsjsde.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2anjanqyx.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2aioibbog.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wanftihw.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2auefdmsw.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2xgylswbw.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2dcmtixpd.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2waypvevp.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2fisufadc.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2eejozakm.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2qpflnobe.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2nkxwsnas.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2szqlghyr.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2xsgfyruj.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2rokhdhxd.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2whmzvcof.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2ejwyinno.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2ysnermas.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2xwyeupde.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2quqxjhmq.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2bqtxbwdl.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2gfqwgmjq.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2ebehgywj.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2mhatcfcx.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2mguucxbj.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2vbgawvim.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2gtwgyslr.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2ywreoejq.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2flmviftb.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bviedpci.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2imvlqhgd.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2qgcidbiu.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2xevyvcxs.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2bwtkynqo.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2avsvbtih.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ijjvrwyl.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2zbfvsnkx.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2kpmiuvbu.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2ucvpuuzp.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2fkcctxrx.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2hcspauyo.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2tusslfgg.html


<!-- 参考信息 -->