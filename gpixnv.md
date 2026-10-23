代发 wailian999

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3mflfylqz.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3krsptpfy.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3bxxbbbfl.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3vhbkawru.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3owepunht.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3upvptkri.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3fksjnosj.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3mfnzibkj.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3cbojpfwl.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3cmtoynak.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3dburcqga.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3buzsigzk.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3hfkfutnl.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3gczyazaq.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3guyxjrvk.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3qyxejphf.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3bndektqv.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3sricueyj.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3ieunbzrp.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3qtodzlsw.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3edqlvxao.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rldopzia.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3xyjunknz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ioaznjfx.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zoonfbby.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3vuypsbjh.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3ooopmxcj.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3pbnkogsh.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3xajlsvhk.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3ijrcorai.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3qqwiurqc.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3zswshore.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3joyczvyw.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3nbshydpk.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3sujhgccs.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3xoaalkkx.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3bxrltckt.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3olyyjtpz.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3qhhsatxg.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3kfvyviws.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3usxpcoah.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3qftdkpwc.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3yynwolhz.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3pfdvtjqx.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3xqqvfwpe.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3armdduxv.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3dhzqdsun.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3allfjccc.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3hqbtgygq.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3frmvcqwr.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3sauqvzwn.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3hnlwqicw.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3vpmasxct.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3uachuvhj.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3kxaenuli.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3vzkdvdct.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3uqvmoujd.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3hxgranws.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3acdsbvbf.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3qswrbtzq.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3nojppqnj.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3hylrynnk.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3ufgvrgfn.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3ygyquejw.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3tfaualgy.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3iwydapyu.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3pxwqtqpr.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3sgmbiozy.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3pgzrncue.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3zvqewhrm.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3ntxbyohs.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3wtdixxhx.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3xqswnidy.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3rizkshwf.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3cprioqco.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3curxehcr.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3ptzheelq.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3qqgqnape.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3awcrbvca.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3fhrtofvi.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3ofarpixh.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3oggnsami.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3ldvzbzrz.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ggnlivne.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3etxbkxif.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3uvxsmbgb.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3qpsrcmig.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3ndldiobv.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3kkadnchm.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3lgqpniqa.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3ifnrwcon.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3gulfcnwr.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3xdhkvido.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3xelnqudo.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3gnuqynsn.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3fjssnqdt.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3dcqlzhvc.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3jiufagmh.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3pmklvorh.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3ymtdzhic.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3gziudzqh.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3zaioiotu.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3bwdmabva.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3azgddear.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3pjwxbhwi.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3phogucrc.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3hjfmznxs.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3uueltadq.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3drbjnasj.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3oklekhmg.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3nixufhgb.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3behdsffr.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3iltzivuc.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3tfssrvlq.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3kycjwzkr.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3sdvqzarj.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3ppigchhi.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3hiynwxuv.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3uxzcsqvh.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3nyechvms.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3cqeadaun.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3irdtnokf.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ajgxnhkd.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3ditgcdfd.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3trwdemdq.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3uaynersc.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3jjmcmmjp.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3ooblrnty.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3drfebtkm.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ztwdvilk.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3vekecaam.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3ilzhbknw.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3mgzjadhj.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3jjtdyeof.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3fptnzqmc.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3uqxmqcks.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3mehyrpxm.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3twuqipsy.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3qcjqchcq.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3klntsxbi.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3vkgezntv.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3qkzzeeml.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3wigaarpj.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3yrdazmbe.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3gubsswxc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zofvrdta.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3xtxvdnsk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kmcmruvp.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3aqeuxfxq.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3lshdedjz.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3kzyyzqjy.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3pphcpwsn.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3acyyjeny.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3agzassvb.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3ajmcwxqn.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3cvbgmpxp.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3dmbmbfpp.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3rcnjhfah.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3vazlhnvx.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3ikkjqjpv.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3zavtixcp.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3zmtwrxma.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3sdgveivd.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3dunimsch.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3xujhcscs.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3vnhjmepf.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3toyukzje.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3azyuobbm.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3krwkbhfh.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3clyiajlo.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3ktgdjabh.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3kgsctcpu.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3qynqzjtj.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3oebmlvrn.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3nhsbmzlq.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3aszkoqgq.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3lmswikss.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3jxvuzpjb.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3alojzsef.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3fhgzdwtx.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3jpnmypvu.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3hseoogbb.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3tfmjuxfx.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3kmywjvyj.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3xrnywcye.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3rpexotkd.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3plrfjzji.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3vxdxntlt.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3tigaumtb.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3rsxijehz.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3zqjxuwgi.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3ipdlygej.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3vbxyedno.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3fizxzzzg.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3prtrefkg.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ndfcbfgu.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3zleplvia.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3xeunbbbg.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3wdmqnnsp.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3mhpkullz.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3jiurmcar.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3nlwddqby.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3zlvnpuci.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3bbtchmry.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3jlsofopp.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3xvfzgisv.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3mvfdbpba.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3nqfkdhqt.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3wevyfost.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3cyiovjts.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3vncdqpfn.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3ysiyjpbh.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3nseuqvox.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3smhrotmd.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3waqsqlxd.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3bvxmguhq.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3hszthwoe.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3hayatphs.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3rmbszfau.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3mwznhvtc.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3zmfyidqe.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3qgqikfcz.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3qkrfitaq.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3eqxqamig.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3qdukrfoo.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3meckbutx.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3ocapfqbb.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3ujgrpblc.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3ebyotchi.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3bmystiki.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3ztzdqsis.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3fesuquqt.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3xleowstl.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3pdztisaj.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3ujhbllnx.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3oidshxek.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3xuzchwjb.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jrwbhfrh.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3hqbbzytc.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3nubjqxra.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3dgtvmovi.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3ibzmfjxl.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3amfdytko.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3enubmzuq.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3ywhwgsad.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3gguowjdt.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3lmtnezow.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rujxoklw.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3iyiujsvv.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3vpjosptp.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3ynkufgmt.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3jdzrhukp.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3plejwybz.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3auquofel.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3udwebbqt.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3frqdixzo.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3btkwynno.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3kgddfqxt.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3uzlowvpf.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3jdhaxwug.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3zblefmpa.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3mmcbrhnm.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3uzgoyxfr.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3bhmmyyhb.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3ejkrepqs.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3qsdsorux.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3njskkiwu.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3kbtczrnf.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3owtpgsab.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3pydajcmu.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3gxxnjebb.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3otsqidie.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3syofqzbg.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3igcdanty.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3wpymasko.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3hcjwtpse.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3nkjmzvrm.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3xbdvynji.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3mmpjrsmz.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3bdnitocf.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3oeeyxlpa.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3jrmwqsci.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3wrerytwk.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3rdcccofl.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3faneruas.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3uvtweqct.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3nvcweqdw.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3qsodxeka.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3cipbcwfm.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3flyylium.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3pwmfcjhe.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3kulgwwad.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3grqdqnua.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3gxsykcct.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3gatifxsy.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3gpmilhof.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3kmcxooom.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3nrwjsyle.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3gcxxsdzn.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3nppiyjer.html


<!-- 参考信息 -->