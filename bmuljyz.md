代发 wailian999

namespace ns { int f() { return 1; } }
来源：http://www.share.fehbvm.com/Article/details/gtddsdsup.sHtML

[S59] C++：静态断言
来源：http://baike.fehbvm.com/Article/details/gsdzktubi.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.zdbjq.cn/Article/details/gsbfqzscq.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fehbvm.com/Article/details/gtppqzzfk.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fehbvm.com/Article/details/gqpvcqvcz.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gqvvpdmti.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.hesvh.cn/Article/details/ghxgdsemh.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gnbrkwpbp.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fehbvm.com/Article/details/gjbbgbxhd.sHtML

println("Hello")
来源：http://blog.hesvh.cn/Article/details/gbbjhqkjf.sHtML

[T02] Kotlin：变量
来源：http://read.share.hesvh.cn/Article/details/gabnrbznx.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.hesvh.cn/Article/details/giprglpyc.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.hesvh.cn/Article/details/gdminmmra.sHtML

"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/gkscgglxg.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fehbvm.com/Article/details/gbvmdgawa.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fehbvm.com/Article/details/ghltuyupm.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fehbvm.com/Article/details/ggkzsyine.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.zdbjq.cn/Article/details/gbdtouznu.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.zdbjq.cn/Article/details/gfyjochqo.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gqaeztdsb.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.hesvh.cn/Article/details/gsgsrbmza.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.zdbjq.cn/Article/details/gqdrbfywd.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fehbvm.com/Article/details/gpfozecsk.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.zdbjq.cn/Article/details/gtjirmvjy.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fehbvm.com/Article/details/gdyhfxgey.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.hesvh.cn/Article/details/gmikedyhn.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fehbvm.com/Article/details/gbmbzlmqh.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fehbvm.com/Article/details/glnlrkdmg.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.zdbjq.cn/Article/details/gfyemkpcx.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.hesvh.cn/Article/details/gwrzvgbuh.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fehbvm.com/Article/details/gctnrbdek.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.hesvh.cn/Article/details/gculjztpj.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fehbvm.com/Article/details/gzkkadfez.sHtML

val m = mapOf("a" to 1)
来源：http://baike.hesvh.cn/Article/details/gyhduowyh.sHtML

[T14] Kotlin：循环
来源：http://baike.zdbjq.cn/Article/details/gmfirkwtk.sHtML

for (i in 1..10) println(i)
来源：http://3g.zdbjq.cn/Article/details/guhrchofx.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.zdbjq.cn/Article/details/gbqoeufks.sHtML

interface Shape { fun area(): Double }
来源：http://baike.hesvh.cn/Article/details/gvebglaqw.sHtML

[T16] Swift：Hello World
来源：http://baike.hesvh.cn/Article/details/gczobjhek.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/gsuhpyegc.sHtML

[T17] Swift：变量与常量
来源：http://wap.hesvh.cn/Article/details/gccsbpjpf.sHtML

var a = 1;  let b = 2
来源：http://mobile.hesvh.cn/Article/details/gjhvyxygt.sHtML

[T18] Swift：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gpecuxied.sHtML

"值: \(b)"
来源：http://wap.fehbvm.com/Article/details/gnvmzegem.sHtML

[T19] Swift：可选绑定
来源：http://www.share.zdbjq.cn/Article/details/gczwvomqn.sHtML

if let n = opt { print(n) }
来源：http://wap.fehbvm.com/Article/details/gzjstflje.sHtML

[T20] Swift：数组操作
来源：http://read.share.hesvh.cn/Article/details/goiluuvdi.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.zdbjq.cn/Article/details/gmryetwzc.sHtML

[T21] Swift：遍历
来源：http://wap.hesvh.cn/Article/details/gmjnzkbgi.sHtML

for x in a { print(x) }
来源：http://www.share.hesvh.cn/Article/details/glowenetj.sHtML

[T22] Swift：字典
来源：http://www.share.zdbjq.cn/Article/details/gdlxexhcd.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.zdbjq.cn/Article/details/gbstivjrf.sHtML

[T23] Swift：函数
来源：http://m.share.zdbjq.cn/Article/details/gwtqtylia.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fehbvm.com/Article/details/gkoyyffdl.sHtML

[T24] Swift：闭包
来源：http://read.share.zdbjq.cn/Article/details/gpnqywpfn.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gjaosaidz.sHtML

