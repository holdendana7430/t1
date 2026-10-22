代发 wailian999

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2mgvqpujp.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2bhjkdbyo.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2npntjrbq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2yqiiruav.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2baogweva.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2dskyrhgh.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2fazwtfnc.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2wejypphm.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2pjaxkmjn.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2igerrfnx.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2kdtvffym.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2tubnuydt.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2rtrhqewx.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2tcvwlarz.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2caxkcqzd.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2pungxunt.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2ezcbviob.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2qnavfmql.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2yqvxjreh.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2xwgzmvcp.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2bgsxkgfk.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2ypbiayzy.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2yaflyngw.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kkcqkghc.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2qvvgezha.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2qfpydnja.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2vagoqxjt.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2dngvpvov.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2iiichcnb.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2rhfnrwkc.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2whafijtm.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2gqflevma.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ivrufmsb.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2oazllydt.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2tuzufzax.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2vxnwzmxe.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2wsifayxz.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2gltjxuyh.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2nthurghl.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2tqgekybf.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2tskcondn.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2mjgliylw.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rnaggrqn.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2nirtdwqk.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2uamxlrer.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2dvnqnrhl.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2yvaliytd.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2gdzyjbxq.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2oijaoklx.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2qarbbvge.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2xayzymiu.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2dddmldcy.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2hbxqhefn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mbzrzpqk.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2ftybtqfc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cyzexvjb.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2kmrhiudj.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2zdcmpxml.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2jqngyqyr.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2udlywhro.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2slyubayt.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2wamrjnuc.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2vcgbdlwl.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2mjgzcsht.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2dvwnwpuy.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2nnbdufph.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2uxptncjx.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2pafmztpx.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2kactgvdf.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2yzacgics.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2gyaylmrd.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2tghlgltm.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2xkxjqzhm.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2sxkuybmt.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2alolzwse.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2urygbesx.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2oyatdtmn.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2fncjyned.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2huosgfcs.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2apdqsmuj.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2mkvidyln.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2xhdfhyto.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2yccubcqf.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2fvuhwbal.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2jfjtkpcd.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2cfdkuxrw.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2iycqddcv.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2uhrsabeo.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2ambtowrx.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2yiivcovv.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2lxunknrh.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2fmyuxaia.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2uygcntkg.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2xsxdqcwf.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2hhyrrymm.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2swutacfo.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2cwcmewxk.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2ercouxeg.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2ppacurpo.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2jhgslpsa.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2gnzujivg.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2becwzohr.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2famabnly.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2nrasgqpt.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2hikcjzfd.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2luhgtveu.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2xtbisdps.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2gbtcekee.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2hpdmiggs.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2dnjljbtk.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2utdprulf.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2nxkbujob.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2efkfkhhm.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2wyeqhxlf.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2oqykeooy.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2skctoovj.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2mbozbbfy.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2cprenwxn.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2wnnheuyz.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2gwjkuwjb.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2yrftjghq.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2bqymkpes.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2smysiuro.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2hwrajues.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2pbogfvrh.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2irhgnssg.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2hkpkpcwl.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2akobnjic.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2tfimehoj.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2pmshklec.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2zdzjjwim.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2ezodegay.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2dvxpekok.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2fehvmrde.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2iuknqcmo.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2bkaxevbp.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wdwsvdvs.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2snjkfgpj.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2xxenlmjo.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2grwllcaf.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2niymhmef.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2yrjngllg.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2fqrubsac.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2zfpftfrh.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2gvcxiura.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2mmsacpro.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2fpxnhewj.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2aaoubgky.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2papzzpwd.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2amyidwac.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2euxbucki.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2crxfxlrn.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2xfgqiede.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cqvnlxrq.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2xpgucowp.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2zaiebdfe.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2wwwmrhuq.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2zddnmilt.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2jmucxvmg.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2hmsdhcyd.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2dzhnimro.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2cmwpbohe.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2sazsovvs.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2yuisbizg.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2mhzprcou.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2laejswhz.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2gtniappc.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2umxovnvv.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2bpauisuk.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2itffyqfv.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2pqqcfyhp.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2bogqhmzy.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2lbokhnrv.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2zvjfakev.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2irknnprt.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2euxpabwq.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2ccecanzg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kbmjysfu.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jkcccpat.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jkuxpzwx.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2qvifwiro.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2sshzrcli.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2zevjddjg.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2xsbpdcvt.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2qgmpwlgf.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2jhjbrdwv.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2phejiiim.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2colnjtit.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2auofmbgj.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2ldbjahxr.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2koyufsjp.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2jwdgtsum.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2ewvrsiql.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2eqtfyqiw.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2ugrjmnoo.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2qlsiwirn.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2qzsvmzmq.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2iqgtwtqj.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2eovbswrt.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2aefaspni.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2allxzqbq.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2ehnfbkgk.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2npbqkajk.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2fazzjsik.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2gkrrgfek.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2cbghiirz.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2mlkxrpid.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2flypxspp.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2jgicuskv.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2zncwnjqp.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2ncsdmiol.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2mfpzulje.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2uehdwvcb.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2vnvneytw.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2ngmgnmny.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2wgmgybyf.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2wlrfygel.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2uzwtihzu.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2snexilfa.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2haqxohsn.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2wsaqeufu.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2pugbmdzv.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2ghfisxgf.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2iutpwaeh.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2lvkwugtk.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2lnjfokkw.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2gopuzpul.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2lanijrvk.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2bpuuratz.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2rjhurjid.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2yhjrxtla.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2txnqnzjf.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2bnksjvlp.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2ryltphmo.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2rgjmyxxx.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2upztglay.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2wgegvikp.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2uyoukydl.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2vuqpjqbc.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2slvlcqig.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2xoycaacm.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2iekhlykc.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ptencgne.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2nvruabic.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2yzciluxe.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2sfeidrbj.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2rdnnligj.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2exysdluq.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2mymfzmdt.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2umgoogho.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2vaqvfldv.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2xvinpsay.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2xwstjncw.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2uhywxbvb.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2ajkpvbjr.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2kphvwpkk.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2ydwvgdjo.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2bvoudfec.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2vtltfjrd.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2ggrrhpvq.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2kvohiwyx.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2phzcnird.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2lanmuqfg.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2ksbkihgr.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2rmhmrckd.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2hkevzhpj.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2xzykxjij.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2rmrvaevz.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2jscivofq.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dlsmklwx.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2lbjhhdil.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2opvqgfhj.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2jwtdkrct.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2zjimctvq.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2wbtqzffv.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2gznhvbds.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2vtbefffq.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2pdjacvjv.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2jkbhzeoh.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2izkpupbo.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2npdakptz.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2uzvhmisc.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2ghxlqrwm.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2sztxspct.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2lgyiznpi.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2qwzllovr.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2jxheaaku.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2dxrnwqbv.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2rlpcrbli.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2ylnsotwu.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2cmpvsibm.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2utigpuin.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2yxfjkejg.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2ptgredie.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2zgeuyxud.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2bawayqoc.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2pjbhqkaz.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2tokiozcn.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2dshmszmw.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2keipyeye.html


<!-- 参考信息 -->