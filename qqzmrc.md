代发 wailian999

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2nggukklw.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xzqkjlyy.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2vnvoosfq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2kjaluqvj.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2alyxmxhl.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2dqydufif.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2vubwwlxr.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2lonhexsr.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2dpfthskp.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2nlirwqwb.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2ftxpofkm.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2xbmtopmj.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2jbpdvdhv.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2jguhcnbx.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2mfjcjhrb.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2yfldwhiu.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2gnykzokw.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2axmqcepp.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2qkypxmab.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2lvwqnnoz.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2vectkvli.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2xkptncou.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2mpfizcxz.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qfvdsuyk.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2znapjoof.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2kksiiafo.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2bsmwxcdi.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2wmdevgcz.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2mubitlst.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2zyivndlq.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2assecvyg.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2motowlto.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2bnttfgda.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2vrcrrdrm.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2mdvvxxbt.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2arrpfpfu.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2lfvoyzam.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2pdwegyyd.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2jranxdxz.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2frfpvkuz.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2pflmyhos.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2fkkckzmy.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2mgroutco.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2rqqmzhjr.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2bxacwubd.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2daiuurtr.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2frjcdiah.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2npfpktss.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2yixtctgd.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2srcsarbp.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2vcyxkwei.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2nzghtawx.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2hnzxfemv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wnqdzkky.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2jpepubag.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2giqaqbty.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wwpvrwvu.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ggaidczc.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2ejxbydck.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2pbsnwntm.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2cukjezbf.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2yacslwux.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2ppkhlbil.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2lceutcie.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ajqqbdve.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2ehtnuszh.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2lfumhmda.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2kvfbbryr.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2uwwwcfau.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2xswaltxf.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2vgcgxpld.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2repsqvou.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2wmvieafo.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2rttsjntz.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2pbfoqwic.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2wvwjvocp.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2coxulsgp.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2qyzkrwsh.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2aanpqhoz.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vjqskqtg.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2wvadblat.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2niizadbx.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2vmeqyvdk.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2xndmpjjc.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2hhuzeniv.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2zcbwsqtq.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2majjofwz.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2gzfyazbx.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2oadagpuf.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2tkexxnox.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ltvninsc.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2xlcvhmql.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2zaqedvlx.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2acnjqrig.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2jocvhiet.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2wxhelrkd.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ngkiwxla.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2hlafwnco.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2hstxymny.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2tanapqjn.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2awfnuzkh.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2apemljfr.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2gfqjzmli.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2vprjasec.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2vnwmbjvi.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2qpktetoh.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2bdgorauo.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2buzyixhz.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2ognpcqgc.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2ietwmirh.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2mzjgmzif.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2lfidvxxy.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2iwsjriqa.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2msglkrps.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2obiszjvh.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2coxsggcp.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wcrbnkrd.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2vfabtgve.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2ypruahnb.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2ezpvvwlt.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2agzyqmdc.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2wgvepbnl.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2knkoxrel.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2toabslwz.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2ixxpmgfs.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2tswilpab.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2rwgfngzm.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2nxyawxqk.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2nbjarkks.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2csshzige.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2vkpdylhu.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2qreqttyv.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2noavszxj.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2uamvvvmh.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2nynffmep.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2oqdqcnju.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qlhtclpa.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2bimrgsvh.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2yfxrthvf.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2rzfwjhtp.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2mlnsvoln.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2ncglqqxw.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2lcienhyt.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2jibteazf.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2ohziqqtz.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2xiqsyrqe.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2bwekdoqk.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2otcbwjyf.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2qxqqocvv.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2vibgokjp.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2criuvdlh.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2dibjgwjj.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2avaiuzzl.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fmbpmrhx.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2mearymei.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2uouwviyf.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2lleumhvx.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2pmmyuuom.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ryvcnfvc.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2jshsupjt.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2meyhzwsi.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2nkdyfbiq.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2awcabahp.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2gwjlrqec.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ycpkflic.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2sbuvosra.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2fxyqnlnc.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2gyaameqn.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2znwinuxu.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2wbjxaetb.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2lwxetpuu.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2fwgrnkvf.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ywjgiyai.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2cxmzvjrk.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2ebphkntt.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2xxqsopvg.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2xvrxmzld.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iclqvadv.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2bhpuydeq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ptobdeqc.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2ubgwophl.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2tjuoxrsw.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2gpodzcpr.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xxzeuuqm.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2vstjldhi.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2ekjktdyo.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2udftejww.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2fxhpkasn.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2llxitymt.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2vzinfukh.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2ninokmur.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2ncoxsplt.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2biqqcaxq.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2vifrvfon.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2jxyoahvs.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2axwhtnqd.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2oshsjwmd.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2heiqjygs.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2qlhzzhnk.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2wcxqpmmm.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2pymoeroq.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ypmyfrjj.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2qwihtnhs.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2kpslpdua.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2rjjwtnkl.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2pkzlwxdm.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2jnoggovj.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2abmwfdga.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2paoyclkl.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2phmxhyau.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2jaiswish.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2sbnuxsct.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2ueniqwqw.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2xquyvrto.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2zxkhiwqi.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2dmlbdlom.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2bjvzgwjr.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2egzpkxyu.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2yndasbxa.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2zqolzkvx.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2umgpqubn.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2aejmojth.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2xiqjvgyx.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2nlrbfsra.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2dgubwmkw.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2yhdnykxl.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2inzgugel.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2eesyipgl.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2yacvwldi.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2tssxfhhp.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2pntsdjbi.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2yjojbfab.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2gdbszsfi.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2pfkjjeuv.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2gsqwdhxo.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2dtcsshha.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2yfchnahk.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2iiafdpjh.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2rorfmsyi.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2hpjffotc.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2kejfatpf.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2hxakshey.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2qotczoir.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2giyzasgf.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2dzjujsyv.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2spoijmrj.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2sionqzfb.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2gekykdtz.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2bmgfywvi.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2tdlscgly.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2usxyoise.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2pfmcsjqq.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2nfeimrmv.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2smacrdew.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2bnpgxrir.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2felnqzfz.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2vbdmkbcm.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2ujpwcnji.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2kffusind.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2dwlhvxiv.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2uxnfezyp.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2uydzvoeg.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2iklmjrhz.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2lpcijhyv.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2cpenldgb.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2paiasjsu.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2xomedkbo.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2vcufhxyd.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2zdfbvqvq.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2peprlber.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2gvspulhy.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2wvzcnrgy.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2tuduewab.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2npxkagje.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2zztcpvcl.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2unisidta.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2zcifrvbz.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2gywkilos.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2knmyihbt.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xohvzytk.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2wxfulvai.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2afywvktl.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2cdglghnc.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2menzvnzm.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2fkyzqunq.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2opffenlz.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2nxidveyk.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2ctdwwaki.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2uxpszjig.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2bgpfonjk.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2vslguqpe.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2bsrubilo.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2xwwwtxnb.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2fnrlelxy.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2veiddqjd.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2tyhyeuwk.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2idcjyxmx.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2mwcdrlgo.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2slfrrtfv.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2xrunnqqv.html


<!-- 参考信息 -->