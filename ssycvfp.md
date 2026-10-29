代发 wailian999

namespace ns { int f() { return 1; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gcgmmsdca.sHtML

[S59] C++：静态断言
来源：http://mobile.zdbjq.cn/Article/details/gfpvbdnwv.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.zdbjq.cn/Article/details/gejbswosv.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fehbvm.com/Article/details/gktuyefyc.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.zdbjq.cn/Article/details/ggpepuwsh.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gevcqhirt.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.hesvh.cn/Article/details/gqtpmfvjg.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gidnfeiyp.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gvzjavrsk.sHtML

println("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gazdiussl.sHtML

[T02] Kotlin：变量
来源：http://baike.hesvh.cn/Article/details/gjfmnyshs.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.hesvh.cn/Article/details/gefkrhmtq.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.zdbjq.cn/Article/details/gmefcnecz.sHtML

"值: $b"
来源：http://baike.fehbvm.com/Article/details/gdsdpyzqs.sHtML

[T04] Kotlin：空安全
来源：http://www.share.hesvh.cn/Article/details/gwwtivhmt.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.hesvh.cn/Article/details/gzrciogpb.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.zdbjq.cn/Article/details/govjqrzgl.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fehbvm.com/Article/details/gmgrlrorb.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.hesvh.cn/Article/details/gvwoetnne.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.hesvh.cn/Article/details/gwvxstycb.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.hesvh.cn/Article/details/gpqklbeqr.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.hesvh.cn/Article/details/gzsstmkgb.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.zdbjq.cn/Article/details/gzapfdstp.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.hesvh.cn/Article/details/gpactlpvf.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.zdbjq.cn/Article/details/gczhnhsop.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.zdbjq.cn/Article/details/gneonkrhv.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.zdbjq.cn/Article/details/ghfsqtyuw.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fehbvm.com/Article/details/gkondywkt.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.hesvh.cn/Article/details/gzrntypzb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.zdbjq.cn/Article/details/gpjmuulgc.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.hesvh.cn/Article/details/gtlzckcww.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.hesvh.cn/Article/details/gkdxaefha.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.zdbjq.cn/Article/details/gtycuehqb.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.zdbjq.cn/Article/details/gzhkypagr.sHtML

[T14] Kotlin：循环
来源：http://mobile.hesvh.cn/Article/details/gucjcudwr.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/grtwecmkl.sHtML

[T15] Kotlin：接口
来源：http://www.share.zdbjq.cn/Article/details/gyfljmqyi.sHtML

interface Shape { fun area(): Double }
来源：http://wap.hesvh.cn/Article/details/gojhsmtwt.sHtML

[T16] Swift：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gifgeepnw.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/gdquwsnbb.sHtML

[T17] Swift：变量与常量
来源：http://blog.zdbjq.cn/Article/details/gbakgpllp.sHtML

var a = 1;  let b = 2
来源：http://wap.zdbjq.cn/Article/details/gbbdqiefj.sHtML

[T18] Swift：字符串插值
来源：http://3g.hesvh.cn/Article/details/gipwgpogc.sHtML

"值: \(b)"
来源：http://blog.hesvh.cn/Article/details/gmqdbqgfx.sHtML

[T19] Swift：可选绑定
来源：http://wap.fehbvm.com/Article/details/gquaaavve.sHtML

if let n = opt { print(n) }
来源：http://m.share.fehbvm.com/Article/details/goroxowye.sHtML

[T20] Swift：数组操作
来源：http://www.share.zdbjq.cn/Article/details/gmzfqfbce.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fehbvm.com/Article/details/ghockiujb.sHtML

[T21] Swift：遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gbznnntqn.sHtML

for x in a { print(x) }
来源：http://baike.fehbvm.com/Article/details/ginhukkrt.sHtML

[T22] Swift：字典
来源：http://mobile.fehbvm.com/Article/details/gyvyxpmpc.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.zdbjq.cn/Article/details/gtfclfrfu.sHtML

[T23] Swift：函数
来源：http://m.share.hesvh.cn/Article/details/gwqjgrdxv.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.hesvh.cn/Article/details/gghyrvfya.sHtML

[T24] Swift：闭包
来源：http://read.share.fehbvm.com/Article/details/gdmchdajx.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.hesvh.cn/Article/details/gujmejgll.sHtML

[T25] Swift：结构体
来源：http://wap.hesvh.cn/Article/details/gvbjmiegc.sHtML

struct P { var x: Int }
来源：http://baike.zdbjq.cn/Article/details/gmdexalid.sHtML

[T26] Swift：类与重写
来源：http://wap.zdbjq.cn/Article/details/gtboahsri.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fehbvm.com/Article/details/gxpizdsxh.sHtML

[T27] Swift：错误处理
来源：http://read.share.zdbjq.cn/Article/details/gluwboceq.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fehbvm.com/Article/details/gskdjctvx.sHtML

[T28] Swift：枚举
来源：http://read.share.fehbvm.com/Article/details/gnvmsvxzm.sHtML

enum Color { case red, green }
来源：http://baike.hesvh.cn/Article/details/gfqngckfv.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.hesvh.cn/Article/details/gndmamojh.sHtML

guard let x = opt else { return }
来源：http://www.m.share.hesvh.cn/Article/details/gxfynxcwj.sHtML

[T30] Swift：协议
来源：http://wap.zdbjq.cn/Article/details/gkjtsguei.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.zdbjq.cn/Article/details/glmrhvcef.sHtML

[T31] Lua：Hello World
来源：http://baike.fehbvm.com/Article/details/gxjislgvf.sHtML

print("Hello")
来源：http://3g.zdbjq.cn/Article/details/gfvkbfkvg.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.hesvh.cn/Article/details/gntmzyqer.sHtML

local a = 1
来源：http://wap.hesvh.cn/Article/details/gdixkukkl.sHtML

[T33] Lua：表（数组）
来源：http://blog.zdbjq.cn/Article/details/gupcktviq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.hesvh.cn/Article/details/gadvwflvh.sHtML

[T34] Lua：遍历表
来源：http://www.share.zdbjq.cn/Article/details/gaqutmllh.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.fehbvm.com/Article/details/gbftoyuvf.sHtML

[T35] Lua：字典表
来源：http://www.share.hesvh.cn/Article/details/gvnzygqbs.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gukkwrfci.sHtML

[T36] Lua：函数
来源：http://3g.hesvh.cn/Article/details/gatvdtusf.sHtML

function add(a, b) return a + b end
来源：http://read.share.fehbvm.com/Article/details/gsntycyuo.sHtML

[T37] Lua：字符串拼接
来源：http://wap.hesvh.cn/Article/details/glnihrgff.sHtML

"a" .. "b"
来源：http://read.share.hesvh.cn/Article/details/gcqrfbxmg.sHtML

[T38] Lua：条件
来源：http://www.m.share.hesvh.cn/Article/details/grpkuwjfm.sHtML

if x > 0 then print("正") end
来源：http://mobile.hesvh.cn/Article/details/grnpojfym.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fehbvm.com/Article/details/gyfeuwvlk.sHtML

string.find(s, "%d+")
来源：http://baike.zdbjq.cn/Article/details/gexvvmvkb.sHtML

[T40] Lua：元表
来源：http://blog.hesvh.cn/Article/details/gujczemoh.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.fehbvm.com/Article/details/ghxwiiofr.sHtML

[T41] Perl：Hello World
来源：http://baike.hesvh.cn/Article/details/guuetyber.sHtML

print "Hello\n";
来源：http://blog.hesvh.cn/Article/details/grtdnyxhv.sHtML

[T42] Perl：变量类型
来源：http://www.share.zdbjq.cn/Article/details/godjcxxjh.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.hesvh.cn/Article/details/guhwdpkcj.sHtML

[T43] Perl：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gkljwhyoh.sHtML

"值: $a"
来源：http://3g.zdbjq.cn/Article/details/gglwikmyc.sHtML

[T44] Perl：条件
来源：http://mobile.fehbvm.com/Article/details/ghhehpbps.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.hesvh.cn/Article/details/ghloicsiv.sHtML

[T45] Perl：数组遍历
来源：http://m.share.fehbvm.com/Article/details/gcbbbsblr.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.zdbjq.cn/Article/details/gdvcjvjdp.sHtML

[T46] Perl：哈希操作
来源：http://3g.hesvh.cn/Article/details/ghutgxkvk.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.hesvh.cn/Article/details/gipyykxjg.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.hesvh.cn/Article/details/gciyjzzri.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.hesvh.cn/Article/details/gkneiahod.sHtML

[T48] Perl：正则替换
来源：http://3g.hesvh.cn/Article/details/gqvqfbord.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.hesvh.cn/Article/details/gucdrxjwz.sHtML

[T49] Perl：函数
来源：http://3g.hesvh.cn/Article/details/gqwcgtrky.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gskyxtqmq.sHtML

[T50] Perl：逐行读文件
来源：http://baike.hesvh.cn/Article/details/ggcmzfdeo.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.fehbvm.com/Article/details/gmtwrpqxt.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.hesvh.cn/Article/details/gyqdizqvt.sHtML

[T51] Scala：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gimrghfvq.sHtML

println("Hello")
来源：http://m.share.fehbvm.com/Article/details/gzivvdexx.sHtML

[T52] Scala：变量
来源：http://m.share.fehbvm.com/Article/details/gnfecthyx.sHtML

val a = 1;  var b = 2
来源：http://3g.fehbvm.com/Article/details/gghajfyyg.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gwfsdclvz.sHtML

s"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/gvlfdnsky.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.hesvh.cn/Article/details/ggjkddqcc.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.zdbjq.cn/Article/details/golytjitj.sHtML

[T55] Scala：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/gblxubcjy.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.hesvh.cn/Article/details/gzxbtpujz.sHtML

[T56] Scala：样例类
来源：http://baike.hesvh.cn/Article/details/gxdwglada.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.zdbjq.cn/Article/details/grnimbunw.sHtML

[T57] Scala：模式匹配
来源：http://mobile.hesvh.cn/Article/details/gmlojpjsu.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.fehbvm.com/Article/details/gjdyohfsh.sHtML

[T58] Scala：函数定义
来源：http://www.blog.hesvh.cn/Article/details/gppxnhslj.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.zdbjq.cn/Article/details/gjltmtzmb.sHtML

[T59] Scala：循环
来源：http://www.share.hesvh.cn/Article/details/gwnbmuyxc.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.zdbjq.cn/Article/details/gfcpxyfhv.sHtML

[T60] Scala：折叠
来源：http://www.m.share.hesvh.cn/Article/details/gptyguuyq.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.hesvh.cn/Article/details/gjnkylmzu.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/giktpzdpt.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.hesvh.cn/Article/details/gdkjaewks.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gswnttsaj.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.zdbjq.cn/Article/details/grlgbgkxv.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.hesvh.cn/Article/details/ggqukqqqk.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.zdbjq.cn/Article/details/gygcfkwar.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.fehbvm.com/Article/details/ghxdfpbxj.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.hesvh.cn/Article/details/gzwuyghgs.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.hesvh.cn/Article/details/gtzwifmfy.sHtML

[U04] Py：变量调试打印
来源：http://m.share.hesvh.cn/Article/details/gjbwycluu.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.fehbvm.com/Article/details/grawuhmgb.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.zdbjq.cn/Article/details/gwlwyymlj.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/gcdgphabl.sHtML

[U06] Py：合并两个字典
来源：http://3g.zdbjq.cn/Article/details/ghzvcwuye.sHtML

{**a, **b}
来源：http://m.share.zdbjq.cn/Article/details/gixoagjvd.sHtML

[U07] Py：反转字典键值
来源：http://baike.fehbvm.com/Article/details/gcpprzqce.sHtML

{v: k for k, v in d.items()}
来源：http://3g.hesvh.cn/Article/details/gqupcpbai.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.fehbvm.com/Article/details/gxcnvbxxq.sHtML

[y for x in nested for y in x]
来源：http://www.share.fehbvm.com/Article/details/gvibkdhgq.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.zdbjq.cn/Article/details/gljvwbrhk.sHtML

max(d, key=d.get)
来源：http://wap.zdbjq.cn/Article/details/gqxdipjmt.sHtML

[U10] Py：按值排序字典
来源：http://www.share.hesvh.cn/Article/details/gpjvjkqfw.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.fehbvm.com/Article/details/gcedekbia.sHtML

[U11] Py：生成器表达式
来源：http://www.share.zdbjq.cn/Article/details/gblbsddfr.sHtML

(x * 2 for x in arr)
来源：http://baike.fehbvm.com/Article/details/gitanrpsf.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.zdbjq.cn/Article/details/gvnrjpywm.sHtML

Counter(arr).most_common(3)
来源：http://blog.fehbvm.com/Article/details/glsategor.sHtML

[U13] Py：固定长度队列
来源：http://baike.fehbvm.com/Article/details/guilbnauc.sHtML

deque(maxlen=10)
来源：http://baike.fehbvm.com/Article/details/gmszzzhzy.sHtML

[U14] Py：分组收集到列表
来源：http://blog.fehbvm.com/Article/details/gfxuhnjfo.sHtML

defaultdict(list)
来源：http://www.blog.fehbvm.com/Article/details/ggeqpslnq.sHtML

[U15] Py：高精度计时
来源：http://www.share.fehbvm.com/Article/details/gnrlippnb.sHtML

t = time.perf_counter()
来源：http://www.m.share.zdbjq.cn/Article/details/gedwglqox.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.hesvh.cn/Article/details/gzvwcdyan.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.fehbvm.com/Article/details/gjeiwytof.sHtML

[U17] Py：初始化日志
来源：http://3g.zdbjq.cn/Article/details/gdohatdcv.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.hesvh.cn/Article/details/ghemmfobw.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.hesvh.cn/Article/details/gfugyrzpp.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.fehbvm.com/Article/details/gutmlafyt.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.zdbjq.cn/Article/details/grflsfmyj.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.hesvh.cn/Article/details/gjjwqctyd.sHtML

[U20] Py：缓存函数结果
来源：http://blog.hesvh.cn/Article/details/gsketbihu.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.zdbjq.cn/Article/details/gkpbmqqlt.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.fehbvm.com/Article/details/gehtwprga.sHtML

@contextlib.contextmanager
来源：http://m.share.hesvh.cn/Article/details/giegtxjkf.sHtML

[U22] Py：矩阵转置
来源：http://wap.hesvh.cn/Article/details/gloutzfyk.sHtML

list(zip(*m))
来源：http://wap.zdbjq.cn/Article/details/gjrgwgwyr.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.fehbvm.com/Article/details/gvemoqtue.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.hesvh.cn/Article/details/gxazwqirj.sHtML

[U24] Py：路径操作
来源：http://mobile.zdbjq.cn/Article/details/gmmjmeyxa.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.hesvh.cn/Article/details/gyntcqjaj.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.hesvh.cn/Article/details/ghsglzhxb.sHtML

csv.DictReader(f)
来源：http://www.m.share.fehbvm.com/Article/details/gjjjtoisw.sHtML

[U26] Py：并发下载
来源：http://blog.zdbjq.cn/Article/details/gzpwaeotq.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.fehbvm.com/Article/details/goaznxspc.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.fehbvm.com/Article/details/gnweqlcjx.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.zdbjq.cn/Article/details/gemgwqdcv.sHtML

[U28] Py：类型别名
来源：http://mobile.fehbvm.com/Article/details/gxcezmjkv.sHtML

UserId = int
来源：http://blog.fehbvm.com/Article/details/gtatusbpw.sHtML

[U29] Py：属性校验
来源：http://www.m.share.fehbvm.com/Article/details/gzizhxtdx.sHtML

@property 与 @x.setter 配合
来源：http://read.share.fehbvm.com/Article/details/gpafciiil.sHtML

[U30] Py：数据类
来源：http://blog.zdbjq.cn/Article/details/gaxbogbtv.sHtML

@dataclass(slots=True)
来源：http://www.share.hesvh.cn/Article/details/gvpeiwnjj.sHtML

[U31] Py：单测
来源：http://read.share.hesvh.cn/Article/details/gauaqowsm.sHtML

python -m pytest -q
来源：http://mobile.fehbvm.com/Article/details/gvjdpbtwg.sHtML

[U32] Py：代码格式化
来源：http://www.share.zdbjq.cn/Article/details/gyyoqetxq.sHtML

ruff format . && ruff check --fix .
来源：http://3g.fehbvm.com/Article/details/gcdiiqjlv.sHtML

[U33] Py：打包发布
来源：http://baike.fehbvm.com/Article/details/gbnclymfb.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.hesvh.cn/Article/details/gzcodchod.sHtML

[U34] Py：判断编码
来源：http://wap.fehbvm.com/Article/details/grzneuuof.sHtML

chardet.detect(raw)
来源：http://3g.hesvh.cn/Article/details/gqiplakpf.sHtML

[U35] Py：发送邮件
来源：http://www.share.zdbjq.cn/Article/details/glqwazixf.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.hesvh.cn/Article/details/guarfplxh.sHtML

[U36] Py：定时任务
来源：http://blog.fehbvm.com/Article/details/ghsnrquzp.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.fehbvm.com/Article/details/ghuqgkzwh.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.fehbvm.com/Article/details/ggwsjnokq.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.fehbvm.com/Article/details/gdmekmhyy.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.zdbjq.cn/Article/details/gkjgoyasi.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.fehbvm.com/Article/details/gimqszvdz.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.hesvh.cn/Article/details/gqlwicctl.sHtML

sys.stdout.isatty()
来源：http://mobile.hesvh.cn/Article/details/glekrcbiy.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.zdbjq.cn/Article/details/gpolqlhys.sHtML

print("err", file=sys.stderr)
来源：http://read.share.fehbvm.com/Article/details/gslsngzwm.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.hesvh.cn/Article/details/gfiladvgv.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.fehbvm.com/Article/details/ghfrervds.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.fehbvm.com/Article/details/gqynyzmrm.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.fehbvm.com/Article/details/gqjaccfsq.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.fehbvm.com/Article/details/geopnwput.sHtML

namespace App\Http;
来源：http://baike.fehbvm.com/Article/details/gosmmqxnu.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.zdbjq.cn/Article/details/gjoqrfxec.sHtML

declare(strict_types=1);
来源：http://www.blog.hesvh.cn/Article/details/galtnvbmi.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.hesvh.cn/Article/details/gttabyozm.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gqoiooqih.sHtML

[U46] PHP：可空类型
来源：http://3g.zdbjq.cn/Article/details/gdrlrvaoz.sHtML

?string $name = null
来源：http://www.blog.zdbjq.cn/Article/details/gaeihcwtp.sHtML

[U47] PHP：联合类型
来源：http://blog.hesvh.cn/Article/details/gnlmfxndg.sHtML

int|string $id
来源：http://mobile.zdbjq.cn/Article/details/gzvvkwnrd.sHtML

[U48] PHP：纯枚举
来源：http://mobile.zdbjq.cn/Article/details/gkwxjutml.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.fehbvm.com/Article/details/gfsmyrtzi.sHtML

[U49] PHP：只读属性
来源：http://m.share.hesvh.cn/Article/details/gqseypakm.sHtML

public readonly string $name
来源：http://read.share.hesvh.cn/Article/details/gwtnmolpc.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.hesvh.cn/Article/details/gqvmagyds.sHtML

public function __construct(private int $id) {}
来源：http://mobile.hesvh.cn/Article/details/gxozoczis.sHtML

[U51] PHP：数组解构
来源：http://read.share.fehbvm.com/Article/details/gtduxnejw.sHtML

[$a, $b] = $arr;
来源：http://www.share.zdbjq.cn/Article/details/guzzmywsy.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.zdbjq.cn/Article/details/gcigvcajl.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.zdbjq.cn/Article/details/gofklnwsb.sHtML

[U53] PHP：空合并运算符
来源：http://wap.hesvh.cn/Article/details/gdjggoyzz.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.zdbjq.cn/Article/details/gkimhdkzm.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.fehbvm.com/Article/details/goztkxeih.sHtML

$obj?->method()
来源：http://blog.fehbvm.com/Article/details/gmfzbkpyw.sHtML

[U55] PHP：match 表达式
来源：http://baike.fehbvm.com/Article/details/gbbdmnkdp.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.hesvh.cn/Article/details/gljewoqrh.sHtML

[U56] PHP：命名参数
来源：http://www.share.fehbvm.com/Article/details/gdounakqf.sHtML

f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/gzlggmpmw.sHtML

[U57] PHP：字符串插值
来源：http://3g.fehbvm.com/Article/details/gsfejlptq.sHtML

"值: {$a}"
来源：http://m.share.fehbvm.com/Article/details/gvnozlldd.sHtML

[U58] PHP：数组三件套
来源：http://wap.hesvh.cn/Article/details/gccwnzhrb.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.fehbvm.com/Article/details/geldolmim.sHtML

[U59] PHP：自定义排序
来源：http://blog.hesvh.cn/Article/details/guqdcwenw.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.zdbjq.cn/Article/details/gwfbvjxch.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.fehbvm.com/Article/details/gmrybjatw.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.zdbjq.cn/Article/details/gmfkjywrc.sHtML

[U61] PHP：正则
来源：http://m.share.zdbjq.cn/Article/details/gvddgcsfe.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.zdbjq.cn/Article/details/gmppliekv.sHtML

[U62] PHP：日期对象
来源：http://read.share.fehbvm.com/Article/details/gfhjhcvle.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.zdbjq.cn/Article/details/gtqpfztik.sHtML

[U63] PHP：文件读写
来源：http://www.blog.zdbjq.cn/Article/details/gcwnbgopf.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.fehbvm.com/Article/details/guzsonngy.sHtML

[U64] PHP：目录遍历
来源：http://3g.hesvh.cn/Article/details/gvbiyxiud.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.zdbjq.cn/Article/details/ggulrqzwe.sHtML

[U65] PHP：会话
来源：http://baike.hesvh.cn/Article/details/gftxmtaga.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gfmivmdsq.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.fehbvm.com/Article/details/gamhuwcbw.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.hesvh.cn/Article/details/griyninth.sHtML

[U67] PHP：处理文件上传
来源：http://blog.fehbvm.com/Article/details/gqminyiug.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.zdbjq.cn/Article/details/gjtpdchsb.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.fehbvm.com/Article/details/giobaxsnl.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.zdbjq.cn/Article/details/gvqlccshi.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.hesvh.cn/Article/details/ghywwvipx.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.fehbvm.com/Article/details/gghuwvqzr.sHtML

[U70] PHP：PDO 事务
来源：http://baike.fehbvm.com/Article/details/gobwmhdlp.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.zdbjq.cn/Article/details/gzhtxfadg.sHtML

[U71] PHP：抛出异常
来源：http://baike.fehbvm.com/Article/details/gtckmtdlx.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.hesvh.cn/Article/details/gyjzxmpip.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.hesvh.cn/Article/details/ganbhqwan.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.zdbjq.cn/Article/details/gbtoijqmf.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.fehbvm.com/Article/details/gclfiiozr.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.fehbvm.com/Article/details/gemliiixt.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.fehbvm.com/Article/details/gmdjjdyne.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.fehbvm.com/Article/details/gnfrbqtff.sHtML

[U75] PHP：依赖注入
来源：http://blog.hesvh.cn/Article/details/gshlkjuuj.sHtML

composer require psr/container
来源：http://read.share.zdbjq.cn/Article/details/ggafvzoof.sHtML

[U76] PHP：简单路由
来源：http://www.share.zdbjq.cn/Article/details/gqkumambm.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.zdbjq.cn/Article/details/gjpvwzdzr.sHtML

[U77] PHP：模板渲染
来源：http://www.share.hesvh.cn/Article/details/gqdceqplr.sHtML

composer require twig/twig
来源：http://www.blog.hesvh.cn/Article/details/gyvvdyxjr.sHtML

[U78] PHP：单元测试
来源：http://3g.zdbjq.cn/Article/details/gaslvdhsj.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.zdbjq.cn/Article/details/gdrkadzpm.sHtML

[U79] PHP：静态分析
来源：http://blog.zdbjq.cn/Article/details/gwxisrera.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.zdbjq.cn/Article/details/grhfqmunh.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.hesvh.cn/Article/details/gxwzkdhoq.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.fehbvm.com/Article/details/gtqmqmlvw.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.hesvh.cn/Article/details/gihbnuqyj.sHtML

npm init -y;  npm i express
来源：http://baike.hesvh.cn/Article/details/gtrsimkzl.sHtML

[U82] JS：package.json 脚本
来源：http://wap.hesvh.cn/Article/details/ggshivmdd.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.hesvh.cn/Article/details/gmlzperff.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.fehbvm.com/Article/details/giyeafdlu.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.hesvh.cn/Article/details/gbesryexx.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.zdbjq.cn/Article/details/gjztdqbtc.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.zdbjq.cn/Article/details/guwieigfp.sHtML


<!-- 参考信息 -->