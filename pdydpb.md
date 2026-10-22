代发 wailian999

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2eqtmgmws.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2gbycloua.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2cxrgxngm.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2wirqssnn.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2tbhqweun.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2nbujgirb.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2pijsepfc.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2gmnvgeon.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2boomsigy.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2vvwaiqtj.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2kudktumg.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2wcnkqnlm.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2ybucoqlw.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2uccnuprv.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2vtmpxlit.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2urmyvudz.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2imchaybj.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2rxlvskxx.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2wrxqevyr.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2gndfizgt.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2vcgwocth.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2jepagxfx.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2jmihvosl.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2vsgkeqcd.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2ayjmgcdg.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2sxndrrgr.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2idhonzby.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jprtajfq.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2ubgfrzyj.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2aocognfk.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2vjcpvdec.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2etetjiqt.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2bbkhpvnn.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2fhphkppj.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2akaroyna.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2zbzsnacj.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2obvyjfny.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2hhjycato.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2tmpsdwuc.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2jzprswin.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2lympjzkj.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2sxthbtje.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2tgsxxvwy.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2oukempyb.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2hafnssqu.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2rohmwlwm.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2sfrkgyky.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2mahyvwxj.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2fhwsyrmf.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2kuffxmwz.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2fsxzynbf.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2hqrhcvyv.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2jogefwcn.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2cjnqpibp.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2ywbdfviy.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2pxjextqi.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2ygzldduy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2prcnyyvo.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2ryzvysra.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jsijtpqb.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2fjoquyrg.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2zkmcgloj.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2tkynetly.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2ofzeespo.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2esgxjfcz.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2nxulxvul.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2gangnkcy.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2cauyndzf.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2xtjdmljo.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2ypsyulsl.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2vwdxixkb.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2exfurlga.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2kfnmvvzu.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2wijedtbi.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2ihrpsjvb.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2oteievgn.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2vytmpwdd.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2zfeanpdn.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2ahhvsgwt.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2llkzwaks.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2lvincwzc.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2zkqlhvca.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2zelnnkio.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2fltyozeb.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2pwleekhc.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zmusnjtm.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2kktpxrmo.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2cptrbfnj.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2ciookava.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2nsqhcoft.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2mkdtoghr.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2kzgesbjh.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2vkcdpvkl.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2nfrelpwh.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2rdtgqihh.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2jrcgoewf.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2lswypwdl.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2gkssdqqn.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2hfcdbvmb.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2oreaijzr.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2szxhmqsy.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2vftkahpa.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2xiwrakgm.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2oeljnldx.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2inztkiyw.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2frdefkgo.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2xyvqffav.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ufyaufwq.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2msndsjcg.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2jfxgklex.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2roxpjxkn.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2vlxnxtcw.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2iglabwkl.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2aatnrhmw.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2rzwhaxjf.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2krdyzbpk.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2jnrxrujw.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2ggwjaawa.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2rhwdadfx.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2fxfhmtht.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2dhgjofyd.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2fjtcmtaz.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2ordzvqqn.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2smajamdz.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2vdpgsqpb.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2yuuzkcov.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2ehesgcio.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2bhwcqlve.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2vdnnlgrs.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2idakhuvh.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2tluaaqyk.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2eubowcik.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2uyziwukr.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2aqiogwci.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2hbplvymi.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2bfsxzqph.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2lgdwctzc.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2dlacegcc.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2pxafrdud.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2hyvirpkd.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ucbgezjb.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2iycaoful.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2smqmujyh.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2spwqdvzs.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2moxgagxz.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2lyanqhdi.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2sfrdrjim.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2haulbpsz.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2rpgygqeo.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2pleetatr.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2tmoosigr.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2lecvekyf.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2szsyzast.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2qmggtsfl.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2nhqzvpsa.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2hotnsyga.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2ihcoafrd.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2hqwslodr.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ujwljghb.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2pmewudcd.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2mucprhiy.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ybztafrm.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2qbejaijw.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2moqqgnzy.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2zzubnjhq.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2yxmqvatj.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2flwssthm.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2hzzlubws.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2ctcvkdup.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2ajaobatu.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2swrekmil.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2rxjxmypz.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2hqvrcxla.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2dsxwmplz.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2joknpioo.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2vqthidyj.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2idffvedc.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2qvtplycy.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2owxophkg.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2hxouxmyg.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2gwwknrug.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ajbodpoe.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2wyaqnhvi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vvwzodfq.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2rrxblwxw.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2qfcxqlrq.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2bqtsuztn.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2auilxsnz.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2ovfzedpq.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2zskzsrta.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2rlhdtfon.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2cgfdnoba.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2udqihish.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2hzydeams.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2newkkwou.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2zzahgggz.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2lljxnsws.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2tauqowme.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2prlojauf.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2cdxxcyrj.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2cjvfbord.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2hekppzna.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2mywykmuj.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2rnrwzuvd.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2pkskgqlx.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2jcwnyznx.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2gmljhnvp.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2matxbhac.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2nldgwwnf.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2dikakgbp.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2gezuijpo.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2cpnlzgil.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2povxgmjf.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2iwvtobkn.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2tuvdlkot.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2wthkwvuw.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2hkafputt.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2qcwagmqv.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2kfcsaexx.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2hndhxjfl.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2qmjpvotd.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2wtbqigjq.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2zwpiupvp.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2yvsrhuge.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2ulbyjvwo.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2milnzicz.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2owrwrxfb.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2ghpdqhtx.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2lwlmssxw.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2uyjxcdel.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2xsrunzpr.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2iblhmynw.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2bavlrrcm.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2rvvwqtno.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2jojrmgyr.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2igrenjqv.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2vqmasuox.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2olxzwzgs.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2onethgjc.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2olfgmhcy.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2nyskidya.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2hricsiqz.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2hudfvcay.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2iosjfwou.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2zvnqlmgj.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2euuqvmug.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2aqyhenbg.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2znffdqvi.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2eydgxbuu.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2epqhcoqk.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2hxywbxpe.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2pvxviuqc.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2ogbqxqgb.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2avafemnh.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2wwegxguz.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2khiesbcr.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2kwdjfipr.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2arqbbfez.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2nbanuxrz.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2dnawyojw.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2kfneiodo.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2sdsgczxe.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2qoprmdhc.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2tsdapknr.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2qegmdrdh.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2rroqtrax.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2tfpmsoaq.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2wpexgviy.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2wbhjozch.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2agqucxtm.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2zqkxlldm.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2jkvcvegu.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2lnmpyugb.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2saiqobon.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2tnetweie.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2aewghkip.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2paxymwik.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2uisqrzzg.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2ovfdtkal.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2bqpblvld.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2jcsywgjp.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2olcdjgpy.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2cfyyltpf.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2masyvxxs.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2hfykfkac.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2vjjzvzry.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2loaakoxb.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2wajulpdx.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2sjhiaiac.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2arrhvvbd.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2fkgjkonx.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2vsfgyzbh.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2bdyjexuj.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2kvtdgjca.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2xkonewhj.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2zqwtgaqt.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2viknldil.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2usvmskak.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2kwgjreqf.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2hisfdgxm.html


<!-- 参考信息 -->