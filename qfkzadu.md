代发 wailian999

[T05] Kotlin：when 表达式
来源：http://read.share.hesvh.cn/Article/details/gjqoksqsf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.zdbjq.cn/Article/details/gywerdttt.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fehbvm.com/Article/details/gtxiwquoj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.hesvh.cn/Article/details/gftrdxabj.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.hesvh.cn/Article/details/gxbpcjobk.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fehbvm.com/Article/details/gtceznojt.sHtML

[T08] Kotlin：数据类
来源：http://baike.hesvh.cn/Article/details/gzgsstqdo.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.hesvh.cn/Article/details/gfhuriovc.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.hesvh.cn/Article/details/gkbrnjrtq.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fehbvm.com/Article/details/gfvjwowfh.sHtML

[T10] Kotlin：默认参数
来源：http://blog.hesvh.cn/Article/details/giomofnud.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.zdbjq.cn/Article/details/gkvvcxtuz.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.zdbjq.cn/Article/details/gcyodplkl.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.hesvh.cn/Article/details/gulvisrpl.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fehbvm.com/Article/details/gyoljsdxe.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gwvgbfcgw.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fehbvm.com/Article/details/gdnexgcda.sHtML

val m = mapOf("a" to 1)
来源：http://blog.zdbjq.cn/Article/details/gttrrwupm.sHtML

[T14] Kotlin：循环
来源：http://baike.hesvh.cn/Article/details/gsarreube.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fehbvm.com/Article/details/ghhxauvpv.sHtML

[T15] Kotlin：接口
来源：http://baike.zdbjq.cn/Article/details/gmjwxoajy.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.hesvh.cn/Article/details/golvegyey.sHtML

[T16] Swift：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gwacldvoi.sHtML

