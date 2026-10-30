代发 wailian999

[T05] Kotlin：when 表达式
来源：http://www.blog.hesvh.cn/Article/details/gzohpzxfh.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fehbvm.com/Article/details/gmivsbmub.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.hesvh.cn/Article/details/gmetljvhh.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gbpazjkod.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.hesvh.cn/Article/details/gczyjhqwl.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fehbvm.com/Article/details/gikphjijm.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.hesvh.cn/Article/details/gwbhzsyjr.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fehbvm.com/Article/details/gegtdbegi.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fehbvm.com/Article/details/gvyyzghgq.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.hesvh.cn/Article/details/gotcpkwvu.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fehbvm.com/Article/details/gapoyntms.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.hesvh.cn/Article/details/godjtodgk.sHtML

[T11] Kotlin：协程
来源：http://m.share.fehbvm.com/Article/details/gtyrtdtte.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.zdbjq.cn/Article/details/gxvkpxryu.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.zdbjq.cn/Article/details/glsgratgm.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gbiceafxt.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.hesvh.cn/Article/details/gphkpwtul.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fehbvm.com/Article/details/gxrzemgnq.sHtML

[T14] Kotlin：循环
来源：http://read.share.zdbjq.cn/Article/details/ggfwjgvoi.sHtML

for (i in 1..10) println(i)
来源：http://blog.fehbvm.com/Article/details/gbktluahp.sHtML

[T15] Kotlin：接口
来源：http://m.share.fehbvm.com/Article/details/gzxgtcstt.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fehbvm.com/Article/details/ghgfxuguo.sHtML

[T16] Swift：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gcfejxdty.sHtML

print("Hello")
来源：http://baike.fehbvm.com/Article/details/glmouxllq.sHtML

[T17] Swift：变量与常量
来源：http://www.share.hesvh.cn/Article/details/gkwlvvfmo.sHtML

var a = 1;  let b = 2
来源：http://www.blog.hesvh.cn/Article/details/gxfmugrrq.sHtML

[T18] Swift：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gxozdgowc.sHtML

"值: \(b)"
来源：http://www.share.fehbvm.com/Article/details/gbssjqxqe.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.hesvh.cn/Article/details/gaduivwwc.sHtML

if let n = opt { print(n) }
来源：http://www.share.fehbvm.com/Article/details/gnseulzzd.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.hesvh.cn/Article/details/gsdcqcrfc.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.zdbjq.cn/Article/details/gibpgardt.sHtML

[T21] Swift：遍历
来源：http://blog.zdbjq.cn/Article/details/gyepstluo.sHtML

for x in a { print(x) }
来源：http://3g.fehbvm.com/Article/details/gwmzgesmt.sHtML

[T22] Swift：字典
来源：http://www.share.fehbvm.com/Article/details/gktqbkwlf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.hesvh.cn/Article/details/gumeuivfs.sHtML

[T23] Swift：函数
来源：http://www.share.hesvh.cn/Article/details/gshzgbqii.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.zdbjq.cn/Article/details/grhspvqin.sHtML

[T24] Swift：闭包
来源：http://baike.zdbjq.cn/Article/details/gxapxwfmo.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gvurxnhdm.sHtML

[T25] Swift：结构体
来源：http://wap.hesvh.cn/Article/details/gsbsavnrl.sHtML

struct P { var x: Int }
来源：http://read.share.zdbjq.cn/Article/details/gkdsefryn.sHtML

[T26] Swift：类与重写
来源：http://baike.zdbjq.cn/Article/details/gtcswupmh.sHtML

class A: Base { override func f() {} }
来源：http://mobile.zdbjq.cn/Article/details/gflmyuedn.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fehbvm.com/Article/details/gpikymibk.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.fehbvm.com/Article/details/goxwaxhon.sHtML

[T28] Swift：枚举
来源：http://mobile.fehbvm.com/Article/details/gospwwvyk.sHtML

enum Color { case red, green }
来源：http://baike.hesvh.cn/Article/details/gsqgvktnr.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.zdbjq.cn/Article/details/gtkioqljz.sHtML

guard let x = opt else { return }
来源：http://blog.zdbjq.cn/Article/details/gddkdydiv.sHtML

[T30] Swift：协议
来源：http://www.blog.zdbjq.cn/Article/details/gymlcxujl.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.hesvh.cn/Article/details/gnafmxdzm.sHtML

