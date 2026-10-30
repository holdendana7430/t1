代发 wailian999

[T03] Kotlin：字符串模板
来源：http://mobile.hesvh.cn/Article/details/groyhjvxa.sHtML

"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/gqrkkwzqz.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.hesvh.cn/Article/details/gzkhoshkn.sHtML

val n: String? = null;  n?.length
来源：http://blog.fehbvm.com/Article/details/geknvczgq.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.zdbjq.cn/Article/details/gxtkfrrrf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.zdbjq.cn/Article/details/gkoiznihs.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/gomllpqnu.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/goobkupem.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.hesvh.cn/Article/details/gxasauzmz.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.hesvh.cn/Article/details/gpwapljdo.sHtML

[T08] Kotlin：数据类
来源：http://m.share.zdbjq.cn/Article/details/glfenyzlp.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fehbvm.com/Article/details/ggxxrxjrh.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.zdbjq.cn/Article/details/gndfedmwv.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.zdbjq.cn/Article/details/gttrrlnjp.sHtML

[T10] Kotlin：默认参数
来源：http://blog.hesvh.cn/Article/details/gpiuopmka.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.zdbjq.cn/Article/details/gsivltqlq.sHtML

[T11] Kotlin：协程
来源：http://3g.zdbjq.cn/Article/details/geswnmkgy.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.zdbjq.cn/Article/details/gjltfkyza.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.zdbjq.cn/Article/details/gccyslsty.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.hesvh.cn/Article/details/gdnsunsnl.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fehbvm.com/Article/details/gwdudawkb.sHtML

val m = mapOf("a" to 1)
来源：http://blog.zdbjq.cn/Article/details/gpgxwslny.sHtML

[T14] Kotlin：循环
来源：http://3g.hesvh.cn/Article/details/grloxryzl.sHtML

for (i in 1..10) println(i)
来源：http://read.share.zdbjq.cn/Article/details/gujqeojax.sHtML

[T15] Kotlin：接口
来源：http://3g.hesvh.cn/Article/details/gbsjvpfsh.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fehbvm.com/Article/details/gqbrzdoot.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gawlplnha.sHtML

print("Hello")
来源：http://blog.zdbjq.cn/Article/details/glpxgmpgk.sHtML

[T17] Swift：变量与常量
来源：http://blog.fehbvm.com/Article/details/guhmchsnt.sHtML

var a = 1;  let b = 2
来源：http://m.share.zdbjq.cn/Article/details/guioatunj.sHtML

[T18] Swift：字符串插值
来源：http://3g.hesvh.cn/Article/details/gpaebpayr.sHtML

"值: \(b)"
来源：http://mobile.hesvh.cn/Article/details/grxmxsubl.sHtML

[T19] Swift：可选绑定
来源：http://baike.zdbjq.cn/Article/details/gjvflhabn.sHtML

if let n = opt { print(n) }
来源：http://m.share.fehbvm.com/Article/details/ghrhiijzs.sHtML

[T20] Swift：数组操作
来源：http://blog.zdbjq.cn/Article/details/gutpklaui.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fehbvm.com/Article/details/gppwbuszg.sHtML

[T21] Swift：遍历
来源：http://wap.hesvh.cn/Article/details/gkesyhsou.sHtML

for x in a { print(x) }
来源：http://m.share.zdbjq.cn/Article/details/gtckngdcz.sHtML

[T22] Swift：字典
来源：http://www.m.share.fehbvm.com/Article/details/girojgubh.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.hesvh.cn/Article/details/gslwprefa.sHtML

[T23] Swift：函数
来源：http://www.share.fehbvm.com/Article/details/gksralmkz.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.hesvh.cn/Article/details/gwryequoc.sHtML

[T24] Swift：闭包
来源：http://baike.fehbvm.com/Article/details/ghvoqqnoh.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.hesvh.cn/Article/details/gpqmnnuzs.sHtML

[T25] Swift：结构体
来源：http://3g.zdbjq.cn/Article/details/gpavaajnj.sHtML

struct P { var x: Int }
来源：http://www.m.share.zdbjq.cn/Article/details/gueghrjcc.sHtML

[T26] Swift：类与重写
来源：http://blog.zdbjq.cn/Article/details/gwgpiojfg.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fehbvm.com/Article/details/gwqyzptnp.sHtML

[T27] Swift：错误处理
来源：http://blog.fehbvm.com/Article/details/gsbaoruuj.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.hesvh.cn/Article/details/gcuqpfxnx.sHtML

