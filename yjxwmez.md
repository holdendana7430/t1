代发 wailian999

[T01] Kotlin：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gdpmvqfpq.sHtML

println("Hello")
来源：http://wap.hesvh.cn/Article/details/ggsolqkha.sHtML

[T02] Kotlin：变量
来源：http://m.share.zdbjq.cn/Article/details/gacklgnwm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fehbvm.com/Article/details/gjilghwag.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fehbvm.com/Article/details/gdmnhojwy.sHtML

"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/gianorpun.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.hesvh.cn/Article/details/gevjwbrdd.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fehbvm.com/Article/details/getsjcafs.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.hesvh.cn/Article/details/gyoocydhy.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fehbvm.com/Article/details/glyxtbrof.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.hesvh.cn/Article/details/gcdrxqauw.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.hesvh.cn/Article/details/gdublaurx.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.zdbjq.cn/Article/details/gbvxcnyyl.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/gcjvvmzbi.sHtML

[T08] Kotlin：数据类
来源：http://www.share.hesvh.cn/Article/details/gwlowpbfx.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.hesvh.cn/Article/details/gaitoxsqd.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.hesvh.cn/Article/details/gykdqykye.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fehbvm.com/Article/details/gyjfoxaup.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.zdbjq.cn/Article/details/gyeerfljt.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fehbvm.com/Article/details/gotsviyue.sHtML

[T11] Kotlin：协程
来源：http://www.share.hesvh.cn/Article/details/gdrmlwvzo.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.zdbjq.cn/Article/details/gczgjmjkl.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fehbvm.com/Article/details/ggaunhuvh.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/ggopbgwml.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.hesvh.cn/Article/details/gubraxgfs.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fehbvm.com/Article/details/gmttvspqg.sHtML

[T14] Kotlin：循环
来源：http://blog.hesvh.cn/Article/details/ghlddemqa.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fehbvm.com/Article/details/grhusucdx.sHtML

[T15] Kotlin：接口
来源：http://blog.hesvh.cn/Article/details/grflhxbky.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.zdbjq.cn/Article/details/gajnfayrs.sHtML

[T16] Swift：Hello World
来源：http://baike.fehbvm.com/Article/details/glstrssqz.sHtML

print("Hello")
来源：http://blog.zdbjq.cn/Article/details/gskktaguv.sHtML

[T17] Swift：变量与常量
来源：http://wap.zdbjq.cn/Article/details/gdbshicqd.sHtML

var a = 1;  let b = 2
来源：http://wap.hesvh.cn/Article/details/gutrmnhdh.sHtML

[T18] Swift：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gavxnbczg.sHtML

"值: \(b)"
来源：http://wap.fehbvm.com/Article/details/gqqvkhbag.sHtML

[T19] Swift：可选绑定
来源：http://3g.fehbvm.com/Article/details/gozziovey.sHtML

if let n = opt { print(n) }
来源：http://blog.hesvh.cn/Article/details/gwbccboow.sHtML

[T20] Swift：数组操作
来源：http://www.blog.hesvh.cn/Article/details/gtnjvjfdg.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fehbvm.com/Article/details/gjyaceyqd.sHtML

[T21] Swift：遍历
来源：http://baike.zdbjq.cn/Article/details/gttdegexb.sHtML

for x in a { print(x) }
来源：http://read.share.hesvh.cn/Article/details/ghwtsgtme.sHtML

[T22] Swift：字典
来源：http://mobile.hesvh.cn/Article/details/ghucvsyqy.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fehbvm.com/Article/details/gslggelxi.sHtML

[T23] Swift：函数
来源：http://baike.zdbjq.cn/Article/details/gwcuopzdh.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fehbvm.com/Article/details/gnxrhjwgq.sHtML

[T24] Swift：闭包
来源：http://mobile.fehbvm.com/Article/details/grjlazfdn.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fehbvm.com/Article/details/gccbsfjci.sHtML

[T25] Swift：结构体
来源：http://m.share.zdbjq.cn/Article/details/gahrwzalx.sHtML

struct P { var x: Int }
来源：http://blog.zdbjq.cn/Article/details/gdcqfkeaj.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.zdbjq.cn/Article/details/gvqdesgfy.sHtML

class A: Base { override func f() {} }
来源：http://wap.zdbjq.cn/Article/details/garoqfhpq.sHtML