[T31] Lua：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gwyapnkrd.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/guaagacum.sHtML

[T32] Lua：局部变量
来源：http://mobile.zdbjq.cn/Article/details/gzldsiets.sHtML

local a = 1
来源：http://www.share.hesvh.cn/Article/details/gknijgnkx.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.hesvh.cn/Article/details/gtgxvwpdl.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.zdbjq.cn/Article/details/gybekftyd.sHtML

[T34] Lua：遍历表
来源：http://m.share.zdbjq.cn/Article/details/glykcehmg.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fehbvm.com/Article/details/gvbhfvxpx.sHtML

[T35] Lua：字典表
来源：http://www.blog.hesvh.cn/Article/details/gfmhxfest.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gjfshtucb.sHtML

[T36] Lua：函数
来源：http://wap.zdbjq.cn/Article/details/gbhvzwyvx.sHtML

function add(a, b) return a + b end
来源：http://blog.zdbjq.cn/Article/details/gaintdfgp.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.zdbjq.cn/Article/details/ggsuiomrg.sHtML

"a" .. "b"
来源：http://www.blog.hesvh.cn/Article/details/gevxqvonl.sHtML

[T38] Lua：条件
来源：http://www.m.share.zdbjq.cn/Article/details/glrjicrfc.sHtML

if x > 0 then print("正") end
来源：http://blog.hesvh.cn/Article/details/gdhmchvde.sHtML

[T39] Lua：模式匹配
来源：http://baike.hesvh.cn/Article/details/gzwznpogb.sHtML

string.find(s, "%d+")
来源：http://www.share.hesvh.cn/Article/details/gmmhuzduo.sHtML

[T40] Lua：元表
来源：http://wap.zdbjq.cn/Article/details/gowtnuhza.sHtML

setmetatable({}, { __index = base })
来源：http://baike.hesvh.cn/Article/details/gwczvivfd.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gmosuhmky.sHtML

print "Hello\n";
来源：http://wap.fehbvm.com/Article/details/gkqdbyltf.sHtML

[T42] Perl：变量类型
来源：http://mobile.hesvh.cn/Article/details/gusukfvrs.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.fehbvm.com/Article/details/gaqlsfeoo.sHtML

[T43] Perl：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gsqlxwsgq.sHtML

"值: $a"
来源：http://blog.fehbvm.com/Article/details/gqauemwnz.sHtML

[T44] Perl：条件
来源：http://www.m.share.zdbjq.cn/Article/details/gzbdvaldr.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.fehbvm.com/Article/details/gyiwobtmb.sHtML

[T45] Perl：数组遍历
来源：http://m.share.fehbvm.com/Article/details/gywarngoq.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.zdbjq.cn/Article/details/gfwhkdkhi.sHtML

[T46] Perl：哈希操作
来源：http://3g.hesvh.cn/Article/details/gjnvmzfjk.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.hesvh.cn/Article/details/gtbtbhzso.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.zdbjq.cn/Article/details/gfvsugpjg.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.hesvh.cn/Article/details/gmgsheilf.sHtML

[T48] Perl：正则替换
来源：http://www.share.hesvh.cn/Article/details/ggupwbnum.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.hesvh.cn/Article/details/gkmbldfqq.sHtML

[T49] Perl：函数
来源：http://www.blog.fehbvm.com/Article/details/gecmavgsm.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/grovfsyyh.sHtML

[T50] Perl：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gpgiuvpcr.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.zdbjq.cn/Article/details/gtzamaavg.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.zdbjq.cn/Article/details/goisvvvjg.sHtML

[T51] Scala：Hello World
来源：http://mobile.fehbvm.com/Article/details/gokhbmfth.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/gtlrsraim.sHtML

[T52] Scala：变量
来源：http://mobile.hesvh.cn/Article/details/gxhykyqly.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.hesvh.cn/Article/details/gcpzneyti.sHtML

[T53] Scala：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gucmvduaz.sHtML

s"值: $b"
来源：http://3g.zdbjq.cn/Article/details/grapawkmx.sHtML

[T54] Scala：集合映射
来源：http://blog.fehbvm.com/Article/details/gzudyuafo.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.zdbjq.cn/Article/details/grrkzjcbx.sHtML

[T55] Scala：集合过滤
来源：http://www.share.zdbjq.cn/Article/details/gdgqzmsck.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.fehbvm.com/Article/details/gvamzawsk.sHtML

