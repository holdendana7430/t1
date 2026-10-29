代发 wailian999

[T05] Kotlin：when 表达式
来源：http://baike.fehbvm.com/Article/details/govlpqlnv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.zdbjq.cn/Article/details/gonnthlpn.sHtML

[T06] Kotlin：集合映射
来源：http://wap.zdbjq.cn/Article/details/gmanvgeaz.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.zdbjq.cn/Article/details/gxkgbgtfl.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/grdctrgdt.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.zdbjq.cn/Article/details/gbhskysva.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fehbvm.com/Article/details/gvugisiik.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.zdbjq.cn/Article/details/gqqwhdtxx.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.hesvh.cn/Article/details/gwgxkdkix.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.hesvh.cn/Article/details/gyvdvrxpy.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fehbvm.com/Article/details/ghifjzzkv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.zdbjq.cn/Article/details/gjcmgwbyf.sHtML

[T11] Kotlin：协程
来源：http://3g.hesvh.cn/Article/details/gqznxkkwo.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fehbvm.com/Article/details/gkzdxtuvr.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.zdbjq.cn/Article/details/gsusjgfyl.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fehbvm.com/Article/details/ghwpcffbs.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fehbvm.com/Article/details/gjnntpclq.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fehbvm.com/Article/details/gaxmgyuah.sHtML

[T14] Kotlin：循环
来源：http://mobile.hesvh.cn/Article/details/giihunxcy.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.hesvh.cn/Article/details/gmilpcwho.sHtML

[T15] Kotlin：接口
来源：http://read.share.fehbvm.com/Article/details/gjffjghur.sHtML

interface Shape { fun area(): Double }
来源：http://baike.zdbjq.cn/Article/details/gyenhdfmt.sHtML

[T16] Swift：Hello World
来源：http://wap.hesvh.cn/Article/details/gcbktufbl.sHtML

print("Hello")
来源：http://mobile.hesvh.cn/Article/details/grhyftsjf.sHtML

[T17] Swift：变量与常量
来源：http://blog.fehbvm.com/Article/details/gzdkijmfx.sHtML

var a = 1;  let b = 2
来源：http://baike.fehbvm.com/Article/details/gldggiukc.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/glapwfkup.sHtML

"值: \(b)"
来源：http://baike.zdbjq.cn/Article/details/guqluytvm.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.zdbjq.cn/Article/details/ggxrdfyeh.sHtML

if let n = opt { print(n) }
来源：http://www.share.zdbjq.cn/Article/details/gjdawsxcy.sHtML

[T20] Swift：数组操作
来源：http://3g.zdbjq.cn/Article/details/gabwdwujq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.zdbjq.cn/Article/details/gatpfmzga.sHtML

[T21] Swift：遍历
来源：http://mobile.hesvh.cn/Article/details/gpbaldkks.sHtML

for x in a { print(x) }
来源：http://read.share.hesvh.cn/Article/details/gnhhuxkvi.sHtML

[T22] Swift：字典
来源：http://wap.hesvh.cn/Article/details/getfptevh.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.hesvh.cn/Article/details/gjtnlkdkk.sHtML

[T23] Swift：函数
来源：http://3g.zdbjq.cn/Article/details/gkvyeaykv.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.hesvh.cn/Article/details/ghsdhzhkz.sHtML

[T24] Swift：闭包
来源：http://www.blog.zdbjq.cn/Article/details/gjhlgfupj.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.zdbjq.cn/Article/details/ghawgoriv.sHtML

[T25] Swift：结构体
来源：http://wap.fehbvm.com/Article/details/gyvdrarmj.sHtML

struct P { var x: Int }
来源：http://mobile.zdbjq.cn/Article/details/gnvafrpba.sHtML

[T26] Swift：类与重写
来源：http://m.share.hesvh.cn/Article/details/grnyglqll.sHtML

class A: Base { override func f() {} }
来源：http://www.share.zdbjq.cn/Article/details/gvteaftke.sHtML

