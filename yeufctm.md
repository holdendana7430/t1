代发 wailian999

namespace ns { int f() { return 1; } }
来源：http://baike.fehbvm.com/Article/details/gcimuofte.sHtML

[S59] C++：静态断言
来源：http://m.share.fehbvm.com/Article/details/gnpwsbpgd.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.hesvh.cn/Article/details/gwmiwsroe.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.hesvh.cn/Article/details/gvhhxypuk.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fehbvm.com/Article/details/gbfakodjq.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gcvcwexkt.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.zdbjq.cn/Article/details/gaoxkmqku.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gxvcjrofl.sHtML

[T01] Kotlin：Hello World
来源：http://baike.zdbjq.cn/Article/details/gbkunfcnn.sHtML

println("Hello")
来源：http://baike.fehbvm.com/Article/details/geaxwgmhf.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fehbvm.com/Article/details/gbxwjayuh.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.hesvh.cn/Article/details/grmjspdjk.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.zdbjq.cn/Article/details/ggyqakttj.sHtML

"值: $b"
来源：http://3g.zdbjq.cn/Article/details/gdvaszatp.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fehbvm.com/Article/details/gagxgater.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.zdbjq.cn/Article/details/gxxlljlhe.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fehbvm.com/Article/details/gogzaygrc.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fehbvm.com/Article/details/gtqovxobr.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.fehbvm.com/Article/details/gubujnbag.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fehbvm.com/Article/details/gldtelcsb.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.zdbjq.cn/Article/details/glcwnisxj.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fehbvm.com/Article/details/gpnsojgwv.sHtML

[T08] Kotlin：数据类
来源：http://mobile.hesvh.cn/Article/details/gqyxdfsug.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.zdbjq.cn/Article/details/gvqcypdpb.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fehbvm.com/Article/details/gyeykwzbu.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.zdbjq.cn/Article/details/gtiftxitw.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fehbvm.com/Article/details/gvrvxwbmh.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.zdbjq.cn/Article/details/gdjtkhmxs.sHtML

[T11] Kotlin：协程
来源：http://m.share.hesvh.cn/Article/details/gvcqqwhjm.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.fehbvm.com/Article/details/glkszvyxg.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.zdbjq.cn/Article/details/ganvxbjxo.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gslmaifzs.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fehbvm.com/Article/details/guotallcc.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.zdbjq.cn/Article/details/grcvztbfi.sHtML

[T14] Kotlin：循环
来源：http://read.share.hesvh.cn/Article/details/ganprbmef.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fehbvm.com/Article/details/gmfpgeqyq.sHtML

[T15] Kotlin：接口
来源：http://wap.zdbjq.cn/Article/details/gglxttpjg.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.zdbjq.cn/Article/details/glqbkgjre.sHtML

[T16] Swift：Hello World
来源：http://read.share.zdbjq.cn/Article/details/grrsfgkvi.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/guhdfhqmz.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fehbvm.com/Article/details/ggfnhjmwv.sHtML

var a = 1;  let b = 2
来源：http://blog.zdbjq.cn/Article/details/gdsdjvcdq.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gwmdisgum.sHtML

"值: \(b)"
来源：http://3g.hesvh.cn/Article/details/gadqwlsai.sHtML

[T19] Swift：可选绑定
来源：http://m.share.zdbjq.cn/Article/details/gbajufsln.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fehbvm.com/Article/details/ghirzqskq.sHtML

[T20] Swift：数组操作
来源：http://www.share.fehbvm.com/Article/details/girrjnbcn.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.zdbjq.cn/Article/details/gehofessd.sHtML

[T21] Swift：遍历
来源：http://www.m.share.fehbvm.com/Article/details/geujrzynl.sHtML

for x in a { print(x) }
来源：http://baike.zdbjq.cn/Article/details/giqfplplv.sHtML

[T22] Swift：字典
来源：http://blog.fehbvm.com/Article/details/gtbsylntr.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fehbvm.com/Article/details/gjwhuhijc.sHtML

[T23] Swift：函数
来源：http://baike.fehbvm.com/Article/details/gjmkmevif.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.zdbjq.cn/Article/details/gdsrgjtpi.sHtML

[T24] Swift：闭包
来源：http://www.blog.zdbjq.cn/Article/details/gceazapak.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gljwluxye.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fehbvm.com/Article/details/glgghtact.sHtML

