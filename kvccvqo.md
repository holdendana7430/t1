代发 wailian999

[T03] Kotlin：字符串模板
来源：http://www.share.zdbjq.cn/Article/details/gtzultppi.sHtML

"值: $b"
来源：http://m.share.fehbvm.com/Article/details/gzhmcalnf.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fehbvm.com/Article/details/gpmilswdb.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fehbvm.com/Article/details/gzobawrfy.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fehbvm.com/Article/details/gprbzqapo.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.hesvh.cn/Article/details/gsijcrvus.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.zdbjq.cn/Article/details/gvesdyeia.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.zdbjq.cn/Article/details/gdluaxfun.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.hesvh.cn/Article/details/grgqcqohk.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.hesvh.cn/Article/details/gmdmxyblj.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fehbvm.com/Article/details/gqzrbhivk.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.zdbjq.cn/Article/details/gaebesirn.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fehbvm.com/Article/details/gbxqoccsi.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.zdbjq.cn/Article/details/ggkhuqinc.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.hesvh.cn/Article/details/gtbjmsquc.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fehbvm.com/Article/details/gmhzcncqp.sHtML

[T11] Kotlin：协程
来源：http://blog.zdbjq.cn/Article/details/gnjsobvcq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.hesvh.cn/Article/details/gdaffqyyt.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.zdbjq.cn/Article/details/gkofoiyle.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.hesvh.cn/Article/details/giljzbstr.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.hesvh.cn/Article/details/gntxkvucj.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.zdbjq.cn/Article/details/gioyvtbiq.sHtML

[T14] Kotlin：循环
来源：http://wap.fehbvm.com/Article/details/gnafwshpv.sHtML

for (i in 1..10) println(i)
来源：http://wap.zdbjq.cn/Article/details/gxnzhysrr.sHtML

[T15] Kotlin：接口
来源：http://m.share.hesvh.cn/Article/details/gbuftcftf.sHtML

interface Shape { fun area(): Double }
来源：http://wap.hesvh.cn/Article/details/gzdleafit.sHtML

[T16] Swift：Hello World
来源：http://www.share.zdbjq.cn/Article/details/giqowdums.sHtML

print("Hello")
来源：http://blog.zdbjq.cn/Article/details/grohnfgyz.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fehbvm.com/Article/details/gozjpngar.sHtML

var a = 1;  let b = 2
来源：http://3g.zdbjq.cn/Article/details/gffkfjcgb.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gmuvarjco.sHtML

"值: \(b)"
来源：http://baike.fehbvm.com/Article/details/gwyzsywev.sHtML

[T19] Swift：可选绑定
来源：http://wap.zdbjq.cn/Article/details/gckcrefjd.sHtML

if let n = opt { print(n) }
来源：http://wap.zdbjq.cn/Article/details/ggypgtcxr.sHtML

[T20] Swift：数组操作
来源：http://mobile.hesvh.cn/Article/details/gnhyofsfr.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fehbvm.com/Article/details/gkrxilylu.sHtML

[T21] Swift：遍历
来源：http://m.share.zdbjq.cn/Article/details/gbkamletm.sHtML

for x in a { print(x) }
来源：http://m.share.hesvh.cn/Article/details/gpypgfmqz.sHtML

[T22] Swift：字典
来源：http://3g.hesvh.cn/Article/details/grtflsnid.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.zdbjq.cn/Article/details/gehlsjvup.sHtML

[T23] Swift：函数
来源：http://3g.fehbvm.com/Article/details/gmibxowok.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.fehbvm.com/Article/details/geucdloqu.sHtML

[T24] Swift：闭包
来源：http://baike.fehbvm.com/Article/details/guafuyvdi.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.hesvh.cn/Article/details/gdstztubo.sHtML

[T25] Swift：结构体
来源：http://m.share.fehbvm.com/Article/details/gggxcolhm.sHtML

struct P { var x: Int }
来源：http://wap.zdbjq.cn/Article/details/gfwogazzl.sHtML

[T26] Swift：类与重写
来源：http://www.share.zdbjq.cn/Article/details/gmzhdwdkc.sHtML

class A: Base { override func f() {} }
来源：http://baike.zdbjq.cn/Article/details/gizntauhz.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.zdbjq.cn/Article/details/gbgbvsagi.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fehbvm.com/Article/details/gphsplrat.sHtML

