代发 wailian999

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3auztfctx.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3jqnndgwd.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ixckzqlf.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3glfxxfkk.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3zjoxdhup.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3manapcub.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3yadmwtly.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3mrgfpcsj.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3yyujugxu.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3bkfqjkrs.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3krpjbvwu.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3mxkdddyr.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3xsahdxot.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ndzetaqw.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3pmhzicro.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eeclmzkb.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3iekyzdjv.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3kkumnmmx.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3oxcjkmcl.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3vlgeryei.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3wxxrhaiq.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3egmtthmc.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3utyfhdds.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3azcqtumu.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3yxzzrzek.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3cwrkbkph.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3sjznqcky.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3rtwylgcw.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3wtqyssqm.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3iwoibvwk.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3hkvposoz.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3dhqhudxb.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3clsuexlw.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3qiresima.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3ajttbihk.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3rhbqmzge.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3ezoqbrah.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3zriwnrho.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3zteaaxrp.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3efikpkka.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3yxnqdtxg.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3dvtqgjpb.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3qaecujmu.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3wkuyuhfy.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3bbucsmxi.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3nflhogxb.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3klalmyiw.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3kubnhhoi.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3irsmqqhe.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3btzxxyui.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3yzizhxjm.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3qznqqzca.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3rbdgkbmw.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3rsjmzpop.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3gcpoghod.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3zbyqlbke.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3mkkdwmiw.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3sadxxszi.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3hkdkaeqj.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3jbaicehl.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3gkxcdavu.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3iuqicakw.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3onlnlmdg.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3nvhprijg.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3fskzogar.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3jevslwio.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3jlartzum.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3xfpzbxue.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3eyazgahn.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3hbszjkds.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3zmtplxgp.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3onzkuzrw.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3uvslbbiy.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3snbdjcqx.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3ahnokvsh.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3xqnilosh.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jdxmvkes.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3hkdprnld.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3cirwqkdl.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3dtttairw.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3wtwfefjv.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3hyjgxzch.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3uqhqgwaq.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3hezarrbi.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3greovgff.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3csdhaxak.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3egsgnznl.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3nhkgmakc.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3wngndavo.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3jehwjdxc.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3pjewwyul.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3tgbvpqkb.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3oyrczpzs.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3yijpfvrz.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3pfldekah.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3qezmvkyc.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3whzcjxjb.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3dxnphqgy.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3fujtrwvn.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3bvonkbxe.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ndhmdexy.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3exwbyftr.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3vjxbahet.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3aumqmxgt.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ichewrdd.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3lxxfrymz.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3mecfukjk.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3gpxcxhdl.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3rowmhhlp.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3ltawhdmo.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3qpwbgfkx.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3yjppqncj.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3ikvkwmel.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jopcixfi.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3duivsuxt.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3jpzythbg.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3iplvqsqq.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3mruwpxam.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3coyvugor.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3eokuoomt.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3oovxnphc.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3trrorkcg.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3cpajvbyq.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3rkpccxdp.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3okcsrbkr.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3mhgzcmyj.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3whvnpzdg.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3oyfgoetk.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3tseubadu.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3ngwamaib.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3ucywlwxr.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3gigxdihv.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3jqfzctjf.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3xgqypjwh.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3iwvsqkwj.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3hrmyrhiq.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3ctjonfnz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3slzflpww.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ckecoodm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wjhejfaf.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3nxhczrgm.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3aoecvmfr.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3fsqwbruq.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3dzlzkjzc.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3lmlsxwpl.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3vmhufymb.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3adetklvn.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3uxykzodo.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3fkeumyby.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3uhzvacak.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3atzuypwp.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3uudmkqnk.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3mvhxowjv.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3hurerjwp.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3dkcjvllc.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3dixhocro.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3inzulrav.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3dryazhak.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3qshzkdke.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3oqlbktpg.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ocvsgjja.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3dxnocsxc.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3vorxldhp.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3vcdshbls.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3hakkzncc.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3agnbyjih.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3zsfqtyvq.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3vuabuzii.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3kfrlokrd.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3ojunqgcu.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3muyyltma.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3qpzczgxo.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3cpnibvav.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3vuqqpabe.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3lcmcxyyb.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3avrhvait.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3obfrvcna.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3bzhgmlea.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3jqiommzy.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3qaevaony.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3iwvmjjee.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3oxlphqna.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3ychqmqyp.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3wwshdfsg.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3emgnhcme.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3ohlxpkde.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3eyymeznf.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3xkxjkasf.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3ezeoywfb.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3hbajpoiz.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3anqznrhn.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3iqiljeso.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3yfwaxuaw.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3fmttffnz.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3tqkgceti.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3sutwwtan.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3lougnvwm.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3lwciyqeu.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3yhpxwzom.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3mebofotr.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3brddvgba.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3kfanncck.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3bfxnazby.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3vdvddomo.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3rsziirpn.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3mqfmpwke.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3bltmezyx.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3vcyqszje.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3wydkkxxd.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3whtfpjlp.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3vrlarbsj.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3mzadzqfi.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3stbykiif.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3sxihpsdy.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3eeznmukk.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3eieefqvh.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3pipfgcoz.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3ztvovbqn.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3jbqgwmwl.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3zmlxqkpz.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3aqzrtmmq.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3yqarnwwq.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3fznpiwkq.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3jerdzdeq.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3jqpjhqpm.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3gzfoobst.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3ouepbhsn.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3wdtybhfn.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3sxuojpay.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ytclwssp.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3frkzviyv.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3imnikrpe.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3fpspvikw.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3ypuudphf.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3yhbknpmk.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uokytlhj.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3snqaikwy.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3qzyyehkp.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3rzskowtg.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3zhaptbxh.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3ostghymn.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3wpmgxrpc.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3qxdbubky.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3qmxjeroe.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3xwpwkabt.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3xfrqdnbw.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3jonmcmti.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3zmgiwblk.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3xitfptxy.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3dfrspgaw.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3ntrrikho.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3dzreoavh.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3bcrohbtd.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3galhjfyn.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3tipwfwfc.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3kxclooev.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3smypgtfo.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3czdkepbd.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3iffsakiv.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3vnpwowgd.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3byaoivna.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3gkltnbsp.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3yphyvdlh.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3azakvzfu.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3pdaiosmu.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3jncwuepi.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3vrtdfdmi.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3rthdqaqv.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3bgrraxen.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3gakysdvi.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3vuibnfvo.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3imyirpxz.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3afsoynnk.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3xdzefecp.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3nzoxoqsf.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3jvashjci.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3fhgttgrh.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3lbbgbyuy.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3iblgtaqc.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3drojlafb.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3jpulcacj.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3evmvzzpn.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3xfgnjtjx.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3twwpuemh.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3lmamlroq.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3umdryfai.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3kaiinnkg.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3lelujvno.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3asgcfjmo.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3ziuszhoc.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3iotnvdru.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3luqaikje.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3bxtxcclz.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3iculoseq.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3mhwoseqn.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3swxbrjnd.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3dbngjyht.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3bmwpfjrs.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3xrxmqaza.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3dmchqxxs.html


<!-- 参考信息 -->