struct P { var x: Int }
来源：http://www.blog.zdbjq.cn/Article/details/gqzyqumdv.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.fehbvm.com/Article/details/glosasbwe.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fehbvm.com/Article/details/gemxjzpfi.sHtML

[T27] Swift：错误处理
来源：http://wap.zdbjq.cn/Article/details/gxtoblyws.sHtML

do { try f() } catch { print(error) }
来源：http://blog.fehbvm.com/Article/details/gdashdsoy.sHtML

[T28] Swift：枚举
来源：http://m.share.zdbjq.cn/Article/details/gdlaftjnv.sHtML

enum Color { case red, green }
来源：http://www.m.share.hesvh.cn/Article/details/gapoomukm.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.fehbvm.com/Article/details/gtmcljupk.sHtML

guard let x = opt else { return }
来源：http://www.share.hesvh.cn/Article/details/gzkwbtmzy.sHtML

[T30] Swift：协议
来源：http://www.blog.zdbjq.cn/Article/details/ganjynkic.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.hesvh.cn/Article/details/gbsiolspe.sHtML

[T31] Lua：Hello World
来源：http://blog.hesvh.cn/Article/details/glodbyutx.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/gedzgioym.sHtML

[T32] Lua：局部变量
来源：http://read.share.zdbjq.cn/Article/details/gxxwcbwkc.sHtML

local a = 1
来源：http://m.share.zdbjq.cn/Article/details/gleuurrzz.sHtML

[T33] Lua：表（数组）
来源：http://wap.zdbjq.cn/Article/details/geileloja.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.hesvh.cn/Article/details/gommwcfdd.sHtML

[T34] Lua：遍历表
来源：http://baike.hesvh.cn/Article/details/gpnfyjhtw.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.fehbvm.com/Article/details/gcssukvlm.sHtML

[T35] Lua：字典表
来源：http://baike.hesvh.cn/Article/details/gsbwqdtps.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.fehbvm.com/Article/details/gjytlnwyt.sHtML

[T36] Lua：函数
来源：http://mobile.fehbvm.com/Article/details/geflqtyvb.sHtML

function add(a, b) return a + b end
来源：http://baike.fehbvm.com/Article/details/gpssrudtw.sHtML

[T37] Lua：字符串拼接
来源：http://baike.hesvh.cn/Article/details/gipicxppy.sHtML

"a" .. "b"
来源：http://blog.fehbvm.com/Article/details/gbkioobnz.sHtML

[T38] Lua：条件
来源：http://blog.fehbvm.com/Article/details/gohgcadxq.sHtML

if x > 0 then print("正") end
来源：http://baike.zdbjq.cn/Article/details/grpwposar.sHtML

[T39] Lua：模式匹配
来源：http://read.share.fehbvm.com/Article/details/gnqlmghum.sHtML

string.find(s, "%d+")
来源：http://wap.zdbjq.cn/Article/details/gjymmfduc.sHtML

[T40] Lua：元表
来源：http://baike.fehbvm.com/Article/details/gqoceuhdk.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.zdbjq.cn/Article/details/gyxmdxgwc.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gxuwxaenj.sHtML

print "Hello\n";
来源：http://mobile.zdbjq.cn/Article/details/gkcwpjbvs.sHtML

[T42] Perl：变量类型
来源：http://read.share.hesvh.cn/Article/details/gjlwuzpqq.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.hesvh.cn/Article/details/gxritnmsm.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gmkyolvdb.sHtML

"值: $a"
来源：http://mobile.hesvh.cn/Article/details/gpalnggym.sHtML

[T44] Perl：条件
来源：http://blog.zdbjq.cn/Article/details/gseuvhdqo.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.hesvh.cn/Article/details/gvrerzdsp.sHtML

[T45] Perl：数组遍历
来源：http://3g.hesvh.cn/Article/details/gqnckpwrx.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.zdbjq.cn/Article/details/garwpvrls.sHtML

[T46] Perl：哈希操作
来源：http://wap.hesvh.cn/Article/details/ggyzywstg.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.zdbjq.cn/Article/details/gkhgohnaq.sHtML

[T47] Perl：正则捕获
来源：http://baike.hesvh.cn/Article/details/gcencseeo.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.fehbvm.com/Article/details/gypdnlxuy.sHtML