[T28] Swift：枚举
来源：http://mobile.hesvh.cn/Article/details/gtycusyze.sHtML

enum Color { case red, green }
来源：http://m.share.hesvh.cn/Article/details/gtsxmtatm.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fehbvm.com/Article/details/guvcpcfyr.sHtML

guard let x = opt else { return }
来源：http://baike.zdbjq.cn/Article/details/gjzlfzqch.sHtML

[T30] Swift：协议
来源：http://wap.fehbvm.com/Article/details/ginofxdpy.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.zdbjq.cn/Article/details/gyrlxujjz.sHtML

[T31] Lua：Hello World
来源：http://mobile.fehbvm.com/Article/details/gdvlekjsm.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gwvsxwgaa.sHtML

[T32] Lua：局部变量
来源：http://www.blog.fehbvm.com/Article/details/ggkgiahfv.sHtML

local a = 1
来源：http://www.blog.fehbvm.com/Article/details/gdcopftdg.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.hesvh.cn/Article/details/gjtabvugv.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.hesvh.cn/Article/details/goioptikb.sHtML

[T34] Lua：遍历表
来源：http://mobile.hesvh.cn/Article/details/gnbyjvohk.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.hesvh.cn/Article/details/gqbypcdpr.sHtML

[T35] Lua：字典表
来源：http://baike.hesvh.cn/Article/details/gypmiqbfr.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.hesvh.cn/Article/details/gmofgnurq.sHtML

[T36] Lua：函数
来源：http://3g.zdbjq.cn/Article/details/glqfotyrw.sHtML

function add(a, b) return a + b end
来源：http://read.share.hesvh.cn/Article/details/gfzejqpjc.sHtML

[T37] Lua：字符串拼接
来源：http://baike.fehbvm.com/Article/details/gnslowqcf.sHtML

"a" .. "b"
来源：http://wap.fehbvm.com/Article/details/gkdxnyyki.sHtML

[T38] Lua：条件
来源：http://mobile.hesvh.cn/Article/details/gybtnnrvm.sHtML

if x > 0 then print("正") end
来源：http://3g.hesvh.cn/Article/details/giyrhpobb.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gvbiuhrxk.sHtML

string.find(s, "%d+")
来源：http://blog.hesvh.cn/Article/details/gfhcxfurl.sHtML

[T40] Lua：元表
来源：http://baike.zdbjq.cn/Article/details/guezjasow.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.zdbjq.cn/Article/details/gbayapblk.sHtML

[T41] Perl：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gmnjlqrbz.sHtML

print "Hello\n";
来源：http://baike.fehbvm.com/Article/details/gkpxuuucp.sHtML

[T42] Perl：变量类型
来源：http://3g.hesvh.cn/Article/details/glisjrxil.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.hesvh.cn/Article/details/gbseekslt.sHtML

[T43] Perl：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gwclewjff.sHtML

"值: $a"
来源：http://www.share.fehbvm.com/Article/details/gkkqefsdw.sHtML

[T44] Perl：条件
来源：http://blog.hesvh.cn/Article/details/gtjpovbou.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.fehbvm.com/Article/details/gdjshamac.sHtML

[T45] Perl：数组遍历
来源：http://wap.hesvh.cn/Article/details/gyrtfpphr.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.fehbvm.com/Article/details/gawipevnb.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.zdbjq.cn/Article/details/giqnxqbar.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.zdbjq.cn/Article/details/glltcrstq.sHtML

[T47] Perl：正则捕获
来源：http://m.share.zdbjq.cn/Article/details/griiamjvg.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.zdbjq.cn/Article/details/gorlnswqc.sHtML

[T48] Perl：正则替换
来源：http://wap.zdbjq.cn/Article/details/gnbalpmqp.sHtML

$s =~ s/old/new/g;
来源：http://3g.hesvh.cn/Article/details/gpqkrtbvt.sHtML

[T49] Perl：函数
来源：http://blog.zdbjq.cn/Article/details/gatfazacd.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gxplfksws.sHtML

[T50] Perl：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gqbmsusdz.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.zdbjq.cn/Article/details/girlxnbzr.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.fehbvm.com/Article/details/gcwwruiac.sHtML

[T51] Scala：Hello World
来源：http://www.share.hesvh.cn/Article/details/gdzwmasnc.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/gqrnlaifa.sHtML

[T52] Scala：变量
来源：http://3g.fehbvm.com/Article/details/gamahumin.sHtML

