代发 wailian999

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3jyipzypr.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3kpjurhhr.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3gcaokncp.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3yhaiboht.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3idpcprsc.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3zajmfavn.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3juiosath.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3iahymcia.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3hrrrkigc.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3esmpchtn.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3qzufrfvb.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3nkqfcbym.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3bowbrxkz.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3zihavhng.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3inwujfps.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3dvrhfirc.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3vyoqxkgs.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3fedstzik.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3lvtaxysr.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3cixgwbey.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3rfcocivl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pozlotyu.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3mwlmrlif.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fmmixcyh.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3aellwish.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3rjmnfvpd.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3vofsgdzt.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3bjtswoie.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3tmlfdnkf.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3hjerstyp.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3lbcmogdo.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3arnpbjms.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3oosklzlu.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3ctcddwub.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3honcjvww.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ftkqexee.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3omlstemg.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3xdrkontp.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3laibogjp.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3cnzgsgpr.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3qphawjjz.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3gdwesjao.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3ieqahjzu.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3mljcxuli.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3dwuakmvz.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3bsoumfwm.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3tdiunyhz.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3dsldtnlb.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3zcxiudvi.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3hemwlzuz.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3qiierfkh.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3umkkdxcx.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3aepiytct.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3uttkgiyc.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3kslqzfsn.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3fnkaauva.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3zycwbizg.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3rfamhdwz.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3qtdkchbg.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3sdoibomx.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3wimbjmge.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3hastmgvk.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3ktvzxprm.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3noyuogmn.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ohhaptey.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3kpmtwfiy.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3qktwtnvo.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3tiayglqs.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3todbibpx.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3teeaycas.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3pkgotwdb.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3lknjredb.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3ujqugrrp.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3gczeftik.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3nnpqhmmv.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3sgdfbxwx.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3tynsaqtx.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3tnmelkrt.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3dnddshby.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3axmsuxkw.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3wlvsatsn.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3rvtnuuqo.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3cxwdqmkh.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3kbhfnzty.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3qswuszql.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3vqdbuxvf.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3kyeubqqc.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3sxqojkbk.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3vnhwsqda.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3wezptyip.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3tsyrjfzs.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3gtnhsvtx.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3dlskecoe.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3zyubukti.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3jgkcjdkd.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3jcvrizzu.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3vyovmyfr.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3izfwvbdm.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3cdvkiyuu.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3aucgczwc.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3fvxxkjzp.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3ykjaennc.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3bhhzauki.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3cbpqbaxf.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3xuzskvra.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3dmmehnzk.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3anlphmnr.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3beuhgbjx.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3neeyuoge.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3cffpkvxu.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3vvgexepg.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3hepyncit.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3fdlzcwgy.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3ktuzprfk.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3yoyivsoe.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3sllbwwwl.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3divtizlb.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3izjoulhh.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3sgpyiqfd.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3ggwmhbag.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3uicieiko.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3lbsulvrs.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3pzvowwgg.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3idyvbvim.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3eydjrppi.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3fnedyvje.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3jwzhzxvm.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3fhqgrsox.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3nofvhxuh.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ulslpgsg.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3tvcvyhpq.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3vzywsgom.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3foxiyowu.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3govuhoay.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3dcuqxjws.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3zfqwrkcd.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3tssnrxmi.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3parkvbhi.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3xvvohfpm.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3wmulbpgo.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3udktgiaw.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3eswtsdcs.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ktkkudef.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3dqnujcne.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3cxxcfjgj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nxjwglts.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gfgoxaer.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fthdebin.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3pnuaeamr.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3eqfmjlow.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3xnsctdmx.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3wwmoncqk.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3sezthvud.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3xhoawvfw.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3fxgehjjt.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3mrvgplhr.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3qmtedgga.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3seltnrzm.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3ngazybao.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3tvnbaemq.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3khmqwgwr.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3nnipvhpv.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3dvcfgxlk.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3rzltynbf.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3rxhdwiqh.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3duibflqq.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3nrwnfajj.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3evioyhvt.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3hhivtbkw.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3szbnhpqn.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3qkbbfilh.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3zqdjkvci.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3xlzjwble.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3plukotac.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3ceyvdwyh.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3gtzwnbls.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3akafwjhg.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3mhhzmexm.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3quqandpu.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3iifpunjo.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3bcvqkexx.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3yvpjiidn.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3vshjlqws.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3mgkxjrts.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3sgklqard.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3ohftwwqq.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3orzvsdxd.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3snlitnev.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3nnzrarzp.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3qvhntizu.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3sspaqqgu.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3shmdtfhm.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3pmdufoxi.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3qvamyjzt.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3gbifbdrx.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3rszeipjo.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3mhsugzmv.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3qlmcamag.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3ktlmebrj.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3nblwwadw.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3vylhddby.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3qxsobaej.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3abaomcda.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3ljwsdstd.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3irlnbhvc.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3kkpuwoze.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3kcwumorl.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3giypqcgj.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3kbuhugqa.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3hyzhznjr.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3jwqbdvws.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3nwltbhmh.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3exdngudx.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3rgllsewy.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3bqxklyzq.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3orpiyqff.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3lfzfiird.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3vvxkjzpo.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3nmyrhdvf.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3cjxptyle.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3ajfaehtl.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3slbujeag.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3smgrrajw.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3dogwujdt.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3siurxstx.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3ptyvofom.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3swirxivo.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3gyzqxual.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3wolptkcp.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3xmdiweav.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3mviporag.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3pfzoxqth.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3kziswrxa.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3txuxabul.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3pdejiucd.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3xkedkxfx.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3vsrwebhp.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3uvrswhxi.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3csctffma.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3hebrwdol.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3stqhdygy.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3vnfrewsh.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3fgbotnec.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3ncpylnuo.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3gwxavnfq.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3levubasj.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3xeezlkkg.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3izzhhqxd.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3ldcvkwku.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3rzbkfufg.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3dwktgayo.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3yzuaqyus.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3wdoodfje.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3iifouitd.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3psgsgpur.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3lrmpebmr.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3wnrbrosx.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3mlevwnbx.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3ntvjsyqc.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ucyvcsjq.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3bcsezthn.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3ykbrdwrv.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3erlaokve.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3mefpspgf.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3gqnxohgi.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3dcucgtns.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3qmheochs.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3skncqwfv.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3tejetcss.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ccnpuktt.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3nouchjga.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3plzgixfp.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3weijnopy.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3jfqnprbm.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ehdkfepm.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3dwrvtikn.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3lwqwxffw.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3gplrdtvt.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3rmygppgh.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3dqcdlipm.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3gihtkezq.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3mbzfnwsk.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3xajowxxl.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3kvvtamkj.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3iezmaalf.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3rzozekep.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3ivpcbrdw.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3vynzxvyz.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3vywviwtu.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3odjtslqb.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3hrhdhblw.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3jvoidqes.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3ygitukgn.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3wiuyemtr.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3xnfhgbzr.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3zzaxsoqq.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3gvzzpjtq.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3zwzonmnm.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3zqjeilky.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3nbxqukwm.html


<!-- 参考信息 -->