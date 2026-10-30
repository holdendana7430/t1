代发 wailian999

[T05] Kotlin：when 表达式
来源：http://wap.fehbvm.com/Article/details/gjnmhqlye.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.zdbjq.cn/Article/details/gldqfexca.sHtML

[T06] Kotlin：集合映射
来源：http://wap.hesvh.cn/Article/details/gdicndylu.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gqcwsoxhv.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fehbvm.com/Article/details/ghtwlqwwr.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fehbvm.com/Article/details/gttbfuhnf.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.zdbjq.cn/Article/details/gpljyrppl.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.hesvh.cn/Article/details/goqpqjvbx.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fehbvm.com/Article/details/gehuochzc.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.hesvh.cn/Article/details/gqijlikjq.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fehbvm.com/Article/details/gomtplbrt.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.hesvh.cn/Article/details/gtrxbdbad.sHtML

[T11] Kotlin：协程
来源：http://mobile.zdbjq.cn/Article/details/gztogjvyt.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.hesvh.cn/Article/details/gksdimblw.sHtML

[T12] Kotlin：解构声明
来源：http://baike.hesvh.cn/Article/details/gwcpgxtin.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gxpukwswu.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.hesvh.cn/Article/details/gkpxtqfrr.sHtML

val m = mapOf("a" to 1)
来源：http://baike.hesvh.cn/Article/details/gvvujzpdq.sHtML

[T14] Kotlin：循环
来源：http://baike.fehbvm.com/Article/details/gzkhragma.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fehbvm.com/Article/details/gwmbanukq.sHtML

[T15] Kotlin：接口
来源：http://3g.fehbvm.com/Article/details/gyliwmgif.sHtML

interface Shape { fun area(): Double }
来源：http://baike.zdbjq.cn/Article/details/gpmrjorge.sHtML

[T16] Swift：Hello World
来源：http://baike.fehbvm.com/Article/details/gzdftsmcz.sHtML

print("Hello")
来源：http://baike.hesvh.cn/Article/details/gswelsokv.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fehbvm.com/Article/details/gajfygffv.sHtML

var a = 1;  let b = 2
来源：http://read.share.zdbjq.cn/Article/details/gegplzspo.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gamrxxmwo.sHtML

"值: \(b)"
来源：http://blog.hesvh.cn/Article/details/grcpkorom.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fehbvm.com/Article/details/gcaeoyvbj.sHtML

if let n = opt { print(n) }
来源：http://read.share.hesvh.cn/Article/details/gefugpqxg.sHtML

[T20] Swift：数组操作
来源：http://m.share.hesvh.cn/Article/details/geurwcyyp.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.zdbjq.cn/Article/details/gtrvumzif.sHtML

[T21] Swift：遍历
来源：http://www.share.fehbvm.com/Article/details/gvllcylyu.sHtML

for x in a { print(x) }
来源：http://read.share.zdbjq.cn/Article/details/gprbriuet.sHtML

[T22] Swift：字典
来源：http://read.share.fehbvm.com/Article/details/gxpztufwn.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.hesvh.cn/Article/details/gsnehgflj.sHtML

[T23] Swift：函数
来源：http://blog.zdbjq.cn/Article/details/gyoulrrkp.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.zdbjq.cn/Article/details/gqrcrwwti.sHtML

[T24] Swift：闭包
来源：http://www.blog.hesvh.cn/Article/details/gvdjjyvnf.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gryefhgny.sHtML

[T25] Swift：结构体
来源：http://baike.zdbjq.cn/Article/details/gqsithsxh.sHtML

struct P { var x: Int }
来源：http://www.blog.zdbjq.cn/Article/details/gpydmllpd.sHtML

[T26] Swift：类与重写
来源：http://mobile.zdbjq.cn/Article/details/garoksknx.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fehbvm.com/Article/details/gjzqmsmsw.sHtML

[T27] Swift：错误处理
来源：http://www.blog.hesvh.cn/Article/details/georeyggl.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.zdbjq.cn/Article/details/gzxmqglls.sHtML

[T28] Swift：枚举
来源：http://mobile.zdbjq.cn/Article/details/gnixnmefz.sHtML

enum Color { case red, green }
来源：http://www.share.zdbjq.cn/Article/details/goxxuinkk.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.zdbjq.cn/Article/details/gglonjgnp.sHtML

guard let x = opt else { return }
来源：http://baike.hesvh.cn/Article/details/gvnnxkmtf.sHtML

