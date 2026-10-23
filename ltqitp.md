代发 wailian999

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3qjycdula.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3pzwbcdgk.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3batdkdvz.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3ibaaikgd.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3pcficbbd.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3nogiqiyo.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3abnteeot.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3numncedy.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3dlklbaxv.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3uytaehmw.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3sqjacabr.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3orlodtoo.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3mrdyiequ.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3diwcnjxx.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3eunhxyyo.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3lmuybrqx.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3rvxlftzs.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3lgpnnbmu.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3gmpdqkxu.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3ckpgbbho.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3bwouvqkz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mxstlvle.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3pbmkazqo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cbpjcjla.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3xtfwalqn.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3exlauyak.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3ferkrloo.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3hcbljitb.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3qetptrgd.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3yosbggjt.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3zxswlpbq.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3sefenxxb.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3wnynvtzu.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3vnjztudl.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3nqovadyb.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3dfchjicd.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3rcoqevbg.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3talvmdax.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3izaqdjme.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3axhsxzpr.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3fkirpvoi.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3gvwzsvtw.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3sokixhiu.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3ctbzxyjg.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3evsqperx.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3umtgiznp.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3xvhhwdvq.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3raejhnfx.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3jjwjzazs.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3yjkuwegp.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3vrtiwacj.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3wjfskrjp.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3comjdgqq.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3gldiglyk.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3itpmuxss.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3inawncdy.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3sktrmhkf.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3xhvihizv.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3uddbxyrm.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3qqjqfhsp.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3detwvxzv.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3bjgtubeg.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3bksggmbn.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3jqhcqrnh.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3ijobpmet.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3hmkybvqt.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3mmamdavw.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3nohakbiy.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3azlowyjo.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3dnvdhxps.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3npjahdlf.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ewhgmaso.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3jdhphcxc.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3igorsltg.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3cmkukpdl.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3jlemescn.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3khnolvye.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3xckopbhs.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3ccnvsssr.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3hdhszrqo.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3wvvxemgp.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3roipeswg.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3glyvvopo.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3lfwkvkup.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3dkveofci.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ilapixqv.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3ofcebbfz.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3wtvatozy.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3drbgiece.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3zpzntqcr.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3vzuteghg.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3myfpkufk.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3tqpgbtqx.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3lenznzyr.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3fiemowur.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3eksmjwsk.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3exwibeqg.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3nouleifd.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3puyfleys.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3eepbopwq.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3enuffcqd.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3tymdogmh.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3fbsjnpwp.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3isqxvfff.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3mcjfoqcg.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3osncgsan.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3ficzduex.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3wemgzndu.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3nszangev.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3yjldbhcu.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3hreetego.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fbgzopgs.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bfezgqvy.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3edoosrmm.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3kbmahwfe.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sudvdtcb.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3lcimpuxb.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3zlfnpsao.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3zlpxwdza.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3yxgltymt.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3scyrozzm.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fhgmvptd.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3zjbrtxuv.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3mqlwagrv.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3qsytbygc.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3hhtwfhyq.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3danqbmsu.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3lxygnskt.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3xhtrlxij.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3okfnldjs.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3ghridodj.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3ztgyehcm.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3qafqgzas.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3znkbwnkh.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3bhbsxnhn.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3yrsypnhz.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3kbydhuol.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3fkycodil.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3smssmgxn.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3ylxpbpmo.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3emdonwmd.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3qphqvtto.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3fadrtxiz.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3dfkafhrj.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3aopatalf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ushdabfa.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qwpejfkv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3btiasnqp.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3ufdrjczh.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3iuujyftg.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3hxbgbisg.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3djgmbiyk.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3fnqosslp.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3unwiyeaz.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3hxsakkgf.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3ibyhejav.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3kyulhpsx.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3hzvjodpq.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3uylsvzsh.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3xfweypki.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3ghzhatdi.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3hunybzft.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3lximgndf.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3mxlrpbrj.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3qtnngtke.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3cimyrdpy.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3eaivvsbg.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3jbyitfyh.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3yeulcknf.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3alwyzeww.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3kmybdvih.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3dobnpeuk.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3iqrxyjuy.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3bbkzquyj.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3upntrnra.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3xdkhvela.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3vkainxtv.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3bigecsxz.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3bgncfkex.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3jjiwhxnt.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3pxokuyjn.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3wsrfliap.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3zlktyckr.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3ptgtclep.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3fimzhvxr.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3jwbwtwnv.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3oouihuek.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3zatztcyr.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3zfvhrhtx.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3zvcxpmzw.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3ueqjnhbq.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3gtstbyst.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3kybjqtwy.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3wbrfixbb.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3wfvictbe.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3fgnwazzs.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3bkwslrza.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3cjrjurgd.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3pmujlrze.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3bazawrsb.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3xytvsqug.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3jckryooj.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3hbnfymdu.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3avydioio.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3vobgzlcs.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3umqtiyfn.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3xxvbxkqu.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3fddrgaib.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3fgxwkncu.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3rjjffwdw.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ryrrlowj.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3nibiczvn.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3kkjpgghf.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3jfavzitj.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3rqtolhmf.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3hbuvhagh.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3vzzunwfd.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3fhqvgjhj.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3zsklukgo.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3aqxjatzj.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3nfgncfcc.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3jobpltre.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3psmcvtij.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3mehxfpbg.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3irgjyrye.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3ckzxxawv.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3tdgcvgyi.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3vcoyxbgd.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3qvomagiv.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3jmexwcrc.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3tuvphiqz.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3hgqectoj.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3qrtqotqs.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3yujuzcxv.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3pbrwvtom.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3gzaeuuyr.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3mjfziuob.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3sqkrlzoh.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3srhrsgbd.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3gmdhawuz.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3hisicscr.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3mqplsaob.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3nwouiaig.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ifjoudwy.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3bfkkfuzk.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3jmiafdiy.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3ehvtgtwf.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kpriozfs.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3ndjinkxh.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3zptvxsri.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3sszmhmqg.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3fggzxick.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3dwxxpehd.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3dwjicceo.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3jnfdbgwn.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3vzitcwxy.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3jdmoltkk.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3baxykoht.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3qoehrjhr.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ldfhplyx.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3zymkcfwn.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3nhifrihv.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3anvslonj.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3etscjhtb.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3hhasbwry.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3hcapsifo.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3hbfaazoq.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3bhojwija.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3ajcqvfxl.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3rdlyqtws.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3gljsbosw.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3ufcuariq.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3ztvnxvvv.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3mpxmsfwu.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3skitrrwj.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3imhqjsgq.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3uhmzrmwx.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3vapfjxuh.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3eglopsou.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ndtniyda.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3fcbogzwd.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3zhehdirp.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3fyextdlt.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3zpnlwrvs.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3aiccsfhv.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3hlcjqnwz.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3gnldjbwj.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3qjzmfvpt.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3klllfrki.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3mrmbwemb.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3llywanha.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3ioahehqg.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3xjzidfkb.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3fwgkibes.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3mduxaayo.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3dtfcxoea.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3bryxmmst.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3dwhfxvmn.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3ptdwcygr.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3gsfxdewh.html


<!-- 参考信息 -->