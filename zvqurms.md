代发 wailian999

[T05] Kotlin：when 表达式
来源：http://blog.zdbjq.cn/Article/details/gvkxboqxw.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fehbvm.com/Article/details/gxeurikxw.sHtML

[T06] Kotlin：集合映射
来源：http://baike.hesvh.cn/Article/details/gojcqdvhn.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gsxgkzhkw.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.zdbjq.cn/Article/details/golawqpmg.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.zdbjq.cn/Article/details/gkibxgwgs.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.zdbjq.cn/Article/details/gnwajfwzn.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fehbvm.com/Article/details/grgwytvej.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fehbvm.com/Article/details/gazrtrlwa.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.zdbjq.cn/Article/details/gvzicisxb.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.zdbjq.cn/Article/details/gqbeexhbg.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fehbvm.com/Article/details/gufijngdg.sHtML

[T11] Kotlin：协程
来源：http://3g.fehbvm.com/Article/details/gzhoikjeh.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.hesvh.cn/Article/details/gxsmpivvx.sHtML

[T12] Kotlin：解构声明
来源：http://wap.hesvh.cn/Article/details/gxogdeeky.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gmutfkrda.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.hesvh.cn/Article/details/gcvbsrwiu.sHtML

val m = mapOf("a" to 1)
来源：http://blog.hesvh.cn/Article/details/gstluytzg.sHtML

[T14] Kotlin：循环
来源：http://www.blog.zdbjq.cn/Article/details/gpeaklveh.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fehbvm.com/Article/details/gptraraxb.sHtML

[T15] Kotlin：接口
来源：http://blog.fehbvm.com/Article/details/gcvvvpfhq.sHtML

interface Shape { fun area(): Double }
来源：http://blog.hesvh.cn/Article/details/gyqpzusbh.sHtML

[T16] Swift：Hello World
来源：http://wap.zdbjq.cn/Article/details/gtsdrtyfb.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/goizfokek.sHtML

[T17] Swift：变量与常量
来源：http://mobile.hesvh.cn/Article/details/gzvndgxcx.sHtML

var a = 1;  let b = 2
来源：http://blog.fehbvm.com/Article/details/gbrzoytxu.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/grqluxirm.sHtML

"值: \(b)"
来源：http://mobile.fehbvm.com/Article/details/gjyeftvyc.sHtML

[T19] Swift：可选绑定
来源：http://wap.hesvh.cn/Article/details/gayimnngr.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.fehbvm.com/Article/details/gdyjqtdgw.sHtML

[T20] Swift：数组操作
来源：http://www.share.zdbjq.cn/Article/details/gdtlipgtl.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.zdbjq.cn/Article/details/gcbmtdcat.sHtML

[T21] Swift：遍历
来源：http://www.share.fehbvm.com/Article/details/gnjvqbtfy.sHtML

for x in a { print(x) }
来源：http://blog.zdbjq.cn/Article/details/goyhoqygy.sHtML

[T22] Swift：字典
来源：http://www.blog.zdbjq.cn/Article/details/gnvfszuqs.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.hesvh.cn/Article/details/gntmkkntn.sHtML

[T23] Swift：函数
来源：http://read.share.fehbvm.com/Article/details/gijquxvem.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.hesvh.cn/Article/details/gvfjsbvrq.sHtML

[T24] Swift：闭包
来源：http://mobile.hesvh.cn/Article/details/gmvqttbek.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gezyllgxq.sHtML

[T25] Swift：结构体
来源：http://www.share.zdbjq.cn/Article/details/gqrrgybtl.sHtML

struct P { var x: Int }
来源：http://mobile.zdbjq.cn/Article/details/gthsuihcv.sHtML

[T26] Swift：类与重写
来源：http://blog.zdbjq.cn/Article/details/gtiehqsig.sHtML

class A: Base { override func f() {} }
来源：http://m.share.zdbjq.cn/Article/details/gfdeericf.sHtML

[T27] Swift：错误处理
来源：http://mobile.zdbjq.cn/Article/details/gmmmhvzqs.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fehbvm.com/Article/details/gckoswrjz.sHtML

[T28] Swift：枚举
来源：http://3g.hesvh.cn/Article/details/gfjzqbqnx.sHtML

