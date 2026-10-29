代发 wailian999

[T07] Kotlin：集合过滤
来源：http://m.share.zdbjq.cn/Article/details/gxtnzraap.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.zdbjq.cn/Article/details/gbkgkwnlq.sHtML

[T08] Kotlin：数据类
来源：http://3g.zdbjq.cn/Article/details/gslylfoql.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fehbvm.com/Article/details/gcsttpuxq.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fehbvm.com/Article/details/gydcghqqb.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fehbvm.com/Article/details/gxdybuaba.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.hesvh.cn/Article/details/ggnlgohsf.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.zdbjq.cn/Article/details/grbbhteuh.sHtML

[T11] Kotlin：协程
来源：http://mobile.fehbvm.com/Article/details/grkltztmd.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.hesvh.cn/Article/details/gsvfwbonb.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fehbvm.com/Article/details/gzsfplxmd.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gtpaofkke.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fehbvm.com/Article/details/gqbotwpng.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.hesvh.cn/Article/details/geypducay.sHtML

[T14] Kotlin：循环
来源：http://baike.hesvh.cn/Article/details/gebpcjntn.sHtML

for (i in 1..10) println(i)
来源：http://mobile.zdbjq.cn/Article/details/gbpvgiavw.sHtML

[T15] Kotlin：接口
来源：http://baike.fehbvm.com/Article/details/gsjnsotfz.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.zdbjq.cn/Article/details/gspxqmfko.sHtML

[T16] Swift：Hello World
来源：http://baike.hesvh.cn/Article/details/gklalxsxp.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/gqdqfjnqg.sHtML

[T17] Swift：变量与常量
来源：http://baike.zdbjq.cn/Article/details/gdjdkfzoz.sHtML

var a = 1;  let b = 2
来源：http://read.share.fehbvm.com/Article/details/gvmoeiney.sHtML

[T18] Swift：字符串插值
来源：http://www.share.hesvh.cn/Article/details/glvyylmka.sHtML

"值: \(b)"
来源：http://blog.zdbjq.cn/Article/details/gqatzzpxn.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fehbvm.com/Article/details/gquuvfbpy.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.fehbvm.com/Article/details/gwcwvlaeq.sHtML

[T20] Swift：数组操作
来源：http://read.share.zdbjq.cn/Article/details/gtuvuwvkd.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.zdbjq.cn/Article/details/gtdgnjxih.sHtML

[T21] Swift：遍历
来源：http://mobile.zdbjq.cn/Article/details/gvloohfst.sHtML

for x in a { print(x) }
来源：http://mobile.fehbvm.com/Article/details/gymjsgecp.sHtML

[T22] Swift：字典
来源：http://blog.fehbvm.com/Article/details/gydkfizaj.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fehbvm.com/Article/details/goxzuagck.sHtML

[T23] Swift：函数
来源：http://m.share.hesvh.cn/Article/details/gpgdtshfz.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.zdbjq.cn/Article/details/giwmnvqcl.sHtML

[T24] Swift：闭包
来源：http://3g.fehbvm.com/Article/details/gvoirajvp.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gtuhlkbom.sHtML

[T25] Swift：结构体
来源：http://wap.fehbvm.com/Article/details/gyfvhhbmr.sHtML

struct P { var x: Int }
来源：http://www.share.fehbvm.com/Article/details/gnetfdscr.sHtML

[T26] Swift：类与重写
来源：http://baike.fehbvm.com/Article/details/gsxwrvncx.sHtML

class A: Base { override func f() {} }
来源：http://3g.fehbvm.com/Article/details/gcfyzvvwl.sHtML

[T27] Swift：错误处理
来源：http://read.share.zdbjq.cn/Article/details/gurcymvme.sHtML

do { try f() } catch { print(error) }
来源：http://baike.fehbvm.com/Article/details/gulxdfqjx.sHtML

[T28] Swift：枚举
来源：http://m.share.hesvh.cn/Article/details/ggfvxvheu.sHtML

enum Color { case red, green }
来源：http://wap.zdbjq.cn/Article/details/gpbbaqbll.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.hesvh.cn/Article/details/ghftqozgq.sHtML

guard let x = opt else { return }
来源：http://read.share.fehbvm.com/Article/details/gmxknkzdp.sHtML

[T30] Swift：协议
来源：http://www.m.share.fehbvm.com/Article/details/gzbglxjqh.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.zdbjq.cn/Article/details/gkygrjkgo.sHtML