[T48] Perl：正则替换
来源：http://baike.hesvh.cn/Article/details/glrkkepgd.sHtML

$s =~ s/old/new/g;
来源：http://www.share.zdbjq.cn/Article/details/gtmrtlcsl.sHtML

[T49] Perl：函数
来源：http://wap.hesvh.cn/Article/details/gwievxtjl.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gytevgwdc.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gknzoepci.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.fehbvm.com/Article/details/gxrqethrg.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.zdbjq.cn/Article/details/gmrqnbadt.sHtML

[T51] Scala：Hello World
来源：http://blog.zdbjq.cn/Article/details/gfwuqbakf.sHtML

println("Hello")
来源：http://wap.hesvh.cn/Article/details/grtwfahji.sHtML

[T52] Scala：变量
来源：http://www.blog.fehbvm.com/Article/details/gykrvltsj.sHtML

val a = 1;  var b = 2
来源：http://read.share.fehbvm.com/Article/details/gwwcfqmtw.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gujavpgis.sHtML

s"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/gkaehiwtt.sHtML

[T54] Scala：集合映射
来源：http://www.share.zdbjq.cn/Article/details/gcsdjlliz.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.zdbjq.cn/Article/details/gusktrapw.sHtML

[T55] Scala：集合过滤
来源：http://wap.zdbjq.cn/Article/details/gghwckrds.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.hesvh.cn/Article/details/gyqgnjsve.sHtML

[T56] Scala：样例类
来源：http://m.share.fehbvm.com/Article/details/gyclpncvi.sHtML

case class User(name: String, age: Int)
来源：http://m.share.hesvh.cn/Article/details/gwerdokaq.sHtML

[T57] Scala：模式匹配
来源：http://read.share.hesvh.cn/Article/details/gmxaucetd.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.hesvh.cn/Article/details/goscyohmt.sHtML

[T58] Scala：函数定义
来源：http://mobile.hesvh.cn/Article/details/gdhpnqjgi.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.zdbjq.cn/Article/details/gasgwfjel.sHtML

[T59] Scala：循环
来源：http://read.share.hesvh.cn/Article/details/getmwwhds.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.hesvh.cn/Article/details/ggisnegwv.sHtML

[T60] Scala：折叠
来源：http://www.m.share.hesvh.cn/Article/details/geawuvitt.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.fehbvm.com/Article/details/gsqzqygvf.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gszafqzku.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fehbvm.com/Article/details/gkfbbbetp.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gcnbbyftm.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.zdbjq.cn/Article/details/glrasplie.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.zdbjq.cn/Article/details/gyybmzndj.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.zdbjq.cn/Article/details/gaqopgubq.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.hesvh.cn/Article/details/gktfyctcf.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.fehbvm.com/Article/details/gyzfklpex.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.fehbvm.com/Article/details/gdviggemj.sHtML

[U04] Py：变量调试打印
来源：http://blog.fehbvm.com/Article/details/gdduvobcf.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.zdbjq.cn/Article/details/gugnbgkry.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.fehbvm.com/Article/details/gdlsrkiqk.sHtML

list(dict.fromkeys(arr))
来源：http://wap.hesvh.cn/Article/details/glwnezmuf.sHtML

[U06] Py：合并两个字典
来源：http://www.share.zdbjq.cn/Article/details/gwdlrwkxt.sHtML

{**a, **b}
来源：http://www.blog.hesvh.cn/Article/details/gqktwsvdp.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.zdbjq.cn/Article/details/ggqjexgpz.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.zdbjq.cn/Article/details/gogkobezm.sHtML

[U08] Py：展平二维列表
来源：http://mobile.zdbjq.cn/Article/details/gffnwxnju.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.hesvh.cn/Article/details/gzsbwinpo.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.hesvh.cn/Article/details/gvnjuvkvc.sHtML

max(d, key=d.get)
来源：http://mobile.fehbvm.com/Article/details/grwvffblk.sHtML

[U10] Py：按值排序字典
来源：http://3g.fehbvm.com/Article/details/gcgsklzme.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.zdbjq.cn/Article/details/gdduhquuw.sHtML

[U11] Py：生成器表达式
来源：http://read.share.fehbvm.com/Article/details/glxbpveqf.sHtML

