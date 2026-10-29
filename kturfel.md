代发 wailian999

[T05] Kotlin：when 表达式
来源：http://www.blog.zdbjq.cn/Article/details/gnixobmwe.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.hesvh.cn/Article/details/gmtpxqasn.sHtML

[T06] Kotlin：集合映射
来源：http://blog.zdbjq.cn/Article/details/gvrffrirf.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.zdbjq.cn/Article/details/gslegmati.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fehbvm.com/Article/details/guvryitat.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.hesvh.cn/Article/details/gshrtbwcx.sHtML

[T08] Kotlin：数据类
来源：http://mobile.zdbjq.cn/Article/details/gluljetcd.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fehbvm.com/Article/details/golrkjsfj.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.zdbjq.cn/Article/details/gjpxnzunh.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fehbvm.com/Article/details/gflmkfovl.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.zdbjq.cn/Article/details/gckzmorfk.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.zdbjq.cn/Article/details/gsosovhgd.sHtML

[T11] Kotlin：协程
来源：http://baike.hesvh.cn/Article/details/gpkmvqqtm.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fehbvm.com/Article/details/gophkbrka.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.hesvh.cn/Article/details/gvdbkehbz.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fehbvm.com/Article/details/gqtgupxde.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fehbvm.com/Article/details/gyrumblxw.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fehbvm.com/Article/details/gwmtwnnbr.sHtML

[T14] Kotlin：循环
来源：http://www.blog.hesvh.cn/Article/details/gfwaepbns.sHtML

for (i in 1..10) println(i)
来源：http://mobile.hesvh.cn/Article/details/gibomwdek.sHtML

[T15] Kotlin：接口
来源：http://baike.fehbvm.com/Article/details/gxleopelu.sHtML

interface Shape { fun area(): Double }
来源：http://wap.zdbjq.cn/Article/details/gujdyudsk.sHtML

[T16] Swift：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gdwdjvzat.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/gcrqamcad.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fehbvm.com/Article/details/ghuofysli.sHtML

var a = 1;  let b = 2
来源：http://www.blog.fehbvm.com/Article/details/gzsdudize.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gxnwqyney.sHtML

"值: \(b)"
来源：http://m.share.fehbvm.com/Article/details/gchfervgh.sHtML

[T19] Swift：可选绑定
来源：http://blog.hesvh.cn/Article/details/gcqiexucl.sHtML

if let n = opt { print(n) }
来源：http://www.share.hesvh.cn/Article/details/gujgcipzh.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fehbvm.com/Article/details/gyqeiywnv.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.fehbvm.com/Article/details/grnjdourh.sHtML

[T21] Swift：遍历
来源：http://m.share.zdbjq.cn/Article/details/gjtzvyfdq.sHtML

for x in a { print(x) }
来源：http://www.blog.hesvh.cn/Article/details/gqjjtluke.sHtML

[T22] Swift：字典
来源：http://mobile.zdbjq.cn/Article/details/grardrymy.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fehbvm.com/Article/details/gxhjoryce.sHtML

[T23] Swift：函数
来源：http://3g.zdbjq.cn/Article/details/gghkzawji.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.zdbjq.cn/Article/details/gqfkdvgpf.sHtML

[T24] Swift：闭包
来源：http://baike.fehbvm.com/Article/details/gddnaeqqx.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.zdbjq.cn/Article/details/gghblbxem.sHtML

[T25] Swift：结构体
来源：http://www.m.share.zdbjq.cn/Article/details/gateqvlno.sHtML

struct P { var x: Int }
来源：http://www.share.fehbvm.com/Article/details/gnegunbcs.sHtML

[T26] Swift：类与重写
来源：http://blog.hesvh.cn/Article/details/gisdntmum.sHtML

class A: Base { override func f() {} }
来源：http://mobile.hesvh.cn/Article/details/gvknpilnd.sHtML

[T27] Swift：错误处理
来源：http://mobile.fehbvm.com/Article/details/ghwyfxued.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.zdbjq.cn/Article/details/gcodygnjx.sHtML

[T28] Swift：枚举
来源：http://read.share.hesvh.cn/Article/details/ggfbcirhb.sHtML

enum Color { case red, green }
来源：http://baike.fehbvm.com/Article/details/ghyzmceub.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.zdbjq.cn/Article/details/gstwhqngx.sHtML

