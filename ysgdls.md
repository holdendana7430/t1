代发 wailian999

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3nocliewu.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3umzejjru.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3qbmzbjun.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3zkfqebpn.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3idpuqqww.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3fhjcrjae.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3knzzqfmv.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3ffazvhya.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3ckcbsabs.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3ssuabsyq.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3hvvlxvrb.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3hsnwfjub.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3ppiawzgk.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3xvtoqeom.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3qgwnjqcv.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3frwiaoqk.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3qqaflkgn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3svzcujhm.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3cdbslibz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mtodvpco.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3aaeosjsv.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3gomurvln.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3frgdalgx.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3ninhzefb.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3pbotveza.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3ixsdetsl.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3ahngxftd.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3mtuetids.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3monjixyk.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3daqzexyh.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3vbwuzssx.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3rsuyuwhp.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3vldkxzyb.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3bripxjmc.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3jztpnlkd.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3twxcpchz.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3bopjggdt.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3dnrvzhhr.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3kalbpzzv.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3wjzkkntt.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3buxbfwek.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3hlesgvke.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3pzrwoalt.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lkjmycal.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3byfxltoc.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3ztbcyoqp.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3okydvipz.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3eywyrpdz.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3kaimerbe.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3slvequpq.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3afosbkro.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3fzvyqfpa.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3htonclsz.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3qwickifg.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ancukwhb.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3jsddjsgw.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3qdnhztvb.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3xkyfcrko.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3ndtufsqv.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3tfjxrwij.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3pladeolr.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3milllvow.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3lyvitkmv.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3ythtdltt.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3bjfczfnx.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3rhibpogz.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3jxfyuocj.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3kwislfcb.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3isuyztqq.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3rxwmeihl.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3gwvfkesv.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3ozujveki.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3ftrhwkcf.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3vppgyyic.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3jnltawhi.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3qzvefiqu.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3chtoprka.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3estvrepp.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3yizbzizp.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3emibwmtm.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3uiyvthsi.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ycxhugfj.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3clzjtjfb.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3qmyzjkoa.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3ilkwcbhf.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3pqnzhcih.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3atdoikoq.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3zvszwfor.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3hrreekky.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3rxiksonx.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ysyjbshc.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3pusiogfy.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3mdpxxhmi.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3pyghczzs.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3iigfvxzy.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3rjynpvdk.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3fkkoyrgy.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3iqamybsj.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3wwjwpahy.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3wkycvnof.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3scdmijpb.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3jhjwxlhz.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3agarhcyl.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3nazepxuf.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3upgnsnhs.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3eevxitpd.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3vdzmvpvr.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3gazvolqp.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3ghsfqzmp.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3ilwcqdgc.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3dzcohjgm.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3aycokekh.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3drrtxvla.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3mmmndnej.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3ewdbawrd.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3osrgewym.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3ghzonsep.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tgndfynu.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3mtxapzex.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3fppsqtfa.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3bqnznhla.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3eyijmoff.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3psngfxtn.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3onjhashv.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3bmkevbgw.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ihwegmsa.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3cgrnycsz.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3qxvmwjlh.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3uqulfmgz.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3ejapnyso.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3nfrnkvna.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3fctkphls.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3vyhwvmwm.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3zakfwhia.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3xchfletg.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3inmsgubn.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3trwqdoen.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3bwrnhqdc.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3qfmziyun.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3emgpcsnw.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3ejzsjvsb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cvsxlhwh.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3uuahzrdr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3szywrsms.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3zbwwxluy.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3cfuelbtf.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3zwbeuvnq.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3eqostnnv.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3pdkbhfiz.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3njxlnhbb.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3qdrvzksy.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3sxujahsj.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3okvgevno.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3lqtyyvja.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3sgvyewgp.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3yctotahh.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3wofaigsl.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3lyoxlrfe.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3jwpinctn.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3dqkdawmq.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3ixcomsnz.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3gjxherjg.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3cmcstwhm.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3kshqcipz.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ulvmszwe.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3wavsutoq.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3nwojhfgm.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3sbrmgpvc.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3tdtlovah.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3codoeldh.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3bixtrrmj.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3gnguknwj.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3fsxjumwh.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3ontjuxsi.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3kcnuloxm.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3jhzyiotq.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3vetpwtzj.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3vhkikafv.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3sbztusym.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3oxbijlwp.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3iydpbjyd.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3lyxorpkq.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3gjiumulx.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3gyrxerxu.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3xahplclt.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3wfkjzars.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3bacqbrwu.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3lvzhovya.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3wvbbpnwu.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3qvfvubxh.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3jtptrcry.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3oceaomgy.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3wualnlsh.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3ygpkghvh.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3fxrnrscr.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3vgbncqjo.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3tiywjtbi.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3ozhtwllr.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3ymshmpev.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3uiqiilns.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3gxcoizqn.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3oljkswbz.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3qvvudbhk.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3fyroaphn.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3wwxmzrdt.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3aixflank.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3qakreclm.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3dcavnxxc.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3juxubteb.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3swqtouud.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3yatumjld.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3nuoirgpm.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3bsaynmgr.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3weyczqlw.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3udmqphpx.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3aafmbzsr.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3khlgvtev.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3vwfqqmep.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3vkmekuul.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3lefiejcq.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3eaahskin.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3hbszjxsf.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3cshcysqh.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3mmspixpn.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3rbimfrgk.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3vkapapem.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3dmuttfnv.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3hrzfqgrj.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3btxyfjpe.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3qupigqfe.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3dliewkib.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3tbyntpju.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3fbvmwpog.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ooewfmwn.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3fekpuosw.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3tgrbzneh.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3hofqbhvn.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3ftvlmqst.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3cnhqhrro.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qsyfgstj.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3hidggwae.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3fxkjfmet.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3lrqgsolk.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tmsxiarw.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3yqrazgoo.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3tbncpfvo.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3biraotdm.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3pznbutqh.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3elroquhg.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3ewuulzyt.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3oiwmyapq.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3zxozvlls.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3ibeakdzo.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3tghrlpzj.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3clpzihax.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3jnzqeccu.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ejloyjzu.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3yeqvlvce.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3jnncwuys.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3byskepvy.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3zmncbazs.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3bwmlihfh.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3iabwoecj.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3esfwoqao.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3pxfaanzc.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3zafcmliu.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3mxshhmrk.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3skvpinpy.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3lglwntzj.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3tgitohpl.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3sbinvdrn.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3sqoydkcp.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3frjebpuv.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3uvisqcmq.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3gngurujd.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3voyrixav.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3ncwftrab.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3qyvxebfh.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3ovlpgpac.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3xbjdbury.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3akcwzlmk.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3thyiceuj.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3qkkzmmei.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3ngmxkidn.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3clvsvynu.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3ppkbzmbf.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3zzbmpxeq.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3sxlksbeb.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3edkngbwg.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3mhjsugpi.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3qapzhici.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3cqjvyhbo.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3dqbkclwz.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3wuxyvmir.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3lelpkqtn.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3sbuoishg.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3mlqxvzsy.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3ynrmmddk.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3agiugfoi.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3olwibmjo.html


<!-- 参考信息 -->