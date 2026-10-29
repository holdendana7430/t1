代发 wailian999

[T01] Kotlin：Hello World
来源：http://read.share.hesvh.cn/Article/details/glhwhwmvm.sHtML

println("Hello")
来源：http://wap.hesvh.cn/Article/details/gpmyqaoeo.sHtML

[T02] Kotlin：变量
来源：http://3g.hesvh.cn/Article/details/gskybiaif.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fehbvm.com/Article/details/gzbvzuyjv.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.zdbjq.cn/Article/details/gttjdisod.sHtML

"值: $b"
来源：http://blog.hesvh.cn/Article/details/gkcbblamo.sHtML

[T04] Kotlin：空安全
来源：http://baike.hesvh.cn/Article/details/ghbesvpwi.sHtML

val n: String? = null;  n?.length
来源：http://3g.hesvh.cn/Article/details/gfigwpcfu.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.zdbjq.cn/Article/details/gszzskvvo.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.hesvh.cn/Article/details/gukkpzvbp.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.hesvh.cn/Article/details/ggmymxtxy.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.zdbjq.cn/Article/details/gefjlclyu.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.zdbjq.cn/Article/details/gkvdgaunf.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fehbvm.com/Article/details/giaygerwr.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.hesvh.cn/Article/details/gwazzwzeh.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.zdbjq.cn/Article/details/gwgwlqjtf.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.zdbjq.cn/Article/details/gvybkxlzp.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.zdbjq.cn/Article/details/ghpkhyylo.sHtML

[T10] Kotlin：默认参数
来源：http://wap.zdbjq.cn/Article/details/gfwqxclcc.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.zdbjq.cn/Article/details/glmejykxt.sHtML

[T11] Kotlin：协程
来源：http://mobile.fehbvm.com/Article/details/gelovwrfm.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.zdbjq.cn/Article/details/gukgtwsew.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fehbvm.com/Article/details/gbvhbuzly.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gepqpkidq.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.hesvh.cn/Article/details/gmiwnssfu.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.hesvh.cn/Article/details/gidulysdo.sHtML

[T14] Kotlin：循环
来源：http://read.share.hesvh.cn/Article/details/gwbvojmlg.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.zdbjq.cn/Article/details/gievzcdun.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.hesvh.cn/Article/details/gojggrhep.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fehbvm.com/Article/details/gjddpekaf.sHtML

[T16] Swift：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gdtgarryv.sHtML