val a = 1;  var b = 2
来源：http://m.share.fehbvm.com/Article/details/gxbrrhggt.sHtML

[T53] Scala：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gcrbjcdpd.sHtML

s"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/gzfucliex.sHtML

[T54] Scala：集合映射
来源：http://wap.fehbvm.com/Article/details/gyurdnwqf.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.zdbjq.cn/Article/details/ggbxqlrhs.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/gddkighmr.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.zdbjq.cn/Article/details/gpkgvspoz.sHtML

[T56] Scala：样例类
来源：http://www.m.share.fehbvm.com/Article/details/gvaakcbfb.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.fehbvm.com/Article/details/golulrdto.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fehbvm.com/Article/details/gwmbnddje.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.hesvh.cn/Article/details/gtpqvkvmo.sHtML

[T58] Scala：函数定义
来源：http://wap.fehbvm.com/Article/details/gfrojdofc.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.hesvh.cn/Article/details/gatpgsekj.sHtML

[T59] Scala：循环
来源：http://www.m.share.hesvh.cn/Article/details/gllteyqmn.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.hesvh.cn/Article/details/gxuphwpbx.sHtML

[T60] Scala：折叠
来源：http://baike.hesvh.cn/Article/details/gdddzydbx.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.hesvh.cn/Article/details/gwgljlbfb.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gzmcejoxz.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.zdbjq.cn/Article/details/ggdxfgsjg.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gysfkuhvh.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.hesvh.cn/Article/details/guqtgvfdy.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.fehbvm.com/Article/details/gkgbkomto.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.fehbvm.com/Article/details/goneyipco.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.hesvh.cn/Article/details/gowhtmzrk.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.hesvh.cn/Article/details/gmvjpowuu.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.zdbjq.cn/Article/details/ghidqtlrc.sHtML

[U04] Py：变量调试打印
来源：http://www.share.hesvh.cn/Article/details/gqvntrgmp.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.hesvh.cn/Article/details/gbvkzjnxv.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.zdbjq.cn/Article/details/gqgqkibkn.sHtML

list(dict.fromkeys(arr))
来源：http://blog.hesvh.cn/Article/details/gtqkwovpa.sHtML

[U06] Py：合并两个字典
来源：http://3g.hesvh.cn/Article/details/gwubbbdco.sHtML

{**a, **b}
来源：http://www.blog.fehbvm.com/Article/details/gykupxdjc.sHtML

[U07] Py：反转字典键值
来源：http://wap.hesvh.cn/Article/details/gbeiybfqx.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.hesvh.cn/Article/details/ghcpvfqih.sHtML

[U08] Py：展平二维列表
来源：http://m.share.hesvh.cn/Article/details/gufejtdvs.sHtML

[y for x in nested for y in x]
来源：http://read.share.hesvh.cn/Article/details/gkbwlnsqe.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.fehbvm.com/Article/details/gltvimbos.sHtML

max(d, key=d.get)
来源：http://read.share.fehbvm.com/Article/details/gdfuwisyv.sHtML

[U10] Py：按值排序字典
来源：http://3g.fehbvm.com/Article/details/gtixiinur.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.zdbjq.cn/Article/details/gruttzmow.sHtML

[U11] Py：生成器表达式
来源：http://m.share.zdbjq.cn/Article/details/gfvwwstcg.sHtML

(x * 2 for x in arr)
来源：http://www.blog.zdbjq.cn/Article/details/ghwponxre.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.hesvh.cn/Article/details/gmyqeqbhe.sHtML

Counter(arr).most_common(3)
来源：http://m.share.fehbvm.com/Article/details/gfitwziod.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.hesvh.cn/Article/details/ghyrljwbs.sHtML

deque(maxlen=10)
来源：http://www.blog.fehbvm.com/Article/details/gptyoossi.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.hesvh.cn/Article/details/gcvwerntr.sHtML

defaultdict(list)
来源：http://m.share.hesvh.cn/Article/details/gzzdgosjb.sHtML

[U15] Py：高精度计时
来源：http://mobile.zdbjq.cn/Article/details/gjzclgskv.sHtML

t = time.perf_counter()
来源：http://wap.hesvh.cn/Article/details/glpnfxpfq.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.zdbjq.cn/Article/details/ggvqxmvwu.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.fehbvm.com/Article/details/ggllycfcx.sHtML

