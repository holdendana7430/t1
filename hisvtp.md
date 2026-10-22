代发 wailian999

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2wuvbfaeo.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2qnvulkvb.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2tviuptmx.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2kfvxvygn.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2stktutgd.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2gabtiaru.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2magctaxn.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2nalamkbw.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2cosvmjje.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2sxttmxmn.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2xiejmcrp.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2usorcyfo.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2hvcqlwxw.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2hmrkvuim.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2cmzockna.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2iuvhlquh.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2mhacsepw.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2jhhrbscv.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2mpsfnifj.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2swvetcri.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2cdmzfhtn.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2anfxsxei.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2foerbpbp.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2hzfrbkxh.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2ydioorav.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vujzcyjz.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2lwhdsvji.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gwkdcqne.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vbmrrcqb.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2whlulcfl.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2ewpqazet.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2mcfnhoji.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2ombwihwp.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2xihjvkny.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2nqgblmnh.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2hjbonofo.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2amcyosja.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2wxhlxjxu.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2koqsecai.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2bmhejuec.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2zfgwkbnw.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2vqmggbpz.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2oukrmenq.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2krzxpzvo.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2uffivhmg.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2gggolcag.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2vgksydnk.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2ekqwkajf.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2upfelaho.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2ilxlcmbe.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2bprcbwew.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2tijgrtwh.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2iiweyjfd.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2ryutreeu.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2ygxohbdv.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2retfezeh.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2oamwrokx.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2trmsvewx.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ptgxipim.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2uuwmjnqb.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2sxzrqzqb.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ppksvpnk.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2xhkdbvzc.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2pevzufkv.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2gyfwgmme.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2bdgfnayy.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2brqxelux.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2qtsffqks.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2qobalyoy.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2kijvhfik.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2giuhqzen.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2cfiachsz.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ufrcntzm.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2vdazgjdu.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2mmhcifmw.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2hfedxgtl.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2pkcoioii.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2edhaqtzq.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2exxfyhbx.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2olcxkciw.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2yoiffccd.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2deudotki.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2ppmpagxs.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2wmxejyqg.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2smeouczd.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2fjwfpedy.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2fqryuton.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2lqkeqwoy.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2cmhlnemt.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2dzstotmm.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2afxojgfq.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2jxffppni.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2dwwhdluv.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2wacyacku.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2ptdytrfn.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2ssqbandv.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2zqchblgg.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2grytisnf.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2mrlxjbpz.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2omtyshnv.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2anahkvzy.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2hoijilva.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2euwfxsrw.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2grwcmoyf.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2aetpqgjm.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2pewvybzl.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2mcozjcic.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2hfxsjwex.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ukjeiqyu.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2vpvmunqg.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2mjswogyd.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2wxrqapjt.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2udqqhdtw.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2tavknbry.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2zkcpkiwf.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2gtxfejkc.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2pqwkcfvk.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2lclptgjf.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2zqoczotw.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2aywkggmd.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2jwmuboxo.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2hqupccev.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2dprgtnwj.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2tfhbqrwd.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2bfmevafv.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2veeuscfm.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2lldfxyel.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2ssdmrqjy.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2tiijbbkk.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2hbsqqdjj.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2odnsdnhf.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2cgnzxmac.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2ftsiuemc.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2nbrbwwvx.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2uvvlvxmn.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2djydhyat.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2lvmcpyzk.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2oiokmhqq.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ktrafwbo.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2nkdmgtqg.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2knweudff.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2vivyllua.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2qhmymnkv.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2jsarwgvl.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2vdtuyheu.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2hqwbiqfy.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2zjnzliuh.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2znbdogja.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2xpxqvqrg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vhurreiy.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lqgotnki.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qsdexjmi.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2rrclenmw.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2bylxlqrw.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2ttzvsgbb.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xhksqpea.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2kwbzcydh.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2xlzaxcln.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2rargptyr.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2oxnntjhz.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2eaiggpwz.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2gpwzqzpl.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2bgtbsefq.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2pdvpyity.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2kvhsyxja.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2crrlfxlw.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2hylwhnbz.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2qhlrhfks.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2xdenrzfl.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2liidggjj.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2hllidutt.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2vcdckyjo.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2mtzjntam.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2jvhckmnw.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2aiqqfvuo.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2gdldgunv.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2oiwwktwo.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2sxcmaych.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2ayigiiss.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2kbyzllsg.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2edqzidmu.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2vmepuawr.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2byavzuqu.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2pvdxyicc.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2dtxbfnjn.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2mltgcjgp.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2qlnwlkui.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2hughlmef.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2csqwwcqi.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2tpgrfebl.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2efdgtwqg.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2mlpcokxy.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2ovlmnuwv.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2bulwegfu.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2zoexglqu.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2ufjjvwzf.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2cesdbvtn.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2vgrrfudp.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2mxjqfpkm.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2cmlhxmtm.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2nfsezuba.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2gazvzxge.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2obbmimua.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2ojtlhobw.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2mcdxknnv.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2yjdzcoeo.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2dpujsefd.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2ndimnzje.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2anuzuubv.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2bbotmoxz.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2womwopgb.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2umvkzgyc.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2xtcqyfcf.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2tkqqudky.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2afttwpai.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2mnxmxkpv.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2gpzvblkv.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2gamdfjut.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2mmtgwfdg.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2oysynteo.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2fxsxedil.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2pjjgizxv.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2gmrufgue.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2emttened.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2yjeueupe.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2lokqvrsb.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2htmdhzah.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2qrvowwyl.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2rcuctzzi.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2xqewijug.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2jjtvvkcj.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2jzmzubrp.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2yfzbmdip.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2wslhvipg.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2odcsnbdh.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2ibykhill.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2bilwoyqe.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2mugxwobt.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2hyqegzas.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2zccludlz.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2fonrpbze.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jvpyqkqr.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2vpdpczej.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2aoieuean.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2zdphyccx.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2xbcmcqvt.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2ikifspxu.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2omiadhbc.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2kqpeudwy.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2cbevmyrf.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2ucrxqhyo.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wasilnmi.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2mmrowhxe.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2nhurdmpu.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2lttkxcus.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2fvntdtvc.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2bncupsem.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2jmfzzvry.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2txmcbxsu.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2fhkdkfui.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2nmaqkjys.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2qqbqcahf.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2mxfufiga.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lwimbueq.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2hccbgnrv.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2ipkbdjtk.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2snquemtm.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2gxmaseua.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2qsccqjyv.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2elrnyvth.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2estoqadz.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2rqgfslvi.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2mgpykhho.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2uefanbsy.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2pscotzwr.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2ljyzyafm.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2dajlvpmc.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2lovdnnvc.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2kitndbda.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2eyiymaas.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2niehntqi.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ydslnlvg.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2rcgowtba.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2ksouvedl.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2dbirbmyj.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2ryufyfdq.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2utmbrsxq.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2irreiazm.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2xbpyqyyd.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2tbjhpwsn.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2ygvmtwwi.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2lauseeeb.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2izlshyid.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2iurjmett.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2xmllmlzn.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2qtqxpcny.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2sqnrnxyc.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2azjzncmq.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2yomjjdsr.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2hjhxpqut.html


<!-- 参考信息 -->