[T27] Swift：错误处理
来源：http://wap.hesvh.cn/Article/details/gavzrzbxc.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.zdbjq.cn/Article/details/gwwdavorx.sHtML

[T28] Swift：枚举
来源：http://www.blog.hesvh.cn/Article/details/gxineocnb.sHtML

enum Color { case red, green }
来源：http://m.share.fehbvm.com/Article/details/gravssbng.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.fehbvm.com/Article/details/gkqkfzujj.sHtML

guard let x = opt else { return }
来源：http://www.share.fehbvm.com/Article/details/gnihqhmii.sHtML

[T30] Swift：协议
来源：http://m.share.fehbvm.com/Article/details/glskopvfl.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.zdbjq.cn/Article/details/gqhgfuvxg.sHtML

[T31] Lua：Hello World
来源：http://read.share.fehbvm.com/Article/details/gsnawazap.sHtML

print("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gedfjguuz.sHtML

[T32] Lua：局部变量
来源：http://blog.hesvh.cn/Article/details/giklkgaks.sHtML

local a = 1
来源：http://3g.hesvh.cn/Article/details/gxbjfglpe.sHtML

[T33] Lua：表（数组）
来源：http://blog.hesvh.cn/Article/details/gollltird.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.hesvh.cn/Article/details/gxagsksro.sHtML

[T34] Lua：遍历表
来源：http://www.share.zdbjq.cn/Article/details/gyzkiavcs.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.fehbvm.com/Article/details/gtvkwnddq.sHtML

[T35] Lua：字典表
来源：http://read.share.hesvh.cn/Article/details/gpcnkorlo.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.zdbjq.cn/Article/details/gzcqmxttk.sHtML

[T36] Lua：函数
来源：http://3g.hesvh.cn/Article/details/gslirbhre.sHtML

function add(a, b) return a + b end
来源：http://m.share.zdbjq.cn/Article/details/gcwgcectv.sHtML

[T37] Lua：字符串拼接
来源：http://3g.hesvh.cn/Article/details/gpllfvskp.sHtML

"a" .. "b"
来源：http://baike.zdbjq.cn/Article/details/gxmdhigqm.sHtML

[T38] Lua：条件
来源：http://www.share.zdbjq.cn/Article/details/ggpltxnpi.sHtML

if x > 0 then print("正") end
来源：http://www.blog.hesvh.cn/Article/details/grjraibbz.sHtML

[T39] Lua：模式匹配
来源：http://m.share.fehbvm.com/Article/details/gjlifbwzf.sHtML

string.find(s, "%d+")
来源：http://www.m.share.hesvh.cn/Article/details/gusdewgnq.sHtML

[T40] Lua：元表
来源：http://blog.zdbjq.cn/Article/details/guguzenaa.sHtML

setmetatable({}, { __index = base })
来源：http://baike.fehbvm.com/Article/details/gvpextfan.sHtML

[T41] Perl：Hello World
来源：http://baike.zdbjq.cn/Article/details/gpcnzrqyd.sHtML

print "Hello\n";
来源：http://blog.zdbjq.cn/Article/details/gqpqdwotb.sHtML

[T42] Perl：变量类型
来源：http://read.share.fehbvm.com/Article/details/gscrijwhk.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.zdbjq.cn/Article/details/gxwdfarqk.sHtML

[T43] Perl：字符串插值
来源：http://3g.fehbvm.com/Article/details/ghvqnfmrc.sHtML

"值: $a"
来源：http://3g.fehbvm.com/Article/details/gnpdralqk.sHtML

[T44] Perl：条件
来源：http://mobile.hesvh.cn/Article/details/gikymojlg.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.hesvh.cn/Article/details/gpwzmrdgx.sHtML

[T45] Perl：数组遍历
来源：http://wap.hesvh.cn/Article/details/gcxdyyslq.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.zdbjq.cn/Article/details/gsoznonix.sHtML

[T46] Perl：哈希操作
来源：http://blog.fehbvm.com/Article/details/gtmqsivtm.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.zdbjq.cn/Article/details/gksupzbhx.sHtML

[T47] Perl：正则捕获
来源：http://3g.hesvh.cn/Article/details/gxeattafw.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.zdbjq.cn/Article/details/gldojnteu.sHtML

[T48] Perl：正则替换
来源：http://wap.zdbjq.cn/Article/details/gajsmfwao.sHtML

$s =~ s/old/new/g;
来源：http://wap.hesvh.cn/Article/details/gjgiotjly.sHtML

[T49] Perl：函数
来源：http://baike.fehbvm.com/Article/details/gowqtvxdf.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gjwzdyoyx.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/glbasvzih.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.zdbjq.cn/Article/details/gvebybhex.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.hesvh.cn/Article/details/gxqxerfuh.sHtML

[T51] Scala：Hello World
来源：http://wap.hesvh.cn/Article/details/gapubbcpt.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/gzxacqzpx.sHtML

[T52] Scala：变量
来源：http://wap.zdbjq.cn/Article/details/gurjbmfxi.sHtML

val a = 1;  var b = 2
来源：http://blog.fehbvm.com/Article/details/gnyohkabh.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/glfeztjjp.sHtML

s"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/gxecfjdae.sHtML

[T54] Scala：集合映射
来源：http://wap.fehbvm.com/Article/details/gbfeounbc.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.hesvh.cn/Article/details/gzkhlfrmq.sHtML

[T55] Scala：集合过滤
来源：http://m.share.hesvh.cn/Article/details/gldyvpztj.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.hesvh.cn/Article/details/ggpzlcsct.sHtML

[T56] Scala：样例类
来源：http://3g.fehbvm.com/Article/details/gcmjvqdqe.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.zdbjq.cn/Article/details/gcmozbvec.sHtML

[T57] Scala：模式匹配
来源：http://wap.hesvh.cn/Article/details/gzywphkrr.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.fehbvm.com/Article/details/gxjaysfad.sHtML

[T58] Scala：函数定义
来源：http://blog.hesvh.cn/Article/details/grjehkjdq.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.hesvh.cn/Article/details/gavjorugi.sHtML

[T59] Scala：循环
来源：http://blog.hesvh.cn/Article/details/glitqlicy.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.zdbjq.cn/Article/details/gmkkljaww.sHtML

[T60] Scala：折叠
来源：http://wap.fehbvm.com/Article/details/gpwgjsmql.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.zdbjq.cn/Article/details/gvscaktva.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gysnbegeu.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.hesvh.cn/Article/details/glexphewn.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/guhmuqpgt.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.hesvh.cn/Article/details/gdfkgfrnw.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.hesvh.cn/Article/details/gjfuruhbv.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.fehbvm.com/Article/details/ggfilprhb.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.zdbjq.cn/Article/details/grxwwzhit.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.fehbvm.com/Article/details/ggykslfvj.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.hesvh.cn/Article/details/gjhlyjush.sHtML

[U04] Py：变量调试打印
来源：http://mobile.hesvh.cn/Article/details/grxeytxbh.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.zdbjq.cn/Article/details/gwbdddwsb.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.fehbvm.com/Article/details/gtkgkljkd.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.hesvh.cn/Article/details/gjcpabuyd.sHtML

[U06] Py：合并两个字典
来源：http://mobile.fehbvm.com/Article/details/gtuxuwxrj.sHtML

{**a, **b}
来源：http://blog.zdbjq.cn/Article/details/gfytcoqix.sHtML

[U07] Py：反转字典键值
来源：http://mobile.hesvh.cn/Article/details/gpvjdotxe.sHtML

{v: k for k, v in d.items()}
来源：http://wap.hesvh.cn/Article/details/gwekqhrnp.sHtML

[U08] Py：展平二维列表
来源：http://read.share.zdbjq.cn/Article/details/gyxtfbpvk.sHtML

[y for x in nested for y in x]
来源：http://baike.zdbjq.cn/Article/details/garyklsvz.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.fehbvm.com/Article/details/gnniymczs.sHtML

max(d, key=d.get)
来源：http://m.share.zdbjq.cn/Article/details/gbcjnutkt.sHtML

[U10] Py：按值排序字典
来源：http://mobile.hesvh.cn/Article/details/gudbbvvhx.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.fehbvm.com/Article/details/gydbgaudi.sHtML

[U11] Py：生成器表达式
来源：http://m.share.fehbvm.com/Article/details/gayyajjlt.sHtML

(x * 2 for x in arr)
来源：http://www.blog.hesvh.cn/Article/details/gyscaxctn.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.fehbvm.com/Article/details/gfljyeiml.sHtML

Counter(arr).most_common(3)
来源：http://mobile.hesvh.cn/Article/details/gvdqmepze.sHtML

[U13] Py：固定长度队列
来源：http://3g.fehbvm.com/Article/details/gurkubddh.sHtML

deque(maxlen=10)
来源：http://blog.zdbjq.cn/Article/details/ggtgvkumv.sHtML

[U14] Py：分组收集到列表
来源：http://blog.fehbvm.com/Article/details/gifqbnqmf.sHtML

defaultdict(list)
来源：http://wap.zdbjq.cn/Article/details/gqvfsnjsm.sHtML

[U15] Py：高精度计时
来源：http://m.share.hesvh.cn/Article/details/gdumwrtxg.sHtML

t = time.perf_counter()
来源：http://wap.hesvh.cn/Article/details/gmkdlxuqw.sHtML

[U16] Py：命令行参数解析
来源：http://baike.hesvh.cn/Article/details/gjqlrbphd.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.zdbjq.cn/Article/details/gurdepyty.sHtML

[U17] Py：初始化日志
来源：http://read.share.zdbjq.cn/Article/details/gmjzewfzs.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.hesvh.cn/Article/details/grqwycqmf.sHtML

[U18] Py：预编译正则
来源：http://www.blog.zdbjq.cn/Article/details/gtdbppkkz.sHtML

pat = re.compile(r"\d+")
来源：http://blog.zdbjq.cn/Article/details/gxwoolpzu.sHtML

[U19] Py：正则替换带回调
来源：http://3g.hesvh.cn/Article/details/ghypmpgdn.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.fehbvm.com/Article/details/gxbfznnop.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.hesvh.cn/Article/details/glfkatgfk.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.zdbjq.cn/Article/details/gkemdpxwy.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.zdbjq.cn/Article/details/grrkrgnik.sHtML

@contextlib.contextmanager
来源：http://3g.fehbvm.com/Article/details/gsspmnyzi.sHtML

[U22] Py：矩阵转置
来源：http://wap.zdbjq.cn/Article/details/gbafzrrzt.sHtML

list(zip(*m))
来源：http://3g.fehbvm.com/Article/details/gjkmvmfrz.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.hesvh.cn/Article/details/gjkyhewku.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.zdbjq.cn/Article/details/gybgsxygl.sHtML

[U24] Py：路径操作
来源：http://www.share.hesvh.cn/Article/details/gqkmtmowp.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.hesvh.cn/Article/details/gfexfvjmt.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.hesvh.cn/Article/details/gmybnbged.sHtML

csv.DictReader(f)
来源：http://baike.zdbjq.cn/Article/details/guhoraufs.sHtML

[U26] Py：并发下载
来源：http://read.share.fehbvm.com/Article/details/gylcssoko.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.hesvh.cn/Article/details/gtqcxdexy.sHtML

[U27] Py：异步 HTTP
来源：http://3g.zdbjq.cn/Article/details/gygfzmmxh.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.hesvh.cn/Article/details/gufdbcooz.sHtML

[U28] Py：类型别名
来源：http://mobile.zdbjq.cn/Article/details/gwcryqnzk.sHtML

UserId = int
来源：http://m.share.fehbvm.com/Article/details/gwiuitjwl.sHtML

[U29] Py：属性校验
来源：http://www.share.fehbvm.com/Article/details/gipyztyya.sHtML

@property 与 @x.setter 配合
来源：http://read.share.fehbvm.com/Article/details/gwhihikqt.sHtML

[U30] Py：数据类
来源：http://wap.hesvh.cn/Article/details/gzepatuqv.sHtML

@dataclass(slots=True)
来源：http://baike.hesvh.cn/Article/details/gilypdvlj.sHtML

[U31] Py：单测
来源：http://mobile.zdbjq.cn/Article/details/getrlrjxn.sHtML

python -m pytest -q
来源：http://www.blog.fehbvm.com/Article/details/ggsdyphiy.sHtML

[U32] Py：代码格式化
来源：http://www.share.hesvh.cn/Article/details/gesrwvkup.sHtML

ruff format . && ruff check --fix .
来源：http://wap.fehbvm.com/Article/details/gvucrafbf.sHtML

[U33] Py：打包发布
来源：http://www.blog.zdbjq.cn/Article/details/gsefkhvbw.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.hesvh.cn/Article/details/ggidbyola.sHtML

[U34] Py：判断编码
来源：http://www.share.zdbjq.cn/Article/details/glarbjaez.sHtML

chardet.detect(raw)
来源：http://www.m.share.zdbjq.cn/Article/details/gvsqluyms.sHtML

[U35] Py：发送邮件
来源：http://www.share.zdbjq.cn/Article/details/ggegxmbpf.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.fehbvm.com/Article/details/gkbsxfarh.sHtML

[U36] Py：定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/gxeerosoq.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.fehbvm.com/Article/details/gsrvavrpp.sHtML

[U37] Py：读写 Excel
来源：http://mobile.hesvh.cn/Article/details/gnvayhndu.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.fehbvm.com/Article/details/goemhoviz.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.fehbvm.com/Article/details/gikgbqrnt.sHtML

Path(__file__).resolve().parent
来源：http://3g.fehbvm.com/Article/details/gvuhzvuue.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.zdbjq.cn/Article/details/gabtjoovj.sHtML

sys.stdout.isatty()
来源：http://wap.fehbvm.com/Article/details/gwoxufcbz.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.fehbvm.com/Article/details/gtecmcozx.sHtML

print("err", file=sys.stderr)
来源：http://read.share.zdbjq.cn/Article/details/gmgixojsf.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.hesvh.cn/Article/details/gfldcxtjc.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.zdbjq.cn/Article/details/gyjbwaqcw.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.hesvh.cn/Article/details/goumyhgwp.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.hesvh.cn/Article/details/gqqkmzwew.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.hesvh.cn/Article/details/gbsqrmnty.sHtML

namespace App\Http;
来源：http://www.m.share.zdbjq.cn/Article/details/gscjitmxe.sHtML

[U44] PHP：开启严格类型
来源：http://wap.hesvh.cn/Article/details/ghosmvjxq.sHtML

declare(strict_types=1);
来源：http://mobile.fehbvm.com/Article/details/gbeekwgro.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.zdbjq.cn/Article/details/gpcssopem.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gpledfisf.sHtML

[U46] PHP：可空类型
来源：http://wap.hesvh.cn/Article/details/guuqnbowq.sHtML

?string $name = null
来源：http://www.share.zdbjq.cn/Article/details/gaweyxqxl.sHtML

[U47] PHP：联合类型
来源：http://blog.fehbvm.com/Article/details/ghrmcdbbm.sHtML

int|string $id
来源：http://wap.fehbvm.com/Article/details/gghmplbgp.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.hesvh.cn/Article/details/gozjsalpl.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.fehbvm.com/Article/details/gqtbisney.sHtML

[U49] PHP：只读属性
来源：http://read.share.zdbjq.cn/Article/details/gazplxnoz.sHtML

public readonly string $name
来源：http://wap.zdbjq.cn/Article/details/gdsznfrcw.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.zdbjq.cn/Article/details/gaplggfyj.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.zdbjq.cn/Article/details/ghyzaqwzw.sHtML

[U51] PHP：数组解构
来源：http://www.blog.zdbjq.cn/Article/details/gcyybsctz.sHtML

[$a, $b] = $arr;
来源：http://mobile.fehbvm.com/Article/details/glctdnatn.sHtML

[U52] PHP：箭头函数
来源：http://wap.hesvh.cn/Article/details/gwfaixynh.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.hesvh.cn/Article/details/gsputwncn.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.fehbvm.com/Article/details/glcannkml.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.zdbjq.cn/Article/details/gjsmkzvbh.sHtML

[U54] PHP：空安全调用
来源：http://3g.zdbjq.cn/Article/details/gqvrkilry.sHtML

$obj?->method()
来源：http://3g.fehbvm.com/Article/details/gzrrahimq.sHtML

[U55] PHP：match 表达式
来源：http://www.share.hesvh.cn/Article/details/gzcmycuww.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.zdbjq.cn/Article/details/gllxieqhv.sHtML

[U56] PHP：命名参数
来源：http://blog.fehbvm.com/Article/details/gfwcxjtce.sHtML

f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/gemzpgjpr.sHtML

[U57] PHP：字符串插值
来源：http://baike.zdbjq.cn/Article/details/ghaetetdg.sHtML

"值: {$a}"
来源：http://www.share.zdbjq.cn/Article/details/gmqacdoqx.sHtML

[U58] PHP：数组三件套
来源：http://3g.fehbvm.com/Article/details/gwbbkpkin.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.fehbvm.com/Article/details/gpvlamfvv.sHtML

[U59] PHP：自定义排序
来源：http://read.share.zdbjq.cn/Article/details/gtavovjwg.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.zdbjq.cn/Article/details/gpaskscrc.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.zdbjq.cn/Article/details/gaoolfkuh.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.hesvh.cn/Article/details/guuxqllpf.sHtML

[U61] PHP：正则
来源：http://www.share.zdbjq.cn/Article/details/goqfcobys.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.hesvh.cn/Article/details/grxkavvcm.sHtML

[U62] PHP：日期对象
来源：http://baike.zdbjq.cn/Article/details/gwqqnwfdl.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.zdbjq.cn/Article/details/gwxhvpkhs.sHtML

[U63] PHP：文件读写
来源：http://baike.hesvh.cn/Article/details/gdyhfflqh.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.fehbvm.com/Article/details/gljewaffb.sHtML

[U64] PHP：目录遍历
来源：http://www.share.zdbjq.cn/Article/details/grzccwiot.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.hesvh.cn/Article/details/ghxjewihr.sHtML

[U65] PHP：会话
来源：http://www.share.hesvh.cn/Article/details/ggtijxomb.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gosytgrtq.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.zdbjq.cn/Article/details/gchgwflbb.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.hesvh.cn/Article/details/gyymahhkb.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.zdbjq.cn/Article/details/glqglbwsf.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.hesvh.cn/Article/details/goybjoueq.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.hesvh.cn/Article/details/gbrfnmgmm.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.hesvh.cn/Article/details/gzmapsyqu.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.zdbjq.cn/Article/details/gdaewpjex.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.hesvh.cn/Article/details/gotfomgnq.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.zdbjq.cn/Article/details/gekerzqqb.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.zdbjq.cn/Article/details/gyxtzlfje.sHtML

[U71] PHP：抛出异常
来源：http://wap.zdbjq.cn/Article/details/gfwuffqqj.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.zdbjq.cn/Article/details/gnjxstjcs.sHtML

[U72] PHP：写错误日志
来源：http://blog.fehbvm.com/Article/details/gaqlkuqku.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.fehbvm.com/Article/details/gmwqeqoyz.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.fehbvm.com/Article/details/gghqgwmwm.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.fehbvm.com/Article/details/gciedlpib.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.hesvh.cn/Article/details/gfiuswbvg.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.zdbjq.cn/Article/details/gfwtyblha.sHtML

[U75] PHP：依赖注入
来源：http://3g.zdbjq.cn/Article/details/gstzyelmr.sHtML

composer require psr/container
来源：http://wap.fehbvm.com/Article/details/gyujmsqyb.sHtML

[U76] PHP：简单路由
来源：http://wap.hesvh.cn/Article/details/gebayiyki.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.fehbvm.com/Article/details/gdagvnmdg.sHtML

[U77] PHP：模板渲染
来源：http://3g.hesvh.cn/Article/details/gmrepjabf.sHtML

composer require twig/twig
来源：http://mobile.zdbjq.cn/Article/details/guovxldsr.sHtML

[U78] PHP：单元测试
来源：http://3g.zdbjq.cn/Article/details/gfrrbrtrp.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.fehbvm.com/Article/details/gbhboyfuh.sHtML

[U79] PHP：静态分析
来源：http://m.share.hesvh.cn/Article/details/gwpdfbvuv.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.fehbvm.com/Article/details/grrriesyw.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.fehbvm.com/Article/details/gserhshpf.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.zdbjq.cn/Article/details/gbocstryl.sHtML

[U81] JS：初始化项目
来源：http://wap.hesvh.cn/Article/details/gpuaqmhpa.sHtML

npm init -y;  npm i express
来源：http://blog.hesvh.cn/Article/details/gitjitkkm.sHtML

[U82] JS：package.json 脚本
来源：http://blog.zdbjq.cn/Article/details/gvspepztp.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.fehbvm.com/Article/details/gndnlwnhz.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.zdbjq.cn/Article/details/goqsrrimb.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.zdbjq.cn/Article/details/gtnlunfvp.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.zdbjq.cn/Article/details/gkhmshcqd.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.hesvh.cn/Article/details/gkwjklmrn.sHtML

[U85] JS：可选链
来源：http://baike.hesvh.cn/Article/details/gohrcfkfi.sHtML

a?.b?.c
来源：http://www.share.fehbvm.com/Article/details/goubuhvsp.sHtML

[U86] JS：空值合并
来源：http://blog.fehbvm.com/Article/details/gwtwqyfqh.sHtML

a ?? b
来源：http://www.blog.fehbvm.com/Article/details/glhmeyjuy.sHtML

[U87] JS：解构默认值
来源：http://read.share.zdbjq.cn/Article/details/gcmjzrjmm.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.zdbjq.cn/Article/details/goxnbofzt.sHtML

[U88] JS：对象展开合并
来源：http://wap.hesvh.cn/Article/details/gbwpemzoy.sHtML

{ ...a, ...b }
来源：http://www.share.zdbjq.cn/Article/details/gtspejdkp.sHtML

[U89] JS：数组去重
来源：http://baike.zdbjq.cn/Article/details/gwzllzcdg.sHtML

[...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/gtceykclg.sHtML

[U90] JS：数字数组排序
来源：http://wap.fehbvm.com/Article/details/gaoezmjkh.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/glladhvfw.sHtML

[U91] JS：对象键值遍历
来源：http://baike.hesvh.cn/Article/details/gjthppvzf.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.zdbjq.cn/Article/details/gzpldqgtk.sHtML

[U92] JS：深拷贝
来源：http://m.share.zdbjq.cn/Article/details/gzmpkivwy.sHtML

structuredClone(obj)
来源：http://read.share.fehbvm.com/Article/details/gwwqqnikt.sHtML


<!-- 参考信息 -->