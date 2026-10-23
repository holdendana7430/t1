代发 wailian999

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3hkxbnmzr.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3shkbpcdc.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3obwyogee.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3osxckwfk.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3jtvxdbax.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3wfkrdiso.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3xuesaphl.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3jebswvlq.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3olyomxhq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3exeupkmb.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3hccwvwxg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bucgmyly.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3mcjiszrv.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3otfsjiuh.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3ldgzmecj.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3fldbijbx.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3vdiqisac.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3rshteaqh.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3kmhhfohe.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3omzurtwn.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3vvkigmso.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3ynhuomzg.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3vlnaswfe.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3hazyxvun.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3mnkomixs.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3fucpjudh.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3yefymycz.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3eeefcxyh.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3qmndkbbj.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3akouxrbk.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3umrkslxe.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3dnpiehvn.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3yiwjfmqw.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3roqfscda.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3kzcjjbqc.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3mxjsfpvg.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3wwtdgybg.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3wloqbxvq.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3yrcyfcek.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3acqzumkx.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3vlexcjae.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3eqsigjdi.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3kwpyyrzi.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3jslthdnk.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3vgjpurlc.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3bzevvrkp.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3faldvaea.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3dsseaizz.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3kwnrcbji.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3tddidapi.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3soxznopt.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3ymvwmnac.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rvjfuyas.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3isfkubuc.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3rmlmonlq.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3ufmiruna.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3tnpuemvr.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3rwpwvluv.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3ptsyuswf.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3nyhhuzxy.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3gbzlktcf.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3zwnckjvp.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3mktmeuzn.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3wjgewzhe.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3opryqahs.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3rnzekqoz.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3jmibvupo.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3pcapjtkw.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3spkylceg.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3flqpakol.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3udwkcvpn.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3ugdrdbvh.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3yzsotlce.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3aqbqrhqp.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3enqphsse.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3cozbdaog.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3kttjvixs.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3exdopyct.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3jpgywrjy.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3cxkqylxh.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3cqtuvduo.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3psbzrfmf.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3vxvssald.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3lqlkhudl.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3vyyyrvkr.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3epjeuhyl.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3robulcxz.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3ugvuosij.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3jdgunjdv.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3jmawlvbv.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3imgdwtlf.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3yeadrjmx.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3erjnmnbs.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3eddnhvan.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3cgnoivac.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3phvpocor.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3dtualxjs.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3dvcrebob.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3holtitmj.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3dpoqwbom.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rvqjuwfd.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3inpibuks.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3grdmnkvo.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3hetgttog.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3pvluhkml.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3qgeygmaj.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3gfanoheb.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3ihtpmyup.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3unllecaf.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3uvljxdni.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3irrbmsft.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3inemqiht.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3naegwgbv.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3kxbcjnuy.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3rhlxekyt.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3ysvyynds.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3bjroiaog.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3zspuwkdh.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3pqejhyvr.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3zewqiqgm.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dodyircg.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3exxfilia.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3zycselrd.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3ojipyggi.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3fwadrhys.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3xsfcbvmj.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3dakxyunh.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3zxofhznd.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3cklsnwom.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3eyofoowz.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3qzpvmjsp.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3anrgcrmt.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3odobxhhq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eouyazqa.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vfitrutn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bkwmckhk.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3pubbhdvu.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3dvhizcan.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3yfkxzycb.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3pwdeotpp.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3zbwavlwb.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3thhyytul.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3wofdtono.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3qqzaafsz.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3amqkfmzf.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3eekqdzgr.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3mipolmvj.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3adziepha.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3ttapcfok.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3hdsxpgbh.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3jumevrls.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3uvgjaope.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3fajjsmji.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3tzfobqmn.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3szoxtsnk.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3flaanpnm.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3pxdmmlxn.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3kaqmfafc.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3huejjoeo.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ifinlhbs.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3nbsvhvfq.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3mkidtvwo.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3vxcneeqc.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3wfnzevvk.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3pllbbrbr.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3wppgfrsw.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3joehbazc.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3mffqcrgy.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3kbhwhtul.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3xvshmsjq.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3vzuhtrip.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3iiewnmmz.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3xqzmbsgs.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3tsgtauzk.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3mgjjhoyg.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3tmnmfveu.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3hzscbgrw.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3axhibmvx.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3lhyvxfac.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3hpcxkeaj.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3kzkhmnac.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3qchgcbys.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3cpzgygkf.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3sjjsngik.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3guzcfrnv.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3cqdjhupd.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3dfchvmok.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3efwptkzs.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3ckmuconi.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3swpdlwvc.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3sepdmekv.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3szftqazl.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3mzdlbsmp.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3vknelqhg.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3rcdeqide.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3yxkszjde.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3ivhhcqap.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3avxvhpta.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3zeitatpx.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3nuaamcwg.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3tarihrfn.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3hwbmeoen.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3gtgfqgru.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3pjxuejps.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3pntdvxoi.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3bwhfwwln.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3mwlqffrx.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3uedmqaqc.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3loklairs.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3llfwvdbh.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3intdmkju.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3djkdcwlq.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3mqkcwiyt.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3wtbddzbl.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3imaxnlsf.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3gjepejkf.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3farnqgru.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3qzpsndmi.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3yqjztzms.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3tupsnkcl.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3wzlxyouo.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3jrkworcc.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3rpqibmca.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3cupqbtql.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3bftekkan.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dhasngpf.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3zvswfaiw.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3lhdfsxai.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3kmdawjuh.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3snftelhw.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3qkvqynrh.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3fvaoshpt.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3sehqewat.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3dxeecthd.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3tijptqie.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yzzriyjd.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3kdtgocsg.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3trebypcu.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3vwegtpko.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3gplmvdxs.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3xbembnuf.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3jpggzkze.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3yoqhljed.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3rjxdymnj.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3mudmevvx.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3lxykjmes.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3wxevptev.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3vnnbfkrz.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3zhfvfkds.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3fazwzjzf.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3sphqazrm.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3ipfilkmm.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3trlyaoxq.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3mcceggwz.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3kesenpjl.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3vbbkmsqr.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3sowuljna.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3dsklkdve.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3coxokyoj.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3vtfputxp.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3mlivglyk.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3pjlayjgm.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qnlixmqp.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3qaapcefx.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3yyotmbyg.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3awmeqnjc.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3cagyhaff.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3svifovyl.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3bdkiinbg.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3vfvwgcta.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3xmfdzrgn.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3vhplacgb.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3plgsgrxl.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3hqpdeyks.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3jedtcvef.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3voejcavp.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3tldkhpsi.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3onorfzyt.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3lgsktjpk.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3ktevnvzt.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3gfejxbrg.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3jlmikoiv.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3apsvntlb.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3tmttnovd.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3icmektmx.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3jikukqhg.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3fmtuwclt.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3xvnbgzlk.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3iioyaxhn.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3rmshyvzu.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3fqizbqcy.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3kgqouocv.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3rgtxqosb.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3fwhzqrco.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3wldckqsz.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3kkcgtrqp.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3rodxjian.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3vhragtuj.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3ifalxmdn.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3jefceyfk.html


<!-- 参考信息 -->