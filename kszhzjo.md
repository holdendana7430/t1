代发 wailian999

[T05] Kotlin：when 表达式
来源：http://mobile.fehbvm.com/Article/details/glgzmsjiw.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.zdbjq.cn/Article/details/gcxaxjrsx.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fehbvm.com/Article/details/gkxkitnti.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fehbvm.com/Article/details/gjtfdebva.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fehbvm.com/Article/details/gnxslqgvx.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.zdbjq.cn/Article/details/gmwdnvsiv.sHtML

[T08] Kotlin：数据类
来源：http://baike.hesvh.cn/Article/details/gxxghnvxg.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.hesvh.cn/Article/details/gguwndxlb.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fehbvm.com/Article/details/gbbhytftw.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fehbvm.com/Article/details/gscnvkkvo.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.zdbjq.cn/Article/details/gjnoptrqo.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fehbvm.com/Article/details/giszshtee.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.hesvh.cn/Article/details/guzadrhqz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.hesvh.cn/Article/details/gazicsyzg.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fehbvm.com/Article/details/gsaudbrdo.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gqnskqmcm.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fehbvm.com/Article/details/gffcucddo.sHtML

val m = mapOf("a" to 1)
来源：http://blog.hesvh.cn/Article/details/ghhkfdglw.sHtML

[T14] Kotlin：循环
来源：http://baike.zdbjq.cn/Article/details/gquqfdhmp.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fehbvm.com/Article/details/gtnlzlhaj.sHtML

[T15] Kotlin：接口
来源：http://3g.fehbvm.com/Article/details/gremhljaf.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fehbvm.com/Article/details/gbyhvjbcv.sHtML

[T16] Swift：Hello World
来源：http://wap.hesvh.cn/Article/details/gyovzoviv.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/grhsmjbqe.sHtML

[T17] Swift：变量与常量
来源：http://blog.fehbvm.com/Article/details/gglrvidau.sHtML

var a = 1;  let b = 2
来源：http://www.share.zdbjq.cn/Article/details/glmpanwxw.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gcoichcox.sHtML

"值: \(b)"
来源：http://blog.zdbjq.cn/Article/details/gbngfxfog.sHtML

[T19] Swift：可选绑定
来源：http://baike.fehbvm.com/Article/details/gwnzfcmaz.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.zdbjq.cn/Article/details/gxhbqtwdj.sHtML

[T20] Swift：数组操作
来源：http://mobile.fehbvm.com/Article/details/ggnzxutua.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fehbvm.com/Article/details/gdyhsejxu.sHtML

[T21] Swift：遍历
来源：http://www.m.share.hesvh.cn/Article/details/gynxqpgpd.sHtML

for x in a { print(x) }
来源：http://www.share.hesvh.cn/Article/details/gnemeqzeh.sHtML

[T22] Swift：字典
来源：http://m.share.fehbvm.com/Article/details/gyinstdvl.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fehbvm.com/Article/details/gdkndjoke.sHtML

[T23] Swift：函数
来源：http://www.m.share.fehbvm.com/Article/details/grcljjubk.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fehbvm.com/Article/details/gcfpnqdsb.sHtML

[T24] Swift：闭包
来源：http://baike.hesvh.cn/Article/details/gjvdtuyfl.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gbzqtdlzi.sHtML

[T25] Swift：结构体
来源：http://m.share.fehbvm.com/Article/details/gldlddrgh.sHtML

struct P { var x: Int }
来源：http://read.share.fehbvm.com/Article/details/giperkpad.sHtML

[T26] Swift：类与重写
来源：http://3g.fehbvm.com/Article/details/gzdbhutei.sHtML

class A: Base { override func f() {} }
来源：http://3g.zdbjq.cn/Article/details/gcvwvklpr.sHtML

[T27] Swift：错误处理
来源：http://baike.hesvh.cn/Article/details/gujbwtsoe.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.hesvh.cn/Article/details/gxmdnionl.sHtML

[T28] Swift：枚举
来源：http://wap.hesvh.cn/Article/details/goyljbtqh.sHtML

enum Color { case red, green }
来源：http://3g.fehbvm.com/Article/details/gkjwphktx.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.zdbjq.cn/Article/details/gcmtulukx.sHtML

guard let x = opt else { return }
来源：http://m.share.fehbvm.com/Article/details/gtzbppfvq.sHtML

