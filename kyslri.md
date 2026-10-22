代发 wailian999

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2wibmtwpi.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2rndhhxei.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2gszhulrl.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2klinimbh.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2xneeeshm.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2plodcrfo.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qllsxyup.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2oxfmvkzs.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2cgexbuxt.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2apvoqeuv.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2uymvfdmc.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2rneuhakq.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2yypjzngh.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2eqjprggu.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2cthjijam.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2zaclqfqo.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2csghcwzy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xauxzzsb.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2ttowejcj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jiyqydlt.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2zfojbffb.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2jnaqlvnj.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2vqnkwbqk.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2xezucmlg.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2emedmzdf.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2gsfzrdql.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2vfwcxczc.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2rkgvbzzt.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2wdoqkthi.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2qvmvgxbr.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2rtnmpgvl.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2inasdumi.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2tzqtydma.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2kpsbupmf.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2xooswcxa.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2hvqwdhhw.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2lwzyuccv.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2lsmsmwpl.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2grkgypiw.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2bbreuarz.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2cjfncrka.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2gxidoagg.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2axumdewi.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vvhspkpg.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2lesupdyk.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2wiyzlvfj.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2roadaxlx.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2urrpkifq.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2vdmausjs.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2oywpctms.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ikhjkrgs.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2lzojobkl.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2tsnssyau.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2uofjiqez.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2tlqudhdt.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2esxljxme.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2rcpgyqwq.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2rgrnngrb.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2bsccjglg.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2opoivhxl.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2vpdawvbf.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2vcjqfznj.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2esnilbru.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2norniody.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2xegwqtbm.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2ixwmlciz.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2tmywrjwp.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2yosbdvgq.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2ffzijrtk.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2xehmogxn.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2sgxyjnsg.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2coehkozj.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2jfcnxsem.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2xsjijyfv.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2owrusrbp.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2lkcjztso.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2twwrjvbi.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2hpdgxjku.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2tftghbue.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2frxrnhjn.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2rudokmfe.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2vvzfjsqm.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2uzhsrnju.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2wyqvdizj.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2jvudcisc.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2bmijjziu.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2nxremkfb.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2aclzwkqc.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2nyyxvmbh.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2egfyhwnv.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2mcjyfyxc.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2evsppdqu.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2btidpnip.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2mwdqvars.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2shplkuir.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2rpnlwrwe.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2iujqfsre.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2ddcclmci.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2ptuxaodx.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2ygdzlgai.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rxvmbohz.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2pgyoihkm.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2nbjoqtwq.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2usgyquky.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2eiztvrov.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2cioigifa.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2nbcifkdt.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lejousec.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2lblyejbn.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ayjwpshz.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2euiasawd.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xutxuzgj.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2kgyupwby.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2qjiczhkh.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2lnsqefmv.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2uryinciz.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2wfpbflak.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2askemcfq.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2xvidbnip.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2nmldecma.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2iisceyws.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2jzgyvaku.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2nxydccce.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2nbcddixy.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2rrrsafnq.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ihyaabfz.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2eegaktpx.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2clncsiab.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yrjnbngv.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ozpmstet.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2ehpcdfla.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2ejhpcaxt.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2viwpyrpc.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2vfyxzpmn.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2fxwaqttg.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2xuxahkem.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2zwaltbyv.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2wgwxouem.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2gmkanurx.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2tyxvmoxt.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2xiokfivt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lhhvzfjh.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qsyzxtmm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lfrhgoce.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2dnfzebun.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2esgtpiqh.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2kkdyimmz.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2djhlvtcc.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2fymmcpvx.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2rkgvcvbs.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2sczkoezp.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2nqihszws.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2ihezeulh.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2lhoygnqw.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2ibuyneyn.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2zwcivvjl.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2lglialsp.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2jeckdjow.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2ouzhbzlm.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2qamjvapk.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2exhxowvp.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2tqzyczzn.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2htacvizb.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2hqjxmppq.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ylcrcmcd.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2esrpfbhc.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2rckouwxk.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2vokcwxrr.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2dnkorucd.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2kzhglwtb.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2edchnqhm.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2esqevguw.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2qvzbwuof.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2fnsregtn.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2lsnfjqgv.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2uodtvkwt.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2hgtklnfr.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2fhzjntil.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2pfrgggrm.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2zoiwhkkz.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2skaszigz.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2yuvpmszx.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2xdwwdvyo.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2upumdybw.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2pmwnmkma.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2jfaavsmd.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2nzkjjlus.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2hqvprize.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2lvkiddbk.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2ppfyrbpb.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2ftgrqega.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2qebramfz.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2xjaqxgwm.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2qwwhyhha.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2fclobeot.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2pmwaixjf.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2dbdvaema.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2gzldswyo.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2qsmcifvq.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2hegjzgbw.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2bzbkrath.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2tqrhmnei.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2rmksldab.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2gcgrjsbx.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2wuimwpdp.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2ojorunhf.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2knawceax.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2biwwvhol.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2oadfqrwh.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2nmdihlte.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2uiaxhyir.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2sqtynsld.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2opdzxixt.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2obezrpxv.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2xabrgnjy.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2dmiwnnar.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2jydhoeua.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2skdymuou.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2xdprofbu.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2sxbercdw.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2lsfggcmh.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2lgocalxl.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2pifayios.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2rkuozhsr.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2wkfzhbgh.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2bhgeeojz.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2bfzazejl.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2dkakxcbk.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2llilghxf.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2mngcqpfz.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2thlioool.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2onoyribl.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2ngnzonjl.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rstqlref.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2jzcughgo.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2fonhdvxt.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2dotxvwhc.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2uxmhhwls.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2gtydqfte.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2pnvmdmii.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2pdvkwazv.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2bcfqekvw.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2mcrnlkim.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oacnhnfx.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2kvuwyppp.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2anterhuj.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2nahrvxem.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2zwcteqpa.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2iuplesif.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2zlozqscy.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2vllvbagw.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2rmnasxyn.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2vucqcrxm.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2ulgeeqil.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2pejnfxaq.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2wehwvtvn.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2hkqlwtza.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2mbfyrbck.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2fyiaorbn.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2tluevzgk.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2swmqpzkc.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2flhbqazn.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2nbgxnaor.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2xkyshttk.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2suqrinjr.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2zgmzrsbs.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2nfnpbbhj.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2zkccjroi.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2ocympmlr.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2ekttglzb.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2tytwxzzv.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2zythfguy.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2civvekmo.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2yuonrhuz.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2znirgpjl.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ajdwnhzx.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2wsenmmzh.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2dfbezyoh.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2ckxcckof.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2ucfpvaop.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2fhjdgype.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2rpduyoym.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2lqnwfxgw.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2xbgtaeof.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2bpmlonyv.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2kyojvvmc.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2wjvkamep.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2fqsxkgzl.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2lcardlgp.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2tyvbtiuk.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2cavsopch.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2difzrrns.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2hwbnnpew.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2uknyjhjd.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2ajqamozj.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2pjnapyal.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2jtyaocnq.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2ykvdiniu.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2vlcchewc.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2igjpmala.html


<!-- 参考信息 -->