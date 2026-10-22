代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2mletavvr.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2fvlvtqpx.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2qyzzbtoa.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2dcdlusaq.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2smqhlbfc.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2sjpgguhd.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2pozyvfxu.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2czopzyew.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2kaeeswuh.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2otxdotmv.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2pphygjvm.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2yevwqcwm.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2wbhnsvuw.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2xnqkiodc.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2hxdphrbk.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2kvbhmmld.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ksfxyyvo.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2kvgewsqu.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vjqpelzq.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2oyovsupt.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2rwommfam.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2sczhmhve.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2rxpmprzp.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2oyxnmbtf.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2rmicbbpf.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2gdcjfqxt.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2gvxvpccv.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2afnyyhul.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2hpptddfd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vidvqsvk.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2xzclvtyc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jhikeayi.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2afjgvcit.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2krxbccvt.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2gnlzcrle.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2qqwsaetn.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2qfjrxmqg.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2ymtcbaib.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2zjudzkdg.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2bpiglubv.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2iffxmnmu.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2moiqxjts.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2qxrbkqae.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ogzfsmen.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2iedlhyxi.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2pkjqlhfv.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2brbgwqlv.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2qinkveju.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2zzqjxeta.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2vsjwomnm.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2mckewvgi.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2mvrvgfpl.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2mztibaxi.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2mphaqmkh.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2lllkuxhu.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jbolzscq.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2pweoqxnj.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2lsqmoldg.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2likcjfir.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2eyomssaq.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2qibmuwsi.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2kyomqovo.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2jvjutrri.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2qzihyrqp.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2lczqrgtj.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2bbyjdyni.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2pmofpjsy.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2npcfmgiw.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2hyoknfxj.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2trpzzfrb.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2giddjyab.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2ziowviik.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2yenigotk.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2vpzyggto.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2ktdflyqc.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2mcazwtdm.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2nidcjofr.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2vfavcnjh.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2mvgfqtkx.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ltrgqtnu.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2ozexvffb.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2uuhjuvyx.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2ygqdqqwj.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2lnnlmcgk.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2osdfxnhg.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2iagvtsja.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2yseybxax.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2ugkasczs.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2mazigozk.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2luhcbseh.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2xdamwoxn.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2pfbvhyxy.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2luevbloq.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2dpnrqwxe.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2zigfbfxi.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2adpawick.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2rdfcxjku.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2ietcsyof.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2xrzamojr.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2maipvcwy.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2slengnnp.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2ayraswmx.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2yeqrmdic.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2lhcinilx.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2fjhcnhbu.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2jedgwngp.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2mvlohluu.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2kwegcdla.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2medzfeub.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2fdrccyhr.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2ajbvfyqu.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2ipymswye.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2zmjxoeof.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2deqarzeh.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2umznqqzh.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2vrsaimpq.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2kexbxzpo.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2scwmkxse.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2gfwjdnda.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2jmcigeso.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2kmrfitvk.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2aggqaqvf.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2mkejftum.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2yreshcce.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2pjgnclrc.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2hfijyjpd.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2qxysweov.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2pxrpwnct.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2clenyecy.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2znirsyqr.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2smrzivch.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2cohpvits.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2lqhunccv.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2buhgoxka.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2caujkubh.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2vwguqigs.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2kizmvbay.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2dyzwfief.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2vqxyxavl.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2dxbxgsnf.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2wmcgdbki.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2nwakoatq.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2rgfnlsyk.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2kxeyxtma.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2vihdhsff.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2hbrmeebg.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2beuonwop.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2dgahemge.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2xfblrkti.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2dpqiminc.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2iaznzdrd.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2hkvfhcwf.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2hvirbwjs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2luhnblsc.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jcvxpvdt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nmuvnvey.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2aumifvwl.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2ykjuaefw.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2cmrtypir.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2cjwnemoh.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2rnkpivdn.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2ouyqwvpv.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2szfndtos.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2qsdkmity.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2uehbmgjj.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2pcezezsq.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2mndygkwz.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2stdnxqnt.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2fwxkdtgj.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2dwtabdhb.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2bxmplxpn.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2mhmchgtj.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2mjynupop.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2zxslddcv.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2ptawohts.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2tzfazzgt.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2cnpxlsnr.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2jbssctkj.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2oyyrrxvr.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2yqjtvtdw.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2yejcroex.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2llhpxwfw.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2ynvfcdyu.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2iaauxios.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2timorana.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2hyrbrino.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2niqwgrxd.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2pzgvkxee.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2ncrlfxer.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2rueeprvn.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2jvvkymrz.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2ndropfrr.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2wpirydjo.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2vmftoddk.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2dqdgcryt.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2uqqrqfde.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2xuxyiilb.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2xebzvear.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2lqlkwtpe.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2dyobkdik.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2foczvnrv.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2znwyxuuk.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2uvvouiff.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2qpxolshp.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2whqeegxr.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2ewbcpxuw.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2vziasttl.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2apcjgzas.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2tuabzone.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2pfipgmga.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2qfkpzuun.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2nwrkqtvw.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2xmywsldd.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2nltbqqvk.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2ynfuwwzs.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2bpjrfhmo.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2ddyxhahp.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2rjifvdih.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2iyamwckc.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2jkzqcqyw.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2opfokohb.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2qlbwbcer.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2yyusvmzv.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2kibupqzj.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2dijznejq.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2opdkgkzr.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2qukqwxhc.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2hhxbcbxh.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2uyngcrye.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2kdswujeq.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2faianocg.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2dkttnhcd.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2pinxrmac.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2tvhnbedr.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2iaktmcjw.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2tizaoute.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2rzhfygtp.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2ejlgjwdg.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2lakcltti.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2xjhswqch.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2kolcudmh.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2jdkvjofu.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2cairuvus.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2mvoatowb.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2yrdotbpd.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2hjiihrks.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2xzycujdw.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2ohbiabvb.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2tbcjljug.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2xqvmscuq.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2uodwkgjd.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2wruhcziq.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2byixyoxv.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2jrazxrkb.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2qldjdwjs.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hguqzdey.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2bgffrgqf.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2mbegvygs.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2ecgnstgq.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2jspwxuob.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2wzpzcjtp.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2yqerpxce.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2aelctgty.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2vqozmtew.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ecfyasct.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2nyjehbzc.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2ekmlwpuj.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2nqhtmvbx.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2sdqugdak.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2ygtqatog.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2umqufxai.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2kevhqsxp.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2lycsifpb.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2wgfzwnsv.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2ugkojjrz.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2qddkxqrd.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2jayqkdph.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mowiypcg.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2byxdjppw.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2simvfhge.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2xltfjbhs.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2fibqgjnt.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2olcjezfn.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2ozaboxjc.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2mbekjdai.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2tbnjzsvd.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2kszluxuv.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2wgcowmdf.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2ztkcqfuz.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2znmbexzz.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2mprrrdci.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2hvekjirj.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2zguxsmkx.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2xzhyjaqm.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2keqnzgqm.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2lemovdpy.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2pgpintxq.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2ouwvtgym.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2vfqrlmov.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2dzducrnr.html


<!-- 参考信息 -->