代发 wailian999

[T07] Kotlin：集合过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbylxwgof.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdskabrhd.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/gtohjqnvt.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjldrjxj.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gmkomxhva.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fanxiaobao.xyz/Article/details/gfupflhtb.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fanxiaobao.xyz/Article/details/gqzrojiwf.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fanxiaobao.xyz/Article/details/gxmfaembq.sHtML

[T11] Kotlin：协程
来源：http://wap.fanxiaobao.xyz/Article/details/gvdzcpqnv.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.fanxiaobao.xyz/Article/details/gulfblqej.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fanxiaobao.xyz/Article/details/gdxdqzuus.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/glpljguww.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjdvoloid.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggzuvfyia.sHtML

[T14] Kotlin：循环
来源：http://blog.fanxiaobao.xyz/Article/details/gpdowiqsj.sHtML

for (i in 1..10) println(i)
来源：http://3g.fanxiaobao.xyz/Article/details/gutqgkuiu.sHtML

[T15] Kotlin：接口
来源：http://www.share.fanxiaobao.xyz/Article/details/gtoofbtaa.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fanxiaobao.xyz/Article/details/grzvwzupj.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbfqftlmr.sHtML

print("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/ggyjqsndj.sHtML

[T17] Swift：变量与常量
来源：http://baike.fanxiaobao.xyz/Article/details/gbohuqxmj.sHtML

var a = 1;  let b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/goeydhdvb.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpdtijwla.sHtML

"值: \(b)"
来源：http://baike.fanxiaobao.xyz/Article/details/glqsktbly.sHtML

[T19] Swift：可选绑定
来源：http://wap.fanxiaobao.xyz/Article/details/gaoalfgbx.sHtML

if let n = opt { print(n) }
来源：http://wap.fanxiaobao.xyz/Article/details/ggxnvudav.sHtML

[T20] Swift：数组操作
来源：http://blog.fanxiaobao.xyz/Article/details/gpecwdrrw.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbhykdgwf.sHtML

[T21] Swift：遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gpequpovv.sHtML

for x in a { print(x) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gppxepeig.sHtML

[T22] Swift：字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gxxwgmxzl.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfnfrzhso.sHtML

[T23] Swift：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gnjxekolx.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fanxiaobao.xyz/Article/details/grbjasbzj.sHtML

[T24] Swift：闭包
来源：http://baike.fanxiaobao.xyz/Article/details/givzdyjep.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggnztlkxn.sHtML

[T25] Swift：结构体
来源：http://wap.fanxiaobao.xyz/Article/details/gldetixzn.sHtML

struct P { var x: Int }
来源：http://wap.fanxiaobao.xyz/Article/details/gwyjadvpm.sHtML

[T26] Swift：类与重写
来源：http://baike.fanxiaobao.xyz/Article/details/goseeqezn.sHtML

class A: Base { override func f() {} }
来源：http://blog.fanxiaobao.xyz/Article/details/ghrdisdpr.sHtML

[T27] Swift：错误处理
来源：http://wap.fanxiaobao.xyz/Article/details/gessepjpp.sHtML

do { try f() } catch { print(error) }
来源：http://baike.fanxiaobao.xyz/Article/details/ghntygbtp.sHtML

[T28] Swift：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gkpbfhvva.sHtML

enum Color { case red, green }
来源：http://wap.fanxiaobao.xyz/Article/details/gccegajdv.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fanxiaobao.xyz/Article/details/givcqqjzy.sHtML

guard let x = opt else { return }
来源：http://baike.fanxiaobao.xyz/Article/details/gnoewwnhi.sHtML

[T30] Swift：协议
来源：http://www.share.fanxiaobao.xyz/Article/details/gsptcbadm.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fanxiaobao.xyz/Article/details/gbsgmefit.sHtML

[T31] Lua：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/goaneaevu.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gptyrgcqc.sHtML

[T32] Lua：局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gtpeppehb.sHtML

local a = 1
来源：http://3g.fanxiaobao.xyz/Article/details/gjugtsmnw.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fanxiaobao.xyz/Article/details/guyzpcvmg.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.fanxiaobao.xyz/Article/details/gorbzqhxi.sHtML

[T34] Lua：遍历表
来源：http://baike.fanxiaobao.xyz/Article/details/gsjvoerqv.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbvwpauvi.sHtML

[T35] Lua：字典表
来源：http://blog.fanxiaobao.xyz/Article/details/gihkmjkne.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjzrdjlzz.sHtML

[T36] Lua：函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gykijfutq.sHtML

function add(a, b) return a + b end
来源：http://3g.fanxiaobao.xyz/Article/details/golpuqahu.sHtML

[T37] Lua：字符串拼接
来源：http://blog.fanxiaobao.xyz/Article/details/gxmjewzli.sHtML

"a" .. "b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gjzzneylk.sHtML

[T38] Lua：条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gbylyrfhd.sHtML

if x > 0 then print("正") end
来源：http://m.share.fanxiaobao.xyz/Article/details/gdzsqhxcq.sHtML

[T39] Lua：模式匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gjrmhgsyx.sHtML

string.find(s, "%d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/gzbttulll.sHtML

[T40] Lua：元表
来源：http://www.share.fanxiaobao.xyz/Article/details/gyunprcks.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fanxiaobao.xyz/Article/details/giosbejlb.sHtML

[T41] Perl：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gcxkkvqpz.sHtML

print "Hello\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxeatsouh.sHtML

[T42] Perl：变量类型
来源：http://3g.fanxiaobao.xyz/Article/details/grdvebdyh.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.fanxiaobao.xyz/Article/details/gfnuwjodo.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggpgsxwfm.sHtML

"值: $a"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxetjxete.sHtML

[T44] Perl：条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gowybrqjz.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glejleocx.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfxbitkdk.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnfkotxqr.sHtML

[T46] Perl：哈希操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gfsemwsdu.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gcnudctem.sHtML

[T47] Perl：正则捕获
来源：http://www.share.fanxiaobao.xyz/Article/details/gkrakdbfm.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gcmppwrxx.sHtML

[T48] Perl：正则替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gurwrwmdj.sHtML

$s =~ s/old/new/g;
来源：http://3g.fanxiaobao.xyz/Article/details/gjitbeddr.sHtML

[T49] Perl：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gcaebrjje.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtpjmghlo.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gtiyxwvwb.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfaxpconw.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gscwcvcfi.sHtML

[T51] Scala：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gyjuvkgfu.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gionkbcpg.sHtML

[T52] Scala：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gekauhulx.sHtML

val a = 1;  var b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzmpmazxa.sHtML

[T53] Scala：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gokiwcfif.sHtML

s"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/gjqcjydma.sHtML

[T54] Scala：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/gjrsposig.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyvjkmnpz.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gxlirphjg.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gouttsbmb.sHtML

[T56] Scala：样例类
来源：http://blog.fanxiaobao.xyz/Article/details/geiwmfiun.sHtML

case class User(name: String, age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/gxqduwbaj.sHtML

[T57] Scala：模式匹配
来源：http://baike.fanxiaobao.xyz/Article/details/guazuvtps.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.fanxiaobao.xyz/Article/details/gjqcyzrxp.sHtML

[T58] Scala：函数定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnbnzkxgz.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fanxiaobao.xyz/Article/details/gitsbsvyf.sHtML

[T59] Scala：循环
来源：http://3g.fanxiaobao.xyz/Article/details/gatwyttyl.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqoyymupg.sHtML

[T60] Scala：折叠
来源：http://m.share.fanxiaobao.xyz/Article/details/goavwuhwl.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnzgnwkcn.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gwgsqjtoo.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gywwuhidz.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwukiavxg.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.fanxiaobao.xyz/Article/details/ghxmeaoxy.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.fanxiaobao.xyz/Article/details/giqsvqwza.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.fanxiaobao.xyz/Article/details/grufkjvvg.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gcwqwtfbq.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.fanxiaobao.xyz/Article/details/gjjmlxwyq.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.fanxiaobao.xyz/Article/details/gezixajlc.sHtML

[U04] Py：变量调试打印
来源：http://wap.fanxiaobao.xyz/Article/details/ghlsftdeu.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.fanxiaobao.xyz/Article/details/ggamspeym.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpfsiqnrk.sHtML

list(dict.fromkeys(arr))
来源：http://blog.fanxiaobao.xyz/Article/details/gmepthfki.sHtML

[U06] Py：合并两个字典
来源：http://m.share.fanxiaobao.xyz/Article/details/gnpssvexu.sHtML

{**a, **b}
来源：http://m.share.fanxiaobao.xyz/Article/details/gslylpycu.sHtML

[U07] Py：反转字典键值
来源：http://wap.fanxiaobao.xyz/Article/details/gntmewita.sHtML

{v: k for k, v in d.items()}
来源：http://baike.fanxiaobao.xyz/Article/details/gmdyvearf.sHtML

[U08] Py：展平二维列表
来源：http://wap.fanxiaobao.xyz/Article/details/gigobxvao.sHtML

[y for x in nested for y in x]
来源：http://m.share.fanxiaobao.xyz/Article/details/gohvybpbl.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.fanxiaobao.xyz/Article/details/gbvdxsrlz.sHtML

max(d, key=d.get)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbculuyse.sHtML

[U10] Py：按值排序字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gcaovqljt.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkpkhhffa.sHtML

[U11] Py：生成器表达式
来源：http://baike.fanxiaobao.xyz/Article/details/geqprxemh.sHtML

(x * 2 for x in arr)
来源：http://wap.fanxiaobao.xyz/Article/details/gdapggkdw.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzewzoqtb.sHtML

Counter(arr).most_common(3)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtijqedyv.sHtML

[U13] Py：固定长度队列
来源：http://wap.fanxiaobao.xyz/Article/details/gepzucgbw.sHtML

deque(maxlen=10)
来源：http://3g.fanxiaobao.xyz/Article/details/ggkakhpta.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.fanxiaobao.xyz/Article/details/guasnyinx.sHtML

defaultdict(list)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbothtyot.sHtML

[U15] Py：高精度计时
来源：http://mobile.fanxiaobao.xyz/Article/details/goryrwjre.sHtML

t = time.perf_counter()
来源：http://3g.fanxiaobao.xyz/Article/details/gdpvmmgwx.sHtML

[U16] Py：命令行参数解析
来源：http://baike.fanxiaobao.xyz/Article/details/gappblxbj.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fanxiaobao.xyz/Article/details/gvkqxbaap.sHtML

[U17] Py：初始化日志
来源：http://wap.fanxiaobao.xyz/Article/details/gtqszimuo.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.fanxiaobao.xyz/Article/details/gdblmqxvg.sHtML

[U18] Py：预编译正则
来源：http://blog.fanxiaobao.xyz/Article/details/gqaomiryc.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/gvosjqlkv.sHtML

[U19] Py：正则替换带回调
来源：http://blog.fanxiaobao.xyz/Article/details/gxiekbkiw.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxngsvtix.sHtML

[U20] Py：缓存函数结果
来源：http://wap.fanxiaobao.xyz/Article/details/gvrftrdrw.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.fanxiaobao.xyz/Article/details/gurjjvvtf.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.fanxiaobao.xyz/Article/details/gzxaymqhr.sHtML

@contextlib.contextmanager
来源：http://www.blog.fanxiaobao.xyz/Article/details/gisykfitm.sHtML

[U22] Py：矩阵转置
来源：http://3g.fanxiaobao.xyz/Article/details/gxtdpanie.sHtML

list(zip(*m))
来源：http://www.share.fanxiaobao.xyz/Article/details/ggbvaxdkj.sHtML

[U23] Py：分块读取大文件
来源：http://3g.fanxiaobao.xyz/Article/details/gfdxrgjmg.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.fanxiaobao.xyz/Article/details/gxioheboo.sHtML

[U24] Py：路径操作
来源：http://baike.fanxiaobao.xyz/Article/details/gcqxhbeaj.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/gguwuhwbe.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.fanxiaobao.xyz/Article/details/gupqfdljn.sHtML

csv.DictReader(f)
来源：http://3g.fanxiaobao.xyz/Article/details/gjcqybeum.sHtML

[U26] Py：并发下载
来源：http://mobile.fanxiaobao.xyz/Article/details/grybpbkzn.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.fanxiaobao.xyz/Article/details/gppkdmmrl.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.fanxiaobao.xyz/Article/details/gbaaqppus.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.fanxiaobao.xyz/Article/details/ggqhanreh.sHtML

[U28] Py：类型别名
来源：http://blog.fanxiaobao.xyz/Article/details/gtltufqic.sHtML

UserId = int
来源：http://mobile.fanxiaobao.xyz/Article/details/gornoequz.sHtML

[U29] Py：属性校验
来源：http://blog.fanxiaobao.xyz/Article/details/gcbqslcfg.sHtML

@property 与 @x.setter 配合
来源：http://blog.fanxiaobao.xyz/Article/details/goexljffn.sHtML

[U30] Py：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/gfenrkmlx.sHtML

@dataclass(slots=True)
来源：http://wap.fanxiaobao.xyz/Article/details/gktchywfv.sHtML

[U31] Py：单测
来源：http://m.share.fanxiaobao.xyz/Article/details/gogkuddhv.sHtML

python -m pytest -q
来源：http://mobile.fanxiaobao.xyz/Article/details/gdushcbop.sHtML

[U32] Py：代码格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnxspraea.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.fanxiaobao.xyz/Article/details/gihutvkjc.sHtML

[U33] Py：打包发布
来源：http://3g.fanxiaobao.xyz/Article/details/glkdqpukm.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.fanxiaobao.xyz/Article/details/gghwdcqvl.sHtML

[U34] Py：判断编码
来源：http://baike.fanxiaobao.xyz/Article/details/gmabbuhwm.sHtML

chardet.detect(raw)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywwjnkth.sHtML

[U35] Py：发送邮件
来源：http://blog.fanxiaobao.xyz/Article/details/ggktznthf.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.fanxiaobao.xyz/Article/details/ginbukexa.sHtML

[U36] Py：定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gguimyyci.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.fanxiaobao.xyz/Article/details/gplpdsfac.sHtML

[U37] Py：读写 Excel
来源：http://wap.fanxiaobao.xyz/Article/details/gacwtbmnd.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.fanxiaobao.xyz/Article/details/gfyilirba.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.fanxiaobao.xyz/Article/details/gvwultcoo.sHtML

Path(__file__).resolve().parent
来源：http://3g.fanxiaobao.xyz/Article/details/gbnauomke.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.fanxiaobao.xyz/Article/details/gwbpbqvgl.sHtML

sys.stdout.isatty()
来源：http://3g.fanxiaobao.xyz/Article/details/ggtrksjem.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.fanxiaobao.xyz/Article/details/ghimieapw.sHtML

print("err", file=sys.stderr)
来源：http://wap.fanxiaobao.xyz/Article/details/gcuczshod.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.fanxiaobao.xyz/Article/details/gargzdzqf.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.fanxiaobao.xyz/Article/details/gusiojypj.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.fanxiaobao.xyz/Article/details/gvobcobtu.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvgbicjqg.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/gtkckxvbz.sHtML

namespace App\Http;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbgfnejpn.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdwknrdpq.sHtML

declare(strict_types=1);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjiqxzgrg.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.fanxiaobao.xyz/Article/details/gdhsmgjjy.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/grtnoazhx.sHtML

[U46] PHP：可空类型
来源：http://3g.fanxiaobao.xyz/Article/details/gfbormihu.sHtML

?string $name = null
来源：http://wap.fanxiaobao.xyz/Article/details/gzmvpuqpn.sHtML

[U47] PHP：联合类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwajjayfd.sHtML

int|string $id
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gubamklrj.sHtML

[U48] PHP：纯枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gqjwjtgfm.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.fanxiaobao.xyz/Article/details/glgzobqzc.sHtML

[U49] PHP：只读属性
来源：http://mobile.fanxiaobao.xyz/Article/details/gteybxzdg.sHtML

public readonly string $name
来源：http://m.share.fanxiaobao.xyz/Article/details/gjkfdosvd.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.fanxiaobao.xyz/Article/details/ghudjylco.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggvqpafuh.sHtML

[U51] PHP：数组解构
来源：http://baike.fanxiaobao.xyz/Article/details/gsmhuwvjb.sHtML

[$a, $b] = $arr;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkxbhavou.sHtML

[U52] PHP：箭头函数
来源：http://3g.fanxiaobao.xyz/Article/details/geuqpfscz.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzlgahnye.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfyysrmjg.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.fanxiaobao.xyz/Article/details/gjbhbtaky.sHtML

[U54] PHP：空安全调用
来源：http://wap.fanxiaobao.xyz/Article/details/gvozabhen.sHtML

$obj?->method()
来源：http://baike.fanxiaobao.xyz/Article/details/ggdwmxzhw.sHtML

[U55] PHP：match 表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gepxeozyy.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.fanxiaobao.xyz/Article/details/gqoarfozv.sHtML

[U56] PHP：命名参数
来源：http://m.share.fanxiaobao.xyz/Article/details/ghyotuvqx.sHtML

f(a: 1, b: 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqmqfbksk.sHtML

[U57] PHP：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/goyzudpqr.sHtML

"值: {$a}"
来源：http://wap.fanxiaobao.xyz/Article/details/gncuyrzgw.sHtML

[U58] PHP：数组三件套
来源：http://mobile.fanxiaobao.xyz/Article/details/gdjaefisu.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/golwukgtl.sHtML

[U59] PHP：自定义排序
来源：http://wap.fanxiaobao.xyz/Article/details/gxebnpvpl.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fanxiaobao.xyz/Article/details/ginnaimkz.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gazuwuowm.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggqxfnnoj.sHtML

[U61] PHP：正则
来源：http://baike.fanxiaobao.xyz/Article/details/ggknzscep.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.fanxiaobao.xyz/Article/details/gauvicyxq.sHtML

[U62] PHP：日期对象
来源：http://mobile.fanxiaobao.xyz/Article/details/gdqsvgdul.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.fanxiaobao.xyz/Article/details/giejvlkuo.sHtML

[U63] PHP：文件读写
来源：http://wap.fanxiaobao.xyz/Article/details/gvxwseubo.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.fanxiaobao.xyz/Article/details/gnchudtzs.sHtML

[U64] PHP：目录遍历
来源：http://3g.fanxiaobao.xyz/Article/details/glufxsnav.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.fanxiaobao.xyz/Article/details/gvanmdmoo.sHtML

[U65] PHP：会话
来源：http://read.share.fanxiaobao.xyz/Article/details/gcyirvbwd.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzxuxdvhu.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.fanxiaobao.xyz/Article/details/gzaekrpml.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gaqytmbjk.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.fanxiaobao.xyz/Article/details/gikxtvyrr.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.fanxiaobao.xyz/Article/details/grvdhajzg.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.fanxiaobao.xyz/Article/details/glkihcylq.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.fanxiaobao.xyz/Article/details/gujdekxng.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.fanxiaobao.xyz/Article/details/gatclledi.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbqcrbwsi.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxfvybfs.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghurfhwix.sHtML

[U71] PHP：抛出异常
来源：http://m.share.fanxiaobao.xyz/Article/details/gqlafbtrv.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvsaclzed.sHtML

[U72] PHP：写错误日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gaghauiyx.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.fanxiaobao.xyz/Article/details/ghtlbasdn.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.fanxiaobao.xyz/Article/details/gkmeqrldo.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvtdndteh.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwnkcwwmk.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcbmmtuvv.sHtML

[U75] PHP：依赖注入
来源：http://www.share.fanxiaobao.xyz/Article/details/gqjnzgape.sHtML

composer require psr/container
来源：http://m.share.fanxiaobao.xyz/Article/details/gzrxupuor.sHtML

[U76] PHP：简单路由
来源：http://blog.fanxiaobao.xyz/Article/details/gbuorucxg.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmgbwosti.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqqgmzanr.sHtML

composer require twig/twig
来源：http://m.share.fanxiaobao.xyz/Article/details/ggtmhigiv.sHtML

[U78] PHP：单元测试
来源：http://wap.fanxiaobao.xyz/Article/details/gfkxwuxjw.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.fanxiaobao.xyz/Article/details/genmeqprq.sHtML

[U79] PHP：静态分析
来源：http://m.share.fanxiaobao.xyz/Article/details/guokjnrsm.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.fanxiaobao.xyz/Article/details/gigglpbbb.sHtML

[U80] PHP：代码规范修复
来源：http://blog.fanxiaobao.xyz/Article/details/grzhkvwiq.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmowgcmno.sHtML

[U81] JS：初始化项目
来源：http://wap.fanxiaobao.xyz/Article/details/guqlzelfy.sHtML

npm init -y;  npm i express
来源：http://3g.fanxiaobao.xyz/Article/details/gfxkynzbl.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.fanxiaobao.xyz/Article/details/gijszlqcp.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.fanxiaobao.xyz/Article/details/gpibauorz.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.fanxiaobao.xyz/Article/details/gbbohlkoa.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.fanxiaobao.xyz/Article/details/gibhiswqi.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.fanxiaobao.xyz/Article/details/gimwtboco.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.fanxiaobao.xyz/Article/details/gvtjzgtqb.sHtML

[U85] JS：可选链
来源：http://mobile.fanxiaobao.xyz/Article/details/glanabcaw.sHtML

a?.b?.c
来源：http://wap.fanxiaobao.xyz/Article/details/gtcdybnyd.sHtML

[U86] JS：空值合并
来源：http://blog.fanxiaobao.xyz/Article/details/gjfuiqzjw.sHtML

a ?? b
来源：http://www.share.fanxiaobao.xyz/Article/details/gqzprwgpg.sHtML

[U87] JS：解构默认值
来源：http://3g.fanxiaobao.xyz/Article/details/gcnefwmtn.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gywmepuqz.sHtML

[U88] JS：对象展开合并
来源：http://m.share.fanxiaobao.xyz/Article/details/gatinzrmm.sHtML

{ ...a, ...b }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjgyoobwd.sHtML

[U89] JS：数组去重
来源：http://mobile.fanxiaobao.xyz/Article/details/gbvrveadc.sHtML

[...new Set(arr)]
来源：http://www.share.fanxiaobao.xyz/Article/details/gxaoqbszx.sHtML

[U90] JS：数字数组排序
来源：http://3g.fanxiaobao.xyz/Article/details/gutnmcwwm.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjvarxtro.sHtML

[U91] JS：对象键值遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gkdehlyvc.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqyirfrrt.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gipgcvjil.sHtML

structuredClone(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/guzdjhekh.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkdpccjpx.sHtML

`共 ${n} 条`
来源：http://blog.fanxiaobao.xyz/Article/details/gjyvkrqji.sHtML

[U94] JS：箭头函数
来源：http://m.share.fanxiaobao.xyz/Article/details/glzsbzyfn.sHtML

const double = x => x * 2;
来源：http://wap.fanxiaobao.xyz/Article/details/gysnhtsey.sHtML


<!-- 参考信息 -->