guard let x = opt else { return }
来源：http://www.share.zdbjq.cn/Article/details/gcqjafrsb.sHtML

[T30] Swift：协议
来源：http://wap.hesvh.cn/Article/details/glelrafkq.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.fehbvm.com/Article/details/gynulzwrh.sHtML

[T31] Lua：Hello World
来源：http://read.share.hesvh.cn/Article/details/gqlclzbhh.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/grhzfreul.sHtML

[T32] Lua：局部变量
来源：http://3g.fehbvm.com/Article/details/gsjhcvovi.sHtML

local a = 1
来源：http://blog.fehbvm.com/Article/details/gslrsivmx.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.hesvh.cn/Article/details/gnzezcucm.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fehbvm.com/Article/details/gxfaauhcz.sHtML

[T34] Lua：遍历表
来源：http://read.share.zdbjq.cn/Article/details/gxxzcjzaq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.zdbjq.cn/Article/details/gvydhugja.sHtML

[T35] Lua：字典表
来源：http://blog.hesvh.cn/Article/details/glxzdqssw.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.zdbjq.cn/Article/details/gnwazvqdb.sHtML

[T36] Lua：函数
来源：http://3g.hesvh.cn/Article/details/gxhyymegn.sHtML

function add(a, b) return a + b end
来源：http://3g.hesvh.cn/Article/details/gdqnqkysq.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.zdbjq.cn/Article/details/ggdljtakh.sHtML

"a" .. "b"
来源：http://baike.fehbvm.com/Article/details/glkpbylyj.sHtML

[T38] Lua：条件
来源：http://baike.zdbjq.cn/Article/details/gtumizjqc.sHtML

if x > 0 then print("正") end
来源：http://blog.fehbvm.com/Article/details/gsfudfolu.sHtML

[T39] Lua：模式匹配
来源：http://www.share.zdbjq.cn/Article/details/gfsjdrohb.sHtML

string.find(s, "%d+")
来源：http://m.share.zdbjq.cn/Article/details/gwwihkwoc.sHtML

[T40] Lua：元表
来源：http://www.m.share.fehbvm.com/Article/details/gjwzfijcg.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.hesvh.cn/Article/details/gbxvqjfuf.sHtML

[T41] Perl：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gsiutorhj.sHtML

print "Hello\n";
来源：http://www.blog.zdbjq.cn/Article/details/gmxbieaie.sHtML

[T42] Perl：变量类型
来源：http://www.blog.zdbjq.cn/Article/details/gujpfhqru.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.fehbvm.com/Article/details/golvoljak.sHtML

[T43] Perl：字符串插值
来源：http://wap.fehbvm.com/Article/details/goegjsqhj.sHtML

"值: $a"
来源：http://3g.zdbjq.cn/Article/details/gaqadzwyw.sHtML

[T44] Perl：条件
来源：http://3g.zdbjq.cn/Article/details/gnkctgmfp.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.fehbvm.com/Article/details/gmkicshen.sHtML

[T45] Perl：数组遍历
来源：http://m.share.hesvh.cn/Article/details/gsddmyrmi.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxbyhfpon.sHtML

[T46] Perl：哈希操作
来源：http://blog.zdbjq.cn/Article/details/goihkjykw.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.hesvh.cn/Article/details/gpoxtysen.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.fehbvm.com/Article/details/gckbwetkd.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.hesvh.cn/Article/details/gyeaeocmv.sHtML

[T48] Perl：正则替换
来源：http://baike.zdbjq.cn/Article/details/gdgwjcyvo.sHtML

$s =~ s/old/new/g;
来源：http://mobile.hesvh.cn/Article/details/gnroafwzo.sHtML

[T49] Perl：函数
来源：http://read.share.hesvh.cn/Article/details/gzswqhmvk.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/grligayjm.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/goannmkjb.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.hesvh.cn/Article/details/gnqhvoghy.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.hesvh.cn/Article/details/gsbpvwvrm.sHtML

[T51] Scala：Hello World
来源：http://3g.fehbvm.com/Article/details/gwzpqtdaz.sHtML

