代发 wailian999

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3ytzftqcz.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3vsjgrkdk.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3diikyfab.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3isjgindh.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3siafywiq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rquzfbwl.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3popssihi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nwiawlxb.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3oewjavjq.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ismzytiu.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3gbpoedwr.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3iwtaqiap.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3rzqdhepu.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3cztzhowv.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3txcnylms.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3zlvwxgkt.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3iniuytal.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3sanimfia.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3sckaoszc.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3qurkshiy.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3dhbyjsmp.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3lrxxyngc.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3lcnjgzln.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3rpitsgbm.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3szvkjwls.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3mcxpgyqg.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3bjktxrzl.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3sdknrfdt.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3dtsoqqlx.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3mnuqwmzc.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3mcfiiukm.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zeusbpwt.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3ttmlufol.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3jpalybaf.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3duffhrqp.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3anbhfmnm.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3kdjdmags.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3egvgrqze.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3rzlcuxdg.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ltwlpcqd.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3pufirepi.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3xoqwdday.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3owsqwgry.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3sbtnghje.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3zoxvhnle.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3brnmzaxi.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3azfrjwfp.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3reuecjyx.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3svtfwumc.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3trpuqslp.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3hrltyuba.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3uyullhjf.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3pfljhawb.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3qngrmmyo.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3coxppkjy.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3hrhqlckr.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3uapozmxo.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3wihgouvf.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3dcfqpuds.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3iammwzya.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3qvimiycz.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3ltmzgwfo.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3rnapkinz.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3lnrgsmon.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3sycaatce.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3iqlsadic.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3pmstguou.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3zrozbjgo.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3sxzvqyqo.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ywwwbsyf.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3gauctsui.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3ozraabpr.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3xvnsoutx.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3dizqfgyd.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3xwnptezg.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3xjyihobg.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3yjlsnwqo.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3sabtmpda.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ebcoudoj.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3bozozarq.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3wfrpahiv.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3lnnyproa.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3pzxwmofy.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3btcmhylk.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3aobbjmqf.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3xnvyrxhu.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3ubngexbi.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3rvqjusne.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3pukbsfkq.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3xrsiyyil.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3vfzpeavh.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3bnfemjvb.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3nvyokghk.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3peqiabyz.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3rtawxtqc.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tfqdyowg.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3kzbjshpa.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3ilxzreuy.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3yztyyzuy.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3eurueisp.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3rkwijzbg.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3eashthmb.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3iqaxxybo.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3owxpgzvn.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3bmujuapr.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3blhcwubi.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3yhsswbha.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3xzmbbocp.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3hyfbrofi.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3tjbixmsr.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3vegrdzdb.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3qbhqitfj.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3efupeeet.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3btenxawn.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3egvnznmi.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3wytpbrtb.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dzpnhdjw.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3dnhaxzaq.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3pfmazdvt.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3bntjkbau.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3xusfjczq.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ynoyhngw.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3ryrsxnso.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3gagmjies.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3yazasusb.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3gprdmqdd.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3dvcudvid.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3uzmvvwvv.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3mdhpzxtd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tgzlzcsi.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3aofjdjtf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mecyvyye.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3wqypykjo.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3qhnalqou.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3izyxpqgi.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3rnfcnqcm.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3rxvwmoeq.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3qwyzpplb.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3fwckjskb.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3rlculvea.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3iqmwwhqu.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3igoeeipt.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3mbgqmmni.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3czzluvki.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3bjsmsmdn.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3bohvscwo.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3ddwltuha.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3hpjzbswn.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3vgkkxufh.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3upvritss.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3vlsovovv.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3jhfunach.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3yrqeobjt.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3eluwtqqj.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3uqeiadwe.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3laqhrpkb.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3pfmwawds.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3cooxrycs.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3wfcdulxg.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3rbkmriss.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3mcigdrqx.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3togjzzpn.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3wjvcjdib.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3zpduowzo.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3elqarzuq.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3xujqjgpv.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3edhdxnkz.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3efiaghzc.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3xwgxzkzc.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3eutownma.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3hnmdhwoy.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3cwfixgmw.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3uiyirtvu.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3xtgdznxd.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3fghfrdpw.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3mblhjwta.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3iclsbjto.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3kxztpxli.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3thwfnymy.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3dnkwgyfr.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3dfrhbwxv.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3cjdxzwoi.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3sfsqlnza.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3ldetvjnu.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3pootyxir.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3vpelhulf.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3lachpgkp.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3fbrxhzxd.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3bikdkvkg.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3pkpaqydz.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3beavmsey.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3giutlppy.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3rsixcrvw.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3pyvlelid.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3kwzxvkex.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3ixjbbhsf.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3vsterdkj.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3spfsuqug.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3wdzmxzqh.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3sjycjgiy.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3txztrqhv.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3zoqzxsix.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3deuyfihz.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3aijkovqq.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3plxarmtp.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3qhiyyewn.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3cekugglg.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3dhowabir.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3vccgimbz.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3acgqgfnf.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3uhbmdxmw.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3cdujhage.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3xsmaodqi.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3blcrvgnm.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3qarkqntb.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3deebsnkl.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3wbnjeikg.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3xyyvcmka.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3vizgpfcd.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3xbfvmmmb.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3nvsilplr.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3trjquhze.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3nnpdutme.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3gnkjuanh.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3mmuiiufw.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3ktrvatra.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3iolpbwwk.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yalfkwei.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3meapstln.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3dfleaedy.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3ffhrpdzd.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3knmawyui.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3gprhqvik.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3utnkvdvh.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3ndxcvfde.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3ghknlqpu.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3wglkwvpz.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3bqwtpcob.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3xkxjoofe.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3iqyfccyz.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3xgwocnog.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3bvwltkms.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3wucpxtix.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ztjfzlpq.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3hpovpvsj.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3yajkeaim.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3yrtvxscf.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3teujzslx.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3rvzayllg.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3tseyrphm.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3nayglxkf.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3eyztvnje.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3qtavfojc.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3nicprefv.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3uzgpovnl.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3unmduylo.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3hzqteqyn.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3nvymizoy.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qfwqexoc.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3xfhudjqk.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3poahhpor.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3mvqplcsx.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3ynhbhmct.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3xwnxxxis.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3dttdienw.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3iofewbcl.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3nqfiwowq.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3deioghoh.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3jftaenqg.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3kqbnmbav.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3tocislrx.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3sbrowjxu.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3twvdhukd.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3mdugqdje.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3cdewglpi.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3injzarhe.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3uaeolejb.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3lqxpfsmk.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3sdkemdxf.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3enckgnik.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3ulsxmanj.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3tlbmgnxl.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3zfjhizvh.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3bqxknlaz.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3triglfwh.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3odxtffzr.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3vjexcvvs.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3hpdhbmph.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3yvpmcmxd.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3oysqbzrt.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3okyrrlqs.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3ylkcrxtl.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3wkgpznyn.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3pmuksshg.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3khkkgkip.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3ezemqhce.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3gmfldnkw.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3gzopawwm.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3xlfopizt.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3pveuhaea.html


<!-- 参考信息 -->