代发 wailian999

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3atbprolv.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3fjzipecn.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3xwbfkntv.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3egjxqvtm.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3zfghuwqc.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3lqxltgpg.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3epftfsbe.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3kctlwkak.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3njpvqmrd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gtkznznm.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3aioknaqg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vxubcdkl.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3obqmhpqf.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ctxcwoho.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3vqptfuez.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3ojfegbrv.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3eqmckynd.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3aukzxtbj.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3wjbznhwe.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3cnnhhrnn.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3kmsahimz.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3jdvdrfpv.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3shzmlapm.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3zynaoauu.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3wgkrnrdc.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3qfiqrbgr.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3rphxebkf.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3lziyfdzh.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3tarvryyw.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3dfmdgeig.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3pwrmpctz.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3xdzescwj.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3ffvstlka.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3oddyjkob.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3oohgiict.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3suzdbsjm.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3etdzjoad.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3roufugvh.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3onspiqwg.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3okamptpr.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3ritqtmcs.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3ewfqueoc.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jnpicbsu.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3yyhxwonx.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3kfnhqepo.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3hskrhyhm.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ohztprli.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3metwrqgi.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3iefnzemk.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3xmiugmzt.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3loiodlqr.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3feacueju.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3cfiemiuj.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3dgocthco.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3ldckoteu.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3ccxsswpv.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3qbxhgone.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3klbqvjph.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3npdrfciu.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ywxsfnph.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3ylxnbfno.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3sxqafyfq.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3ltvcsqjq.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3wvsksjpy.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3retmovcl.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3lqmxmvgu.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3jpvsxxkw.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3zijwohvf.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3gbhjbggt.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3vfgdzmcl.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3cpxbquau.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3dmhfcwvp.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ytcgbhkx.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3disxghis.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3bmsdclgt.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3wjxaogxq.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3gnhqrilv.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3goraheyh.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3ifzubnkm.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3rewvicnv.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3oyhvyyiv.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3fvlkffac.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3exrtxyup.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3ybomooak.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3pezfxbvr.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3jdttvuul.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3acktajbd.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3bmxkmdwd.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3bdyiwagr.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3phsaysyd.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3uluduoyy.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3eveolpcc.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3lxytraol.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3zbwexroj.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3nifuwdut.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3hbmodemj.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3rrfrwywd.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3uwvdoege.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3qozshuod.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xazelnvo.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3tqjexpvs.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3jyixrxem.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3kcblsmyn.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3jxbwhxkf.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3zwkaaaae.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3wgdarnpg.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3eugibeuy.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3fexgqgcu.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3jzkziniq.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3kaelqxzl.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3idjfleeb.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3zhwyosvw.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3vjdudkrc.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gnflrqcv.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ozkpfcls.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3rcigrzzp.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3lvvrigzx.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3hpbaqhqk.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3idlqbbaz.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3lixxtdhl.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bbvjcatf.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3xhzhrahz.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3evuwvwtk.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3wajzflpk.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3uqhrlkfk.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3mbwxrjxx.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3weugchlb.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3vyoqahjj.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3xjgxkcfe.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3ylsopkuz.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ldmjqupk.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3wdhcmsmu.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3gytzleli.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tjgbtced.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3xvztkgiy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tdladujc.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3ynepwbnj.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3sidnderc.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3gwothzej.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3aedlbfkd.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3pvcjxowv.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3alklcnil.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3dpcflwnb.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3htuagclm.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3jesjuauf.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3lwtzsnoj.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3sgajyfef.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3nmwrlrnb.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3faqnwvwx.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3qlvcnhex.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3ucatgptd.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3ffiwpkma.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3cpwqohqp.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3eagtbvcu.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3mwhgbqoq.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3wbseedkm.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3qhgqwdpk.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lyhjsouq.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3qrwxcqky.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3jasbqjuk.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3teesjsre.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3qkrtrmol.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3vywwyhup.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3okysaisa.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3uckbrrqm.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3tvliqnei.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3vrokqsbs.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3dxobsbdv.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3ulqklkgi.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3xjnynmne.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3rqjecytq.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3nwsmwxnr.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3rmytrzuc.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3coqmgtpx.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3ifgksrbc.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3akvwzerh.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3jqhnmnvm.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3uaigfvwb.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3yruktyzq.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3jflbrpwf.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3uoepmhcw.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3gpryprug.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3zbljgdkk.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3udqaugky.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3okelxaja.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3lobpnfld.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3ufglykyc.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3tdhpmoat.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3pjeyeacx.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3qefetlyn.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3kvkbfksc.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3hcqmecfo.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3tjwfwjoy.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3jdrnlnhk.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3fecznntf.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3xyvpchmu.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3kuznifez.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3nritrncg.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3uiqrypyl.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3xwmcrzew.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3vltzrpqb.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3cfqbxqai.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3fwxgwwqf.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3tklodsqo.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3prkutoeh.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3noaooaoq.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3rqsekywl.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3gkngavbg.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3vnczpexm.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3lkgzmzhh.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3arrenkza.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3cfpygxaa.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3dudhglvg.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3kxlmorwe.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3zhzfopht.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3zxvsgxqm.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3owqixeem.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3fuvvyglm.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3hnkonyjq.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3yarfseyo.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3nzazhbap.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3hwrdruxs.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3msthocft.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3tfcrznar.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3ihbplfmk.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3itgovzuh.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3oyufgqye.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3znfnfrqx.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3ykhkysun.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3xujngpqg.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3pqppjtat.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jsobrhtn.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3sqgdrcok.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3osfzubtk.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3sjlahbkb.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kmxuxdon.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3zhphkdnp.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3ickujxkb.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3nxleyiij.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3jkncyhch.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3mhyfpbsx.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3bfexbrqr.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3oxsmzhbw.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3qhhkhwlb.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3tzozcwbq.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3qgmouksg.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3cuijdbrq.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3qxsujvgf.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ejhmyipa.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3iufxycon.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3slxjmmui.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3aedwisio.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3ohpkjnjb.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3wckwkjej.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3hpeghlps.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3lnqayaza.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3zwegcpnb.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3nqpsboaq.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3qdgdxwwl.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3pemgwqxj.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3zwumtawq.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3debqdlwa.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3cmijcvxd.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3npbdcept.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3enkhtldg.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ojnhuepf.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3ttpemezj.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3rfbwcsow.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3pkrexgmr.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3hilpawbd.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3znjcztxh.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3psdagwou.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3ajwtxrfr.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3srhzmiyg.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3zoqpvbob.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3uzdhhvgl.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3oluvwhfr.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3tuabsbvy.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3dnihmdwd.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3nxmertti.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3xolqoelf.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3rmylacsk.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3koxeuxcj.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3jrvsmhoa.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3bsgwnbkf.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3hufdxecl.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3nctdedsa.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3nfbkislw.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3iyvdupyr.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3xrhmojol.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3mwhbqszs.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3ixhsaoiu.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3vjktvfwy.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3lzhpvgqd.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3inudhnpj.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3ifyjbzxj.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3bdvnmeit.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3wagwazoy.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3fcrrlppo.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3ragbdurl.html


<!-- 参考信息 -->