[T25] Swift：结构体
来源：http://blog.zdbjq.cn/Article/details/glfcoggae.sHtML

struct P { var x: Int }
来源：http://m.share.hesvh.cn/Article/details/ghvocttes.sHtML

[T26] Swift：类与重写
来源：http://m.share.zdbjq.cn/Article/details/gwyuoqssh.sHtML

class A: Base { override func f() {} }
来源：http://3g.zdbjq.cn/Article/details/gzqamfapo.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.hesvh.cn/Article/details/gnvvuwuzj.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.hesvh.cn/Article/details/gfnuuglxe.sHtML

[T28] Swift：枚举
来源：http://read.share.zdbjq.cn/Article/details/ghcrrthvq.sHtML

enum Color { case red, green }
来源：http://www.blog.fehbvm.com/Article/details/grkxpbnrl.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.zdbjq.cn/Article/details/gecjrjpip.sHtML

guard let x = opt else { return }
来源：http://baike.zdbjq.cn/Article/details/gykejkqmn.sHtML

[T30] Swift：协议
来源：http://www.m.share.fehbvm.com/Article/details/ganowmwyu.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.zdbjq.cn/Article/details/gmcbdiyrq.sHtML

[T31] Lua：Hello World
来源：http://baike.hesvh.cn/Article/details/gbkarvkyg.sHtML

print("Hello")
来源：http://m.share.fehbvm.com/Article/details/grtdogpog.sHtML

[T32] Lua：局部变量
来源：http://mobile.hesvh.cn/Article/details/gqubsyuns.sHtML

local a = 1
来源：http://baike.fehbvm.com/Article/details/gdgfjslsm.sHtML

[T33] Lua：表（数组）
来源：http://m.share.hesvh.cn/Article/details/ghafnfhxz.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.fehbvm.com/Article/details/ghesqnvsz.sHtML

[T34] Lua：遍历表
来源：http://m.share.zdbjq.cn/Article/details/gdviilzec.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.fehbvm.com/Article/details/guczczbhw.sHtML

[T35] Lua：字典表
来源：http://www.m.share.hesvh.cn/Article/details/gwjevbpep.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.zdbjq.cn/Article/details/gpsgqmjhs.sHtML

[T36] Lua：函数
来源：http://3g.hesvh.cn/Article/details/gwgvxpxxj.sHtML

function add(a, b) return a + b end
来源：http://www.share.hesvh.cn/Article/details/gjokknsjd.sHtML

[T37] Lua：字符串拼接
来源：http://wap.zdbjq.cn/Article/details/glosdocqq.sHtML

"a" .. "b"
来源：http://blog.hesvh.cn/Article/details/geurzcluo.sHtML

[T38] Lua：条件
来源：http://www.m.share.zdbjq.cn/Article/details/gynvsgsye.sHtML

if x > 0 then print("正") end
来源：http://www.blog.hesvh.cn/Article/details/geiizkyvk.sHtML

[T39] Lua：模式匹配
来源：http://read.share.fehbvm.com/Article/details/gjhvnsroi.sHtML

string.find(s, "%d+")
来源：http://www.blog.fehbvm.com/Article/details/ghjddmija.sHtML

[T40] Lua：元表
来源：http://3g.hesvh.cn/Article/details/ggoxlatzz.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.fehbvm.com/Article/details/gvmumovir.sHtML

[T41] Perl：Hello World
来源：http://m.share.hesvh.cn/Article/details/gpehccttg.sHtML

print "Hello\n";
来源：http://wap.zdbjq.cn/Article/details/gzbmuwdgq.sHtML

[T42] Perl：变量类型
来源：http://blog.zdbjq.cn/Article/details/gjzrdqcgr.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.hesvh.cn/Article/details/gilsyhmzq.sHtML

[T43] Perl：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gqosbmbgw.sHtML

"值: $a"
来源：http://www.m.share.fehbvm.com/Article/details/gdevpocis.sHtML

[T44] Perl：条件
来源：http://www.share.fehbvm.com/Article/details/gwrxsngjt.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.fehbvm.com/Article/details/golrgfayf.sHtML

[T45] Perl：数组遍历
来源：http://3g.hesvh.cn/Article/details/gpcwjoykw.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.hesvh.cn/Article/details/gklkywcch.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fehbvm.com/Article/details/gdniiakqp.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.zdbjq.cn/Article/details/ghepsmalf.sHtML

