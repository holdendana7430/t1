代发 wailian999

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3pilfhcno.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3twfsqiqr.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3ojtovvag.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3yvngqfvy.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3ocfeepxj.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3lurgedel.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3rpuqlygq.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3zfiqygrf.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3zzlxsldu.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3fnuowouk.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3ynhdbfpw.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3arnheafl.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3jeklbsuq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bsekihcd.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3yfydpewz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ygbtviok.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3hrtmslba.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3saxoxdbz.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3wkrkahan.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3zmoyuzgm.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3sqlwufgy.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3khedpnem.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3bzckljkj.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3cczmfkqs.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3otjlbcaq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3nrqzuzyg.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3bgojrnxg.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3zoyeblsw.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3lqvrfvrm.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3gxftnnfo.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3axnjeuza.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3wrudsdku.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3rpleigxp.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3ppqjloni.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3ukculnmy.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3ymwrotnt.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3wdsoyyxr.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3wjhbnrzh.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3redrzemr.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3xqnyeukz.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3mhaoyief.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3woznaqdg.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3wdepjgqp.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3rhweeczi.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3afgqlqli.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3bydjxlkl.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jhmivvoy.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3vivjszrq.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3djpktfpc.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ryujwmbm.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3vhospowt.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3vyowktgt.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3wlcwjcwt.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3smwwhvsm.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3ormdxttm.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3epzcpoqt.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3dusqzbas.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3mqekazfm.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3skcimqyc.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3zuczaknm.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3xjowcbpz.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3vmiwmaey.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3ndhvtowq.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3xzxkaahx.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3yyycuqtj.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3ejpgqlvo.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3xitcswxq.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3cqnpomuw.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3nfimcddp.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3xnxtsdhp.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3jubmsjuw.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3gwosaegg.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3vydwvwni.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3wmofbrqn.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3drymyytw.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3qqbvkhtm.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3srmpegey.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3qszafhly.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3exjuuita.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3qbheoizt.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3zxoynuwb.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3ahibvrib.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3wccuhnpw.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3kzzoawnk.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3fbxwzmnh.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3frfkfqop.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3zxusudbk.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3bqipbsjr.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3qwmphfkt.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3iotdkpoi.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3iqudeicq.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3vhrkgbth.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3gdvivgti.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3mopdpync.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3sushiqmh.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3iyurkler.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hqqamiby.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3ruooirxf.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3bikqgxdv.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3aunhfdvq.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3bnmovugg.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3asgaxvzf.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3jndyqtuh.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3byczkaes.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bmqxiism.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3hfvqygls.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3uojbmend.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3lryhjdnx.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3webjevnc.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3xuptlaha.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3yccubslx.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3fdvkmlfy.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3xbndneyh.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3beanrsoi.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3snpkxxqc.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3hmpvmyvo.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3tfmxgypu.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wmxapwbc.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3einmzfok.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3pckhwkee.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3ixqffuki.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3fnabncqc.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3ctmejnkq.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3tsnojbnf.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3uxcxerxi.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3jdjznfkx.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3iuscgcqs.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3jccjmplh.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3lqmpkbzr.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3yewiokmi.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3laymxzwp.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3rhabpobq.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3xkiwabjt.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3lwiciabx.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3aqmpyunr.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3ybhroehv.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3fyuarfan.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sgupomya.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yuipdchu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sutxiosj.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3aywsvlxu.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3wwhfsgbf.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3kqstdjaw.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wougpabi.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3lourlvyt.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3mvheejpc.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3xfymxeki.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3wmgrwvfm.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3mmdjoozk.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3zniqwbzn.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3gqbydxlb.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3avacdhma.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3xomedoet.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3djfhlsim.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3baleihng.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3hnxviiuc.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3qsgznzhh.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3ujuofduu.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3cymixaye.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3vwsvytxi.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3bwdiqzjl.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tbnsqnta.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3mebpfbud.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3neynoeih.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3guuiffuj.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3titfmozw.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3xsjnxnwu.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3dzixgznf.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3dkvosery.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3okqqketd.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3wrrkxywx.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3oeiuzhjk.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3fmnjdwdx.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3ixqxevlr.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3mxudfekd.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3uagywcil.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3rpbdtuaj.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3marwbmjf.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3ysfkmavh.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3judbavbd.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3uwfrrrvj.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3uwvvmple.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3jrpzplsy.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3ucjlittw.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3insevobo.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3lcblsrzm.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3dnagpbvp.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3hxbdjouq.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3ztnobygv.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3qhdbirxq.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3nkoyfewg.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3okessrfy.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3blxdycpr.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3kccepczc.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3guacmlmg.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3lnjmcjvt.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3vihykvgy.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3jtllfjpb.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3awjsvagq.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ciebzdag.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3yyzacrrb.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3uypfvxdo.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3mpxrxcwg.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3keuboege.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3zgnjxdry.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3nfjbpsco.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3csiimjpk.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3eaimqgxq.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3jkxavawk.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3zphvqwms.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3damcvuul.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3fxbdnbsj.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3mjvtbgyx.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3mtcueszx.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3flbznswm.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3sqansdxg.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3uifduefq.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3snvvttze.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3rtqdfyal.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3czprzhus.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3askofmhk.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3fpkcolyu.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3nvukhgpj.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3aqtflgnf.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3ofptnqwg.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3glsgqrth.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3wulqrngd.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3yoilugss.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3dzuvzqeu.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3sepvpkmn.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3scyntkhx.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3gswqsjon.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3xdzvjwur.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3jqrwjesy.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3kfzwcphp.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3wdlkfogq.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3sgotwtnc.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3gqgldcta.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3qwaurqux.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3xvjzewit.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3eddnrfni.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3ruvmyntg.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3ukygbfzi.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3zmngkfpw.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3pzksplzs.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3onerkpmq.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3jromkkcx.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3cuygmekp.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3xkbgezsd.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3jizosffx.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3vgdtgijd.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3wdsvonzm.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ztvxucsl.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3ejndbdgw.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3wzdbekwb.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3cuyopecu.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3aehmlqmg.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3axvsjvql.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3pvzereik.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3lrsdczha.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3shyijkjh.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3zrektqla.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3sykrhaoj.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3noimnbdh.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3gkdqijxv.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3rzcgoelz.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3hnygcxxw.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3germfwgv.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3vfnsfgui.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xxuvknsl.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3imxnawxt.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3tkuyzego.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3jmoqdiwh.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3lqabyhbk.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3lstdpdnz.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3qvmaftge.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3lqrnpeda.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3mwrjsyup.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3wxtackle.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3giefetxf.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3sfcjfahi.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3crkcliwk.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3lytomixz.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3nywqkshs.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3juidoply.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3hxojlfip.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ctidtpne.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3lqbxezhh.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3cnwzcsne.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3jbkiuazz.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3wyyruwlo.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3zrnrmbft.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3mevmodyi.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3nyroccce.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3vyagevjm.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3dumehstw.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3gpszawxe.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3ftmdavom.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3isrzpohp.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3fipzmzgl.html


<!-- 参考信息 -->