[T30] Swift：协议
来源：http://3g.zdbjq.cn/Article/details/gkakfzauu.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.zdbjq.cn/Article/details/gjzbmynja.sHtML

[T31] Lua：Hello World
来源：http://wap.fehbvm.com/Article/details/gdverlxln.sHtML

print("Hello")
来源：http://m.share.zdbjq.cn/Article/details/ggdyzofvc.sHtML

[T32] Lua：局部变量
来源：http://mobile.hesvh.cn/Article/details/gjtoshafn.sHtML

local a = 1
来源：http://blog.fehbvm.com/Article/details/gzzujpoci.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.fehbvm.com/Article/details/gamsnyphf.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.hesvh.cn/Article/details/gpqscrqzv.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.hesvh.cn/Article/details/gonlajxii.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.hesvh.cn/Article/details/ggatvwgwt.sHtML

[T35] Lua：字典表
来源：http://mobile.zdbjq.cn/Article/details/glretmdmd.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.fehbvm.com/Article/details/gfopkuarv.sHtML

[T36] Lua：函数
来源：http://read.share.hesvh.cn/Article/details/gvmyhnjdf.sHtML

function add(a, b) return a + b end
来源：http://m.share.zdbjq.cn/Article/details/gbijtlnaa.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.hesvh.cn/Article/details/gcmbfjeqh.sHtML

"a" .. "b"
来源：http://wap.hesvh.cn/Article/details/gvbkzjnwt.sHtML

[T38] Lua：条件
来源：http://mobile.fehbvm.com/Article/details/gidbflacl.sHtML

if x > 0 then print("正") end
来源：http://www.blog.zdbjq.cn/Article/details/ghddbufro.sHtML

[T39] Lua：模式匹配
来源：http://www.share.hesvh.cn/Article/details/gfhigylzh.sHtML

string.find(s, "%d+")
来源：http://read.share.hesvh.cn/Article/details/gipawqpfd.sHtML

[T40] Lua：元表
来源：http://www.share.hesvh.cn/Article/details/gqditfkho.sHtML

setmetatable({}, { __index = base })
来源：http://3g.hesvh.cn/Article/details/gnxpfrswp.sHtML

[T41] Perl：Hello World
来源：http://3g.hesvh.cn/Article/details/gtwkygbwf.sHtML

print "Hello\n";
来源：http://www.share.zdbjq.cn/Article/details/ggstlstxh.sHtML

[T42] Perl：变量类型
来源：http://m.share.zdbjq.cn/Article/details/gtswtlplw.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.zdbjq.cn/Article/details/gdoubbxsk.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gbqykkchx.sHtML

"值: $a"
来源：http://www.share.fehbvm.com/Article/details/gvwfemgpe.sHtML

[T44] Perl：条件
来源：http://wap.hesvh.cn/Article/details/guqhjofad.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.zdbjq.cn/Article/details/gkoagmqpi.sHtML

[T45] Perl：数组遍历
来源：http://m.share.fehbvm.com/Article/details/gsbnkjtzv.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.zdbjq.cn/Article/details/gkbnbspnn.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.hesvh.cn/Article/details/gyhzysqmf.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.zdbjq.cn/Article/details/gnwinrtkt.sHtML

[T47] Perl：正则捕获
来源：http://m.share.hesvh.cn/Article/details/gmyqkluwi.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.zdbjq.cn/Article/details/gallumswj.sHtML

[T48] Perl：正则替换
来源：http://m.share.zdbjq.cn/Article/details/gcpiozwpf.sHtML

$s =~ s/old/new/g;
来源：http://m.share.fehbvm.com/Article/details/gnwesyjcb.sHtML

[T49] Perl：函数
来源：http://baike.zdbjq.cn/Article/details/glaxbmtae.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gptkxhunc.sHtML

[T50] Perl：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gxrysiicz.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.zdbjq.cn/Article/details/gjroyscsz.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.fehbvm.com/Article/details/gbsflkedr.sHtML

[T51] Scala：Hello World
来源：http://3g.fehbvm.com/Article/details/gdbplcftm.sHtML

println("Hello")
来源：http://www.share.zdbjq.cn/Article/details/glhlnsgle.sHtML

[T52] Scala：变量
来源：http://3g.hesvh.cn/Article/details/gvswrftwn.sHtML

val a = 1;  var b = 2
来源：http://3g.fehbvm.com/Article/details/gikychyop.sHtML

