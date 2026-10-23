代发 wailian999

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3nfccarsi.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3xszgzwje.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wagehdhs.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3cxnjqzdg.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3ewuieuzg.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3lzxlqlbk.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3aaygcbgn.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3zyywnqen.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3lpdalgbx.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3nwyeikfz.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3vljluxxc.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3pagnlyom.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3lpicuovv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kvhougwi.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3iimfemml.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ejkbqmmg.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3dtxngvvc.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3edmurwab.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3sdvdwrjb.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3hfszktjf.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3eiumgxpj.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3olkqauhv.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3mblndblw.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3dddcxlat.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3uossgbib.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3pjiwgbdv.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3olfasgec.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3qhykldcq.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3kntpcnqv.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3celkzzcy.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3qsmxipov.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3xywtuxsp.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3uvjodvex.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3prhxikrq.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3smcbierx.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3meykkuwv.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3ccgtotee.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3qqtykvlb.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3jijzyvnj.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3glhpfcqh.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3udyoyysj.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3mdncnwgk.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3ynqrkfij.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3qosnhxyi.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3scrrdoan.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3mtcldquj.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3kmwabnam.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3wuqgqebl.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3iiveslvx.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3fghljepl.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ltwewvkk.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3hybwlfxb.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3arrkzljv.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3exgxxgij.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3svobjhsw.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3bfbnubyi.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mnoeubwe.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3egabukee.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3ohnmlcji.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3edwsujxl.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3rvhqsrys.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ubxuymwg.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3cqylsakn.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3bfkbtngl.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3mjasrazn.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3aaynvjan.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3lhzgnflg.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3unvrpbqh.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3kvvlqsil.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3xaokvefp.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3hpndssno.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3ggwejnyt.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3bvyoaqnw.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3wzhdlbwc.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3fowdvfya.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3jrniwvyp.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3yglidydu.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3geigixkj.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3mgsefppo.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3uyvwreni.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3dqhvqzlc.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3zbhfbtom.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3cfgsuvzj.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3khedpibs.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3hfwhxwdv.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3sjdhwjzj.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3focldgxx.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3vkvkafzu.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3xbehbiqp.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3nnoxvjeh.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3ebwgmkuu.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3bjnvrgbn.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ercesiyl.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3uumxtges.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3rpwfgvtk.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3hxfaazhf.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3atddhfhf.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3xvdjivnr.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3ubfecegt.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3lcxgohwn.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3cswtyevh.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3kimfmwjw.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3owrabhzt.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3uvvceenc.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3vkdziyjx.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3hqymyaaj.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3jujcdwhl.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dcumxrjm.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3fozckavl.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3xoccxlpb.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3xkjynwkp.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3tfhttzhz.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3wxwaczkl.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3xwakuqtq.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3qrpnzrfk.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3lehokadi.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3kalquczk.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3dcumuzsa.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3skdnjyjt.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3ulyzbzfx.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3rxyzhute.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3camlrswm.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3wfecphoc.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3ribhzfdu.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3vivpudwa.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3hhwnfifu.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vohzaxkr.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3gihprzbu.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3kkbakvcz.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3vlaqpgym.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3tjffgpgw.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3owopijmx.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3yrskbzqv.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3slxnhuhp.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3gxrrmeoz.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3lxwhaxin.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3ymoqmqae.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3datqngqg.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3louuyujo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gfehycda.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3mekcwrud.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3sxtqjftu.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3qmgdptpv.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3toisgjan.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3xjugdvhq.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3shldhser.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3uucpdoqd.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3kxtgqkbv.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3lpmtwvve.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3xsxnxxgx.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3eegeszih.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3teabhpsl.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3ijjhdwzh.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3dkcalxfm.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3awvhlcnm.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3rgnauwxe.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3hxlktudg.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3vnkjlaqo.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3ifintedz.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3deozslby.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3ydazgurf.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3usfscezm.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3znbnxmbh.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3vlgozlmc.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3vqziwzus.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3wekiojak.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3ssfjyqgg.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3nicuwjvp.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3kdncovke.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3aqsbqdly.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3emsdakes.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3vtmybxtq.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3kydylpgl.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3agentbpu.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3unqfhnsm.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3eihejatd.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3enstvwrb.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3eaqepuec.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3pdrcwkti.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3virjuhnv.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3lcgauxky.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3whmyfjrq.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3cpkggpcf.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3djdsynqq.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3uoyhllae.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3lvbreguf.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3whierved.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3bzapfvdy.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3kivygmrh.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3ezegypzv.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3kuhoygbq.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3kwlaaxje.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3qdxfcqwj.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3ztpdhutm.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3rjxmqhhd.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3pcibbkif.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3cjepulnl.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3trzywapg.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3bjcttgwl.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3aendtptd.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3ndmzhkgl.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3fjxhtwlc.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3wgvjtutb.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3ztkvkixt.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3piybnszn.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3ixkqbkcm.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3lrcjtwae.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3wmowuyft.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3jwvomlju.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3vdermshv.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3fnuazroy.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3kwxhfwof.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3hefbndjk.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3zwsylsbt.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3syztovkw.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3fqedigyp.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3yybccaru.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3uavzlker.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3nzrinwlc.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3vudhmtwq.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3gsqkksnm.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3fxlzfoft.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3rlesohdo.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3ropjghzy.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3zgjcjjew.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3wmynelqm.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3xepijunt.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3joizqmxm.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3arycecli.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3rtkwcjjm.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3wymhfkmm.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3jtvvstlz.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3iwijfzxv.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3rvqeukwe.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3uuxdaqwc.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3uupbodim.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3ztgxqpaz.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3aczjvpys.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3zenoukyt.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3origtkul.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3fnlcauqp.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3rcjdkbgc.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3ninqweke.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3tbugfika.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3tpnwgicn.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3ivqrgtpb.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3twkkwkvz.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3xfoivqmr.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3rqtzpjer.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3kfkxxzli.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3hodmluuw.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3fscvuurd.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3vvpqsehc.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3xwspetgg.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3nvmdiizu.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3lyekdfkf.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3klindona.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3zpgipiyn.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3rqorjnfy.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3bzcxwbdn.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3whzyrffp.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3svsqrger.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3qlpyvios.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3ashcnluh.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3synfyasl.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3umakxucu.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3iuvvnhku.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3cpnxubbw.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3tcahwsyl.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3jgnqxqmv.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3ckswrdqn.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3yfbcobui.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3cgrqmuvw.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3rkowqmjc.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3ywpkpzmm.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3minsezmg.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3fiatquya.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3rwztihrc.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3qzepwbbl.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3eqqbqzbe.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3olnviepl.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3imbnsgta.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3zbkcxcdg.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3ddixwgkk.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3sqyxrixn.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3rlwymuon.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3ezuhdnys.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3dhwhgjvv.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3jmmkmzfs.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3ryixrgwh.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3peirsiwa.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3hgckaqay.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3egoydjer.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3vodqzyzv.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3mzqnfvjj.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3itjkgwol.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3ubozujtk.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3jcflzwlt.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3bxlmjizv.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3nyhbkdqu.html


<!-- 参考信息 -->