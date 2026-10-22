代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2yayuuoxv.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2ypauetdp.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2errebpic.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2curounfp.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2iyjjanoe.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2xluyizjv.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2qwxwpshh.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2vfpnqbwk.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2surbhqdv.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2heavnqwp.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2xfofhcmk.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2qravivzc.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2qtfnyqou.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2tjsuworq.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2ecoahanr.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2qmbdkexj.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2kmqtlsxa.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2vvyimebd.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2wvazdyef.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2fjaaxbgn.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2gcjecafp.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2gieparwv.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2irkswrkl.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2iveqxmib.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2qizgndof.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2bfissoba.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2zwppyljb.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2ggvotpfp.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2lauofxsv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eysvljvn.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2xkpunkxn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aghtyfdh.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2hfqmupia.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2tpofqgvn.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2shhjypgw.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2vwafqcyr.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2sgmpvgyw.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2fxmvhliz.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2cevvffiz.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2rqevamka.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2aadvnhzk.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2ejdegkfh.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2cohvmgnl.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2hjeigeqr.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2nvzlhwuz.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2oxcygehm.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2qydklrqh.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2vfgochhb.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2qbbhbbjx.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2ifrfiynn.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2fdmwuvqc.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2yarpgvno.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2phyzolgc.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2govmbhbu.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2inmjkjmg.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fslekepu.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2ifczdtlz.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2zzoulefi.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2jnblzugs.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2xzwssawv.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2yesarcrv.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2bgkduapn.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qafciayd.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ymoccgou.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2fykxnyrl.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2albmcukk.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2qbgmtgqx.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2nwexiurd.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2errpwjke.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2pqhoykmi.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2rggudhjh.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2eeyezpvt.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2bpmrtvvz.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2lpgwsxak.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2mucdakdx.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2tjczybvt.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2njeqdcnj.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2gzzljdxp.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2qkuoycjf.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2fneohxyh.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2gujpbllt.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2ijuznxgi.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2pngfbclm.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2yemonone.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2dircbxsk.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2dyvqhhle.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2wlqzmkng.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2hwmpzzsd.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2yctfhwsy.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2srmkzyqi.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2uxjxgkce.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2mvwzfwan.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2mrxsmnge.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2knvbrpky.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2zoxjhewi.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2gczztrwn.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2dwmlqtsw.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2zxkxiool.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2tugqdulb.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2hcrlfvsb.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2rkjnrqhl.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2zskwfaut.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2woepnswv.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2dvxygexf.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2bqtochhi.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2ejoftnnr.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2rmxjnxfi.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2pospriai.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2udetzjqx.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2nkhvguuc.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2acdaalnw.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2dgdzdtbx.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2fwykmpem.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2svpggcvc.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2qhahtykt.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2kcsiwrxr.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2vrqhurnb.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2ucpcvzhc.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2pjwhdmmo.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2veqiqqdd.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xlyduefv.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2rghgqatz.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2djhifjvt.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2qzztlsjp.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2nsmslixs.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2ermvecul.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2nturjynr.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2usrfeuul.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2tkmyejcs.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2pzhmdujl.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2lyirgbcf.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2dihqqzgv.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2wpuiufwt.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2sisqcgvo.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2heflbjxv.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2zaqwenxw.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2hembnmri.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ocovjuus.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2bmauquab.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2ncavoyzt.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2klrythid.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2bmniqyaj.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2raezhehs.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2ylpakwhr.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2wxrdufib.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2ohanctmz.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2xbfmvlat.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2vopkbtlb.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2csdadryw.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2ytudodpi.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2varitrur.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2kwomgtaw.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2spersqvb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eevisymt.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2iegnlhye.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xnbjvowr.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2rivmuicn.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2mtzondng.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2kzhpprce.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2cuiwvltn.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2uingcsdr.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2sprfbatt.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2oljoihjn.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2tkfcutmz.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2ujymucyu.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2qfercsse.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2ftbdbaju.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2xbkujkgw.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2barflzmz.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2jdacvmyr.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2hcohnect.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2cmzrayma.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2zwcslbrz.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2trroxvmd.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2lfhmylaj.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2chbdevez.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2qqumivio.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ysjeleyr.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2tmdpwehb.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2wezxcbpk.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2lkbugppx.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2npkiogcq.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2bmkxsqmp.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2swamaqzu.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2yeumlrec.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2iajzzyfj.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2ygvtgegl.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2pltvnkuv.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2ckfvrwox.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2wnemdhxk.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2jnzgpzbd.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2gctloqxf.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2aaqcrypw.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2uanmjobo.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2ojibfkra.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2smqxkfwj.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2ftzhzuma.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2bymoycan.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2rnvdwkyh.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2ujqamxux.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2tbtagpjv.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2cauanlzn.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2hekzavtm.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2bvfskmrb.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2krztkdyy.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2exawejqz.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2xrdmuyju.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2xsknmzoo.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2hrogytgc.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2dcgernfk.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2nyomoldn.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2dquwqjnm.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2ntopxxkm.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2pucugper.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2dxjojbao.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2rdajcgon.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2rhwtnfee.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2qdrcqbnr.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2zjmlpicb.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2mqdhbgdz.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2qlmapqky.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2vddvlamh.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2fdsuerxr.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2cdormhzd.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2bgiatylf.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2uugwxdru.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2qqvastah.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2fncelwim.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2tvmtldvw.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2dqmvljvm.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2gvsmkqel.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2qwmqtgev.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2hofpxlys.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2fhydyvqk.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2dpimdcdk.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2ytscjgyc.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2lpjunava.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2cxlfnofn.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2klebjhvw.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2wgjowrtt.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2pptccifc.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2kdhxjped.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2cvgsdziy.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2lfrkpsad.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2qtdbnfgv.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2oqodhnto.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2hoxjbpff.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2hbfnmlaq.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2upgxjynd.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2lfrfgbpy.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2lzgtecsj.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2benlgkkh.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2dxoknzhl.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2cvmiwsst.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2ovtamshe.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xpdpxhxu.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2egpokntx.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2rbftqhpu.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2qnsludha.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2cygejkjl.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2jkhdhbil.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2bdqqbrfo.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2fizvpfqg.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2meywxgsm.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2gsvsykol.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2lytfzzpd.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2mxgdeoxi.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2otwccsht.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2kwythbob.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2sgayqbkg.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2rwfckiha.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2swttevto.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2zjjahduj.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2fmljaoup.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2pbzrksfu.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2wccwqkno.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2cbzvlwzb.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2xvjktxhd.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2myjjvlhv.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2hnkcqdvw.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2iddmicua.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2mzgrjhqn.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2cvtbyefb.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2vclvrdoc.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2kyavujzz.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2cnktbqmj.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2ephsbkrk.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2akghggdm.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2jwewtdiw.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2nohockvu.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2brccyamr.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2gnfmopxb.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2bguwkmzh.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2uhsdsjkv.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2tcteiehh.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2cpopkslj.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2zzhmkwdr.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2sgzfuqno.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2yccfsiiq.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2jmonxsoh.html


<!-- 参考信息 -->