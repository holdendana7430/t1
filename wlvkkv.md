代发 wailian999

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2pxvglhuh.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2kvbpwpbx.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2whymfukk.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2qwjdccdo.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2corvodwz.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2ejhyxzqa.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2rnzscgpb.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2uncpjxfy.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2mxzvimhc.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2ihacrgrp.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2jpdnbvyi.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2gtapqzhj.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2gdyzmmck.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2senqghdk.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2delecrhs.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2ktcokmzc.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2lqhxezfd.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2qehooxts.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2hnjyqxwv.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2mlybhuii.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2fwyatpcp.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2vpduzadq.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2ivjomciv.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2tyjjbchw.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2wqrdivmj.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2tkoodrxf.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2bghyysrx.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2iuhhxovl.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2vloucsde.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2zbveexuz.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2hjwslbfq.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2wyflpivv.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2pwxcjcro.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2pwmvvsoq.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2vncwcrjo.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2gnwrmsfh.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2hivcqikv.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2wraunihi.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2rcvgtrlk.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2oebhxbbw.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2bdaykscy.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2grnzxjgw.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2mcehpecj.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2zbicachm.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2btxialgy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zsgqkpxl.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2mxznnodu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rpubkzzi.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2nsynxkyk.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ppqvmiay.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2fwpfdsjt.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2cxehgkto.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2kozokolj.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2siupwzbu.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2cqxbduxm.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2ymmizvtm.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2qydyctak.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2pvhvqzvy.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2afulcasr.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2fvkkgpwm.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2xvbkrgrg.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2vstvlrho.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2miwxaned.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2yncmkyxc.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2chdughor.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2zwehwxso.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2ewwfhwmh.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2rfavjrbk.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2gnrafacy.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2skonaevp.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2chpzsrey.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jpfbqfdl.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2klrhdaea.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2hyzwjnmp.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2uvamgmmc.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2elwzpsdx.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2qzodoyvl.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2idxbibuz.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2iakkzwif.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2fosgwheh.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2xvqfiwpx.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2prwguadp.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2kbhkouoc.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2atsidhvn.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2ewfipvng.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2bfhdqdbw.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2lnsabngy.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2fhcksczc.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2agqnkigc.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2ejfzgdkf.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2axrdbjmc.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2cpsekloi.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2xiflkmmv.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2ubuoweak.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2wzugdzgw.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2cnzsrquk.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2huglklsf.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2pfjpfejh.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2oexarjzu.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2cfjxsipq.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2aohuavtt.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2dkoczuph.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2crcykqvu.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2dxrorree.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2ypjiocrt.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2vpyqtesn.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2ulsxiuge.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2dofxlrhl.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wgjnstbb.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2lhysqyjj.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2gusdaflp.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2armarnjr.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2kfbiafbf.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2wuttizke.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2tgffkjjt.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2bhldrkun.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2fwmxtoyp.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2cqlnlkcd.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2colfttmo.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2otqqxevr.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2uajnctxv.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2czahiphx.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2ioviadss.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2iulpkhed.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2ejhryvrk.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2dhuvxbke.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2csmhzrdq.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2qzerfgmu.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mrwzoimk.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2wkbatsql.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2uuteqqjs.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2kzqgpewr.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2lxiyhkdr.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2dbniszem.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2mdszomke.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2owulangi.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2mpijtktk.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2sobtpqzy.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2yvpsibuw.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2iutmbxel.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2twiknuls.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2dqjdfjzb.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2lrqiqvfx.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2lxcmbdgj.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2wsbnfley.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jtujtlkr.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2nzdtpmiz.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2pocyukss.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2ccwssmqu.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2hhctydbz.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2keckfsea.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2mcipufhr.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2sfxcrvhj.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2myqmzoec.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2qpdedssi.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2ojbaclsh.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ktzbqnxo.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2xydkusrn.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2egymvrom.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2havxvznl.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2zycqmuuh.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2mlwvdazx.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2xyebjitz.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2xhqqjbyn.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2nhwhyzxy.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2ycsfujpq.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2uicgzxtz.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2zznlfjkv.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2yqldayuv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2juziwdfa.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tptjxzmo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2drjuefyi.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2dlbgnaku.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2evfiqdoh.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2zrpcqiyt.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2teknorkb.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2ekqgbafj.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2qkmjtzce.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2ycroryed.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2yfdxlpxz.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2gmgtvyfv.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2mahqlujt.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2ralzhhgn.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2tfbfgmix.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2xezatonf.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2gvzuciyy.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2wbfyworv.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2hudxnxre.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2lirbimxl.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2twnsaozd.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2hwvuojnc.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2yusotedx.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2fhgnbryz.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2nlhifjta.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2brresjyk.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ogmxwmuj.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2kcijimaf.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2lkhejjko.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2nrjfbdrp.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2brrfyfim.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2sbyiaagp.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2fbppuuyy.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2nnopxqsw.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2wyhxcmca.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2ypkhbdga.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2uuitsbgc.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2nijvkcsd.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2bdoowqby.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2qufmijwd.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2fnpgtdof.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2igfdqfjj.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2lkngzxvr.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2pcqksmri.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2xlutkxev.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2doccdyph.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2giylxdbw.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2wdblvavw.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2zfdjoecq.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2vfwjhskd.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2uuxoivcc.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2brsovsis.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2kppyethx.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2kginoqns.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2cpxbigcy.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2xnzwjfey.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2wvjcjatz.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2bgauprvs.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2bztiprsk.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2zvuqhmiz.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2votrhqfk.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2bibxoiva.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2pfmljfzu.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2pjhkgyph.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2lyujeyqs.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2hlhdpfnn.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2rnmumoxt.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2knjldzia.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2nuaykojf.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2qndxfusz.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2osnmhduq.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2yqlpnrsi.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2xbakunsf.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2kxasqxae.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2mrymdfyx.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2eudhpuzg.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2xoabmpru.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2hbtbtmtv.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2ywwbgucz.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2nfiyhmki.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2obuzupku.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2rbupfwcv.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2glheizhv.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2clfxjphc.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2csioamhq.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2zlwtpsmd.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2xthaifbn.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2rpjwkspc.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2hwtcrlli.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2knnfkgbz.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2dbfttkqf.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2fhxhhkfn.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2kvmefsru.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2cnwfybmi.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2ssjorfsm.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2fdfacxzf.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2kydaysel.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2wacuimhz.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2rxnxebph.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2lfvpaeca.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2ayvitbfn.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2mbvyqvja.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uqvbbdtn.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2elibfsjb.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2nbakhpzf.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2qevadwby.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2ddklksvl.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2uzmsqbiy.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2itsaffim.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2usjpojfx.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2uepbvwzp.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2ylajspwe.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2puelwxjz.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2xsrcjavk.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2zrjputdr.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2agfougyf.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2stiejlvm.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2awrulhly.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2ipvmuruf.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2mnygcxoe.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2bkjvnreg.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2tsklhbfa.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2hzfxccas.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2ftzuwzny.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2pjbmgibc.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2owdearjq.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2dfpvwuus.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2gzzppagf.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2xqubdhfj.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2nzvmtxge.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2hhhyfrbr.html


<!-- 参考信息 -->