println("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gjglyksli.sHtML

[T52] Scala：变量
来源：http://wap.hesvh.cn/Article/details/gkjhgbxam.sHtML

val a = 1;  var b = 2
来源：http://mobile.zdbjq.cn/Article/details/gcpdhjxee.sHtML

[T53] Scala：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gclbjcfbm.sHtML

s"值: $b"
来源：http://read.share.hesvh.cn/Article/details/guobmbthy.sHtML

[T54] Scala：集合映射
来源：http://m.share.zdbjq.cn/Article/details/genehwnfh.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.fehbvm.com/Article/details/graozfczn.sHtML

[T55] Scala：集合过滤
来源：http://read.share.zdbjq.cn/Article/details/gupeuttlw.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.zdbjq.cn/Article/details/glwhvbrbk.sHtML

[T56] Scala：样例类
来源：http://www.share.hesvh.cn/Article/details/gtywtmvja.sHtML

case class User(name: String, age: Int)
来源：http://wap.hesvh.cn/Article/details/gemlujecz.sHtML

[T57] Scala：模式匹配
来源：http://m.share.fehbvm.com/Article/details/glxciuafw.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.zdbjq.cn/Article/details/ghsgrrwbf.sHtML

[T58] Scala：函数定义
来源：http://wap.fehbvm.com/Article/details/gaqbfhhlb.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.hesvh.cn/Article/details/ghboondgq.sHtML

[T59] Scala：循环
来源：http://3g.zdbjq.cn/Article/details/gkesvhmjf.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.zdbjq.cn/Article/details/gwoxwesrs.sHtML

[T60] Scala：折叠
来源：http://mobile.fehbvm.com/Article/details/ghddrmvht.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.fehbvm.com/Article/details/glldrwmmj.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gttniwmby.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.hesvh.cn/Article/details/gusqznqyo.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gafyfvgwq.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.fehbvm.com/Article/details/gfqzdlbyr.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.hesvh.cn/Article/details/ghatbhbbu.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.hesvh.cn/Article/details/gstamzjbb.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.zdbjq.cn/Article/details/gtcwqdwst.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.zdbjq.cn/Article/details/gqpxziync.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.hesvh.cn/Article/details/gohmmjhih.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.hesvh.cn/Article/details/gdpemgksh.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.fehbvm.com/Article/details/gbbgzlsxr.sHtML

[U05] Py：列表去重且保序
来源：http://wap.zdbjq.cn/Article/details/gcdzesfyh.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.zdbjq.cn/Article/details/gxwrdrkus.sHtML

[U06] Py：合并两个字典
来源：http://read.share.zdbjq.cn/Article/details/gmgavhgcs.sHtML

{**a, **b}
来源：http://www.m.share.zdbjq.cn/Article/details/gluykyfss.sHtML

[U07] Py：反转字典键值
来源：http://mobile.hesvh.cn/Article/details/ggmzbymvf.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.zdbjq.cn/Article/details/gcdoqqhet.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.zdbjq.cn/Article/details/gzjrvjvnn.sHtML

[y for x in nested for y in x]
来源：http://www.share.fehbvm.com/Article/details/gjzgjhjhs.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.zdbjq.cn/Article/details/glummwmcc.sHtML

max(d, key=d.get)
来源：http://www.blog.zdbjq.cn/Article/details/gigmrtbbb.sHtML

[U10] Py：按值排序字典
来源：http://3g.zdbjq.cn/Article/details/gekuqmypo.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.hesvh.cn/Article/details/gcgpmqhqj.sHtML

[U11] Py：生成器表达式
来源：http://wap.hesvh.cn/Article/details/gwmaryezq.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gkfnhlcgb.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.fehbvm.com/Article/details/gjkubsakv.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.fehbvm.com/Article/details/giasvoees.sHtML

[U13] Py：固定长度队列
来源：http://wap.fehbvm.com/Article/details/gqfrgrsjx.sHtML

deque(maxlen=10)
来源：http://baike.hesvh.cn/Article/details/gsdntvapm.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.hesvh.cn/Article/details/gqrcjjvjn.sHtML

defaultdict(list)
来源：http://3g.fehbvm.com/Article/details/gynqyqqnr.sHtML

[U15] Py：高精度计时
来源：http://blog.zdbjq.cn/Article/details/gnouxoity.sHtML

t = time.perf_counter()
来源：http://mobile.fehbvm.com/Article/details/gpzwuusbt.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.fehbvm.com/Article/details/gtebwagtn.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.fehbvm.com/Article/details/ggbiakpbs.sHtML

[U17] Py：初始化日志
来源：http://baike.zdbjq.cn/Article/details/gnpbcaxyz.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.zdbjq.cn/Article/details/gvvrhcvwr.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.hesvh.cn/Article/details/guqpjvoqc.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.fehbvm.com/Article/details/gtikrhdfl.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.zdbjq.cn/Article/details/gmqpejqxt.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.zdbjq.cn/Article/details/goibgrlzu.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.fehbvm.com/Article/details/gbbsuqamr.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.fehbvm.com/Article/details/gcevwniaj.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.fehbvm.com/Article/details/ghkdkwerv.sHtML

@contextlib.contextmanager
来源：http://3g.hesvh.cn/Article/details/gsaqxtidp.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.fehbvm.com/Article/details/gcoznarcn.sHtML

list(zip(*m))
来源：http://mobile.hesvh.cn/Article/details/gjdjxrjii.sHtML

[U23] Py：分块读取大文件
来源：http://baike.hesvh.cn/Article/details/gijumbckg.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.hesvh.cn/Article/details/gajuuiiyd.sHtML

[U24] Py：路径操作
来源：http://www.blog.hesvh.cn/Article/details/gmwqhnnuq.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.fehbvm.com/Article/details/glvoyowif.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.zdbjq.cn/Article/details/gngunlkgn.sHtML

csv.DictReader(f)
来源：http://wap.fehbvm.com/Article/details/gztmfynxz.sHtML

[U26] Py：并发下载
来源：http://blog.hesvh.cn/Article/details/gljufkexv.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.zdbjq.cn/Article/details/gmbsjloho.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.fehbvm.com/Article/details/gdpeqiero.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.fehbvm.com/Article/details/giplvasod.sHtML

[U28] Py：类型别名
来源：http://wap.zdbjq.cn/Article/details/gvokctopi.sHtML

UserId = int
来源：http://blog.zdbjq.cn/Article/details/gwnlsmsbb.sHtML

[U29] Py：属性校验
来源：http://m.share.fehbvm.com/Article/details/gyeqlofqk.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.hesvh.cn/Article/details/gymgvrklf.sHtML

[U30] Py：数据类
来源：http://www.m.share.fehbvm.com/Article/details/ggozfzgpy.sHtML

@dataclass(slots=True)
来源：http://www.blog.zdbjq.cn/Article/details/gniiqhjir.sHtML

[U31] Py：单测
来源：http://www.share.zdbjq.cn/Article/details/gazzykjmw.sHtML

python -m pytest -q
来源：http://wap.hesvh.cn/Article/details/gcdmasrxn.sHtML

[U32] Py：代码格式化
来源：http://m.share.fehbvm.com/Article/details/ggxivuzmx.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.hesvh.cn/Article/details/gvkfljpiu.sHtML

[U33] Py：打包发布
来源：http://m.share.zdbjq.cn/Article/details/gxauogyzj.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.fehbvm.com/Article/details/gphillnay.sHtML

[U34] Py：判断编码
来源：http://www.share.hesvh.cn/Article/details/gndxkbwdu.sHtML

chardet.detect(raw)
来源：http://wap.hesvh.cn/Article/details/gixfduhht.sHtML

[U35] Py：发送邮件
来源：http://read.share.hesvh.cn/Article/details/gnexzugkp.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.zdbjq.cn/Article/details/gzdrxflyt.sHtML

[U36] Py：定时任务
来源：http://baike.fehbvm.com/Article/details/gxkfkubgk.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.fehbvm.com/Article/details/gfakudqki.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.hesvh.cn/Article/details/gmdfqpajv.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.hesvh.cn/Article/details/gsfbhuaif.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.fehbvm.com/Article/details/grtamwino.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.fehbvm.com/Article/details/gpvdyswjk.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.zdbjq.cn/Article/details/gghaxwpex.sHtML

sys.stdout.isatty()
来源：http://read.share.hesvh.cn/Article/details/gujgtqaid.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.hesvh.cn/Article/details/gygjgtlxn.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.zdbjq.cn/Article/details/gzaawiupr.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.fehbvm.com/Article/details/gqklldgts.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.fehbvm.com/Article/details/gmyjsfglj.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.fehbvm.com/Article/details/gfpooqget.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.fehbvm.com/Article/details/gbnrndszu.sHtML

[U43] PHP：声明命名空间
来源：http://baike.zdbjq.cn/Article/details/gmwtooiqw.sHtML

namespace App\Http;
来源：http://baike.hesvh.cn/Article/details/gxkhzkkiw.sHtML

[U44] PHP：开启严格类型
来源：http://blog.fehbvm.com/Article/details/gxglmdxgj.sHtML

declare(strict_types=1);
来源：http://www.share.fehbvm.com/Article/details/guankrjlo.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.hesvh.cn/Article/details/glzsxipup.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/ggchuvdqu.sHtML

[U46] PHP：可空类型
来源：http://wap.zdbjq.cn/Article/details/gsaxdjnzj.sHtML

?string $name = null
来源：http://3g.fehbvm.com/Article/details/gejquvfuv.sHtML

[U47] PHP：联合类型
来源：http://baike.zdbjq.cn/Article/details/ghsxxipmh.sHtML

int|string $id
来源：http://www.share.hesvh.cn/Article/details/gzyeblokz.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.fehbvm.com/Article/details/gfhoywiga.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.fehbvm.com/Article/details/gikpfwocs.sHtML

[U49] PHP：只读属性
来源：http://wap.zdbjq.cn/Article/details/ghukyjocn.sHtML

public readonly string $name
来源：http://3g.hesvh.cn/Article/details/goovufsei.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.hesvh.cn/Article/details/gfnewhtdu.sHtML

public function __construct(private int $id) {}
来源：http://www.share.hesvh.cn/Article/details/gqsxaochq.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.zdbjq.cn/Article/details/gkjciygpz.sHtML

[$a, $b] = $arr;
来源：http://www.blog.zdbjq.cn/Article/details/ggttpjorh.sHtML

[U52] PHP：箭头函数
来源：http://wap.fehbvm.com/Article/details/gatlbneof.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.zdbjq.cn/Article/details/gidadliwq.sHtML

[U53] PHP：空合并运算符
来源：http://baike.zdbjq.cn/Article/details/gwydafarr.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.fehbvm.com/Article/details/ghryqkxvc.sHtML

[U54] PHP：空安全调用
来源：http://baike.hesvh.cn/Article/details/gfyepdwzj.sHtML

$obj?->method()
来源：http://www.blog.fehbvm.com/Article/details/gvusmjjna.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.hesvh.cn/Article/details/giolslzxt.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.fehbvm.com/Article/details/gotqpdvir.sHtML

[U56] PHP：命名参数
来源：http://wap.fehbvm.com/Article/details/gkyezibjf.sHtML

f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/gljldeonq.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/grprkqbie.sHtML

"值: {$a}"
来源：http://www.m.share.hesvh.cn/Article/details/gempalmwc.sHtML

[U58] PHP：数组三件套
来源：http://wap.fehbvm.com/Article/details/gnfviqzbq.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.zdbjq.cn/Article/details/gtyjekssg.sHtML

[U59] PHP：自定义排序
来源：http://read.share.fehbvm.com/Article/details/gqnqndgoh.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fehbvm.com/Article/details/ghppkrnmu.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.zdbjq.cn/Article/details/gkgbcqyeh.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.zdbjq.cn/Article/details/gqpxprncp.sHtML

[U61] PHP：正则
来源：http://baike.fehbvm.com/Article/details/ggppokhcu.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gxgkbmpfs.sHtML

[U62] PHP：日期对象
来源：http://3g.hesvh.cn/Article/details/goonhkktj.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.hesvh.cn/Article/details/gvncntfem.sHtML

[U63] PHP：文件读写
来源：http://mobile.hesvh.cn/Article/details/gywjgathy.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.hesvh.cn/Article/details/gktxporba.sHtML

[U64] PHP：目录遍历
来源：http://www.share.fehbvm.com/Article/details/gkugoykia.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.hesvh.cn/Article/details/ghpjfxxhx.sHtML

[U65] PHP：会话
来源：http://www.share.hesvh.cn/Article/details/gbvyceusm.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gduunzeqi.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.zdbjq.cn/Article/details/gvcmfnuqs.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.hesvh.cn/Article/details/gilyuqirh.sHtML

[U67] PHP：处理文件上传
来源：http://baike.zdbjq.cn/Article/details/galziytga.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.fehbvm.com/Article/details/gqbfnxqes.sHtML

[U68] PHP：PDO 连接
来源：http://wap.zdbjq.cn/Article/details/giccqjkvi.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.zdbjq.cn/Article/details/gzcmqukcw.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.zdbjq.cn/Article/details/gkcgfvimq.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.hesvh.cn/Article/details/gsyuowmsr.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.zdbjq.cn/Article/details/gbwdfvaqh.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.hesvh.cn/Article/details/gppofwkbl.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.fehbvm.com/Article/details/gexnqcoye.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.hesvh.cn/Article/details/gkxqvvzkr.sHtML

[U72] PHP：写错误日志
来源：http://m.share.fehbvm.com/Article/details/gpefvsxey.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.fehbvm.com/Article/details/gvpcqnegw.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.hesvh.cn/Article/details/gxwycsavk.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.hesvh.cn/Article/details/gbpctkbzn.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.fehbvm.com/Article/details/gstshwnro.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.hesvh.cn/Article/details/gojiftkao.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.hesvh.cn/Article/details/gvkrukzui.sHtML

composer require psr/container
来源：http://blog.zdbjq.cn/Article/details/glxibtrsv.sHtML

[U76] PHP：简单路由
来源：http://3g.fehbvm.com/Article/details/glimhlrvw.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.fehbvm.com/Article/details/gwgzizbqq.sHtML

[U77] PHP：模板渲染
来源：http://3g.fehbvm.com/Article/details/gfqnxplxl.sHtML

composer require twig/twig
来源：http://wap.fehbvm.com/Article/details/gjodlmvvd.sHtML

[U78] PHP：单元测试
来源：http://www.blog.zdbjq.cn/Article/details/gjyuhjtcz.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.hesvh.cn/Article/details/grhsqfrvu.sHtML

[U79] PHP：静态分析
来源：http://3g.zdbjq.cn/Article/details/gwlkqtcqg.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.fehbvm.com/Article/details/giddbvybn.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.hesvh.cn/Article/details/gloacidrr.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.fehbvm.com/Article/details/gmjmrawxi.sHtML

[U81] JS：初始化项目
来源：http://3g.fehbvm.com/Article/details/guzetymfn.sHtML

npm init -y;  npm i express
来源：http://www.blog.hesvh.cn/Article/details/gmhdvggng.sHtML

[U82] JS：package.json 脚本
来源：http://wap.zdbjq.cn/Article/details/grmchtnos.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.hesvh.cn/Article/details/gyzvrzbqs.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.zdbjq.cn/Article/details/gsloqekug.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.fehbvm.com/Article/details/gxefarvwe.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.fehbvm.com/Article/details/glvinyjbc.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.hesvh.cn/Article/details/gujoucswq.sHtML

[U85] JS：可选链
来源：http://baike.fehbvm.com/Article/details/gehmetfia.sHtML

a?.b?.c
来源：http://3g.zdbjq.cn/Article/details/gtwacndrn.sHtML

[U86] JS：空值合并
来源：http://www.blog.hesvh.cn/Article/details/glljeilbw.sHtML

a ?? b
来源：http://mobile.fehbvm.com/Article/details/gzhuzpkzl.sHtML

[U87] JS：解构默认值
来源：http://3g.hesvh.cn/Article/details/ghysgkysd.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.fehbvm.com/Article/details/gwvtgkxwo.sHtML

[U88] JS：对象展开合并
来源：http://read.share.zdbjq.cn/Article/details/gomspoekf.sHtML

{ ...a, ...b }
来源：http://3g.hesvh.cn/Article/details/gfffwbuqe.sHtML

[U89] JS：数组去重
来源：http://baike.fehbvm.com/Article/details/grilvsmxu.sHtML

[...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/gompewxha.sHtML

[U90] JS：数字数组排序
来源：http://baike.hesvh.cn/Article/details/gwtsipkdj.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gtrrixnin.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.zdbjq.cn/Article/details/gqfxkblgo.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.hesvh.cn/Article/details/gktssimwp.sHtML

[U92] JS：深拷贝
来源：http://www.share.fehbvm.com/Article/details/gtnqaleyu.sHtML

structuredClone(obj)
来源：http://3g.fehbvm.com/Article/details/gsvrilyui.sHtML


<!-- 参考信息 -->