print("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gpoaaigas.sHtML

[T17] Swift：变量与常量
来源：http://blog.hesvh.cn/Article/details/gyhrpcxdn.sHtML

var a = 1;  let b = 2
来源：http://blog.hesvh.cn/Article/details/gnhugrjbi.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/garalsbad.sHtML

"值: \(b)"
来源：http://www.share.zdbjq.cn/Article/details/gkunssttd.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.zdbjq.cn/Article/details/guqrfvsxf.sHtML

if let n = opt { print(n) }
来源：http://www.blog.hesvh.cn/Article/details/gprrwbqex.sHtML

[T20] Swift：数组操作
来源：http://wap.hesvh.cn/Article/details/gipdpqndp.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.hesvh.cn/Article/details/ggytdhkbz.sHtML

[T21] Swift：遍历
来源：http://blog.zdbjq.cn/Article/details/guiaelnpo.sHtML

for x in a { print(x) }
来源：http://baike.fehbvm.com/Article/details/gtwdagmbj.sHtML

[T22] Swift：字典
来源：http://www.share.hesvh.cn/Article/details/gibjgemcb.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.zdbjq.cn/Article/details/ghdumettm.sHtML

[T23] Swift：函数
来源：http://3g.fehbvm.com/Article/details/gmmeavjrc.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.zdbjq.cn/Article/details/gpszarbme.sHtML

[T24] Swift：闭包
来源：http://blog.fehbvm.com/Article/details/gzbxqrmdy.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gpojoaxnt.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fehbvm.com/Article/details/gywjoymre.sHtML

struct P { var x: Int }
来源：http://m.share.hesvh.cn/Article/details/gxdogxshu.sHtML

[T26] Swift：类与重写
来源：http://baike.hesvh.cn/Article/details/gmczdusbr.sHtML

class A: Base { override func f() {} }
来源：http://m.share.zdbjq.cn/Article/details/ggqjweoul.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.hesvh.cn/Article/details/griwznqip.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.zdbjq.cn/Article/details/gctlxxaso.sHtML

[T28] Swift：枚举
来源：http://3g.zdbjq.cn/Article/details/gihfudplj.sHtML

enum Color { case red, green }
来源：http://mobile.hesvh.cn/Article/details/gzoimofet.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.zdbjq.cn/Article/details/gvlvygwni.sHtML

guard let x = opt else { return }
来源：http://m.share.hesvh.cn/Article/details/gswsypgst.sHtML

[T30] Swift：协议
来源：http://m.share.fehbvm.com/Article/details/gveeuuysp.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.fehbvm.com/Article/details/gzewkpzov.sHtML

[T31] Lua：Hello World
来源：http://wap.zdbjq.cn/Article/details/gozdlnfyh.sHtML

print("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gondvxkdv.sHtML

[T32] Lua：局部变量
来源：http://blog.fehbvm.com/Article/details/gxsxigkkr.sHtML

local a = 1
来源：http://m.share.hesvh.cn/Article/details/gperkdksw.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.fehbvm.com/Article/details/gtltnuqls.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.fehbvm.com/Article/details/gurvkkspc.sHtML

[T34] Lua：遍历表
来源：http://3g.zdbjq.cn/Article/details/gcosauceq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.hesvh.cn/Article/details/gvxwituvv.sHtML

[T35] Lua：字典表
来源：http://read.share.fehbvm.com/Article/details/goaxclwmn.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gieqjveye.sHtML

[T36] Lua：函数
来源：http://www.blog.zdbjq.cn/Article/details/ggyxukqol.sHtML

function add(a, b) return a + b end
来源：http://www.blog.zdbjq.cn/Article/details/gskftdvob.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.fehbvm.com/Article/details/gmbcrjwaq.sHtML

"a" .. "b"
来源：http://read.share.zdbjq.cn/Article/details/gsybdtdvx.sHtML

[T38] Lua：条件
来源：http://read.share.hesvh.cn/Article/details/gadijvzvt.sHtML

if x > 0 then print("正") end
来源：http://m.share.hesvh.cn/Article/details/guuemocru.sHtML

[T39] Lua：模式匹配
来源：http://read.share.zdbjq.cn/Article/details/gxuhdpuyz.sHtML

string.find(s, "%d+")
来源：http://wap.fehbvm.com/Article/details/gxrkgoimk.sHtML

[T40] Lua：元表
来源：http://www.blog.hesvh.cn/Article/details/gzzcmwlhc.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.hesvh.cn/Article/details/gznuitjax.sHtML

[T41] Perl：Hello World
来源：http://baike.hesvh.cn/Article/details/grzyurvkx.sHtML

print "Hello\n";
来源：http://baike.zdbjq.cn/Article/details/gqrueslzg.sHtML

[T42] Perl：变量类型
来源：http://wap.zdbjq.cn/Article/details/gigtepiwh.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.zdbjq.cn/Article/details/gjnfbbxpx.sHtML

[T43] Perl：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gmswyouam.sHtML

"值: $a"
来源：http://mobile.hesvh.cn/Article/details/gzzcvcpqq.sHtML

[T44] Perl：条件
来源：http://m.share.hesvh.cn/Article/details/gbhrylehz.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.hesvh.cn/Article/details/gccxrnixe.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.zdbjq.cn/Article/details/ggeqsclar.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fehbvm.com/Article/details/gvpgqvvtt.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.fehbvm.com/Article/details/gppcpbndw.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.zdbjq.cn/Article/details/gaihcjpop.sHtML

[T47] Perl：正则捕获
来源：http://www.share.hesvh.cn/Article/details/gwfpthmdm.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.fehbvm.com/Article/details/ghwppeipk.sHtML

[T48] Perl：正则替换
来源：http://mobile.hesvh.cn/Article/details/gehqxpxew.sHtML

$s =~ s/old/new/g;
来源：http://3g.hesvh.cn/Article/details/getlfusml.sHtML

[T49] Perl：函数
来源：http://www.share.fehbvm.com/Article/details/gagpbtzak.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gtgbgfban.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gpzqwaqyf.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.fehbvm.com/Article/details/ggqwqvjar.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.hesvh.cn/Article/details/gemlqdhvt.sHtML

[T51] Scala：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gtfnzpvje.sHtML

println("Hello")
来源：http://wap.hesvh.cn/Article/details/gwhbkfjce.sHtML

[T52] Scala：变量
来源：http://read.share.zdbjq.cn/Article/details/gxihxohqa.sHtML

val a = 1;  var b = 2
来源：http://blog.hesvh.cn/Article/details/ghcvirbmy.sHtML

[T53] Scala：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gsshtsxbp.sHtML

s"值: $b"
来源：http://www.blog.hesvh.cn/Article/details/gtuitpjrg.sHtML

[T54] Scala：集合映射
来源：http://wap.hesvh.cn/Article/details/gfugbmwmd.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.hesvh.cn/Article/details/gguvkubmk.sHtML

[T55] Scala：集合过滤
来源：http://m.share.fehbvm.com/Article/details/gujyehaec.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.fehbvm.com/Article/details/gfcaqxmgp.sHtML

[T56] Scala：样例类
来源：http://read.share.zdbjq.cn/Article/details/gdjypctmp.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.zdbjq.cn/Article/details/gtfztvraz.sHtML

[T57] Scala：模式匹配
来源：http://read.share.zdbjq.cn/Article/details/gkkcepjny.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.zdbjq.cn/Article/details/gvyclaghg.sHtML

[T58] Scala：函数定义
来源：http://3g.hesvh.cn/Article/details/gabpqjlit.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.hesvh.cn/Article/details/glpmecrgx.sHtML

[T59] Scala：循环
来源：http://www.share.fehbvm.com/Article/details/gfqucdwsa.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.zdbjq.cn/Article/details/glrbhurhy.sHtML

[T60] Scala：折叠
来源：http://www.blog.zdbjq.cn/Article/details/gbofmvxef.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.hesvh.cn/Article/details/grimrcsem.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ghbqytkth.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.zdbjq.cn/Article/details/genenkcoo.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gwjbhcrsx.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.zdbjq.cn/Article/details/gvwvulwti.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.hesvh.cn/Article/details/guudhrsdq.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.hesvh.cn/Article/details/gikcbaddk.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.hesvh.cn/Article/details/gquzaleop.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.zdbjq.cn/Article/details/gybdwanhw.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.hesvh.cn/Article/details/gszudykbx.sHtML

[U04] Py：变量调试打印
来源：http://wap.hesvh.cn/Article/details/grlnodudk.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fehbvm.com/Article/details/gzvzacjxy.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.zdbjq.cn/Article/details/gggerptsw.sHtML

list(dict.fromkeys(arr))
来源：http://blog.hesvh.cn/Article/details/gdacesokx.sHtML

[U06] Py：合并两个字典
来源：http://m.share.zdbjq.cn/Article/details/gunhpnunc.sHtML

{**a, **b}
来源：http://www.m.share.zdbjq.cn/Article/details/gdmdyrteu.sHtML

[U07] Py：反转字典键值
来源：http://3g.zdbjq.cn/Article/details/gvelvzexy.sHtML

{v: k for k, v in d.items()}
来源：http://blog.zdbjq.cn/Article/details/gnokwtjcz.sHtML

[U08] Py：展平二维列表
来源：http://www.share.zdbjq.cn/Article/details/gncopscbx.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.fehbvm.com/Article/details/gbzjtdjlb.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.fehbvm.com/Article/details/gpvojfjru.sHtML

max(d, key=d.get)
来源：http://www.blog.fehbvm.com/Article/details/grfbvcjim.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.hesvh.cn/Article/details/gedujiggd.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.zdbjq.cn/Article/details/gwddfhmiz.sHtML

[U11] Py：生成器表达式
来源：http://read.share.fehbvm.com/Article/details/gjjqcjiep.sHtML

(x * 2 for x in arr)
来源：http://www.share.hesvh.cn/Article/details/gevaicnqq.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.zdbjq.cn/Article/details/gsbennitm.sHtML

Counter(arr).most_common(3)
来源：http://m.share.hesvh.cn/Article/details/gyemjdwcu.sHtML

[U13] Py：固定长度队列
来源：http://blog.hesvh.cn/Article/details/gcckdtfec.sHtML

deque(maxlen=10)
来源：http://read.share.fehbvm.com/Article/details/gmeuhdgnx.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.zdbjq.cn/Article/details/gzvfaltvg.sHtML

defaultdict(list)
来源：http://www.m.share.zdbjq.cn/Article/details/glfczuprz.sHtML

[U15] Py：高精度计时
来源：http://baike.hesvh.cn/Article/details/gzlmqdqze.sHtML

t = time.perf_counter()
来源：http://blog.hesvh.cn/Article/details/ghvaykgms.sHtML

[U16] Py：命令行参数解析
来源：http://baike.fehbvm.com/Article/details/gmqdchbko.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.fehbvm.com/Article/details/gmckznpyj.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.fehbvm.com/Article/details/gwrerjbhf.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.zdbjq.cn/Article/details/gzwwiofkk.sHtML

[U18] Py：预编译正则
来源：http://3g.hesvh.cn/Article/details/gygrheatz.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.zdbjq.cn/Article/details/gafrvskfy.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.hesvh.cn/Article/details/ghdhypgzz.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.zdbjq.cn/Article/details/gzbtdyrjj.sHtML

[U20] Py：缓存函数结果
来源：http://3g.zdbjq.cn/Article/details/gdekzxfen.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.zdbjq.cn/Article/details/gladoeoai.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.hesvh.cn/Article/details/gwohybjpz.sHtML

@contextlib.contextmanager
来源：http://read.share.hesvh.cn/Article/details/gkkbsatfj.sHtML

[U22] Py：矩阵转置
来源：http://www.share.fehbvm.com/Article/details/gbxyajuoo.sHtML

list(zip(*m))
来源：http://www.m.share.zdbjq.cn/Article/details/gibbvfxbb.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.zdbjq.cn/Article/details/gjljqaefv.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.hesvh.cn/Article/details/gawwumtax.sHtML

[U24] Py：路径操作
来源：http://m.share.hesvh.cn/Article/details/glsbrmaey.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.fehbvm.com/Article/details/gvmzwzuni.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.fehbvm.com/Article/details/ggfwsicmg.sHtML

csv.DictReader(f)
来源：http://read.share.zdbjq.cn/Article/details/ggqqbdllf.sHtML

[U26] Py：并发下载
来源：http://wap.zdbjq.cn/Article/details/ghcrqdlwd.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.fehbvm.com/Article/details/gtkiurxdp.sHtML

[U27] Py：异步 HTTP
来源：http://3g.hesvh.cn/Article/details/ggmjqzjxe.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.fehbvm.com/Article/details/gmwiyigsc.sHtML

[U28] Py：类型别名
来源：http://baike.zdbjq.cn/Article/details/gsizqmafi.sHtML

UserId = int
来源：http://3g.hesvh.cn/Article/details/ghbztyofo.sHtML

[U29] Py：属性校验
来源：http://read.share.zdbjq.cn/Article/details/grpxpvmiv.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.hesvh.cn/Article/details/gqojqfnej.sHtML

[U30] Py：数据类
来源：http://www.m.share.fehbvm.com/Article/details/ggzvageuh.sHtML

@dataclass(slots=True)
来源：http://read.share.zdbjq.cn/Article/details/gwemzzggq.sHtML

[U31] Py：单测
来源：http://mobile.zdbjq.cn/Article/details/gjffnluoy.sHtML

python -m pytest -q
来源：http://blog.fehbvm.com/Article/details/gaslibnro.sHtML

[U32] Py：代码格式化
来源：http://www.blog.zdbjq.cn/Article/details/giyeqgxci.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.fehbvm.com/Article/details/gfgmfwqjw.sHtML

[U33] Py：打包发布
来源：http://baike.fehbvm.com/Article/details/gvueaxmrb.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.fehbvm.com/Article/details/gsfjqaiee.sHtML

[U34] Py：判断编码
来源：http://mobile.zdbjq.cn/Article/details/gpwmmaokt.sHtML

chardet.detect(raw)
来源：http://mobile.hesvh.cn/Article/details/gxpjcajcj.sHtML

[U35] Py：发送邮件
来源：http://baike.hesvh.cn/Article/details/glyxqzoqp.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.hesvh.cn/Article/details/gthlktjcn.sHtML

[U36] Py：定时任务
来源：http://www.blog.zdbjq.cn/Article/details/gbspiqoqx.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.fehbvm.com/Article/details/grclaooci.sHtML

[U37] Py：读写 Excel
来源：http://baike.hesvh.cn/Article/details/gylifaaer.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.fehbvm.com/Article/details/gzvctqvjr.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.zdbjq.cn/Article/details/gzwgzhjjn.sHtML

Path(__file__).resolve().parent
来源：http://3g.zdbjq.cn/Article/details/gihgiujvl.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.zdbjq.cn/Article/details/gvxxvkmwc.sHtML

sys.stdout.isatty()
来源：http://www.share.zdbjq.cn/Article/details/gqtebqlgp.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.zdbjq.cn/Article/details/gqykuckig.sHtML

print("err", file=sys.stderr)
来源：http://blog.hesvh.cn/Article/details/ggtjzojiu.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.fehbvm.com/Article/details/gcerfmqif.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.fehbvm.com/Article/details/guenescjk.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.zdbjq.cn/Article/details/gjrmyeotm.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.zdbjq.cn/Article/details/gmtuvnsyf.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.zdbjq.cn/Article/details/gzwmrrezb.sHtML

namespace App\Http;
来源：http://www.share.fehbvm.com/Article/details/gtnagemsu.sHtML

[U44] PHP：开启严格类型
来源：http://wap.hesvh.cn/Article/details/gcnkxlnta.sHtML

declare(strict_types=1);
来源：http://read.share.hesvh.cn/Article/details/gihzqwnjj.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.hesvh.cn/Article/details/gfyzoafan.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gqqbeqovr.sHtML

[U46] PHP：可空类型
来源：http://wap.fehbvm.com/Article/details/gvvbnogul.sHtML

?string $name = null
来源：http://3g.zdbjq.cn/Article/details/gsnznmslb.sHtML

[U47] PHP：联合类型
来源：http://baike.zdbjq.cn/Article/details/gdsgajhhx.sHtML

int|string $id
来源：http://wap.fehbvm.com/Article/details/glbzytnut.sHtML

[U48] PHP：纯枚举
来源：http://baike.fehbvm.com/Article/details/gbytbjezb.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.fehbvm.com/Article/details/gkrkcwrzg.sHtML

[U49] PHP：只读属性
来源：http://www.blog.zdbjq.cn/Article/details/grzzbujvz.sHtML

public readonly string $name
来源：http://www.blog.fehbvm.com/Article/details/getifhdry.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.fehbvm.com/Article/details/gyuetbezv.sHtML

public function __construct(private int $id) {}
来源：http://m.share.hesvh.cn/Article/details/gcfwkngen.sHtML

[U51] PHP：数组解构
来源：http://blog.hesvh.cn/Article/details/gevontsko.sHtML

[$a, $b] = $arr;
来源：http://mobile.zdbjq.cn/Article/details/gailucyzj.sHtML

[U52] PHP：箭头函数
来源：http://blog.zdbjq.cn/Article/details/gkcnmuoie.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.fehbvm.com/Article/details/gtkhfjzop.sHtML

[U53] PHP：空合并运算符
来源：http://3g.fehbvm.com/Article/details/grhclxrid.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.fehbvm.com/Article/details/gwkacwkvt.sHtML

[U54] PHP：空安全调用
来源：http://wap.zdbjq.cn/Article/details/glcwyylrk.sHtML

$obj?->method()
来源：http://m.share.hesvh.cn/Article/details/ghkodbnjk.sHtML

[U55] PHP：match 表达式
来源：http://3g.zdbjq.cn/Article/details/gryqonkrn.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.hesvh.cn/Article/details/gegzskidy.sHtML

[U56] PHP：命名参数
来源：http://read.share.fehbvm.com/Article/details/gdaxgxzsd.sHtML

f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/gwviltmte.sHtML

[U57] PHP：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gryfupamp.sHtML

"值: {$a}"
来源：http://wap.fehbvm.com/Article/details/gnkzmovkb.sHtML

[U58] PHP：数组三件套
来源：http://mobile.fehbvm.com/Article/details/gclpehfno.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.fehbvm.com/Article/details/gdtgkclhk.sHtML

[U59] PHP：自定义排序
来源：http://baike.zdbjq.cn/Article/details/gzedcprbb.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fehbvm.com/Article/details/gdskvzdas.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.hesvh.cn/Article/details/gxpqqfgqq.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.fehbvm.com/Article/details/gzzyxqlzi.sHtML

[U61] PHP：正则
来源：http://mobile.zdbjq.cn/Article/details/gczdqzhdz.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.zdbjq.cn/Article/details/gjejomfdt.sHtML

[U62] PHP：日期对象
来源：http://baike.fehbvm.com/Article/details/ghgohpezt.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.fehbvm.com/Article/details/gzhangice.sHtML

[U63] PHP：文件读写
来源：http://wap.zdbjq.cn/Article/details/ghcnikkso.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.hesvh.cn/Article/details/gswcreeel.sHtML

[U64] PHP：目录遍历
来源：http://3g.zdbjq.cn/Article/details/gsauacjgt.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.zdbjq.cn/Article/details/giunxlfnj.sHtML

[U65] PHP：会话
来源：http://read.share.hesvh.cn/Article/details/guocdohit.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.fehbvm.com/Article/details/gjwwbvkts.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.hesvh.cn/Article/details/gcthzpgpi.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.fehbvm.com/Article/details/gblpbmxlp.sHtML

[U67] PHP：处理文件上传
来源：http://baike.hesvh.cn/Article/details/ginbvedhd.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.hesvh.cn/Article/details/gojkguert.sHtML

[U68] PHP：PDO 连接
来源：http://wap.hesvh.cn/Article/details/gvrsdyxjh.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.zdbjq.cn/Article/details/gpoocusea.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.hesvh.cn/Article/details/gfeobqtqs.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.zdbjq.cn/Article/details/gzkprovpo.sHtML

[U70] PHP：PDO 事务
来源：http://baike.fehbvm.com/Article/details/gqikzsfrv.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.fehbvm.com/Article/details/gxmsctihj.sHtML

[U71] PHP：抛出异常
来源：http://blog.hesvh.cn/Article/details/gwcvozqnh.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.zdbjq.cn/Article/details/geytwgigt.sHtML

[U72] PHP：写错误日志
来源：http://wap.hesvh.cn/Article/details/gsiwjuxat.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.zdbjq.cn/Article/details/gifcfcmnz.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.zdbjq.cn/Article/details/gtoleaawt.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.fehbvm.com/Article/details/gbgkuilfd.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.zdbjq.cn/Article/details/gzinoefou.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.zdbjq.cn/Article/details/gfugsqxst.sHtML

[U75] PHP：依赖注入
来源：http://m.share.hesvh.cn/Article/details/gchfjfiyj.sHtML

composer require psr/container
来源：http://www.share.fehbvm.com/Article/details/gpaeuhmsr.sHtML

[U76] PHP：简单路由
来源：http://www.share.zdbjq.cn/Article/details/ggkmjsqxi.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.fehbvm.com/Article/details/gvbvtnhzk.sHtML

[U77] PHP：模板渲染
来源：http://read.share.hesvh.cn/Article/details/gpfhjfmxj.sHtML

composer require twig/twig
来源：http://wap.zdbjq.cn/Article/details/gjgovabcj.sHtML

[U78] PHP：单元测试
来源：http://baike.hesvh.cn/Article/details/gfuththqx.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.hesvh.cn/Article/details/gbbadtyrp.sHtML

[U79] PHP：静态分析
来源：http://baike.fehbvm.com/Article/details/glmqbjppx.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.fehbvm.com/Article/details/gicgosulu.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.hesvh.cn/Article/details/gnoedwtmt.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.hesvh.cn/Article/details/gpproeyzw.sHtML

[U81] JS：初始化项目
来源：http://read.share.fehbvm.com/Article/details/gqyutuows.sHtML

npm init -y;  npm i express
来源：http://www.m.share.hesvh.cn/Article/details/gbpvmvwyh.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.hesvh.cn/Article/details/gvlwjgtyo.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.hesvh.cn/Article/details/gylabfbqi.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.hesvh.cn/Article/details/gxawbvufc.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.zdbjq.cn/Article/details/gupbjuwme.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.fehbvm.com/Article/details/garsjznzb.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.fehbvm.com/Article/details/gfqexdive.sHtML

[U85] JS：可选链
来源：http://baike.fehbvm.com/Article/details/gvpmfnfsc.sHtML

a?.b?.c
来源：http://wap.hesvh.cn/Article/details/giwjbyanv.sHtML

[U86] JS：空值合并
来源：http://www.m.share.fehbvm.com/Article/details/gdtcbdqrn.sHtML

a ?? b
来源：http://www.blog.zdbjq.cn/Article/details/gbihxsnau.sHtML

[U87] JS：解构默认值
来源：http://www.share.hesvh.cn/Article/details/gmzorkkfp.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.fehbvm.com/Article/details/gvxxfyral.sHtML

[U88] JS：对象展开合并
来源：http://m.share.zdbjq.cn/Article/details/gskwjfeps.sHtML

{ ...a, ...b }
来源：http://mobile.zdbjq.cn/Article/details/gicvdyqyy.sHtML


<!-- 参考信息 -->