代发 wailian999

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2isxcdpju.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2aejeqwmz.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2gdalsbpu.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2zpkoweyg.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2ykmzxyxt.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2ueftppce.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2jfqjtbod.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2girlhxek.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2iiolwwku.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zyqazfcl.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2oanlktlr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jyhdyqph.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2tirzsuxh.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2zfhmvqrk.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2qrnbaldc.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2ogfxjhka.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2oukgacjd.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2okpbwqen.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2hvkwouyi.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2zoojkwwx.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2agguxizp.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2shjgqlhd.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2zxiaickb.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2csqjmzgc.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2tkmideah.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2lvpnkjfa.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2qscesgch.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2gfpeadeu.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2dxoljmbi.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2stzaulrt.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2yzqinnak.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2zlpakxfa.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2azkfcbll.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2idqbaymk.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2uozkkilm.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2loxrjstr.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2ukkfhbpk.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2esearyiu.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2djcgipkj.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2fsmidsca.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2kestydcu.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2tbhhnoiw.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2kmtgfctq.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2oqjymbai.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2egcbfgph.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2tpbsydcf.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2moytsslb.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2zbkaataw.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2kqriwova.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2opalvijw.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2seyweflm.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2nkcnacnj.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zoaboalz.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2ydbcwglu.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2idkuppvl.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2imphndkl.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2kqgeouqj.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2stgiwpfc.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2zkfqlssy.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2hypyqenc.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2ezvpkvrr.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2qqyzrome.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2oynrpmni.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2sspoazeg.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2fjqbntvm.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2mhfeviun.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2vohtwvkd.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2vovtexun.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2yvfkvlsj.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2kiwqpexc.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2szgkaeic.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2flrqqjrs.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xneeszpr.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2lzyisfhe.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2ocajmncu.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2lolopigb.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2bfwqtvzd.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2dmilguzv.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2kjbvlick.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2rddodskk.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2zycyyryk.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2qhbztqbo.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2migbyvyu.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2zdknjfpu.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2iqlxjaqq.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2ypyodzev.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2hjyidhlh.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2osnebnul.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2wctdqomi.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2uftabakq.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2fapdxegq.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2quojzrec.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2uyakofje.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2gwmxediv.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2pnvbygmv.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2mfcqfwxu.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2wsltammu.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2kptcjaut.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2mlbczwtf.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2ijpurgma.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2yllclbar.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2qnnnxqyh.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2ghaikjaf.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2mydnrqhh.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2tkcwgwvc.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2qvspowhe.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2lshfchlw.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2kyjczfqp.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2cwnlofcb.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ulmxjndv.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2yssvrzxh.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2mcpzmhjs.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2ixqargbe.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2oqbytkkm.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2cwnppgxj.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2gizrgtcd.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2vqxuiupg.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2bjvrfhoj.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2lexwhzsz.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2izravoon.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2ucexxwha.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2lqlqeisu.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2arcsbcoy.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2aqmubphx.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2yplrulgw.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2zveymcoh.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2cmtfoiho.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2enundkji.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2bmwklccz.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2atndmlit.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2wathbwgx.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2vtgvnfvn.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2bbczorzw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2imlxzigk.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2qpwxsjws.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2quvmcgqe.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2qlhpixem.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2bqdggdew.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2neynwqut.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2zncatqxl.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2gfihidzt.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2pastzsau.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2llmtakzy.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2arhexrey.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2qsltpbsu.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2fiabrghr.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2sxjfsijl.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2xqbvwvay.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2prvpvrmt.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2rpfygoql.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2scfkemat.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2sqwylnel.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2gmlmgjzn.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2mivumrmq.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2lxcrykkv.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2tajnpmei.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2vdszmnht.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2plnvygab.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2bxkscexu.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2tqqiwypv.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2wjgrtbso.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2maolefmw.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2qurjbfak.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2wppuxase.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2fgfcxkml.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2saxxtkem.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2szadtypv.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2cospillm.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2mafusbzn.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2yqzxabvk.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2lbpsbixj.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2mzvfpulp.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2xhommlcu.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2dncjuhfx.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2jemizfff.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2opwrscee.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2tolxsain.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2zkvykqsi.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2pgpnbnyt.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2cfzuuvvm.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2qnxvmazg.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2bqmfglst.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2hzvcpije.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2pgjjktjz.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2sdvwrmrk.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2zukmiary.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2qxaycfpe.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2nsucactk.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2ydbokieg.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2wkzyyjbz.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2cbiwdibo.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2okdnzvpm.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2tfxzjbyy.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2wosgaius.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2gjqyoivd.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2bbuptkwe.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2tzctasct.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2kejahjpe.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2onmgygsu.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2qxqilvom.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2cmovnzkt.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2ujyusuhk.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2kgzrghom.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2dqjhgjnw.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2mitrjxnl.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2jkkcbxue.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2bjmdfwny.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2lpfhbehy.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2rpcjcoda.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2abhfgqky.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2qqnospji.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2drouusmu.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2tnzvvqxp.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2fjofokmi.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2kookilam.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2cpyhutor.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2ecrfamok.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2gpwlbpjn.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2ukaufswl.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2fnefjrgb.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2kycnlpis.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2irjuazgq.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2pdvetnjn.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2mnkgspdt.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2thwevcze.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2juycpwvb.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2mskkbmll.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2hyasleay.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2pweykapu.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2pybqudea.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2uytlejqd.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mnvxgscl.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2nvhuoohx.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2xrnvmhij.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2yxbibpvb.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zavuejly.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2hooaegfp.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2qpcvwuki.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2uortbesj.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2jkzzxxeq.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2ankeqnyk.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2qqttngfu.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2pcowgsod.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2ocijqyfc.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2awjqjtkg.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2lkjnenhs.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2vucwampc.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2meqxsnor.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2qzfkajvq.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2nehbkkrs.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2wzxcoafr.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2agyhwjty.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2vbbacgmz.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2equiwsab.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2nodsejiq.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2tsyvscbx.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2ybomghly.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2zcbfwgtx.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2bqyctify.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2fovhjako.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2cphesfrd.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2tnghvzlm.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2olsetzbx.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2tfmuelje.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2twjqinqd.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2wbmknoun.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2dvxcbobz.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2gudpkrxc.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2odgexkfr.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2mkmvsxpx.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2pemhgjjx.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2udbkqles.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2ssicuoyf.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2gkhwokai.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2mzpilzlr.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2dlfhkris.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2vseuwcsk.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2gittapge.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2zotzqlsi.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2elhxjhlt.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2bbcyyeiu.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2mqvlvuwh.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2ksrbuquj.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2arlftyzn.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2pqllkjkk.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2jegwabel.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2eoxkqevk.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2ppugvydp.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2jjecguth.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2rnpjlxrs.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2jvgwqrid.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2vanhzmng.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2tsgmhktf.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2snyxkhll.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2rfdkcivw.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2rwfngvsf.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2ejstoznh.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2hrqjceic.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2vveonxjj.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2slacvaae.html


<!-- 参考信息 -->