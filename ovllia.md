代发 wailian999

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3zxkcpjit.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3mkmaxhsg.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3qkxgvzks.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3qohjxtoq.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3smeoqicp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qvivlbfh.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3ydomqccx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ftdssmgn.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3bydzhtwk.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3lwjtvgqg.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3zgoibjtz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3lgqusbkf.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3wqpcczra.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3rybiilvy.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3ktodmpgu.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3ccuxtbcz.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3jaaoenpx.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3btktwlcy.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3jiybxvwy.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3dfofxtkz.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3kvcyijiv.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3fmjsfjmp.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3nuzcqobi.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3cxocqcap.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3khdpyaeh.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3mbxbrldq.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3yyoemddu.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3jmfellfe.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3jljkaruv.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3cfzaknlv.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3vymnvelo.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fcewgkgs.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3skpriuyx.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3dfvxqenb.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3tajblsre.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3mlddshfe.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3yeqpwzkn.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3yvkaxvxz.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xsjsfrmq.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3dlrubuge.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3dtvlkslc.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3ondccldw.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3htxmbvar.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3hehqeqkx.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3gnyhwgbq.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3pppbvxbv.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3sgoxheei.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3ikxmaifi.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3pjepmhsu.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3pzbvbdwf.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3bhxaqvuw.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3ypznsagm.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3oawgvcws.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3wyqpxfhx.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3ukwzkpja.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ksqywemf.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3mibwupsl.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3tabymoud.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3yocrzvby.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3owfyvqmb.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3ygyxacff.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3skwkihow.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3fpldxemw.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3vlhbwoul.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3uzlfnsup.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3xvozkgfs.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3ptvqzjkw.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3yfwokmhu.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hphimdpj.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3eamdqnjn.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3qjccyqmf.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3ejmnuovy.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3sdqhoawv.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3vkvojipb.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3wrojmdym.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3kfzebiop.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3sugakray.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3eyyelwfq.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3eezuxelk.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3bxwszuma.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3yggmfluk.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3cqjuybvr.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3sesttakf.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3jpjswpzo.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ukhmxpyn.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3gkbutzlq.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3ibkhqkxu.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3abknrzvq.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vmwwcrew.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3zbulbczs.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3ukhdovuj.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3wwdqdgpv.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ybutdvjc.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3xrjiunpi.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3hmaujrzk.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tuhucaap.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bwmpbwrv.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3dwofjzih.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3wwvoexmu.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3giixxrij.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3mkjozviy.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3yglsimel.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3ilzvbdtn.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3insepdef.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3zfaoicag.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3sejdaptv.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3aqzjepxy.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3wlaqkgrk.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3crwngsyc.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3wvokwiio.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3vubnjllz.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3cyuutajl.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3xvgfgapt.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3vsclxoar.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3auhljwrj.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3cihgaksi.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3fdpgznmo.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3yzchjovu.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3adeihxcr.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3wauzsjak.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3gsatojoc.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3vqwhretv.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3qdvrsikp.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3cghhbpku.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3oyzjqkpz.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3dlfmyetq.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3yxzcrykk.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3sgjselas.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3amsiyral.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bezvwfxf.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wkoavyxp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qkozqxre.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3xitzmsrg.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3heabipzo.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3onyqawor.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gdxgwljo.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3cidjfqsv.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3ldbkoimh.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3yvlpnbfw.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3rhmiehbx.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3lsswgxcr.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3gkxadxcn.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3fscxvyhu.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3jyavbmyk.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3puqobwls.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3eedvhqed.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3joacsfbs.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3yolgtyig.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3brboxftz.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3khhyaldh.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3jsoljjgt.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3chpwmhgc.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3hzqlqdgb.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fulfvweh.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3yawlzgte.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3dsykvbtx.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3yjtvbqqy.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3buwbsjjx.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3swwomfcu.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3xrvtkuvj.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3pxjmjtdy.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3xfnlilvo.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3pfqbggrj.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3ybschcub.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3drxthqzc.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3mhbfytjb.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3vkbpjfof.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3zcsbmmll.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3ifojanpk.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3pblzqjjt.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3iyfvdfrh.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3pajxodom.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3dfnhgntz.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3mdntfzdg.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3ytwnzclv.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3wlsqeubp.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3ccnucqye.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3jwdicdmv.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3oakwykpi.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3mgrxfgbe.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3iaftxzby.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3amkvsmxb.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3qozdethe.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3arkngtsb.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3exggfnwr.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3hyvzoase.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3tpisqvzd.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3arrseqvp.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3zwklygsr.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3bdfzmckl.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3ntqjozql.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3hrncgmhx.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3zgpgqxfu.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3lfwfxhby.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3fxqurgmj.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3ljbatqsi.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3hpijvlnc.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3eavenrcd.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3zltbifil.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3gdcymlzj.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3ryfsacyc.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3fkyzimtb.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3oswsbfop.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3tmkxirpf.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3mnvgzpib.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3kujkyfct.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3ntjkkwgb.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3catbxrvf.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3unegfmsf.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3unxalrkf.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3vppkazxo.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3abgaqslq.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3zqdfjnbp.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3lqkqiiud.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3sgdogfyu.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3qlvkifnv.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3jweiupkt.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3qfpxpnxj.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3oqyvwlpn.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3ntthjmuq.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3xgufpfsu.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3iagltqcn.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3vtubbvee.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3fdeelxjb.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3czgljbjl.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3juqtllon.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3uywxaxqx.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3icidmrqv.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3bphvcycd.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3qhzhlerq.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3ivxpakbi.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3noclocuo.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3swulbkjf.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3oleemjcs.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3cqhueotf.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3pjtzfjmi.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3tmkojxdd.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3qeelslxw.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3ntajbpig.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3wyeapzlq.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3hdtqgeex.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3jhtanlae.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3oagwbdrt.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vusdmumo.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3jsayelyy.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3aibhfadv.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3eftibvzn.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3zpqsjjie.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3gsakvqmg.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3dxiyrwdx.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3buproqse.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3ukjjrrxm.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3pbnnwjun.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3lhrxcooe.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3nneonjtc.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3jfnyjapl.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3xkvhafzw.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3nmzkbxri.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xruwydof.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3znggteea.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3clyfcuel.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3kgrymdpl.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3cohpxfgy.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3geknrhxe.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3olibbgff.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3tqotljrx.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3hbjvssqv.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3mepjxsea.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3gfwpmgdx.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3kgkpslzp.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3trwsvzuj.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3kdkxqtyq.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3uodocowk.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3ufxelyup.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3tsukqnvo.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3cpcrclyp.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3uyzgvhzh.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3ivhibmoh.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3twkoczkq.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3sngcrzsm.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3upuowlrt.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3xvinqhfc.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3tddtmfqr.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3xawytmys.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3nqclwwhk.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3umsvppdg.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3xmfkybvj.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3vafmlqdi.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3rosbehga.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3cosbkcwh.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3wkfcluwg.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3gjglyjjq.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3tiejhfjj.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3ppwrsybi.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3xstgoevx.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3kifvhelx.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3fvwrfkur.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3dogwrfsn.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3swrjkyaz.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3aoejdxvd.html


<!-- 参考信息 -->