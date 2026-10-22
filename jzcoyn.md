代发 wailian999

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2qamucphw.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2arvqyjsw.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2qkamserw.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2awncpdcw.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2pgviygqo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mydkhkim.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2lildzuup.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pdwtmexb.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vrivrucs.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ulxxldpf.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2aanypbyq.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2trcuvwky.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2hdkyisgk.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2sfptzerm.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2torarqnw.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2fvwslpjp.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2ekctufhn.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2ftfsahsp.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2hsdddayz.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2buhcxvyg.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2fgdisibn.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2erswacpy.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2maxtmqrg.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2xplhpwko.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2mosuohwt.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2elzfswdl.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2ehcjsgiy.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2hwqjdrgm.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2efwuqyje.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2ciwkgzlk.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2yzubzlnv.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2pznzydwr.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2zsvkvpgd.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2paqfqlnx.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2wectxlzt.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2elgpcwgj.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2bowyuvya.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2swbmqckg.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vpfoinht.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2cdtfrefq.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2haypdjxa.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2xylhcyvy.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2vxihqxqd.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2lmplzzjt.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2yosbrybj.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2pdyskxub.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2zzohahhm.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2eeeeolne.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2pxsaxyyb.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2lasnhzxq.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2akeqlgxi.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2vqbaxhvb.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2gpnkayxb.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2cflrafeh.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2ssbubtco.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2bshwwjsu.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2xxefmrnu.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2zwrfvwor.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2amlysljd.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2smwmtuba.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2djmsfcyq.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2rekpjkib.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2moaczixh.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2ntjyhukj.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2suafmlvk.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2imdbggfb.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2kefrkxhp.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2qbyanvio.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2fgoqwpnr.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2xxrmwnhv.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2sipicwys.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2uawgwfnh.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2eigmkghp.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2faypnbtr.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2qmwljose.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2gyqftadd.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2qrutmiaj.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2fcfmriva.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2qrafwsgm.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2kkbtbdhb.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2qwomjbca.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2acbwhrck.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2dscxbxle.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2chykkjet.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2laevxqhi.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2iwtqnhpm.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2lohtpvqn.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2hmnwvygq.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2iuwctphn.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2lyyztppq.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2vplserrs.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2dyemhkdq.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2vdvflajr.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2yjoamjsv.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2shxcoglf.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2pzaoxyqz.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2nbmarweb.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2pxqjgnxq.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2yliwippx.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2zkpfcljn.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2ibhzwhob.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2qmrberee.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2nibyhwje.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2lslcyurz.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2amppxhxl.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2psdtyeei.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2lqrbsqzp.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2rkjvicqz.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2cgpajpiu.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2khcinizg.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2dfsnexmc.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2kztbmbyg.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2umanqjol.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2knvjilkm.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2tspecemz.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2aaccemfk.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ejvvtovz.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2onsslbka.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2whacabjd.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2avfyxxht.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2uekfagrd.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2nkhfbxmd.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2qnpbszjl.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2szdtwnyv.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2yvofheak.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2ywscgtnf.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2uztqtyvk.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2yngyhfbx.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2qapadqdh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zbscgdlq.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pfjolgty.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zhhdegid.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2lscrxfcr.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2fwdsrtnn.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2dywrhnvo.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2mdykxntc.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2rbteyqyz.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2czzssjsy.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2ebkjmtlz.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2yariqdbf.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2bazlklsn.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2cofdhhpd.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2qntmubpl.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2nzzmsjbz.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2oxjvtatc.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2hyvkydou.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2dlhbcvxo.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2ceeadspx.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2utiuoitr.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2qoztpcus.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2tkmsfltk.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2udkgkewa.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2dkkrzrez.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bbvmfjha.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2usehosyc.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2assbkjky.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2yrmzgnvc.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2pxiuwwrz.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2lwagbfcl.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2ktdbthtn.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2xhhvcuio.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2bumpeoro.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2dasvedxe.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2cqjexgbs.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2kbscyrkw.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2ztryelzy.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2iczwoxrn.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2nffcuikk.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2gzabxltp.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2zpfurkhi.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2cnahrtgr.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2spxgprrj.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2ghmdyiwt.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2mfalswgw.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2rlunktil.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2qqsawsez.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2gvhizykf.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2nmrlfprc.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2vvtfifyn.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2eqvdhvwa.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2fsfydtkz.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2kjveyivn.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2pxmrngsb.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2lplunppq.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2rbdncqyz.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2rnkioiep.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2qfkfdqxe.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2rowbbbrv.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2hihgfohg.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2gubomqdd.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2xdunmeqe.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2llvhffwx.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2ovvijeee.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2fuvhrwuc.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2oraapcoa.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2wpqgrdxt.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2ynkjsueh.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2rnfgqknm.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2zqvchanj.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2ggiwqaso.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2bhoayein.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2xhhmwliy.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2ehhyrsjr.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2omwkfzom.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2yrcrtvxg.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2ocniycjh.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2xcgslmjg.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2gujqtsto.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2mriupdfs.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2qcbtdbti.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2cwfgbpvn.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2buaqjpbe.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2fktklysp.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2byhyyxkv.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2draulvnz.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2lokcouna.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2wfcehaiu.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2dnwgxwdv.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2foaejofd.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2krsvnrdw.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2fifitxqj.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2yqzxlyar.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2vdewluar.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2rghhhymt.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2jrznqxyg.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2iysyobql.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2tkkhnsbx.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vytlsktg.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2tdltryee.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2eczjxchw.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2vyjnfmsk.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tclphsdj.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2zmjfuwlz.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2gioriadw.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2dfnyxixc.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2lroanscy.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2qcqaokgq.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2xliexiqg.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2rgzrolim.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2cpptzcaf.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2thopjtab.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2pgvbuonc.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2mglpijbq.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gkovmsxz.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2wnemcxce.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2icqiudin.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2cgnbasic.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2gqpkxzpq.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2yqrevyfk.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2ffkqoibf.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2honkrnnk.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2utoxyunr.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2noyspajn.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2bficzmdq.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2jnybbrbf.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2cqbkwhyv.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2yqavjbjx.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2rfeilyon.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2tklfdwqt.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2hvkrfszb.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2gulmtjjt.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2hothwkho.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2dzhawljc.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2jcrnroou.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2iwecxngf.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2kpfmgcdn.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2cpidlqzj.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2jageutnf.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2pufohivs.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2zlwospyv.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2jfpsdnxy.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2yekcksgh.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2pmwavykh.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2rhdmqghf.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2aunasrwb.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2jshaqncf.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2jhleqptd.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2yeynhkuy.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2yyyracns.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2qajpsdiv.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2bqgjmusq.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2mlpmmypo.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2wqrumrxe.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2dphvnqvy.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2pmvkunuc.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2moagfhal.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2dkfijcnk.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2pievhsul.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2aauvjhyd.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2bokelkux.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2luduetga.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2sehwfyuw.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2lrprimbb.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2njfgqcqm.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2rzdqvdnb.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2sejdwgjm.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2ttxxuske.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2vfxzzxrn.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2kqlyaeqr.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2tiykfhjz.html


<!-- 参考信息 -->