[T31] Lua：Hello World
来源：http://baike.zdbjq.cn/Article/details/gskpthtsq.sHtML

print("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gyxyjxrwl.sHtML

[T32] Lua：局部变量
来源：http://mobile.zdbjq.cn/Article/details/gybbwcjjw.sHtML

local a = 1
来源：http://www.blog.zdbjq.cn/Article/details/gwrclpwhn.sHtML

[T33] Lua：表（数组）
来源：http://mobile.hesvh.cn/Article/details/gjgxmtsox.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.zdbjq.cn/Article/details/gabxczdlb.sHtML

[T34] Lua：遍历表
来源：http://wap.fehbvm.com/Article/details/glfagzuag.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.hesvh.cn/Article/details/genvojjhs.sHtML

[T35] Lua：字典表
来源：http://www.m.share.zdbjq.cn/Article/details/gynjquzvh.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.hesvh.cn/Article/details/ggwwqqueb.sHtML

[T36] Lua：函数
来源：http://m.share.zdbjq.cn/Article/details/gnjonlpsa.sHtML

function add(a, b) return a + b end
来源：http://wap.zdbjq.cn/Article/details/gikokypzj.sHtML

[T37] Lua：字符串拼接
来源：http://3g.zdbjq.cn/Article/details/gteltyjvn.sHtML

"a" .. "b"
来源：http://blog.hesvh.cn/Article/details/gaddhzffo.sHtML

[T38] Lua：条件
来源：http://mobile.hesvh.cn/Article/details/gkxzdukjz.sHtML

if x > 0 then print("正") end
来源：http://read.share.fehbvm.com/Article/details/gdlnyjjzq.sHtML

[T39] Lua：模式匹配
来源：http://read.share.hesvh.cn/Article/details/gqoniwhmf.sHtML

string.find(s, "%d+")
来源：http://3g.zdbjq.cn/Article/details/gdgrvhmoa.sHtML

[T40] Lua：元表
来源：http://baike.fehbvm.com/Article/details/gpoxglpkd.sHtML

setmetatable({}, { __index = base })
来源：http://baike.zdbjq.cn/Article/details/gjhiygcud.sHtML

[T41] Perl：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gtwejenwn.sHtML

print "Hello\n";
来源：http://m.share.hesvh.cn/Article/details/gtsgjhppk.sHtML

[T42] Perl：变量类型
来源：http://baike.hesvh.cn/Article/details/gnjfqarpj.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.fehbvm.com/Article/details/gtgqdozsw.sHtML

[T43] Perl：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gwcuoldrm.sHtML

"值: $a"
来源：http://mobile.fehbvm.com/Article/details/gnuovzqbj.sHtML

[T44] Perl：条件
来源：http://read.share.fehbvm.com/Article/details/gmxexgjyu.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.hesvh.cn/Article/details/gvmkgrxzb.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gevuvuisu.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.zdbjq.cn/Article/details/glyqmxzlu.sHtML

[T46] Perl：哈希操作
来源：http://3g.fehbvm.com/Article/details/glbuwubyh.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.fehbvm.com/Article/details/gemiahrfy.sHtML

[T47] Perl：正则捕获
来源：http://wap.hesvh.cn/Article/details/gcvsvbtht.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.fehbvm.com/Article/details/gftcqtaao.sHtML

[T48] Perl：正则替换
来源：http://baike.zdbjq.cn/Article/details/ggaifaapt.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.zdbjq.cn/Article/details/gtqzrnvdk.sHtML

[T49] Perl：函数
来源：http://baike.zdbjq.cn/Article/details/ggfrnmrkt.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gezkwkcmy.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gsbhzydeq.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.zdbjq.cn/Article/details/ggyvodpik.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.fehbvm.com/Article/details/gvvrlveps.sHtML

[T51] Scala：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gepvockww.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/gpttykkdp.sHtML

[T52] Scala：变量
来源：http://wap.hesvh.cn/Article/details/gbvarfpum.sHtML

val a = 1;  var b = 2
来源：http://wap.hesvh.cn/Article/details/gxiwzmwuu.sHtML

[T53] Scala：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gipfkfunf.sHtML

s"值: $b"
来源：http://3g.hesvh.cn/Article/details/gtjwrrtqw.sHtML

[T54] Scala：集合映射
来源：http://wap.zdbjq.cn/Article/details/gxsmtakke.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.fehbvm.com/Article/details/gjgsmognj.sHtML

[T55] Scala：集合过滤
来源：http://mobile.hesvh.cn/Article/details/gvfmgufcm.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.hesvh.cn/Article/details/gsedkmpuh.sHtML

[T56] Scala：样例类
来源：http://www.blog.zdbjq.cn/Article/details/gduizmjac.sHtML

case class User(name: String, age: Int)
来源：http://blog.fehbvm.com/Article/details/ggdrcuitj.sHtML

[T57] Scala：模式匹配
来源：http://wap.hesvh.cn/Article/details/ghfmzklgy.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.fehbvm.com/Article/details/ghrgmevmb.sHtML

[T58] Scala：函数定义
来源：http://m.share.fehbvm.com/Article/details/gehrdpduc.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.zdbjq.cn/Article/details/ghdfiefiy.sHtML

[T59] Scala：循环
来源：http://m.share.zdbjq.cn/Article/details/godvuxfbr.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/gxedxtqhr.sHtML

[T60] Scala：折叠
来源：http://m.share.hesvh.cn/Article/details/gwsnoting.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.hesvh.cn/Article/details/gucmwfkzs.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gfxlcfauu.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.zdbjq.cn/Article/details/gcvpyxbpa.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gwzeatehc.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.zdbjq.cn/Article/details/gwlwwhxtd.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.hesvh.cn/Article/details/glnhjlqjv.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.hesvh.cn/Article/details/geuurspwg.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.hesvh.cn/Article/details/gnfvjrzoy.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.fehbvm.com/Article/details/gorkgncrn.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.zdbjq.cn/Article/details/gyfebidxf.sHtML

[U04] Py：变量调试打印
来源：http://3g.zdbjq.cn/Article/details/gidibxrwh.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.zdbjq.cn/Article/details/gqgaezsmy.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.hesvh.cn/Article/details/gbrkyuase.sHtML

list(dict.fromkeys(arr))
来源：http://blog.fehbvm.com/Article/details/goyhqzxsm.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.zdbjq.cn/Article/details/gqvooqiod.sHtML

{**a, **b}
来源：http://m.share.hesvh.cn/Article/details/gslipxsgb.sHtML

[U07] Py：反转字典键值
来源：http://m.share.zdbjq.cn/Article/details/gluuzecue.sHtML

{v: k for k, v in d.items()}
来源：http://blog.hesvh.cn/Article/details/gvbcziazm.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.hesvh.cn/Article/details/gqnhdyooj.sHtML

[y for x in nested for y in x]
来源：http://3g.hesvh.cn/Article/details/ghuyodmvh.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.zdbjq.cn/Article/details/gsqivbrjc.sHtML

max(d, key=d.get)
来源：http://mobile.fehbvm.com/Article/details/gqgngaasg.sHtML

[U10] Py：按值排序字典
来源：http://wap.hesvh.cn/Article/details/gknwwmuso.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.hesvh.cn/Article/details/grekqpugg.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gfkjcofll.sHtML

(x * 2 for x in arr)
来源：http://read.share.fehbvm.com/Article/details/gzyvjxiqu.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.zdbjq.cn/Article/details/gsxzqfkvy.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.zdbjq.cn/Article/details/gzrnfmxzt.sHtML

[U13] Py：固定长度队列
来源：http://baike.hesvh.cn/Article/details/gisklgjyt.sHtML

deque(maxlen=10)
来源：http://mobile.fehbvm.com/Article/details/gmfjuacxg.sHtML

[U14] Py：分组收集到列表
来源：http://wap.zdbjq.cn/Article/details/gngbmcdfz.sHtML

defaultdict(list)
来源：http://mobile.hesvh.cn/Article/details/gfijgdofu.sHtML

[U15] Py：高精度计时
来源：http://mobile.fehbvm.com/Article/details/geqskzoac.sHtML

t = time.perf_counter()
来源：http://www.blog.zdbjq.cn/Article/details/gshxzfnpm.sHtML

[U16] Py：命令行参数解析
来源：http://3g.fehbvm.com/Article/details/glmcwbxio.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.fehbvm.com/Article/details/geovtwsbh.sHtML

[U17] Py：初始化日志
来源：http://mobile.fehbvm.com/Article/details/ganqyatbf.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.zdbjq.cn/Article/details/gokcgxbdj.sHtML

[U18] Py：预编译正则
来源：http://www.blog.zdbjq.cn/Article/details/grgnkaoia.sHtML

pat = re.compile(r"\d+")
来源：http://wap.zdbjq.cn/Article/details/grtevifsp.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.zdbjq.cn/Article/details/gncuvyhko.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.hesvh.cn/Article/details/gfyeqzgpd.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.hesvh.cn/Article/details/gomxiutje.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.zdbjq.cn/Article/details/gwbujqnzp.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.zdbjq.cn/Article/details/ganttstmq.sHtML

@contextlib.contextmanager
来源：http://blog.fehbvm.com/Article/details/gmfasalpt.sHtML

[U22] Py：矩阵转置
来源：http://m.share.zdbjq.cn/Article/details/gewmjfswc.sHtML

list(zip(*m))
来源：http://3g.fehbvm.com/Article/details/ggjkjmjqo.sHtML

[U23] Py：分块读取大文件
来源：http://wap.fehbvm.com/Article/details/grtcezaqt.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.hesvh.cn/Article/details/gkvgghjcz.sHtML

[U24] Py：路径操作
来源：http://www.m.share.fehbvm.com/Article/details/gyetfpfiz.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.fehbvm.com/Article/details/gihiwbqny.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.fehbvm.com/Article/details/gqqwxikta.sHtML

csv.DictReader(f)
来源：http://blog.fehbvm.com/Article/details/gkrbvsosq.sHtML

[U26] Py：并发下载
来源：http://www.share.hesvh.cn/Article/details/gcqeschwh.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.hesvh.cn/Article/details/gkxvribzb.sHtML

[U27] Py：异步 HTTP
来源：http://wap.fehbvm.com/Article/details/gvkelinnk.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.hesvh.cn/Article/details/gthdufbyo.sHtML

[U28] Py：类型别名
来源：http://m.share.zdbjq.cn/Article/details/gtrtyfmqh.sHtML

UserId = int
来源：http://blog.zdbjq.cn/Article/details/ggmgbyoke.sHtML

[U29] Py：属性校验
来源：http://www.share.zdbjq.cn/Article/details/gatfajcgk.sHtML

@property 与 @x.setter 配合
来源：http://www.share.zdbjq.cn/Article/details/gnxplusbs.sHtML

[U30] Py：数据类
来源：http://mobile.hesvh.cn/Article/details/goaeiqexo.sHtML

@dataclass(slots=True)
来源：http://mobile.zdbjq.cn/Article/details/gnjajxbyo.sHtML

[U31] Py：单测
来源：http://wap.hesvh.cn/Article/details/gcntirpam.sHtML

python -m pytest -q
来源：http://mobile.fehbvm.com/Article/details/gtqnqfbbt.sHtML

[U32] Py：代码格式化
来源：http://read.share.hesvh.cn/Article/details/gbnxbzjbx.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.zdbjq.cn/Article/details/gzgrjchzn.sHtML

[U33] Py：打包发布
来源：http://read.share.hesvh.cn/Article/details/ghssrhbmq.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.fehbvm.com/Article/details/gicmrefff.sHtML

[U34] Py：判断编码
来源：http://www.blog.zdbjq.cn/Article/details/gzrexnecj.sHtML

chardet.detect(raw)
来源：http://mobile.hesvh.cn/Article/details/grkiodspf.sHtML

[U35] Py：发送邮件
来源：http://mobile.zdbjq.cn/Article/details/getarbsfi.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.hesvh.cn/Article/details/gymrnevlx.sHtML

[U36] Py：定时任务
来源：http://www.blog.hesvh.cn/Article/details/gchsmwwax.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.zdbjq.cn/Article/details/gbeoapkwr.sHtML

[U37] Py：读写 Excel
来源：http://read.share.hesvh.cn/Article/details/gtiblxqsr.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.hesvh.cn/Article/details/gmfodkzdk.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.fehbvm.com/Article/details/gfayoeurs.sHtML

Path(__file__).resolve().parent
来源：http://read.share.fehbvm.com/Article/details/gglgmfidd.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.fehbvm.com/Article/details/gtozwuibd.sHtML

sys.stdout.isatty()
来源：http://baike.zdbjq.cn/Article/details/gndtrgpay.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.hesvh.cn/Article/details/gaqqprnyo.sHtML

print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/ghowofupa.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.hesvh.cn/Article/details/gpiuydsly.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.fehbvm.com/Article/details/gtpvbusry.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.zdbjq.cn/Article/details/gzrpbimvd.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.hesvh.cn/Article/details/gscjdzobe.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.hesvh.cn/Article/details/gecaygzsh.sHtML

namespace App\Http;
来源：http://mobile.zdbjq.cn/Article/details/guzniqsnl.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.hesvh.cn/Article/details/gdzemxzdg.sHtML

declare(strict_types=1);
来源：http://blog.hesvh.cn/Article/details/gbupifyhq.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.fehbvm.com/Article/details/gnrxyakib.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gpksrfwav.sHtML

[U46] PHP：可空类型
来源：http://blog.zdbjq.cn/Article/details/gjrjtivyk.sHtML

?string $name = null
来源：http://read.share.hesvh.cn/Article/details/gfadautvr.sHtML

[U47] PHP：联合类型
来源：http://mobile.fehbvm.com/Article/details/glekoszqw.sHtML

int|string $id
来源：http://3g.zdbjq.cn/Article/details/gioxjmkrx.sHtML

[U48] PHP：纯枚举
来源：http://3g.fehbvm.com/Article/details/gmltaeibl.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.hesvh.cn/Article/details/goawfgyks.sHtML

[U49] PHP：只读属性
来源：http://wap.hesvh.cn/Article/details/gkasbxjvr.sHtML

public readonly string $name
来源：http://blog.fehbvm.com/Article/details/gtwnzwvrr.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.fehbvm.com/Article/details/gvyviwoke.sHtML

public function __construct(private int $id) {}
来源：http://read.share.zdbjq.cn/Article/details/gdsjwbwgp.sHtML

[U51] PHP：数组解构
来源：http://www.blog.zdbjq.cn/Article/details/gyiakondb.sHtML

[$a, $b] = $arr;
来源：http://www.share.fehbvm.com/Article/details/gwajnuhxv.sHtML

[U52] PHP：箭头函数
来源：http://m.share.fehbvm.com/Article/details/gzvwyblvv.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.hesvh.cn/Article/details/gpqceagpa.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.zdbjq.cn/Article/details/geksijwgu.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.hesvh.cn/Article/details/gdxyenkey.sHtML

[U54] PHP：空安全调用
来源：http://wap.fehbvm.com/Article/details/gfzljrbip.sHtML

$obj?->method()
来源：http://wap.fehbvm.com/Article/details/gpklxwhho.sHtML

[U55] PHP：match 表达式
来源：http://read.share.fehbvm.com/Article/details/ggywrksoc.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.zdbjq.cn/Article/details/ggdozwolk.sHtML

[U56] PHP：命名参数
来源：http://www.blog.zdbjq.cn/Article/details/gqukficey.sHtML

f(a: 1, b: 2)
来源：http://baike.zdbjq.cn/Article/details/gvvdjgroo.sHtML

[U57] PHP：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gdfcfafgp.sHtML

"值: {$a}"
来源：http://baike.hesvh.cn/Article/details/glbxnoizj.sHtML

[U58] PHP：数组三件套
来源：http://m.share.hesvh.cn/Article/details/gqjfiacrt.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.zdbjq.cn/Article/details/gjuhyehbp.sHtML

[U59] PHP：自定义排序
来源：http://m.share.fehbvm.com/Article/details/gslxeavnw.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.hesvh.cn/Article/details/gjpkfhixk.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.zdbjq.cn/Article/details/goqjimtnp.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.hesvh.cn/Article/details/gfhojcubq.sHtML

[U61] PHP：正则
来源：http://mobile.hesvh.cn/Article/details/gqhalxgtx.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.fehbvm.com/Article/details/gwsnxesxv.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.fehbvm.com/Article/details/gybkiycft.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.zdbjq.cn/Article/details/gcgtfdoyw.sHtML

[U63] PHP：文件读写
来源：http://3g.zdbjq.cn/Article/details/gbolrohcj.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.hesvh.cn/Article/details/gkdnbhboz.sHtML

[U64] PHP：目录遍历
来源：http://www.share.hesvh.cn/Article/details/ghnmcwxar.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.zdbjq.cn/Article/details/gokuudufp.sHtML

[U65] PHP：会话
来源：http://read.share.fehbvm.com/Article/details/gudhemviu.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.hesvh.cn/Article/details/ggcvhczhp.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.fehbvm.com/Article/details/gmdpyujbo.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.fehbvm.com/Article/details/gbgkfkafg.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.fehbvm.com/Article/details/gfjzqzarg.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.zdbjq.cn/Article/details/goutbtzbi.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.fehbvm.com/Article/details/glizuklmw.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.zdbjq.cn/Article/details/gghoomley.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.hesvh.cn/Article/details/gcchagpum.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.fehbvm.com/Article/details/gexrhaqck.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.fehbvm.com/Article/details/gtgxvclre.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.zdbjq.cn/Article/details/glyihfvll.sHtML

[U71] PHP：抛出异常
来源：http://mobile.hesvh.cn/Article/details/gphvfnftn.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.zdbjq.cn/Article/details/gjawphdlu.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.fehbvm.com/Article/details/gxluqmcjd.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.fehbvm.com/Article/details/gnjolnakd.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.fehbvm.com/Article/details/giimcnhar.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.zdbjq.cn/Article/details/gvbymlwyd.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.zdbjq.cn/Article/details/gjlwbqllh.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.fehbvm.com/Article/details/gttxgqbgh.sHtML

[U75] PHP：依赖注入
来源：http://m.share.fehbvm.com/Article/details/gxditgyrt.sHtML

composer require psr/container
来源：http://m.share.hesvh.cn/Article/details/gvydnlzoo.sHtML

[U76] PHP：简单路由
来源：http://mobile.zdbjq.cn/Article/details/gblikbylb.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.hesvh.cn/Article/details/gttcghviu.sHtML

[U77] PHP：模板渲染
来源：http://mobile.hesvh.cn/Article/details/ghdbauesi.sHtML

composer require twig/twig
来源：http://www.share.hesvh.cn/Article/details/gjmtoydzf.sHtML

[U78] PHP：单元测试
来源：http://3g.hesvh.cn/Article/details/gkylywrco.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.fehbvm.com/Article/details/gbkbtfujc.sHtML

[U79] PHP：静态分析
来源：http://mobile.hesvh.cn/Article/details/gyrdbiogw.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.fehbvm.com/Article/details/gssozjdbj.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.fehbvm.com/Article/details/gttnavaft.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.fehbvm.com/Article/details/gyatalwom.sHtML

[U81] JS：初始化项目
来源：http://m.share.zdbjq.cn/Article/details/gjgedkpnp.sHtML

npm init -y;  npm i express
来源：http://mobile.hesvh.cn/Article/details/grnzpncts.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.zdbjq.cn/Article/details/gtrjunmtr.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.hesvh.cn/Article/details/gtxjxflbx.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.hesvh.cn/Article/details/gxjuvgkqp.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.hesvh.cn/Article/details/gplroaiaf.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.zdbjq.cn/Article/details/ghkeovjgp.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.hesvh.cn/Article/details/gqgetbrmo.sHtML

[U85] JS：可选链
来源：http://wap.zdbjq.cn/Article/details/gfhmvpaje.sHtML

a?.b?.c
来源：http://baike.fehbvm.com/Article/details/gytnveaif.sHtML

[U86] JS：空值合并
来源：http://3g.fehbvm.com/Article/details/glzuhpqxw.sHtML

a ?? b
来源：http://www.blog.hesvh.cn/Article/details/gelnlrbki.sHtML

[U87] JS：解构默认值
来源：http://mobile.hesvh.cn/Article/details/ghtqjukir.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.zdbjq.cn/Article/details/gzjxlkdxy.sHtML

[U88] JS：对象展开合并
来源：http://blog.fehbvm.com/Article/details/gjiyawfyh.sHtML

{ ...a, ...b }
来源：http://3g.fehbvm.com/Article/details/gprdgthwj.sHtML

[U89] JS：数组去重
来源：http://www.m.share.fehbvm.com/Article/details/ganczptar.sHtML

[...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/gyckxfofx.sHtML

[U90] JS：数字数组排序
来源：http://baike.zdbjq.cn/Article/details/gwbayesjk.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/gxiybgrhq.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.zdbjq.cn/Article/details/gnkkflljw.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.fehbvm.com/Article/details/gqrnmhyaf.sHtML

[U92] JS：深拷贝
来源：http://baike.fehbvm.com/Article/details/ggsokcupz.sHtML

structuredClone(obj)
来源：http://m.share.hesvh.cn/Article/details/gmbflnzph.sHtML

[U93] JS：模板字符串
来源：http://m.share.zdbjq.cn/Article/details/gtfqenner.sHtML

`共 ${n} 条`
来源：http://blog.hesvh.cn/Article/details/ghyfznnpa.sHtML

[U94] JS：箭头函数
来源：http://m.share.zdbjq.cn/Article/details/gprofmjeb.sHtML

const double = x => x * 2;
来源：http://baike.zdbjq.cn/Article/details/gyehsbekh.sHtML


<!-- 参考信息 -->