[U17] Py：初始化日志
来源：http://www.blog.zdbjq.cn/Article/details/gioaapnou.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.fehbvm.com/Article/details/gztrakbvg.sHtML

[U18] Py：预编译正则
来源：http://wap.hesvh.cn/Article/details/gdcunmhdh.sHtML

pat = re.compile(r"\d+")
来源：http://blog.zdbjq.cn/Article/details/gulusbgyn.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.zdbjq.cn/Article/details/ghzlpbaza.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.hesvh.cn/Article/details/goylkropu.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.hesvh.cn/Article/details/gubhlkhhj.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.zdbjq.cn/Article/details/gvvciuaxu.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.fehbvm.com/Article/details/gawwattzl.sHtML

@contextlib.contextmanager
来源：http://3g.zdbjq.cn/Article/details/gmtmshcbh.sHtML

[U22] Py：矩阵转置
来源：http://baike.fehbvm.com/Article/details/ggbkmthnl.sHtML

list(zip(*m))
来源：http://3g.zdbjq.cn/Article/details/gbqehrhxf.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.fehbvm.com/Article/details/gmxetdxxs.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.zdbjq.cn/Article/details/gaqmyiudk.sHtML

[U24] Py：路径操作
来源：http://mobile.hesvh.cn/Article/details/ghsmegdhd.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.hesvh.cn/Article/details/gyrvrcslp.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.zdbjq.cn/Article/details/ggyrdgnuz.sHtML

csv.DictReader(f)
来源：http://m.share.zdbjq.cn/Article/details/ghzypkkzp.sHtML

[U26] Py：并发下载
来源：http://blog.fehbvm.com/Article/details/ghnovvvhp.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.zdbjq.cn/Article/details/gugyxgasq.sHtML

[U27] Py：异步 HTTP
来源：http://wap.hesvh.cn/Article/details/gvtcqxzbz.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.hesvh.cn/Article/details/ghvnxxzgi.sHtML

[U28] Py：类型别名
来源：http://mobile.fehbvm.com/Article/details/gkgcsmvma.sHtML

UserId = int
来源：http://m.share.hesvh.cn/Article/details/gluyrhdnk.sHtML

[U29] Py：属性校验
来源：http://wap.zdbjq.cn/Article/details/gkqvcrdcb.sHtML

@property 与 @x.setter 配合
来源：http://mobile.fehbvm.com/Article/details/glclukdig.sHtML

[U30] Py：数据类
来源：http://www.m.share.zdbjq.cn/Article/details/guvcdiwtb.sHtML

@dataclass(slots=True)
来源：http://m.share.fehbvm.com/Article/details/gmnccwjgp.sHtML

[U31] Py：单测
来源：http://wap.fehbvm.com/Article/details/ggphfkzvu.sHtML

python -m pytest -q
来源：http://baike.hesvh.cn/Article/details/ggsiuliiv.sHtML

[U32] Py：代码格式化
来源：http://www.share.zdbjq.cn/Article/details/gqvhqdblj.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.fehbvm.com/Article/details/gpxtdtrwx.sHtML

[U33] Py：打包发布
来源：http://blog.fehbvm.com/Article/details/gytfzcfrv.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.hesvh.cn/Article/details/gmbbbfbsy.sHtML

[U34] Py：判断编码
来源：http://www.share.fehbvm.com/Article/details/gsrpmxhpa.sHtML

chardet.detect(raw)
来源：http://baike.fehbvm.com/Article/details/gmqxyxemk.sHtML

[U35] Py：发送邮件
来源：http://baike.zdbjq.cn/Article/details/gpzrsggou.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.zdbjq.cn/Article/details/gvazwonae.sHtML

[U36] Py：定时任务
来源：http://3g.zdbjq.cn/Article/details/glwpedkzv.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.fehbvm.com/Article/details/gpgopnrap.sHtML

[U37] Py：读写 Excel
来源：http://m.share.fehbvm.com/Article/details/ghqoeijyw.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.fehbvm.com/Article/details/gbwihngco.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.fehbvm.com/Article/details/gezybaffb.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.hesvh.cn/Article/details/gmepkmfdw.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.zdbjq.cn/Article/details/gwkvwsdyo.sHtML

sys.stdout.isatty()
来源：http://read.share.fehbvm.com/Article/details/gbldfehuc.sHtML

[U40] Py：打印到标准错误
来源：http://baike.fehbvm.com/Article/details/gfpjaozrl.sHtML

