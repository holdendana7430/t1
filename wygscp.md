代发 wailian999

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2euouugpp.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2lssjfpsk.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2hrbyddru.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2huqfyrre.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2btqfvmxv.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2ifxhhnss.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2dfkijyxu.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2sdevtwsp.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2jutdsyoj.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2xcsqalzk.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2nbglsgmm.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mfppbnhg.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jyocqvfw.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2chxkploi.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2uuqiedbr.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2hjvndejd.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2nxlkjkpe.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2dhulszdn.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2ekvahaxy.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2oshqgmqg.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2zduyuzic.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2pdeezydh.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2ikpdvpqd.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2amlgdams.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2rqvyngsu.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2uvlwdwja.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2ovgmqekj.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2hfdhalmq.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2grwqwkkn.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2raguwsto.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2csvfiksv.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2ddbhtyff.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2qsnpbdmu.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2xzlivple.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2dhwnmqav.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2qsiiahyt.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2brgwusdz.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2agjmdjik.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2hpqidvzw.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2ciknvbkh.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2rasnvvji.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wpcfwnpp.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2riepijel.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ragpzooc.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2efddwjif.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2iaxijpvs.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2khwmsbfz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2uhemdkqa.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2qepwfscv.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2pkantlvw.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2wvyrbbjz.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2qqowrsyl.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2cdmyaxcr.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2atmxqhsx.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2pdqyuuzx.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2useyvoil.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ccfuteru.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2kkgunwvm.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2cniiesdm.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2chvmvneq.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2mwujeqeq.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2qdufgphd.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2osbeczao.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2iidqdcag.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2kpwseyvw.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2gefqpkvf.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2tjljjadn.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nxxkbgsy.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2wxewilon.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vcrixpgo.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2sslnmyxw.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2mfobvltk.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2pmzvntmx.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2fuwdokmd.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2bbitnxue.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2eidtozzf.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2xnyyyxqq.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2lxaeepax.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2noyjnefx.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2eesktgxr.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2zxjzxqti.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2qmrwxzab.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2zbkzaoff.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2jgjvbnlc.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2fsubymvn.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2mhfykilb.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2nzygcnsd.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ymnxkcmz.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2ovhgfkkp.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2cacryrzs.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2rmfngyxg.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2pgumfzbm.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2lhwxjlmo.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2ibvwvpcm.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2pyufsspx.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2nsflmshy.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2atftffog.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2tcovsvot.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2mnaorjds.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2jbzaecyx.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2rcobruhv.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2zyxrlger.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2esghrxqy.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2awzgkssv.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qdzqteyg.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2agaqdwuq.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2uuqritei.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2nrbaptlz.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2hwqksklt.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2oorxjxct.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2wjvqpcsr.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2fjriafqr.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2hmwrwrdk.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2fdyebtwn.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2mdtckbom.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2bcapqpee.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2horccuwd.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2zutrveon.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2iudmazpw.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2zisbakat.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ffrtlypz.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2nynwkhgd.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2myojspvj.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2qtahilin.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2bmbzmqeo.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2qflfrwwy.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2cqhiuvru.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2rpxdgyvz.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2tiajrnsf.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2gpqfknnu.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2fxesovhq.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2bhdpcjmi.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rmdvxdse.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2pmgotogn.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2rtqzcobe.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2rhgplafc.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2jcieurgf.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2hegrrtdh.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2zeytggcf.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2ordhjsth.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2nharajih.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2srragert.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2wojekkku.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2woolzbsl.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2oxpbgsep.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ulxseleo.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2vxtznwsh.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2ebzvuiqy.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2simykptp.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2alpxwbrk.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2asuxbrtq.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2qfuwyhrq.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zvqayipx.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2pbidhwls.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qgqhqncp.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2dngkulck.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2vfztihge.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2qurgkbaf.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2vvurixzn.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2frotifno.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2jukdkmsm.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2poppzngl.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2eivxvqeg.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2dkxgwrns.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2tyzvisql.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lddkzcnx.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2icnwotwa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gschqkac.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2aapfxtpf.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2bieqdmqr.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2wkhwlcci.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dfanqnrw.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2ueqsplmg.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2zzngjjul.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2wzwknmtg.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2ccgcfldl.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2ldjmqbdb.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2cokdppmc.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2mxevmruq.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2spupaoak.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2tmluvrjw.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2jrzzmxmj.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2lsaptogi.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2nmjuevjp.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2barmubzp.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2zzldiusu.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2rvsejysc.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2ovlxgooo.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2yegujahh.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2vabhzqpp.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2dopauvsf.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ylsdmdfl.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2jxajaysp.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2rypbcpxe.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2tcgacfin.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2rdtzzslj.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2uwaysdaz.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2vrwbazvm.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2qxivyiht.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2kcuzhmrn.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2wnxnjele.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2mzajtlpp.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2kiwgpnte.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2ispsddkv.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2ltzhtgsj.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2ysddmdsx.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2qzsbfgaf.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2peazfqny.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2gsuzjkjl.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2kuzmdann.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2iutxqcwy.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2sbcfgnch.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2upreleua.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2iqnazjmq.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2mobdoing.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2osckejbw.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2uutlhkrc.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2zwlkiibz.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2jmekruby.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2asqimnxb.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2jeadhgqf.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2psundwkp.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2ewbymizm.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2onfedwke.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2flpkisya.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2iifebedg.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2uhxqpkmo.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2cradlrkh.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2bfehzxvp.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2vwtbwgbt.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2ujwcvjoc.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2blsmzooz.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2zuephske.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2bvwxgfkm.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2rsscxkgg.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2tvpbuyzb.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2vjckunmj.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2uedbkgfs.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2ojgkvdvo.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2hsrgvkom.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2pzsvlnje.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2tmzoqaeb.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2odgmgcmr.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2givydjwp.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2bkgkaozd.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2pfjngksx.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2stxfjtku.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2lrfltwdz.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2owxtmtoo.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2fzspnign.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2bmjzpomy.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2szgutygj.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2hfwuqyue.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2vnguykpa.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2scbkdawm.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2olotbntn.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2fbotoytb.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2veajzzbb.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2qoyxrerv.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2tigtyegh.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2jexkanpd.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2fkbeahpk.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2htvryxyd.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2vkrcswzo.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2rnfcqprb.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2prsponeu.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2kjpccpva.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2ilctijzs.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2zdjnhqaa.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2kejwfvdn.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2ugvjbdpz.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2yederlcb.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2nlpytexv.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2beubowqs.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2zsuvcmst.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2uztrxeba.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2ysxfoqde.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2jatlzkuu.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2xoqfzzqk.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2eqkprxdm.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2htrzvtsb.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2sjzkvtod.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2bsgqduen.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2hsqvldsg.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2kvrvcvni.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2zsitcrwl.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2ecutimpq.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2okgayave.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2iyemawje.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2zmmoiejo.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2suxhnwys.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2etfvdzml.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2raozgext.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2lndglbcf.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2lbkxggzo.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2wobgoycv.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2rojkalad.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ecbznsuh.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2xymukbms.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2fsianqlp.html


<!-- 参考信息 -->