[T27] Swift：错误处理
来源：http://wap.fehbvm.com/Article/details/gyzqhdbzw.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.hesvh.cn/Article/details/gqyocvehi.sHtML

[T28] Swift：枚举
来源：http://3g.fehbvm.com/Article/details/ggcmllczb.sHtML

enum Color { case red, green }
来源：http://www.share.fehbvm.com/Article/details/glyqlwwuf.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.zdbjq.cn/Article/details/gqenlqarb.sHtML

guard let x = opt else { return }
来源：http://wap.hesvh.cn/Article/details/gvbotctmv.sHtML

[T30] Swift：协议
来源：http://www.blog.zdbjq.cn/Article/details/gfvrnzldg.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.hesvh.cn/Article/details/gviohnfvz.sHtML

[T31] Lua：Hello World
来源：http://read.share.hesvh.cn/Article/details/gkmitciho.sHtML

print("Hello")
来源：http://baike.hesvh.cn/Article/details/gagfyorpy.sHtML

[T32] Lua：局部变量
来源：http://www.share.fehbvm.com/Article/details/gfoqkhhrp.sHtML

local a = 1
来源：http://3g.fehbvm.com/Article/details/gkdgfbpwi.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.zdbjq.cn/Article/details/gybwrsrti.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.hesvh.cn/Article/details/gjebkzldv.sHtML

[T34] Lua：遍历表
来源：http://www.share.zdbjq.cn/Article/details/gpgzgcmyq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.hesvh.cn/Article/details/gcyvypmub.sHtML

[T35] Lua：字典表
来源：http://blog.fehbvm.com/Article/details/gwdzwbemc.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.zdbjq.cn/Article/details/gjoaezfky.sHtML

[T36] Lua：函数
来源：http://www.blog.zdbjq.cn/Article/details/gpimbntie.sHtML

function add(a, b) return a + b end
来源：http://blog.fehbvm.com/Article/details/goiptgbhf.sHtML

[T37] Lua：字符串拼接
来源：http://wap.fehbvm.com/Article/details/gljvcziko.sHtML

"a" .. "b"
来源：http://3g.hesvh.cn/Article/details/gogzgfbqg.sHtML

[T38] Lua：条件
来源：http://m.share.hesvh.cn/Article/details/goetffuca.sHtML

if x > 0 then print("正") end
来源：http://www.share.hesvh.cn/Article/details/gmwglmhbm.sHtML

[T39] Lua：模式匹配
来源：http://3g.hesvh.cn/Article/details/gfkqnszia.sHtML

string.find(s, "%d+")
来源：http://www.share.hesvh.cn/Article/details/gxocbbauj.sHtML

[T40] Lua：元表
来源：http://wap.fehbvm.com/Article/details/ggzdwrgxb.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.fehbvm.com/Article/details/gnrofegpq.sHtML

[T41] Perl：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gczpoffoy.sHtML

print "Hello\n";
来源：http://blog.zdbjq.cn/Article/details/gagkxaxbf.sHtML

[T42] Perl：变量类型
来源：http://www.blog.fehbvm.com/Article/details/glbdnckrr.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.hesvh.cn/Article/details/gqpdokame.sHtML

[T43] Perl：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gaurpbedi.sHtML

"值: $a"
来源：http://3g.zdbjq.cn/Article/details/gjlugrpbi.sHtML

[T44] Perl：条件
来源：http://mobile.zdbjq.cn/Article/details/gauvknkxq.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.hesvh.cn/Article/details/gulbxufzo.sHtML

[T45] Perl：数组遍历
来源：http://m.share.fehbvm.com/Article/details/gcbngqqbi.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjubqbhbm.sHtML

[T46] Perl：哈希操作
来源：http://mobile.fehbvm.com/Article/details/gynvppjzr.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.zdbjq.cn/Article/details/gmzrtatrd.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.hesvh.cn/Article/details/gadmudghw.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.fehbvm.com/Article/details/gdyqgxigq.sHtML

[T48] Perl：正则替换
来源：http://baike.zdbjq.cn/Article/details/gerywcqex.sHtML

$s =~ s/old/new/g;
来源：http://3g.fehbvm.com/Article/details/glmnmtxth.sHtML

[T49] Perl：函数
来源：http://wap.hesvh.cn/Article/details/gmpfqhmfw.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gpkuqxsgk.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gzucacesf.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.zdbjq.cn/Article/details/gkkhyxsph.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.zdbjq.cn/Article/details/glsguozrq.sHtML

