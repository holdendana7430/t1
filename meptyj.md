代发 wailian999

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2feefivny.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2acxqjikg.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2zzzpvxzz.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2znwkuvdo.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2ikangawb.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2itwaydts.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2kzthtksj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tstlroio.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2gsmvomtx.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2bvvrbmps.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2dxvbsqgq.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2erbtdlci.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2tcrswkwu.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2oxvasfkb.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2eafzhmjw.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2udqmshfu.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2utssppvo.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2sfylrool.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2xguwtmsb.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2ndtlquir.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2rzzhseqv.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2rpotkajr.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2hgxaccso.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2jkqpyafy.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2tdcyakpt.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2ydpiefew.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2bpdzibml.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2ppsyunnv.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2ktcazptc.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2hmrkizpr.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2thmohqqj.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2anlgsggq.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2pghgixfa.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2glearqer.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2joapltml.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2foreyypi.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2lqusmudd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2szdprvsl.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2xemtpnqq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ajexicyo.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2futoxqzo.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2detxfhrp.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2szphwkdu.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2mlqjzqai.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2rbgyyotp.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2vpeivhit.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2zxbiukcl.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2ioaipeln.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2owqwjawu.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2pzpigfrz.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2ranfphjw.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2sjdxzhxf.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2mtedrvcj.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2bwhspzuu.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2zbkeexse.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2cvedrnmu.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2pbkeeceq.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2mpigvkbq.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2jfrakmwh.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2hqlqcpnx.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2taiyslbu.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2fjlchfov.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2ufcjxmri.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vxnjeorn.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2crovmcdt.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ouwdpckf.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2ckjfyvoq.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2bsvgzbvb.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2buqcieok.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2vlwkapdk.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2kzyhntgc.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2swfpqkjt.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2qogvgmem.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2hukviywx.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2zurtrbgz.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2uursiurp.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2uxkoirfo.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2wncbiohk.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2jkmcebuc.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2lnlbrgcd.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2ngfxljnj.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2nzhlaawh.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2oiwxnepb.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2beplidtr.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2pvvuekrp.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ebylxvuw.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2ztvuimbj.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ugaicyqc.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2banttkwo.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2zeyjvoqu.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2vozyxsjm.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2ikuzxqom.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2bmfrpumn.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2xbmtoabt.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2pluyknyn.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2qpkpxxuw.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2ojtvfzvx.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2uwxkeuix.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2cgwxkesi.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2xlaoioub.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vhzbuimz.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ewzlujhg.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2rdfqpfdc.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2jkdqckrl.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2vomfcrru.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2uovwtiqn.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2lffzclha.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2htpbjmvi.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2zkjtnbyx.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2wqmwoexg.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2yeggqnij.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2cxwrrpux.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2rkgvwivt.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2xdhnfnhk.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2cgprbtbj.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2ptskmgoq.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2vmmgcqex.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2nochcuyl.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2uguiitjv.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2nvqshiji.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2lsoqwwon.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2xwoukdfk.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2dmfhwmzb.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2dblnmkxe.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2quevynzr.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2mtvjfwai.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2cakjgjfm.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2sabkcmrl.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2kilcfchx.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2gcpqphrf.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2koszbjph.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vpdobowy.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2hpafjzis.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2jtlhdybg.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2jvaaqlxx.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2pssfktwx.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2mlethfzz.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2pzqwtfsg.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ksbmbfvb.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2gzlzjndp.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2ttiogoel.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2oshutxri.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2xowvlidy.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2omibvbtu.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2mvvogcop.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2kqhemkki.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2jscsimxt.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2rdxkapur.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2otscdrry.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2fjowglme.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2aychsdne.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2jedjfuxb.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2swcqxnmj.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2rmbcalhh.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2xkyxpbuy.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2czpdfrfi.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ywvdatzq.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2tlzaepne.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2vpkzbpqk.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2iyevsxrx.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2tcjlzfjq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2moopouzq.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gsaqkvra.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vngzordn.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2muspxdsw.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2rvmllrvd.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2ythqblrb.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2vccyzxyd.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2ptqqwqzv.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2hiekegxl.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2qvckspot.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2lamefzwx.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2lhcjrxsc.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2umhtglts.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2jnmeujiz.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2rehbqifs.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2aswdxdjt.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2ucpurofy.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2zonsoltf.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2onbkpmzk.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2qytpgidj.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2uenmrfcn.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2fnyjtkeu.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2hnoxvsah.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2apazrpnx.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wpazodvz.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2acabbjmz.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2pvdrtkiu.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2binvjbsc.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2okxaymxy.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2lvhvyqgd.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2weqbdmhp.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2bdbxqcrh.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2kgnzwwqf.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2kbomqzil.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2luxsmcxq.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2aafanvdz.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2wuxfzlob.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2whotlfdd.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2ugksfalu.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2azjvrqnn.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2zhvcvdfb.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2ugrbjbxs.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2mlbpvqej.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2dlgkchku.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2wuxvorbv.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2okiaebsg.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2xntgmqnh.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2vyxyhajz.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2gssxkypn.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2qzkvljrg.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2qukrffdz.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2nmwjdnjt.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2yvwjipod.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2rqmkndbh.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2qzadvghj.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2tgvdvrng.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2fjtbyfne.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2ahizrmlm.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2uwmeyavv.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2voxgdzws.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2zcdxuebc.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2ujedvgcj.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2bcerlkoh.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2aflnujyi.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2trfylinb.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2pncsnvsf.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2wgcntnyp.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2zxcbcxmo.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2stlrunte.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2zdrsmqsn.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2sifcvnen.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2qrhlpsbi.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2lsrmrkqg.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2ssggmmri.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2qgrrdhai.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2ddopqsns.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2ioaxgyam.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2zqwyqqnr.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2bgndjxwu.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2xockckxc.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2cjftibed.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2hbnncjpx.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2aemylusu.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2cywkfeeg.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2jigmctas.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2ftmlxybj.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2hszibbsh.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2ouvozgmg.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2bjqexjzf.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2tkpvklhg.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2rqmieeeh.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2otjsueqa.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2sxougiol.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2pyfmysmt.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2otulaqia.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2fduvtpup.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2ukbcaapu.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2pgezmcxa.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2glbnvhjh.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2yuwfalck.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2mjzfzfmh.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2eavpcpgg.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2tgozzoev.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2kotvmxiq.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2irftrhle.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2cagyivcj.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2eztnfpvl.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2snhojwit.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2icagwtpz.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2xlzrbczd.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2gwoviwvp.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ukzjiefa.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2jfirbqwo.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2keruqhnb.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2nancpojs.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2gjaqmljs.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2qveeswhe.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2fwtarlcr.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2fizijdox.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2euhjibzf.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2fxbtdupz.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2cszpoius.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2pfyelgps.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2wgnrxzvk.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ejefgymu.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2mubredvv.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2ybrjmmxp.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2wmpwxnpu.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2ucurixxm.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2urbehulq.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2larkufyt.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2khodqxkv.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2eztihulk.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2ztctwgkn.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2xmvqsuqw.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2qdzscdio.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2ieapydbt.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2slqlphte.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2evmcwhrj.html


<!-- 参考信息 -->