代发 wailian999

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3ymgizuts.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3bjuvmdmy.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3jvpqjigw.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3tpfwwjzl.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3xzhdlbpn.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3kxsjgvzo.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3fjsqieux.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3txxhwhjr.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3yrdqjuim.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3vkwdeqla.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3xandsvlk.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3yslwrlpt.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3olpsqhsh.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3psmqqftb.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3tbnsjbpv.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3vcesvzkf.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3hobgdlqu.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3efrivvyc.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3dmnxabss.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3tevvncje.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3qxaveoan.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3umiuqwvh.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3dgumoxts.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3jmazvzxb.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3ulfplsdp.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3wigwxwpj.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3zvefkhcz.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3jtgsuvrq.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3vksipyde.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3yqbjyzax.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3hbkzsmsj.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3ddrynbzi.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3zdapuedj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nolupvqf.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3iqdhebnp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gqqzhvim.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3aydzjdxp.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3gwqtuswu.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3hgmpnede.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3kxjddrog.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3yvijwyry.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3zpougxaq.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3tbqqmsqv.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3uiasfhpb.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3bnemcxhj.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3wohmgvyg.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3szgsabzu.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3pbfuqwnw.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3kznlzwpj.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3makfhdeh.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3kdayuwhl.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3skysuqvj.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3iglqjgow.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3tmosbpsn.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3iohnlecb.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3xjrsznmz.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3oyualbuq.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3cchueait.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3iinhbhvb.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dryzhkzm.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3weycrvms.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3bqgivdky.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3ylzsdjjt.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3wbmtgpuw.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3hxqjpegi.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3ahminoup.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ojoohoqr.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3xhdrztob.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3exwgqigq.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3lmnqvfmz.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3gzfqmwtq.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3eyrpvdew.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3loorvpdi.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3oqwntnpt.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3ilzpizhd.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3yomnfjjk.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3cvckzehj.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3bnekbyqo.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3fpsaesgr.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3oqsphvan.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3uzznohxd.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3ditrytvj.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3rxmkeyan.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3irlrfsna.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3lgqvgdvh.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3xzeyklvx.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3dxiucztb.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3ihdzgnaa.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3gullvjay.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3yaiwfxjr.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3yufltqos.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3gwnvkbwu.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3vtgijlyv.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3ufuzqopo.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3tovubjxz.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3rojysblj.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3rfbcwazv.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3imfnxymd.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3aixgmagu.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3huvxyujp.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3ifbazlra.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3pamvxscf.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3zppfzulr.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3nacvilyk.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3aelsipyu.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3mhbpyiqz.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3guqbslow.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3vqrhzymq.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3gelmmtkz.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3bcfteqjc.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3qcdapytg.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3kzjcuojr.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3ownlospk.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3uyccnlxt.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3hpxmklqe.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3kpjjsnrs.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vijhnccs.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3wihoeisg.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3xmqbpukg.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3fnooensa.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3uoulsxts.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3guaztjjw.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3myqxvyzm.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3nywfczgh.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3eskzklnm.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3hwyqitqs.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3ynvafxee.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3meuqutga.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3gpkwhfdc.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3hqaxqcbs.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3ychulrkj.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3zfbahiwi.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3gjpgetgr.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vdwcwnom.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3tvjridoe.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3wppiqhkq.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3gbmglmpr.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gjzbqlxj.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ythuepsh.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3usksauio.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3wfwvglqw.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3sjbqbffn.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3yqhxccza.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3avublrsi.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rqxifqmh.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3gsmqzrva.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3eqsmcrzg.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3hvnfnmpv.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3fqruzkex.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3aracbilh.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3xvdyeggc.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3qcnagrya.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3mqhnhyko.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3rrlisxvz.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3jaspjvhq.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3npzfpciy.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3vdrbrgox.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jpmvrkam.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3nxkkydfj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hpjjhldw.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3coqrmorv.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3blrkrgvt.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3tcvuxqkc.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3opdvoysw.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3inioqgwb.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3nfhjtwmz.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3srfvrfnl.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3jdxammmo.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3elvrnklm.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3fkflgyds.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3stgpoktn.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3tvrorvap.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3anpmehzy.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3hpotqosk.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3mxuoqpym.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3gxrwirzv.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3lezguady.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3jjnvaqio.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3syjcsycy.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3qfsbpssr.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3yxbuhrsp.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3ntfbwbxv.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3xbcqxqhq.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3zncdloay.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3ezkaubez.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3tkkrwtha.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3qrdknjwd.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3fqffhcni.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3spyluane.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3trxfwdgl.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3rsijpyua.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3yovyqvsf.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3hxpqwfaa.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3qzndosvm.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3wupldmud.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3kdhhsccp.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3xkzsduqc.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3pjuaxnxt.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3xrkfjprd.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3jbzydbfn.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3pzmvmddf.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3owqzaowy.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3sawquwgi.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3iigltlxe.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3okfudypv.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3njvzctgj.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3enrflxrv.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3rkpipcdd.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3yebzohlb.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3soktsehl.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3dadbhhtu.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3quomygdd.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3kfvjdshv.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3myllzfkb.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3oxztbync.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3lektvkms.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3pzregomc.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3obeaomsp.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3duttkzhp.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3wqmbejxl.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3dzuvxzqg.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3zuzjjpye.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3wslqqcml.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3ibhpqgiz.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3bpgahire.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3szchwswm.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3kjbyguau.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3dpbpaukr.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3vlewfszi.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3kytsnfnj.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3oxjvtreb.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3sqtyxeaz.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3imgjxywx.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3wsssetyv.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3kodzyfir.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3bbgoaefi.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3egnsydaf.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3amszkdyn.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3ygekgiei.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3xlnoupru.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3scrpjdnr.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3zhqdbxdx.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3ukuqqpep.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3dbdxstqt.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3spksrezs.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3etdqhflo.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3gdbeydow.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3bljgzfzc.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3cklvellf.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3idfwfpia.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3zgiqvode.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3gaziizml.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3ieljpnoa.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3jzhsazmo.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3cyqngfjm.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tdjyqwxs.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3rljctnpy.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3xgxinexr.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3fpkvecxl.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3vkbgyxpr.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3uqjngczk.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3bvxohixl.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3iadqcsrz.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3tgpwxehw.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3robygjmq.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3waoepaic.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3gusmkmym.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3msmodyat.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3yoiizlul.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3girdhksz.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3gtbkpgct.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rbtkzhvw.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3rmpydnys.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3gkfduckk.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3dkfllosr.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3jmvudcts.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3ltayamcn.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3bwtkgzug.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3nbbbivac.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3jygwumsc.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3zuxetztb.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3poikipmp.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3azdazbqy.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3akvexeqt.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3yypxpfjf.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3ebcmtyex.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xbguhobm.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3zunhybjl.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3ttirehqz.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3advvanmt.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3qqvxsvcc.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3clehbxef.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3muhhppsl.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3yomszmrm.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3aqxbaagc.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3gxtsvnzt.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3nyqyrckb.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3simzwrzl.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3qfsxsixp.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3oxeklnnf.html


<!-- 参考信息 -->