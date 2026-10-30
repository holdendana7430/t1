代发 wailian999

[T01] Kotlin：Hello World
来源：http://wap.fehbvm.com/Article/details/gqgemkijc.sHtML

println("Hello")
来源：http://3g.hesvh.cn/Article/details/gufacigaj.sHtML

[T02] Kotlin：变量
来源：http://3g.fehbvm.com/Article/details/gusidfuii.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.zdbjq.cn/Article/details/gmjxsxhkk.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.zdbjq.cn/Article/details/gkyapacnn.sHtML

"值: $b"
来源：http://read.share.zdbjq.cn/Article/details/guvautyij.sHtML

[T04] Kotlin：空安全
来源：http://wap.hesvh.cn/Article/details/gydjimetz.sHtML

val n: String? = null;  n?.length
来源：http://wap.zdbjq.cn/Article/details/gophodmzv.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.hesvh.cn/Article/details/gsxpuptat.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.hesvh.cn/Article/details/gdcmpkobm.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/gmzudddun.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gezrgghkp.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.hesvh.cn/Article/details/gpdpbjini.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.hesvh.cn/Article/details/gcinyrncp.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fehbvm.com/Article/details/gojrkumst.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fehbvm.com/Article/details/ggimqwvty.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.hesvh.cn/Article/details/gxdafquwi.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.hesvh.cn/Article/details/ghovhxfip.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fehbvm.com/Article/details/gcnvlvnvx.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fehbvm.com/Article/details/ggflwiewp.sHtML

[T11] Kotlin：协程
来源：http://www.share.hesvh.cn/Article/details/ggzgolzwo.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.zdbjq.cn/Article/details/gqwknlwwv.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fehbvm.com/Article/details/gzhkagilc.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/ghholvyvk.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.zdbjq.cn/Article/details/gcritbwrd.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fehbvm.com/Article/details/gnihqqckq.sHtML

[T14] Kotlin：循环
来源：http://m.share.hesvh.cn/Article/details/gwfpfxdjg.sHtML

for (i in 1..10) println(i)
来源：http://baike.zdbjq.cn/Article/details/ggemzjixc.sHtML

[T15] Kotlin：接口
来源：http://www.blog.zdbjq.cn/Article/details/gbwzowclr.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.fehbvm.com/Article/details/gouxyheyi.sHtML

[T16] Swift：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gdlkkeckq.sHtML

