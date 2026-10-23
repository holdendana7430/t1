代发 wailian999

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3npsmdncy.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3doggleic.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3oscwkkbi.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3sxmgjtwk.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ybdwgbza.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3ecfszpqr.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3hxncxzof.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3pxxovfis.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3bxeanina.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3ekaqirii.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3xaweuvqw.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3jbjvblnd.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ceemqngg.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3ubgzexzf.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qnslmjdg.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3tnxciwio.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3blqebmtr.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3tnxkkqcb.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3jbbazecz.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3zkadpeyw.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3fhameucp.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3cnfturza.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3tfmmzblg.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3dinffrij.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3puwybqnz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3thujhcgc.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3zjvvwsbe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wlnggowi.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3oucryfsd.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3zptefpyr.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3mjffwspy.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3biveexuc.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3npsqpkji.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3hhicxjjo.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3rrhxomex.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3yqnvbvyo.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3jgoybumc.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3bjtuxvae.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3qdpathfb.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3yurmmvbb.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3gsfqwrff.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3hvphcykk.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3trmahwmu.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3gqipdntg.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3arkdvsqj.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3jkgfwvvw.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3soenbzec.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3pvloozks.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3dekcjnkv.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3bwlhnnqd.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3igdzofiu.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ulnvfusk.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3zpskewxk.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3twowyveg.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3norwgpvv.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3lvyewqhy.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3xguxpsah.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3uvngyeyp.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vbpnvelj.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3uynvmqtw.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3ahgnaoho.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3krqrollb.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3zsjpmisi.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3oykyejhy.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3dtlihmjg.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3gnruvatq.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3zjkwlrcm.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3cdijtlbi.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3pyzicebv.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3bbxnsrge.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3ebtpbzgl.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3hukxfnnw.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3hqwbanyi.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3usuzztiw.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3laanauiq.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3hcreqjwp.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3iwihuasu.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3yuoqwwek.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3sxtoqgqf.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3kxhzgzxc.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3cjiwhsbu.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3qsxphids.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3vfhctryg.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3opsgbnzz.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3joqbckvr.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3vfpfydki.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3ziujzzdl.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3tvnegihj.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3pkwfmebd.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3aiprharl.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3zdryfibb.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3ufyrmktd.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3wllsfueo.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3lvtvfgqj.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3ltdxqbvg.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3atcnlqjd.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3kyrdwluw.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3jriuytqt.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3diduymed.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3iouxwccb.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3mrlrfwqc.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3avglsmzh.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3idhwnerf.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3zczdmmgs.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3rhkzdvps.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3jvicxyej.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3ylyengwx.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3fhebglkd.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3arvphlxp.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3vqvyxhgw.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3dznmwkqo.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3cpsmsvba.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3xhcsseoz.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3lbdxbsun.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3cfigmsqt.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3xenpmkln.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3rkubtttm.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3scwmxoiu.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3xpitdcht.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dujfyzet.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3bdbuphkj.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3ehmohrmi.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3ubbdnmlp.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3nfyelgcm.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3izqwytvw.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3wjjhpnke.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3xglzbiay.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3bwoloaqm.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3zoyqjunn.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gdmzuggz.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3gmvrblmb.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3wpryyayr.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3rpkqlori.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3swjqsviu.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3ysastudf.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3cbxoebrj.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3bpioxyax.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3stpczehf.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3ackguybw.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3orzwkhne.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3ecshiiqy.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3orhejdzf.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3cfxozafh.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3esdvqwja.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ksegthwr.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3squjrarj.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3wfrdeord.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3pnyfuptj.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3jipbkncr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lrldjywh.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3gpnaqfny.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tkjwiysc.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3ymkgdkwr.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3rcwwpmbk.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3nwooyajb.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ybgrarnu.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3ydibckox.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3proqrmpp.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3ejwatgzp.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3iecyronn.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3zeztvcep.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3qqzxskqz.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3frbcexgj.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3nxkapbgw.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3iorpbfhj.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3lubjzwke.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3qlwcvofc.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3ocowswbe.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3fghzklin.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3iptjsemm.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3tvruxpbf.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3wwyofyoy.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3vnbujksq.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lqoubfsl.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3nxcndlhn.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3axwxchlj.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3zwrrjmjj.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3qgirhiwv.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3wsvwrcmh.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3xgatezuf.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3hiflxkvg.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3ujgrbvyx.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3ysrztuag.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3jyfghopj.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3yifzconk.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3uubogdcm.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3qsqrzzqb.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3blpwppfs.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3cyyibrhv.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3uuifuyjv.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3rhjumsue.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3acbnmqsl.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3fjoaxbfo.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3ikebwkiq.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3tkucoukx.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3pfdoucbh.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3bqfweqhz.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3nkewvrnk.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3snjmydod.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3zjdguzva.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3ojshzzfm.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3rkdqaprw.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3qpxgpvgl.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3vctigcin.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3rqhtxbxy.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3whyebsjx.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3dymlsyeh.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3ggrxxeyv.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3jvjmzoqf.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3mtyzvtue.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3wavfrgas.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3kdcntedp.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3mkbayxjj.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3enwksrap.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3nzxrfwoy.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3ogdnkjtk.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3vtqkbxzy.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3hnllieji.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3yfrkktff.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3paphryyy.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3esmxmzbc.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3aduymxlv.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3ckikfwmu.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3ldtzafng.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3qbmakowe.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3nbhszwfg.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3szldxnbk.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3xrdbhnoy.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3crnbjxsj.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3xeiqrglj.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3qnpjcsbm.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3wxexjnpc.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3catewfgf.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3vmeygrho.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3ioweupge.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3oxrftyub.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3zjnauzyk.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3otmlsvqj.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3cedqmmmj.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3hylkuwfs.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3wsfrbplp.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dnbflqyq.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3shfwfdpr.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3lnorluhb.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3pmcxkfwi.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3rypvvdnn.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3wmahllrt.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3esqovzdr.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3bblkrmwd.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3bipazroz.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3jiuubvlg.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3akotckzw.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3ggqkkxnu.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3rawxxksi.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3vipcplve.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3cgxonqnw.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3gdfkezjb.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3iqmxxhya.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3mvfxnivb.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3rxldaquq.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3oqnvxjqd.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3zgpikwii.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3fkbnvbai.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gfyybdft.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3xbonptze.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3dzypwrfl.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3jawvnqte.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rrgucgqt.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3cgwtrzxp.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3yjuakeye.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3degfvjqt.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ujteoepy.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3cyebtcma.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3aqzukksn.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3gukigvqb.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3lmyhajyb.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3yalqgldl.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3imhtbhue.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3vdvbybhl.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3idymxaav.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3dhejoxlf.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3jktwoozk.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3xlloduoo.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3jahdlqln.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3ryfirrqk.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3siuggebo.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3vpjxbvqd.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3wbarshys.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3zzaqdnsc.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3xqxjqyfp.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3yhtqwshq.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3xvifsmfy.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3dsusatde.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3zyrpcnbc.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3wqyilway.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3qunfeadb.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3lxivtdke.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3sseaunkb.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3jwqrviip.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3tteseyas.html


<!-- 参考信息 -->