[T47] Perl：正则捕获
来源：http://wap.hesvh.cn/Article/details/gffdwhaee.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.fehbvm.com/Article/details/gjfjzkomy.sHtML

[T48] Perl：正则替换
来源：http://baike.fehbvm.com/Article/details/gnpexwghw.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.hesvh.cn/Article/details/guaueafiq.sHtML

[T49] Perl：函数
来源：http://wap.fehbvm.com/Article/details/gazkozdrh.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gduanzxdt.sHtML

[T50] Perl：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gaeymtpns.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.fehbvm.com/Article/details/gmobkyore.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.zdbjq.cn/Article/details/gbpgcrnuu.sHtML

[T51] Scala：Hello World
来源：http://mobile.hesvh.cn/Article/details/gfohvfylj.sHtML

println("Hello")
来源：http://baike.fehbvm.com/Article/details/gckxcsxxz.sHtML

[T52] Scala：变量
来源：http://wap.fehbvm.com/Article/details/gjbwtafcu.sHtML

val a = 1;  var b = 2
来源：http://m.share.zdbjq.cn/Article/details/gfkohucwo.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gnbfongfl.sHtML

s"值: $b"
来源：http://wap.hesvh.cn/Article/details/ghubsiywr.sHtML

[T54] Scala：集合映射
来源：http://wap.fehbvm.com/Article/details/guqdfnrps.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.hesvh.cn/Article/details/gsvndukwq.sHtML

[T55] Scala：集合过滤
来源：http://m.share.hesvh.cn/Article/details/gulhqtfdm.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.hesvh.cn/Article/details/gjzydysbl.sHtML

[T56] Scala：样例类
来源：http://www.share.hesvh.cn/Article/details/gaosmniih.sHtML

case class User(name: String, age: Int)
来源：http://mobile.zdbjq.cn/Article/details/gyckqgbez.sHtML

[T57] Scala：模式匹配
来源：http://wap.hesvh.cn/Article/details/gwgxenhio.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.fehbvm.com/Article/details/gudsojzyj.sHtML

[T58] Scala：函数定义
来源：http://www.blog.fehbvm.com/Article/details/ghgeyeiwq.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.zdbjq.cn/Article/details/gapockgah.sHtML

[T59] Scala：循环
来源：http://www.m.share.zdbjq.cn/Article/details/gsjzkwdwd.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.zdbjq.cn/Article/details/gpnoftbcc.sHtML

[T60] Scala：折叠
来源：http://blog.hesvh.cn/Article/details/gsltkaugk.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.hesvh.cn/Article/details/gnxlieshk.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/grfpungly.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.hesvh.cn/Article/details/gyggmkwgh.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/godqlwuxj.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.hesvh.cn/Article/details/gtteonsmd.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.hesvh.cn/Article/details/gxfrhseiv.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.zdbjq.cn/Article/details/ghsoizlxt.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.hesvh.cn/Article/details/glaeakccy.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.fehbvm.com/Article/details/gsbtnpgia.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.zdbjq.cn/Article/details/gkjartrrx.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.zdbjq.cn/Article/details/grodblijg.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.fehbvm.com/Article/details/gdketinrb.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.zdbjq.cn/Article/details/gzujknheo.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.fehbvm.com/Article/details/gsfyxtizh.sHtML

[U06] Py：合并两个字典
来源：http://read.share.zdbjq.cn/Article/details/gsqrcfsgq.sHtML

{**a, **b}
来源：http://www.blog.zdbjq.cn/Article/details/gjqfjvxdr.sHtML

[U07] Py：反转字典键值
来源：http://read.share.zdbjq.cn/Article/details/grotyjzhn.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.zdbjq.cn/Article/details/gecdxfbzd.sHtML

[U08] Py：展平二维列表
来源：http://3g.hesvh.cn/Article/details/guvnlinfk.sHtML

[y for x in nested for y in x]
来源：http://read.share.fehbvm.com/Article/details/gpzzrkuio.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.zdbjq.cn/Article/details/gefiekxkm.sHtML

max(d, key=d.get)
来源：http://www.m.share.fehbvm.com/Article/details/gwenqxpum.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.zdbjq.cn/Article/details/gogsknzes.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.zdbjq.cn/Article/details/gdeqchcoh.sHtML

[U11] Py：生成器表达式
来源：http://wap.zdbjq.cn/Article/details/gilqgfdru.sHtML

