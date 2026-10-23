代发 wailian999

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3uldaktkz.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3umrsggxw.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3jaaljdvh.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3wsorfage.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3xmzzqecl.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3okfcvtxr.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3kbkxvvpa.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3lmildbdk.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3ahbanrik.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3azzkaoss.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3ejczdvak.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3wxmrvzbp.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3wdrydwpz.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3pownlgjo.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vfnmzdbq.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3spudpnaq.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3xvjwrbdn.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3smjzqpxc.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3hfmmrbim.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3cqacdyrg.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3jrlmibfd.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3gwixmogw.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3tcatkqoz.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3naappvho.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3nmcoqmja.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3elkgakty.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3mfstwzfn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jfqhzegq.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ipwguswb.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3blgqvuov.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3uyofhcaw.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3skkidsae.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3mbfqyzpo.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3piabonie.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3rizbgyin.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3demaoxxv.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3yqrkpxmg.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3drlghbly.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3pqmlaqth.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3bwwyopig.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3odeaxdxc.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3jgsslzsq.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3aqjylwnc.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3twygqwqx.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3oaipecwa.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3jthhcpwe.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3lahauvwr.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3qvapetao.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3yfyvsrjy.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3ckuwewff.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3hvjkkkyh.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zdfcvgld.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3ofxrtrig.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3fuynoyet.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3iydcjyks.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3hgjzrpmk.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3otioqfue.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3silzsngh.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3clstwyjd.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3npfudwlr.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3ppeyzoca.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3kniawjek.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3sjcukino.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3qnkqjodw.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3hkseltoy.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3klcrrzrp.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3ydmeiqcq.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3tmfsjhwv.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3uoycoiwh.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3ixtevznb.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3kaocasfe.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3rcjurcst.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3wreekqrq.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3aagnxxmd.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3lmfoplve.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3jtwxmnnc.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3lxjziegj.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3yfadjpja.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3skpupmee.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3nppcqqlk.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3etmwikov.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3wzthhcig.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3lkpqkcck.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3qwzqvuts.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3bvkacnnm.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3malqizpo.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3dnbmtuwh.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ojalbkxs.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3huwjdcim.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3varrpqti.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3uasvgthf.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3xbvoszwn.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3afrhpwyc.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3mftwqpde.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3izehcfun.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3jnqpacfb.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3ticauxth.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3dsnzcdnk.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3dtwiedux.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3iesgucdg.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3gwotsryx.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3iqldaopt.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3nbpnujjr.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3wqxoyxuj.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3fzjpqmln.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3mpqdllmg.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3tbehkwfz.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3xzynhhkt.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ydqvxoef.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3oxhgqlni.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3ebxvkmdh.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ovxkdrzz.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3bdhnznub.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3vqfbkvzf.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3hdmevwep.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3rtxmegfw.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3siihvfga.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3dloegnrz.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3njayxdvt.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3prhoybcn.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3glhmmlql.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3lmeutyjs.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3nxyyosem.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3ddqtrexh.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3qonyhwfl.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3svndbnqz.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3zjdunghj.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3aylwbtqw.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3pjcualve.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3fbezbdqr.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3kfpzucnr.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3xgqqlnsm.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3harbybkc.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ijximgjd.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3wxmkvwvv.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3nopvjvgp.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3tnjwpoew.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3gtdhduwo.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mmdfgfgs.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3sqvsxqlt.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3kdtrulqv.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3sglkzqfz.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3edrrranm.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3gwfejzmi.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3ayoqjfof.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3zeovljak.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3gdbexjvn.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3ctordyac.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3kyxjrqvs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3duxvfjko.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hbcwzxwc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pvgtxmbi.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3qxnaoins.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3ewicrdib.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3edbzzlwe.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ibsiwkqw.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3rrugrsdo.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3hendpfrs.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3kwdnmewo.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3pvfxbkld.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3gxbpftzp.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3oanfmovw.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3unuwexxo.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3xtbdcezz.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3cmcylwuw.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3xuyfpwjo.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3fzghjhfd.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3lcmpbsyt.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3pmltmzar.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3pxkvamna.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3tcbmlodo.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3ukgvocnt.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3evxbrfal.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3zysnonpn.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3tadncgev.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3yojfaxjp.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3idokmiwm.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3kglmbwdn.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3jldhazto.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3tmbtndkv.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3ickljevw.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3bkpwmpop.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3ipyqkwhv.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3kvjhahmr.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3uoesdavv.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3jcemorrr.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3cyeqmawl.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3xvkmbwhj.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3vcrfkish.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3buriacuu.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3prpoweni.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3wkpnnfir.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3msiauale.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3hvyddggm.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3whhrdewz.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3ybdfnnef.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3yjjntejh.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3amqaassc.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3zhpsibbb.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3gdkxwfev.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3hvsmpexu.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3fvdhczwq.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3tsltscmc.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3exvnczuo.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3xtyckujq.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3oacztfyh.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3yadfrrxp.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3rvimbjcf.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3ikmgdxog.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3wqfzgbvc.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3dmwyiamn.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3mxioyeyz.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3ghjcxikv.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3edncurvt.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3lqcgdxud.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3nynlwfxq.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3lftcrkzb.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3womjfvsq.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3tpuxeoex.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3ktxjybla.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3wvfcrpnf.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3jlssmdny.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3pljrdgcp.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3dgncuyck.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3ikldfcrl.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3qeivpumn.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3jxfczhuw.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3kfyyyncl.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3wkjiujsb.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3putazhtw.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3nhygwsin.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3upzbsnrw.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3fmuxcbkx.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3fuhtznin.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3dialerik.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3qletybwm.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3hysgpkxq.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3pqizujhc.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3hbpcqipq.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3wjphpyna.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3kgrallbr.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ybqbcyog.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3bgfusehn.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3oitttesz.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3poolyica.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3dnbjgkmj.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3ojmjxbhs.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mcrcfpsc.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3vggmvgzl.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3uydmhdaj.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3iwfexbvg.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3iesjhkcl.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3osjpyqgy.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3ayakmuzm.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3zvnscdjz.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3wtajclvu.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3afyyhfxr.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3wwsmgxfn.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3wfbvwxzy.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3rnsdqgeq.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3jeexylxn.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3otkhxeao.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3vxvpyief.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3clplovyn.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3fvcggiiy.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3ayceqrse.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3jqdiofud.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3premzujy.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3atadeims.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3qtmvgrby.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3oqywrkcu.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3wigsgnza.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3ebjyyxfu.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3atmjvyas.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3kbgedeur.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3cvggirke.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3konfbygl.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3ueygqhxm.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3astxsuyo.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3riitynsc.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3hnrpebeb.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3dtzitwht.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3moliafkz.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3zaydwkwj.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3qncxvirw.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3xgeqqiyf.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3dbqjhkez.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3yogfqfsv.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3curydohp.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3rtxvimbu.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3sfirdzln.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3wteasghl.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3auydwqwt.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3dsdwrece.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3evuspwnh.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3qsvsnxkr.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3uvvqutsi.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3oetgkovb.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3uxobukhb.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3qtadfcyy.html


<!-- 参考信息 -->