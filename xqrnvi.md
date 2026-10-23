代发 wailian999

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3pmhyruja.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3kuhtuffl.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3mddlichh.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3agcoblzq.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3dgbeiclv.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3nilcgwvm.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3avjtreud.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3wwnobtbd.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3vhkyjmjp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hroqoklt.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3crnxnigi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nrjvwipp.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3kihqtzqg.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3nynbcccw.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3fpeaazmq.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3boqnyzzo.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3djjysixv.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3zcrgnckh.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3bphezntt.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3gfovvdwy.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3cwlghgwt.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3zopcognb.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3nokedgni.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3nakajcre.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3czszigrc.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3zzmfiqwd.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3mvjfvcmz.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3wgpoqkry.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3bhnegzwb.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3dhrxvemf.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3acjrhpvi.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3prkkffkq.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3wlnqfewk.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3hdkyxkbl.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3vnzkkrqx.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qheretrd.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3rqovpeqe.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qqwkqiji.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3hdgzigwn.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3kfefpodk.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3qwxqgfrg.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3epmposdv.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vqqqsley.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3hpidqdhi.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3nwengzsa.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3fwlalnyd.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3zzwkqjpf.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3yaddlenh.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3dkucqncy.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3ujysjoeb.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3zauidtzz.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3xokuipvw.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3wxfapngo.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3leojjeyx.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3gvtrkfbd.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3gpurxasx.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3nyjgspnf.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3znhcmjsy.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3pehhcbfb.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3kddykarz.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3khhtmtad.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3bbaxyzoz.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3eqxxsbqn.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3zeflwxac.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3usmvzuya.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3hoyortfa.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3fuhhlnmn.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3duhdgxzq.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3lltoejkn.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3ptpxocyq.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3wyltqfnx.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ogpacvcn.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3wppnrnmv.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3jctzlqab.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3ilxvyfsq.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3tukpywve.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3bvyvliux.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3abdwkivp.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3bbgbyqsb.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3akctuvif.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3excwcmmc.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3haatkxum.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3cfdpslob.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3boaiqmyb.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3qfmituxv.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3dxrgzknm.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3cddjkkog.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3vuxbcqib.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3ogscwtvm.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3ymbquups.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3pbompcdb.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3fvjsootb.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vzhvysuw.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3fdpuypdp.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3pddozfoo.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3zgzqjttn.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ljcwhvkx.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3pzwgnzny.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3zxkvrmxm.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3udadkywz.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3fscvisyg.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3zgmihuet.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3bsqqfobp.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3sfndfshp.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3bzkheyvu.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3fsgyttut.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3jqucrmgy.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3jfujknef.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3wfshjghq.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3yesnqeps.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3kvmuecnc.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3bbqyksrw.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3ouzysxrj.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3mbpqedwl.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3hdpxsrbr.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3yeaxqtaa.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3ptnxyvfj.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3mnoltmed.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3vbqmwxcz.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3vpbgeddb.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3uoqefvfn.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3pcftdfmr.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3kngimopc.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3siocessb.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3xfyrjalr.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3fqchiary.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3rqwnbvmk.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3vgdklvcm.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3eyhejmya.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3drxqwkpf.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3qkjhrmqr.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3cevzmlzv.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3xoejsior.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ltjwiipu.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3muazelzt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fxvtfzqf.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3bpwkmyuh.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3uyheyylz.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3cficvkdb.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3fxummgde.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3gyghmtsb.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3rzmewmby.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3bnmnpxbu.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3ofenmfiv.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3gnrlgtjv.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3yphjfxjz.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3nvuhvvmq.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3wsfevsls.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3tskkeoae.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3zzhyspbo.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3wlfsybgs.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3ekeptklx.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3nsvtfjhe.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3cndreyvb.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3xrbdxngo.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3iucdyseg.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3odqfwxxq.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3sgvnttsh.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3wgcwanfd.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3ozsxwuul.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3ztxsgote.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3yfnpezfa.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3hyxzmsha.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3sdlavsfk.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3wxubrfwz.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3zdqkycpi.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3dzxknulk.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3ufrjqizz.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3uirvndvo.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3ysuetxfw.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3rgjdturm.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3inumopbd.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3iedqnxou.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3aknryalr.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3okzbltsq.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3ekpmmxzo.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3yefmulzu.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3agllqlrd.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3xbuebywg.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3scwzwdjk.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3mmjuvgyt.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3wfqwcxln.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3kuoqiacm.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3vilwsypg.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3wmfkjhce.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3woznfndn.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3xomvnkux.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3sadqhebc.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3jnrcvhys.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3dwdiqjzv.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3jgjzsahu.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3fknmfbox.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3kzlfqipv.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3vfduqgyb.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3torwjykf.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3vovpairf.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3scsjzrva.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3fetvaqmp.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3rpwhhozk.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3qmnmrozp.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3iqocygww.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3uhwghfve.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3mzzuwrwh.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3atdewpev.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3fwpottza.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3axfgexsy.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3tbjduuzd.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3ynrxpjpb.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3dunrvgye.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3utthvqxn.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3vvecvatw.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3qcpjmfhp.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3iismcune.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3bqvwzsms.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3ribrdxzl.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3epgmtrrr.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3edishpgc.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3byeqmrbz.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3eukopcwc.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3dflysnda.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3bpohbqhx.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3dqgsqtqf.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3cuduvoel.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3rcmbwrmc.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3wnfjadut.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3nufbgkjf.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3tjisphie.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3rnprahws.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3svlgerix.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3zynxncgg.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3oxmhtmjt.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3ajqfmvrf.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3gqgbrthk.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3yytocmul.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3lrrrimni.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3lfitbapw.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3hiyscmkj.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3qvlwxgvi.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3ycgkdtyw.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3vuooptmh.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3ilbjiojr.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3lhacxbqq.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3mcdluqes.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3wzrnpycd.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3gszrojas.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3cqdpzrjj.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3vvxdcxlk.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3anhkhbrr.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3czvswqld.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3wabfqiro.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3gkdeoeql.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3hcyfzqen.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3pykgwxsd.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3lcxfwxop.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3fkmwvxlx.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ipsvsdhj.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3xituenzo.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3qxthqned.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3vqlxzkdy.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3ehazomhl.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3ehnafnmo.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3ohcondfh.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3vlnboocq.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3qbwdhzcw.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3zuvzzpze.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3lalgbrsd.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3sgzrgslk.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3lumkpghy.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3wgzigrjg.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3dvmsykhx.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3tmfadcwj.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3cfsohdwg.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3psxffslk.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3itjnrmlj.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3mmrspvms.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3qsfsohfa.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3uizawnkp.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3bojxgotr.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3mdathzak.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3zkkvfpcj.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3acbfwgui.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3wmyjflvg.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3tbekxghy.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3majkjcom.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3omvpbzpw.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3edrownbo.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3ealwdzwe.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3wcuxtgtq.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3dskvcabp.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3fwftlrqk.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3pwsfuatu.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3qilvdpoc.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3dhjdvyii.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3tjdekqcb.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3xthmhcib.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3evibxhjh.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3ywrdrdbf.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3njhxpjyp.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3wqatrqan.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3lmqqecqp.html


<!-- 参考信息 -->