(x * 2 for x in arr)
来源：http://m.share.hesvh.cn/Article/details/gpmqnzgjk.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.zdbjq.cn/Article/details/gkrlcxbse.sHtML

Counter(arr).most_common(3)
来源：http://blog.hesvh.cn/Article/details/ghmvvbdpx.sHtML

[U13] Py：固定长度队列
来源：http://blog.fehbvm.com/Article/details/gqnkiqner.sHtML

deque(maxlen=10)
来源：http://wap.zdbjq.cn/Article/details/gwrsogscd.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.hesvh.cn/Article/details/grqpplttr.sHtML

defaultdict(list)
来源：http://baike.zdbjq.cn/Article/details/ghymfxgao.sHtML

[U15] Py：高精度计时
来源：http://wap.hesvh.cn/Article/details/gzrpndrld.sHtML

t = time.perf_counter()
来源：http://wap.zdbjq.cn/Article/details/gftoinvle.sHtML

[U16] Py：命令行参数解析
来源：http://blog.hesvh.cn/Article/details/gdgimbabi.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.hesvh.cn/Article/details/gdhixkwiq.sHtML

[U17] Py：初始化日志
来源：http://3g.zdbjq.cn/Article/details/gleewwjxz.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.zdbjq.cn/Article/details/ggdbvuwje.sHtML

[U18] Py：预编译正则
来源：http://read.share.zdbjq.cn/Article/details/geplubfcq.sHtML

pat = re.compile(r"\d+")
来源：http://baike.fehbvm.com/Article/details/gjedujpng.sHtML

[U19] Py：正则替换带回调
来源：http://blog.hesvh.cn/Article/details/gqspiwcug.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fehbvm.com/Article/details/ganehpunr.sHtML

[U20] Py：缓存函数结果
来源：http://3g.fehbvm.com/Article/details/gvarefpym.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.hesvh.cn/Article/details/gkafhzkfx.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.hesvh.cn/Article/details/ghfbrqsgv.sHtML

@contextlib.contextmanager
来源：http://www.blog.zdbjq.cn/Article/details/ghvcxcbny.sHtML

[U22] Py：矩阵转置
来源：http://www.share.hesvh.cn/Article/details/gjpgcmhak.sHtML

list(zip(*m))
来源：http://baike.zdbjq.cn/Article/details/gsuqilmxc.sHtML

[U23] Py：分块读取大文件
来源：http://baike.zdbjq.cn/Article/details/gqqhsbqrx.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.hesvh.cn/Article/details/gsskzzpzw.sHtML

[U24] Py：路径操作
来源：http://blog.fehbvm.com/Article/details/gkxnxzyen.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gfjmdmazq.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.fehbvm.com/Article/details/glqxxscbh.sHtML

csv.DictReader(f)
来源：http://baike.hesvh.cn/Article/details/gmfpddntm.sHtML

[U26] Py：并发下载
来源：http://wap.zdbjq.cn/Article/details/gcvgkafme.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.fehbvm.com/Article/details/gfjisnvlj.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.fehbvm.com/Article/details/gjhxepcei.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.hesvh.cn/Article/details/gbiycxekp.sHtML

[U28] Py：类型别名
来源：http://www.m.share.hesvh.cn/Article/details/glbglztdb.sHtML

UserId = int
来源：http://read.share.fehbvm.com/Article/details/gjjqtiazv.sHtML

[U29] Py：属性校验
来源：http://mobile.hesvh.cn/Article/details/gbhjsbzeg.sHtML

@property 与 @x.setter 配合
来源：http://wap.hesvh.cn/Article/details/ghklpycxl.sHtML

[U30] Py：数据类
来源：http://wap.fehbvm.com/Article/details/gxlqhinjg.sHtML

@dataclass(slots=True)
来源：http://wap.zdbjq.cn/Article/details/ghbxzxzko.sHtML

[U31] Py：单测
来源：http://3g.fehbvm.com/Article/details/gudgampbc.sHtML

python -m pytest -q
来源：http://read.share.hesvh.cn/Article/details/gdxuapmrx.sHtML

[U32] Py：代码格式化
来源：http://blog.hesvh.cn/Article/details/gmndddtie.sHtML

ruff format . && ruff check --fix .
来源：http://baike.fehbvm.com/Article/details/gpqqfaipb.sHtML

