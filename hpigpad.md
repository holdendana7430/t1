代发 wailian999

namespace ns { int f() { return 1; } }
来源：http://wap.fehbvm.com/Article/details/gqegfqzdw.sHtML

[S59] C++：静态断言
来源：http://3g.fehbvm.com/Article/details/gjzybzujg.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fehbvm.com/Article/details/gdprloxpv.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fehbvm.com/Article/details/gfttsiwdk.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.zdbjq.cn/Article/details/gucmgvxzf.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gmwhhgvoo.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.hesvh.cn/Article/details/guzgevpdb.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gxvcwrevf.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gwooironh.sHtML

println("Hello")
来源：http://www.blog.fehbvm.com/Article/details/geqyopnxq.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fehbvm.com/Article/details/gmidvucdv.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.zdbjq.cn/Article/details/gqefehalu.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.zdbjq.cn/Article/details/gzyocomlb.sHtML

"值: $b"
来源：http://www.blog.fehbvm.com/Article/details/gtlxoxbct.sHtML

[T04] Kotlin：空安全
来源：http://read.share.zdbjq.cn/Article/details/gssfgghdn.sHtML

val n: String? = null;  n?.length
来源：http://wap.fehbvm.com/Article/details/giisjprct.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.zdbjq.cn/Article/details/gelcxjkzp.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.zdbjq.cn/Article/details/gepoynmtt.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.zdbjq.cn/Article/details/gupkpucav.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/ghtebrsna.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.hesvh.cn/Article/details/gbftogxaz.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.hesvh.cn/Article/details/ghedgikzh.sHtML

[T08] Kotlin：数据类
来源：http://www.share.zdbjq.cn/Article/details/gfeumgpxp.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.hesvh.cn/Article/details/gawtywert.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.hesvh.cn/Article/details/gdhxnaptf.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.hesvh.cn/Article/details/gcqymnudk.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fehbvm.com/Article/details/gnvapffvf.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fehbvm.com/Article/details/ghfbybxni.sHtML

[T11] Kotlin：协程
来源：http://wap.zdbjq.cn/Article/details/gvvvsupwj.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.zdbjq.cn/Article/details/glyosambs.sHtML

[T12] Kotlin：解构声明
来源：http://baike.hesvh.cn/Article/details/gxoiipehq.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fehbvm.com/Article/details/gscmvzwdd.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fehbvm.com/Article/details/gkwnqvrmf.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.zdbjq.cn/Article/details/gqwwlwrah.sHtML

[T14] Kotlin：循环
来源：http://m.share.zdbjq.cn/Article/details/gdusciuzy.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.hesvh.cn/Article/details/gcpnurbgr.sHtML

[T15] Kotlin：接口
来源：http://mobile.hesvh.cn/Article/details/gzbsqvlmv.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fehbvm.com/Article/details/gzwbklddj.sHtML

[T16] Swift：Hello World
来源：http://baike.hesvh.cn/Article/details/grkomiawq.sHtML

print("Hello")
来源：http://read.share.hesvh.cn/Article/details/ghfgdbveq.sHtML

[T17] Swift：变量与常量
来源：http://mobile.zdbjq.cn/Article/details/gcxcactgx.sHtML

var a = 1;  let b = 2
来源：http://mobile.fehbvm.com/Article/details/gtyyqzlyg.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gcxgfxyct.sHtML

"值: \(b)"
来源：http://www.share.hesvh.cn/Article/details/gjotprcny.sHtML

[T19] Swift：可选绑定
来源：http://3g.zdbjq.cn/Article/details/grblvgzvh.sHtML

if let n = opt { print(n) }
来源：http://m.share.fehbvm.com/Article/details/ggycdmpbp.sHtML

[T20] Swift：数组操作
来源：http://www.blog.hesvh.cn/Article/details/grxbkueae.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.hesvh.cn/Article/details/gmoansahw.sHtML

[T21] Swift：遍历
来源：http://www.blog.hesvh.cn/Article/details/gvipggpat.sHtML

for x in a { print(x) }
来源：http://blog.fehbvm.com/Article/details/gnmsmzkzy.sHtML

[T22] Swift：字典
来源：http://read.share.hesvh.cn/Article/details/glkcnmede.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fehbvm.com/Article/details/gjxfqrrcn.sHtML

[T23] Swift：函数
来源：http://www.share.fehbvm.com/Article/details/goaybvqdf.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.hesvh.cn/Article/details/gppdpwtrk.sHtML

