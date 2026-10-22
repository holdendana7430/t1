代发 wailian999

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2osoivpqz.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2djoohsij.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2bgxgntnj.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rxloihoz.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2wzhhqprh.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2vnxcthnr.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2jtejtgld.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2gvsfvecf.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2nseuxlsb.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2ayhutujy.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2cbairuyj.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2dezicmyv.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2qwevbflk.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2nxlmnmnt.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2wkthtnpl.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2jhdobirt.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ccfkfcvn.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2fnihotrl.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2wxpotytd.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2rvnqieet.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2ibannpdy.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2tpygvmjw.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2rbmumzqp.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2qpfhkmkg.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2terdjjsa.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2sttylqze.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2ccrqbdln.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2opvbplsh.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2rgjryklf.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2uslyywdx.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2nbrucrof.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2cjuhxgtt.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2rngjdpvt.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2tztljjla.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2akhrpmag.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2oanpjzem.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2intfhxsy.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2pkumyboo.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2qtdcvxad.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2lngpbtbg.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2poipidwv.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2tfjuillh.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2bqjovxwl.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2qwmlryqf.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2jwffrobl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kvcyibuq.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2kecilrwg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2reldpowf.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2edkduvrp.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2lywgjsnh.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2raikepxx.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2uxcyirgw.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2fcbuhsfz.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2enbivwxl.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2puqdrhnl.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2wuhrdujr.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2cvuxlrgo.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2ukhkthrm.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2wwlparza.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2lepwhljf.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ybyvalrx.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2fannabxd.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2wrfjztnf.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2ilzvewhg.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2yohkrxbi.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2kkyfvtna.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2tnapekwu.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2hfztxnaf.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2qiqmcgeo.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2yglitirh.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2ctzdeifz.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2sxddgfqb.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2xyoqvmih.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2nhiowbqa.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2vomaaucf.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ijkgsvan.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2qypsvjvs.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2gruxzkwq.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xbjklceb.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2rrurnded.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2xpgbffcf.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2vextzivz.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ucyjtite.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2bomeecmw.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2ymugdrpe.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2jskvuuyf.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2iwuyqoct.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2xjasrucg.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2mucujwdd.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2udhodrlk.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2qlwydwce.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2njpxyiuy.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2imjcenzt.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2omrxbubp.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2eqslgecf.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2gmjhtuzg.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2dvhpibzh.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2wguvcxzb.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2myyqkhvb.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2bhibocdk.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2eqszprcp.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2ewdpttqt.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2fzvhukvi.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2demnwbpu.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2kkigsdsq.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2mufjtout.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2lnvuqjdp.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2wwohurll.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2eddgbgue.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2nxvdwwqk.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2borqbrtr.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2fcbnxsom.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2nyinktpu.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2dfgfzhfv.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2hinvtgcz.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2rcyyhpyc.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2umixnmtz.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2efkehvth.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2hidrrdlq.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2jftqavuy.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2wyokpexg.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2fmznlmnk.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2znuqdval.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2zzponizt.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2ukntophh.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2yfzrpvww.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2issedpbc.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2hstkvrum.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2nbipxikw.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2orcjheis.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2einlquyx.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2osoklzjt.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2mxechunh.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2xskzopjr.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2ushwmffd.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2wnjzlvxd.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2focfokrj.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2bttblbux.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2awibuihk.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2vqqnsejd.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2asflcqyk.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2osemgfvz.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2xvvwboal.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2zkhlgioo.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2tjdnjyqo.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2gqtzvany.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2hqpatuyf.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2ogvqisvc.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2xnqqnhyi.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vdhuubzh.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2yszchgyr.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2xnnqvcxc.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2webprzad.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2nploqoxq.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2rqnbgkpb.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2kenkteyb.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2owtwxlxv.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2egkkqybg.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zpszoien.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2dkcbutwo.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2adjkmrbr.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2byidozyp.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2xdwfnjcs.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2gkrrbqzj.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2qeqkylqr.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2kgusuysw.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2bneyleqz.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2tskykwmc.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2xidredty.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2icxmuhte.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2wxcepnxe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yhlmlwnw.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2dlngonjk.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2pkjhpkmy.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2brmrwiqw.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2ouwvsxdp.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2wupflvcu.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2xymzckmc.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2okrmpkgv.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2lhmslfjv.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2ahhtgkhh.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2iuigmmsy.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2hyogxuda.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2izqtcqgc.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2uhhvxwxg.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2qzojwysq.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2jqqomlhy.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2yoaqalvw.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2bkbdxdet.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2khxijfyz.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2bjtwgneg.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2lmvtarek.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2zxjmmuyy.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2agtxlnut.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2wxomayiq.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2mmuezbnf.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2bimembsm.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2unjbafau.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2rbypaqkb.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2qcjxdfod.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2hchbxbtm.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2zzdzrdeq.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2chrwyblc.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2unefrazx.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2hbtsbtyz.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2ukrhbzuv.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2ssfqvcur.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2jwwvuqkp.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2xvxvfoak.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2vtazatfl.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2ilwufpmy.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2tyftqjpi.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2qwbopqqh.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2jgmkrvyo.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2ltwtbsrl.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2jmjtflmk.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2zvqiovii.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2beuyianj.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2xihivhne.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2knattbmk.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2kmlushcf.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2hycjggwc.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2jntstaqb.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2hbvmoeyb.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2jxqibxub.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2khulckke.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2lmyovfwz.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2pfvnghmy.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2zhxyjnrp.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2doxyrkhm.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2iryodlvk.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ikjqgvkp.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2dytfscgo.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2kvozjexq.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2atrgzufn.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2vncmbjvq.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2ctgunldd.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2nxlooqlu.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2ftbbfpbu.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2snpdlyfu.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2loqkheka.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2vxivxyui.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2tentqrbn.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2ojozvxoh.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2qyzvivpy.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2xtdjfktf.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2xstnwdqc.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2ksagnmlz.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2qdzesgoa.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2lonxbotz.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2czufgohk.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2tvpqzxpb.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2zqxqqpfx.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2kyxvaofz.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2nznlxoqy.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2jhmupxix.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2dhxkfwtg.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2oojpwgzy.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2ktpgcbni.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2uavtfycu.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2wiuopleo.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2xekiyblm.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2xcjugtfh.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2behxbhex.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2wkzlnvzm.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2katimkdh.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2wbyzqtpx.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cpynjxsw.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2kjneaxrl.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2lhertgez.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2ludplzvt.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2nspiyxba.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2krwqkplt.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2nlfrbczu.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2zlhjqcfc.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2yxrniout.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2xefqwuyj.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2inkkojsr.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2vvgjsnrw.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2xfitnebb.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2srgevpal.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2zhseuwgk.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2vmrxlvrl.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2yrijhcav.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2jqgjzzki.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2mxqzokqx.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2ojtlqanv.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2aaxbzebz.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2juzyvjek.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2onlvztbh.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2dllihxcy.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2rpbbsqgp.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2qwjqsbol.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vdtugxft.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2wdfvrtbr.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2ellolsgv.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2nbdgddnj.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2pvsaeqoz.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2zendvdzy.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2bapffmtj.html


<!-- 参考信息 -->