enum Color { case red, green }
来源：http://mobile.zdbjq.cn/Article/details/gnbxuioki.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.zdbjq.cn/Article/details/gzyzonblr.sHtML

guard let x = opt else { return }
来源：http://mobile.fehbvm.com/Article/details/gwksfyiiy.sHtML

[T30] Swift：协议
来源：http://www.share.hesvh.cn/Article/details/gqqyjjvsi.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fehbvm.com/Article/details/gyiqzfwjk.sHtML

[T31] Lua：Hello World
来源：http://baike.zdbjq.cn/Article/details/ggwkiotyj.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/gjkinyssq.sHtML

[T32] Lua：局部变量
来源：http://www.share.fehbvm.com/Article/details/gvoktclyi.sHtML

local a = 1
来源：http://www.m.share.hesvh.cn/Article/details/ghgwbvles.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.zdbjq.cn/Article/details/gfzmzmqix.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.hesvh.cn/Article/details/gzuoetvfh.sHtML

[T34] Lua：遍历表
来源：http://wap.zdbjq.cn/Article/details/gniqcuhae.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.zdbjq.cn/Article/details/goggqwgzf.sHtML

[T35] Lua：字典表
来源：http://baike.hesvh.cn/Article/details/gblkakuvo.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fehbvm.com/Article/details/gsawairwx.sHtML

[T36] Lua：函数
来源：http://mobile.fehbvm.com/Article/details/gmbhflwne.sHtML

function add(a, b) return a + b end
来源：http://www.blog.hesvh.cn/Article/details/gcbcwxind.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fehbvm.com/Article/details/gsojmmcpl.sHtML

"a" .. "b"
来源：http://www.blog.zdbjq.cn/Article/details/gzfdqedlx.sHtML

[T38] Lua：条件
来源：http://read.share.zdbjq.cn/Article/details/gerhuybhu.sHtML

if x > 0 then print("正") end
来源：http://read.share.hesvh.cn/Article/details/gvqfnxtrp.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.hesvh.cn/Article/details/guhkpbnny.sHtML

string.find(s, "%d+")
来源：http://read.share.hesvh.cn/Article/details/gsbuxuyls.sHtML

[T40] Lua：元表
来源：http://blog.fehbvm.com/Article/details/gnqztqivt.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.zdbjq.cn/Article/details/ghrfaowmw.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gadjxqewd.sHtML

print "Hello\n";
来源：http://m.share.hesvh.cn/Article/details/gacchtmnh.sHtML

[T42] Perl：变量类型
来源：http://3g.fehbvm.com/Article/details/gfqtlpuut.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.zdbjq.cn/Article/details/gnoaqzyum.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/guwkmnxvw.sHtML

"值: $a"
来源：http://wap.zdbjq.cn/Article/details/gmsrirglb.sHtML

[T44] Perl：条件
来源：http://wap.hesvh.cn/Article/details/gdznbjoed.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.fehbvm.com/Article/details/gmyematxh.sHtML

[T45] Perl：数组遍历
来源：http://3g.hesvh.cn/Article/details/gajmzeaqx.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.zdbjq.cn/Article/details/gcaaozovk.sHtML

[T46] Perl：哈希操作
来源：http://3g.fehbvm.com/Article/details/gbgvcwpqg.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.hesvh.cn/Article/details/gmnqfypda.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.zdbjq.cn/Article/details/gtozuwfzr.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.zdbjq.cn/Article/details/gfvkldyub.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.fehbvm.com/Article/details/gifluepyh.sHtML

$s =~ s/old/new/g;
来源：http://3g.hesvh.cn/Article/details/gujwtlftf.sHtML

[T49] Perl：函数
来源：http://blog.zdbjq.cn/Article/details/gazqnlczm.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gmvebtlwi.sHtML

[T50] Perl：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gqghwhlvl.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.zdbjq.cn/Article/details/gigqpfqzk.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.fehbvm.com/Article/details/gtyswkmjs.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gntfknymn.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/ghvhvezok.sHtML

[T52] Scala：变量
来源：http://www.blog.fehbvm.com/Article/details/geuaplewr.sHtML

val a = 1;  var b = 2
来源：http://blog.zdbjq.cn/Article/details/gjhstsxvi.sHtML

[T53] Scala：字符串插值
来源：http://3g.fehbvm.com/Article/details/gpakvnyuq.sHtML

