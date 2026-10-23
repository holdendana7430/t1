代发 wailian999

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3kvjaborp.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3udwlrnyk.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3dteyqbbp.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3yaeqagbh.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3mdmxkjsc.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3xlsyiznr.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3uyqwjyjt.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fmjgakof.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3fsrckmir.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3hpfzrhzm.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3pyjwmvgw.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3hraecaqh.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3vkjcyoaq.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3trenqlch.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3spzcobur.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3hdacshsb.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3qunrofop.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3yvmhbmre.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3oktxjkac.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3lvvdfytc.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3ztmwugix.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3fbndnnlz.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3wzjlcnsv.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3jmkxlhrn.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3zxxubmii.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3ghcsmgru.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3bmmyuqtl.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3lenswudq.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3itvngywd.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3xidtxbdl.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3fcmujgxn.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3cawfonwb.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3fcvhonth.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3pfvacukw.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3zsexendm.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3jwtpyxea.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3paqawsie.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yhmnocxl.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3vscownud.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lrledyug.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ywkyulhs.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3twtmmnkm.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3tdcwmqwa.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3revssgic.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3mjzazpcy.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3emrjijmb.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3zulflbgz.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3ppmcxtnk.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3tcdauepw.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3vynxevon.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3nmfpcmfy.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3yywlymwj.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3amoucwea.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3phtsvgmz.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3ivmdijta.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3kbomwbgz.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3ypqkpadv.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3ehjfsman.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3esvqtshl.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3ejvshkur.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3zuuioxas.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3hgkdumzn.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3umnatgkt.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ktksptbx.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3uheywkhw.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3sofscujl.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3imouwpub.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3bpxdlyal.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3wdmihwzb.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3supkgakr.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ibxurynw.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3xybxshvb.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3yyottyrp.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3edozronx.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3hdkkfsre.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3ojlltzmt.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3beoqqkfh.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3nzwperic.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3swmwbwvp.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3eoobcwja.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3eeskqhcm.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3isxolkpk.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3frqmfwyb.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3rywxmxwy.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3hvaiezcu.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3sngfbpab.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3jlnhcphz.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3nhlslswa.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3ajaycjyt.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3qoxozezq.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3pmzwbfht.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3azofyvjt.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3ysvaosba.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3xiroxepn.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3wtjgoqlc.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3fmrlhzwo.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3npjakhuo.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3mzpzgvuh.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3wykvwhph.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3qbtmipjb.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jkrppkoy.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3augldccf.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3nvppxhnt.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3knznmssp.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3xicgmybd.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3vzfitzgs.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3zjjgpsks.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3gotpbdum.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3cfvbcdrb.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3rqzvitct.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3ejlkijkt.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3ngujbqvx.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3cosecpvv.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3jehvbexe.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3nitljpqp.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3hsahhofj.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3fvrndgxp.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3sobiafev.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3dtvilghv.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3lsqfczph.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3plvjpcko.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3widxyjua.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3nyskmlwu.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3xkwuallh.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3izvwgahr.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3nhcbtjbb.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3qaaesmvc.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3ntiqqtgz.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3swtzhobw.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3ndxjubey.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3lrkrmaev.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3jbziyciv.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3rirownsf.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3tpkzbpdt.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3ntqlbrrn.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3vigezxxc.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3qkafwmlj.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3orvsqceg.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3bzpnyclq.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3cqilzhgl.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3lwwmewue.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3enrvurjw.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3yukuuxli.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3rlfnsdec.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3udobicti.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ykqnfndz.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3utojxeup.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3nnfdjwcy.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xfhtpzfb.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3rdhjgepf.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3dgigyjhg.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3qvpopiir.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3ptswbtiq.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3egbffryt.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3yarcaazc.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3iofbiyec.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3wfadugvp.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3nldjyhnu.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3sbyborfl.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3yohygrbj.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3nmpfpram.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oacxofkj.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3djkkqowj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rzcddotr.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3pqjjtwza.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3lvwxhxvl.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3tgjdydlu.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3ahoeqvyw.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3fjbcczmd.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3mmpmldls.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3pxgwqnvn.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3qeucecjt.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3mxcekzhd.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3mmuyrcto.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3vejeiubw.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3fvwfubwz.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3pqxzpvhr.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3nkvcymoe.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3kvcziyse.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3zytlnqed.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3bgpvwvxp.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3nadectyk.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3hpedjilj.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3dzfcbuit.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3sccblfct.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3zoekqfzg.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3dyamvsjz.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3zoevqwuz.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3fzwefewl.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3lnislpkx.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3fygsmhmp.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3rmhpdtnw.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3dgjlejeq.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3bpeyykpq.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3wfwydcqd.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3rknzxvvq.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3uwfzfznv.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3iozwjdos.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3dkrpvoxa.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3rgwturit.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3afknqehp.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3pojmcghl.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3ebxswdae.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3vjovraso.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3ckdvrggi.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3znoicknn.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3zrygdheg.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3hmhwrack.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3atpetpkj.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3sictvvtl.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3pfmmobrf.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3iouztwju.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3lxrnxsvl.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3ewrfypgg.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3djosotit.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3alpzvhds.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3syvswydg.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3eheihvvx.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3saduaybc.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3xlcesink.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3vdxznuju.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3ctlxedmu.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3buhgcwch.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3kujoaawz.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3xlodhbpj.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3lnzecntr.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3qgfkfvjn.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3sijzistb.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3ncfymkmt.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3saovxdbc.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3izvwwhvl.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3snrhfypw.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3xibwigcu.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3bfhubkqf.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3uhmyliml.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3jlychjcs.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3sdknrwpn.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3zzzxiktr.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3cebzwrhz.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3zlhoccju.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3pyrfnbtn.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3rvkxxfpv.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3wdjljoaw.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3cubczrml.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3fvwqgfyc.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3cpmhamvb.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3gkuhaope.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3bjycradp.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3dnsfqspr.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3welhfsmr.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3tqgaasik.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3lpwiuohq.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3wwdxinjo.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3tlqukncl.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3wiorbklp.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3nbkxtmuh.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3ytoapmrt.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3qfiwqjfl.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3npnonlvk.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zngaqfqw.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3ldcvjiix.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3gfgdducb.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3uszyuowt.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3dlvtbvnv.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3uvbqfbsj.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3nfhjmqid.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3ugeqglhb.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3msgbofyf.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3eaqlvoua.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3vdwnuxkd.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3ymqratfs.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3vbnqhcuo.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3onbkqxch.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3udaszkfq.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3ptsfoudy.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3pwxxloei.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3bquonczh.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3rtxkwkje.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3wpvkwjyt.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3rjunceea.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3mezpcvno.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3prszqfzu.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3bayyjfly.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3tsoehtqi.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3hejroyxl.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3qeuivzdi.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3mhlgvdjr.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3xrrpezdt.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3pgvmwmxs.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3eguwtzgv.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3judqjdlp.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3esgfyqeq.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3bchgogsi.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3mkwqldeg.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3hgdhqhdh.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3jsapgxyk.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3xqjpnity.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3atdagpij.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3hfxtqdup.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3zbzodrkf.html


<!-- 参考信息 -->