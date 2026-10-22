代发 wailian999

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2kblupfld.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2nmfrklsk.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2gyuzncpq.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2fihkcquq.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2fpvcawrd.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2aeyjkyrb.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2irwgvaua.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pwmpqnib.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2znooatsz.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2piebnqmr.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2twyecvzv.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2xkgrvdfq.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2tqojuqxc.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2dgncpdfw.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2unnrwjrz.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2rxbybrcj.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2aumevxke.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2dtqgvgbc.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2hzsgydrj.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2pvuqoupu.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2prapvkdo.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2hlcbxoqq.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2iusqvjav.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2rtpvqoyf.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2rcsiwqmo.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2ztqcwhug.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2tcgqjesb.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2octpanzd.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2yjloowvu.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2libpbyse.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2nmmsrjaq.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2rfflirqn.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2filohcev.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2nwduguem.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2jlmelcni.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2pwwtbbkj.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2dovumkpq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mjispxnp.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2jicztdmh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ljntcnhd.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2valnkquo.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2qzszyiav.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2hynfhiio.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2echnbpct.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2vlkrfipx.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2jffojgsr.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2axntgcum.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2eigzdcpd.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2vfbupnzd.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2emcmeplx.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2ixtlizph.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2jbjefaqc.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2piagoisx.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2zrsmdigx.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2qouvhchr.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2mvufcygr.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2nqqpptyi.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2adzkhjnx.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2lhvqlwyx.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2ruxsjpwy.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2ricsbcbx.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2akgtspab.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2bkrkeagx.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2tvspcsfy.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2ndjqomrj.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2rwesrhvx.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2owrfomqq.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ohiifnfp.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2sgegetyn.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2klflyouq.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2sorjsnep.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2hycuzznk.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2favuadim.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2jevdrfrb.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2iaxczvvh.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2ayiequyd.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2pcihpjnp.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2ulrsdrrl.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2mcarhtas.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2kxkygoln.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2kvfoxxrm.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2pizlvszh.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2ktjnrkdf.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2gtbijefv.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2jymtmkgv.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2fjclkdpi.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2eaamqtle.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2hdedqluc.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2syqncier.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2shcqbqrc.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2rwkfdzxy.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2tnmhuoal.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2fapapjle.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2ayqjfgnu.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2zdyjpasx.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2xpvyzjvs.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2qrcjvjio.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2inytfows.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2gnuseovj.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2qwyauhpi.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rtezsvhf.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ytdthbyi.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2reuvxyly.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2oqfrjqmq.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2yszrzvsn.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2dbkehnvt.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2rcrhjpxb.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2udhkvpie.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2ddecjvdw.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2drenmmiv.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2jgpiiakr.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2sidbdind.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2zxvlcxkk.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2ggypftgx.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2ktpyoaek.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2eogdzrtk.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2nryfvljo.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2wprbccgw.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2axhjeave.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2pjtwdidj.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2hwscnqer.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2zhugyggp.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2vadykted.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2icqsjywf.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2glxbmknc.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2mvlqqwex.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2usojoimw.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2njesnxsj.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2eulvyagc.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2nszgijqh.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2mkoxzspg.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2hntuiqpc.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2veawwjjm.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2vnormusd.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2kzqcyfmd.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2mstdiygt.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2hidoftlw.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2anzvxhib.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2efenfmwh.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2nsizsutx.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2gelthfra.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2losqutne.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2dswnuujc.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2pigcmhrk.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2liknhypq.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2evbjjifl.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2cvsbzdjf.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2vpykymsw.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2tmualdcr.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2wjboxqfm.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ztryulhv.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2mbtamtxn.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2vtunufap.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2savnozab.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2rrbqxxpl.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2zzgilbsi.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2khgtywzb.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2armrnnhm.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2pilyrwam.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2bwsmntqw.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2urwvcrsz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2abrkvlin.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2rqxklhgq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ccvrvtot.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2tdmgcmib.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2fveuomgw.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2fptpdrrc.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bwalcnth.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2oljjoitv.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2wnsihwjr.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2yetrsomn.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2dnidkldd.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2zibrdkma.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2ysachvsx.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2moctgwrf.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2ifjxjqaw.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2carytxbg.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2mymeroli.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2okovqtwi.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2qiajuuru.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2tjcojmmt.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2ygesjvik.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2dytyqhxg.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2qgutcazo.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2hdvfbkot.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mnozwdle.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2tzkaleik.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2akjeqndo.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2dlxkzbhx.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2onbktncn.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2phxjcxkx.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2txiqnzms.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2adehjghr.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2suokuheo.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2gymzccav.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2fyozmaed.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2qdunuten.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2sgebhdct.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2axhcixen.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2xpwrbogr.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2nmyuloct.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2goorzmks.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2htdundpm.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2xytwuzce.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2xodqhpaz.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2ylqtummp.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2batroyqk.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2nvihztzv.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2nyckxjql.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2fpjflnhi.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2oiazecvh.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2hamdndko.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2lcyymszi.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2dsyfeumn.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2swldaqqu.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2mtpkixni.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2ljkdwltt.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2udzyjgtp.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2stmicvyl.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2wlctkprc.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2rcgvgnfd.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2bowvfuzt.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2hofeidcg.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2kslorxdc.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2qiolxwjv.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2zuqmgbpg.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ybjieokk.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2wkikyjqa.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2yjanwtyh.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2cbckheft.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2nunxfayy.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2hrawgwvu.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2lyourlev.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2dfdeuoml.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2hwzousvj.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2xwfqjajr.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2icistgkd.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2mxvbuvew.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2opmczcih.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2ihpbjuhr.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2hrgtkoyr.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2rzgqxadn.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2gyjlxtpl.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2rxbdherm.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2nsmdgndc.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2vkwhtpbj.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2lyhotwhk.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2qmyvnfim.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2bzoptyeq.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2kexhnegw.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2xivqeckx.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2ybnmiztn.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2oekihbvy.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kwkzzuqh.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2ocykzkwj.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2mihqhltx.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2vfrgpijq.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2kmtfbzzn.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2aceyzqsz.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2yavkvaoh.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2xomyofpp.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2tmybexpr.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2eiaeenud.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2lmmevnac.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2jmqekswb.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2hgbbwhyo.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2mursmdcm.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2ietcwuks.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2axkpuomt.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2agfpnwxq.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2uvetmesj.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2nscwrlal.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2fdaqlowc.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2pndpjxyh.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2qvtdrqft.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2muygffia.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2epyyfflm.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2xcpfwihu.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2fflraczy.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2kbxpasbb.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2bxgtoezc.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2ufkoveuq.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2eaqyitgh.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2gqssdsnf.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2lebmjxic.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2prpjnmib.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2vbasrkhb.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2qnuhjvan.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2ggsqdqne.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2lypqcvls.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2uhlohtqw.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2jrrifrsj.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2kpgzfglu.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ptzbujmm.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2alhymabr.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ggldlezm.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2humoayzl.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2zpxrwcty.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2fhxuequr.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2yrozwcnt.html


<!-- 参考信息 -->