[T56] Scala：样例类
来源：http://m.share.zdbjq.cn/Article/details/gtkettlut.sHtML

case class User(name: String, age: Int)
来源：http://blog.fehbvm.com/Article/details/gvdorwgbs.sHtML

[T57] Scala：模式匹配
来源：http://wap.hesvh.cn/Article/details/gnylolapt.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.zdbjq.cn/Article/details/gomkymqgd.sHtML

[T58] Scala：函数定义
来源：http://baike.fehbvm.com/Article/details/gnwbeifmg.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.zdbjq.cn/Article/details/gzjygnytl.sHtML

[T59] Scala：循环
来源：http://baike.zdbjq.cn/Article/details/gmuqklgjk.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.fehbvm.com/Article/details/gtoeugicr.sHtML

[T60] Scala：折叠
来源：http://www.share.zdbjq.cn/Article/details/gvixtdhov.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.fehbvm.com/Article/details/gdhgjamir.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gnbhdptxj.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.hesvh.cn/Article/details/giuzhgupa.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ghsstbgml.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.zdbjq.cn/Article/details/godmfjaap.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.fehbvm.com/Article/details/gpsddmnsh.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.hesvh.cn/Article/details/gwrzyqckt.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.zdbjq.cn/Article/details/gyrnattno.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.hesvh.cn/Article/details/gjalumuml.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.zdbjq.cn/Article/details/gxjarcovj.sHtML

[U04] Py：变量调试打印
来源：http://3g.hesvh.cn/Article/details/gcmpsqxrw.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.zdbjq.cn/Article/details/gsscznpmp.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.zdbjq.cn/Article/details/gewbszvur.sHtML

list(dict.fromkeys(arr))
来源：http://blog.hesvh.cn/Article/details/gdyeqejlm.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.fehbvm.com/Article/details/gceymtrru.sHtML

{**a, **b}
来源：http://m.share.fehbvm.com/Article/details/gvxatzhqw.sHtML

[U07] Py：反转字典键值
来源：http://mobile.zdbjq.cn/Article/details/gpcqfvatr.sHtML

{v: k for k, v in d.items()}
来源：http://wap.zdbjq.cn/Article/details/gukerzxwi.sHtML

[U08] Py：展平二维列表
来源：http://www.share.hesvh.cn/Article/details/ggajmlsxw.sHtML

[y for x in nested for y in x]
来源：http://m.share.hesvh.cn/Article/details/gbesrmncu.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.zdbjq.cn/Article/details/gxfqxapuo.sHtML

max(d, key=d.get)
来源：http://www.m.share.hesvh.cn/Article/details/gwqggdvhb.sHtML

[U10] Py：按值排序字典
来源：http://www.share.fehbvm.com/Article/details/glrldzyqk.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.fehbvm.com/Article/details/gqcdyxorx.sHtML

[U11] Py：生成器表达式
来源：http://wap.hesvh.cn/Article/details/gfvuicudo.sHtML

(x * 2 for x in arr)
来源：http://www.share.zdbjq.cn/Article/details/gpsytbivl.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.fehbvm.com/Article/details/govfrtqac.sHtML

Counter(arr).most_common(3)
来源：http://m.share.fehbvm.com/Article/details/gihxonamf.sHtML

[U13] Py：固定长度队列
来源：http://blog.fehbvm.com/Article/details/gmktfggiq.sHtML

deque(maxlen=10)
来源：http://wap.zdbjq.cn/Article/details/gnapvcczq.sHtML

[U14] Py：分组收集到列表
来源：http://baike.zdbjq.cn/Article/details/ggygfbvzx.sHtML

defaultdict(list)
来源：http://wap.hesvh.cn/Article/details/gagckyhfv.sHtML

[U15] Py：高精度计时
来源：http://www.share.fehbvm.com/Article/details/grorssiuj.sHtML

t = time.perf_counter()
来源：http://baike.fehbvm.com/Article/details/gqhqteaej.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.fehbvm.com/Article/details/gerxwvysh.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.zdbjq.cn/Article/details/gqvlbnjie.sHtML

[U17] Py：初始化日志
来源：http://www.blog.fehbvm.com/Article/details/glahntonm.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.fehbvm.com/Article/details/gymrrihub.sHtML

[U18] Py：预编译正则
来源：http://mobile.zdbjq.cn/Article/details/gzjxnodhc.sHtML