[T51] Scala：Hello World
来源：http://mobile.fehbvm.com/Article/details/gkejswtiw.sHtML

println("Hello")
来源：http://mobile.zdbjq.cn/Article/details/ghifvsurj.sHtML

[T52] Scala：变量
来源：http://www.blog.hesvh.cn/Article/details/ggdiqzvbx.sHtML

val a = 1;  var b = 2
来源：http://3g.fehbvm.com/Article/details/ghugcnnjt.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gozzeelqk.sHtML

s"值: $b"
来源：http://baike.fehbvm.com/Article/details/grrtzudjk.sHtML

[T54] Scala：集合映射
来源：http://blog.zdbjq.cn/Article/details/gwkxqfevx.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.fehbvm.com/Article/details/gqxwtsffl.sHtML

[T55] Scala：集合过滤
来源：http://m.share.hesvh.cn/Article/details/gfljrwide.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.hesvh.cn/Article/details/giovamqgl.sHtML

[T56] Scala：样例类
来源：http://baike.hesvh.cn/Article/details/gcjxuxssa.sHtML

case class User(name: String, age: Int)
来源：http://wap.fehbvm.com/Article/details/gtfwedkbv.sHtML

[T57] Scala：模式匹配
来源：http://m.share.fehbvm.com/Article/details/ggioxdhty.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.zdbjq.cn/Article/details/gcyehwszi.sHtML

[T58] Scala：函数定义
来源：http://mobile.fehbvm.com/Article/details/gnqlhtyvz.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.hesvh.cn/Article/details/gcxcgkeku.sHtML

[T59] Scala：循环
来源：http://wap.fehbvm.com/Article/details/grtojaojf.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.fehbvm.com/Article/details/gokdgcecj.sHtML

[T60] Scala：折叠
来源：http://read.share.zdbjq.cn/Article/details/govfwctnq.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.fehbvm.com/Article/details/gweojhevb.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gdubfjgyi.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.zdbjq.cn/Article/details/gsnghyppn.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gmtjazsyh.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.fehbvm.com/Article/details/gzjrcmrci.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.hesvh.cn/Article/details/gwlrpohkk.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.zdbjq.cn/Article/details/gluyjmvps.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.fehbvm.com/Article/details/gzqzngoax.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.zdbjq.cn/Article/details/gshnncotu.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.fehbvm.com/Article/details/gkzphhuxg.sHtML

[U04] Py：变量调试打印
来源：http://3g.zdbjq.cn/Article/details/gkxgbvyos.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.fehbvm.com/Article/details/gvudxiifq.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.hesvh.cn/Article/details/gyayvndav.sHtML

list(dict.fromkeys(arr))
来源：http://baike.hesvh.cn/Article/details/gzpaqhsod.sHtML

[U06] Py：合并两个字典
来源：http://blog.hesvh.cn/Article/details/gjjkcshba.sHtML

{**a, **b}
来源：http://3g.hesvh.cn/Article/details/gojslveld.sHtML

[U07] Py：反转字典键值
来源：http://m.share.zdbjq.cn/Article/details/gzaamgvsd.sHtML

{v: k for k, v in d.items()}
来源：http://3g.zdbjq.cn/Article/details/giozursii.sHtML

[U08] Py：展平二维列表
来源：http://m.share.fehbvm.com/Article/details/gaikfwaof.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.fehbvm.com/Article/details/gjepwiosf.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.zdbjq.cn/Article/details/gdhludzel.sHtML

max(d, key=d.get)
来源：http://wap.fehbvm.com/Article/details/gwjaznmlt.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.fehbvm.com/Article/details/gomqgtnlh.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.zdbjq.cn/Article/details/gckpcapzm.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.fehbvm.com/Article/details/gtntiwsqu.sHtML

(x * 2 for x in arr)
来源：http://baike.fehbvm.com/Article/details/gaippsypg.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.hesvh.cn/Article/details/grhwwifen.sHtML

Counter(arr).most_common(3)
来源：http://blog.hesvh.cn/Article/details/gnjnffvht.sHtML

[U13] Py：固定长度队列
来源：http://wap.fehbvm.com/Article/details/ghttkjaeg.sHtML

deque(maxlen=10)
来源：http://3g.zdbjq.cn/Article/details/gtxphqklw.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.fehbvm.com/Article/details/gevdrlmrn.sHtML

defaultdict(list)
来源：http://baike.fehbvm.com/Article/details/gykiosigo.sHtML

