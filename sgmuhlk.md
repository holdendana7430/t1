代发 wailian999

[T05] Kotlin：when 表达式
来源：http://3g.hesvh.cn/Article/details/gkroottpk.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.zdbjq.cn/Article/details/glkifpygh.sHtML

[T06] Kotlin：集合映射
来源：http://3g.zdbjq.cn/Article/details/ghjuozrss.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gvqowqrkj.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.hesvh.cn/Article/details/glqbttcoo.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.zdbjq.cn/Article/details/gklwonkca.sHtML

[T08] Kotlin：数据类
来源：http://blog.zdbjq.cn/Article/details/gbsmpqzgo.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fehbvm.com/Article/details/gyjirqeik.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fehbvm.com/Article/details/gxbekvjrl.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fehbvm.com/Article/details/gufnvkzqj.sHtML

[T10] Kotlin：默认参数
来源：http://baike.zdbjq.cn/Article/details/gpkgzvagx.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fehbvm.com/Article/details/gcrfptsxq.sHtML

[T11] Kotlin：协程
来源：http://wap.hesvh.cn/Article/details/geqvakzqi.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.hesvh.cn/Article/details/ginwcmcql.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.hesvh.cn/Article/details/geaegtaur.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gffscsjax.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.hesvh.cn/Article/details/glujyuudg.sHtML

val m = mapOf("a" to 1)
来源：http://blog.hesvh.cn/Article/details/ggybcvluj.sHtML

[T14] Kotlin：循环
来源：http://mobile.fehbvm.com/Article/details/gnmdozebu.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.zdbjq.cn/Article/details/gghqmbslw.sHtML

[T15] Kotlin：接口
来源：http://3g.zdbjq.cn/Article/details/gehgtrhfr.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.hesvh.cn/Article/details/gpsevhyhe.sHtML

[T16] Swift：Hello World
来源：http://mobile.hesvh.cn/Article/details/gaiukzkvj.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/ggxnhvwxc.sHtML

[T17] Swift：变量与常量
来源：http://m.share.hesvh.cn/Article/details/gudpxxcew.sHtML

var a = 1;  let b = 2
来源：http://www.blog.fehbvm.com/Article/details/gfwdgtfpo.sHtML

[T18] Swift：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gmctrcbbz.sHtML

"值: \(b)"
来源：http://www.blog.fehbvm.com/Article/details/gfdbvipyr.sHtML

[T19] Swift：可选绑定
来源：http://wap.fehbvm.com/Article/details/ggpmnmapj.sHtML

if let n = opt { print(n) }
来源：http://read.share.fehbvm.com/Article/details/gfzjhofvj.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fehbvm.com/Article/details/gzwkbtykg.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fehbvm.com/Article/details/gyljzcfmg.sHtML

[T21] Swift：遍历
来源：http://www.blog.fehbvm.com/Article/details/glukmvxzn.sHtML

for x in a { print(x) }
来源：http://3g.zdbjq.cn/Article/details/grkvhxdnx.sHtML

[T22] Swift：字典
来源：http://blog.hesvh.cn/Article/details/ghsmmyzkw.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.hesvh.cn/Article/details/givyiadxw.sHtML

[T23] Swift：函数
来源：http://blog.fehbvm.com/Article/details/gavmxrgby.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.zdbjq.cn/Article/details/gplsvzmcx.sHtML

[T24] Swift：闭包
来源：http://read.share.fehbvm.com/Article/details/gvupcvwja.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gxlxkivnj.sHtML

[T25] Swift：结构体
来源：http://www.share.zdbjq.cn/Article/details/gufjqsxrn.sHtML

struct P { var x: Int }
来源：http://www.share.zdbjq.cn/Article/details/gnejpzbtg.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.zdbjq.cn/Article/details/gtejwlubi.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.zdbjq.cn/Article/details/giqoucdqt.sHtML

[T27] Swift：错误处理
来源：http://3g.fehbvm.com/Article/details/grrhtyawo.sHtML

do { try f() } catch { print(error) }
来源：http://3g.fehbvm.com/Article/details/gwszvvrgs.sHtML

[T28] Swift：枚举
来源：http://www.share.fehbvm.com/Article/details/gozmaumtg.sHtML

enum Color { case red, green }
来源：http://baike.fehbvm.com/Article/details/gtficshoy.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.hesvh.cn/Article/details/gkzohgduk.sHtML

guard let x = opt else { return }
来源：http://wap.hesvh.cn/Article/details/gezqojaov.sHtML

