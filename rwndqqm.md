代发 wailian999

[T05] Kotlin：when 表达式
来源：http://wap.fehbvm.com/Article/details/garitajnw.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.zdbjq.cn/Article/details/gksrdyeth.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fehbvm.com/Article/details/gglgdnlzg.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.hesvh.cn/Article/details/gwiinhhio.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.hesvh.cn/Article/details/gucnkyxow.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.hesvh.cn/Article/details/gufoetqai.sHtML

[T08] Kotlin：数据类
来源：http://3g.hesvh.cn/Article/details/gruswzrap.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fehbvm.com/Article/details/guulmnwnu.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.hesvh.cn/Article/details/gxezekrft.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.hesvh.cn/Article/details/gqxvoomgo.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fehbvm.com/Article/details/gtocebjfr.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.hesvh.cn/Article/details/gmmxlwdrx.sHtML

[T11] Kotlin：协程
来源：http://baike.zdbjq.cn/Article/details/glodcuvde.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.zdbjq.cn/Article/details/gmramgdme.sHtML

[T12] Kotlin：解构声明
来源：http://wap.hesvh.cn/Article/details/gslebsfja.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fehbvm.com/Article/details/gxsdejpvn.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.zdbjq.cn/Article/details/gwxnxemgi.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.hesvh.cn/Article/details/gprafuiqk.sHtML

[T14] Kotlin：循环
来源：http://blog.hesvh.cn/Article/details/grosktdzd.sHtML

for (i in 1..10) println(i)
来源：http://read.share.hesvh.cn/Article/details/gmrzuklcx.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fehbvm.com/Article/details/gkvlwnoog.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.zdbjq.cn/Article/details/ghephwhtp.sHtML

[T16] Swift：Hello World
来源：http://3g.zdbjq.cn/Article/details/gmcyvpaka.sHtML

