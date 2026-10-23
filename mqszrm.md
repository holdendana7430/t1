代发 wailian999

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3zmpmfbdy.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3axfretcn.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3ozhqpyso.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3rwrilkik.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3pscljmgx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uygtlbzq.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3nyhzixop.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ugmskqrs.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3symlnmwe.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3qyosxquf.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3ikcaxemo.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3yjizlass.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3vfpdprfd.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3rajvwxjy.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3ofekowkq.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3mkdzgfyx.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3jrheljjx.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3yvqpstfw.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3xfaclyig.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3rqxrinoj.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3ebvduxlt.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3utacepoi.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3mpatxdfn.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3xnwlzibd.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3bkjmmktc.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3zcbniotp.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3apmcljhl.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3trlvnphl.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3vhvuxebf.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3rynkjiiu.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3jjwtkzuv.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gunidsph.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3bydmvloi.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gycnmwni.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3wtdmmdsm.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3wcrgxdsg.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3jolojzeh.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3toletdnc.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tcytdeqm.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3vmuewkar.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3zebszidt.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3mrdvlbpv.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3kpaekvqz.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3vpnxkwzn.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3tjxfuvmo.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3pgtmmwnp.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3moxuqtkr.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3lxriyqaj.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3klvhqpjz.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3esjfohii.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3pyxgqjla.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3zeuoufxt.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3tsgkbnya.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3vgvjafvo.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3dnksotnd.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3dzbvzkgx.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3jaepbubr.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3dmufwvou.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3dwumemsd.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3vohxnfba.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3vthbpwbu.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3npvdjvoz.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ftpfprrp.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3bqbmyete.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3ypqspsfy.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3aujmdocs.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3qxsjtkch.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3tuehdllw.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3pvzjpzbs.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ycocfraa.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3mjszdekg.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3neaeioyq.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3dfixxgqh.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3njwailie.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3iwgdwwiq.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3aippdqqb.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3sdbkxnax.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3dhuirbcq.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ayjsqxpq.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3gbogtwlc.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3pwxuxbyj.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3xgxwzzit.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3vzdyrtog.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3vbrqeang.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3weoceevl.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3mfldingc.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3upyyurgz.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3qhpdzctp.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3dtmgmlub.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3xkljhnli.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3hjuywlms.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3tbuknzuu.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3pvzvktgc.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3bgjaixwn.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3eeosqgec.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ympefejy.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3alxsyeje.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3cyadxhmy.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3aozsgngs.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3fscokmza.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3exhnbhte.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3pbbcctac.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3ytzpzmro.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3ugrkawgb.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3vpfrkilo.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fgyofivf.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ciqpeqiy.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3trwxagdi.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3uasbjqqs.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3txfwxgim.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3xczcclvg.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3mwkbosru.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3tjfepfdu.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3uqscnthu.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3sueprnzb.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3cxhtvzhp.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3thcxdkjh.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3qpgdidjp.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wwszxvqr.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3ebkxorfa.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3fkjawjuu.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3snjxehfc.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3qbolspxf.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3fecvbmuu.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3uozsmnaa.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3cmijrdos.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3zlyhfilg.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3hskjbpky.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3eohouayp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gutdwrvk.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rjepytku.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iykfcgcg.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3xrxxyiyj.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3oidacbzm.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3pqgiqwov.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3cqgfjldq.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3eckipqae.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3fwkgyttk.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3hufbmldt.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3yphgrreb.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3pfakhpxl.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ojhnkgpy.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3djahjhkm.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3gikyzqga.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3bfsgnrtg.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3zftiokrl.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3uwtotbcx.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3yumsiohs.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3dlhwando.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3fhadyvhy.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3oxaotdhn.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3qxcesmjj.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ojtihzzm.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cuvlrgug.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3puqzitpo.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3fqjitldm.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3kvdypptb.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3exmislhx.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3weibtucv.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3wsmcnnry.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3rrjosxxr.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3wxknphny.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3ekopsuel.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3vsihykhm.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3lylzuxvp.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3kxgrwwpb.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3ykmexapz.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3tmtdyglq.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3szsjraga.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3camtftbk.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3behymftg.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3wsxjghyt.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3iphsjbxq.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3tqiwdiii.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3lcrlyjnl.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3ypxcgfjm.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3dedsbkai.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3sxrifmhb.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3srritmqk.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3sxyhtyxw.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3pwlpbzyc.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3xvxgnrck.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3mhaxvkml.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3iuqcegmh.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3rtgzwire.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3lhccgtwi.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3iouwyney.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3xpcioegh.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3xqlcrmrp.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3ykjtvwlq.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3ohwuskur.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3cubyhusk.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3cwzhnvob.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3iuyhldgc.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3cjxljffm.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3rmyailtl.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3xfjvugrm.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3kwaejyax.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3nkudntoc.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3wfauwaev.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3tcemuefk.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3qxgenafs.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3sxjgshde.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3tsqflwjm.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3xbjmzjcn.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3thaxknxw.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3xsbbuaid.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3jgvaohgn.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3immlooqy.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3yrugukvt.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3wheijxjo.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3gufcpzia.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3iqiszbot.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3efqkdmuf.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3uotaukeg.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3affkjlgm.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3clrlaize.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3vutggtpy.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3viwpsiac.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3rjtbchwc.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3zcxtmkiq.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lfiziqar.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3rwpseovq.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3wyztdsaf.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3ydqmupyk.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3grzajqwh.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3gazakngr.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3vwjjkwnw.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3emmwpvpf.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3narcrqzw.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3xymcjtbg.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jdttfafy.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3nnnhuvxh.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3qljoybrn.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3kczcdpjr.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3trtvlbef.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3cirbfrcn.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3ntkawlwn.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3vivutvmx.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3hjiztkix.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3lldlahcv.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3gpezyvyr.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3dghgywfm.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3hbmdwhfp.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3gwifyvio.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3fpdusieu.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3gpupdrbz.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3tmbluygb.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3grsmrffm.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3uoazojjx.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3wnjfueyq.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3cimqapnd.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3tzyhqxmq.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3qpttxfyo.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3yjluxcnz.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3qedyutic.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3mmegoybl.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3zydluieq.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3mgwkwqob.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3yfldtrva.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3jyehmfjl.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3gxxwgbxa.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3aysbgjlw.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3gnhtjigl.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3fumjjoqy.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3ovlznsci.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3fwigbzyt.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3nbcfysbg.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3rwgcdmta.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3ajazugda.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3sgxryfvm.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3gaxydkvj.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3tlhlsqyo.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3ocmtbvok.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3nwgbijrl.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3bfylvuao.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3ohiclmux.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3akadnbat.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3tirtahhl.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3zbyagzen.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3dfuzntnm.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3ehxpcqab.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3rfvrciuv.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3qciylxst.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3iwydijfs.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3faimcsox.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3rijzetiv.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3jeadgnsu.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3rafknpas.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3ftgwtjva.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3wpcmagql.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3pmjypaec.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3nsqwtgqt.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3rhzbsiva.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3gtuucvly.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3yskchjzv.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3clhphoud.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3ycphjymf.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3dwkvzogf.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3ixkgnqhy.html


<!-- 参考信息 -->