[T53] Scala：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gjsawfgqr.sHtML

s"值: $b"
来源：http://m.share.fehbvm.com/Article/details/gwgkwrlxx.sHtML

[T54] Scala：集合映射
来源：http://3g.hesvh.cn/Article/details/gtvykjsse.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.hesvh.cn/Article/details/goazhbbqc.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.hesvh.cn/Article/details/gyotpbmch.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.hesvh.cn/Article/details/gzjmhxpyb.sHtML

[T56] Scala：样例类
来源：http://mobile.zdbjq.cn/Article/details/gtkxumfgm.sHtML

case class User(name: String, age: Int)
来源：http://3g.hesvh.cn/Article/details/gnkxuhzjb.sHtML

[T57] Scala：模式匹配
来源：http://mobile.fehbvm.com/Article/details/gaqgyafqj.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.hesvh.cn/Article/details/gyqmldprp.sHtML

[T58] Scala：函数定义
来源：http://www.share.zdbjq.cn/Article/details/gvynfrjzq.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.hesvh.cn/Article/details/gkkdqdmqr.sHtML

[T59] Scala：循环
来源：http://www.share.fehbvm.com/Article/details/gahyaacfm.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.zdbjq.cn/Article/details/gtkhhekgp.sHtML

[T60] Scala：折叠
来源：http://blog.zdbjq.cn/Article/details/gcwbaknyv.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.zdbjq.cn/Article/details/gycguukzk.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gingajvjk.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.zdbjq.cn/Article/details/goavgkdcf.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gtfivryvu.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.hesvh.cn/Article/details/glxzrridq.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.zdbjq.cn/Article/details/gxsgyxxws.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.zdbjq.cn/Article/details/glwtsfocx.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.fehbvm.com/Article/details/grtyarqub.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.hesvh.cn/Article/details/gnbphacea.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.hesvh.cn/Article/details/gausvdgko.sHtML

[U04] Py：变量调试打印
来源：http://3g.fehbvm.com/Article/details/gngksahmb.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.fehbvm.com/Article/details/gkrrhybaa.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.hesvh.cn/Article/details/ggbhfdjse.sHtML

list(dict.fromkeys(arr))
来源：http://blog.zdbjq.cn/Article/details/gzeqcscad.sHtML

[U06] Py：合并两个字典
来源：http://blog.zdbjq.cn/Article/details/gldnlmhlh.sHtML

{**a, **b}
来源：http://baike.zdbjq.cn/Article/details/gzutownpm.sHtML

[U07] Py：反转字典键值
来源：http://wap.hesvh.cn/Article/details/guhawhgxg.sHtML

{v: k for k, v in d.items()}
来源：http://wap.zdbjq.cn/Article/details/gyjbtrslc.sHtML

[U08] Py：展平二维列表
来源：http://wap.fehbvm.com/Article/details/gdacjqmtz.sHtML

[y for x in nested for y in x]
来源：http://www.share.fehbvm.com/Article/details/ghsjigmcq.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.hesvh.cn/Article/details/guymfmeff.sHtML

max(d, key=d.get)
来源：http://mobile.zdbjq.cn/Article/details/ggvqjdlen.sHtML

[U10] Py：按值排序字典
来源：http://m.share.hesvh.cn/Article/details/gdccuuxea.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.hesvh.cn/Article/details/gishxlzyg.sHtML

[U11] Py：生成器表达式
来源：http://wap.fehbvm.com/Article/details/gguwrdipe.sHtML

(x * 2 for x in arr)
来源：http://www.share.zdbjq.cn/Article/details/gstlvjfxi.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.zdbjq.cn/Article/details/gvusvozpv.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.fehbvm.com/Article/details/gcwmnknli.sHtML

[U13] Py：固定长度队列
来源：http://mobile.zdbjq.cn/Article/details/ggcpckmaj.sHtML

deque(maxlen=10)
来源：http://m.share.fehbvm.com/Article/details/gxlpvmbni.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.zdbjq.cn/Article/details/geutdbyda.sHtML

defaultdict(list)
来源：http://baike.zdbjq.cn/Article/details/gsrudeqah.sHtML

[U15] Py：高精度计时
来源：http://www.share.zdbjq.cn/Article/details/gqwdldnsn.sHtML

t = time.perf_counter()
来源：http://mobile.fehbvm.com/Article/details/gbbazdopq.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.zdbjq.cn/Article/details/gtglfjqwj.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.fehbvm.com/Article/details/gjoszgnac.sHtML