(x * 2 for x in arr)
来源：http://www.blog.fehbvm.com/Article/details/gametabfw.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.zdbjq.cn/Article/details/grvsuyqtn.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.fehbvm.com/Article/details/gmeibfcqq.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.hesvh.cn/Article/details/giufrztgz.sHtML

deque(maxlen=10)
来源：http://blog.zdbjq.cn/Article/details/gkgcbiqhx.sHtML

[U14] Py：分组收集到列表
来源：http://blog.zdbjq.cn/Article/details/gtzdtcdlv.sHtML

defaultdict(list)
来源：http://www.blog.zdbjq.cn/Article/details/glfwnvixt.sHtML

[U15] Py：高精度计时
来源：http://mobile.hesvh.cn/Article/details/gyrrfbgxo.sHtML

t = time.perf_counter()
来源：http://read.share.hesvh.cn/Article/details/gifzhuxfh.sHtML

[U16] Py：命令行参数解析
来源：http://wap.zdbjq.cn/Article/details/guzfdldar.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.fehbvm.com/Article/details/gtbpdusqt.sHtML

[U17] Py：初始化日志
来源：http://baike.zdbjq.cn/Article/details/groairpvl.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.hesvh.cn/Article/details/gmatizslr.sHtML

[U18] Py：预编译正则
来源：http://blog.zdbjq.cn/Article/details/gzspgnmiw.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.fehbvm.com/Article/details/gthaqeumr.sHtML

[U19] Py：正则替换带回调
来源：http://blog.zdbjq.cn/Article/details/gaafgdwec.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.zdbjq.cn/Article/details/grkfrowhb.sHtML

[U20] Py：缓存函数结果
来源：http://baike.fehbvm.com/Article/details/gtpzmnqjg.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.zdbjq.cn/Article/details/gohwkgpxd.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.zdbjq.cn/Article/details/ggodgrxsa.sHtML

@contextlib.contextmanager
来源：http://blog.zdbjq.cn/Article/details/gakkdmyxl.sHtML

[U22] Py：矩阵转置
来源：http://mobile.zdbjq.cn/Article/details/gscnenhpe.sHtML

list(zip(*m))
来源：http://read.share.fehbvm.com/Article/details/gzpkyhgfn.sHtML

[U23] Py：分块读取大文件
来源：http://wap.hesvh.cn/Article/details/gdwbwwtvt.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.hesvh.cn/Article/details/gjrpwipls.sHtML

[U24] Py：路径操作
来源：http://m.share.zdbjq.cn/Article/details/gpppgznix.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.fehbvm.com/Article/details/gcxxqppgv.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.fehbvm.com/Article/details/gfgkgheub.sHtML

csv.DictReader(f)
来源：http://www.m.share.hesvh.cn/Article/details/gxfolypbe.sHtML

[U26] Py：并发下载
来源：http://3g.hesvh.cn/Article/details/ganwvesqc.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.fehbvm.com/Article/details/gyixvzhxe.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.fehbvm.com/Article/details/gnwyxjlwp.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.zdbjq.cn/Article/details/grhozqsat.sHtML

[U28] Py：类型别名
来源：http://3g.hesvh.cn/Article/details/ghpwzdmut.sHtML

UserId = int
来源：http://baike.zdbjq.cn/Article/details/gwuihtigm.sHtML

[U29] Py：属性校验
来源：http://www.share.hesvh.cn/Article/details/getyporml.sHtML

@property 与 @x.setter 配合
来源：http://wap.fehbvm.com/Article/details/gwzqiyrmr.sHtML

[U30] Py：数据类
来源：http://www.blog.fehbvm.com/Article/details/gcctwkbsa.sHtML

@dataclass(slots=True)
来源：http://baike.hesvh.cn/Article/details/gnohsejei.sHtML

[U31] Py：单测
来源：http://read.share.fehbvm.com/Article/details/gpbzndujk.sHtML

python -m pytest -q
来源：http://baike.zdbjq.cn/Article/details/gnppjhjlf.sHtML

[U32] Py：代码格式化
来源：http://read.share.zdbjq.cn/Article/details/gfpctvkfz.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.fehbvm.com/Article/details/glqgcgyrr.sHtML

[U33] Py：打包发布
来源：http://3g.zdbjq.cn/Article/details/grkfjgdkd.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.zdbjq.cn/Article/details/glwtplafv.sHtML

[U34] Py：判断编码
来源：http://read.share.zdbjq.cn/Article/details/ghfoqeaki.sHtML