print("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gxtmcqlob.sHtML

[T17] Swift：变量与常量
来源：http://wap.hesvh.cn/Article/details/gqlqixzia.sHtML

var a = 1;  let b = 2
来源：http://wap.zdbjq.cn/Article/details/gxvlltwjg.sHtML

[T18] Swift：字符串插值
来源：http://wap.hesvh.cn/Article/details/gfzhlvnzz.sHtML

"值: \(b)"
来源：http://baike.zdbjq.cn/Article/details/gylbwuweu.sHtML

[T19] Swift：可选绑定
来源：http://wap.zdbjq.cn/Article/details/gqwczjcmy.sHtML

if let n = opt { print(n) }
来源：http://baike.zdbjq.cn/Article/details/gdbgohwdr.sHtML

[T20] Swift：数组操作
来源：http://read.share.hesvh.cn/Article/details/gqestifhs.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.hesvh.cn/Article/details/guuuhwqqf.sHtML

[T21] Swift：遍历
来源：http://www.m.share.fehbvm.com/Article/details/gpuwokesv.sHtML

for x in a { print(x) }
来源：http://mobile.zdbjq.cn/Article/details/gtbsomjkf.sHtML

[T22] Swift：字典
来源：http://mobile.fehbvm.com/Article/details/gbfbrteho.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.hesvh.cn/Article/details/goxvadann.sHtML

[T23] Swift：函数
来源：http://wap.fehbvm.com/Article/details/gxfgpkorn.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fehbvm.com/Article/details/giegrnwdt.sHtML

[T24] Swift：闭包
来源：http://wap.zdbjq.cn/Article/details/gxkgqnmic.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.hesvh.cn/Article/details/gvjbbcdjv.sHtML

[T25] Swift：结构体
来源：http://wap.hesvh.cn/Article/details/giwabgjiz.sHtML

struct P { var x: Int }
来源：http://wap.hesvh.cn/Article/details/gfwnopaaq.sHtML

[T26] Swift：类与重写
来源：http://mobile.fehbvm.com/Article/details/grjfhtzpw.sHtML

class A: Base { override func f() {} }
来源：http://3g.fehbvm.com/Article/details/goinhlext.sHtML

[T27] Swift：错误处理
来源：http://baike.fehbvm.com/Article/details/ggdwgmlez.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.hesvh.cn/Article/details/gjfwmuqtn.sHtML

[T28] Swift：枚举
来源：http://blog.hesvh.cn/Article/details/gthowrdaq.sHtML

enum Color { case red, green }
来源：http://mobile.hesvh.cn/Article/details/gnznaxxre.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.zdbjq.cn/Article/details/goxjlhszk.sHtML

guard let x = opt else { return }
来源：http://www.share.fehbvm.com/Article/details/grqzlykyn.sHtML

[T30] Swift：协议
来源：http://www.blog.zdbjq.cn/Article/details/gozpbpcre.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fehbvm.com/Article/details/gqipkovdj.sHtML

[T31] Lua：Hello World
来源：http://mobile.hesvh.cn/Article/details/grcispgvk.sHtML

print("Hello")
来源：http://wap.fehbvm.com/Article/details/gnfwpdvvb.sHtML

[T32] Lua：局部变量
来源：http://read.share.fehbvm.com/Article/details/gqnpxlhdj.sHtML

local a = 1
来源：http://baike.zdbjq.cn/Article/details/gnkiegamk.sHtML

[T33] Lua：表（数组）
来源：http://wap.hesvh.cn/Article/details/givdiiumc.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.zdbjq.cn/Article/details/glkgcqyal.sHtML

[T34] Lua：遍历表
来源：http://www.blog.zdbjq.cn/Article/details/gknbbkkvj.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fehbvm.com/Article/details/grraqnrms.sHtML

[T35] Lua：字典表
来源：http://www.blog.zdbjq.cn/Article/details/gvmfxawpk.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.zdbjq.cn/Article/details/gkvojssxr.sHtML

[T36] Lua：函数
来源：http://wap.zdbjq.cn/Article/details/ggjssgerg.sHtML

function add(a, b) return a + b end
来源：http://3g.hesvh.cn/Article/details/gavdllzgi.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.zdbjq.cn/Article/details/gqbmtdsvg.sHtML

"a" .. "b"
来源：http://m.share.hesvh.cn/Article/details/gqnxwnvmk.sHtML

[T38] Lua：条件
来源：http://mobile.zdbjq.cn/Article/details/gytfjkqhz.sHtML

if x > 0 then print("正") end
来源：http://www.blog.hesvh.cn/Article/details/giwrpoyqh.sHtML

[T39] Lua：模式匹配
来源：http://blog.fehbvm.com/Article/details/gxxicxuco.sHtML

string.find(s, "%d+")
来源：http://www.share.hesvh.cn/Article/details/giekfdcyk.sHtML

[T40] Lua：元表
来源：http://www.m.share.zdbjq.cn/Article/details/grcykzcax.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.fehbvm.com/Article/details/gfdpnentj.sHtML

[T41] Perl：Hello World
来源：http://baike.zdbjq.cn/Article/details/gntyeymwp.sHtML

print "Hello\n";
来源：http://baike.fehbvm.com/Article/details/geeddayjs.sHtML

[T42] Perl：变量类型
来源：http://m.share.zdbjq.cn/Article/details/gxmocxkcb.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.hesvh.cn/Article/details/gcegwxrwk.sHtML

[T43] Perl：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gsyotakwi.sHtML

"值: $a"
来源：http://mobile.zdbjq.cn/Article/details/gxbugwnoo.sHtML

[T44] Perl：条件
来源：http://baike.hesvh.cn/Article/details/ghxsbjvji.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.hesvh.cn/Article/details/grjoeimsk.sHtML

[T45] Perl：数组遍历
来源：http://3g.fehbvm.com/Article/details/gphvrpaty.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.fehbvm.com/Article/details/ggmqbbawe.sHtML

[T46] Perl：哈希操作
来源：http://read.share.hesvh.cn/Article/details/gwwpcgnso.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.hesvh.cn/Article/details/gixchfxcc.sHtML

[T47] Perl：正则捕获
来源：http://wap.fehbvm.com/Article/details/gbysrphzq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.fehbvm.com/Article/details/gvcjuwpmp.sHtML

[T48] Perl：正则替换
来源：http://mobile.fehbvm.com/Article/details/gnzgfhdpg.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.fehbvm.com/Article/details/glmvahvuu.sHtML

[T49] Perl：函数
来源：http://www.share.zdbjq.cn/Article/details/gutupdbov.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/ggltflwef.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/grfvgtojm.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.hesvh.cn/Article/details/gjbuallqq.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.hesvh.cn/Article/details/ghdbiqhzs.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gjzfwxerb.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/gjvuqztoq.sHtML

[T52] Scala：变量
来源：http://wap.hesvh.cn/Article/details/gamhhupxx.sHtML

val a = 1;  var b = 2
来源：http://www.share.hesvh.cn/Article/details/gaysintgd.sHtML

[T53] Scala：字符串插值
来源：http://wap.fehbvm.com/Article/details/gkbvcqolc.sHtML

s"值: $b"
来源：http://blog.zdbjq.cn/Article/details/gxjzcjmpb.sHtML

[T54] Scala：集合映射
来源：http://wap.zdbjq.cn/Article/details/gygamsaih.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gmpmchorg.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fehbvm.com/Article/details/gvhaciiyz.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.fehbvm.com/Article/details/gpueikzuh.sHtML

[T56] Scala：样例类
来源：http://www.blog.hesvh.cn/Article/details/gjrsihbia.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.zdbjq.cn/Article/details/gqzqeyust.sHtML

[T57] Scala：模式匹配
来源：http://read.share.hesvh.cn/Article/details/gbqrlyunt.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.zdbjq.cn/Article/details/gifmxykks.sHtML

[T58] Scala：函数定义
来源：http://read.share.hesvh.cn/Article/details/gmjrgfved.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.fehbvm.com/Article/details/gcvlrnbai.sHtML

[T59] Scala：循环
来源：http://blog.fehbvm.com/Article/details/gmwbuafmi.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.fehbvm.com/Article/details/gkvnkulxc.sHtML

[T60] Scala：折叠
来源：http://www.m.share.zdbjq.cn/Article/details/gbalkhyzf.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.hesvh.cn/Article/details/guvylreat.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gtxukipfe.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fehbvm.com/Article/details/gseybjdua.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/goofsffue.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.zdbjq.cn/Article/details/gpqlygszc.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.fehbvm.com/Article/details/gtstbltbp.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.hesvh.cn/Article/details/gzlqafjha.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.hesvh.cn/Article/details/gystwnibg.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.fehbvm.com/Article/details/gmemwxxqo.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.zdbjq.cn/Article/details/gohlpebcs.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.zdbjq.cn/Article/details/ggkrjekjo.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.hesvh.cn/Article/details/ghichnwoq.sHtML

[U05] Py：列表去重且保序
来源：http://3g.zdbjq.cn/Article/details/gstqdlbgg.sHtML

list(dict.fromkeys(arr))
来源：http://wap.zdbjq.cn/Article/details/gwxrkkwbu.sHtML

[U06] Py：合并两个字典
来源：http://3g.hesvh.cn/Article/details/gdceyvcro.sHtML

{**a, **b}
来源：http://wap.zdbjq.cn/Article/details/gxyfvvgtd.sHtML

[U07] Py：反转字典键值
来源：http://blog.zdbjq.cn/Article/details/gqfeljilq.sHtML

{v: k for k, v in d.items()}
来源：http://3g.hesvh.cn/Article/details/gzgjkvkfd.sHtML

[U08] Py：展平二维列表
来源：http://blog.fehbvm.com/Article/details/glggrtplz.sHtML

[y for x in nested for y in x]
来源：http://www.share.zdbjq.cn/Article/details/gofmcbmpy.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.zdbjq.cn/Article/details/gmwkvpmqz.sHtML

max(d, key=d.get)
来源：http://3g.hesvh.cn/Article/details/gaeakvmba.sHtML

[U10] Py：按值排序字典
来源：http://m.share.fehbvm.com/Article/details/gavajuixy.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.fehbvm.com/Article/details/goueqrpjp.sHtML

[U11] Py：生成器表达式
来源：http://wap.hesvh.cn/Article/details/gttrlzldy.sHtML

(x * 2 for x in arr)
来源：http://mobile.hesvh.cn/Article/details/gukknmchs.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.fehbvm.com/Article/details/geyaratgx.sHtML

Counter(arr).most_common(3)
来源：http://read.share.hesvh.cn/Article/details/glbogabwh.sHtML

[U13] Py：固定长度队列
来源：http://baike.zdbjq.cn/Article/details/groitopvp.sHtML

deque(maxlen=10)
来源：http://baike.zdbjq.cn/Article/details/glksmrsgb.sHtML

[U14] Py：分组收集到列表
来源：http://3g.zdbjq.cn/Article/details/gfrdhgren.sHtML

defaultdict(list)
来源：http://mobile.zdbjq.cn/Article/details/gthxoeula.sHtML

[U15] Py：高精度计时
来源：http://blog.hesvh.cn/Article/details/gyhspitme.sHtML

t = time.perf_counter()
来源：http://www.blog.hesvh.cn/Article/details/gzuogmjcw.sHtML

[U16] Py：命令行参数解析
来源：http://baike.hesvh.cn/Article/details/gzdchbzrx.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.fehbvm.com/Article/details/gdfvltgmb.sHtML

[U17] Py：初始化日志
来源：http://m.share.fehbvm.com/Article/details/glsrvidcr.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.hesvh.cn/Article/details/gchhxpieb.sHtML

[U18] Py：预编译正则
来源：http://read.share.hesvh.cn/Article/details/gneqtdpus.sHtML

pat = re.compile(r"\d+")
来源：http://blog.fehbvm.com/Article/details/gvpgmossh.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.zdbjq.cn/Article/details/gsyfztdky.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.zdbjq.cn/Article/details/gndxxwoul.sHtML

[U20] Py：缓存函数结果
来源：http://wap.zdbjq.cn/Article/details/gswkgopqr.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.hesvh.cn/Article/details/gtzafgybr.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.zdbjq.cn/Article/details/gjviyxuym.sHtML

@contextlib.contextmanager
来源：http://read.share.zdbjq.cn/Article/details/glcyblsof.sHtML

[U22] Py：矩阵转置
来源：http://m.share.zdbjq.cn/Article/details/gvgjavegi.sHtML

list(zip(*m))
来源：http://blog.fehbvm.com/Article/details/ghtxdmdap.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.zdbjq.cn/Article/details/gzflylgde.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.hesvh.cn/Article/details/gnvzdtlwf.sHtML

[U24] Py：路径操作
来源：http://read.share.hesvh.cn/Article/details/gcgfvlfdp.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/gwouycuhn.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.hesvh.cn/Article/details/gloonmaim.sHtML

csv.DictReader(f)
来源：http://read.share.hesvh.cn/Article/details/gdmuqpmrs.sHtML

[U26] Py：并发下载
来源：http://www.share.fehbvm.com/Article/details/ghammdqvh.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.fehbvm.com/Article/details/gjdcupxdc.sHtML

[U27] Py：异步 HTTP
来源：http://blog.zdbjq.cn/Article/details/gxjjcyvbk.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.hesvh.cn/Article/details/grswozjad.sHtML

[U28] Py：类型别名
来源：http://www.share.fehbvm.com/Article/details/guambflon.sHtML

UserId = int
来源：http://wap.zdbjq.cn/Article/details/gkgizmjqm.sHtML

[U29] Py：属性校验
来源：http://m.share.hesvh.cn/Article/details/gwhnkyxdw.sHtML

@property 与 @x.setter 配合
来源：http://blog.hesvh.cn/Article/details/geopqghjv.sHtML

[U30] Py：数据类
来源：http://3g.fehbvm.com/Article/details/gkgcvhrpi.sHtML

@dataclass(slots=True)
来源：http://read.share.fehbvm.com/Article/details/gidftiouc.sHtML

[U31] Py：单测
来源：http://wap.hesvh.cn/Article/details/gyraqgady.sHtML

python -m pytest -q
来源：http://3g.zdbjq.cn/Article/details/gezkywjkj.sHtML

[U32] Py：代码格式化
来源：http://blog.zdbjq.cn/Article/details/ghoenfwpb.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.zdbjq.cn/Article/details/gveybwqig.sHtML

[U33] Py：打包发布
来源：http://wap.hesvh.cn/Article/details/giukjppin.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.fehbvm.com/Article/details/gsyzdmmcx.sHtML

[U34] Py：判断编码
来源：http://baike.fehbvm.com/Article/details/gulcjnbvk.sHtML

chardet.detect(raw)
来源：http://3g.fehbvm.com/Article/details/gevkmcclp.sHtML

[U35] Py：发送邮件
来源：http://read.share.zdbjq.cn/Article/details/gcnuqwobh.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.zdbjq.cn/Article/details/gtvlvcsgn.sHtML

[U36] Py：定时任务
来源：http://read.share.fehbvm.com/Article/details/gqmbebupw.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.zdbjq.cn/Article/details/gbhdpaxqw.sHtML

[U37] Py：读写 Excel
来源：http://blog.hesvh.cn/Article/details/gdamhvuwf.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.fehbvm.com/Article/details/gncqytphm.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.fehbvm.com/Article/details/gcsutpgpx.sHtML

Path(__file__).resolve().parent
来源：http://read.share.fehbvm.com/Article/details/grylhnffs.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.hesvh.cn/Article/details/gbfphuici.sHtML

sys.stdout.isatty()
来源：http://mobile.fehbvm.com/Article/details/gagkahpod.sHtML

[U40] Py：打印到标准错误
来源：http://blog.fehbvm.com/Article/details/gzqsgdizq.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.zdbjq.cn/Article/details/gluyhukbj.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.zdbjq.cn/Article/details/gsdkqxhrn.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.fehbvm.com/Article/details/guaamwcss.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.zdbjq.cn/Article/details/gfrtsbnlk.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.fehbvm.com/Article/details/geaubxuaj.sHtML

[U43] PHP：声明命名空间
来源：http://3g.fehbvm.com/Article/details/ghzlnwooz.sHtML

namespace App\Http;
来源：http://m.share.hesvh.cn/Article/details/gwlwpjdwh.sHtML

[U44] PHP：开启严格类型
来源：http://blog.fehbvm.com/Article/details/gfdckduzj.sHtML

declare(strict_types=1);
来源：http://baike.fehbvm.com/Article/details/gokvdkhtm.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.hesvh.cn/Article/details/gjwdlgill.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gythceoqg.sHtML

[U46] PHP：可空类型
来源：http://www.share.hesvh.cn/Article/details/goznvhokd.sHtML

?string $name = null
来源：http://wap.fehbvm.com/Article/details/gkhkwrmpp.sHtML

[U47] PHP：联合类型
来源：http://wap.zdbjq.cn/Article/details/gbufzlzek.sHtML

int|string $id
来源：http://mobile.zdbjq.cn/Article/details/gymcvujmi.sHtML

[U48] PHP：纯枚举
来源：http://3g.hesvh.cn/Article/details/gzgewwdkr.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.hesvh.cn/Article/details/gbqhztaib.sHtML

[U49] PHP：只读属性
来源：http://blog.hesvh.cn/Article/details/goxklgifa.sHtML

public readonly string $name
来源：http://www.blog.fehbvm.com/Article/details/giyyandpd.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.fehbvm.com/Article/details/gwqtnktmj.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.hesvh.cn/Article/details/grfcqhwqq.sHtML

[U51] PHP：数组解构
来源：http://www.share.fehbvm.com/Article/details/gqzbxkzgy.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.zdbjq.cn/Article/details/gwapxbpre.sHtML

[U52] PHP：箭头函数
来源：http://3g.fehbvm.com/Article/details/gizyskmjs.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.hesvh.cn/Article/details/gqnkzikor.sHtML

[U53] PHP：空合并运算符
来源：http://3g.fehbvm.com/Article/details/gxbjroiuo.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.fehbvm.com/Article/details/grzeddusg.sHtML

[U54] PHP：空安全调用
来源：http://mobile.zdbjq.cn/Article/details/gpndwvtfg.sHtML

$obj?->method()
来源：http://www.share.hesvh.cn/Article/details/gjsdnucem.sHtML

[U55] PHP：match 表达式
来源：http://www.share.zdbjq.cn/Article/details/gwzjluvay.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.fehbvm.com/Article/details/guwtuffxl.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.fehbvm.com/Article/details/gerinhtwc.sHtML

f(a: 1, b: 2)
来源：http://wap.zdbjq.cn/Article/details/guwhbyxuu.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gtzncqiuk.sHtML

"值: {$a}"
来源：http://m.share.hesvh.cn/Article/details/gbzbsugde.sHtML

[U58] PHP：数组三件套
来源：http://mobile.zdbjq.cn/Article/details/gaufcavri.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.fehbvm.com/Article/details/gctkydjvs.sHtML

[U59] PHP：自定义排序
来源：http://wap.zdbjq.cn/Article/details/gmwwaudgc.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.zdbjq.cn/Article/details/gcstqdiwa.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.fehbvm.com/Article/details/gyjblfcmp.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.fehbvm.com/Article/details/gydoncrpd.sHtML

[U61] PHP：正则
来源：http://read.share.fehbvm.com/Article/details/gzesfudnz.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.hesvh.cn/Article/details/goawrjvme.sHtML

[U62] PHP：日期对象
来源：http://m.share.hesvh.cn/Article/details/gizhyarab.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.zdbjq.cn/Article/details/gywghzshj.sHtML

[U63] PHP：文件读写
来源：http://www.share.hesvh.cn/Article/details/glsnyeexh.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.hesvh.cn/Article/details/giwkzmght.sHtML

[U64] PHP：目录遍历
来源：http://blog.fehbvm.com/Article/details/gjottpnxv.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.fehbvm.com/Article/details/gvtuiqmoa.sHtML

[U65] PHP：会话
来源：http://read.share.fehbvm.com/Article/details/gbcnmtvln.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gzbmujqst.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.hesvh.cn/Article/details/gdabqtfrh.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.hesvh.cn/Article/details/gysmvhxiz.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.hesvh.cn/Article/details/gqmkrfmtc.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.zdbjq.cn/Article/details/gzirkklkv.sHtML

[U68] PHP：PDO 连接
来源：http://blog.zdbjq.cn/Article/details/golosvtlj.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.fehbvm.com/Article/details/gpvzoqhwr.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.fehbvm.com/Article/details/ghgyfreul.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.hesvh.cn/Article/details/gvtqqrznf.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.hesvh.cn/Article/details/gzivvcudt.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.fehbvm.com/Article/details/gofoymhef.sHtML

[U71] PHP：抛出异常
来源：http://wap.hesvh.cn/Article/details/geegxefxf.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.fehbvm.com/Article/details/gekfpdfad.sHtML

[U72] PHP：写错误日志
来源：http://blog.hesvh.cn/Article/details/gxirofmnz.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.fehbvm.com/Article/details/ggpuueiyr.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.fehbvm.com/Article/details/gesuxgfsq.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.zdbjq.cn/Article/details/ggnazdsuu.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.fehbvm.com/Article/details/gtwbzwcsx.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.fehbvm.com/Article/details/grizgxpys.sHtML

[U75] PHP：依赖注入
来源：http://www.share.fehbvm.com/Article/details/goizrnrmm.sHtML

composer require psr/container
来源：http://mobile.hesvh.cn/Article/details/gwwtuyarf.sHtML

[U76] PHP：简单路由
来源：http://blog.hesvh.cn/Article/details/ghwoqrruk.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.fehbvm.com/Article/details/gcymmajtg.sHtML

[U77] PHP：模板渲染
来源：http://baike.zdbjq.cn/Article/details/gvhtxahwe.sHtML

composer require twig/twig
来源：http://www.blog.fehbvm.com/Article/details/gbsisqqli.sHtML

[U78] PHP：单元测试
来源：http://read.share.hesvh.cn/Article/details/gybvtjvcf.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.zdbjq.cn/Article/details/gceexidnn.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.hesvh.cn/Article/details/gocpqsevj.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.zdbjq.cn/Article/details/gyyceuens.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.zdbjq.cn/Article/details/gltfiybsd.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.fehbvm.com/Article/details/gqtajrxfx.sHtML

[U81] JS：初始化项目
来源：http://www.share.hesvh.cn/Article/details/givytlyoa.sHtML

npm init -y;  npm i express
来源：http://read.share.hesvh.cn/Article/details/gvjgbimlb.sHtML

[U82] JS：package.json 脚本
来源：http://blog.hesvh.cn/Article/details/ghvejtetf.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.fehbvm.com/Article/details/gtvweahal.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.fehbvm.com/Article/details/gjrdhybaf.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.fehbvm.com/Article/details/geexfyknx.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.fehbvm.com/Article/details/gdvzywdwn.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.zdbjq.cn/Article/details/goaeugaxe.sHtML

[U85] JS：可选链
来源：http://www.blog.hesvh.cn/Article/details/grhykupwk.sHtML

a?.b?.c
来源：http://3g.zdbjq.cn/Article/details/glvmqsxck.sHtML

[U86] JS：空值合并
来源：http://blog.zdbjq.cn/Article/details/gbgjehjey.sHtML

a ?? b
来源：http://read.share.zdbjq.cn/Article/details/gnpkyokwx.sHtML

[U87] JS：解构默认值
来源：http://3g.fehbvm.com/Article/details/gawcoquve.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.zdbjq.cn/Article/details/gwbtwklhg.sHtML

[U88] JS：对象展开合并
来源：http://baike.zdbjq.cn/Article/details/gqlvtvdqy.sHtML

{ ...a, ...b }
来源：http://3g.hesvh.cn/Article/details/gfyuralbc.sHtML


<!-- 参考信息 -->