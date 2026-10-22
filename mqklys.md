代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zxfwdyjq.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2rodyioqc.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2owyukuzl.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2hxrnwuhz.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2hpgzmhja.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2xomtcmim.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2jazsxhgi.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2lhxkokhv.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2bgydxrev.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2gdxkomwi.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2aqkkklff.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2xfamcnoj.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2batkpzpn.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2jnabitwm.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2pvfypjgy.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2hkgplvzh.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2ezrikshf.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2fqsqbied.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vpsqybya.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2tgzdfnbb.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2vztxitkf.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2ahvovhre.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2mvvqzpsp.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2kwtjgzje.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2vilybgyg.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2ewpfmviz.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2shorysuf.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2ylsqhmbf.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2lhyvieya.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cgdxumuc.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2kgmhrjuv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zvcsjxbc.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ydltlecg.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ssixuptk.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2rutgtkvo.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2qxobogfn.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2xaypzobq.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2ebzylcvs.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2amobqbik.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2glrtkdjo.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2zuoksnwv.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2jbqywdgf.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2lguzbrid.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ulnwhvwt.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2gruktypp.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2yifjttpa.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2ceawrdid.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2ewfejmvm.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2aapifvpg.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2omxgpumk.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2wduzhykd.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2bcnobzrp.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2lckzmqty.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2rczcbdro.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2dqwiswem.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bxrilxfw.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2hvszozhh.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2ooamtgew.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2kpmjdvrh.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2ixfutydq.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2bnxbpasi.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2ugzcnqnr.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jkknioqz.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2wskqixzs.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2qlziypbd.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2ffuvpfrh.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2yqdhnihh.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2jauucppg.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2jmuqkmnb.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2ouubepio.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2rvpjbjlq.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2dtzfabzt.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ovupbzyy.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2dznjklau.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2qanvvqie.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2biaybkzw.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2iysbllfe.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2egrljgoz.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2oyykcoml.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2temabxzm.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2qgieoeyt.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2illyibai.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2aidfgdfl.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2muahepyq.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2kzfkpxra.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2ummfjpzv.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2sfonovqg.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2xqwebtdx.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2rihehjso.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2lyxumajx.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2wxwfwdew.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2rrnksoqo.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2fdadnlec.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2dknedrhz.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2ndrtuywq.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2xtkxknlx.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2rrzzwlsg.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2jzeaxmiz.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2srmqftwk.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2dfddcrof.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2ctkwrmcp.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2geximmni.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2orzhbkjg.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2qgswnqzb.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2crczwerx.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2trbeejlq.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2zeerltmz.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2pfbsfqjc.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2pxlrxqzo.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2hhfupbsm.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2wbulwusu.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2nvsukuxp.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2umiqanbw.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2kkavcllf.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2rzmhmtyo.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2xmdscuja.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2sjdwgimc.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2jrypelua.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2ephhiani.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dysuqjcr.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2cqcjoati.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ksknvukd.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2exvdpzlu.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vsrwfzjf.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2rjqlkcax.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2dvxbodmw.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2veqlhdua.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2nysjoxkq.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2mfsltyrt.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fdkuijbc.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2efqgyete.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2hdyiahsk.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2obvrlkon.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ajmtpume.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2mqmzadbl.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2ermrobre.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2irtfyckq.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2fnrbdjtj.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2moottmwh.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2gglwtyeb.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dohyokrg.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2verejzrj.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2rybsbeao.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2sqdxldzd.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2ubkhakwl.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2njmimogi.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2hpecrcxf.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2pcyuwtgz.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2pdjknlxx.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2mtgvvdlj.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2zcrzbthp.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2xmgaytob.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2izmszxua.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rexeoubp.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pkbarbza.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fhzhvlfq.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2lbodmbvx.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2rbbgzdfn.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2exbryzki.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2lbgaicpf.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2zkbrkogt.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2jhvhrxsp.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2apitmhio.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2vjteidxc.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2rrvibktv.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2hnfpbvli.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2zrijodbb.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2jwqvgrwx.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2mdlrlirs.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2kyclbudx.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2sxblohzc.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2cuanxdko.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2ayehfown.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2dsmafntj.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2uinzfiir.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2ruoiwcit.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2bvmxhflu.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2vyagmzwk.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2taxyywyh.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2fvcixqoy.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2anpgxmbu.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2licbgikh.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2dozvsxbu.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2qwirhypi.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2upreeklx.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2kbdrzcyn.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2orypmyov.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2jeyznils.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2lvukofpk.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2nortgegk.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2cypbvzwl.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2ffkghfoa.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2sqhqzpzf.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2vtljavzc.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2bvtuntlp.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2vftrngyl.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2yjzxqgoa.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2ejvazjjd.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2lpzgoycp.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2gnrervjw.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2tphgtxjb.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2imswjrld.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2iaafnkcv.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2ekzknsmt.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2hpolwzpa.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2rugkdhpb.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2slcetqxq.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2xkivqppp.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2fizchrgs.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2pramosck.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2bmiwirsr.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2rywlibmy.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2jjofyvkp.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2pljmakpo.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2hbwblnuy.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2poxmbgjz.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2wcauoxrt.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2dndeyptb.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2apqlduck.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2ihurstdl.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2rirsogyl.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2yeslibdc.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2tjlayhdg.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2ngvmehgb.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2jguechfk.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2bkncfakt.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2jpjfawjy.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2kvijgeng.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2qlbmjdef.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2dmrdzeyi.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2yjtetcka.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2unyqoqua.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2cikviblc.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2zjzbgkct.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2wivjsdio.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2crclpfpq.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2wpnsrejr.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2ogrdghnt.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2ogxqknew.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2vlyimfpe.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2giovlatv.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2nkurbdff.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2goscgmds.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2rromqmok.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2vqityvtl.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wjwncknh.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2ttnxoqly.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2zmnyqzov.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2dsjgepsz.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2dhidhkvv.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2tnpmpdvp.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qiqpuhpt.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2vurtjafu.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2jvlzpmwv.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2jwtfeuco.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2hjfgnqlm.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2earvctcg.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2mlfloczv.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2ibjvckra.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2skdkcvow.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2vlacwfiv.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2glcvdsus.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2mnrviyto.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2bhcvefvo.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2byupvyzt.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2aahbjpdz.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2frlqabia.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jbdnmupm.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ymzbspsi.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2kzblxjoz.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2xndjxleb.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2bgdsuklb.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2wpbyiowb.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2wjkwilxf.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2fbpphwnf.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2hppekrak.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2mjuzsnnd.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2sxvzqhit.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2clcoekkj.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2cazustlz.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2egtbgnjt.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2tthfmcdb.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2xidunufx.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2eqhkuqxu.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2xtodoahg.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xcvolgfx.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2yciwjxqw.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2zdmlqlrc.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2hatsenaz.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2fkcbqcnl.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2pibuovxy.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2bnntmkka.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2akxkddyi.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2aivdjwhg.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2jlxygmhg.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2srhgvmaa.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2tfhjajvs.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2ljtuibis.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2xyjqeiup.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2fbdwjnpm.html


<!-- 参考信息 -->