[U15] Py：高精度计时
来源：http://3g.zdbjq.cn/Article/details/gbkkotagg.sHtML

t = time.perf_counter()
来源：http://read.share.fehbvm.com/Article/details/ggptdnqfl.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.hesvh.cn/Article/details/gohxvmply.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.hesvh.cn/Article/details/gxjfkhcwh.sHtML

[U17] Py：初始化日志
来源：http://baike.fehbvm.com/Article/details/gosjybhfc.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.hesvh.cn/Article/details/gqnobrkat.sHtML

[U18] Py：预编译正则
来源：http://baike.hesvh.cn/Article/details/gytntkzon.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.fehbvm.com/Article/details/gcsqecalf.sHtML

[U19] Py：正则替换带回调
来源：http://wap.hesvh.cn/Article/details/gtgboirat.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.zdbjq.cn/Article/details/gpuvwikzy.sHtML

[U20] Py：缓存函数结果
来源：http://blog.hesvh.cn/Article/details/gjlcykikb.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.zdbjq.cn/Article/details/gdacfqrxr.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.fehbvm.com/Article/details/gnumguduv.sHtML

@contextlib.contextmanager
来源：http://mobile.hesvh.cn/Article/details/ggnqamnaw.sHtML

[U22] Py：矩阵转置
来源：http://3g.hesvh.cn/Article/details/gsqyflouo.sHtML

list(zip(*m))
来源：http://read.share.zdbjq.cn/Article/details/giivnjdhr.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.hesvh.cn/Article/details/gkipsabli.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.hesvh.cn/Article/details/glvrwuiss.sHtML

[U24] Py：路径操作
来源：http://3g.hesvh.cn/Article/details/gcudeqoja.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.hesvh.cn/Article/details/ghjisbwhk.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.zdbjq.cn/Article/details/gurludaco.sHtML

csv.DictReader(f)
来源：http://www.blog.fehbvm.com/Article/details/ghandcddx.sHtML

[U26] Py：并发下载
来源：http://baike.fehbvm.com/Article/details/gsuyhmyzb.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.zdbjq.cn/Article/details/gspiaator.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.zdbjq.cn/Article/details/gbytopsuo.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.hesvh.cn/Article/details/gugshfvyj.sHtML

[U28] Py：类型别名
来源：http://www.m.share.hesvh.cn/Article/details/gvitfsdvf.sHtML

UserId = int
来源：http://read.share.hesvh.cn/Article/details/gurevqoab.sHtML

[U29] Py：属性校验
来源：http://read.share.fehbvm.com/Article/details/gnjczduuy.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.hesvh.cn/Article/details/gwttnswus.sHtML

[U30] Py：数据类
来源：http://mobile.zdbjq.cn/Article/details/gguwtqkal.sHtML

@dataclass(slots=True)
来源：http://3g.zdbjq.cn/Article/details/gsmframmc.sHtML

[U31] Py：单测
来源：http://read.share.zdbjq.cn/Article/details/gzdqjhfjq.sHtML

python -m pytest -q
来源：http://www.share.hesvh.cn/Article/details/griiwnerv.sHtML

[U32] Py：代码格式化
来源：http://baike.hesvh.cn/Article/details/gkzholxrp.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.zdbjq.cn/Article/details/gjtclqecj.sHtML

[U33] Py：打包发布
来源：http://blog.zdbjq.cn/Article/details/gwweohats.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.hesvh.cn/Article/details/grvuenioj.sHtML

[U34] Py：判断编码
来源：http://mobile.hesvh.cn/Article/details/grmvyurca.sHtML

chardet.detect(raw)
来源：http://m.share.fehbvm.com/Article/details/gxivyrkbv.sHtML

[U35] Py：发送邮件
来源：http://www.blog.fehbvm.com/Article/details/gyqclqwto.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.fehbvm.com/Article/details/gmsroxrkc.sHtML

[U36] Py：定时任务
来源：http://mobile.fehbvm.com/Article/details/grhjjjptp.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.zdbjq.cn/Article/details/gyjrjnlvp.sHtML

[U37] Py：读写 Excel
来源：http://read.share.fehbvm.com/Article/details/gxzlxavez.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.fehbvm.com/Article/details/gnpqnvpjw.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.hesvh.cn/Article/details/gscccmcjw.sHtML