[T30] Swift：协议
来源：http://www.m.share.zdbjq.cn/Article/details/glqkbooyt.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.zdbjq.cn/Article/details/glqebheqg.sHtML

[T31] Lua：Hello World
来源：http://www.share.hesvh.cn/Article/details/gcgtbzudq.sHtML

print("Hello")
来源：http://baike.hesvh.cn/Article/details/gvilbvmsq.sHtML

[T32] Lua：局部变量
来源：http://blog.zdbjq.cn/Article/details/glewwrpmk.sHtML

local a = 1
来源：http://mobile.zdbjq.cn/Article/details/gawvomnyt.sHtML

[T33] Lua：表（数组）
来源：http://www.share.fehbvm.com/Article/details/geqajjcmm.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.fehbvm.com/Article/details/gnpqrmtby.sHtML

[T34] Lua：遍历表
来源：http://m.share.hesvh.cn/Article/details/gsechclws.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.hesvh.cn/Article/details/gvpubbjtd.sHtML

[T35] Lua：字典表
来源：http://3g.hesvh.cn/Article/details/gutuwzlic.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fehbvm.com/Article/details/gxalrtyka.sHtML

[T36] Lua：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gbrjtqvwt.sHtML

function add(a, b) return a + b end
来源：http://blog.hesvh.cn/Article/details/gtmufsupy.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.hesvh.cn/Article/details/gynfazifd.sHtML

"a" .. "b"
来源：http://baike.fehbvm.com/Article/details/gcyeigqpl.sHtML

[T38] Lua：条件
来源：http://mobile.zdbjq.cn/Article/details/gnvjikcyk.sHtML

if x > 0 then print("正") end
来源：http://mobile.zdbjq.cn/Article/details/gysswwdji.sHtML

[T39] Lua：模式匹配
来源：http://wap.fehbvm.com/Article/details/gosscbfkb.sHtML

string.find(s, "%d+")
来源：http://wap.hesvh.cn/Article/details/gsekfkfde.sHtML

[T40] Lua：元表
来源：http://mobile.hesvh.cn/Article/details/gqcbustfp.sHtML

setmetatable({}, { __index = base })
来源：http://baike.fehbvm.com/Article/details/gpxjewowz.sHtML

[T41] Perl：Hello World
来源：http://wap.fehbvm.com/Article/details/gphcyqlqh.sHtML

print "Hello\n";
来源：http://read.share.zdbjq.cn/Article/details/gpglxfuvh.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.zdbjq.cn/Article/details/govgndzzx.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.hesvh.cn/Article/details/grgpssqfm.sHtML

[T43] Perl：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gzdbnnmfy.sHtML

"值: $a"
来源：http://www.m.share.hesvh.cn/Article/details/gninihwkh.sHtML

[T44] Perl：条件
来源：http://www.blog.fehbvm.com/Article/details/ggjozeyox.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.hesvh.cn/Article/details/gbshjkqyx.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.fehbvm.com/Article/details/gqlzjkcqg.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.zdbjq.cn/Article/details/gcbacjfoo.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.zdbjq.cn/Article/details/gxagkwdmt.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.zdbjq.cn/Article/details/ggrbxyjxf.sHtML

[T47] Perl：正则捕获
来源：http://baike.fehbvm.com/Article/details/gtxmkdrow.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.hesvh.cn/Article/details/glngznuah.sHtML

[T48] Perl：正则替换
来源：http://read.share.hesvh.cn/Article/details/gjkudxkbg.sHtML

$s =~ s/old/new/g;
来源：http://mobile.hesvh.cn/Article/details/gymksxiil.sHtML

[T49] Perl：函数
来源：http://m.share.fehbvm.com/Article/details/gscdjwmin.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gjmruwfmt.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gmolsfudj.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.fehbvm.com/Article/details/gtxpzcuoh.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.hesvh.cn/Article/details/gtvxlcvls.sHtML

[T51] Scala：Hello World
来源：http://read.share.fehbvm.com/Article/details/gpfbqngmk.sHtML

println("Hello")
来源：http://www.blog.fehbvm.com/Article/details/geliockej.sHtML

[T52] Scala：变量
来源：http://www.share.fehbvm.com/Article/details/gsijznxwq.sHtML

val a = 1;  var b = 2
来源：http://m.share.zdbjq.cn/Article/details/ggcwkfwrs.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gjmjjgfen.sHtML

