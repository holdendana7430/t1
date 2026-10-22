代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2nbczthxo.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2gwqswmww.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2toekvtmu.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2ucznjvsw.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2btvttqks.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2kwzewbbd.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2kabefqiq.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2qzctfrsc.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2inzzcnmy.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2hnxrxeug.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2xasliosx.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2bxfwahbn.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2nykideou.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2prvpsuac.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2odaoohpy.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2mwascnob.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2dmimuooy.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2cnepuqrn.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2yxnsyshq.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2jteztwmo.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2klvolrec.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2djkbvycc.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2fozfwnvl.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2chiumjax.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2lpxohdln.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2cohzrmtg.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2pgjypvsg.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2zqxpfswl.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2bywvlyqf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kbrnxsoq.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2vtcqhfho.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2grxgmmnx.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2hgmxpomu.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2kdtuqelj.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2lfjpvdxa.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2qgfnjzyb.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2yuodgyxp.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2lniqmfrq.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2huozgryv.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2xyzppwnk.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2atiaifmh.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2pjpirwod.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2zcumzage.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2opschuzl.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2sfkwzjak.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2ikcyqmcd.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2zafjtwlg.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2seizsthq.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2jncpdisr.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2odnazcfg.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2cqlponoy.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2sybnvptc.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2ajzlpqfz.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2qvsbuwdl.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2rccznbvt.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ukvqntyr.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2qotslmer.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2nddrixjc.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2uxuaxgpi.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2bfcztxva.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2dzkjshzs.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2aekzmbct.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xhtiqoqj.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2jjlfqowi.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2cmdvgjcg.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2zisisduf.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2kpxrcahk.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2fqwilfby.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2rdnmgxvu.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2xzieknjq.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2peqfanlw.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2zdvlyalb.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wboxhdmn.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2hcyfjpkh.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2edblzdai.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2yhkfdxec.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2icwlsrrq.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2unwtfgkb.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2yekdjdje.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2qdlnxqbk.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2ipofmbnl.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2nkgnbbpw.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2yaslhiei.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2chfzflkq.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2xxcemzlt.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2fokxuwnx.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2bvuaycyh.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2ctvbiaci.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2qtglwxso.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2hsgtuqbe.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2adpxhket.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2zyjfccyv.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mdvcbqhl.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2piyagykg.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2gxzkkvph.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2ojvtmxto.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2jlwrpwze.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2txumukhr.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2noyjgotq.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2crhmlidn.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2oeayoxfo.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2huyyzkyb.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2qtldqpis.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2gaimleyy.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2hdoescom.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2llluaxno.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2qmvwtxud.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2qnbzmzlz.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2brnvuuyx.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2ovrvazdq.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2dofxgpzd.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2luzaoimr.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2dzxsfzum.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2hcjoqcmd.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2fbventtd.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2piclesjm.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2cvdrjcrl.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2ernjrdoo.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2malsbhij.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2dmlcxbid.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2iaxmvunp.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2isdfznem.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2vipdzwpa.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sqoqlmdt.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2uryarvmz.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2pjevqrfz.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2fifsltlw.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2tqlbccmi.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2tohvxfgk.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2qiregcpx.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2degwvpqy.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2igmblahp.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2cnykddol.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2oifznifr.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2krtrkrpy.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2kbpowoff.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2qoyvqmlb.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2akfhlscl.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2xetspqbq.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2nibdpatp.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vhruiuma.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2kxdehyrs.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2eystfqbu.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2rgybkmtg.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2kftcyoza.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2osqfuynu.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2yicojlzc.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2biiimeuv.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2tvskdkid.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2xyhyhpvz.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2wrtqsjsb.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2nyepujid.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2khrfgvbe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fwfmzjyt.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2usbhfcrf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ijqojssf.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2luthpxrt.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2qnbehtmb.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2ymdtevmc.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2bbsbknxi.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2jqeeofqs.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2yfqqcfot.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2xjsekzff.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2hvicfkcy.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2qwgogptx.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2msuiaall.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2pudlcfvk.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2ybmxwmbp.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2lgfegbab.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2woghywia.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2vdqaipnb.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2igxiiafq.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2sdbkogms.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2uopyclno.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2znegxztj.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2cfpqtdwq.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2mhovhovt.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ggnenuta.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2pvgegapd.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2wtjwctbm.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2pucscarx.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2alfykslg.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2nnuztmti.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2ogaojiiy.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2jyimgior.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2thgmmjbf.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2gupktwak.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2bdmylwdh.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2jhhgfrve.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2vdbwfapn.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2kuzwddng.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2tlqsiztm.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2tghvjasd.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2jxgpxtjc.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2qrakrhne.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2ufnczhro.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2vpjgnodo.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2kqerfemb.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2ceqnjcds.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2istrlfvy.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2sudwhdak.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2mdatadsb.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2vwiefwkg.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2bhpnqcuk.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2qtumkfny.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2rtaoagbv.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2dvgvqqoe.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2nakcelka.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2otgxhtut.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2bdpzvgbk.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2fkgrcodi.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2xaubcxqx.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2eocqcxhr.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2amcyumjt.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2leagmdez.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2uhmlntwm.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2jjyzzyfb.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2ipobzczn.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2vsfpqryh.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2cwutzuzc.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2lvfgichu.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2ybppdupi.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2mkhvoixb.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2lqhgejml.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2rxvjsbjv.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2dcmnxnpy.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2xrtafizs.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2hthritgj.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2koeooyun.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2nwsmkwwp.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2jgdkrwwm.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2udulmwxf.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2pztinuri.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2khnqqujj.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2vfmjqddc.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2nnnedvop.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2jsjzebkz.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2wgsnydnp.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2txvechvg.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2zknvkcnl.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2zmgirhaw.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2nghhbmka.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2letgzyqa.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2zdsouxom.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2mgfajjbd.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ewitvatq.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2mgasbbha.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2qftlqsyz.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2svtddtdb.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2lwbsplqj.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2gklrdflr.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2tbaxurdz.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2dbrwbckz.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2ptmbdrkr.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2dbubreyw.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jshcbpog.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2ayszjwzi.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2owrioaxg.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2athbpefr.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2lqtitmgb.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2gkfponod.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2rlwcigry.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2kspoeggv.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2nplmxmsf.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2xdbfutgj.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2ygeukxhp.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2zdlbvuwu.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gmchwjht.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2kgdavzmq.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2dgpkwalt.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2qsdqlidn.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2fgzmbxvt.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2hcqctvdj.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2edzlzsff.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2sweljtah.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2cgkhkxhl.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2fwtqcoyk.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2igffyrla.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2ffhaqtnm.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2pptglijo.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2xhkqoakn.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2iecvsyzs.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2yzmbdszn.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2wcxnmcmz.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2zuuspbcf.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ydcrwogx.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2uwsriytv.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2tacccrie.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2wjwpgwrr.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2jhlluepj.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2pjiznbdx.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2vbooakbk.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2xeczkoml.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2etrblicy.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2qanwskdf.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2cukesbjo.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2rqmkmqzw.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2hvnfkury.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2tnxzxcws.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2twpkwync.html


<!-- 参考信息 -->