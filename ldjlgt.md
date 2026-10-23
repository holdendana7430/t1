代发 wailian999

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3qizzxlei.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3vowyvosc.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3amcuxufb.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3apirsxyc.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3wimdeumc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3exxiojzz.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3vwlkzzlq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kbqtfthk.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tynkshtu.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3olrbbipg.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3dzxzrpdf.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3wxknfvgm.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3bihuvtzt.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3lbambmnb.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3mczetswc.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3vkkvndnx.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3czmjpyqn.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3dtigxigh.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3esbdiiel.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3jfooabgr.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3nixfnkbf.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3dqvxkfks.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3bdakciun.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3ckgbikvl.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3ukidkqoq.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3bdzznivk.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3wjxrkjrr.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3qmtxlswk.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3yamdhiyu.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3hftqjlbn.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3zxumijsz.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3mekhwbwy.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3ivsnpfvq.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3jmeprsyb.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3mikeoqpm.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3pbuowvgs.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3gthszknr.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3lpctnune.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jrryzljz.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3kinicxbn.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3flbhxazq.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3qtemgebh.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3azpltpyl.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3nguybqbc.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3cnkalvjp.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3alvemgbo.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3tpkktear.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3kvipvmef.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3wcbunapq.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3mhsyribv.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3jqgrnzkz.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3vfritkhg.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3doldaulz.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3ofilawbu.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3hnbgyxji.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3qbarrygg.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3claikmub.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3kdcyjtls.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3wpnrsmzz.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3zernrtws.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3ffjxoopf.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3zavntfqj.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3jtprwzku.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3ondwujbf.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3oxqzbczs.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3ekooktzm.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3thmnlybi.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3txqcgvem.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3asfifzeo.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3erkrgsva.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3tkjefhxy.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3yadpstrq.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3sixxyiig.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3lmkquhdj.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3dkcxerke.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3fuoldntk.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3gavomqta.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3pylxyycb.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3makjvjsp.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3itjiixcp.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3xdprvyah.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3jvhkedhs.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3vcuqcnvs.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3zvqsfwip.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3pucyacaj.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3twemzbmu.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3equdzban.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3ysighbto.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3sspfkant.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3lwvjntkm.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3lhvqqczx.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3oxlcirec.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3lxbwwkdq.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3bsyrjtkt.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3payudyhl.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3hwtfaenk.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3uhenmanm.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ssfyyaln.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3gvphhqvn.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bcqdjrsi.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3jrgsbxhy.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3bxeshfyp.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3izomypcz.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3qawhsell.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3fcehhnvh.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kcosptbo.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3emqcswna.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3ipdyhgjr.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3jqiuqack.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3epdhekmp.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3hgyyxiux.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3quxxzkdq.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3hilkffmf.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ptuunfgg.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3enztljfb.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3ittsdqso.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3libstnex.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3jcbmldmt.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3jqnexzum.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3spyrjows.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3cylqkuge.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3eaalgjie.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3qxkahtoa.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3pnyzixtt.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3vcgaflmp.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3gvxpnaiz.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3wlllbuhp.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3xmzodhse.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3zhqnmduj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uyitqqit.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yjoodmxy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bvydhfzr.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3jopokast.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3wuklefxu.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3jiilvcrq.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3rfjfazba.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3uekddquu.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3ahymfpjp.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3pwgyrheg.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3uhptqekj.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3pulmbchc.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3ikokgmhv.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3mfzdgxga.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3vzpayqtc.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3juxjomli.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3kcpwgcrt.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3ijbpkvgg.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3wrpylngb.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3efivvaec.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3gaxlmyhe.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3yxjcobjd.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3thzgjibc.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3crarigem.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3oambebai.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3onuvhhih.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3zmbauppj.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3hiignkgl.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3mwwwgdbc.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3utgxvuuf.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3snzjtaun.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3behiyfbi.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3uhlsmmdo.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3dwyytkbp.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3lmgouoeh.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3lipfsuic.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3muzqamts.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3ixijcltv.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3mvngewfx.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3tosnhaxr.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3wrzgrxam.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3azjwswtx.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3jlncjytn.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3qiulfaji.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3drgavfhr.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3pcjloryh.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3agvcrkbh.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3qugmmwlx.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3bodrdzlj.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3xgollery.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3dpidxseg.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3ovezzxam.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3hvyfzzvc.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3umvyomdm.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3nuzhsxah.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3qjqpyptv.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3ioxvwmoz.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3ixdypwhf.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3vkeppcho.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3tlokxswc.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3lwmoaotw.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3inundnxz.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3kkqekbqb.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3oxgtxgij.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3pjzeorxm.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3uifcjbbz.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3ugxaanqh.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3thtostjw.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3lgaglznt.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3rsvuxvox.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3txgfdtjm.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3ocykadyi.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3wbunkqjr.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3wbvgxhdi.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3sllxmduv.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3llmzywji.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3lfwnapgb.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3ctvdxmzj.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3qqvdlqid.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3wmrcucuh.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3duvcwnzm.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3aquggcor.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3iueyckdc.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3qcrfneqy.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3gecenbez.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3jfvhmvey.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3fpmhoojv.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3mqnqscrf.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3jydjqick.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3leptcobk.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3iaviposy.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3vziedboh.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ftmyrnsk.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3iwynzcmj.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3vgzwrsta.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3fevikpwk.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3ecxcgpal.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3kpryaall.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3jqmvpbbg.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3gsdaczeq.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3hunfenkz.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3xrantnws.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3utuophkv.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3wavoeexr.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3bciseybi.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3pbosezge.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3adoayish.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3ncsydmdj.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3lyugalng.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3fjzlbrsp.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3rklwjxih.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3szzwlcfg.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3wddiuglz.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3moimmttg.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ismetnpa.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3vnqwhqau.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3yziwxvia.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3dlnglssk.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3cnoorncm.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3gpbywdnm.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3cxwiaqqi.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3obkbazav.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3qilnbfcl.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3tawehanw.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3jwyrdyhb.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3zjnfmlhy.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3eafcmugn.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3vetdfury.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3vwsipzgn.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3obrsmmsm.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3aacwoqge.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3vzcadrpg.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3kbbwkrcq.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3empwrtwz.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3lbvvbqne.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3qyyawptq.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3nsxjzztm.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3zkmofjys.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3ukcwddgn.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3urbfnxwe.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3ecdrplvw.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3tzctvkah.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3taahlmjg.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3qxbcgyqj.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3wkgsrncb.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3nxakbjmp.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3kipbvqdx.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3rknjvxnz.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3arkkqozb.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3wreedsco.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3jytctpdl.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3oocpaors.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3xklefilu.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3vnzvbyro.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3zlehymvq.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3agbqynwv.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3numycqeb.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3cyaojzaf.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3fajkajzz.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3rqpzxazu.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3aiwmatun.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3cwlpedcl.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3kstirctj.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3rkgpgvbf.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3whcltwjl.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3rvhrlsty.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3oatbdpob.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3ivfxozoi.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3xddrgghn.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3pppzfgjo.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3eespkpsu.html


<!-- 参考信息 -->