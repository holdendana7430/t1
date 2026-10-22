代发 wailian999

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2vcgegeil.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2rhaxgstm.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2mxlhsbwo.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2nmlwzxxs.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2zryzliwo.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2fozjbyxz.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2avvvqqca.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2wmjvuwne.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2fsylhynp.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2vmvqltfa.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rbvzflzx.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2jfdhpanf.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2axfpritv.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2vxfsqrrh.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2nmnrkblg.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2cnsdxpes.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2khybmclq.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2hayrikll.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2fhcdqgpj.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2mvzfjrsb.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2dhbmonoa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uqvhsodt.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2kvrliyck.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fkmwwmwp.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2tggzxiuk.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ztajhkpw.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2rkyejdjw.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2lbniclei.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2winfsrjx.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2ivdeztin.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2wlggqgys.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2myzzoqvk.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2kyfcdxiu.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2vgytjxon.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2xydwdrve.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2mlsxocpz.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2gimvdwkv.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2hqpzmzpp.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2bsnjkvvx.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2ttgkgvis.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2iubshpsp.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2bpdslmpa.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2xpscmubb.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2pvtmxlbj.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2khsydeoo.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2ozozsijo.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2ynscleem.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2nqpduqaw.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2udmubcjr.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2hmgroygq.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2nqptnkmv.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2vmgnpfwq.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2kvyljmom.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2uljfxxrp.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2encmoicf.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2sevurmqk.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2bilnaxvh.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2gbljdvzr.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ohwipelj.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2luqvyixs.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2ktmnffmf.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2oodbnlcs.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2kdilikuq.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2qrmlshdj.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2ykekotck.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2udxdirjy.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2pzeayvpc.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2aalvewuj.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ololeduc.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2taqutswj.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2toubwiki.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2qifetasq.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2xeulaqek.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2wtttgpel.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2qllwynif.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2nhbltnwm.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2gybzenlw.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2jlzzhnpq.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2xxyupbmg.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2ukroenhb.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2qynnofkl.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2oqrhykdv.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2whrolxbd.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2nnzuydey.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ngzgpgdz.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2xhyyhwnz.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2qnovopsu.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2lvuorrsa.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2vcizzije.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2sgjzqbgj.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2qxoebras.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2khnclyox.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2qchlcpgu.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2mkrdjbsm.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2mabizybe.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2fnifmepn.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2linjrpfi.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2ahibfoio.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2ypbqhokx.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2esnwjwhq.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2mvlgkeuf.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2krdkmyqw.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2ouxkbxgm.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2gekgkgyi.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2pgomfzry.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2mhnzxmnz.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2grlnobde.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2inmgqxhr.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2mmszczkj.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2yrhobjxw.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2kqsflnfd.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2ornbysuo.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2pvmivsaw.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2rwsrhihi.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2qtfghzry.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2xegoodvf.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2nzrwkgcm.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2kibjwrzt.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2apgtmzoc.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2rxadwcsx.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ggwlfkll.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2wscryvpq.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2pppddpxn.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2ccotuecf.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2xjtykekj.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2immsfbek.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2sgdgextf.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2pkxlrceh.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2namkipkv.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ieqgycve.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2qoprugaf.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2rwlgdbkr.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2akglgzwr.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2muviptxq.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ctgwhlai.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2swpzmmnx.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2qexbrdiu.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2llbyoknx.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2qqtiloon.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2dwuwfozw.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2vrrduhyn.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2ybtalkyw.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2vibtdyaa.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2relqcana.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2wvxfkrxc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rwgzsykg.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2enjzivrk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xmwerskm.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2mognjzfd.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2npfsuqch.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2moruxvtx.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2iaoiswei.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2vryyqhxj.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2qdzriqcu.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2rajquvvh.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2alobrwpa.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2opclxmqf.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2cnhrrurs.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2rqtpwtwt.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2ihlpsxxf.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2uhnvhzrk.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2lmjrjnug.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2ateudazz.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2dtepezsn.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2frizinvu.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2dgpoaraj.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2mywtutph.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2fqllgkbo.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2qwvhyqal.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2gsavkdys.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2sdrcoxsf.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2gazhjhaz.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2irtrnbpx.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2ttvnvvzv.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2gpfajraa.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2yiokpufs.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2nmvbaglu.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2ruzaeali.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2vypaqyfs.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2bczsinbj.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2ucsjwlaw.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2qlkcvpcq.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2pvbpilqv.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2gzrsmmyj.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2naarsqdc.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2runlrebl.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2zgocbqvz.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2hjxqkjnw.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2vmkbtoko.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2bihfbbfl.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2xxcvkylf.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2sflpnkkh.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2tkpjfnrx.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2ixhbdqio.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2ambxwfub.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2czluzlmw.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2vojandwm.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2jojhzrks.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2nhwxumdq.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2aejffkjq.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2iqccrzoc.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2mxipapgg.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2xnuagphr.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2xmtbfqdy.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2idmhwynn.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2jfqwdkhh.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2ksjtethz.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2wcbnoqvu.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2otsonynf.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2pavkaiwt.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ifzehgdi.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2exxtatnc.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2qjgvzngz.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2hpxpzdwy.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2vlzvvgei.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2newfejyx.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2ryvzxrhy.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2vygsejxw.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2fgndwdnl.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2ilxweyrn.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2iwguwgyt.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2hiqdukat.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2veasdtqf.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2spskzfiy.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2mbzizfms.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2zlyvmeso.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2xdockmak.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2kogvcjzi.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2halpcybv.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2tvxtjozi.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2svuxaydq.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2jzosoquh.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2ovjdrjrm.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2hkujauni.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2teeqorbu.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2vfkiitky.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2zvspjopb.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vxccduud.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2kqoktdef.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2cllropfc.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2knnrvqzg.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2tkmawdwz.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2lageioqf.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2eeinrgqd.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2dnqgmtka.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2qzosemyg.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2xjiunmyq.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ynklgjss.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2xmzuqjan.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2jcmxgcji.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2gcrsaixt.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2tfqpezkc.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2hewvaiea.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2hclgaxmg.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2dauzoqxs.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2ahjnwdga.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2xibpkwop.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2qughceeq.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2ivmwwbbl.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2aqsytuse.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ljeqknuj.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2xviyoarm.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2vgjromha.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2awrdxidt.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2nfsiaval.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2usbvjtdt.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2klbsuxis.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2ejcvtdow.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2xewzklxb.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2sbexbmad.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2nwbidefz.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2mxdjkrgo.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2xkjxqdnp.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2iodceqap.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2rwljvzbd.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2tedsjfhf.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2dugrrzef.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2qbsuoqja.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2kxwnlrkj.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2nmdgpdog.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2zlrrdqrj.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2vitzntok.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2udjztcth.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2nqstmtqj.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2ycozvhax.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2yowvtpcu.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2brepjyqv.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2altqlzaj.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2xprzbusl.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2zlkdxhuw.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2jxnvwahw.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2kwngsqzb.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2nvkxbdxk.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2rsdkjlmx.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2ksxcrtmv.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2ibzpvxoa.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2qhytoyiq.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2isltqjzu.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2dyxjjhmk.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2vjgfntwc.html


<!-- 参考信息 -->