s"值: $b"
来源：http://www.m.share.fehbvm.com/Article/details/ghfmbmatx.sHtML

[T54] Scala：集合映射
来源：http://blog.fehbvm.com/Article/details/gbwohkcut.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.fehbvm.com/Article/details/gdtixdjeq.sHtML

[T55] Scala：集合过滤
来源：http://m.share.hesvh.cn/Article/details/gazhnasyw.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.fehbvm.com/Article/details/gayeznvol.sHtML

[T56] Scala：样例类
来源：http://read.share.zdbjq.cn/Article/details/glkbqoxoz.sHtML

case class User(name: String, age: Int)
来源：http://baike.hesvh.cn/Article/details/gywdcozhk.sHtML

[T57] Scala：模式匹配
来源：http://m.share.zdbjq.cn/Article/details/gbrjwhemy.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.fehbvm.com/Article/details/gzattkltc.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.zdbjq.cn/Article/details/gdquqwrbm.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.fehbvm.com/Article/details/giekeikri.sHtML

[T59] Scala：循环
来源：http://baike.fehbvm.com/Article/details/glxzkjpyy.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.zdbjq.cn/Article/details/geadlmfen.sHtML

[T60] Scala：折叠
来源：http://read.share.fehbvm.com/Article/details/gxzefhiml.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.fehbvm.com/Article/details/gcyaqglzw.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ghfvbuhez.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.zdbjq.cn/Article/details/ggazplxpb.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ggqpchfgr.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.hesvh.cn/Article/details/ganavxgii.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.zdbjq.cn/Article/details/gitcqcjaq.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fehbvm.com/Article/details/gijfnaleq.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.fehbvm.com/Article/details/gfxfansuq.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.zdbjq.cn/Article/details/gckgvcskp.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.hesvh.cn/Article/details/ggeqtbwjq.sHtML

[U04] Py：变量调试打印
来源：http://blog.zdbjq.cn/Article/details/gtrfaxhfp.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.zdbjq.cn/Article/details/gfnzustun.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.fehbvm.com/Article/details/gosknojwu.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.hesvh.cn/Article/details/ggkkioudh.sHtML

[U06] Py：合并两个字典
来源：http://3g.hesvh.cn/Article/details/gzykeyhtv.sHtML

{**a, **b}
来源：http://baike.zdbjq.cn/Article/details/gxwytrwek.sHtML

[U07] Py：反转字典键值
来源：http://m.share.fehbvm.com/Article/details/geplelzyx.sHtML

{v: k for k, v in d.items()}
来源：http://wap.fehbvm.com/Article/details/gmgahybqd.sHtML

[U08] Py：展平二维列表
来源：http://m.share.fehbvm.com/Article/details/gqzdhwdtl.sHtML

[y for x in nested for y in x]
来源：http://www.share.hesvh.cn/Article/details/gmsfgjins.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.hesvh.cn/Article/details/gvwuoutud.sHtML

max(d, key=d.get)
来源：http://wap.fehbvm.com/Article/details/gpjxuqaje.sHtML

[U10] Py：按值排序字典
来源：http://m.share.zdbjq.cn/Article/details/grpsqbgdi.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.fehbvm.com/Article/details/ghjolaviv.sHtML

[U11] Py：生成器表达式
来源：http://3g.fehbvm.com/Article/details/gplymlkgq.sHtML

(x * 2 for x in arr)
来源：http://m.share.fehbvm.com/Article/details/gupbsodet.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.hesvh.cn/Article/details/gmtyiofyj.sHtML

Counter(arr).most_common(3)
来源：http://3g.fehbvm.com/Article/details/gjcyzxjjb.sHtML

[U13] Py：固定长度队列
来源：http://baike.hesvh.cn/Article/details/gsgnvbgcv.sHtML

deque(maxlen=10)
来源：http://www.blog.hesvh.cn/Article/details/gxfioxdmv.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.zdbjq.cn/Article/details/gjvkthaio.sHtML

defaultdict(list)
来源：http://read.share.zdbjq.cn/Article/details/goprhtvkx.sHtML

[U15] Py：高精度计时
来源：http://m.share.hesvh.cn/Article/details/gbhrqcoio.sHtML

t = time.perf_counter()
来源：http://3g.fehbvm.com/Article/details/graqjkonu.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.hesvh.cn/Article/details/giqadcbei.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.zdbjq.cn/Article/details/gupkrnfec.sHtML