[T24] Swift：闭包
来源：http://www.m.share.hesvh.cn/Article/details/gtiuotlpa.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fehbvm.com/Article/details/gulmhbwcr.sHtML

[T25] Swift：结构体
来源：http://baike.fehbvm.com/Article/details/gymvkwpko.sHtML

struct P { var x: Int }
来源：http://blog.hesvh.cn/Article/details/gkhtnuwfe.sHtML

[T26] Swift：类与重写
来源：http://read.share.fehbvm.com/Article/details/gbgyvcsbp.sHtML

class A: Base { override func f() {} }
来源：http://3g.hesvh.cn/Article/details/gwbqfmmat.sHtML

[T27] Swift：错误处理
来源：http://www.blog.zdbjq.cn/Article/details/gmwvepkrk.sHtML

do { try f() } catch { print(error) }
来源：http://3g.hesvh.cn/Article/details/gaxuwwvjb.sHtML

[T28] Swift：枚举
来源：http://read.share.hesvh.cn/Article/details/gvlziuave.sHtML

enum Color { case red, green }
来源：http://wap.hesvh.cn/Article/details/gynnapkoy.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.hesvh.cn/Article/details/guxdvwcqf.sHtML

guard let x = opt else { return }
来源：http://m.share.hesvh.cn/Article/details/gcgynbvue.sHtML

[T30] Swift：协议
来源：http://www.blog.zdbjq.cn/Article/details/gayxzyqpr.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fehbvm.com/Article/details/gizifchrw.sHtML

[T31] Lua：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gazzjhiye.sHtML