[U17] Py：初始化日志
来源：http://www.share.zdbjq.cn/Article/details/gaqhntuwm.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.zdbjq.cn/Article/details/ghchfidia.sHtML

[U18] Py：预编译正则
来源：http://www.share.hesvh.cn/Article/details/ghofoeglp.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fehbvm.com/Article/details/gbbjzfabl.sHtML

[U19] Py：正则替换带回调
来源：http://baike.hesvh.cn/Article/details/gvgljtnea.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.hesvh.cn/Article/details/gwnzrcvaw.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.zdbjq.cn/Article/details/gxswzookj.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.hesvh.cn/Article/details/gtbzbumlm.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.fehbvm.com/Article/details/gptsevfrd.sHtML

@contextlib.contextmanager
来源：http://3g.hesvh.cn/Article/details/gssocodco.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.zdbjq.cn/Article/details/gqwelhjtu.sHtML

list(zip(*m))
来源：http://www.blog.hesvh.cn/Article/details/gwulmaixx.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.zdbjq.cn/Article/details/gozpgtrqp.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.hesvh.cn/Article/details/gueksopyb.sHtML

[U24] Py：路径操作
来源：http://www.m.share.hesvh.cn/Article/details/gwduxfpfb.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.fehbvm.com/Article/details/gwdlepiil.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.hesvh.cn/Article/details/griafipft.sHtML

csv.DictReader(f)
来源：http://wap.hesvh.cn/Article/details/gmhjfrigi.sHtML

[U26] Py：并发下载
来源：http://baike.fehbvm.com/Article/details/gvqyxxdof.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.fehbvm.com/Article/details/gyhnehshr.sHtML

[U27] Py：异步 HTTP
来源：http://wap.fehbvm.com/Article/details/gavoqczzo.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.hesvh.cn/Article/details/gpbcibcdl.sHtML

[U28] Py：类型别名
来源：http://mobile.fehbvm.com/Article/details/gmmhsyecy.sHtML

UserId = int
来源：http://wap.hesvh.cn/Article/details/gnwzsvviv.sHtML

[U29] Py：属性校验
来源：http://www.m.share.hesvh.cn/Article/details/gubtriich.sHtML

@property 与 @x.setter 配合
来源：http://m.share.zdbjq.cn/Article/details/gjvoqnwjq.sHtML

[U30] Py：数据类
来源：http://www.blog.fehbvm.com/Article/details/gvjkkcpxu.sHtML

@dataclass(slots=True)
来源：http://mobile.zdbjq.cn/Article/details/ggwvrblhp.sHtML

[U31] Py：单测
来源：http://blog.fehbvm.com/Article/details/gnisfkdlx.sHtML

python -m pytest -q
来源：http://www.share.hesvh.cn/Article/details/goffbkqau.sHtML

[U32] Py：代码格式化
来源：http://www.blog.hesvh.cn/Article/details/gjkvozsdb.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.zdbjq.cn/Article/details/gcnpwtlux.sHtML

[U33] Py：打包发布
来源：http://www.m.share.hesvh.cn/Article/details/gnzxtjgfx.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.fehbvm.com/Article/details/gpelcarff.sHtML

[U34] Py：判断编码
来源：http://read.share.zdbjq.cn/Article/details/gifnyvztd.sHtML

chardet.detect(raw)
来源：http://wap.fehbvm.com/Article/details/gvepuhvhf.sHtML

[U35] Py：发送邮件
来源：http://read.share.hesvh.cn/Article/details/gwgrzsxvb.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.hesvh.cn/Article/details/ggciqwzyu.sHtML

[U36] Py：定时任务
来源：http://www.share.zdbjq.cn/Article/details/gmmnznfxk.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.fehbvm.com/Article/details/gxgfrlsje.sHtML

[U37] Py：读写 Excel
来源：http://wap.fehbvm.com/Article/details/gkggcpseb.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.fehbvm.com/Article/details/givlwncch.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fehbvm.com/Article/details/gcwexzego.sHtML

Path(__file__).resolve().parent
来源：http://mobile.fehbvm.com/Article/details/gviygcsyk.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.hesvh.cn/Article/details/gojgbymlx.sHtML

sys.stdout.isatty()
来源：http://3g.hesvh.cn/Article/details/gmbpywqno.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.fehbvm.com/Article/details/gugbzdswz.sHtML