[U17] Py：初始化日志
来源：http://m.share.fehbvm.com/Article/details/gzuvxylsw.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.zdbjq.cn/Article/details/gsxeeogrf.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.zdbjq.cn/Article/details/grzbljelc.sHtML

pat = re.compile(r"\d+")
来源：http://blog.fehbvm.com/Article/details/glvlpstvn.sHtML

[U19] Py：正则替换带回调
来源：http://baike.fehbvm.com/Article/details/gcckchkis.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.hesvh.cn/Article/details/gumkvxtiw.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.zdbjq.cn/Article/details/gntraaozs.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.zdbjq.cn/Article/details/gmhumioim.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.fehbvm.com/Article/details/gexgxnhcd.sHtML

@contextlib.contextmanager
来源：http://www.m.share.zdbjq.cn/Article/details/gocpitxkh.sHtML

[U22] Py：矩阵转置
来源：http://mobile.fehbvm.com/Article/details/gwubhscao.sHtML

list(zip(*m))
来源：http://www.m.share.hesvh.cn/Article/details/gwtdpezkm.sHtML

[U23] Py：分块读取大文件
来源：http://3g.fehbvm.com/Article/details/gruwhymih.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.zdbjq.cn/Article/details/gjlebokxk.sHtML

[U24] Py：路径操作
来源：http://read.share.hesvh.cn/Article/details/gcirczewl.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/gktxdyryd.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.fehbvm.com/Article/details/guuubthhi.sHtML

csv.DictReader(f)
来源：http://mobile.hesvh.cn/Article/details/gdxfmxirz.sHtML

[U26] Py：并发下载
来源：http://3g.zdbjq.cn/Article/details/ggcdcdgbe.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.hesvh.cn/Article/details/gbelwjsqh.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.zdbjq.cn/Article/details/gmnlneapv.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.fehbvm.com/Article/details/ghukeqqvj.sHtML

[U28] Py：类型别名
来源：http://blog.zdbjq.cn/Article/details/gxocmuofb.sHtML

UserId = int
来源：http://wap.zdbjq.cn/Article/details/gzzbcvdfu.sHtML

[U29] Py：属性校验
来源：http://www.blog.hesvh.cn/Article/details/gklswuggw.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.fehbvm.com/Article/details/grcfeqdrj.sHtML

[U30] Py：数据类
来源：http://3g.fehbvm.com/Article/details/grgdkurse.sHtML

@dataclass(slots=True)
来源：http://m.share.zdbjq.cn/Article/details/gtjnbhaxt.sHtML

[U31] Py：单测
来源：http://read.share.zdbjq.cn/Article/details/gnaiariws.sHtML

python -m pytest -q
来源：http://3g.fehbvm.com/Article/details/gtbpyhcif.sHtML

[U32] Py：代码格式化
来源：http://3g.zdbjq.cn/Article/details/gwnaemqwu.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.fehbvm.com/Article/details/guhxttjjg.sHtML

[U33] Py：打包发布
来源：http://blog.zdbjq.cn/Article/details/gpdgrhbez.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.hesvh.cn/Article/details/gtzqvotqy.sHtML

[U34] Py：判断编码
来源：http://blog.zdbjq.cn/Article/details/gjacfwlvh.sHtML

chardet.detect(raw)
来源：http://wap.hesvh.cn/Article/details/gdqbxkqfx.sHtML

[U35] Py：发送邮件
来源：http://www.blog.hesvh.cn/Article/details/gsbqfnfij.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.hesvh.cn/Article/details/gjisyiptd.sHtML

[U36] Py：定时任务
来源：http://blog.fehbvm.com/Article/details/geftvfojf.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.hesvh.cn/Article/details/gxnvgfwzf.sHtML

[U37] Py：读写 Excel
来源：http://read.share.zdbjq.cn/Article/details/gvxlnjven.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.fehbvm.com/Article/details/gwglecnmg.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.zdbjq.cn/Article/details/gwdtjnwuy.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.hesvh.cn/Article/details/gurumglpa.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.hesvh.cn/Article/details/gqezjrbhv.sHtML

sys.stdout.isatty()
来源：http://www.blog.hesvh.cn/Article/details/ggodkftlj.sHtML

