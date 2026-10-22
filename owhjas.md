代发 wailian999

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2kukdysek.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2oczdfxul.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2uycvqtqn.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2ynreobbg.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2gdlhblge.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2aeualgpm.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2pyhgqxzj.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2ammyaahj.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2qirmlxwi.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2symwdkgq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2zuptdowt.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2vupbndqm.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2wilfskku.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2alzhocsj.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2bajmcnds.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fqctbwwe.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2gfhntfrh.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2jyfckzxp.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2demevsbm.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2kogftxww.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2nkklnykw.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2ajexnchc.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2dmdzzqbo.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2xckocufh.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2duebytfw.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2louyzfle.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2jppycosp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2alzeqaew.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2lzfjyhcy.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2ppcaswka.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2sygjtqel.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2qlasltiu.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2hsqhqzjl.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2cpqjgwfb.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2yohhomqd.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2rjsvxgsy.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2qnpqfjae.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2lyquxruv.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2wuacxpfw.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ktafeaux.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2otoiycml.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2dyyqrcxi.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2maqsuaiv.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2bmvezxyi.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2hqzkyjlv.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2bvgboumd.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2tsvxndts.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2dkcvyads.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2cvzeiucz.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2rjaxsmuh.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2vkijvtqy.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2irkuutqa.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2bkzgjdyq.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2ynpltden.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2vegwagaa.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2gnjrneon.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2frpoqeos.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2fiiznuwt.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2jspiytav.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2cexystkk.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2hozeonoj.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2vfczirib.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2dmsrvfsb.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2azptgszz.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2hinhdzeb.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2adkaojpz.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2rcgnaohq.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2pweqdocs.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2waybjrmd.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2qdbvocas.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2tbogqqkt.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2dbfdddlo.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2kuhfcypu.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2tqgeckbo.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2qtzzkgzm.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2gvozbbyv.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2smkmgaps.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2nzlldayv.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2wopcmmcn.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2aavyfumb.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2flzeblpk.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2dliqoikn.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2ztxobwie.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2kfjmsjla.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2uxstpehr.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2mmjgspme.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2kggxrmud.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2xnrsntts.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2ewjaaxnq.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2zmvcqtyn.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2pziaqgjy.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2qlvrrhej.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2lkhaciup.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2hsgakyqa.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2hvvxnqlk.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2plhpablo.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2zwwgiztw.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2gzbjijxs.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2pcahkhpk.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2feaquidp.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2npaqblod.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2stilnuru.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2mstjlobg.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rrlnuuac.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vfpphdcd.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2mywbqrun.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2duojhzjj.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2wkrwheui.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2fafnzovf.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2akzovsqd.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2kxbyzgrm.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2xkmdnrtk.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2mmegqrko.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2cbophsdd.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2rpkwxqjq.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2fvtvnrus.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2jpmwmxgj.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vfsqpijb.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2bscdcwgf.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2mnfvgpft.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2cpggcezp.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2isgtsqpz.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2xjaqqarm.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2tmiprief.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2uojgpkab.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2iasglfpv.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2xkueoxdw.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2anxzufrg.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2jokggygv.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2nesfvcmp.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2hnncgivg.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2wwkyixyy.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2gfkbrxul.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2ndtflady.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2odyxehsk.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2kdelpifl.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2msukkfgg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kvwgupvh.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2eolfjaka.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nwkobnmw.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2lmackycs.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2rhcavnxj.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2svnzqfyu.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fjpgtqzt.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2hethuwne.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2hdsiudmp.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2mitidxhe.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2ucpppfft.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2majzfuhr.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2uregpeyu.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2mylefjyw.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2xebxypfv.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2siznirlf.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2fzyvuchj.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2pgqfmzyr.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2mnhpgkln.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2mclrjyuv.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2ynhmbrbp.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2xzfrivdr.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2yonputde.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2bjnbfxzo.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ziiuexpb.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2nkwbthjv.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2qjhzlmxw.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2cpxcjvhc.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2svfdiyzg.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2krghhnlh.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2fppxmhic.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2afrfykun.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2zltormrv.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2cwukbjvm.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2ysplgcbf.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2azycbaqe.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2dlkulpdn.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2yxnevpsf.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2eygmnlmt.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2ixoluagt.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2ccuykofm.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2clzukywa.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2tfbprakk.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2hxraxnay.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2pakbepdg.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2tudtakei.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2sialttre.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2cqidjwhe.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2cqnurenv.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2wfnspcvg.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2kyoprbrr.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2ewsepzel.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2hwogsexl.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2mgxuscjt.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2zkyfxktk.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2jcisuoxk.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2vldtzfxv.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2skalfziu.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2husmvoeg.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2vkpdmtrr.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2usosyoxa.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2voerpgtx.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2zafvaewj.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2bndsmwbg.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2lyjprloo.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2gznliahf.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2tjjubymy.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2mbzpcajs.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2argoywuh.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2szjiqoek.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2xuowohkc.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2eoznazps.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2ltnpcmiy.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2gsahvptc.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2sgisvtpc.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2rgemxzkp.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2zxcdyuwh.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2amuawfaf.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2ksdgqukf.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2vddmkkvx.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2bxxxtuuq.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2zcqgsqmg.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2lzmqbdqn.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2sbggaoai.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2obyklkul.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2mymthtji.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2yyjnqvfn.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2uhcowpao.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2mlpyziea.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2fgruoalm.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2julvudtn.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2eebthfar.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ehjsuffx.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2jvaaacim.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2olfcbjyb.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2uugmzpqb.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2nrlsvxec.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2eihvztha.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lzkrngya.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2lxpyodvt.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2volqiyon.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2ekhhzsqn.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oqyqvkiv.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2xjsafgab.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2iqlyivss.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2sjfiqjyq.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2rwqukjto.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2qzmrduve.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2cbsvwalc.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2yxrulkwi.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2flybrlnp.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2elngidvj.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2monasplr.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2lwpxgkpm.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gayeioqn.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2gfcpvcmr.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2ijytdwgs.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2doyxzlys.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2tncysjly.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2blitlynt.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2nxravwfw.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2jyagstlg.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2mnytmyas.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2ziwlmydj.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2xoyyvxru.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2qvuwfcmv.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2xpsqlvgz.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2fnkqcyjz.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2ydnnesbl.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2mqrmbpkj.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2lthlzrgo.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2ewtbpltf.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ggnxjnda.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2ontgocjc.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2albtxuiz.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2jcwqsorf.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2cinbyhnl.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2unbjznyv.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2qaawhnyt.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2ccprskxw.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2gtzbvdle.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2vqyyyevt.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2eeqjwqmg.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2jzzerovg.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2vulpapvq.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2mskcwbrr.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2itvivntb.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2mmjkqtbt.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2sshjsvwb.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2xfobmylc.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2nhqzvrfj.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2kklkfopo.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2nnpcxsfo.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2tkxrcneg.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2uuuuwxfc.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2txqgtcsg.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2xksvjprw.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2atlmqcyu.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2tzvjixtm.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2jniskfar.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2fdewafbx.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2uwhbbyhg.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2cljaqewm.html


<!-- 参考信息 -->