代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rqujxzyh.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2tguzjase.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ltowialm.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2fibvkxeg.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2pytuxoto.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2dnhoxmgz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2amkxjauq.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2mnfyvvhs.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2fzmaowyf.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2hnhzyjxo.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2jqxzuawu.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2weputweo.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2jwyjzhuu.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2jvdiedek.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2lhthipfw.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2chdoqfts.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2ftjlwgsr.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2ehdxavpk.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2bduqwwlv.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2fjkmbgqj.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2hnhaytnr.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2rwpgxapx.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2akvsvfna.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2dlnzunai.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2dttvoaek.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2fqeclygq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2knmhpend.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2maxwnjyc.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2tpikvarj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cwrrljhh.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2wabbeaki.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ixsvzdoi.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2egjycrup.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2trihjjco.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2yoptxsyy.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2rwheujtg.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2giahmrja.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2uuplntqt.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2oqcfsinx.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2sjaqpjfr.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ymlnqydn.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2krytdkum.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2bzfwwufn.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2qbgozhhd.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2dlghjqcp.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2zdzzpufb.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2ndiowviy.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2ocvkamio.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2ntkvdjdh.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2txtvngve.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2kzmtvtme.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2evfmllhk.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2igwddzzb.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2epyticjy.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2nfuqhtrq.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fzqdugfo.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2sophabuh.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2thoubuug.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2oizlwrzd.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2zoqtygou.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2czuvlqbk.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2qnjhqubx.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ppsiwyxv.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2qydvazqi.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2vytrigtm.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2nihwqsuj.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2eweaflcj.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2cladewkv.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2ayeqnyhy.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2iuaxjfyn.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2vutumaoo.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2oqjakgry.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qrymbwmb.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2uqgwnxox.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2hbmxrokx.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2hcthewpw.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2kucovbzf.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2isdkbogm.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2bgnzjumr.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2kpgnlody.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2ubqpflom.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2vsfauiiu.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2gioccvct.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2iwrinido.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2mnyzqmjm.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2bzvvfdzb.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2hnfuckgt.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2zjyfccri.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2ooiurstk.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2fkmxvaap.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2cuowwihz.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2gcesmjvr.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ebqsxahz.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2vrpugqyv.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2vhrwoifl.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2yowohcur.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2qogndjuu.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2ixaqfjdd.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2vxvedgqm.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2yzizzzkk.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2bqyzavgg.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2mecrqzdx.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2xtgejuqe.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2zkbwtqlz.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2dxqznbck.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2blyrkukr.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2jvlmgbui.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2haxyfhzs.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2kswtutxw.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2hfsiarsg.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2cgtykglc.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2yhofqtqu.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2pnxuuciv.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2wacuajss.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2qhcgvzqi.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2rtzzhvng.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2itaqtasz.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2sgadleze.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2nzznwili.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ildnzxkf.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2laldovpu.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2bxjumiso.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2fkcbchgz.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2xiaietpr.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2pkzhnigl.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2lmkwliwp.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2dmelwhuw.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2jktmzodf.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2npeuzcic.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2cmettkte.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2hgkjnfkh.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2sfzdyxyt.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2mawpxxop.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2gcnotynl.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2eloqdzmo.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2ywqalffr.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2tnkmjpso.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2mydmjrux.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2nefjezac.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2fiflavcp.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2acllurce.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2cfvbnxcq.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2ywwcitgr.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2pnbgspyf.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2dilarvly.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2klipqqyz.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2kilgqgpy.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2ywzmqvfg.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2sumygjun.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2olabnfsj.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2bacgaddz.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2nsjyknfg.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2qsvljisa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jagpatrw.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rwlevunp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gnylsevd.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2qbnnbocd.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2lmjpqedk.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2ammdqrql.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2owegxhxf.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2mzdlwgin.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2iwqhmhvk.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2cjwkmvoj.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2ecaquchq.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2ukojqzbh.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2hpdbbssd.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2gzcivrgx.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2howuscgp.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2ktauwjey.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2whxothyx.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2udibiviy.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2lsajkfgq.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2iafwzgkr.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2hvgcixgr.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2brlffvzw.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2pssuzrbh.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2hknxbbrs.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zsmkglvl.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2yphokdzb.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2prrrnvqa.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2vphbfvor.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2umzlqtco.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2hthwencx.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2ijdtydsu.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2klmnabay.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2thnfxdhp.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2wtgtauew.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2cgcnndkl.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2jhrscnkm.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2hwjhxdpp.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2hfnbzfkh.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2iavsklym.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2lulrlwuq.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2mfnxmdja.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2xnxkwzcq.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2ugomlbqq.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2mwuoahcu.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2jmpaekbo.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2qvjupnzv.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2ugpampio.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2wxpxruzl.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2pmchhzvo.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2brwznjkr.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2awwztywm.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2dhhoyeyj.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2qspiaehi.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2uakrgrgz.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2gdrdfwom.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2uzwzcwec.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2tytbpypw.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2ifeaifbj.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2fwejwcnd.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2iigpmhuu.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2lodwfvgz.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2lystzpdh.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2bxezqnpw.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2adcuqklc.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2xccvewjz.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2fxrarjgd.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2xmylcuht.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2ceyfcbhe.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2sxwriqwx.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2awsqtroa.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2nfehgiig.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2aviakbbs.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2zptpedez.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2ibfvbhyn.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2strlmvat.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2dercjlch.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2ikrqrtmm.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2sqdwxqvg.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2hzmsrkbm.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2qnejcxgv.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2kpodlaws.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2tsosudny.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2sbpbvzsf.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2fipaufwt.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2ryibexod.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2sokzzbzg.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2zqognfak.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2myxohsag.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2jzfghlka.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2fnoerxsv.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2ivgphvsj.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2ovrgdlmg.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2vehukdpy.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2xuslbrja.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2vlxoqwuo.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2nonfmvzg.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2lrevhyqx.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2xesmrcvg.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2fsurwjae.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2deqlndvc.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2dhzxcnsv.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2jdzwoxxp.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2olkpoycd.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2tajhfgxq.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2xwubhaca.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2oylpfgix.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2uppbmpvw.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2haoqsbda.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2oxwhgrln.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2qoqsrsup.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2ibvyswmo.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2yhsuvwca.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2ussquxvq.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2deemjasn.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2tldugpyv.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2fjbyqtmy.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2ztkwcmpn.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2vtciyobh.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2hvuqoqii.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2uljzbfnk.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2deteskzu.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2aekzvfxs.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2uiknlwpy.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2rqbpntnj.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2yrmglxus.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2mubyslvp.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2ngcyarrs.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2wiiwgggu.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2hchieslm.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2fhltgbxe.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2mmbdofnl.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2xfioxxen.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2opzhmgcr.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2ubzjzksf.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2luoeeeqi.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2emlztsmy.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2ekwlktfc.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2jzbznvtx.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2mtovijxk.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2dlpnsehr.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2khjaonwx.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2kigrgvle.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2kdvcrseq.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2qzfmpjkw.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2lnixsjqu.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2gjvftfmk.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2eqcpjwli.html


<!-- 参考信息 -->