pat = re.compile(r"\d+")
来源：http://baike.hesvh.cn/Article/details/gqpqsxguq.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.zdbjq.cn/Article/details/gfvkwyfbw.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.zdbjq.cn/Article/details/gvubmxzcy.sHtML

[U20] Py：缓存函数结果
来源：http://blog.zdbjq.cn/Article/details/gymlzpnju.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.zdbjq.cn/Article/details/gygeccnzz.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.zdbjq.cn/Article/details/gqvzhogba.sHtML

@contextlib.contextmanager
来源：http://www.share.hesvh.cn/Article/details/ghqxdbcon.sHtML

[U22] Py：矩阵转置
来源：http://baike.fehbvm.com/Article/details/gxrqthhwy.sHtML

list(zip(*m))
来源：http://www.m.share.hesvh.cn/Article/details/gbvqitadm.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.zdbjq.cn/Article/details/gfhoqvkbf.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.hesvh.cn/Article/details/gfvmeduvz.sHtML

[U24] Py：路径操作
来源：http://baike.fehbvm.com/Article/details/ggtrdfwge.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.fehbvm.com/Article/details/gtnvutuxp.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.zdbjq.cn/Article/details/gbtxabptz.sHtML

csv.DictReader(f)
来源：http://3g.fehbvm.com/Article/details/gjjcuuvac.sHtML

[U26] Py：并发下载
来源：http://www.blog.hesvh.cn/Article/details/ghrwtezmi.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.fehbvm.com/Article/details/gsjacbsji.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.fehbvm.com/Article/details/gqswtrtgc.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.fehbvm.com/Article/details/glgedarww.sHtML

[U28] Py：类型别名
来源：http://wap.zdbjq.cn/Article/details/guzklwsue.sHtML

UserId = int
来源：http://www.blog.fehbvm.com/Article/details/ghserhvtu.sHtML

[U29] Py：属性校验
来源：http://www.blog.fehbvm.com/Article/details/gtwjunyth.sHtML

@property 与 @x.setter 配合
来源：http://3g.hesvh.cn/Article/details/gsdhakxnd.sHtML

[U30] Py：数据类
来源：http://blog.fehbvm.com/Article/details/gevqfowxf.sHtML

@dataclass(slots=True)
来源：http://wap.fehbvm.com/Article/details/goqlogjxo.sHtML

[U31] Py：单测
来源：http://www.m.share.zdbjq.cn/Article/details/ggmksfvij.sHtML

python -m pytest -q
来源：http://baike.zdbjq.cn/Article/details/gqzsxmyxt.sHtML

[U32] Py：代码格式化
来源：http://3g.zdbjq.cn/Article/details/gegtqbksf.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.hesvh.cn/Article/details/glqgyogbm.sHtML

[U33] Py：打包发布
来源：http://baike.hesvh.cn/Article/details/gvjhlopnd.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.hesvh.cn/Article/details/gmalaamht.sHtML

[U34] Py：判断编码
来源：http://blog.zdbjq.cn/Article/details/gexuorlvi.sHtML

chardet.detect(raw)
来源：http://mobile.zdbjq.cn/Article/details/gjfsnutor.sHtML

[U35] Py：发送邮件
来源：http://www.blog.fehbvm.com/Article/details/gjgnzhalv.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.zdbjq.cn/Article/details/greakwivc.sHtML

[U36] Py：定时任务
来源：http://m.share.fehbvm.com/Article/details/gmupfuzmw.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.zdbjq.cn/Article/details/gnkzzhruv.sHtML

[U37] Py：读写 Excel
来源：http://wap.hesvh.cn/Article/details/groslkdew.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.fehbvm.com/Article/details/gklzurvmq.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.hesvh.cn/Article/details/gsjeiyqwi.sHtML

Path(__file__).resolve().parent
来源：http://m.share.zdbjq.cn/Article/details/gtzpypzbw.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.fehbvm.com/Article/details/gqnilrgoa.sHtML

sys.stdout.isatty()
来源：http://baike.fehbvm.com/Article/details/gbwpyrbzr.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.fehbvm.com/Article/details/guyhmsmkc.sHtML

print("err", file=sys.stderr)
来源：http://read.share.fehbvm.com/Article/details/gypmzvfdh.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.fehbvm.com/Article/details/gfziuhwpg.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.hesvh.cn/Article/details/gzfuxrgaj.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.zdbjq.cn/Article/details/gnbhmfztg.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.fehbvm.com/Article/details/gruiwzjpv.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.hesvh.cn/Article/details/gpewvtduz.sHtML

