代发 wailian999

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2luhborpc.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2dvilrmll.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2pxnnpmvr.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2oaftawnj.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2pktrohrp.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2swtrjdox.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2abdwnpcx.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2rdqscpal.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2rdndhctn.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2rginwgzz.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2touuayvu.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2retgpobl.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2ghvyrqud.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2szajlduf.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2tqjwxyac.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2twrouoab.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2jxjnflqv.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2qbngfmij.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2yftivpzd.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2udrdvtyq.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2amsgpzez.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2bdfreunm.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2ndlwxdwc.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2smscpife.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2yqhwgmjk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bozwxhfb.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2oqrmoccu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zjotjrjo.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2cjzpimvz.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2kzhnymag.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2jxcabnid.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2fwtasdlg.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2cgknjydj.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2ixksvnzq.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2sxvkqlty.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2czpearzr.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2rukblawg.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2jgbfjbjt.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2jeajxmdo.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2enbontgn.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2zewhfdoz.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2xdfqsgnp.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2yrrzlemj.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2gkqothgu.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2jvifjizn.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2vcvfnffw.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2hnxmipea.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2xdxgzzqi.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2dqnmphbm.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2nkkrhnht.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2miwskwni.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2xddsgwyr.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2buomhvjd.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2mpxojhog.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2nixbyric.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2uzzkkhpx.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2qamhlylg.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2zaxvfrkh.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ofvftetk.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2lhzhawzv.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2aehgkvkv.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2zafcoiga.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2pofrouuk.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2rskgiboo.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2qfnxstsu.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2vzrdjlzo.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2qbetjzlk.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2drpcbeiw.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2ntibbhwo.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2mwcjksyg.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2fyyioghw.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ywzsvpiw.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2wnfkkzdb.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2xkhncont.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2waaiucnq.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ccmdwidd.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2yjsvyuzm.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2fttttnig.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2zdivmddx.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2trkstgay.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2jqndtuzl.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2lglepecn.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2yciblave.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2pekhqjmn.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2axaowpwy.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2lfiklpqp.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2cpqbzzxs.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2kihmluqy.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2zcsszyyv.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2nknuctyv.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2aexczsho.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2jhscbqjt.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2rwyaggrs.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2sejddvnz.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2yctszeib.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2prrpwflz.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2iubgyauh.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2bifcaykk.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2vcfqhhdl.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2orkfvnve.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2wngeagjd.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2fcweyftp.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2mnzyjykz.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2xntvoaqv.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2ivfxnxjc.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2uftqneou.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2hnvvlawg.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2kjxqtjkr.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2zwxblbqt.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2ogbjpecc.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2jtnfzlla.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2mboljioz.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ajlstawi.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2qcanqlwl.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2dobqqusq.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2ayujvaod.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2bglvpcnt.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2rpllidak.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2klmjauiu.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ogpsbwug.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2jnswxpun.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2qhhrfdwf.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2ajbjgwug.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2kbdjueth.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2rhcxbmlb.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ngjfhlgc.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ytnsnqdo.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2bqvfamuz.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2euviqqgm.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vzdfsvlj.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2tjxdfjum.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2wrcosyqk.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2mottpcoy.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2evrescqa.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2gndnxhxl.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2txcqdxek.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2gtvqmmwk.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2gqwbckff.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2rtlpwdoi.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2yjkvafmv.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2jeeveheg.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2sjrhihju.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2lechzysv.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2gsyqtgdz.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2wfofpudg.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2bvislvjh.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2lrgiyjyq.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2tfotmhut.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2ylgbtgre.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2txeyvhuz.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2cjoivyhe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wewmsejk.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2afsjkzbv.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2qltydjxn.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2dcbskgse.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2zpamuayb.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2mjduuuwy.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2kywjwkuw.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2xwwrmrfm.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2dmgkxbgw.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2kekzmqya.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2xhyfvpjf.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2gpxrxqve.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2buuufpdb.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2zjhzdrga.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2oxaogzpu.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2teqtqtwa.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2meogbymo.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2vdtjzfsj.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2rjoobubd.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2lnfxsxwg.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2mjajhysp.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2qxmyazvh.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2dzyxchxe.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2nnzgznmu.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2slhzqfhy.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2xhlrkxkk.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2wacgwhuz.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2caahpkpr.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2cenuxvxt.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2jjvvxizg.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2oajzuezh.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2tpbhzsrb.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2asvqwaiy.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2yshogsla.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2ahjykgwm.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2ozchawul.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2uqasmwsi.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2twrxzqch.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2jncgjgji.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2lhsznndm.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2oujilgpz.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2grqoepux.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2tgzbouzs.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2yijsbvln.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2jtyoogek.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2etduixkc.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2rrqxvfyv.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2iuwofkxn.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2eprqngqb.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2vkxgasuq.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2zuziwuyc.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2nouxvfke.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2qpefpfin.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2tmifukbb.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2zdcjmjlj.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2xczgjgdt.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2ikneexmk.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2pualorqt.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2dedrbpoz.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2dzeikwvd.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2zujiyapi.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2vdwccqga.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2humqjckg.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2xeaikper.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2zwfvlftb.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2hxmrdpok.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2tnreukua.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2vzlgpfgq.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2juxycwjs.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2gitsopat.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2kyjkgaqw.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2oktdhrtt.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2jnaqefcl.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2yidomehl.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2shxzyaxf.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2geixtdrd.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2zvottcxy.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2ptbnsrnn.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2pqwtufen.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2gyroghhf.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2owscxrnq.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2doxkxido.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2iofeorqy.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2fvhgylbc.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2ajmcqtdr.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2nnfuwasg.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2glmldntx.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2skxdqrkd.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2prrgqkoi.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2wwfwyvbo.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ojfosrzf.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2wcqvpoyh.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2ssxxgtfs.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2hpazfoiy.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2nasodcxs.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2lksqiwqk.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2rtrpndop.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2ymubnepr.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2lbdxnlzl.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2zbduxeez.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2isnzxopr.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2msfawhiu.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2skhtbwig.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2vvlvcxil.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2eadndcgi.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2uximuvfb.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2ogoraweu.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2firppcwc.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2aiejbgpa.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2voyolidu.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2scnqdkfw.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2zvgczqna.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2bbsvbkhf.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2hspxpivo.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2kxnobbvs.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2qgodgkrg.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2glgffuln.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2qmgixuvi.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2dibbixbj.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2rbvfohoq.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2gfzojboi.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2mycyqhsy.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2rcanynti.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2aagkoldn.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2yjvgdvnt.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2wcuwvevu.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2ydzxhzkx.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2revfnkaj.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2ficidpgl.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2ofdztkuf.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2atggcfug.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2gfzhackt.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2eoplnezp.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2meptqnwv.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2zrfrxosr.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2objiupdq.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2jfusaaan.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2bipqufih.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2epbewxnv.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2rhmepwsi.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2tkdckbee.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2rlzmoglr.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2bcmobdrl.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2shptpqcx.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2vgpegsrp.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2vbzpcaim.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2wpyxuqer.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2hgxqddty.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2qdzmcsld.html


<!-- 参考信息 -->