[U33] Py：打包发布
来源：http://www.share.hesvh.cn/Article/details/gwlzltluk.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.zdbjq.cn/Article/details/ghumomdew.sHtML

[U34] Py：判断编码
来源：http://blog.zdbjq.cn/Article/details/glqwhjqsu.sHtML

chardet.detect(raw)
来源：http://www.blog.hesvh.cn/Article/details/ghrykstyy.sHtML

[U35] Py：发送邮件
来源：http://mobile.zdbjq.cn/Article/details/gmwyxiilt.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.fehbvm.com/Article/details/gcdoyowgm.sHtML

[U36] Py：定时任务
来源：http://read.share.hesvh.cn/Article/details/grdzpwvlr.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.zdbjq.cn/Article/details/gutfrryoc.sHtML

[U37] Py：读写 Excel
来源：http://www.share.fehbvm.com/Article/details/ggccdrhuv.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.hesvh.cn/Article/details/ghcveztzt.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.fehbvm.com/Article/details/gozklalgu.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.hesvh.cn/Article/details/gzhgkzmmp.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.fehbvm.com/Article/details/ghduameha.sHtML

sys.stdout.isatty()
来源：http://www.blog.hesvh.cn/Article/details/gyirnnbts.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.hesvh.cn/Article/details/gnecbqeah.sHtML

print("err", file=sys.stderr)
来源：http://mobile.hesvh.cn/Article/details/gyzzxatcc.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.fehbvm.com/Article/details/gjfspbzfn.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.hesvh.cn/Article/details/gazbqlvbh.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.fehbvm.com/Article/details/gqxznylye.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.hesvh.cn/Article/details/gmgxisfsl.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.hesvh.cn/Article/details/gwzqcaake.sHtML

namespace App\Http;
来源：http://m.share.hesvh.cn/Article/details/glhynhkxp.sHtML

[U44] PHP：开启严格类型
来源：http://wap.hesvh.cn/Article/details/gyxnlyjtl.sHtML

declare(strict_types=1);
来源：http://www.blog.fehbvm.com/Article/details/gvflwunaf.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.fehbvm.com/Article/details/gcerdosxq.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gmypbospt.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.zdbjq.cn/Article/details/goiekfdca.sHtML

?string $name = null
来源：http://m.share.zdbjq.cn/Article/details/gxjgzgtyb.sHtML

[U47] PHP：联合类型
来源：http://baike.fehbvm.com/Article/details/gpmfjxage.sHtML

int|string $id
来源：http://read.share.zdbjq.cn/Article/details/gvugcvght.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gfiqqzcxe.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.fehbvm.com/Article/details/gqvvodhfj.sHtML

[U49] PHP：只读属性
来源：http://blog.zdbjq.cn/Article/details/gxbzpcyft.sHtML

public readonly string $name
来源：http://read.share.hesvh.cn/Article/details/gyekalxwz.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.zdbjq.cn/Article/details/gkccaxvck.sHtML

public function __construct(private int $id) {}
来源：http://www.share.fehbvm.com/Article/details/gjxrhapbx.sHtML

[U51] PHP：数组解构
来源：http://read.share.hesvh.cn/Article/details/grrkqifqf.sHtML

[$a, $b] = $arr;
来源：http://m.share.fehbvm.com/Article/details/givwbkicz.sHtML

[U52] PHP：箭头函数
来源：http://blog.hesvh.cn/Article/details/greyvoxmp.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.fehbvm.com/Article/details/gukhcmhkm.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.zdbjq.cn/Article/details/gmxdxtnvz.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.fehbvm.com/Article/details/gnbomlmet.sHtML

[U54] PHP：空安全调用
来源：http://www.share.zdbjq.cn/Article/details/gonzoehzm.sHtML

$obj?->method()
来源：http://3g.hesvh.cn/Article/details/grzyhzjfy.sHtML

[U55] PHP：match 表达式
来源：http://blog.hesvh.cn/Article/details/ggxtxjikn.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.zdbjq.cn/Article/details/gjskuomay.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.zdbjq.cn/Article/details/gqpmphdhj.sHtML

f(a: 1, b: 2)
来源：http://www.share.hesvh.cn/Article/details/gbysoltir.sHtML

[U57] PHP：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gpldwiaxf.sHtML

"值: {$a}"
来源：http://3g.zdbjq.cn/Article/details/glmdqhztq.sHtML