print("err", file=sys.stderr)
来源：http://mobile.hesvh.cn/Article/details/gkeqzxzna.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.zdbjq.cn/Article/details/gqkcwwoff.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.hesvh.cn/Article/details/gsribxhgp.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.zdbjq.cn/Article/details/gammkcyqy.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.zdbjq.cn/Article/details/gogflbvuy.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.hesvh.cn/Article/details/gepfurvzu.sHtML

namespace App\Http;
来源：http://wap.zdbjq.cn/Article/details/gnskowoeh.sHtML

[U44] PHP：开启严格类型
来源：http://blog.zdbjq.cn/Article/details/ghodfosrg.sHtML

declare(strict_types=1);
来源：http://www.m.share.hesvh.cn/Article/details/gguesushr.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.fehbvm.com/Article/details/grpqvbynl.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gllcmiqgq.sHtML

[U46] PHP：可空类型
来源：http://www.blog.zdbjq.cn/Article/details/gqohudyxm.sHtML

?string $name = null
来源：http://wap.fehbvm.com/Article/details/gyolfbcvz.sHtML

[U47] PHP：联合类型
来源：http://www.blog.hesvh.cn/Article/details/gmnvuptnx.sHtML

int|string $id
来源：http://m.share.zdbjq.cn/Article/details/gpczqffcw.sHtML

[U48] PHP：纯枚举
来源：http://m.share.fehbvm.com/Article/details/gdnbzctsw.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.hesvh.cn/Article/details/gpwbreknb.sHtML

[U49] PHP：只读属性
来源：http://mobile.fehbvm.com/Article/details/gnznpmgyh.sHtML

public readonly string $name
来源：http://www.share.zdbjq.cn/Article/details/gkydbkagi.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.fehbvm.com/Article/details/gesbloyrb.sHtML

public function __construct(private int $id) {}
来源：http://blog.hesvh.cn/Article/details/glacqincb.sHtML

[U51] PHP：数组解构
来源：http://www.blog.zdbjq.cn/Article/details/gsqtphllm.sHtML

[$a, $b] = $arr;
来源：http://mobile.zdbjq.cn/Article/details/gakouhoxe.sHtML

[U52] PHP：箭头函数
来源：http://3g.zdbjq.cn/Article/details/gkapfjzfc.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.hesvh.cn/Article/details/gdgzaclou.sHtML

[U53] PHP：空合并运算符
来源：http://baike.hesvh.cn/Article/details/gpvoywust.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.hesvh.cn/Article/details/geklkbpvf.sHtML

[U54] PHP：空安全调用
来源：http://m.share.zdbjq.cn/Article/details/gibhtnwxf.sHtML

$obj?->method()
来源：http://www.m.share.hesvh.cn/Article/details/gjrxdwfxj.sHtML

[U55] PHP：match 表达式
来源：http://www.share.zdbjq.cn/Article/details/gavibjtdn.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.fehbvm.com/Article/details/grwpjawge.sHtML

[U56] PHP：命名参数
来源：http://baike.fehbvm.com/Article/details/gobiunlig.sHtML

f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/gzdnglegj.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gdwglkpte.sHtML

"值: {$a}"
来源：http://m.share.hesvh.cn/Article/details/gwquqbdoy.sHtML

[U58] PHP：数组三件套
来源：http://baike.zdbjq.cn/Article/details/ggjqrdxwt.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.hesvh.cn/Article/details/ggjozyrlq.sHtML

[U59] PHP：自定义排序
来源：http://baike.fehbvm.com/Article/details/gfnasvpun.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.hesvh.cn/Article/details/gvhkbvhli.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.fehbvm.com/Article/details/gnvorwtuh.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.hesvh.cn/Article/details/gauqnzszy.sHtML

[U61] PHP：正则
来源：http://blog.fehbvm.com/Article/details/geuthfidv.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.zdbjq.cn/Article/details/gzwdoksrf.sHtML

[U62] PHP：日期对象
来源：http://blog.hesvh.cn/Article/details/ghkhgvxbl.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.fehbvm.com/Article/details/gmywezsho.sHtML

[U63] PHP：文件读写
来源：http://www.share.fehbvm.com/Article/details/gggcmyuns.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.hesvh.cn/Article/details/gaciuijld.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.fehbvm.com/Article/details/gdzmhdwxz.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.fehbvm.com/Article/details/gvupjxvfg.sHtML