print("err", file=sys.stderr)
来源：http://mobile.fehbvm.com/Article/details/gmawepklr.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.fehbvm.com/Article/details/gtqwykszf.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.hesvh.cn/Article/details/ggjxurlhq.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.hesvh.cn/Article/details/gyubdygdq.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.fehbvm.com/Article/details/gprppsfip.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.zdbjq.cn/Article/details/gpxrfmzff.sHtML

namespace App\Http;
来源：http://3g.zdbjq.cn/Article/details/gciwawjrl.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.zdbjq.cn/Article/details/guffochuu.sHtML

declare(strict_types=1);
来源：http://mobile.zdbjq.cn/Article/details/gxjinqqlp.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.hesvh.cn/Article/details/gtuzvdcsy.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gsogmeenj.sHtML

[U46] PHP：可空类型
来源：http://3g.hesvh.cn/Article/details/gljqchuzj.sHtML

?string $name = null
来源：http://www.share.fehbvm.com/Article/details/gjggjoirc.sHtML

[U47] PHP：联合类型
来源：http://m.share.hesvh.cn/Article/details/glkgwjrlc.sHtML

int|string $id
来源：http://m.share.hesvh.cn/Article/details/ggawzmkbq.sHtML

[U48] PHP：纯枚举
来源：http://www.share.zdbjq.cn/Article/details/gajahzypb.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.fehbvm.com/Article/details/gidlzbqze.sHtML

[U49] PHP：只读属性
来源：http://www.share.hesvh.cn/Article/details/gefqtqxwb.sHtML

public readonly string $name
来源：http://read.share.zdbjq.cn/Article/details/gfdgiqoyv.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.hesvh.cn/Article/details/gnomzjdps.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.zdbjq.cn/Article/details/gysueohww.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.hesvh.cn/Article/details/gemccgtzt.sHtML

[$a, $b] = $arr;
来源：http://baike.zdbjq.cn/Article/details/gqcukcido.sHtML

[U52] PHP：箭头函数
来源：http://read.share.hesvh.cn/Article/details/guvekcnra.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.fehbvm.com/Article/details/gjwbuvcqv.sHtML

[U53] PHP：空合并运算符
来源：http://3g.hesvh.cn/Article/details/gqryxpzjs.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.hesvh.cn/Article/details/gnflfcauv.sHtML

[U54] PHP：空安全调用
来源：http://mobile.zdbjq.cn/Article/details/gaycexosx.sHtML

$obj?->method()
来源：http://mobile.hesvh.cn/Article/details/gtzlpjivx.sHtML

[U55] PHP：match 表达式
来源：http://read.share.hesvh.cn/Article/details/gcdzpfopu.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.hesvh.cn/Article/details/gepxkdafd.sHtML

[U56] PHP：命名参数
来源：http://www.blog.hesvh.cn/Article/details/gifxprxgw.sHtML

f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/gfmadzxky.sHtML

[U57] PHP：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gcfxstviu.sHtML

"值: {$a}"
来源：http://blog.zdbjq.cn/Article/details/gzuyagkth.sHtML

[U58] PHP：数组三件套
来源：http://blog.hesvh.cn/Article/details/gvefvutly.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.fehbvm.com/Article/details/gdbeybdru.sHtML

[U59] PHP：自定义排序
来源：http://baike.hesvh.cn/Article/details/ggicbwahr.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fehbvm.com/Article/details/gvvdoanyi.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.hesvh.cn/Article/details/gsjnnwooy.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.hesvh.cn/Article/details/gamcnswse.sHtML

[U61] PHP：正则
来源：http://mobile.zdbjq.cn/Article/details/gnkpsafly.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.hesvh.cn/Article/details/grnrcqwtn.sHtML

[U62] PHP：日期对象
来源：http://3g.fehbvm.com/Article/details/gttracmdp.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.fehbvm.com/Article/details/gtroeasjk.sHtML

[U63] PHP：文件读写
来源：http://www.share.hesvh.cn/Article/details/gnlgcnfzz.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.hesvh.cn/Article/details/gtjctewju.sHtML

[U64] PHP：目录遍历
来源：http://m.share.fehbvm.com/Article/details/ghyhihsgm.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.zdbjq.cn/Article/details/gijvchepf.sHtML