[T30] Swift：协议
来源：http://blog.hesvh.cn/Article/details/gwcqqwmxa.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.hesvh.cn/Article/details/gjdcwfqze.sHtML

[T31] Lua：Hello World
来源：http://3g.zdbjq.cn/Article/details/gmttztlbn.sHtML

print("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gauoollyr.sHtML

[T32] Lua：局部变量
来源：http://blog.zdbjq.cn/Article/details/gntorjuze.sHtML

local a = 1
来源：http://wap.hesvh.cn/Article/details/gmfxdcmol.sHtML

[T33] Lua：表（数组）
来源：http://m.share.fehbvm.com/Article/details/gqgssbthy.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.hesvh.cn/Article/details/greknzgsd.sHtML

[T34] Lua：遍历表
来源：http://read.share.hesvh.cn/Article/details/gpjzjbjqy.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.zdbjq.cn/Article/details/ghjiigrlj.sHtML

[T35] Lua：字典表
来源：http://baike.zdbjq.cn/Article/details/gxpkswhvc.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.fehbvm.com/Article/details/gxvfilrol.sHtML

[T36] Lua：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gufqhnbvy.sHtML

function add(a, b) return a + b end
来源：http://read.share.zdbjq.cn/Article/details/gbwdpfvdd.sHtML

[T37] Lua：字符串拼接
来源：http://wap.hesvh.cn/Article/details/guetzjuas.sHtML

"a" .. "b"
来源：http://read.share.fehbvm.com/Article/details/gtdvyvzwy.sHtML

[T38] Lua：条件
来源：http://www.m.share.fehbvm.com/Article/details/grfplouel.sHtML

if x > 0 then print("正") end
来源：http://wap.hesvh.cn/Article/details/gcldoplom.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.zdbjq.cn/Article/details/gdznimske.sHtML

string.find(s, "%d+")
来源：http://www.share.hesvh.cn/Article/details/gxihzoubp.sHtML

[T40] Lua：元表
来源：http://3g.hesvh.cn/Article/details/gqharhcgq.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.hesvh.cn/Article/details/gdddjstlz.sHtML

[T41] Perl：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gczlkggrj.sHtML

print "Hello\n";
来源：http://3g.fehbvm.com/Article/details/ggflabiol.sHtML

[T42] Perl：变量类型
来源：http://www.blog.hesvh.cn/Article/details/gpywmdriw.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.fehbvm.com/Article/details/gdazugtby.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/griqkxhdy.sHtML

"值: $a"
来源：http://www.m.share.fehbvm.com/Article/details/gccxjmrgj.sHtML

[T44] Perl：条件
来源：http://www.m.share.zdbjq.cn/Article/details/gwutmhsts.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.hesvh.cn/Article/details/gdzgwkesm.sHtML

[T45] Perl：数组遍历
来源：http://wap.hesvh.cn/Article/details/gzhjkjkaw.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.zdbjq.cn/Article/details/gbvfvfaos.sHtML

[T46] Perl：哈希操作
来源：http://mobile.fehbvm.com/Article/details/grrhpfbet.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.fehbvm.com/Article/details/gxyjmysqe.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.zdbjq.cn/Article/details/gqreondca.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.hesvh.cn/Article/details/ggnqnzzuc.sHtML

[T48] Perl：正则替换
来源：http://wap.fehbvm.com/Article/details/gsshwtidd.sHtML

$s =~ s/old/new/g;
来源：http://baike.zdbjq.cn/Article/details/gjirgkalv.sHtML

[T49] Perl：函数
来源：http://www.blog.hesvh.cn/Article/details/gqpskllyw.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gsqhwalcs.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/grypdroiv.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.fehbvm.com/Article/details/gzwogxull.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.hesvh.cn/Article/details/gignwckiy.sHtML

[T51] Scala：Hello World
来源：http://wap.fehbvm.com/Article/details/gjpvvtspo.sHtML

println("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gogavzndh.sHtML

[T52] Scala：变量
来源：http://www.m.share.zdbjq.cn/Article/details/gmfwdciqt.sHtML

val a = 1;  var b = 2
来源：http://mobile.hesvh.cn/Article/details/giwycrirj.sHtML

[T53] Scala：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gapkwuomi.sHtML

s"值: $b"
来源：http://wap.zdbjq.cn/Article/details/gxddhsgcj.sHtML

[T54] Scala：集合映射
来源：http://wap.fehbvm.com/Article/details/galrppqew.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.zdbjq.cn/Article/details/gbnsfwfoj.sHtML

[T55] Scala：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/gyjzqonnh.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.hesvh.cn/Article/details/glwvouikz.sHtML

[T56] Scala：样例类
来源：http://m.share.zdbjq.cn/Article/details/gmqnbeuqz.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.hesvh.cn/Article/details/gswlezhva.sHtML

[T57] Scala：模式匹配
来源：http://www.share.zdbjq.cn/Article/details/gnxtruqpr.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.hesvh.cn/Article/details/gjmalzeds.sHtML

[T58] Scala：函数定义
来源：http://wap.zdbjq.cn/Article/details/gpvdgsghi.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.zdbjq.cn/Article/details/gpfxlihxv.sHtML

[T59] Scala：循环
来源：http://wap.hesvh.cn/Article/details/gpmbmxnzi.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fehbvm.com/Article/details/gkdydehto.sHtML

[T60] Scala：折叠
来源：http://blog.zdbjq.cn/Article/details/gejpnjdjd.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.zdbjq.cn/Article/details/gqbrzsccv.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gxldyznqd.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fehbvm.com/Article/details/gcagyltzq.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gpaipynqc.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.zdbjq.cn/Article/details/gkvwpqgng.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.fehbvm.com/Article/details/glfafvfws.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.hesvh.cn/Article/details/gtlxvfnae.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.fehbvm.com/Article/details/ghyfproid.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.fehbvm.com/Article/details/gcupvujdj.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.hesvh.cn/Article/details/gocidhlry.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.hesvh.cn/Article/details/gmgffflqa.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fehbvm.com/Article/details/ggdvriyxi.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.fehbvm.com/Article/details/grezbltvr.sHtML

list(dict.fromkeys(arr))
来源：http://3g.fehbvm.com/Article/details/ggujsarsn.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fehbvm.com/Article/details/ghugstowx.sHtML

{**a, **b}
来源：http://wap.zdbjq.cn/Article/details/gkwwkmesd.sHtML

[U07] Py：反转字典键值
来源：http://read.share.zdbjq.cn/Article/details/geswqnrlj.sHtML

{v: k for k, v in d.items()}
来源：http://baike.hesvh.cn/Article/details/gdlesfylp.sHtML

[U08] Py：展平二维列表
来源：http://mobile.fehbvm.com/Article/details/gkuvwxuqv.sHtML

[y for x in nested for y in x]
来源：http://www.blog.fehbvm.com/Article/details/gmnaqwbyv.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.hesvh.cn/Article/details/gjhauoukp.sHtML

max(d, key=d.get)
来源：http://read.share.zdbjq.cn/Article/details/gjmsrdpnc.sHtML

[U10] Py：按值排序字典
来源：http://read.share.hesvh.cn/Article/details/gpfwigytg.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.fehbvm.com/Article/details/gywsgwucm.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gjpmnvays.sHtML

(x * 2 for x in arr)
来源：http://blog.zdbjq.cn/Article/details/gphwnxvap.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.hesvh.cn/Article/details/gujtnyixy.sHtML

Counter(arr).most_common(3)
来源：http://baike.zdbjq.cn/Article/details/gpcrswqhm.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.fehbvm.com/Article/details/gxtrlwkwj.sHtML

deque(maxlen=10)
来源：http://www.blog.fehbvm.com/Article/details/gxjgzymuz.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.zdbjq.cn/Article/details/gpxpfqchr.sHtML

defaultdict(list)
来源：http://baike.zdbjq.cn/Article/details/gxjrmqnbm.sHtML

[U15] Py：高精度计时
来源：http://m.share.zdbjq.cn/Article/details/glclpevkt.sHtML

t = time.perf_counter()
来源：http://www.share.fehbvm.com/Article/details/gazqulkvp.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.zdbjq.cn/Article/details/gtiyfepwy.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.zdbjq.cn/Article/details/gznbjjqth.sHtML

[U17] Py：初始化日志
来源：http://read.share.fehbvm.com/Article/details/gkoalzifj.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.hesvh.cn/Article/details/gpdxbgbet.sHtML

[U18] Py：预编译正则
来源：http://www.share.zdbjq.cn/Article/details/glxugrfkp.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.zdbjq.cn/Article/details/gzerlmrlb.sHtML

[U19] Py：正则替换带回调
来源：http://baike.fehbvm.com/Article/details/gkpopyhyx.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.hesvh.cn/Article/details/gngashpjb.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.fehbvm.com/Article/details/gftoxdhkc.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.fehbvm.com/Article/details/gnbywliah.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.zdbjq.cn/Article/details/gbjlglgpj.sHtML

@contextlib.contextmanager
来源：http://www.share.zdbjq.cn/Article/details/ggkosqrml.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.fehbvm.com/Article/details/gtqhkgzyt.sHtML

list(zip(*m))
来源：http://www.share.zdbjq.cn/Article/details/grhhhfwcj.sHtML

[U23] Py：分块读取大文件
来源：http://blog.fehbvm.com/Article/details/ggglhyzrz.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.hesvh.cn/Article/details/gzvftvhvl.sHtML

[U24] Py：路径操作
来源：http://m.share.hesvh.cn/Article/details/grhqcfcaq.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.hesvh.cn/Article/details/ggbeujyty.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.hesvh.cn/Article/details/gaxegfccf.sHtML

csv.DictReader(f)
来源：http://read.share.fehbvm.com/Article/details/gbwacuxio.sHtML

[U26] Py：并发下载
来源：http://wap.zdbjq.cn/Article/details/gekrrglhi.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.fehbvm.com/Article/details/ghdiquhkm.sHtML

[U27] Py：异步 HTTP
来源：http://wap.fehbvm.com/Article/details/gdvzhfnsq.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.fehbvm.com/Article/details/gnelolwih.sHtML

[U28] Py：类型别名
来源：http://www.share.fehbvm.com/Article/details/gslruspxf.sHtML

UserId = int
来源：http://www.blog.fehbvm.com/Article/details/gaoyktbym.sHtML

[U29] Py：属性校验
来源：http://3g.hesvh.cn/Article/details/gxvxvzswt.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.zdbjq.cn/Article/details/gtmdbheso.sHtML

[U30] Py：数据类
来源：http://3g.hesvh.cn/Article/details/girgwcaxd.sHtML

@dataclass(slots=True)
来源：http://www.share.hesvh.cn/Article/details/goqpgvwbu.sHtML

[U31] Py：单测
来源：http://wap.zdbjq.cn/Article/details/gzcsuwsrd.sHtML

python -m pytest -q
来源：http://www.m.share.hesvh.cn/Article/details/geaoqfupo.sHtML

[U32] Py：代码格式化
来源：http://blog.fehbvm.com/Article/details/gjooerveh.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.fehbvm.com/Article/details/ggoyxlikr.sHtML

[U33] Py：打包发布
来源：http://www.share.fehbvm.com/Article/details/gwlubahmu.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.fehbvm.com/Article/details/gspnqxjgx.sHtML

[U34] Py：判断编码
来源：http://read.share.zdbjq.cn/Article/details/gmrwyosls.sHtML

chardet.detect(raw)
来源：http://baike.fehbvm.com/Article/details/guxqvsmpp.sHtML

[U35] Py：发送邮件
来源：http://read.share.hesvh.cn/Article/details/gjqzdgvvx.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.fehbvm.com/Article/details/gywfslhxh.sHtML

[U36] Py：定时任务
来源：http://mobile.fehbvm.com/Article/details/gcxleszsz.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.fehbvm.com/Article/details/gzqyryvfp.sHtML

[U37] Py：读写 Excel
来源：http://baike.zdbjq.cn/Article/details/gkfczphdn.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.hesvh.cn/Article/details/gztfxbxbj.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.hesvh.cn/Article/details/gjdiotdun.sHtML

Path(__file__).resolve().parent
来源：http://m.share.zdbjq.cn/Article/details/ggqvimxfr.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.zdbjq.cn/Article/details/gnwytjaow.sHtML

sys.stdout.isatty()
来源：http://www.share.hesvh.cn/Article/details/gwkdriysd.sHtML

[U40] Py：打印到标准错误
来源：http://blog.hesvh.cn/Article/details/gfcoiitce.sHtML

print("err", file=sys.stderr)
来源：http://wap.fehbvm.com/Article/details/goglgbpbs.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.zdbjq.cn/Article/details/gogbyuiaj.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.zdbjq.cn/Article/details/gckoxvacn.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.zdbjq.cn/Article/details/gmqfyuwdd.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.hesvh.cn/Article/details/grnioduza.sHtML

[U43] PHP：声明命名空间
来源：http://baike.hesvh.cn/Article/details/gbqnjrsqu.sHtML

namespace App\Http;
来源：http://www.blog.zdbjq.cn/Article/details/gplsyweer.sHtML

[U44] PHP：开启严格类型
来源：http://wap.hesvh.cn/Article/details/gghomdpxb.sHtML

declare(strict_types=1);
来源：http://m.share.zdbjq.cn/Article/details/gzkoxsokw.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.zdbjq.cn/Article/details/gljymbktv.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/grcahucud.sHtML

[U46] PHP：可空类型
来源：http://baike.hesvh.cn/Article/details/gcenxsrwy.sHtML

?string $name = null
来源：http://3g.fehbvm.com/Article/details/gjwmxnivx.sHtML

[U47] PHP：联合类型
来源：http://blog.zdbjq.cn/Article/details/ghcsncqhh.sHtML

int|string $id
来源：http://wap.hesvh.cn/Article/details/gjflvlcgk.sHtML

[U48] PHP：纯枚举
来源：http://read.share.fehbvm.com/Article/details/gsxyucmfj.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.hesvh.cn/Article/details/gslklwulm.sHtML

[U49] PHP：只读属性
来源：http://blog.zdbjq.cn/Article/details/gzrrjtlkj.sHtML

public readonly string $name
来源：http://3g.fehbvm.com/Article/details/gpqmgcbvz.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.zdbjq.cn/Article/details/gnayrbhat.sHtML

public function __construct(private int $id) {}
来源：http://read.share.zdbjq.cn/Article/details/ggwiybeqv.sHtML

[U51] PHP：数组解构
来源：http://wap.zdbjq.cn/Article/details/gvosjegph.sHtML

[$a, $b] = $arr;
来源：http://mobile.hesvh.cn/Article/details/gjtmpbnei.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.hesvh.cn/Article/details/gvoiafudn.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.hesvh.cn/Article/details/giiflmgrl.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.hesvh.cn/Article/details/gbosemmop.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.zdbjq.cn/Article/details/gvozggsjh.sHtML

[U54] PHP：空安全调用
来源：http://baike.fehbvm.com/Article/details/gytrdkzmd.sHtML

$obj?->method()
来源：http://wap.zdbjq.cn/Article/details/gllvjoqmt.sHtML

[U55] PHP：match 表达式
来源：http://wap.zdbjq.cn/Article/details/gkdofrodo.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.hesvh.cn/Article/details/gxsrsulqr.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.fehbvm.com/Article/details/gwbznbwzt.sHtML

f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/gmlibyjvl.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gbbvvvzjz.sHtML

"值: {$a}"
来源：http://www.blog.zdbjq.cn/Article/details/gjobwgdyv.sHtML

[U58] PHP：数组三件套
来源：http://mobile.fehbvm.com/Article/details/gcloliybc.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.fehbvm.com/Article/details/gknbawzzf.sHtML

[U59] PHP：自定义排序
来源：http://baike.fehbvm.com/Article/details/gituokwmr.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.zdbjq.cn/Article/details/gfaltkxaw.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.fehbvm.com/Article/details/ghqomqeow.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.hesvh.cn/Article/details/gkkooagvy.sHtML

[U61] PHP：正则
来源：http://baike.fehbvm.com/Article/details/gdtexufsb.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.hesvh.cn/Article/details/gbcvqkavp.sHtML

[U62] PHP：日期对象
来源：http://www.share.hesvh.cn/Article/details/gwbpimjiw.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.zdbjq.cn/Article/details/gdvswqdor.sHtML

[U63] PHP：文件读写
来源：http://blog.zdbjq.cn/Article/details/gpbxdagnz.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.fehbvm.com/Article/details/gslnjbsnr.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gadkwzqaj.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.hesvh.cn/Article/details/gckuuaxbh.sHtML

[U65] PHP：会话
来源：http://www.share.hesvh.cn/Article/details/geuxocmpq.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gkmhvzbrw.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.hesvh.cn/Article/details/gejclrgdd.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.hesvh.cn/Article/details/ggvhucsuf.sHtML

[U67] PHP：处理文件上传
来源：http://baike.zdbjq.cn/Article/details/glsiiflgh.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.fehbvm.com/Article/details/gqultwtyi.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.hesvh.cn/Article/details/gprjeyxmb.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.fehbvm.com/Article/details/gvetfhzrl.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.hesvh.cn/Article/details/gbbkdojin.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.fehbvm.com/Article/details/gxdxbegaw.sHtML

[U70] PHP：PDO 事务
来源：http://wap.zdbjq.cn/Article/details/gijaokwwb.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.zdbjq.cn/Article/details/gjlxtcnme.sHtML

[U71] PHP：抛出异常
来源：http://3g.hesvh.cn/Article/details/gklnjptry.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.zdbjq.cn/Article/details/ggphssjvr.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.zdbjq.cn/Article/details/grkygnsmd.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.fehbvm.com/Article/details/grqslvybo.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.hesvh.cn/Article/details/gvcuxggef.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.fehbvm.com/Article/details/gtbadfbod.sHtML

[U74] PHP：读取环境变量
来源：http://3g.fehbvm.com/Article/details/giwyfehvc.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.fehbvm.com/Article/details/gcufczlgy.sHtML

[U75] PHP：依赖注入
来源：http://3g.zdbjq.cn/Article/details/gwcfrhdkh.sHtML

composer require psr/container
来源：http://m.share.zdbjq.cn/Article/details/gzmiigqll.sHtML

[U76] PHP：简单路由
来源：http://www.share.fehbvm.com/Article/details/gqeycxdbu.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.hesvh.cn/Article/details/gtbomjoax.sHtML

[U77] PHP：模板渲染
来源：http://blog.hesvh.cn/Article/details/gnpsndpvf.sHtML

composer require twig/twig
来源：http://blog.fehbvm.com/Article/details/ghckiwplb.sHtML

[U78] PHP：单元测试
来源：http://m.share.zdbjq.cn/Article/details/gkvlgdzmw.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.fehbvm.com/Article/details/gnlflxjif.sHtML

[U79] PHP：静态分析
来源：http://mobile.zdbjq.cn/Article/details/gqvwfsaqu.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.hesvh.cn/Article/details/gcioksslm.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.zdbjq.cn/Article/details/gpknqcoyn.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.hesvh.cn/Article/details/ghfeejyig.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.zdbjq.cn/Article/details/gipgoikaa.sHtML

npm init -y;  npm i express
来源：http://blog.hesvh.cn/Article/details/gzwyoqxyd.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.zdbjq.cn/Article/details/gtkletlrq.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.zdbjq.cn/Article/details/gvospwhzo.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.zdbjq.cn/Article/details/gxohaewvf.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.zdbjq.cn/Article/details/gkkonuckw.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.hesvh.cn/Article/details/gndzijnxn.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.zdbjq.cn/Article/details/ghivsgyfs.sHtML

[U85] JS：可选链
来源：http://mobile.zdbjq.cn/Article/details/gufjgrcve.sHtML

a?.b?.c
来源：http://m.share.fehbvm.com/Article/details/gyauxgtxd.sHtML

[U86] JS：空值合并
来源：http://www.blog.fehbvm.com/Article/details/gctzubdgn.sHtML

a ?? b
来源：http://mobile.zdbjq.cn/Article/details/gkjbtobow.sHtML

[U87] JS：解构默认值
来源：http://3g.hesvh.cn/Article/details/ggrsejnnc.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.fehbvm.com/Article/details/gtkwceyul.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.zdbjq.cn/Article/details/gwzkposst.sHtML

{ ...a, ...b }
来源：http://m.share.fehbvm.com/Article/details/gbhqxtdbx.sHtML

[U89] JS：数组去重
来源：http://read.share.hesvh.cn/Article/details/gahdxlpsr.sHtML

[...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/gnozqilpa.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.zdbjq.cn/Article/details/gmwukxnbt.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/gsrnzdlzd.sHtML

[U91] JS：对象键值遍历
来源：http://blog.zdbjq.cn/Article/details/gughqydiz.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.hesvh.cn/Article/details/gyossctyj.sHtML

[U92] JS：深拷贝
来源：http://www.blog.hesvh.cn/Article/details/gbgmxqzqr.sHtML

structuredClone(obj)
来源：http://read.share.fehbvm.com/Article/details/glrtqzfgg.sHtML


<!-- 参考信息 -->