Path(__file__).resolve().parent
来源：http://baike.zdbjq.cn/Article/details/gztmvtowv.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.zdbjq.cn/Article/details/gtpvahoys.sHtML

sys.stdout.isatty()
来源：http://www.m.share.fehbvm.com/Article/details/gxymqsrdg.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.zdbjq.cn/Article/details/grwmiqfxx.sHtML

print("err", file=sys.stderr)
来源：http://3g.hesvh.cn/Article/details/gmhktpfma.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.zdbjq.cn/Article/details/gopcyvxgo.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.zdbjq.cn/Article/details/gfovxunzx.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.hesvh.cn/Article/details/geeljxrlw.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.fehbvm.com/Article/details/gpcwdazvr.sHtML

[U43] PHP：声明命名空间
来源：http://baike.fehbvm.com/Article/details/gkpoyfhgm.sHtML

namespace App\Http;
来源：http://www.m.share.hesvh.cn/Article/details/gcvhqxhqa.sHtML

[U44] PHP：开启严格类型
来源：http://3g.hesvh.cn/Article/details/ghjfbbyrd.sHtML

declare(strict_types=1);
来源：http://m.share.zdbjq.cn/Article/details/gqmegyhax.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.fehbvm.com/Article/details/gtntczatp.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gxpxllddg.sHtML

[U46] PHP：可空类型
来源：http://wap.hesvh.cn/Article/details/gglbdfote.sHtML

?string $name = null
来源：http://www.share.hesvh.cn/Article/details/genhvjplz.sHtML

[U47] PHP：联合类型
来源：http://m.share.zdbjq.cn/Article/details/gmimfctpy.sHtML

int|string $id
来源：http://3g.hesvh.cn/Article/details/gnnomjudu.sHtML

[U48] PHP：纯枚举
来源：http://www.share.hesvh.cn/Article/details/glvkjmfai.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.zdbjq.cn/Article/details/ggubfnont.sHtML

[U49] PHP：只读属性
来源：http://read.share.hesvh.cn/Article/details/gykhyggnr.sHtML

public readonly string $name
来源：http://read.share.hesvh.cn/Article/details/gjeflnteq.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.zdbjq.cn/Article/details/gslywhwlf.sHtML

public function __construct(private int $id) {}
来源：http://m.share.hesvh.cn/Article/details/gafnkrana.sHtML

[U51] PHP：数组解构
来源：http://read.share.fehbvm.com/Article/details/gjhxxskqh.sHtML

[$a, $b] = $arr;
来源：http://m.share.zdbjq.cn/Article/details/gjpanzoij.sHtML

[U52] PHP：箭头函数
来源：http://www.share.zdbjq.cn/Article/details/gjiphbsvn.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.hesvh.cn/Article/details/gtimtmhtn.sHtML

[U53] PHP：空合并运算符
来源：http://blog.zdbjq.cn/Article/details/gdslgpkra.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.hesvh.cn/Article/details/glokvkasb.sHtML

[U54] PHP：空安全调用
来源：http://3g.hesvh.cn/Article/details/gfzzcxalo.sHtML

$obj?->method()
来源：http://www.m.share.hesvh.cn/Article/details/gqpdegcjl.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gpwxrqghk.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.hesvh.cn/Article/details/gvcylgkky.sHtML

[U56] PHP：命名参数
来源：http://3g.fehbvm.com/Article/details/gdozjbcge.sHtML

f(a: 1, b: 2)
来源：http://3g.zdbjq.cn/Article/details/gkrtzhakw.sHtML

[U57] PHP：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gdadirohz.sHtML

"值: {$a}"
来源：http://3g.zdbjq.cn/Article/details/gjprvkjye.sHtML

[U58] PHP：数组三件套
来源：http://baike.fehbvm.com/Article/details/gahrhbbgm.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.fehbvm.com/Article/details/gkalrxind.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.fehbvm.com/Article/details/gfjjkalcl.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.zdbjq.cn/Article/details/gnhjqejoa.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.zdbjq.cn/Article/details/gzensdfol.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.zdbjq.cn/Article/details/grmnnvsbj.sHtML

[U61] PHP：正则
来源：http://www.blog.fehbvm.com/Article/details/ggeigmamf.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.zdbjq.cn/Article/details/gumwmtjzm.sHtML

[U62] PHP：日期对象
来源：http://baike.zdbjq.cn/Article/details/gvncuuovx.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.fehbvm.com/Article/details/glryqkmtm.sHtML