print("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gnlnnqnoq.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fehbvm.com/Article/details/gdxawnlyf.sHtML

var a = 1;  let b = 2
来源：http://blog.hesvh.cn/Article/details/guvfjohqu.sHtML

[T18] Swift：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gitxfxpwt.sHtML

"值: \(b)"
来源：http://blog.zdbjq.cn/Article/details/gcbtbuopi.sHtML

[T19] Swift：可选绑定
来源：http://wap.fehbvm.com/Article/details/gfuwyflri.sHtML

if let n = opt { print(n) }
来源：http://baike.zdbjq.cn/Article/details/gafrbnzcx.sHtML

[T20] Swift：数组操作
来源：http://mobile.zdbjq.cn/Article/details/gramnsdqa.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fehbvm.com/Article/details/grojwufdd.sHtML

[T21] Swift：遍历
来源：http://baike.hesvh.cn/Article/details/ghgnheoak.sHtML

for x in a { print(x) }
来源：http://baike.fehbvm.com/Article/details/gkheqhmmp.sHtML

[T22] Swift：字典
来源：http://www.blog.fehbvm.com/Article/details/ghbbqjvgd.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.hesvh.cn/Article/details/gnygrpvcv.sHtML

[T23] Swift：函数
来源：http://mobile.fehbvm.com/Article/details/gdbikbbnn.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fehbvm.com/Article/details/gllcqkuts.sHtML

[T24] Swift：闭包
来源：http://blog.fehbvm.com/Article/details/ghbqmiwxk.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fehbvm.com/Article/details/gqclbbqfl.sHtML

[T25] Swift：结构体
来源：http://m.share.hesvh.cn/Article/details/gemsalkit.sHtML

struct P { var x: Int }
来源：http://wap.zdbjq.cn/Article/details/gvvzqbhwh.sHtML

[T26] Swift：类与重写
来源：http://baike.zdbjq.cn/Article/details/ggogztlrt.sHtML

class A: Base { override func f() {} }
来源：http://3g.fehbvm.com/Article/details/gbgjbcibs.sHtML

[T27] Swift：错误处理
来源：http://3g.fehbvm.com/Article/details/gsrouchxu.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.hesvh.cn/Article/details/grlhacwvf.sHtML

[T28] Swift：枚举
来源：http://read.share.fehbvm.com/Article/details/gtgplizzj.sHtML

enum Color { case red, green }
来源：http://3g.hesvh.cn/Article/details/gvtsoahod.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.zdbjq.cn/Article/details/gqcazomyk.sHtML

guard let x = opt else { return }
来源：http://read.share.hesvh.cn/Article/details/gbyenhrgz.sHtML

[T30] Swift：协议
来源：http://www.m.share.zdbjq.cn/Article/details/gfcrwszkb.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.fehbvm.com/Article/details/gludfgpsj.sHtML

[T31] Lua：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gqmzwqapa.sHtML

print("Hello")
来源：http://blog.zdbjq.cn/Article/details/gwyvxcmum.sHtML

[T32] Lua：局部变量
来源：http://read.share.hesvh.cn/Article/details/gbouopssz.sHtML

local a = 1
来源：http://m.share.fehbvm.com/Article/details/gnjnubkms.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.fehbvm.com/Article/details/gwlkaeovz.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.fehbvm.com/Article/details/gsvucqudx.sHtML

[T34] Lua：遍历表
来源：http://m.share.hesvh.cn/Article/details/gfjjybnnu.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.zdbjq.cn/Article/details/gtzckqvmg.sHtML

[T35] Lua：字典表
来源：http://www.share.zdbjq.cn/Article/details/gduwgrizg.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.zdbjq.cn/Article/details/ghldxjrlm.sHtML

[T36] Lua：函数
来源：http://blog.zdbjq.cn/Article/details/gusywcczi.sHtML

function add(a, b) return a + b end
来源：http://blog.fehbvm.com/Article/details/ggldbbkzy.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.fehbvm.com/Article/details/ggmobucxa.sHtML

"a" .. "b"
来源：http://3g.zdbjq.cn/Article/details/gqslzulma.sHtML

[T38] Lua：条件
来源：http://3g.hesvh.cn/Article/details/gcfhmdmai.sHtML

if x > 0 then print("正") end
来源：http://wap.fehbvm.com/Article/details/gqkjtyddy.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.fehbvm.com/Article/details/gjywzlrzs.sHtML

string.find(s, "%d+")
来源：http://www.m.share.hesvh.cn/Article/details/gpfjkknzy.sHtML

[T40] Lua：元表
来源：http://www.share.fehbvm.com/Article/details/gvucvbhaz.sHtML

setmetatable({}, { __index = base })
来源：http://wap.fehbvm.com/Article/details/gotgyjghj.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gnhptoqov.sHtML

print "Hello\n";
来源：http://blog.zdbjq.cn/Article/details/gmguuathe.sHtML

[T42] Perl：变量类型
来源：http://www.blog.fehbvm.com/Article/details/gcjvflpii.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.fehbvm.com/Article/details/ggeofigsg.sHtML

[T43] Perl：字符串插值
来源：http://baike.hesvh.cn/Article/details/gzlfltuxa.sHtML

"值: $a"
来源：http://www.share.hesvh.cn/Article/details/gfvewbpgq.sHtML

[T44] Perl：条件
来源：http://3g.zdbjq.cn/Article/details/goagfulxm.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.hesvh.cn/Article/details/guivsripy.sHtML

[T45] Perl：数组遍历
来源：http://wap.zdbjq.cn/Article/details/gpswyapbx.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.hesvh.cn/Article/details/gctxkotaf.sHtML

[T46] Perl：哈希操作
来源：http://blog.hesvh.cn/Article/details/gxypdsxwo.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.fehbvm.com/Article/details/gahhsfwcj.sHtML

[T47] Perl：正则捕获
来源：http://baike.fehbvm.com/Article/details/gunabjurc.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.zdbjq.cn/Article/details/gllytywhf.sHtML

[T48] Perl：正则替换
来源：http://read.share.fehbvm.com/Article/details/gsxtszsld.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.fehbvm.com/Article/details/gtebcxjci.sHtML

[T49] Perl：函数
来源：http://www.share.hesvh.cn/Article/details/gkyszsfra.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gcgmuhezw.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gdfalzegc.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.zdbjq.cn/Article/details/gsenvkpla.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.zdbjq.cn/Article/details/gggdhigrk.sHtML

[T51] Scala：Hello World
来源：http://baike.hesvh.cn/Article/details/gfdkpbkhr.sHtML

println("Hello")
来源：http://blog.hesvh.cn/Article/details/gbznyzyif.sHtML

[T52] Scala：变量
来源：http://www.blog.hesvh.cn/Article/details/gaeddhacf.sHtML

val a = 1;  var b = 2
来源：http://www.share.zdbjq.cn/Article/details/gujshxybl.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gtntqbpmp.sHtML

s"值: $b"
来源：http://www.blog.fehbvm.com/Article/details/goybjdymx.sHtML

[T54] Scala：集合映射
来源：http://blog.zdbjq.cn/Article/details/gnxjzlzhu.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.hesvh.cn/Article/details/gthfnafko.sHtML

[T55] Scala：集合过滤
来源：http://baike.hesvh.cn/Article/details/gfgdslsbp.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.zdbjq.cn/Article/details/gzhugwetd.sHtML

[T56] Scala：样例类
来源：http://m.share.fehbvm.com/Article/details/glvpkzsej.sHtML

case class User(name: String, age: Int)
来源：http://blog.zdbjq.cn/Article/details/gujmtjghf.sHtML

[T57] Scala：模式匹配
来源：http://baike.fehbvm.com/Article/details/gpfyqkxvu.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.hesvh.cn/Article/details/gjaefsurw.sHtML

[T58] Scala：函数定义
来源：http://wap.fehbvm.com/Article/details/grjkfmdii.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.hesvh.cn/Article/details/gbwrecrxr.sHtML

[T59] Scala：循环
来源：http://blog.fehbvm.com/Article/details/giutgyavh.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fehbvm.com/Article/details/grqwneyaz.sHtML

[T60] Scala：折叠
来源：http://mobile.hesvh.cn/Article/details/gyjscldat.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.zdbjq.cn/Article/details/gxpjoljis.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/grcozzycb.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.zdbjq.cn/Article/details/gvotgnfld.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/grnyovisf.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.fehbvm.com/Article/details/goqyhufsw.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.fehbvm.com/Article/details/glyhoqoiw.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.fehbvm.com/Article/details/ghdojbinj.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.hesvh.cn/Article/details/gfmebdbqp.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.hesvh.cn/Article/details/gkqdhedtm.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.zdbjq.cn/Article/details/gvubakgbr.sHtML

[U04] Py：变量调试打印
来源：http://m.share.hesvh.cn/Article/details/gjhuthqqi.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.hesvh.cn/Article/details/gcvmpabjw.sHtML

[U05] Py：列表去重且保序
来源：http://wap.fehbvm.com/Article/details/gdjgpamkq.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.hesvh.cn/Article/details/gcpwgcjqy.sHtML

[U06] Py：合并两个字典
来源：http://baike.fehbvm.com/Article/details/gifhmezbh.sHtML

{**a, **b}
来源：http://blog.zdbjq.cn/Article/details/grahdzast.sHtML

[U07] Py：反转字典键值
来源：http://mobile.zdbjq.cn/Article/details/gewxkljlc.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.fehbvm.com/Article/details/gorwylkgn.sHtML

[U08] Py：展平二维列表
来源：http://baike.zdbjq.cn/Article/details/gymrgjmsx.sHtML

[y for x in nested for y in x]
来源：http://3g.hesvh.cn/Article/details/gphrntjjs.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.fehbvm.com/Article/details/gypahjyys.sHtML

max(d, key=d.get)
来源：http://baike.zdbjq.cn/Article/details/gvlleoyoh.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.fehbvm.com/Article/details/gqlpzbmnb.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.fehbvm.com/Article/details/govepiaji.sHtML

[U11] Py：生成器表达式
来源：http://www.share.zdbjq.cn/Article/details/gyujslxcb.sHtML

(x * 2 for x in arr)
来源：http://read.share.zdbjq.cn/Article/details/ggtjlapvd.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.fehbvm.com/Article/details/gffprwyuq.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.fehbvm.com/Article/details/gwqcirakz.sHtML

[U13] Py：固定长度队列
来源：http://m.share.hesvh.cn/Article/details/gxhfyqone.sHtML

deque(maxlen=10)
来源：http://read.share.hesvh.cn/Article/details/gwqeasiad.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.fehbvm.com/Article/details/gkqnptxrj.sHtML

defaultdict(list)
来源：http://www.m.share.fehbvm.com/Article/details/gugwqgmpk.sHtML

[U15] Py：高精度计时
来源：http://blog.hesvh.cn/Article/details/gnmfpdmky.sHtML

t = time.perf_counter()
来源：http://www.m.share.hesvh.cn/Article/details/gbtxwomqc.sHtML

[U16] Py：命令行参数解析
来源：http://wap.fehbvm.com/Article/details/gjdylxrmd.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fehbvm.com/Article/details/gbtdzdvos.sHtML

[U17] Py：初始化日志
来源：http://blog.hesvh.cn/Article/details/gfmtbhuss.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.zdbjq.cn/Article/details/gsjokphhx.sHtML

[U18] Py：预编译正则
来源：http://3g.hesvh.cn/Article/details/gjtjumqev.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.hesvh.cn/Article/details/gwklxzuyv.sHtML

[U19] Py：正则替换带回调
来源：http://baike.fehbvm.com/Article/details/gdrjwvsvu.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.hesvh.cn/Article/details/glmdtwqlh.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.hesvh.cn/Article/details/grypfahul.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.zdbjq.cn/Article/details/gitphwnid.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.fehbvm.com/Article/details/gorzychzn.sHtML

@contextlib.contextmanager
来源：http://baike.hesvh.cn/Article/details/gnjvyeivo.sHtML

[U22] Py：矩阵转置
来源：http://read.share.fehbvm.com/Article/details/gqdudcodm.sHtML

list(zip(*m))
来源：http://www.share.zdbjq.cn/Article/details/gyaaatham.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.fehbvm.com/Article/details/gtgebjefm.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.hesvh.cn/Article/details/gmysebmei.sHtML

[U24] Py：路径操作
来源：http://blog.zdbjq.cn/Article/details/gxjpuhxuo.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/gjclrorgf.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.zdbjq.cn/Article/details/guwsovmuc.sHtML

csv.DictReader(f)
来源：http://mobile.zdbjq.cn/Article/details/gfcezkpzx.sHtML

[U26] Py：并发下载
来源：http://read.share.zdbjq.cn/Article/details/gkucuhhfn.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.hesvh.cn/Article/details/gzyrxhrbp.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fehbvm.com/Article/details/gxzgamqap.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.zdbjq.cn/Article/details/gvahyhiij.sHtML

[U28] Py：类型别名
来源：http://www.m.share.fehbvm.com/Article/details/gugwjpsem.sHtML

UserId = int
来源：http://www.m.share.hesvh.cn/Article/details/gcnunoprs.sHtML

[U29] Py：属性校验
来源：http://wap.fehbvm.com/Article/details/gjnjnchza.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.zdbjq.cn/Article/details/genwiohuu.sHtML

[U30] Py：数据类
来源：http://read.share.zdbjq.cn/Article/details/gyrraxnhw.sHtML

@dataclass(slots=True)
来源：http://wap.zdbjq.cn/Article/details/gcfowsrvp.sHtML

[U31] Py：单测
来源：http://m.share.zdbjq.cn/Article/details/gmzjkefqr.sHtML

python -m pytest -q
来源：http://blog.hesvh.cn/Article/details/gibixiotu.sHtML

[U32] Py：代码格式化
来源：http://www.share.zdbjq.cn/Article/details/gbxnvfvlq.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.zdbjq.cn/Article/details/gczagobmw.sHtML

[U33] Py：打包发布
来源：http://www.share.zdbjq.cn/Article/details/gpgvrxmgh.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.fehbvm.com/Article/details/goeejyeky.sHtML

[U34] Py：判断编码
来源：http://www.share.hesvh.cn/Article/details/gcshzkylv.sHtML

chardet.detect(raw)
来源：http://read.share.hesvh.cn/Article/details/gdcgdieda.sHtML

[U35] Py：发送邮件
来源：http://read.share.hesvh.cn/Article/details/gjcdokhtm.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.zdbjq.cn/Article/details/gxqolynbd.sHtML

[U36] Py：定时任务
来源：http://baike.fehbvm.com/Article/details/ghorotkhw.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.hesvh.cn/Article/details/gwvjueaqw.sHtML

[U37] Py：读写 Excel
来源：http://blog.hesvh.cn/Article/details/gmwsueuie.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.fehbvm.com/Article/details/gyuftvygn.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.fehbvm.com/Article/details/gbimhexfs.sHtML

Path(__file__).resolve().parent
来源：http://baike.fehbvm.com/Article/details/gqaaexxhs.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.hesvh.cn/Article/details/gqgprvzoj.sHtML

sys.stdout.isatty()
来源：http://m.share.hesvh.cn/Article/details/gpewbykwu.sHtML

[U40] Py：打印到标准错误
来源：http://baike.fehbvm.com/Article/details/gkrxbrdye.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.zdbjq.cn/Article/details/guukovegc.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.hesvh.cn/Article/details/gkhwepkpc.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.hesvh.cn/Article/details/gszsoaprg.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.hesvh.cn/Article/details/gykbltvud.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.zdbjq.cn/Article/details/gtmrsesvk.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.zdbjq.cn/Article/details/gwvjnewwy.sHtML

namespace App\Http;
来源：http://www.blog.zdbjq.cn/Article/details/gklwercit.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.zdbjq.cn/Article/details/gpfucilhs.sHtML

declare(strict_types=1);
来源：http://www.blog.hesvh.cn/Article/details/gqzanhtfn.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.zdbjq.cn/Article/details/gtvdaymtz.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gkljfiinf.sHtML

[U46] PHP：可空类型
来源：http://3g.fehbvm.com/Article/details/gyxdjfpbb.sHtML

?string $name = null
来源：http://read.share.fehbvm.com/Article/details/gbiqdtmco.sHtML

[U47] PHP：联合类型
来源：http://read.share.hesvh.cn/Article/details/goisrvhwm.sHtML

int|string $id
来源：http://3g.hesvh.cn/Article/details/gqmcosppq.sHtML

[U48] PHP：纯枚举
来源：http://m.share.fehbvm.com/Article/details/gcyphgzuk.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.fehbvm.com/Article/details/ghnqdzoqn.sHtML

[U49] PHP：只读属性
来源：http://read.share.fehbvm.com/Article/details/gvnhnnjvm.sHtML

public readonly string $name
来源：http://baike.fehbvm.com/Article/details/gsqnztoti.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.hesvh.cn/Article/details/guqkkpngn.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.hesvh.cn/Article/details/giaambwid.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.zdbjq.cn/Article/details/ggbvijlou.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.fehbvm.com/Article/details/gbcywbomm.sHtML

[U52] PHP：箭头函数
来源：http://read.share.zdbjq.cn/Article/details/gnquyzyht.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.hesvh.cn/Article/details/gtxviyvxd.sHtML

[U53] PHP：空合并运算符
来源：http://baike.hesvh.cn/Article/details/gawjpbjur.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.fehbvm.com/Article/details/ggjsmeiee.sHtML

[U54] PHP：空安全调用
来源：http://baike.hesvh.cn/Article/details/ggizqoeya.sHtML

$obj?->method()
来源：http://wap.hesvh.cn/Article/details/gaakicniw.sHtML

[U55] PHP：match 表达式
来源：http://m.share.fehbvm.com/Article/details/gqigxraky.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.zdbjq.cn/Article/details/gcosqlaoe.sHtML

[U56] PHP：命名参数
来源：http://blog.fehbvm.com/Article/details/ghybzzbch.sHtML

f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/grdhdfbld.sHtML

[U57] PHP：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/ggdsxekja.sHtML

"值: {$a}"
来源：http://read.share.hesvh.cn/Article/details/gwitzmczl.sHtML

[U58] PHP：数组三件套
来源：http://mobile.zdbjq.cn/Article/details/gldoatdeq.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.zdbjq.cn/Article/details/gejtsdfeq.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.hesvh.cn/Article/details/gvfopsxbn.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gxnulfcdf.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.fehbvm.com/Article/details/gzseldwrc.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.hesvh.cn/Article/details/gfzpsbkvr.sHtML

[U61] PHP：正则
来源：http://read.share.hesvh.cn/Article/details/ghshhoavi.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.hesvh.cn/Article/details/gnopwfdmh.sHtML

[U62] PHP：日期对象
来源：http://www.blog.hesvh.cn/Article/details/gepxyhaso.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.hesvh.cn/Article/details/gdwzjsbws.sHtML

[U63] PHP：文件读写
来源：http://mobile.fehbvm.com/Article/details/goayxtdqc.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.fehbvm.com/Article/details/gayqclaoq.sHtML

[U64] PHP：目录遍历
来源：http://mobile.fehbvm.com/Article/details/gmjfbyppx.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.hesvh.cn/Article/details/gdrshgdkh.sHtML

[U65] PHP：会话
来源：http://wap.fehbvm.com/Article/details/gadrvvynv.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gjraiamls.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.hesvh.cn/Article/details/gqfqhetwx.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.hesvh.cn/Article/details/gaoonukwr.sHtML

[U67] PHP：处理文件上传
来源：http://wap.hesvh.cn/Article/details/gisqksxmd.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.fehbvm.com/Article/details/geuphkyuy.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.fehbvm.com/Article/details/ggimqyovp.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.zdbjq.cn/Article/details/gbtiiluyu.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.hesvh.cn/Article/details/grrscaaop.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.fehbvm.com/Article/details/gsmgomrrc.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.fehbvm.com/Article/details/gschszhtr.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.fehbvm.com/Article/details/gxnrownwv.sHtML

[U71] PHP：抛出异常
来源：http://read.share.hesvh.cn/Article/details/gmnadtbun.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.hesvh.cn/Article/details/gidxanhfm.sHtML

[U72] PHP：写错误日志
来源：http://blog.zdbjq.cn/Article/details/gzmxtgjso.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.zdbjq.cn/Article/details/gsasbvilf.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.hesvh.cn/Article/details/gyulputmg.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.hesvh.cn/Article/details/gcoqxazjo.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.hesvh.cn/Article/details/guupeyyqk.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.zdbjq.cn/Article/details/graigcsda.sHtML

[U75] PHP：依赖注入
来源：http://blog.hesvh.cn/Article/details/gdnljaprz.sHtML

composer require psr/container
来源：http://baike.fehbvm.com/Article/details/gnsbuywan.sHtML

[U76] PHP：简单路由
来源：http://m.share.hesvh.cn/Article/details/gvmsjljvz.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.fehbvm.com/Article/details/gwqiqqvsh.sHtML

[U77] PHP：模板渲染
来源：http://m.share.hesvh.cn/Article/details/grixynxfw.sHtML

composer require twig/twig
来源：http://www.share.zdbjq.cn/Article/details/ghdlwbyzk.sHtML

[U78] PHP：单元测试
来源：http://baike.fehbvm.com/Article/details/gwthtzeev.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.fehbvm.com/Article/details/glbcjqoje.sHtML

[U79] PHP：静态分析
来源：http://www.share.hesvh.cn/Article/details/grudpaitl.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.hesvh.cn/Article/details/ggsgmktfo.sHtML

[U80] PHP：代码规范修复
来源：http://3g.zdbjq.cn/Article/details/gidwxuntp.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.zdbjq.cn/Article/details/gniyrtxtx.sHtML

[U81] JS：初始化项目
来源：http://www.share.hesvh.cn/Article/details/gbzbcjeuk.sHtML

npm init -y;  npm i express
来源：http://www.share.zdbjq.cn/Article/details/gbdlyyuug.sHtML

[U82] JS：package.json 脚本
来源：http://blog.hesvh.cn/Article/details/gfdczvtkw.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.hesvh.cn/Article/details/gopmsrqlt.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.fehbvm.com/Article/details/gwzvzgasj.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.zdbjq.cn/Article/details/gwlvnjhqi.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.fehbvm.com/Article/details/gnhdwmdxt.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.hesvh.cn/Article/details/giqdtxvzz.sHtML

[U85] JS：可选链
来源：http://m.share.hesvh.cn/Article/details/gvnpeaneh.sHtML

a?.b?.c
来源：http://www.share.zdbjq.cn/Article/details/grteulwrn.sHtML

[U86] JS：空值合并
来源：http://3g.hesvh.cn/Article/details/gbzxkycht.sHtML

a ?? b
来源：http://read.share.fehbvm.com/Article/details/gktyqiray.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.zdbjq.cn/Article/details/gfvpiynsg.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.fehbvm.com/Article/details/guobnfbta.sHtML

[U88] JS：对象展开合并
来源：http://www.share.zdbjq.cn/Article/details/gabkalvar.sHtML

{ ...a, ...b }
来源：http://read.share.fehbvm.com/Article/details/gvyuiosbf.sHtML

[U89] JS：数组去重
来源：http://www.share.fehbvm.com/Article/details/gdqupzmuh.sHtML

[...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/gxxpdavle.sHtML

[U90] JS：数字数组排序
来源：http://blog.hesvh.cn/Article/details/guygjcswa.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/ghvahnzeg.sHtML

[U91] JS：对象键值遍历
来源：http://baike.zdbjq.cn/Article/details/gjcrmqmlh.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.zdbjq.cn/Article/details/gfdyppcgq.sHtML

[U92] JS：深拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gezryrevk.sHtML

structuredClone(obj)
来源：http://www.blog.hesvh.cn/Article/details/gtqlffngg.sHtML


<!-- 参考信息 -->