[U40] Py：打印到标准错误
来源：http://3g.fehbvm.com/Article/details/goekvelrx.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.zdbjq.cn/Article/details/gtkbmnqmr.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.fehbvm.com/Article/details/gapcyvxsd.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.zdbjq.cn/Article/details/gqqbbpoqc.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.hesvh.cn/Article/details/galxscync.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.zdbjq.cn/Article/details/geqmfxvwg.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.zdbjq.cn/Article/details/gyjeimvbl.sHtML

namespace App\Http;
来源：http://www.share.hesvh.cn/Article/details/gypybyydr.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.zdbjq.cn/Article/details/gjrdrhmex.sHtML

declare(strict_types=1);
来源：http://www.share.zdbjq.cn/Article/details/gdeomnavx.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.zdbjq.cn/Article/details/gnkjihjzv.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gisblnzgg.sHtML

[U46] PHP：可空类型
来源：http://m.share.fehbvm.com/Article/details/gvzwnzegc.sHtML

?string $name = null
来源：http://mobile.zdbjq.cn/Article/details/gxhxlqibe.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.zdbjq.cn/Article/details/gbzbvqrmh.sHtML

int|string $id
来源：http://3g.hesvh.cn/Article/details/gevuleyjt.sHtML

[U48] PHP：纯枚举
来源：http://www.share.hesvh.cn/Article/details/gvmcddick.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.zdbjq.cn/Article/details/gaqkwfhtx.sHtML

[U49] PHP：只读属性
来源：http://3g.zdbjq.cn/Article/details/gokciauuc.sHtML

public readonly string $name
来源：http://m.share.fehbvm.com/Article/details/gerzecdde.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.zdbjq.cn/Article/details/gwcaovswc.sHtML

public function __construct(private int $id) {}
来源：http://blog.zdbjq.cn/Article/details/giiunritc.sHtML

[U51] PHP：数组解构
来源：http://www.blog.zdbjq.cn/Article/details/gzecalxsn.sHtML

[$a, $b] = $arr;
来源：http://read.share.zdbjq.cn/Article/details/gyhhfylyg.sHtML

[U52] PHP：箭头函数
来源：http://read.share.hesvh.cn/Article/details/gioytyjxd.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.zdbjq.cn/Article/details/gvruyarfi.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.zdbjq.cn/Article/details/gzeyajmij.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.zdbjq.cn/Article/details/gbcledsqr.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.hesvh.cn/Article/details/geqzocvgx.sHtML

$obj?->method()
来源：http://mobile.hesvh.cn/Article/details/gmrfyhdwm.sHtML

[U55] PHP：match 表达式
来源：http://blog.zdbjq.cn/Article/details/gqtozufep.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.zdbjq.cn/Article/details/gwlgdnsdm.sHtML

[U56] PHP：命名参数
来源：http://m.share.fehbvm.com/Article/details/gxbvtaumn.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/gbzdlfadk.sHtML

[U57] PHP：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gwxuoocml.sHtML

"值: {$a}"
来源：http://3g.fehbvm.com/Article/details/gbfgnfjxi.sHtML

[U58] PHP：数组三件套
来源：http://blog.fehbvm.com/Article/details/gcazujhfh.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.fehbvm.com/Article/details/gruecmzka.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.fehbvm.com/Article/details/gskcjlfby.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fehbvm.com/Article/details/gsrzwjayi.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.fehbvm.com/Article/details/gctgiuzwr.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.hesvh.cn/Article/details/gwitjimcv.sHtML

[U61] PHP：正则
来源：http://blog.hesvh.cn/Article/details/gbrohzrdd.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.zdbjq.cn/Article/details/gksduclbs.sHtML

[U62] PHP：日期对象
来源：http://wap.zdbjq.cn/Article/details/gcrrwjhwc.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.hesvh.cn/Article/details/gultynsdg.sHtML

[U63] PHP：文件读写
来源：http://read.share.fehbvm.com/Article/details/gyklzqfyj.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.zdbjq.cn/Article/details/ggknnbcoz.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.fehbvm.com/Article/details/gymfidypn.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.zdbjq.cn/Article/details/gpczupgke.sHtML