print("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gypfezzlt.sHtML

[T17] Swift：变量与常量
来源：http://read.share.hesvh.cn/Article/details/gubqplbil.sHtML

var a = 1;  let b = 2
来源：http://wap.zdbjq.cn/Article/details/gguuhrgxm.sHtML

[T18] Swift：字符串插值
来源：http://wap.fehbvm.com/Article/details/gxykarfoe.sHtML

"值: \(b)"
来源：http://read.share.fehbvm.com/Article/details/ghgrxmnmm.sHtML

[T19] Swift：可选绑定
来源：http://blog.zdbjq.cn/Article/details/gcvhxfuuv.sHtML

if let n = opt { print(n) }
来源：http://wap.fehbvm.com/Article/details/gyjdnrowa.sHtML

[T20] Swift：数组操作
来源：http://blog.hesvh.cn/Article/details/gkpsuaumx.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.zdbjq.cn/Article/details/gofprnspe.sHtML

[T21] Swift：遍历
来源：http://www.m.share.zdbjq.cn/Article/details/glzuwfjaq.sHtML

for x in a { print(x) }
来源：http://www.share.zdbjq.cn/Article/details/gnupxxbka.sHtML

[T22] Swift：字典
来源：http://3g.zdbjq.cn/Article/details/ghukcpsey.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.hesvh.cn/Article/details/gguzoekru.sHtML

[T23] Swift：函数
来源：http://baike.zdbjq.cn/Article/details/gveukqadp.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.zdbjq.cn/Article/details/gffcdrigc.sHtML

[T24] Swift：闭包
来源：http://blog.zdbjq.cn/Article/details/guhvencit.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.hesvh.cn/Article/details/gmwsczrxj.sHtML

[T25] Swift：结构体
来源：http://blog.hesvh.cn/Article/details/giskwntwz.sHtML

struct P { var x: Int }
来源：http://www.blog.zdbjq.cn/Article/details/gfxyvehjv.sHtML

[T26] Swift：类与重写
来源：http://m.share.fehbvm.com/Article/details/gdmkevmjp.sHtML

class A: Base { override func f() {} }
来源：http://baike.hesvh.cn/Article/details/gcxcveynd.sHtML

[T27] Swift：错误处理
来源：http://blog.hesvh.cn/Article/details/glermmrtc.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.fehbvm.com/Article/details/gdzsmevez.sHtML

[T28] Swift：枚举
来源：http://www.blog.hesvh.cn/Article/details/ghexqgfqq.sHtML

enum Color { case red, green }
来源：http://3g.fehbvm.com/Article/details/gjpfovjrk.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.fehbvm.com/Article/details/gejkprojv.sHtML

guard let x = opt else { return }
来源：http://m.share.hesvh.cn/Article/details/gpfktuptd.sHtML

[T30] Swift：协议
来源：http://blog.hesvh.cn/Article/details/gbuqycbfc.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.hesvh.cn/Article/details/grvvxxwbu.sHtML

[T31] Lua：Hello World
来源：http://blog.hesvh.cn/Article/details/gdmmtegve.sHtML

print("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gbhqiqxrp.sHtML

[T32] Lua：局部变量
来源：http://www.share.fehbvm.com/Article/details/godksyddb.sHtML

local a = 1
来源：http://read.share.zdbjq.cn/Article/details/gkjrzdfyd.sHtML

[T33] Lua：表（数组）
来源：http://mobile.fehbvm.com/Article/details/glkfabbmh.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.fehbvm.com/Article/details/gtipyqruu.sHtML

[T34] Lua：遍历表
来源：http://3g.fehbvm.com/Article/details/gvfwbnaqs.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.hesvh.cn/Article/details/gbqtgrxwo.sHtML

[T35] Lua：字典表
来源：http://read.share.zdbjq.cn/Article/details/gwyrkoufi.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.hesvh.cn/Article/details/gawunxfku.sHtML

[T36] Lua：函数
来源：http://www.share.zdbjq.cn/Article/details/gtmuiqhli.sHtML

function add(a, b) return a + b end
来源：http://blog.fehbvm.com/Article/details/gwjwevcjc.sHtML

[T37] Lua：字符串拼接
来源：http://baike.zdbjq.cn/Article/details/gedsysaie.sHtML

"a" .. "b"
来源：http://www.m.share.hesvh.cn/Article/details/glhkvvrku.sHtML

[T38] Lua：条件
来源：http://www.share.hesvh.cn/Article/details/gedosewpg.sHtML

if x > 0 then print("正") end
来源：http://3g.hesvh.cn/Article/details/gvxnvntoa.sHtML

[T39] Lua：模式匹配
来源：http://wap.fehbvm.com/Article/details/gixstguvw.sHtML

string.find(s, "%d+")
来源：http://www.share.fehbvm.com/Article/details/giampepsx.sHtML

[T40] Lua：元表
来源：http://read.share.zdbjq.cn/Article/details/gsjhsqgkf.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.fehbvm.com/Article/details/gdigccdbx.sHtML

[T41] Perl：Hello World
来源：http://baike.hesvh.cn/Article/details/gfaqrvgje.sHtML

print "Hello\n";
来源：http://www.share.zdbjq.cn/Article/details/ghbzrvlvv.sHtML

[T42] Perl：变量类型
来源：http://mobile.zdbjq.cn/Article/details/gmbeporol.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.hesvh.cn/Article/details/gehzmgvsp.sHtML

[T43] Perl：字符串插值
来源：http://wap.fehbvm.com/Article/details/gonbchojf.sHtML

"值: $a"
来源：http://blog.fehbvm.com/Article/details/gyhfzacgr.sHtML

[T44] Perl：条件
来源：http://wap.zdbjq.cn/Article/details/gcxxfueox.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.hesvh.cn/Article/details/gezzwcqta.sHtML

[T45] Perl：数组遍历
来源：http://read.share.zdbjq.cn/Article/details/gsospnuct.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.hesvh.cn/Article/details/ggqtbjxzw.sHtML

[T46] Perl：哈希操作
来源：http://wap.zdbjq.cn/Article/details/gubmcduyo.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.fehbvm.com/Article/details/gfaceptpf.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.zdbjq.cn/Article/details/gelvxkvym.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.zdbjq.cn/Article/details/glylwsiyq.sHtML

[T48] Perl：正则替换
来源：http://wap.hesvh.cn/Article/details/gxuxirumy.sHtML

$s =~ s/old/new/g;
来源：http://mobile.zdbjq.cn/Article/details/gulamoslj.sHtML

[T49] Perl：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gudngutok.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gvmrxmaip.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gllvbhiat.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.fehbvm.com/Article/details/genrexheb.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.fehbvm.com/Article/details/gboedfgml.sHtML

[T51] Scala：Hello World
来源：http://read.share.hesvh.cn/Article/details/gfhehzsvq.sHtML

println("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gqpruqter.sHtML

[T52] Scala：变量
来源：http://wap.fehbvm.com/Article/details/gekvjzlko.sHtML

val a = 1;  var b = 2
来源：http://wap.hesvh.cn/Article/details/gtekxgjea.sHtML

[T53] Scala：字符串插值
来源：http://wap.hesvh.cn/Article/details/gfrwesttt.sHtML

s"值: $b"
来源：http://wap.fehbvm.com/Article/details/goiravezq.sHtML

[T54] Scala：集合映射
来源：http://read.share.fehbvm.com/Article/details/gkszutqhg.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.hesvh.cn/Article/details/gxvxzazzy.sHtML

[T55] Scala：集合过滤
来源：http://blog.zdbjq.cn/Article/details/gjxprmxqj.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.hesvh.cn/Article/details/gvswkfixl.sHtML

[T56] Scala：样例类
来源：http://3g.fehbvm.com/Article/details/gzaaarvrz.sHtML

case class User(name: String, age: Int)
来源：http://www.share.fehbvm.com/Article/details/goozzuirs.sHtML

[T57] Scala：模式匹配
来源：http://baike.fehbvm.com/Article/details/gqkfgpyfb.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.fehbvm.com/Article/details/gpqhmtgew.sHtML

[T58] Scala：函数定义
来源：http://baike.hesvh.cn/Article/details/gpnxzhczi.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.hesvh.cn/Article/details/gsqwoszyf.sHtML

[T59] Scala：循环
来源：http://mobile.zdbjq.cn/Article/details/gboftqmgr.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.zdbjq.cn/Article/details/gsuxdonjq.sHtML

[T60] Scala：折叠
来源：http://blog.fehbvm.com/Article/details/gyuhzanki.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.fehbvm.com/Article/details/gaoxxyqkb.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gguqlngny.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gswfiullz.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gyamdxeca.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.hesvh.cn/Article/details/gfuhmamcu.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.zdbjq.cn/Article/details/gvzxoawus.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.fehbvm.com/Article/details/gdtjgjfjy.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.hesvh.cn/Article/details/gzrxtkqmx.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.fehbvm.com/Article/details/gpqzhlija.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.fehbvm.com/Article/details/gwlzpudod.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.hesvh.cn/Article/details/gznypibfy.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.fehbvm.com/Article/details/gzwxbdcst.sHtML

[U05] Py：列表去重且保序
来源：http://wap.hesvh.cn/Article/details/geofhxyck.sHtML

list(dict.fromkeys(arr))
来源：http://3g.zdbjq.cn/Article/details/godbtfftn.sHtML

[U06] Py：合并两个字典
来源：http://baike.fehbvm.com/Article/details/gydauazqo.sHtML

{**a, **b}
来源：http://www.blog.hesvh.cn/Article/details/gpahofdxv.sHtML

[U07] Py：反转字典键值
来源：http://m.share.hesvh.cn/Article/details/gpheckaev.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.zdbjq.cn/Article/details/gtjmmncwj.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.hesvh.cn/Article/details/gcuskmzhx.sHtML

[y for x in nested for y in x]
来源：http://read.share.hesvh.cn/Article/details/gwfnxjtxt.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.zdbjq.cn/Article/details/gddnmqrcn.sHtML

max(d, key=d.get)
来源：http://wap.fehbvm.com/Article/details/grwuhzeix.sHtML

[U10] Py：按值排序字典
来源：http://wap.hesvh.cn/Article/details/gfwuakjrk.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.zdbjq.cn/Article/details/grxbqdrek.sHtML

[U11] Py：生成器表达式
来源：http://mobile.fehbvm.com/Article/details/gmjrvulyt.sHtML

(x * 2 for x in arr)
来源：http://m.share.fehbvm.com/Article/details/globihgni.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.hesvh.cn/Article/details/gotjhvlhe.sHtML

Counter(arr).most_common(3)
来源：http://m.share.zdbjq.cn/Article/details/gpuavyzku.sHtML

[U13] Py：固定长度队列
来源：http://wap.zdbjq.cn/Article/details/gcpqskmsp.sHtML

deque(maxlen=10)
来源：http://m.share.hesvh.cn/Article/details/gmuveaofn.sHtML

[U14] Py：分组收集到列表
来源：http://blog.hesvh.cn/Article/details/gcnxlvdjb.sHtML

defaultdict(list)
来源：http://3g.fehbvm.com/Article/details/gfibemdda.sHtML

[U15] Py：高精度计时
来源：http://baike.zdbjq.cn/Article/details/gcrsrxpog.sHtML

t = time.perf_counter()
来源：http://read.share.fehbvm.com/Article/details/gyrzuijfk.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.fehbvm.com/Article/details/gsxeunilr.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.hesvh.cn/Article/details/glxuuqtwu.sHtML

[U17] Py：初始化日志
来源：http://wap.fehbvm.com/Article/details/gttdhctnl.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.fehbvm.com/Article/details/gluqipjro.sHtML

[U18] Py：预编译正则
来源：http://3g.fehbvm.com/Article/details/gaknwnlft.sHtML

pat = re.compile(r"\d+")
来源：http://3g.zdbjq.cn/Article/details/gguqwrqvm.sHtML

[U19] Py：正则替换带回调
来源：http://baike.zdbjq.cn/Article/details/gogukxtgp.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.hesvh.cn/Article/details/gwzruwssk.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.zdbjq.cn/Article/details/gvnzdfzho.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.hesvh.cn/Article/details/glvvxvfqi.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.hesvh.cn/Article/details/gzrksuzjz.sHtML

@contextlib.contextmanager
来源：http://blog.fehbvm.com/Article/details/gxqoeslde.sHtML

[U22] Py：矩阵转置
来源：http://read.share.fehbvm.com/Article/details/gnuvbzyej.sHtML

list(zip(*m))
来源：http://read.share.fehbvm.com/Article/details/gxyesfrgi.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.hesvh.cn/Article/details/gotmfpvft.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.hesvh.cn/Article/details/gprpljaec.sHtML

[U24] Py：路径操作
来源：http://blog.hesvh.cn/Article/details/gvjkbghdw.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.fehbvm.com/Article/details/gfozrvnsz.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.zdbjq.cn/Article/details/gzlkmwper.sHtML

csv.DictReader(f)
来源：http://mobile.hesvh.cn/Article/details/gfhwsjqxf.sHtML

[U26] Py：并发下载
来源：http://wap.hesvh.cn/Article/details/gxbgolmyt.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.hesvh.cn/Article/details/glppivqsh.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.hesvh.cn/Article/details/gvvuxeezk.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.hesvh.cn/Article/details/gtefahmcq.sHtML

[U28] Py：类型别名
来源：http://www.share.zdbjq.cn/Article/details/gmlkrqvlb.sHtML

UserId = int
来源：http://mobile.zdbjq.cn/Article/details/givtzvnzd.sHtML

[U29] Py：属性校验
来源：http://read.share.zdbjq.cn/Article/details/gplxjoqri.sHtML

@property 与 @x.setter 配合
来源：http://wap.zdbjq.cn/Article/details/gtdpbxocg.sHtML

[U30] Py：数据类
来源：http://baike.zdbjq.cn/Article/details/gibmijbhf.sHtML

@dataclass(slots=True)
来源：http://baike.zdbjq.cn/Article/details/giupysgag.sHtML

[U31] Py：单测
来源：http://www.share.hesvh.cn/Article/details/gxwmrmvia.sHtML

python -m pytest -q
来源：http://www.blog.fehbvm.com/Article/details/gyurxpknk.sHtML

[U32] Py：代码格式化
来源：http://m.share.zdbjq.cn/Article/details/gadanldef.sHtML

ruff format . && ruff check --fix .
来源：http://blog.zdbjq.cn/Article/details/gyypqzaql.sHtML

[U33] Py：打包发布
来源：http://wap.zdbjq.cn/Article/details/genmcqdfy.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.fehbvm.com/Article/details/gbqevxlji.sHtML

[U34] Py：判断编码
来源：http://www.share.fehbvm.com/Article/details/gejaevpff.sHtML

chardet.detect(raw)
来源：http://www.share.hesvh.cn/Article/details/gzsdttlvf.sHtML

[U35] Py：发送邮件
来源：http://www.share.hesvh.cn/Article/details/gkccxnaos.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.hesvh.cn/Article/details/gthniltdn.sHtML

[U36] Py：定时任务
来源：http://m.share.hesvh.cn/Article/details/grdldpgnr.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.zdbjq.cn/Article/details/gcljlxnmg.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.zdbjq.cn/Article/details/gkyzaxwmo.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.zdbjq.cn/Article/details/gdvowttdc.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.fehbvm.com/Article/details/gyungwxcq.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.fehbvm.com/Article/details/gkubknvbq.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.fehbvm.com/Article/details/gcvxyyqdp.sHtML

sys.stdout.isatty()
来源：http://baike.hesvh.cn/Article/details/gtybhgzmk.sHtML

[U40] Py：打印到标准错误
来源：http://3g.fehbvm.com/Article/details/gupmkrxzm.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.zdbjq.cn/Article/details/gmcpwzqwr.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.zdbjq.cn/Article/details/grojiigyc.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.hesvh.cn/Article/details/gbzcujfjy.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.zdbjq.cn/Article/details/gfhifmxut.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.fehbvm.com/Article/details/gadjesrey.sHtML

[U43] PHP：声明命名空间
来源：http://baike.hesvh.cn/Article/details/gfqguqhjp.sHtML

namespace App\Http;
来源：http://www.blog.hesvh.cn/Article/details/gpsiycdut.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.zdbjq.cn/Article/details/gdwsxsgtx.sHtML

declare(strict_types=1);
来源：http://www.share.fehbvm.com/Article/details/gfmxnxqvb.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.hesvh.cn/Article/details/gamktkqya.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gkobompyz.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.fehbvm.com/Article/details/gqpeesanp.sHtML

?string $name = null
来源：http://3g.fehbvm.com/Article/details/gxrgaiakk.sHtML

[U47] PHP：联合类型
来源：http://wap.fehbvm.com/Article/details/gbaesfpli.sHtML

int|string $id
来源：http://read.share.fehbvm.com/Article/details/gblpihhsw.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.fehbvm.com/Article/details/gdtzuviwn.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.zdbjq.cn/Article/details/gblyoqlsl.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.zdbjq.cn/Article/details/gxvvoowjk.sHtML

public readonly string $name
来源：http://www.m.share.zdbjq.cn/Article/details/gwbyefgqt.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.zdbjq.cn/Article/details/gohakxcny.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gydytvywv.sHtML

[U51] PHP：数组解构
来源：http://blog.fehbvm.com/Article/details/gguqyvamp.sHtML

[$a, $b] = $arr;
来源：http://blog.hesvh.cn/Article/details/gghqfnjyx.sHtML

[U52] PHP：箭头函数
来源：http://m.share.fehbvm.com/Article/details/gwrqfjxol.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.zdbjq.cn/Article/details/gmsiralox.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.hesvh.cn/Article/details/gfvuitnpg.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.hesvh.cn/Article/details/gotqamkjt.sHtML

[U54] PHP：空安全调用
来源：http://baike.fehbvm.com/Article/details/gkilsrndp.sHtML

$obj?->method()
来源：http://wap.zdbjq.cn/Article/details/gomnntfub.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.hesvh.cn/Article/details/gpskgmevd.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.fehbvm.com/Article/details/gcdbzsvza.sHtML

[U56] PHP：命名参数
来源：http://mobile.hesvh.cn/Article/details/gkqvcujrl.sHtML

f(a: 1, b: 2)
来源：http://mobile.hesvh.cn/Article/details/gxyqffhun.sHtML

[U57] PHP：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gixuraykt.sHtML

"值: {$a}"
来源：http://m.share.fehbvm.com/Article/details/gnnbqzzkq.sHtML

[U58] PHP：数组三件套
来源：http://wap.zdbjq.cn/Article/details/gslheaysj.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gwxsflyjh.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.zdbjq.cn/Article/details/gacqmgjxk.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.zdbjq.cn/Article/details/gmffesejm.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.fehbvm.com/Article/details/guehwgjqu.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.hesvh.cn/Article/details/gixitcdqj.sHtML

[U61] PHP：正则
来源：http://wap.hesvh.cn/Article/details/guozyyyoy.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.zdbjq.cn/Article/details/glbfyuxkw.sHtML

[U62] PHP：日期对象
来源：http://wap.hesvh.cn/Article/details/gjdfsspaq.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.fehbvm.com/Article/details/gnkrsckju.sHtML

[U63] PHP：文件读写
来源：http://mobile.zdbjq.cn/Article/details/ggoboysvs.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.zdbjq.cn/Article/details/gyfgutivp.sHtML

[U64] PHP：目录遍历
来源：http://mobile.zdbjq.cn/Article/details/gidknvbel.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.hesvh.cn/Article/details/gmrcptvrr.sHtML

[U65] PHP：会话
来源：http://blog.zdbjq.cn/Article/details/gwopbpmus.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gqinqcsft.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.fehbvm.com/Article/details/gljrggecj.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.fehbvm.com/Article/details/grymeazrj.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.zdbjq.cn/Article/details/gdtkzktxm.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.hesvh.cn/Article/details/gcqfpnhdh.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.zdbjq.cn/Article/details/glredturj.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.zdbjq.cn/Article/details/gapnusxbc.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.fehbvm.com/Article/details/gnrqyquky.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.zdbjq.cn/Article/details/gfaqugyeg.sHtML

[U70] PHP：PDO 事务
来源：http://baike.zdbjq.cn/Article/details/gskphkmrq.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.zdbjq.cn/Article/details/gmcbqaocl.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.fehbvm.com/Article/details/gofpkpmvo.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.zdbjq.cn/Article/details/gzvplakwy.sHtML

[U72] PHP：写错误日志
来源：http://www.share.hesvh.cn/Article/details/gfovyocuj.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.zdbjq.cn/Article/details/gknpvqhrr.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.fehbvm.com/Article/details/gcjthlhtr.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.zdbjq.cn/Article/details/gfahswyep.sHtML

[U74] PHP：读取环境变量
来源：http://wap.zdbjq.cn/Article/details/gsfulgvdq.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.hesvh.cn/Article/details/gnwertoji.sHtML

[U75] PHP：依赖注入
来源：http://wap.fehbvm.com/Article/details/ghxyybdie.sHtML

composer require psr/container
来源：http://baike.zdbjq.cn/Article/details/gifigyclw.sHtML

[U76] PHP：简单路由
来源：http://m.share.zdbjq.cn/Article/details/ggnjbaaou.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.hesvh.cn/Article/details/ggenuqjbp.sHtML

[U77] PHP：模板渲染
来源：http://read.share.fehbvm.com/Article/details/gbqrrcvqk.sHtML

composer require twig/twig
来源：http://wap.zdbjq.cn/Article/details/gculcpajk.sHtML

[U78] PHP：单元测试
来源：http://3g.fehbvm.com/Article/details/gadeoldpz.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.fehbvm.com/Article/details/grxhfqykp.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.fehbvm.com/Article/details/glrzehuem.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.zdbjq.cn/Article/details/gxewgdazn.sHtML

[U80] PHP：代码规范修复
来源：http://3g.fehbvm.com/Article/details/gceogzsnk.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.zdbjq.cn/Article/details/geitwavob.sHtML

[U81] JS：初始化项目
来源：http://blog.fehbvm.com/Article/details/gbrxncvvr.sHtML

npm init -y;  npm i express
来源：http://www.blog.fehbvm.com/Article/details/gpvegmckf.sHtML

[U82] JS：package.json 脚本
来源：http://baike.hesvh.cn/Article/details/glmnowgxu.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.zdbjq.cn/Article/details/gilkznxro.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.zdbjq.cn/Article/details/gigdqkwfq.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.zdbjq.cn/Article/details/gkumlftyt.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.fehbvm.com/Article/details/gfbbrpahk.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.hesvh.cn/Article/details/gbtcvvgqd.sHtML

[U85] JS：可选链
来源：http://mobile.zdbjq.cn/Article/details/gprtczfcm.sHtML

a?.b?.c
来源：http://www.m.share.zdbjq.cn/Article/details/gvgjizgak.sHtML

[U86] JS：空值合并
来源：http://wap.zdbjq.cn/Article/details/gnsvcxrpf.sHtML

a ?? b
来源：http://www.m.share.hesvh.cn/Article/details/gcjuhmypl.sHtML

[U87] JS：解构默认值
来源：http://blog.zdbjq.cn/Article/details/gkidnnimg.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.fehbvm.com/Article/details/gyzinkfkj.sHtML

[U88] JS：对象展开合并
来源：http://mobile.fehbvm.com/Article/details/ghysnrimc.sHtML

{ ...a, ...b }
来源：http://read.share.zdbjq.cn/Article/details/ginwaxlzf.sHtML

[U89] JS：数组去重
来源：http://m.share.hesvh.cn/Article/details/gwozzmwxu.sHtML

[...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/glyfvmbdf.sHtML

[U90] JS：数字数组排序
来源：http://wap.hesvh.cn/Article/details/gdtqyipsr.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gjuuzbisg.sHtML

[U91] JS：对象键值遍历
来源：http://3g.fehbvm.com/Article/details/gtmshrldn.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.fehbvm.com/Article/details/gogcghaqm.sHtML

[U92] JS：深拷贝
来源：http://baike.fehbvm.com/Article/details/ghofresnn.sHtML

structuredClone(obj)
来源：http://www.share.zdbjq.cn/Article/details/gzqxayqan.sHtML


<!-- 参考信息 -->