s"值: $b"
来源：http://wap.hesvh.cn/Article/details/glxatwmsu.sHtML

[T54] Scala：集合映射
来源：http://www.share.hesvh.cn/Article/details/gbykboujz.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.zdbjq.cn/Article/details/gaqgcefiz.sHtML

[T55] Scala：集合过滤
来源：http://wap.hesvh.cn/Article/details/gcarzbqqu.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.fehbvm.com/Article/details/gaeybphup.sHtML

[T56] Scala：样例类
来源：http://www.share.fehbvm.com/Article/details/gxskdgdvv.sHtML

case class User(name: String, age: Int)
来源：http://baike.zdbjq.cn/Article/details/gbkedvqri.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fehbvm.com/Article/details/gdgtzrmfj.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.hesvh.cn/Article/details/gccgnikvh.sHtML

[T58] Scala：函数定义
来源：http://m.share.hesvh.cn/Article/details/gntddgxyq.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.fehbvm.com/Article/details/gdtdwyysh.sHtML

[T59] Scala：循环
来源：http://www.blog.hesvh.cn/Article/details/gtukxplyr.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.hesvh.cn/Article/details/gaqueqpxm.sHtML

[T60] Scala：折叠
来源：http://m.share.fehbvm.com/Article/details/gajpnwggg.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.zdbjq.cn/Article/details/gyxgyleyh.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gyegdnkwf.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fehbvm.com/Article/details/gsmeexdia.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/glmyqhcgo.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.hesvh.cn/Article/details/gjloymzkq.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.fehbvm.com/Article/details/grlwbgjok.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.hesvh.cn/Article/details/gaedddiwg.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.hesvh.cn/Article/details/gwleqhftl.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.hesvh.cn/Article/details/gdiecpgxb.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.fehbvm.com/Article/details/gquqhgxhr.sHtML

[U04] Py：变量调试打印
来源：http://www.share.zdbjq.cn/Article/details/ggidhrrlk.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fehbvm.com/Article/details/gnzlwzopm.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.zdbjq.cn/Article/details/gddrsbkju.sHtML

list(dict.fromkeys(arr))
来源：http://blog.hesvh.cn/Article/details/gjpvtducd.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.fehbvm.com/Article/details/gsjfwequj.sHtML

{**a, **b}
来源：http://mobile.fehbvm.com/Article/details/gqajnorwo.sHtML

[U07] Py：反转字典键值
来源：http://mobile.fehbvm.com/Article/details/gkblbeaov.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.zdbjq.cn/Article/details/gfppogpwc.sHtML

[U08] Py：展平二维列表
来源：http://mobile.zdbjq.cn/Article/details/gfrprocrc.sHtML

[y for x in nested for y in x]
来源：http://blog.zdbjq.cn/Article/details/gfppsqigy.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.hesvh.cn/Article/details/gsfdgmapk.sHtML

max(d, key=d.get)
来源：http://www.blog.fehbvm.com/Article/details/gahelwdds.sHtML

[U10] Py：按值排序字典
来源：http://mobile.hesvh.cn/Article/details/geeambemb.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.fehbvm.com/Article/details/gocvzwgoe.sHtML

[U11] Py：生成器表达式
来源：http://wap.hesvh.cn/Article/details/gdytutedj.sHtML

(x * 2 for x in arr)
来源：http://baike.zdbjq.cn/Article/details/gwsjrrvmr.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.fehbvm.com/Article/details/gwdyycfzs.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.zdbjq.cn/Article/details/ggziwsavu.sHtML

[U13] Py：固定长度队列
来源：http://www.share.fehbvm.com/Article/details/gswwnpjgs.sHtML

deque(maxlen=10)
来源：http://wap.fehbvm.com/Article/details/ggyweorca.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.fehbvm.com/Article/details/gyjprgtrr.sHtML

defaultdict(list)
来源：http://wap.fehbvm.com/Article/details/gdyhamsds.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.fehbvm.com/Article/details/gsgeojbpr.sHtML

t = time.perf_counter()
来源：http://3g.hesvh.cn/Article/details/gzoponxpf.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.zdbjq.cn/Article/details/grehjdnle.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.hesvh.cn/Article/details/gbnpnkriz.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.zdbjq.cn/Article/details/gybjqdnds.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.hesvh.cn/Article/details/gwhreaoce.sHtML