print("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gwizcbldc.sHtML

[T32] Lua：局部变量
来源：http://3g.hesvh.cn/Article/details/gawksadck.sHtML

local a = 1
来源：http://www.m.share.zdbjq.cn/Article/details/gegahivzm.sHtML

[T33] Lua：表（数组）
来源：http://baike.fehbvm.com/Article/details/gwujfdtge.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.fehbvm.com/Article/details/grljfnkbl.sHtML

[T34] Lua：遍历表
来源：http://3g.hesvh.cn/Article/details/gynwoyruu.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.hesvh.cn/Article/details/gkytxwldi.sHtML

[T35] Lua：字典表
来源：http://www.m.share.zdbjq.cn/Article/details/ghtnudlxp.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.hesvh.cn/Article/details/gpezvcmfd.sHtML

[T36] Lua：函数
来源：http://baike.hesvh.cn/Article/details/gnhtemzhn.sHtML

function add(a, b) return a + b end
来源：http://baike.zdbjq.cn/Article/details/gmvmakgbd.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.hesvh.cn/Article/details/gxnhvjfkj.sHtML

"a" .. "b"
来源：http://blog.fehbvm.com/Article/details/ggcugwfiw.sHtML

[T38] Lua：条件
来源：http://mobile.fehbvm.com/Article/details/gzmgjamfb.sHtML

if x > 0 then print("正") end
来源：http://baike.fehbvm.com/Article/details/gnrsbcwki.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.fehbvm.com/Article/details/gdntjskji.sHtML

string.find(s, "%d+")
来源：http://www.blog.fehbvm.com/Article/details/gefwienpt.sHtML

[T40] Lua：元表
来源：http://baike.hesvh.cn/Article/details/gzzhlwevs.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.zdbjq.cn/Article/details/gdgbzvaiv.sHtML

[T41] Perl：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gnvipzfoi.sHtML

print "Hello\n";
来源：http://3g.fehbvm.com/Article/details/gbnmhehmo.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.zdbjq.cn/Article/details/gfpdwfzqt.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.hesvh.cn/Article/details/gbqgflnjw.sHtML

[T43] Perl：字符串插值
来源：http://wap.hesvh.cn/Article/details/gmrwrpeei.sHtML

"值: $a"
来源：http://www.m.share.zdbjq.cn/Article/details/gramlhckk.sHtML

[T44] Perl：条件
来源：http://3g.hesvh.cn/Article/details/gxovebpmb.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.hesvh.cn/Article/details/gqdeubuek.sHtML

[T45] Perl：数组遍历
来源：http://m.share.zdbjq.cn/Article/details/geheybyla.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.fehbvm.com/Article/details/gywlqniet.sHtML

[T46] Perl：哈希操作
来源：http://baike.zdbjq.cn/Article/details/gflckwael.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.fehbvm.com/Article/details/gvdkykopk.sHtML

[T47] Perl：正则捕获
来源：http://read.share.zdbjq.cn/Article/details/ggzsmtzca.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.fehbvm.com/Article/details/grswntpbf.sHtML

[T48] Perl：正则替换
来源：http://3g.zdbjq.cn/Article/details/gxjxwmutr.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.fehbvm.com/Article/details/gccfcvnhx.sHtML

[T49] Perl：函数
来源：http://baike.hesvh.cn/Article/details/gdajrmpco.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gzlpmfylq.sHtML

[T50] Perl：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gkhaxrkjm.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.fehbvm.com/Article/details/gcxamvokj.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.fehbvm.com/Article/details/gnmklpeeu.sHtML

[T51] Scala：Hello World
来源：http://m.share.fehbvm.com/Article/details/gedxlyibx.sHtML

println("Hello")
来源：http://blog.fehbvm.com/Article/details/gmrdookau.sHtML

[T52] Scala：变量
来源：http://www.m.share.hesvh.cn/Article/details/gwhfocpnb.sHtML

val a = 1;  var b = 2
来源：http://mobile.hesvh.cn/Article/details/genrxzury.sHtML

[T53] Scala：字符串插值
来源：http://baike.hesvh.cn/Article/details/gjhkxujrl.sHtML

s"值: $b"
来源：http://3g.hesvh.cn/Article/details/gbpkdkcgg.sHtML

[T54] Scala：集合映射
来源：http://www.blog.fehbvm.com/Article/details/gkmdlrizq.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.fehbvm.com/Article/details/gykiurylo.sHtML

[T55] Scala：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/gdsexpasm.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.hesvh.cn/Article/details/gkgzemfxs.sHtML

[T56] Scala：样例类
来源：http://m.share.fehbvm.com/Article/details/galpgnaok.sHtML

case class User(name: String, age: Int)
来源：http://baike.hesvh.cn/Article/details/gqmiphszk.sHtML

[T57] Scala：模式匹配
来源：http://read.share.fehbvm.com/Article/details/gvcmyyjuz.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.fehbvm.com/Article/details/gjliunbyw.sHtML

[T58] Scala：函数定义
来源：http://www.blog.zdbjq.cn/Article/details/gbnolbvnw.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.hesvh.cn/Article/details/glapmpkzn.sHtML

[T59] Scala：循环
来源：http://3g.hesvh.cn/Article/details/ghssnyvzt.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.zdbjq.cn/Article/details/gpmedrtva.sHtML

[T60] Scala：折叠
来源：http://baike.zdbjq.cn/Article/details/gfkneyole.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.fehbvm.com/Article/details/gaoiwhyut.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ghikzgzma.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.fehbvm.com/Article/details/gskccnmtw.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gdhoaisjs.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.hesvh.cn/Article/details/guxtcpkrd.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.hesvh.cn/Article/details/gdmdoybzv.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.fehbvm.com/Article/details/ghogkfghx.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.hesvh.cn/Article/details/gpkfnclaf.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.hesvh.cn/Article/details/gutocpqok.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.fehbvm.com/Article/details/gesdmmqpa.sHtML

[U04] Py：变量调试打印
来源：http://3g.fehbvm.com/Article/details/gwidqrslp.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.hesvh.cn/Article/details/gfozrrbub.sHtML

[U05] Py：列表去重且保序
来源：http://baike.hesvh.cn/Article/details/gvqzkrdrr.sHtML

list(dict.fromkeys(arr))
来源：http://3g.fehbvm.com/Article/details/ghwoijhaw.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.hesvh.cn/Article/details/gpxoacqqr.sHtML

{**a, **b}
来源：http://read.share.fehbvm.com/Article/details/gtwkkyfry.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.hesvh.cn/Article/details/gqnonzjlo.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.zdbjq.cn/Article/details/gfkhyniez.sHtML

[U08] Py：展平二维列表
来源：http://read.share.fehbvm.com/Article/details/glscqkhzj.sHtML

[y for x in nested for y in x]
来源：http://read.share.zdbjq.cn/Article/details/gzdsooykp.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.hesvh.cn/Article/details/ggwkbrvvc.sHtML

max(d, key=d.get)
来源：http://3g.fehbvm.com/Article/details/ggygblhfw.sHtML

[U10] Py：按值排序字典
来源：http://read.share.zdbjq.cn/Article/details/gkuhdcuud.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.fehbvm.com/Article/details/gtmhbmkng.sHtML

[U11] Py：生成器表达式
来源：http://wap.zdbjq.cn/Article/details/ggyaupmem.sHtML

(x * 2 for x in arr)
来源：http://m.share.fehbvm.com/Article/details/gjswgjkju.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.hesvh.cn/Article/details/gqemfwylm.sHtML

Counter(arr).most_common(3)
来源：http://blog.hesvh.cn/Article/details/gfzjxklgi.sHtML

[U13] Py：固定长度队列
来源：http://3g.fehbvm.com/Article/details/gxezbntul.sHtML

deque(maxlen=10)
来源：http://read.share.hesvh.cn/Article/details/gdcgbejrg.sHtML

[U14] Py：分组收集到列表
来源：http://3g.fehbvm.com/Article/details/gjiqmfhcw.sHtML

defaultdict(list)
来源：http://www.share.fehbvm.com/Article/details/gplxgkygt.sHtML

[U15] Py：高精度计时
来源：http://baike.fehbvm.com/Article/details/gymoqxtbi.sHtML

t = time.perf_counter()
来源：http://www.share.hesvh.cn/Article/details/gzckbbmsz.sHtML

[U16] Py：命令行参数解析
来源：http://baike.fehbvm.com/Article/details/gyckaomub.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.zdbjq.cn/Article/details/gmilovveo.sHtML

[U17] Py：初始化日志
来源：http://m.share.zdbjq.cn/Article/details/gsghuqzmx.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fehbvm.com/Article/details/gqknutdud.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.zdbjq.cn/Article/details/glafqramo.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.hesvh.cn/Article/details/gmhisappc.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.fehbvm.com/Article/details/gjmvdagbi.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.fehbvm.com/Article/details/gldhdekub.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.hesvh.cn/Article/details/gsjpdkgjl.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.fehbvm.com/Article/details/gmxhthruw.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.zdbjq.cn/Article/details/gsjyhocja.sHtML

@contextlib.contextmanager
来源：http://3g.zdbjq.cn/Article/details/gixgtzrwo.sHtML

[U22] Py：矩阵转置
来源：http://mobile.fehbvm.com/Article/details/gtzjpodiy.sHtML

list(zip(*m))
来源：http://blog.hesvh.cn/Article/details/gknhxtklh.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.hesvh.cn/Article/details/gtvkjwlww.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.fehbvm.com/Article/details/gemtfqcsh.sHtML

[U24] Py：路径操作
来源：http://m.share.fehbvm.com/Article/details/gmsuijfns.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.zdbjq.cn/Article/details/gohnuukzj.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.zdbjq.cn/Article/details/gbjnpreeb.sHtML

csv.DictReader(f)
来源：http://m.share.zdbjq.cn/Article/details/gdhheqlda.sHtML

[U26] Py：并发下载
来源：http://blog.hesvh.cn/Article/details/gqlvuozlh.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.hesvh.cn/Article/details/gjymagpoh.sHtML

[U27] Py：异步 HTTP
来源：http://wap.fehbvm.com/Article/details/gocrcyblg.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.zdbjq.cn/Article/details/gdaxsfrom.sHtML

[U28] Py：类型别名
来源：http://3g.hesvh.cn/Article/details/gvblxmxsd.sHtML

UserId = int
来源：http://baike.hesvh.cn/Article/details/gotcpghoc.sHtML

[U29] Py：属性校验
来源：http://blog.zdbjq.cn/Article/details/gsfddpoeh.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.zdbjq.cn/Article/details/giiedhqwx.sHtML

[U30] Py：数据类
来源：http://m.share.fehbvm.com/Article/details/gunhantac.sHtML

@dataclass(slots=True)
来源：http://read.share.fehbvm.com/Article/details/gvkiwytjr.sHtML

[U31] Py：单测
来源：http://baike.fehbvm.com/Article/details/gyldjommk.sHtML

python -m pytest -q
来源：http://baike.hesvh.cn/Article/details/gelxgsaqu.sHtML

[U32] Py：代码格式化
来源：http://blog.fehbvm.com/Article/details/gihgogbnp.sHtML

ruff format . && ruff check --fix .
来源：http://blog.hesvh.cn/Article/details/gpanbgaaw.sHtML

[U33] Py：打包发布
来源：http://m.share.hesvh.cn/Article/details/giysylgjp.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.fehbvm.com/Article/details/geuupntvp.sHtML

[U34] Py：判断编码
来源：http://baike.hesvh.cn/Article/details/gorrdpxyy.sHtML

chardet.detect(raw)
来源：http://www.m.share.hesvh.cn/Article/details/gkwstjnei.sHtML

[U35] Py：发送邮件
来源：http://read.share.hesvh.cn/Article/details/giatbfems.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.hesvh.cn/Article/details/gwyzzhirg.sHtML

[U36] Py：定时任务
来源：http://www.m.share.fehbvm.com/Article/details/gfycuspin.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.zdbjq.cn/Article/details/gqhwkkczi.sHtML

[U37] Py：读写 Excel
来源：http://m.share.fehbvm.com/Article/details/gvlsohrbj.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.hesvh.cn/Article/details/gnjcnthvt.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.zdbjq.cn/Article/details/guhfwpgkm.sHtML

Path(__file__).resolve().parent
来源：http://wap.zdbjq.cn/Article/details/gclpozqpy.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.hesvh.cn/Article/details/gydfhgrej.sHtML

sys.stdout.isatty()
来源：http://mobile.zdbjq.cn/Article/details/gmpsfqjdu.sHtML

[U40] Py：打印到标准错误
来源：http://blog.zdbjq.cn/Article/details/gbcfomtgw.sHtML

print("err", file=sys.stderr)
来源：http://baike.zdbjq.cn/Article/details/ggtjpadem.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.hesvh.cn/Article/details/gikbmpqrj.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.hesvh.cn/Article/details/ghqmuowtc.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.fehbvm.com/Article/details/gozpvrhcd.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.zdbjq.cn/Article/details/gpetbixjt.sHtML

[U43] PHP：声明命名空间
来源：http://baike.zdbjq.cn/Article/details/ghingopjn.sHtML

namespace App\Http;
来源：http://baike.zdbjq.cn/Article/details/grqtoxitc.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.hesvh.cn/Article/details/grlfaevxn.sHtML

declare(strict_types=1);
来源：http://blog.zdbjq.cn/Article/details/ggvpvycve.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.fehbvm.com/Article/details/gcqaltmiw.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gsogvuktn.sHtML

[U46] PHP：可空类型
来源：http://wap.zdbjq.cn/Article/details/gxgobmuoq.sHtML

?string $name = null
来源：http://www.m.share.zdbjq.cn/Article/details/guetxzapg.sHtML

[U47] PHP：联合类型
来源：http://baike.fehbvm.com/Article/details/gardqposv.sHtML

int|string $id
来源：http://baike.zdbjq.cn/Article/details/gkoncyiuo.sHtML

[U48] PHP：纯枚举
来源：http://blog.hesvh.cn/Article/details/gqkiopqbp.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.zdbjq.cn/Article/details/ghlejprxx.sHtML

[U49] PHP：只读属性
来源：http://www.share.hesvh.cn/Article/details/gklqtnzyu.sHtML

public readonly string $name
来源：http://wap.fehbvm.com/Article/details/gvlmjvgfv.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.hesvh.cn/Article/details/gyhlkeqmd.sHtML

public function __construct(private int $id) {}
来源：http://mobile.hesvh.cn/Article/details/gavtufari.sHtML

[U51] PHP：数组解构
来源：http://baike.zdbjq.cn/Article/details/gmzgqrffv.sHtML

[$a, $b] = $arr;
来源：http://baike.fehbvm.com/Article/details/gsjtmkwkq.sHtML

[U52] PHP：箭头函数
来源：http://m.share.zdbjq.cn/Article/details/gtbchhfug.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.hesvh.cn/Article/details/ghezrhlew.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.zdbjq.cn/Article/details/gtkkswczv.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.fehbvm.com/Article/details/glnyuqqfp.sHtML

[U54] PHP：空安全调用
来源：http://3g.hesvh.cn/Article/details/gcqnmmpst.sHtML

$obj?->method()
来源：http://baike.hesvh.cn/Article/details/gretscgxu.sHtML

[U55] PHP：match 表达式
来源：http://blog.zdbjq.cn/Article/details/gmdelgfik.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.fehbvm.com/Article/details/ggzjxvyvq.sHtML

[U56] PHP：命名参数
来源：http://baike.hesvh.cn/Article/details/gifuzwwli.sHtML

f(a: 1, b: 2)
来源：http://www.share.zdbjq.cn/Article/details/goccynxid.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gwekdgxre.sHtML

"值: {$a}"
来源：http://www.share.hesvh.cn/Article/details/gqobfvhgb.sHtML

[U58] PHP：数组三件套
来源：http://mobile.hesvh.cn/Article/details/gfdstpdal.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.fehbvm.com/Article/details/gknsbhsfl.sHtML

[U59] PHP：自定义排序
来源：http://blog.hesvh.cn/Article/details/gnhcyhymj.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fehbvm.com/Article/details/gtlmqghtr.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.fehbvm.com/Article/details/glzghqnsy.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.hesvh.cn/Article/details/gvmcffgoo.sHtML

[U61] PHP：正则
来源：http://mobile.hesvh.cn/Article/details/gzsnwdjfz.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fehbvm.com/Article/details/glfegvzzw.sHtML

[U62] PHP：日期对象
来源：http://read.share.zdbjq.cn/Article/details/grrmstyqc.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.hesvh.cn/Article/details/gribcxewf.sHtML

[U63] PHP：文件读写
来源：http://www.blog.hesvh.cn/Article/details/gukrvdmxn.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.hesvh.cn/Article/details/gbigjyfpr.sHtML

[U64] PHP：目录遍历
来源：http://read.share.hesvh.cn/Article/details/gfumbwmvq.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.zdbjq.cn/Article/details/ghnxmrwep.sHtML

[U65] PHP：会话
来源：http://3g.hesvh.cn/Article/details/gzmgxaken.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gocopfkot.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.hesvh.cn/Article/details/gvrcygxbi.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.zdbjq.cn/Article/details/gkjsolrwh.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.zdbjq.cn/Article/details/gpvlknosy.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.zdbjq.cn/Article/details/gkutqphcb.sHtML

[U68] PHP：PDO 连接
来源：http://baike.fehbvm.com/Article/details/gcnvcopsv.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.fehbvm.com/Article/details/gufprzcis.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.hesvh.cn/Article/details/gmanevzlz.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.zdbjq.cn/Article/details/ghoezgrmh.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.hesvh.cn/Article/details/gaicjfywp.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.fehbvm.com/Article/details/gixfmfqof.sHtML

[U71] PHP：抛出异常
来源：http://baike.zdbjq.cn/Article/details/grljdwfwm.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.fehbvm.com/Article/details/ggefmoner.sHtML

[U72] PHP：写错误日志
来源：http://baike.hesvh.cn/Article/details/gqwuzlmed.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.zdbjq.cn/Article/details/gektbuwww.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.fehbvm.com/Article/details/gupcqnyzk.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.fehbvm.com/Article/details/gwzlkekcg.sHtML

[U74] PHP：读取环境变量
来源：http://blog.hesvh.cn/Article/details/gmruisgyl.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.hesvh.cn/Article/details/ghgiuzfpv.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.fehbvm.com/Article/details/ghamtzwos.sHtML

composer require psr/container
来源：http://www.m.share.fehbvm.com/Article/details/goxxxixme.sHtML

[U76] PHP：简单路由
来源：http://www.blog.zdbjq.cn/Article/details/gtvlkaosu.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.fehbvm.com/Article/details/gknnnrjaj.sHtML

[U77] PHP：模板渲染
来源：http://mobile.zdbjq.cn/Article/details/gzxdwnrqc.sHtML

composer require twig/twig
来源：http://3g.fehbvm.com/Article/details/gdyhtdquv.sHtML

[U78] PHP：单元测试
来源：http://www.blog.hesvh.cn/Article/details/gvmujzieq.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.zdbjq.cn/Article/details/gsauiipbo.sHtML

[U79] PHP：静态分析
来源：http://3g.fehbvm.com/Article/details/geukwiknj.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.fehbvm.com/Article/details/gdsumjltw.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.fehbvm.com/Article/details/gkrslznju.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.fehbvm.com/Article/details/gedggmpis.sHtML

[U81] JS：初始化项目
来源：http://wap.fehbvm.com/Article/details/gmhcfobxl.sHtML

npm init -y;  npm i express
来源：http://www.blog.hesvh.cn/Article/details/gxijezqli.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.fehbvm.com/Article/details/giezpertk.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.fehbvm.com/Article/details/gmhselexr.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.zdbjq.cn/Article/details/gsdvmmwki.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.zdbjq.cn/Article/details/gqgncxyct.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.zdbjq.cn/Article/details/gedvgfwkz.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.fehbvm.com/Article/details/gkxirtkzj.sHtML


<!-- 参考信息 -->