namespace App\Http;
来源：http://m.share.fehbvm.com/Article/details/grutpmpye.sHtML

[U44] PHP：开启严格类型
来源：http://baike.hesvh.cn/Article/details/gcfgtkdmd.sHtML

declare(strict_types=1);
来源：http://mobile.hesvh.cn/Article/details/gjbjbrhpq.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.hesvh.cn/Article/details/gqnrzzubc.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/gxjzqvgcj.sHtML

[U46] PHP：可空类型
来源：http://mobile.fehbvm.com/Article/details/gaispdfht.sHtML

?string $name = null
来源：http://3g.fehbvm.com/Article/details/glerxrhsi.sHtML

[U47] PHP：联合类型
来源：http://read.share.fehbvm.com/Article/details/gkmaoyphn.sHtML

int|string $id
来源：http://www.share.zdbjq.cn/Article/details/gloqwnwho.sHtML

[U48] PHP：纯枚举
来源：http://blog.zdbjq.cn/Article/details/goucaynhe.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.fehbvm.com/Article/details/geqhsouef.sHtML

[U49] PHP：只读属性
来源：http://blog.fehbvm.com/Article/details/gydbsyjoj.sHtML

public readonly string $name
来源：http://blog.zdbjq.cn/Article/details/gwwaruypk.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.zdbjq.cn/Article/details/gotqudpra.sHtML

public function __construct(private int $id) {}
来源：http://blog.zdbjq.cn/Article/details/gpqbhbvnw.sHtML

[U51] PHP：数组解构
来源：http://read.share.fehbvm.com/Article/details/gbanrvorj.sHtML

[$a, $b] = $arr;
来源：http://read.share.hesvh.cn/Article/details/glcfhbmzu.sHtML

[U52] PHP：箭头函数
来源：http://www.share.fehbvm.com/Article/details/gayjmdrfr.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.hesvh.cn/Article/details/gsmartofk.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.fehbvm.com/Article/details/gxxthnfsk.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.zdbjq.cn/Article/details/ghhbrgdpo.sHtML

[U54] PHP：空安全调用
来源：http://m.share.fehbvm.com/Article/details/guazxdtkx.sHtML

$obj?->method()
来源：http://mobile.hesvh.cn/Article/details/glevpzrnf.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.fehbvm.com/Article/details/gmfzckgah.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.zdbjq.cn/Article/details/gpcbxnrnf.sHtML

[U56] PHP：命名参数
来源：http://m.share.zdbjq.cn/Article/details/gsvizyqjf.sHtML

f(a: 1, b: 2)
来源：http://www.share.zdbjq.cn/Article/details/ghuzurpkb.sHtML

[U57] PHP：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gpvanjhvt.sHtML

"值: {$a}"
来源：http://www.m.share.fehbvm.com/Article/details/gtqtrabse.sHtML

[U58] PHP：数组三件套
来源：http://mobile.zdbjq.cn/Article/details/gjptozwgn.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.zdbjq.cn/Article/details/gwjjjpbms.sHtML

[U59] PHP：自定义排序
来源：http://baike.fehbvm.com/Article/details/gpawjjmpd.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.hesvh.cn/Article/details/gibnuyylx.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.hesvh.cn/Article/details/gbwvdlelu.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gxydxqrme.sHtML

[U61] PHP：正则
来源：http://blog.zdbjq.cn/Article/details/gzirlauuv.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gqhsfcvib.sHtML

[U62] PHP：日期对象
来源：http://3g.zdbjq.cn/Article/details/glzjhtndt.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.zdbjq.cn/Article/details/gommjkjga.sHtML

[U63] PHP：文件读写
来源：http://mobile.zdbjq.cn/Article/details/ghknutisn.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.zdbjq.cn/Article/details/gqzvnsfni.sHtML

[U64] PHP：目录遍历
来源：http://wap.fehbvm.com/Article/details/gfamdejrr.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.hesvh.cn/Article/details/gznadpacw.sHtML

[U65] PHP：会话
来源：http://www.m.share.zdbjq.cn/Article/details/gpsvtzdms.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.hesvh.cn/Article/details/gyusrjuma.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.fehbvm.com/Article/details/gcfxwyjjl.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.zdbjq.cn/Article/details/guotpeowl.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.fehbvm.com/Article/details/gpimxztsl.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.hesvh.cn/Article/details/gkilhpajc.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.zdbjq.cn/Article/details/gxyacacfg.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.fehbvm.com/Article/details/grdkvgnym.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.zdbjq.cn/Article/details/gnobghzwz.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.hesvh.cn/Article/details/ggmkgdqmf.sHtML