[U18] Py：预编译正则
来源：http://mobile.fehbvm.com/Article/details/gkcssehmf.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.hesvh.cn/Article/details/gryxiiwwi.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.fehbvm.com/Article/details/gmnyfhwoc.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.hesvh.cn/Article/details/glvyexqca.sHtML

[U20] Py：缓存函数结果
来源：http://3g.hesvh.cn/Article/details/gbwcsdjgy.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.hesvh.cn/Article/details/gcyhzttpu.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.hesvh.cn/Article/details/gvvaakvtc.sHtML

@contextlib.contextmanager
来源：http://www.m.share.fehbvm.com/Article/details/grtsergfo.sHtML

[U22] Py：矩阵转置
来源：http://www.share.hesvh.cn/Article/details/gzbzzegco.sHtML

list(zip(*m))
来源：http://read.share.zdbjq.cn/Article/details/gsabgilzh.sHtML

[U23] Py：分块读取大文件
来源：http://3g.hesvh.cn/Article/details/gqquyvmjm.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.fehbvm.com/Article/details/gwatfmlmk.sHtML

[U24] Py：路径操作
来源：http://baike.hesvh.cn/Article/details/gycuhhhiw.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.zdbjq.cn/Article/details/gjjvwrydo.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.fehbvm.com/Article/details/glyygiwup.sHtML

csv.DictReader(f)
来源：http://www.blog.fehbvm.com/Article/details/ggzlwkxik.sHtML

[U26] Py：并发下载
来源：http://read.share.zdbjq.cn/Article/details/ghwazjmvn.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.hesvh.cn/Article/details/gpzjfnoai.sHtML

[U27] Py：异步 HTTP
来源：http://baike.zdbjq.cn/Article/details/ggvczcuvy.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.zdbjq.cn/Article/details/gxdyvhjmy.sHtML

[U28] Py：类型别名
来源：http://3g.hesvh.cn/Article/details/glbcsidax.sHtML

UserId = int
来源：http://www.blog.zdbjq.cn/Article/details/gqybvxpaz.sHtML

[U29] Py：属性校验
来源：http://wap.zdbjq.cn/Article/details/gnjbibsrp.sHtML

@property 与 @x.setter 配合
来源：http://read.share.zdbjq.cn/Article/details/gcdhoffom.sHtML

[U30] Py：数据类
来源：http://baike.zdbjq.cn/Article/details/gnopeyhob.sHtML

@dataclass(slots=True)
来源：http://www.blog.fehbvm.com/Article/details/gbuauvsgu.sHtML

[U31] Py：单测
来源：http://www.share.hesvh.cn/Article/details/gzxiffrkr.sHtML

python -m pytest -q
来源：http://mobile.hesvh.cn/Article/details/gglghdipq.sHtML

[U32] Py：代码格式化
来源：http://read.share.fehbvm.com/Article/details/gciywyodu.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.zdbjq.cn/Article/details/ggcnqwbbu.sHtML

[U33] Py：打包发布
来源：http://wap.fehbvm.com/Article/details/gyzscclrk.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.zdbjq.cn/Article/details/gmrswwwde.sHtML

[U34] Py：判断编码
来源：http://mobile.hesvh.cn/Article/details/gzhksowir.sHtML

chardet.detect(raw)
来源：http://baike.fehbvm.com/Article/details/gokcopkqu.sHtML

[U35] Py：发送邮件
来源：http://read.share.zdbjq.cn/Article/details/gnfymgqmf.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.fehbvm.com/Article/details/gsotnpbfr.sHtML

[U36] Py：定时任务
来源：http://www.blog.hesvh.cn/Article/details/gyamhknnn.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.fehbvm.com/Article/details/gpidktahe.sHtML

[U37] Py：读写 Excel
来源：http://wap.hesvh.cn/Article/details/gsnbfivuv.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.zdbjq.cn/Article/details/gaxgjueim.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.zdbjq.cn/Article/details/gqoleknvv.sHtML

Path(__file__).resolve().parent
来源：http://baike.zdbjq.cn/Article/details/grgqortzz.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.zdbjq.cn/Article/details/ggdgmjvue.sHtML

sys.stdout.isatty()
来源：http://mobile.fehbvm.com/Article/details/gkpdtbyjz.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.zdbjq.cn/Article/details/gdjbkinzt.sHtML

print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/gniqrjgxg.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.zdbjq.cn/Article/details/gsapkqccw.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.hesvh.cn/Article/details/gkyqjtaaw.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.zdbjq.cn/Article/details/gatgpnaxb.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.zdbjq.cn/Article/details/gfrrovvca.sHtML