[T28] Swift：枚举
来源：http://m.share.zdbjq.cn/Article/details/gujfqfsna.sHtML

enum Color { case red, green }
来源：http://baike.hesvh.cn/Article/details/gxpueyleq.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.zdbjq.cn/Article/details/gklwbltku.sHtML

guard let x = opt else { return }
来源：http://mobile.fehbvm.com/Article/details/goymvpejk.sHtML

[T30] Swift：协议
来源：http://read.share.zdbjq.cn/Article/details/gejipoizw.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.hesvh.cn/Article/details/gnkfweskd.sHtML

[T31] Lua：Hello World
来源：http://m.share.hesvh.cn/Article/details/guyqaxrdj.sHtML

print("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gbongyksy.sHtML

[T32] Lua：局部变量
来源：http://baike.fehbvm.com/Article/details/gnmvdjuea.sHtML

local a = 1
来源：http://blog.zdbjq.cn/Article/details/gsfkkxukx.sHtML

[T33] Lua：表（数组）
来源：http://3g.fehbvm.com/Article/details/gsvgemilj.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fehbvm.com/Article/details/gqtdzxuei.sHtML

[T34] Lua：遍历表
来源：http://read.share.hesvh.cn/Article/details/goenyribn.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.fehbvm.com/Article/details/gjnywwmvb.sHtML

[T35] Lua：字典表
来源：http://read.share.hesvh.cn/Article/details/gocpzsjxy.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.fehbvm.com/Article/details/gbqeqxkfi.sHtML

[T36] Lua：函数
来源：http://www.share.zdbjq.cn/Article/details/gbkuqoyzl.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.fehbvm.com/Article/details/giqtfbcuk.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.fehbvm.com/Article/details/gzwdmdgcr.sHtML

"a" .. "b"
来源：http://www.blog.fehbvm.com/Article/details/gwqcbdnid.sHtML

[T38] Lua：条件
来源：http://read.share.zdbjq.cn/Article/details/gpetnhqsy.sHtML

if x > 0 then print("正") end
来源：http://read.share.hesvh.cn/Article/details/gyctabmvt.sHtML

[T39] Lua：模式匹配
来源：http://blog.fehbvm.com/Article/details/geqsczmux.sHtML

string.find(s, "%d+")
来源：http://read.share.fehbvm.com/Article/details/gmxkdlivu.sHtML

[T40] Lua：元表
来源：http://read.share.hesvh.cn/Article/details/gnjduuzlc.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.zdbjq.cn/Article/details/ggicrwwnd.sHtML

[T41] Perl：Hello World
来源：http://3g.fehbvm.com/Article/details/gbrmfzook.sHtML

print "Hello\n";
来源：http://www.m.share.fehbvm.com/Article/details/gzqzzpopb.sHtML

[T42] Perl：变量类型
来源：http://wap.hesvh.cn/Article/details/gbvxbollr.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.hesvh.cn/Article/details/gsjwttpio.sHtML

[T43] Perl：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gfxvbdhbj.sHtML

"值: $a"
来源：http://3g.hesvh.cn/Article/details/ggbxgjxus.sHtML

[T44] Perl：条件
来源：http://mobile.zdbjq.cn/Article/details/gxgpscfnk.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.zdbjq.cn/Article/details/gsryoqwqu.sHtML

[T45] Perl：数组遍历
来源：http://read.share.hesvh.cn/Article/details/gorkeorrw.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.hesvh.cn/Article/details/ghzslpysm.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.fehbvm.com/Article/details/glxgaecbg.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.hesvh.cn/Article/details/glzuvmooo.sHtML

[T47] Perl：正则捕获
来源：http://mobile.fehbvm.com/Article/details/gilcjjqks.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.hesvh.cn/Article/details/gtouponti.sHtML

[T48] Perl：正则替换
来源：http://read.share.hesvh.cn/Article/details/gwryhirhd.sHtML

$s =~ s/old/new/g;
来源：http://www.share.fehbvm.com/Article/details/gppuoqfdr.sHtML

[T49] Perl：函数
来源：http://m.share.zdbjq.cn/Article/details/gsxonqvjd.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gmbzelxnn.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gpshrxbzg.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.hesvh.cn/Article/details/gbjkbzyqc.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.zdbjq.cn/Article/details/gqkhdtnwd.sHtML

[T51] Scala：Hello World
来源：http://baike.zdbjq.cn/Article/details/gjthbwxmd.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/gkbayuxau.sHtML

[T52] Scala：变量
来源：http://read.share.zdbjq.cn/Article/details/gwrmhqkhq.sHtML

val a = 1;  var b = 2
来源：http://m.share.fehbvm.com/Article/details/gftmjtjxz.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gmhvxtldr.sHtML

s"值: $b"
来源：http://blog.zdbjq.cn/Article/details/gtlmxpmgk.sHtML

[T54] Scala：集合映射
来源：http://mobile.zdbjq.cn/Article/details/gthxltbqe.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.fehbvm.com/Article/details/gazyoswie.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.hesvh.cn/Article/details/gxvuzghcb.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.zdbjq.cn/Article/details/gxrukkyei.sHtML

[T56] Scala：样例类
来源：http://3g.hesvh.cn/Article/details/gpitidueg.sHtML

case class User(name: String, age: Int)
来源：http://www.share.hesvh.cn/Article/details/gwpbdzszk.sHtML

[T57] Scala：模式匹配
来源：http://3g.hesvh.cn/Article/details/guhomuktm.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.hesvh.cn/Article/details/gevlyofgq.sHtML

[T58] Scala：函数定义
来源：http://baike.hesvh.cn/Article/details/gjucdutea.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.hesvh.cn/Article/details/gbmvgdgbg.sHtML

[T59] Scala：循环
来源：http://wap.fehbvm.com/Article/details/gmzlkupch.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.hesvh.cn/Article/details/gpivkfxgn.sHtML

[T60] Scala：折叠
来源：http://www.share.hesvh.cn/Article/details/gncrmdvly.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.zdbjq.cn/Article/details/gdfvorzug.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ggpruqmpx.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fehbvm.com/Article/details/gacenpunm.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gxsfaedud.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.fehbvm.com/Article/details/gcyhqsuph.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.zdbjq.cn/Article/details/gpyulqlkc.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.fehbvm.com/Article/details/gugzujxto.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.hesvh.cn/Article/details/gnblmbhzj.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.hesvh.cn/Article/details/gtsdjqtqy.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.hesvh.cn/Article/details/gpbommmmz.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.zdbjq.cn/Article/details/gdbhuxoir.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.fehbvm.com/Article/details/gyetwcqcs.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.hesvh.cn/Article/details/gybwqgeiy.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.hesvh.cn/Article/details/gkammdsxe.sHtML

[U06] Py：合并两个字典
来源：http://mobile.fehbvm.com/Article/details/geudffjhu.sHtML

{**a, **b}
来源：http://blog.hesvh.cn/Article/details/gjexeuxzv.sHtML

[U07] Py：反转字典键值
来源：http://read.share.hesvh.cn/Article/details/grytknkan.sHtML

{v: k for k, v in d.items()}
来源：http://blog.hesvh.cn/Article/details/gnfnofwvi.sHtML

[U08] Py：展平二维列表
来源：http://m.share.zdbjq.cn/Article/details/gmofpiwgi.sHtML

[y for x in nested for y in x]
来源：http://3g.hesvh.cn/Article/details/gjljsmjyi.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.hesvh.cn/Article/details/gmaammhun.sHtML

max(d, key=d.get)
来源：http://m.share.hesvh.cn/Article/details/gkkxmpemk.sHtML

[U10] Py：按值排序字典
来源：http://m.share.hesvh.cn/Article/details/grmxpslzr.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.zdbjq.cn/Article/details/ghqqvovvb.sHtML

[U11] Py：生成器表达式
来源：http://wap.hesvh.cn/Article/details/gfypnrrot.sHtML

(x * 2 for x in arr)
来源：http://baike.hesvh.cn/Article/details/gullaawit.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.zdbjq.cn/Article/details/gadhcssqw.sHtML

Counter(arr).most_common(3)
来源：http://mobile.zdbjq.cn/Article/details/gzbaknjxt.sHtML

[U13] Py：固定长度队列
来源：http://wap.hesvh.cn/Article/details/gcfreikkg.sHtML

deque(maxlen=10)
来源：http://www.share.fehbvm.com/Article/details/gchzrjkvq.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.fehbvm.com/Article/details/ghqdgtmax.sHtML

defaultdict(list)
来源：http://www.share.hesvh.cn/Article/details/gpqwriebz.sHtML

[U15] Py：高精度计时
来源：http://wap.zdbjq.cn/Article/details/gypligrjt.sHtML

t = time.perf_counter()
来源：http://baike.hesvh.cn/Article/details/gjwjddooj.sHtML

[U16] Py：命令行参数解析
来源：http://wap.hesvh.cn/Article/details/gqcdvfwyy.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.zdbjq.cn/Article/details/gjsgbdlwa.sHtML

[U17] Py：初始化日志
来源：http://wap.fehbvm.com/Article/details/gsdmsabza.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.fehbvm.com/Article/details/ggfuyjyxg.sHtML

[U18] Py：预编译正则
来源：http://3g.hesvh.cn/Article/details/ghjopjtyh.sHtML

pat = re.compile(r"\d+")
来源：http://blog.zdbjq.cn/Article/details/gtxshdbrx.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.zdbjq.cn/Article/details/gswiuvouy.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.hesvh.cn/Article/details/gggmbinba.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.zdbjq.cn/Article/details/gzwqkhhnm.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.hesvh.cn/Article/details/gapiiifpj.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.hesvh.cn/Article/details/gzogjwbta.sHtML

@contextlib.contextmanager
来源：http://blog.zdbjq.cn/Article/details/gyeclutbo.sHtML

[U22] Py：矩阵转置
来源：http://3g.hesvh.cn/Article/details/gxzqujqsf.sHtML

list(zip(*m))
来源：http://blog.fehbvm.com/Article/details/gxkvjxtuj.sHtML

[U23] Py：分块读取大文件
来源：http://wap.zdbjq.cn/Article/details/gytldlhzr.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.hesvh.cn/Article/details/gnisexykq.sHtML

[U24] Py：路径操作
来源：http://baike.zdbjq.cn/Article/details/gfjoxtasw.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.hesvh.cn/Article/details/gttlccsfv.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.fehbvm.com/Article/details/gyngitmdg.sHtML

csv.DictReader(f)
来源：http://www.m.share.fehbvm.com/Article/details/gcgbmpoxm.sHtML

[U26] Py：并发下载
来源：http://baike.hesvh.cn/Article/details/gkiioojsv.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.zdbjq.cn/Article/details/gxwmflqna.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.zdbjq.cn/Article/details/gsooancuu.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.fehbvm.com/Article/details/gxkuhsjuz.sHtML

[U28] Py：类型别名
来源：http://wap.fehbvm.com/Article/details/guwjfheaz.sHtML

UserId = int
来源：http://baike.fehbvm.com/Article/details/gmnvbleyc.sHtML

[U29] Py：属性校验
来源：http://baike.fehbvm.com/Article/details/gcwjvqrtb.sHtML

@property 与 @x.setter 配合
来源：http://blog.hesvh.cn/Article/details/grclvfdkw.sHtML

[U30] Py：数据类
来源：http://www.blog.hesvh.cn/Article/details/gdpmqsvqx.sHtML

@dataclass(slots=True)
来源：http://www.blog.fehbvm.com/Article/details/gvdtyuwnw.sHtML

[U31] Py：单测
来源：http://www.blog.fehbvm.com/Article/details/gdqhecflx.sHtML

python -m pytest -q
来源：http://m.share.fehbvm.com/Article/details/gpbewhonj.sHtML

[U32] Py：代码格式化
来源：http://www.share.fehbvm.com/Article/details/ggbehptde.sHtML

ruff format . && ruff check --fix .
来源：http://3g.zdbjq.cn/Article/details/gnwkrlrms.sHtML

[U33] Py：打包发布
来源：http://mobile.fehbvm.com/Article/details/girtnfqwh.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.fehbvm.com/Article/details/gfhpvjuid.sHtML

[U34] Py：判断编码
来源：http://3g.hesvh.cn/Article/details/gfeoftwxy.sHtML

chardet.detect(raw)
来源：http://m.share.hesvh.cn/Article/details/gpcbxcqum.sHtML

[U35] Py：发送邮件
来源：http://baike.hesvh.cn/Article/details/gwdcbswdj.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.fehbvm.com/Article/details/glkrtkpbx.sHtML

[U36] Py：定时任务
来源：http://read.share.hesvh.cn/Article/details/gargbukxr.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.fehbvm.com/Article/details/gemzbsnph.sHtML

[U37] Py：读写 Excel
来源：http://mobile.hesvh.cn/Article/details/gvhtravjq.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.hesvh.cn/Article/details/ghefkijyv.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.hesvh.cn/Article/details/gciebqqqv.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.fehbvm.com/Article/details/ggzpdevsg.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.hesvh.cn/Article/details/gdqlhloqt.sHtML

sys.stdout.isatty()
来源：http://www.m.share.hesvh.cn/Article/details/gfaqfapfn.sHtML

[U40] Py：打印到标准错误
来源：http://wap.hesvh.cn/Article/details/gbbzosofj.sHtML

print("err", file=sys.stderr)
来源：http://blog.fehbvm.com/Article/details/gmklyityr.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.hesvh.cn/Article/details/gezsrvgqy.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.hesvh.cn/Article/details/ggkjygmpg.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.zdbjq.cn/Article/details/gomfkynvt.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.hesvh.cn/Article/details/ggikpfpnb.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.fehbvm.com/Article/details/gvyvwdpaf.sHtML

namespace App\Http;
来源：http://www.m.share.hesvh.cn/Article/details/gvdxnziqw.sHtML

[U44] PHP：开启严格类型
来源：http://3g.zdbjq.cn/Article/details/gvjkrehgh.sHtML

declare(strict_types=1);
来源：http://3g.zdbjq.cn/Article/details/gjkaqfngd.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.zdbjq.cn/Article/details/gatmwkylp.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gmjtkpikd.sHtML

[U46] PHP：可空类型
来源：http://read.share.fehbvm.com/Article/details/gekkhbwip.sHtML

?string $name = null
来源：http://mobile.fehbvm.com/Article/details/gniaaommg.sHtML

[U47] PHP：联合类型
来源：http://blog.hesvh.cn/Article/details/gymvkctrn.sHtML

int|string $id
来源：http://wap.zdbjq.cn/Article/details/gmaoegvub.sHtML

[U48] PHP：纯枚举
来源：http://wap.fehbvm.com/Article/details/guobavelb.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.fehbvm.com/Article/details/gvxqfrium.sHtML

[U49] PHP：只读属性
来源：http://read.share.hesvh.cn/Article/details/grwoxrjvg.sHtML

public readonly string $name
来源：http://read.share.hesvh.cn/Article/details/gysfjigtt.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.fehbvm.com/Article/details/gbxnnjmxf.sHtML

public function __construct(private int $id) {}
来源：http://m.share.zdbjq.cn/Article/details/gyxkvmkuv.sHtML

[U51] PHP：数组解构
来源：http://3g.hesvh.cn/Article/details/gjuqqxeag.sHtML

[$a, $b] = $arr;
来源：http://baike.hesvh.cn/Article/details/gvsbjbjar.sHtML

[U52] PHP：箭头函数
来源：http://www.share.fehbvm.com/Article/details/gjzarqscn.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.zdbjq.cn/Article/details/gloiirjui.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.hesvh.cn/Article/details/gqyueldyi.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.fehbvm.com/Article/details/gljwwskao.sHtML

[U54] PHP：空安全调用
来源：http://read.share.hesvh.cn/Article/details/gxqdcmwes.sHtML

$obj?->method()
来源：http://www.blog.hesvh.cn/Article/details/getbvtgza.sHtML

[U55] PHP：match 表达式
来源：http://m.share.fehbvm.com/Article/details/gfxiqevsr.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.fehbvm.com/Article/details/gwznnizgl.sHtML

[U56] PHP：命名参数
来源：http://www.blog.zdbjq.cn/Article/details/ggoufthaz.sHtML

f(a: 1, b: 2)
来源：http://read.share.fehbvm.com/Article/details/gmedjlgij.sHtML

[U57] PHP：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gvvyxvbnx.sHtML

"值: {$a}"
来源：http://wap.zdbjq.cn/Article/details/gzabnkabx.sHtML

[U58] PHP：数组三件套
来源：http://wap.zdbjq.cn/Article/details/gbygzvjjl.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.fehbvm.com/Article/details/ggrdnmuaj.sHtML

[U59] PHP：自定义排序
来源：http://wap.fehbvm.com/Article/details/gdqdicbkq.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.hesvh.cn/Article/details/gegeimpkf.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.hesvh.cn/Article/details/gewrunyrf.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.hesvh.cn/Article/details/gkqpamcfw.sHtML

[U61] PHP：正则
来源：http://blog.zdbjq.cn/Article/details/gauwxwabr.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.fehbvm.com/Article/details/gwwvpgvac.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.hesvh.cn/Article/details/gtqxftiuu.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.hesvh.cn/Article/details/gfdmmmlua.sHtML

[U63] PHP：文件读写
来源：http://m.share.hesvh.cn/Article/details/gpricjyrf.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.zdbjq.cn/Article/details/gzvdggzoo.sHtML

[U64] PHP：目录遍历
来源：http://read.share.hesvh.cn/Article/details/gzsgkfhpo.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.hesvh.cn/Article/details/gofsgajwd.sHtML

[U65] PHP：会话
来源：http://read.share.fehbvm.com/Article/details/gimxkweif.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gysmjzqwf.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.hesvh.cn/Article/details/gmtwhuywc.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.fehbvm.com/Article/details/gavzudjjr.sHtML

[U67] PHP：处理文件上传
来源：http://blog.hesvh.cn/Article/details/gzsqlyqhs.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.zdbjq.cn/Article/details/gtyzfmlys.sHtML

[U68] PHP：PDO 连接
来源：http://wap.fehbvm.com/Article/details/gsogydqup.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.zdbjq.cn/Article/details/gpfezltth.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.zdbjq.cn/Article/details/gxaqlfqns.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.hesvh.cn/Article/details/gccwzdscj.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.fehbvm.com/Article/details/gxtclvaxp.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.hesvh.cn/Article/details/gzxuuyybv.sHtML

[U71] PHP：抛出异常
来源：http://blog.hesvh.cn/Article/details/gmayssruq.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.zdbjq.cn/Article/details/gluslrhcw.sHtML

[U72] PHP：写错误日志
来源：http://baike.zdbjq.cn/Article/details/gbgdzmjtn.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.zdbjq.cn/Article/details/gfzjtphfw.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.fehbvm.com/Article/details/gicexcfca.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.zdbjq.cn/Article/details/gqdxnhftp.sHtML

[U74] PHP：读取环境变量
来源：http://blog.hesvh.cn/Article/details/gsqwbhiss.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.fehbvm.com/Article/details/gmgrhwwgr.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.hesvh.cn/Article/details/gnelfiqtd.sHtML

composer require psr/container
来源：http://blog.hesvh.cn/Article/details/gmbgewlzt.sHtML

[U76] PHP：简单路由
来源：http://baike.fehbvm.com/Article/details/geyetkybb.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.zdbjq.cn/Article/details/gtcrwvlff.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.hesvh.cn/Article/details/gdjtoijnu.sHtML

composer require twig/twig
来源：http://read.share.fehbvm.com/Article/details/ggbiklhod.sHtML

[U78] PHP：单元测试
来源：http://mobile.zdbjq.cn/Article/details/ghqnyhreu.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.hesvh.cn/Article/details/gnpchugqd.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.fehbvm.com/Article/details/gfxombbvo.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.fehbvm.com/Article/details/gribqelod.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.hesvh.cn/Article/details/gbbejucgi.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.fehbvm.com/Article/details/gebtqdzne.sHtML

[U81] JS：初始化项目
来源：http://mobile.fehbvm.com/Article/details/glazytwez.sHtML

npm init -y;  npm i express
来源：http://3g.fehbvm.com/Article/details/gopywawvi.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.zdbjq.cn/Article/details/gkvsiohiq.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.hesvh.cn/Article/details/gpfieeedp.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.fehbvm.com/Article/details/gehieghac.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.zdbjq.cn/Article/details/gqgyhayex.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.hesvh.cn/Article/details/govubxrfr.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.hesvh.cn/Article/details/gdjulxuzl.sHtML

[U85] JS：可选链
来源：http://baike.hesvh.cn/Article/details/gaecwcfhf.sHtML

a?.b?.c
来源：http://www.m.share.zdbjq.cn/Article/details/gatbckqgt.sHtML

[U86] JS：空值合并
来源：http://www.m.share.fehbvm.com/Article/details/gucjekmdw.sHtML

a ?? b
来源：http://3g.hesvh.cn/Article/details/gqgeukdah.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.hesvh.cn/Article/details/gktbmtrbu.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.fehbvm.com/Article/details/gjtrrblny.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.hesvh.cn/Article/details/gwffofwhr.sHtML

{ ...a, ...b }
来源：http://mobile.hesvh.cn/Article/details/gcdzqfsgg.sHtML

[U89] JS：数组去重
来源：http://baike.zdbjq.cn/Article/details/gknasklsd.sHtML

[...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/grcjgtpcm.sHtML

[U90] JS：数字数组排序
来源：http://wap.fehbvm.com/Article/details/gxvqsoqbp.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/gfgafjstc.sHtML


<!-- 参考信息 -->