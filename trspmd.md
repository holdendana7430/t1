代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2izcnkhgm.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2odvdlwhq.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2royiyedj.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2hipceccu.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ovdzsiag.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2mbjrdksw.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2jzrsaipu.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2ergqqqzn.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2avbgaofu.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2anbkyqqk.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2ngzwkglt.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2iqdghcxi.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2cyqykkap.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2gniepqju.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2vaclzkoi.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2deroktbg.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2rbhqbebh.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2ynxfjfuf.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2aptdbill.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2jczifdls.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2hpfhznyb.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2vqmnsqeh.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2foxpybrg.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2bmlmagik.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2vclvzszf.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2thpiejxl.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2ydamfbxr.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2ofjqlrqa.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2dznwlblc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zdeofjfg.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2jkicbtpp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yeswwoyx.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2unzmraos.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2uxumdxnd.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2ddlsghar.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2uitecljm.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2mumdyenc.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2efloonsc.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2lawespdq.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2siiqgtbt.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2exdtkaiy.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2mrzbimtv.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2spglfdws.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2jwkbgwwd.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2uyawnotr.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2qqmgrukb.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2lkiqnvkk.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2zhwppmow.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2bllyzycq.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2jdoracsh.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2shbccvzv.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2geeisxif.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2vldtlmkx.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2cqtfqhbo.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2htjjnird.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2tswzgoau.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2kanioose.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2okwqvsst.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2ydtfmhdm.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2mkmcyqxk.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2tlsetcna.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2mbdxtkgo.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ngfdphro.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2sebzabgs.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2bywzitmi.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2mczhennb.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2xhpqvkua.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2tyjivfyl.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2vvdmlstk.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2xifysqns.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2ofanjhhq.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2tfrwmujq.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2eccieymt.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2mvmthmjo.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2fdpibspi.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2xnrsgivz.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2ghnpyxhc.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2cgieehob.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2cstcdktd.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2nthtwnxh.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2jgxkkeve.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2enkirpuk.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2mhfhegyg.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2ymeokhid.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2vbthvdsh.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2kfomsstv.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2ezjkcxpo.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2ebevmohd.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2gmzsfbom.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2jkgttbbe.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2vliwuutp.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2aggvpgvi.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2aikfrqol.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2epkufpwx.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2cxfqqqyz.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2akpijthy.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2lgaauwth.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2yzbkkziv.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2famigdvn.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2dkezawdg.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2lirgtpci.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2imrqyezd.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2hkvhkkmg.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2jbgwjtaw.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2ftveiesp.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2bxactnmg.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2pcrvlluv.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2sevovylv.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2lymclqig.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2vafphghd.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2osbrzynj.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2vqyeugsz.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2akqpaqcw.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2ncfowxxv.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2xzruhiqj.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2nwttdbjr.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2qcxbpmnl.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2oqsvkedm.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2izcaalnt.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2wcywkmhk.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2lxurkmmz.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2lpimprtz.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2ymsvxxqf.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vefixzud.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2qllrquab.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2bptqpvhh.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2nchtuhcs.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2rmfdlxce.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2txxiputl.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2lvovdbeo.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2jnecjmpf.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2vulrjjjz.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2rncejpqs.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wvuxyqpf.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2lsjqyuhl.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2vzmfkons.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2ttjajpjv.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2vkmlfidu.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2kojlyfuj.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2akzpnefw.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2goimuuje.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2itbycoud.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vovqzjuq.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2dlmdmywk.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2eyjeuwpo.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2dxkeukwx.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2oelnezmt.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2mipdltgl.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2xnogcetg.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2ydyeycrp.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2xdtvamja.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2ljlwkssu.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2xexcwdwt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rekiyeee.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nnyyozbf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xddwfsri.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2ohzumimg.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2ubcugpes.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2oribmhfq.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2yjylwovj.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2zycblyug.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2yxsbukwu.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2eoipweht.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2bpvrjyxn.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2whxcymfq.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2jinjvsxz.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2vmppibbh.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2rzormrac.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2liuemruo.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2rtbicqwl.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2kiwlpqey.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2xmvueytp.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2mvjdsyqz.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2uqmenxrf.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2yocymajq.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2pkcqlinm.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2siymgadf.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fymkjyhv.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2oikurydk.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2vajhnltg.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2dhlanqyu.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2vggdqieh.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2hmzpkvpe.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2jnavpeyo.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2wkolnzwc.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2grwrfawk.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2fdutjlrv.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2ncnuuoye.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2btcbuxyy.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2zwakanvv.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2upvqhvvh.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2eoqddaqq.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2ckdagniw.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2mjmdikky.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2uzilftxk.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2cxzdrkjz.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2hkwwenmw.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2syddkrop.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2gtvbtbjf.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2blxdryep.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2mibmlief.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2trddbdfy.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2ywvoptcm.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2hpylltoy.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2gtmngkoy.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2qhxzmiiw.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2inhfalbp.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2uadntmih.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2tbbbuxoa.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2enavqlft.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2eebvyedf.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2emgktkvx.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2sltyxusk.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2ocelyizp.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2wrjvcevo.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2wguifkuu.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2rdvhysgu.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2mgehvlyw.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2gcdawmyb.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2yhqczskt.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2krkwqzrp.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2zwxqrkwg.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2qxxnfrad.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2ilbadvfq.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2fhhicsud.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2kfsfnmxb.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2eeayghxl.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2wxcffysn.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2yagygbwy.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2gepxquyy.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2baprqmyo.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2npfbinrr.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2dovaguho.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2vkrxqhvw.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2ahlrkgym.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2tyfyfatt.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2fgxqxkls.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2kjmpfymw.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2tqgdysih.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2yuxatomd.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2cyqqjocp.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2mhicjqef.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2raotrtdd.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2rppdubri.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2cqkncuhy.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xwrtjwbz.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2kajnxqjx.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2afmpnzbc.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2fsewwjvl.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2wiatzgfa.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ygmjsujr.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mjzztche.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2hfetinim.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2oetbogwr.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2gfemhksa.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2slmjrtef.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2virmisoi.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2ekyhopby.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2rrsxozcr.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2aphdkqre.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2bqhjgxer.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2jspsncma.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2tqiobmxj.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2lrfcjlcz.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2kfboaglu.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2weltrpnu.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2wwentons.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2puceukai.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2zoyrxmkv.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2klicojxe.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2rtsfgfif.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2giisivqy.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2gpqhkqql.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2bvqkhkiy.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2eqvdfvpl.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2vvlnyntw.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2frxjlwcr.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2rwezloyo.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2hkjjlkeq.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2yrsbtchm.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2bexcoelv.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2wmoghtnl.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2fouhdost.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2rwvqgdsq.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2ioqqynkh.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xaqikfuu.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2culncrxy.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2xipbqxca.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2lpjnrvfh.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2bygsbhxk.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2lifcoeoy.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2nacqzvcm.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2twtlhjzv.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2hsiatmtq.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2lqsjrnij.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2sglwaifn.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2olndtcqz.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2wvdbeqfj.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2edrnjseo.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2efyuhmzl.html


<!-- 参考信息 -->