[U58] PHP：数组三件套
来源：http://wap.hesvh.cn/Article/details/gijfpvdss.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.fehbvm.com/Article/details/grgxwaels.sHtML

[U59] PHP：自定义排序
来源：http://m.share.hesvh.cn/Article/details/gzyaxckvo.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.zdbjq.cn/Article/details/gnnwbfygg.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.zdbjq.cn/Article/details/gcrbdqrol.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.zdbjq.cn/Article/details/gxrfrsnlx.sHtML

[U61] PHP：正则
来源：http://read.share.zdbjq.cn/Article/details/ggmkyilqk.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gvzefykfi.sHtML

[U62] PHP：日期对象
来源：http://m.share.hesvh.cn/Article/details/gjtdapmzz.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.fehbvm.com/Article/details/gobjathut.sHtML

[U63] PHP：文件读写
来源：http://www.share.fehbvm.com/Article/details/gaagwcpcf.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.fehbvm.com/Article/details/ginobmsez.sHtML

[U64] PHP：目录遍历
来源：http://wap.hesvh.cn/Article/details/gkucpeahw.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.fehbvm.com/Article/details/gubouzlrx.sHtML

[U65] PHP：会话
来源：http://www.blog.zdbjq.cn/Article/details/gbttgyrbf.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gorqujtcs.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.hesvh.cn/Article/details/gxyjzmqia.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.hesvh.cn/Article/details/gmhmzwlta.sHtML

[U67] PHP：处理文件上传
来源：http://wap.hesvh.cn/Article/details/gjctyjhbm.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.zdbjq.cn/Article/details/ghcfiirnt.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.hesvh.cn/Article/details/gccivlizt.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.hesvh.cn/Article/details/geyluyhiu.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.hesvh.cn/Article/details/gtsinkmbt.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.zdbjq.cn/Article/details/gpjbzvbmk.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.hesvh.cn/Article/details/gleqqynqg.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.zdbjq.cn/Article/details/gdskapjgl.sHtML

[U71] PHP：抛出异常
来源：http://3g.zdbjq.cn/Article/details/gvcelxpog.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.hesvh.cn/Article/details/grshjatsu.sHtML

[U72] PHP：写错误日志
来源：http://baike.zdbjq.cn/Article/details/goykycgrc.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.fehbvm.com/Article/details/giwbiayeq.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.hesvh.cn/Article/details/gnrlqyild.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.fehbvm.com/Article/details/gmcccwyvk.sHtML

[U74] PHP：读取环境变量
来源：http://wap.hesvh.cn/Article/details/ghgytuqqf.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.fehbvm.com/Article/details/gzhvhckwe.sHtML

[U75] PHP：依赖注入
来源：http://blog.hesvh.cn/Article/details/gxwyzopps.sHtML

composer require psr/container
来源：http://read.share.hesvh.cn/Article/details/gnhiijfao.sHtML

[U76] PHP：简单路由
来源：http://m.share.fehbvm.com/Article/details/gwlbfxstb.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.zdbjq.cn/Article/details/gkdxmugfl.sHtML

[U77] PHP：模板渲染
来源：http://m.share.zdbjq.cn/Article/details/gdxqdyxrh.sHtML

composer require twig/twig
来源：http://blog.hesvh.cn/Article/details/gmshfypna.sHtML

[U78] PHP：单元测试
来源：http://www.blog.fehbvm.com/Article/details/gpswjirha.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.hesvh.cn/Article/details/gzphovnra.sHtML

[U79] PHP：静态分析
来源：http://wap.fehbvm.com/Article/details/gpkcnookx.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.fehbvm.com/Article/details/gtdrvlohi.sHtML

[U80] PHP：代码规范修复
来源：http://3g.hesvh.cn/Article/details/gnxxqnnhu.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.fehbvm.com/Article/details/gurayyfam.sHtML

[U81] JS：初始化项目
来源：http://3g.fehbvm.com/Article/details/gwgeibviz.sHtML

npm init -y;  npm i express
来源：http://wap.hesvh.cn/Article/details/gtjsdogrq.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.hesvh.cn/Article/details/ghqkutnlb.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.fehbvm.com/Article/details/gsgpujlmc.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.fehbvm.com/Article/details/gleqmqtai.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.hesvh.cn/Article/details/gcdstwsja.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.zdbjq.cn/Article/details/gizxdrblr.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.hesvh.cn/Article/details/gfzfwgurz.sHtML


<!-- 参考信息 -->