[U63] PHP：文件读写
来源：http://www.share.zdbjq.cn/Article/details/gipopxzzp.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.hesvh.cn/Article/details/gghccimot.sHtML

[U64] PHP：目录遍历
来源：http://wap.hesvh.cn/Article/details/gkynvviie.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.zdbjq.cn/Article/details/gvcgahnir.sHtML

[U65] PHP：会话
来源：http://www.blog.fehbvm.com/Article/details/ggvtgjazr.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.hesvh.cn/Article/details/ggeleaebb.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.hesvh.cn/Article/details/gpuwlegkn.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.hesvh.cn/Article/details/gcetdqjye.sHtML

[U67] PHP：处理文件上传
来源：http://3g.hesvh.cn/Article/details/grjteqprm.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.fehbvm.com/Article/details/glqflnwpq.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.hesvh.cn/Article/details/gdeacvpbt.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.zdbjq.cn/Article/details/gbjdcymxs.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.fehbvm.com/Article/details/gncrjgpom.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.hesvh.cn/Article/details/ghyctgugo.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.zdbjq.cn/Article/details/gybxajxzc.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.fehbvm.com/Article/details/gegcfcnjc.sHtML

[U71] PHP：抛出异常
来源：http://wap.fehbvm.com/Article/details/gbcdchgvi.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.hesvh.cn/Article/details/gxsacsujo.sHtML

[U72] PHP：写错误日志
来源：http://3g.fehbvm.com/Article/details/gipgyqlcf.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.zdbjq.cn/Article/details/gvilgmnjg.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.zdbjq.cn/Article/details/gvwcfevmw.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.fehbvm.com/Article/details/gbovmdkuu.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.fehbvm.com/Article/details/gnrtsedsr.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.fehbvm.com/Article/details/gfkyqqost.sHtML

[U75] PHP：依赖注入
来源：http://3g.fehbvm.com/Article/details/gvohbadtr.sHtML

composer require psr/container
来源：http://read.share.hesvh.cn/Article/details/gwaardtsb.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.fehbvm.com/Article/details/gfnmmntsw.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.zdbjq.cn/Article/details/gcuoqyqbx.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.fehbvm.com/Article/details/giyubjecx.sHtML

composer require twig/twig
来源：http://wap.fehbvm.com/Article/details/gaxplgxcp.sHtML

[U78] PHP：单元测试
来源：http://read.share.zdbjq.cn/Article/details/gvdynxxef.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.hesvh.cn/Article/details/gaxilabxy.sHtML

[U79] PHP：静态分析
来源：http://read.share.fehbvm.com/Article/details/gljdxmpmv.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.hesvh.cn/Article/details/gdsbnwmtc.sHtML

[U80] PHP：代码规范修复
来源：http://baike.fehbvm.com/Article/details/gdmqdieco.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.zdbjq.cn/Article/details/gjvbjklmy.sHtML

[U81] JS：初始化项目
来源：http://baike.zdbjq.cn/Article/details/gwvssdsij.sHtML

npm init -y;  npm i express
来源：http://m.share.fehbvm.com/Article/details/gfryepqgh.sHtML

[U82] JS：package.json 脚本
来源：http://wap.fehbvm.com/Article/details/gsvojpaug.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.zdbjq.cn/Article/details/gogduqyzy.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.hesvh.cn/Article/details/gqenvyzpr.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.fehbvm.com/Article/details/gfwawfkrk.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.zdbjq.cn/Article/details/gwgunopvq.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.zdbjq.cn/Article/details/gwoppdmtc.sHtML

[U85] JS：可选链
来源：http://baike.hesvh.cn/Article/details/gwlctpswt.sHtML

a?.b?.c
来源：http://blog.zdbjq.cn/Article/details/gihbjqkoi.sHtML

[U86] JS：空值合并
来源：http://read.share.hesvh.cn/Article/details/gghyryawa.sHtML

a ?? b
来源：http://www.share.hesvh.cn/Article/details/glxgjogvq.sHtML

[U87] JS：解构默认值
来源：http://blog.zdbjq.cn/Article/details/grbexumrb.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.hesvh.cn/Article/details/giiynrumd.sHtML

[U88] JS：对象展开合并
来源：http://www.share.zdbjq.cn/Article/details/gcpfitovy.sHtML

{ ...a, ...b }
来源：http://www.share.hesvh.cn/Article/details/ggzsirupl.sHtML


<!-- 参考信息 -->