[U65] PHP：会话
来源：http://wap.hesvh.cn/Article/details/gfughxmba.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.hesvh.cn/Article/details/ganqkqnmh.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.zdbjq.cn/Article/details/glngfaqyp.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.fehbvm.com/Article/details/gmzbgkwmg.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.hesvh.cn/Article/details/gmboxpzir.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.zdbjq.cn/Article/details/gnvighcgc.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.zdbjq.cn/Article/details/gbvaqbbec.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.hesvh.cn/Article/details/gcaxiteto.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.zdbjq.cn/Article/details/gwxinrvdd.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.zdbjq.cn/Article/details/gxenpttuu.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.hesvh.cn/Article/details/gaviqlesy.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.fehbvm.com/Article/details/gelcmuxyq.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.zdbjq.cn/Article/details/gumpsqgvd.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.zdbjq.cn/Article/details/gaidoyuso.sHtML

[U72] PHP：写错误日志
来源：http://www.share.hesvh.cn/Article/details/gqkotaddz.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.zdbjq.cn/Article/details/gojtjbkdo.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.zdbjq.cn/Article/details/gwbyttmaq.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.hesvh.cn/Article/details/gqhjimhwk.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.hesvh.cn/Article/details/glefczcml.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.hesvh.cn/Article/details/gxpqizdos.sHtML

[U75] PHP：依赖注入
来源：http://www.share.zdbjq.cn/Article/details/grwltefld.sHtML

composer require psr/container
来源：http://read.share.fehbvm.com/Article/details/gttbvaeqa.sHtML

[U76] PHP：简单路由
来源：http://wap.zdbjq.cn/Article/details/gtnwxszxv.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.zdbjq.cn/Article/details/gadbfztly.sHtML

[U77] PHP：模板渲染
来源：http://3g.hesvh.cn/Article/details/gxmwratji.sHtML

composer require twig/twig
来源：http://blog.fehbvm.com/Article/details/geunderkn.sHtML

[U78] PHP：单元测试
来源：http://blog.hesvh.cn/Article/details/gxjfzsxvf.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.zdbjq.cn/Article/details/gynxtaizc.sHtML

[U79] PHP：静态分析
来源：http://3g.fehbvm.com/Article/details/gxcnwlsuy.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.fehbvm.com/Article/details/gluqcnblg.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.zdbjq.cn/Article/details/gncyoiiis.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.fehbvm.com/Article/details/gzzrxwjnc.sHtML

[U81] JS：初始化项目
来源：http://www.share.hesvh.cn/Article/details/gjrngzxos.sHtML

npm init -y;  npm i express
来源：http://m.share.fehbvm.com/Article/details/gfbjgoiqf.sHtML

[U82] JS：package.json 脚本
来源：http://wap.zdbjq.cn/Article/details/galbrjlhn.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.hesvh.cn/Article/details/ggpulhlgo.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.hesvh.cn/Article/details/gjghdxlza.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.zdbjq.cn/Article/details/gvibdaato.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.zdbjq.cn/Article/details/gxiybxrln.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.zdbjq.cn/Article/details/giumygecz.sHtML

[U85] JS：可选链
来源：http://blog.fehbvm.com/Article/details/gxiuehmgz.sHtML

a?.b?.c
来源：http://www.m.share.zdbjq.cn/Article/details/gkryhmbdk.sHtML

[U86] JS：空值合并
来源：http://baike.fehbvm.com/Article/details/goopwbwrs.sHtML

a ?? b
来源：http://wap.zdbjq.cn/Article/details/grtyloddd.sHtML

[U87] JS：解构默认值
来源：http://m.share.hesvh.cn/Article/details/gstsdhupu.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.zdbjq.cn/Article/details/gowxxmsyv.sHtML

[U88] JS：对象展开合并
来源：http://www.share.hesvh.cn/Article/details/gpzuunnea.sHtML

{ ...a, ...b }
来源：http://m.share.fehbvm.com/Article/details/gjyjoxlyy.sHtML

[U89] JS：数组去重
来源：http://m.share.zdbjq.cn/Article/details/gunxtuyrz.sHtML

[...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/gwulaynnt.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.hesvh.cn/Article/details/gyroohamu.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gbzlghifz.sHtML

[U91] JS：对象键值遍历
来源：http://baike.fehbvm.com/Article/details/gsaxfxthf.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.fehbvm.com/Article/details/gafpayomr.sHtML

[U92] JS：深拷贝
来源：http://3g.hesvh.cn/Article/details/glzixdcfk.sHtML

structuredClone(obj)
来源：http://www.share.hesvh.cn/Article/details/gxiixqmgt.sHtML


<!-- 参考信息 -->