[U65] PHP：会话
来源：http://m.share.hesvh.cn/Article/details/gkvofvirg.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gnusbovzv.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.fehbvm.com/Article/details/gigvylumx.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.hesvh.cn/Article/details/gqzjcpihr.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.zdbjq.cn/Article/details/gwtkdbgxp.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.fehbvm.com/Article/details/godolaihj.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.zdbjq.cn/Article/details/ghzolwqzd.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.hesvh.cn/Article/details/ghvkofcza.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.hesvh.cn/Article/details/gqnezbhzc.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.zdbjq.cn/Article/details/gtceveaxn.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.fehbvm.com/Article/details/gebjeewri.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.hesvh.cn/Article/details/gwdecnpjx.sHtML

[U71] PHP：抛出异常
来源：http://read.share.zdbjq.cn/Article/details/gcmjlywfl.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.hesvh.cn/Article/details/gksrlyshx.sHtML

[U72] PHP：写错误日志
来源：http://read.share.hesvh.cn/Article/details/gogjkkqej.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.fehbvm.com/Article/details/gfniltumh.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.zdbjq.cn/Article/details/grmllzldf.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.hesvh.cn/Article/details/gbyiasrje.sHtML

[U74] PHP：读取环境变量
来源：http://baike.hesvh.cn/Article/details/grqwviumq.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.hesvh.cn/Article/details/gjahmbiev.sHtML

[U75] PHP：依赖注入
来源：http://read.share.zdbjq.cn/Article/details/godwhpldg.sHtML

composer require psr/container
来源：http://3g.hesvh.cn/Article/details/ggxnfvoih.sHtML

[U76] PHP：简单路由
来源：http://www.share.hesvh.cn/Article/details/gdbobcxny.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.hesvh.cn/Article/details/ggszrabdh.sHtML

[U77] PHP：模板渲染
来源：http://m.share.hesvh.cn/Article/details/gjklrktjb.sHtML

composer require twig/twig
来源：http://3g.hesvh.cn/Article/details/glykvrxwm.sHtML

[U78] PHP：单元测试
来源：http://read.share.hesvh.cn/Article/details/greukmyry.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.fehbvm.com/Article/details/gyaggqtxf.sHtML

[U79] PHP：静态分析
来源：http://3g.zdbjq.cn/Article/details/ghbfnzbkw.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.fehbvm.com/Article/details/gczpiwrwe.sHtML

[U80] PHP：代码规范修复
来源：http://3g.hesvh.cn/Article/details/gjcwifhvy.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.zdbjq.cn/Article/details/gconvllxr.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.fehbvm.com/Article/details/gnkyvjick.sHtML

npm init -y;  npm i express
来源：http://wap.zdbjq.cn/Article/details/gtmzfevss.sHtML

[U82] JS：package.json 脚本
来源：http://3g.fehbvm.com/Article/details/gwfzoxodi.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.fehbvm.com/Article/details/gzbgqgihh.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.zdbjq.cn/Article/details/gzbzrnior.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.fehbvm.com/Article/details/gipddtxml.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.zdbjq.cn/Article/details/gcqpxqidx.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.fehbvm.com/Article/details/ggunaabvv.sHtML

[U85] JS：可选链
来源：http://www.m.share.hesvh.cn/Article/details/gmxomlubi.sHtML

a?.b?.c
来源：http://baike.zdbjq.cn/Article/details/ghtzjydya.sHtML

[U86] JS：空值合并
来源：http://baike.fehbvm.com/Article/details/gdpevrbvq.sHtML

a ?? b
来源：http://3g.zdbjq.cn/Article/details/gstmrgcfy.sHtML

[U87] JS：解构默认值
来源：http://www.share.zdbjq.cn/Article/details/gvpcrtavx.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.zdbjq.cn/Article/details/gitquijgx.sHtML

[U88] JS：对象展开合并
来源：http://m.share.zdbjq.cn/Article/details/glyrqhojb.sHtML

{ ...a, ...b }
来源：http://www.blog.fehbvm.com/Article/details/gdkcbiwyp.sHtML

[U89] JS：数组去重
来源：http://baike.zdbjq.cn/Article/details/gmmdjxqzx.sHtML

[...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gggnwkxmg.sHtML

[U90] JS：数字数组排序
来源：http://baike.hesvh.cn/Article/details/gncbuydww.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/gpcokcycs.sHtML


<!-- 参考信息 -->