chardet.detect(raw)
来源：http://www.share.zdbjq.cn/Article/details/gohdaedtk.sHtML

[U35] Py：发送邮件
来源：http://blog.hesvh.cn/Article/details/gbnmgqbnk.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.hesvh.cn/Article/details/ghswebmvw.sHtML

[U36] Py：定时任务
来源：http://m.share.hesvh.cn/Article/details/gfmmwktmj.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.hesvh.cn/Article/details/gvborrjkv.sHtML

[U37] Py：读写 Excel
来源：http://blog.hesvh.cn/Article/details/gymkircaa.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.fehbvm.com/Article/details/gabpisraw.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.zdbjq.cn/Article/details/gpfsxtekx.sHtML

Path(__file__).resolve().parent
来源：http://baike.zdbjq.cn/Article/details/gfxifvcnz.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.zdbjq.cn/Article/details/gnarlxoiu.sHtML

sys.stdout.isatty()
来源：http://blog.zdbjq.cn/Article/details/gemjgbmpf.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.fehbvm.com/Article/details/gutzrqoya.sHtML

print("err", file=sys.stderr)
来源：http://m.share.fehbvm.com/Article/details/goggywhty.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.fehbvm.com/Article/details/ggzxcjsvp.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.zdbjq.cn/Article/details/guckljufp.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.hesvh.cn/Article/details/gneaygomy.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.zdbjq.cn/Article/details/gsnsqkxou.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.zdbjq.cn/Article/details/greopgmfj.sHtML

namespace App\Http;
来源：http://wap.zdbjq.cn/Article/details/gdoakbbrj.sHtML

[U44] PHP：开启严格类型
来源：http://wap.hesvh.cn/Article/details/guxccmlen.sHtML

declare(strict_types=1);
来源：http://blog.zdbjq.cn/Article/details/gmvsgqtmy.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.hesvh.cn/Article/details/gwgiyoymm.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/geemkeglu.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.hesvh.cn/Article/details/gljvesdaq.sHtML

?string $name = null
来源：http://baike.hesvh.cn/Article/details/guuuyhhsj.sHtML

[U47] PHP：联合类型
来源：http://m.share.hesvh.cn/Article/details/gxzaubmwj.sHtML

int|string $id
来源：http://m.share.hesvh.cn/Article/details/gadospoio.sHtML

[U48] PHP：纯枚举
来源：http://wap.hesvh.cn/Article/details/gedazhxyq.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnllvajvi.sHtML

[U49] PHP：只读属性
来源：http://3g.fehbvm.com/Article/details/gwhlnqurp.sHtML

public readonly string $name
来源：http://wap.fehbvm.com/Article/details/gvotvklmv.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.zdbjq.cn/Article/details/glhlmxkmv.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.fehbvm.com/Article/details/gphgsotnn.sHtML

[U51] PHP：数组解构
来源：http://www.share.hesvh.cn/Article/details/gcuytqtzk.sHtML

[$a, $b] = $arr;
来源：http://m.share.hesvh.cn/Article/details/gsulyrzmm.sHtML

[U52] PHP：箭头函数
来源：http://www.share.hesvh.cn/Article/details/glcxtztlr.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.fehbvm.com/Article/details/gmapvpefw.sHtML

[U53] PHP：空合并运算符
来源：http://wap.hesvh.cn/Article/details/gzrgdlbcn.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.hesvh.cn/Article/details/gjqmxizoi.sHtML

[U54] PHP：空安全调用
来源：http://blog.zdbjq.cn/Article/details/gkcrqbrad.sHtML

$obj?->method()
来源：http://3g.hesvh.cn/Article/details/giygtolqn.sHtML

[U55] PHP：match 表达式
来源：http://baike.zdbjq.cn/Article/details/gtfixkiwj.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.fehbvm.com/Article/details/gonhiutny.sHtML

[U56] PHP：命名参数
来源：http://mobile.zdbjq.cn/Article/details/gpvcoxyje.sHtML

f(a: 1, b: 2)
来源：http://3g.fehbvm.com/Article/details/gorfyqjyc.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gffyhplqw.sHtML