[U43] PHP：声明命名空间
来源：http://baike.hesvh.cn/Article/details/gpslqgaru.sHtML

namespace App\Http;
来源：http://blog.fehbvm.com/Article/details/gskefyefq.sHtML

[U44] PHP：开启严格类型
来源：http://blog.hesvh.cn/Article/details/girvpdgmb.sHtML

declare(strict_types=1);
来源：http://blog.zdbjq.cn/Article/details/ghzovpzpe.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.fehbvm.com/Article/details/gpyoihbjs.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gyfffdgiu.sHtML

[U46] PHP：可空类型
来源：http://mobile.fehbvm.com/Article/details/gcdlgxbpe.sHtML

?string $name = null
来源：http://m.share.zdbjq.cn/Article/details/gennkxiks.sHtML

[U47] PHP：联合类型
来源：http://mobile.hesvh.cn/Article/details/gdswjifmp.sHtML

int|string $id
来源：http://wap.hesvh.cn/Article/details/gndvmhjjh.sHtML

[U48] PHP：纯枚举
来源：http://blog.fehbvm.com/Article/details/gdrpaiifa.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.fehbvm.com/Article/details/guzpaykkc.sHtML

[U49] PHP：只读属性
来源：http://m.share.zdbjq.cn/Article/details/gcewyrrum.sHtML

public readonly string $name
来源：http://blog.zdbjq.cn/Article/details/gucjnhxlm.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.zdbjq.cn/Article/details/ghrfrijfk.sHtML

public function __construct(private int $id) {}
来源：http://www.share.hesvh.cn/Article/details/gvpigiska.sHtML

[U51] PHP：数组解构
来源：http://read.share.hesvh.cn/Article/details/ghsymdlop.sHtML

[$a, $b] = $arr;
来源：http://mobile.zdbjq.cn/Article/details/guhasbngo.sHtML

[U52] PHP：箭头函数
来源：http://wap.zdbjq.cn/Article/details/glfncwlpu.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.fehbvm.com/Article/details/goncbogms.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.fehbvm.com/Article/details/germvrjvo.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.zdbjq.cn/Article/details/gwxwytlxl.sHtML

[U54] PHP：空安全调用
来源：http://www.share.hesvh.cn/Article/details/gstjqbxli.sHtML

$obj?->method()
来源：http://mobile.hesvh.cn/Article/details/gixkhuxfi.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.hesvh.cn/Article/details/gulstewax.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.zdbjq.cn/Article/details/gwshyqwez.sHtML

[U56] PHP：命名参数
来源：http://www.blog.fehbvm.com/Article/details/gcnahkkim.sHtML

f(a: 1, b: 2)
来源：http://wap.hesvh.cn/Article/details/gyvlirbpi.sHtML

[U57] PHP：字符串插值
来源：http://baike.zdbjq.cn/Article/details/ggexyoxra.sHtML

"值: {$a}"
来源：http://3g.fehbvm.com/Article/details/glndpenvn.sHtML

[U58] PHP：数组三件套
来源：http://blog.hesvh.cn/Article/details/gdqismeec.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.fehbvm.com/Article/details/gprowcxwt.sHtML

[U59] PHP：自定义排序
来源：http://blog.zdbjq.cn/Article/details/gptjdcgjw.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.zdbjq.cn/Article/details/gsblaahbz.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.zdbjq.cn/Article/details/ghjharcid.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.hesvh.cn/Article/details/gzhjuhqia.sHtML

[U61] PHP：正则
来源：http://wap.fehbvm.com/Article/details/gzgwvoxew.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.fehbvm.com/Article/details/gfieocyjp.sHtML

[U62] PHP：日期对象
来源：http://3g.zdbjq.cn/Article/details/grvqlhups.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.zdbjq.cn/Article/details/gbioepvve.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.fehbvm.com/Article/details/gkjyvyybd.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.zdbjq.cn/Article/details/gcmfesaea.sHtML

[U64] PHP：目录遍历
来源：http://wap.hesvh.cn/Article/details/giphjilfl.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.hesvh.cn/Article/details/gsbqbkdkb.sHtML

[U65] PHP：会话
来源：http://wap.fehbvm.com/Article/details/gnluvvcak.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gwqwumckr.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.fehbvm.com/Article/details/gpwitgxpi.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.zdbjq.cn/Article/details/gkpsxxwbo.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.zdbjq.cn/Article/details/gqaaqlcff.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.zdbjq.cn/Article/details/gqjtqjlbw.sHtML