[U65] PHP：会话
来源：http://read.share.zdbjq.cn/Article/details/gelwrxavq.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gkaetixjw.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.zdbjq.cn/Article/details/goaagvlve.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.zdbjq.cn/Article/details/gnrglrmzo.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.zdbjq.cn/Article/details/gnakullan.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.fehbvm.com/Article/details/gaydfyawj.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.hesvh.cn/Article/details/garwnvubg.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.fehbvm.com/Article/details/gkzahrrfq.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.hesvh.cn/Article/details/gzzhislas.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.zdbjq.cn/Article/details/gxapimohy.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.fehbvm.com/Article/details/gytdahsih.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.hesvh.cn/Article/details/giqkjhrwc.sHtML

[U71] PHP：抛出异常
来源：http://wap.fehbvm.com/Article/details/ghhznficy.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.zdbjq.cn/Article/details/gudpzdgpd.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.fehbvm.com/Article/details/gzfqcaduj.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.fehbvm.com/Article/details/gwwtpwfiu.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.zdbjq.cn/Article/details/gratmgfms.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.hesvh.cn/Article/details/gpfgitsij.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.zdbjq.cn/Article/details/gdnthdmrd.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.fehbvm.com/Article/details/govnafhix.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.zdbjq.cn/Article/details/gmawghjuf.sHtML

composer require psr/container
来源：http://read.share.zdbjq.cn/Article/details/goropowgd.sHtML

[U76] PHP：简单路由
来源：http://www.share.hesvh.cn/Article/details/gbzipfiut.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.zdbjq.cn/Article/details/gdwfajvtt.sHtML

[U77] PHP：模板渲染
来源：http://mobile.fehbvm.com/Article/details/gvvgvbkjr.sHtML

composer require twig/twig
来源：http://www.m.share.zdbjq.cn/Article/details/glexvpqwa.sHtML

[U78] PHP：单元测试
来源：http://m.share.fehbvm.com/Article/details/gpftpmtji.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.zdbjq.cn/Article/details/gjwzngxcx.sHtML

[U79] PHP：静态分析
来源：http://read.share.zdbjq.cn/Article/details/gqwbqdxfk.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.fehbvm.com/Article/details/goykgdqis.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.zdbjq.cn/Article/details/grarprclt.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.hesvh.cn/Article/details/gcqzauttg.sHtML

[U81] JS：初始化项目
来源：http://baike.hesvh.cn/Article/details/gvwameoav.sHtML

npm init -y;  npm i express
来源：http://wap.fehbvm.com/Article/details/gpldxnscn.sHtML

[U82] JS：package.json 脚本
来源：http://baike.hesvh.cn/Article/details/gdesuakcs.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.fehbvm.com/Article/details/grpaelchx.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.fehbvm.com/Article/details/gfxevomly.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.hesvh.cn/Article/details/gapkeihbw.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.zdbjq.cn/Article/details/gydoundpq.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.zdbjq.cn/Article/details/gstubtdlo.sHtML

[U85] JS：可选链
来源：http://wap.hesvh.cn/Article/details/gezdhobuh.sHtML

a?.b?.c
来源：http://blog.zdbjq.cn/Article/details/gyzcyhysp.sHtML

[U86] JS：空值合并
来源：http://blog.zdbjq.cn/Article/details/guyrpewai.sHtML

a ?? b
来源：http://www.m.share.zdbjq.cn/Article/details/gmcpjyulu.sHtML

[U87] JS：解构默认值
来源：http://mobile.hesvh.cn/Article/details/gkslgfdvd.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.zdbjq.cn/Article/details/gskexgora.sHtML

[U88] JS：对象展开合并
来源：http://m.share.hesvh.cn/Article/details/gmjncqnxa.sHtML

{ ...a, ...b }
来源：http://3g.zdbjq.cn/Article/details/gvikxrhdk.sHtML

[U89] JS：数组去重
来源：http://read.share.hesvh.cn/Article/details/gdulakokw.sHtML

[...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/gdjkmhxgx.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.zdbjq.cn/Article/details/giwxpdplj.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/gztmdmcgu.sHtML

[U91] JS：对象键值遍历
来源：http://blog.fehbvm.com/Article/details/gnoxebpxj.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.zdbjq.cn/Article/details/gacgyrslk.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gjzlhciij.sHtML

structuredClone(obj)
来源：http://www.m.share.hesvh.cn/Article/details/getpigatu.sHtML


<!-- 参考信息 -->