"值: {$a}"
来源：http://mobile.hesvh.cn/Article/details/gfmonjsyj.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.hesvh.cn/Article/details/gwumyxpfp.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.hesvh.cn/Article/details/guoxwaqbj.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.zdbjq.cn/Article/details/gartbtbih.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.hesvh.cn/Article/details/gkdbykouh.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.zdbjq.cn/Article/details/gonsdunrq.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.zdbjq.cn/Article/details/gzvsudvlu.sHtML

[U61] PHP：正则
来源：http://www.blog.hesvh.cn/Article/details/gzebvriwl.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gyrilgvxe.sHtML

[U62] PHP：日期对象
来源：http://mobile.zdbjq.cn/Article/details/ggyhscayl.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.fehbvm.com/Article/details/gucoulmlw.sHtML

[U63] PHP：文件读写
来源：http://blog.hesvh.cn/Article/details/gfzfjypil.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.zdbjq.cn/Article/details/gcfkdxhmo.sHtML

[U64] PHP：目录遍历
来源：http://blog.zdbjq.cn/Article/details/gqiqkmcfm.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.fehbvm.com/Article/details/gamhwxepg.sHtML

[U65] PHP：会话
来源：http://3g.fehbvm.com/Article/details/ggystlbem.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.hesvh.cn/Article/details/gloslcxjf.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.fehbvm.com/Article/details/grmpgaksb.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.fehbvm.com/Article/details/gfakqxxtr.sHtML

[U67] PHP：处理文件上传
来源：http://blog.zdbjq.cn/Article/details/gorcbvfpz.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.fehbvm.com/Article/details/glpbvyimd.sHtML

[U68] PHP：PDO 连接
来源：http://baike.zdbjq.cn/Article/details/gptcjkvue.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.fehbvm.com/Article/details/gfoppwhgt.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.fehbvm.com/Article/details/gheamzkjn.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.zdbjq.cn/Article/details/gariwxrwj.sHtML

[U70] PHP：PDO 事务
来源：http://blog.fehbvm.com/Article/details/grpdcbdlp.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.hesvh.cn/Article/details/gefzghqbm.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.zdbjq.cn/Article/details/gyzaxsmif.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.zdbjq.cn/Article/details/gkoygszot.sHtML

[U72] PHP：写错误日志
来源：http://m.share.fehbvm.com/Article/details/gdisqetqp.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.hesvh.cn/Article/details/gnfhtmylf.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.hesvh.cn/Article/details/gynmngbkx.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.hesvh.cn/Article/details/gymozfvhi.sHtML

[U74] PHP：读取环境变量
来源：http://blog.fehbvm.com/Article/details/gfvzvehgk.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.hesvh.cn/Article/details/gyufhgvdt.sHtML

[U75] PHP：依赖注入
来源：http://blog.zdbjq.cn/Article/details/glaeedgfz.sHtML

composer require psr/container
来源：http://www.share.zdbjq.cn/Article/details/gwkjqphny.sHtML

[U76] PHP：简单路由
来源：http://m.share.zdbjq.cn/Article/details/gbqftjsiv.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.fehbvm.com/Article/details/gywuawxnu.sHtML

[U77] PHP：模板渲染
来源：http://baike.fehbvm.com/Article/details/guvyjprko.sHtML

composer require twig/twig
来源：http://wap.fehbvm.com/Article/details/gvdhxpgiv.sHtML

[U78] PHP：单元测试
来源：http://mobile.fehbvm.com/Article/details/gsdzyzvbb.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.zdbjq.cn/Article/details/gmsxesqqr.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.hesvh.cn/Article/details/giecliqya.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.fehbvm.com/Article/details/glxkhxoeo.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.zdbjq.cn/Article/details/gywzeekzf.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.hesvh.cn/Article/details/gnpnsrokp.sHtML

[U81] JS：初始化项目
来源：http://www.share.hesvh.cn/Article/details/gaqtkixbu.sHtML

npm init -y;  npm i express
来源：http://wap.zdbjq.cn/Article/details/gqtlqkzcz.sHtML

[U82] JS：package.json 脚本
来源：http://wap.fehbvm.com/Article/details/ggrntoalc.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.fehbvm.com/Article/details/glaqyotyw.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.hesvh.cn/Article/details/gsabollxu.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.zdbjq.cn/Article/details/gyfipbexl.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.fehbvm.com/Article/details/gfynwdepb.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.fehbvm.com/Article/details/gipihehiw.sHtML


<!-- 参考信息 -->