[U68] PHP：PDO 连接
来源：http://blog.zdbjq.cn/Article/details/gjauikitr.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.hesvh.cn/Article/details/greoztajk.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.hesvh.cn/Article/details/gvdlounze.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.zdbjq.cn/Article/details/gybihcosy.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.hesvh.cn/Article/details/gxstwxngl.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.hesvh.cn/Article/details/ghwomknpk.sHtML

[U71] PHP：抛出异常
来源：http://baike.fehbvm.com/Article/details/gkohkkfph.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.hesvh.cn/Article/details/gyunifigh.sHtML

[U72] PHP：写错误日志
来源：http://wap.fehbvm.com/Article/details/gbqwqikcb.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.hesvh.cn/Article/details/gfeyscdsc.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.hesvh.cn/Article/details/gyriaqbbt.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.hesvh.cn/Article/details/gfpjezbow.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.fehbvm.com/Article/details/gdepgxggt.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.zdbjq.cn/Article/details/golclqptj.sHtML

[U75] PHP：依赖注入
来源：http://baike.zdbjq.cn/Article/details/gdehhgafx.sHtML

composer require psr/container
来源：http://read.share.zdbjq.cn/Article/details/gixnzzdxp.sHtML

[U76] PHP：简单路由
来源：http://www.blog.hesvh.cn/Article/details/gnacolgow.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.fehbvm.com/Article/details/gozwzebzp.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.zdbjq.cn/Article/details/geodmlmaw.sHtML

composer require twig/twig
来源：http://www.m.share.zdbjq.cn/Article/details/gtrtdaarw.sHtML

[U78] PHP：单元测试
来源：http://read.share.zdbjq.cn/Article/details/gbkumddnz.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.hesvh.cn/Article/details/gdrqzujvs.sHtML

[U79] PHP：静态分析
来源：http://www.blog.fehbvm.com/Article/details/gubyxejdh.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.hesvh.cn/Article/details/gwzeevnpe.sHtML

[U80] PHP：代码规范修复
来源：http://3g.hesvh.cn/Article/details/gfilvrrea.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.zdbjq.cn/Article/details/gmvmeakdc.sHtML

[U81] JS：初始化项目
来源：http://www.share.fehbvm.com/Article/details/ghfmywpev.sHtML

npm init -y;  npm i express
来源：http://m.share.fehbvm.com/Article/details/ggthekmqy.sHtML

[U82] JS：package.json 脚本
来源：http://3g.fehbvm.com/Article/details/gvgloxcne.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.fehbvm.com/Article/details/gxlksdiaz.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.zdbjq.cn/Article/details/gdmbwaufd.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.zdbjq.cn/Article/details/gbcfcbefh.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.zdbjq.cn/Article/details/gfljswarl.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.fehbvm.com/Article/details/gkginuveo.sHtML

[U85] JS：可选链
来源：http://m.share.hesvh.cn/Article/details/gmodvlkjw.sHtML

a?.b?.c
来源：http://3g.fehbvm.com/Article/details/gtvraucno.sHtML

[U86] JS：空值合并
来源：http://www.share.hesvh.cn/Article/details/gyteibxti.sHtML

a ?? b
来源：http://www.m.share.hesvh.cn/Article/details/gxgrwtjch.sHtML

[U87] JS：解构默认值
来源：http://wap.fehbvm.com/Article/details/gjwwpcxrk.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.zdbjq.cn/Article/details/gxnrqudxy.sHtML

[U88] JS：对象展开合并
来源：http://blog.hesvh.cn/Article/details/gstodabdp.sHtML

{ ...a, ...b }
来源：http://m.share.zdbjq.cn/Article/details/gphnjdutx.sHtML

[U89] JS：数组去重
来源：http://baike.hesvh.cn/Article/details/gmjruwekv.sHtML

[...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/gsqbdnfam.sHtML

[U90] JS：数字数组排序
来源：http://blog.fehbvm.com/Article/details/gfnhgjadv.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gucezrgum.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.fehbvm.com/Article/details/gvcsrbgox.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.hesvh.cn/Article/details/gultjssqi.sHtML

[U92] JS：深拷贝
来源：http://blog.hesvh.cn/Article/details/guivjjdca.sHtML

structuredClone(obj)
来源：http://3g.zdbjq.cn/Article/details/ggojwmbca.sHtML


<!-- 参考信息 -->