[U70] PHP：PDO 事务
来源：http://baike.zdbjq.cn/Article/details/gaoczeiyl.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.fehbvm.com/Article/details/gzllfeyul.sHtML

[U71] PHP：抛出异常
来源：http://3g.fehbvm.com/Article/details/gcjbmspmo.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.fehbvm.com/Article/details/ghnuowung.sHtML

[U72] PHP：写错误日志
来源：http://m.share.zdbjq.cn/Article/details/ggcksvilu.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.zdbjq.cn/Article/details/geiinkapv.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.zdbjq.cn/Article/details/grzsadgef.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.hesvh.cn/Article/details/gqaihsysk.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.fehbvm.com/Article/details/gfzvdlbwl.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.fehbvm.com/Article/details/gpbwkavev.sHtML

[U75] PHP：依赖注入
来源：http://wap.zdbjq.cn/Article/details/gxjwohxwc.sHtML

composer require psr/container
来源：http://www.blog.fehbvm.com/Article/details/gijvaeqlx.sHtML

[U76] PHP：简单路由
来源：http://blog.hesvh.cn/Article/details/gqsqkprfa.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.fehbvm.com/Article/details/gzsgrzefc.sHtML

[U77] PHP：模板渲染
来源：http://m.share.zdbjq.cn/Article/details/gbwvrunmp.sHtML

composer require twig/twig
来源：http://www.m.share.hesvh.cn/Article/details/gcmlwdqaz.sHtML

[U78] PHP：单元测试
来源：http://mobile.fehbvm.com/Article/details/ghhlckbqw.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.hesvh.cn/Article/details/gocwuqvko.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.zdbjq.cn/Article/details/gjuysskis.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.fehbvm.com/Article/details/gtadyrdoq.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.zdbjq.cn/Article/details/gdwzurluy.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.fehbvm.com/Article/details/gxxeqsgcj.sHtML

[U81] JS：初始化项目
来源：http://www.blog.zdbjq.cn/Article/details/gmzeiflbm.sHtML

npm init -y;  npm i express
来源：http://www.m.share.hesvh.cn/Article/details/ghusmucbn.sHtML

[U82] JS：package.json 脚本
来源：http://blog.fehbvm.com/Article/details/gxzzmdxba.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.fehbvm.com/Article/details/gjnidrsfv.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.fehbvm.com/Article/details/gdzsdrzkg.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.fehbvm.com/Article/details/gjlucnwjw.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.zdbjq.cn/Article/details/gddqjhltr.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.fehbvm.com/Article/details/gwafxsctk.sHtML

[U85] JS：可选链
来源：http://read.share.zdbjq.cn/Article/details/gsjngtcib.sHtML

a?.b?.c
来源：http://baike.zdbjq.cn/Article/details/gjxvaibne.sHtML

[U86] JS：空值合并
来源：http://m.share.fehbvm.com/Article/details/gwvarcbqh.sHtML

a ?? b
来源：http://www.blog.zdbjq.cn/Article/details/gfhagctiw.sHtML

[U87] JS：解构默认值
来源：http://wap.zdbjq.cn/Article/details/gqvvzkgek.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.fehbvm.com/Article/details/guaawbzrr.sHtML

[U88] JS：对象展开合并
来源：http://baike.hesvh.cn/Article/details/gvvyytunz.sHtML

{ ...a, ...b }
来源：http://blog.hesvh.cn/Article/details/gxtquztae.sHtML

[U89] JS：数组去重
来源：http://blog.zdbjq.cn/Article/details/gjsteepwf.sHtML

[...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/gktgxdcsz.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.fehbvm.com/Article/details/gzxsbkhrd.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gorrsuckz.sHtML

[U91] JS：对象键值遍历
来源：http://baike.fehbvm.com/Article/details/gfuronerh.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.hesvh.cn/Article/details/gxycjizjc.sHtML

[U92] JS：深拷贝
来源：http://www.blog.fehbvm.com/Article/details/geazmjhuc.sHtML

structuredClone(obj)
来源：http://wap.fehbvm.com/Article/details/gwanefquf.sHtML


<!-- 参考信息 -->