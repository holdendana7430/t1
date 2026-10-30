代发 wailian999

[T03] Kotlin：字符串模板
来源：http://baike.fanxiaobao.xyz/Article/details/ggnqduoki.sHtML

"值: $b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gnzpzgltj.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzvyifjmx.sHtML

val n: String? = null;  n?.length
来源：http://3g.fanxiaobao.xyz/Article/details/gutuyunsi.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gtjkfmhxr.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpmokfjgm.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fanxiaobao.xyz/Article/details/gljurhfxr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gnlltrkzb.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fanxiaobao.xyz/Article/details/girtnqjsp.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fanxiaobao.xyz/Article/details/gbccpkaca.sHtML

[T08] Kotlin：数据类
来源：http://blog.fanxiaobao.xyz/Article/details/gdjmeeqbj.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fanxiaobao.xyz/Article/details/gnequiyzd.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fanxiaobao.xyz/Article/details/gsgeebaeq.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fanxiaobao.xyz/Article/details/glmdhodow.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsccucgqb.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fanxiaobao.xyz/Article/details/ghavrxsus.sHtML

[T11] Kotlin：协程
来源：http://read.share.fanxiaobao.xyz/Article/details/ghtadwjuz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjkisqchf.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fanxiaobao.xyz/Article/details/gbjppyiew.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbeacfgdz.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwmmvjchm.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gonfwcawm.sHtML

[T14] Kotlin：循环
来源：http://blog.fanxiaobao.xyz/Article/details/gnmuswzsy.sHtML

for (i in 1..10) println(i)
来源：http://3g.fanxiaobao.xyz/Article/details/gcnsewuun.sHtML

[T15] Kotlin：接口
来源：http://wap.fanxiaobao.xyz/Article/details/gffftueea.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fanxiaobao.xyz/Article/details/gjemgpbsn.sHtML

[T16] Swift：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gwvfxoyut.sHtML

print("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/geqimxehu.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gfakcnogl.sHtML

var a = 1;  let b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gpdpaplkw.sHtML

[T18] Swift：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gmhdmxezi.sHtML

"值: \(b)"
来源：http://read.share.fanxiaobao.xyz/Article/details/gacaeursw.sHtML

[T19] Swift：可选绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gzwjkkgqf.sHtML

if let n = opt { print(n) }
来源：http://baike.fanxiaobao.xyz/Article/details/gfqrvwnjy.sHtML

[T20] Swift：数组操作
来源：http://3g.fanxiaobao.xyz/Article/details/gfmtgvflz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fanxiaobao.xyz/Article/details/gajijeuvn.sHtML

[T21] Swift：遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gdzyuuqiu.sHtML

for x in a { print(x) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gefernhpz.sHtML

[T22] Swift：字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gxzwejmtq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/ggxsjclfa.sHtML

[T23] Swift：函数
来源：http://3g.fanxiaobao.xyz/Article/details/geqqhvrzo.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gonlxzkvg.sHtML

[T24] Swift：闭包
来源：http://baike.fanxiaobao.xyz/Article/details/geoxwdvru.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsimqxxdq.sHtML

[T25] Swift：结构体
来源：http://www.share.fanxiaobao.xyz/Article/details/glzjwcugs.sHtML

struct P { var x: Int }
来源：http://read.share.fanxiaobao.xyz/Article/details/grqwqmkxb.sHtML

[T26] Swift：类与重写
来源：http://baike.fanxiaobao.xyz/Article/details/goydanzwm.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fanxiaobao.xyz/Article/details/guylxmakb.sHtML

[T27] Swift：错误处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gjeoyuhru.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gakpcmkcf.sHtML

[T28] Swift：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gujcuazzg.sHtML

enum Color { case red, green }
来源：http://blog.fanxiaobao.xyz/Article/details/gnvdefviy.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fanxiaobao.xyz/Article/details/gnyakegkk.sHtML

guard let x = opt else { return }
来源：http://blog.fanxiaobao.xyz/Article/details/gthwskvmd.sHtML

[T30] Swift：协议
来源：http://baike.fanxiaobao.xyz/Article/details/ggjnmqzht.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.fanxiaobao.xyz/Article/details/gqwtcdcyu.sHtML

[T31] Lua：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gzfmgoduz.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxnmizpzj.sHtML

[T32] Lua：局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gndduubga.sHtML

local a = 1
来源：http://www.share.fanxiaobao.xyz/Article/details/gusycxeuo.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcytvtgzh.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fanxiaobao.xyz/Article/details/ggseuqpms.sHtML

[T34] Lua：遍历表
来源：http://wap.fanxiaobao.xyz/Article/details/gavqtkcdj.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.fanxiaobao.xyz/Article/details/gtbbaqdsb.sHtML

[T35] Lua：字典表
来源：http://m.share.fanxiaobao.xyz/Article/details/gmbrkfmwu.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmlpsqstt.sHtML

[T36] Lua：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gvfvapcha.sHtML

function add(a, b) return a + b end
来源：http://www.blog.fanxiaobao.xyz/Article/details/grcaadqxi.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grcfjwsjk.sHtML

"a" .. "b"
来源：http://baike.fanxiaobao.xyz/Article/details/gujlftbek.sHtML

[T38] Lua：条件
来源：http://wap.fanxiaobao.xyz/Article/details/giudvhfqi.sHtML

if x > 0 then print("正") end
来源：http://read.share.fanxiaobao.xyz/Article/details/gvlkeqbrb.sHtML

[T39] Lua：模式匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gkntzwakc.sHtML

string.find(s, "%d+")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gofdxqour.sHtML

[T40] Lua：元表
来源：http://read.share.fanxiaobao.xyz/Article/details/gmnwlhksv.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.fanxiaobao.xyz/Article/details/gkkxtmycx.sHtML

[T41] Perl：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwbebesor.sHtML

print "Hello\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/gyqvacifc.sHtML

[T42] Perl：变量类型
来源：http://baike.fanxiaobao.xyz/Article/details/gsflxksoa.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpzvzaqum.sHtML

[T43] Perl：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gfbqunztv.sHtML

"值: $a"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gemofnydd.sHtML

[T44] Perl：条件
来源：http://m.share.fanxiaobao.xyz/Article/details/grkjayvox.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gjfbubbrq.sHtML

[T45] Perl：数组遍历
来源：http://baike.fanxiaobao.xyz/Article/details/guujfnzko.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.fanxiaobao.xyz/Article/details/griinkvyw.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gqtstfpls.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gxudhsbmw.sHtML

[T47] Perl：正则捕获
来源：http://baike.fanxiaobao.xyz/Article/details/gvtpxcvtn.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggzqwfvcp.sHtML

[T48] Perl：正则替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gmwqacgce.sHtML

$s =~ s/old/new/g;
来源：http://blog.fanxiaobao.xyz/Article/details/gurjqvjaz.sHtML

[T49] Perl：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gbcmtytjv.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggvakrhmo.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/goasuhwns.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.fanxiaobao.xyz/Article/details/gevixtkwb.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.fanxiaobao.xyz/Article/details/goiwqcenj.sHtML

[T51] Scala：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gacqsuksh.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/giwzueife.sHtML

[T52] Scala：变量
来源：http://wap.fanxiaobao.xyz/Article/details/gjjlhkqmk.sHtML

val a = 1;  var b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gyejxfbgt.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpviwxwvz.sHtML

s"值: $b"
来源：http://baike.fanxiaobao.xyz/Article/details/gjgkeogbq.sHtML

[T54] Scala：集合映射
来源：http://3g.fanxiaobao.xyz/Article/details/gbdbwwvtn.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxcnqijdh.sHtML

[T55] Scala：集合过滤
来源：http://wap.fanxiaobao.xyz/Article/details/goonfyzwx.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.fanxiaobao.xyz/Article/details/glvbcymui.sHtML

[T56] Scala：样例类
来源：http://baike.fanxiaobao.xyz/Article/details/gfgwpcpkv.sHtML

case class User(name: String, age: Int)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbywzbjnu.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcbokconz.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gyrfdiyvz.sHtML

[T58] Scala：函数定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gutkjqksp.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.fanxiaobao.xyz/Article/details/giqnsojxr.sHtML

[T59] Scala：循环
来源：http://wap.fanxiaobao.xyz/Article/details/gkganyvju.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.fanxiaobao.xyz/Article/details/gqrcoormh.sHtML

[T60] Scala：折叠
来源：http://3g.fanxiaobao.xyz/Article/details/goedefcbz.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.fanxiaobao.xyz/Article/details/gbmzacbeo.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gtyoebhkp.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gomxtvwae.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gyzipyjqw.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.fanxiaobao.xyz/Article/details/gdcbeywhj.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.fanxiaobao.xyz/Article/details/gpzyowzkk.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.fanxiaobao.xyz/Article/details/gerxkyxur.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gahazvyly.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.fanxiaobao.xyz/Article/details/glqbhvdfj.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.fanxiaobao.xyz/Article/details/gzwsagkkj.sHtML

[U04] Py：变量调试打印
来源：http://read.share.fanxiaobao.xyz/Article/details/glgfwzawh.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.fanxiaobao.xyz/Article/details/gevgvuqoj.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzihuvcsw.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.fanxiaobao.xyz/Article/details/grxoogpoe.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggwnxvnno.sHtML

{**a, **b}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpoorusrw.sHtML

[U07] Py：反转字典键值
来源：http://www.share.fanxiaobao.xyz/Article/details/gvfqfzsjx.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.fanxiaobao.xyz/Article/details/gljtibarp.sHtML

[U08] Py：展平二维列表
来源：http://mobile.fanxiaobao.xyz/Article/details/gocdxoxgc.sHtML

[y for x in nested for y in x]
来源：http://www.share.fanxiaobao.xyz/Article/details/gtkvjwmgw.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.fanxiaobao.xyz/Article/details/giqkmzrse.sHtML

max(d, key=d.get)
来源：http://blog.fanxiaobao.xyz/Article/details/gwyeluojc.sHtML

[U10] Py：按值排序字典
来源：http://3g.fanxiaobao.xyz/Article/details/gqgtxwtij.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.fanxiaobao.xyz/Article/details/gdvrhutyb.sHtML

[U11] Py：生成器表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gfafnwwdh.sHtML

(x * 2 for x in arr)
来源：http://wap.fanxiaobao.xyz/Article/details/gmgppvmcn.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.fanxiaobao.xyz/Article/details/gexahyszo.sHtML

Counter(arr).most_common(3)
来源：http://wap.fanxiaobao.xyz/Article/details/gzcrhapop.sHtML

[U13] Py：固定长度队列
来源：http://mobile.fanxiaobao.xyz/Article/details/gzrzxpmeo.sHtML

deque(maxlen=10)
来源：http://baike.fanxiaobao.xyz/Article/details/gquvpmzce.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.fanxiaobao.xyz/Article/details/guocxjvof.sHtML

defaultdict(list)
来源：http://baike.fanxiaobao.xyz/Article/details/gsnynolza.sHtML

[U15] Py：高精度计时
来源：http://read.share.fanxiaobao.xyz/Article/details/gazdxeioq.sHtML

t = time.perf_counter()
来源：http://3g.fanxiaobao.xyz/Article/details/gdwclfeuj.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.fanxiaobao.xyz/Article/details/gkfvkroxv.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.fanxiaobao.xyz/Article/details/gacoqwvpx.sHtML

[U17] Py：初始化日志
来源：http://baike.fanxiaobao.xyz/Article/details/gyyeniprb.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.fanxiaobao.xyz/Article/details/gfqlcunvt.sHtML

[U18] Py：预编译正则
来源：http://m.share.fanxiaobao.xyz/Article/details/gltongcbw.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.fanxiaobao.xyz/Article/details/ggetxkmxv.sHtML

[U19] Py：正则替换带回调
来源：http://blog.fanxiaobao.xyz/Article/details/gvjxlbbse.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqeqhvxvd.sHtML

[U20] Py：缓存函数结果
来源：http://3g.fanxiaobao.xyz/Article/details/gpxfztfee.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.fanxiaobao.xyz/Article/details/gjlpjqnbp.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.fanxiaobao.xyz/Article/details/gfhewrhki.sHtML

@contextlib.contextmanager
来源：http://www.share.fanxiaobao.xyz/Article/details/gcqftjbqo.sHtML

[U22] Py：矩阵转置
来源：http://m.share.fanxiaobao.xyz/Article/details/gdgsbqupe.sHtML

list(zip(*m))
来源：http://mobile.fanxiaobao.xyz/Article/details/gvetniwcb.sHtML

[U23] Py：分块读取大文件
来源：http://blog.fanxiaobao.xyz/Article/details/geumsopas.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsaxitdbj.sHtML

[U24] Py：路径操作
来源：http://wap.fanxiaobao.xyz/Article/details/gkkoiukly.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.fanxiaobao.xyz/Article/details/grbphjqeq.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.fanxiaobao.xyz/Article/details/gafbkdgfb.sHtML

csv.DictReader(f)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjkgizxnz.sHtML

[U26] Py：并发下载
来源：http://baike.fanxiaobao.xyz/Article/details/gdkxjziag.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.fanxiaobao.xyz/Article/details/gifnzljsg.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fanxiaobao.xyz/Article/details/grnuwbymf.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.fanxiaobao.xyz/Article/details/gigcretof.sHtML

[U28] Py：类型别名
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvtjxlurl.sHtML

UserId = int
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giuyfkwif.sHtML

[U29] Py：属性校验
来源：http://blog.fanxiaobao.xyz/Article/details/gcajmvlno.sHtML

@property 与 @x.setter 配合
来源：http://read.share.fanxiaobao.xyz/Article/details/gnemttsjo.sHtML

[U30] Py：数据类
来源：http://baike.fanxiaobao.xyz/Article/details/gmmukdpmf.sHtML

@dataclass(slots=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gldymqjgh.sHtML

[U31] Py：单测
来源：http://baike.fanxiaobao.xyz/Article/details/gnnnukkaa.sHtML

python -m pytest -q
来源：http://www.share.fanxiaobao.xyz/Article/details/geeylwngl.sHtML

[U32] Py：代码格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gmmgaebgg.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvrxwqrjk.sHtML

[U33] Py：打包发布
来源：http://blog.fanxiaobao.xyz/Article/details/gnzvaklyr.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.fanxiaobao.xyz/Article/details/gqeedwrxk.sHtML

[U34] Py：判断编码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdlmwfcul.sHtML

chardet.detect(raw)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwugxfmpi.sHtML

[U35] Py：发送邮件
来源：http://baike.fanxiaobao.xyz/Article/details/ggsyvxhlx.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqsqreuhh.sHtML

[U36] Py：定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/gponuyekt.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqzxaytyw.sHtML

[U37] Py：读写 Excel
来源：http://blog.fanxiaobao.xyz/Article/details/gjolowwno.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.fanxiaobao.xyz/Article/details/gmlrkvybg.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.fanxiaobao.xyz/Article/details/gzpeszadt.sHtML

Path(__file__).resolve().parent
来源：http://read.share.fanxiaobao.xyz/Article/details/grdpihyet.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.fanxiaobao.xyz/Article/details/gfhnmajoc.sHtML

sys.stdout.isatty()
来源：http://wap.fanxiaobao.xyz/Article/details/goobnaqra.sHtML

[U40] Py：打印到标准错误
来源：http://wap.fanxiaobao.xyz/Article/details/gqznagohp.sHtML

print("err", file=sys.stderr)
来源：http://baike.fanxiaobao.xyz/Article/details/galhybocn.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.fanxiaobao.xyz/Article/details/geozfzzyw.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gngfkndse.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxppbpsub.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gewhnxmcs.sHtML

[U43] PHP：声明命名空间
来源：http://wap.fanxiaobao.xyz/Article/details/ghlgpgpmt.sHtML

namespace App\Http;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdjwponrg.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.fanxiaobao.xyz/Article/details/giqrnpozk.sHtML

declare(strict_types=1);
来源：http://wap.fanxiaobao.xyz/Article/details/gkblhedxc.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.fanxiaobao.xyz/Article/details/grxbhmyqc.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/guxadstza.sHtML

[U46] PHP：可空类型
来源：http://mobile.fanxiaobao.xyz/Article/details/ggsogkywr.sHtML

?string $name = null
来源：http://baike.fanxiaobao.xyz/Article/details/gbhtniccn.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glpcnxnvn.sHtML

int|string $id
来源：http://mobile.fanxiaobao.xyz/Article/details/ghbvcraau.sHtML

[U48] PHP：纯枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/ghkvouxuz.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gweaokwjv.sHtML

[U49] PHP：只读属性
来源：http://3g.fanxiaobao.xyz/Article/details/gwgdyfrvf.sHtML

public readonly string $name
来源：http://www.share.fanxiaobao.xyz/Article/details/gidmvghfu.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.fanxiaobao.xyz/Article/details/gibihxcyr.sHtML

public function __construct(private int $id) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gmtbyfjzk.sHtML

[U51] PHP：数组解构
来源：http://3g.fanxiaobao.xyz/Article/details/gnvqnknwk.sHtML

[$a, $b] = $arr;
来源：http://blog.fanxiaobao.xyz/Article/details/grnxmhwgc.sHtML

[U52] PHP：箭头函数
来源：http://m.share.fanxiaobao.xyz/Article/details/ggvjndbgl.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnmkawdyj.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.fanxiaobao.xyz/Article/details/gsjbwiuct.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gupvmrawz.sHtML

[U54] PHP：空安全调用
来源：http://blog.fanxiaobao.xyz/Article/details/gxjvzsbuh.sHtML

$obj?->method()
来源：http://read.share.fanxiaobao.xyz/Article/details/gpppfxqog.sHtML

[U55] PHP：match 表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gtopidnev.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.fanxiaobao.xyz/Article/details/gcucfiojn.sHtML

[U56] PHP：命名参数
来源：http://m.share.fanxiaobao.xyz/Article/details/giaccfuue.sHtML

f(a: 1, b: 2)
来源：http://wap.fanxiaobao.xyz/Article/details/ggygtmqzy.sHtML

[U57] PHP：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gclarghzq.sHtML

"值: {$a}"
来源：http://m.share.fanxiaobao.xyz/Article/details/ggnnneeah.sHtML

[U58] PHP：数组三件套
来源：http://read.share.fanxiaobao.xyz/Article/details/gxcwkinyr.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.fanxiaobao.xyz/Article/details/gtpdotayx.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzpsmkqds.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbmptzrqc.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.fanxiaobao.xyz/Article/details/gjptpkdnn.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwztifabr.sHtML

[U61] PHP：正则
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsamwxzlm.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmhuxnpwl.sHtML

[U62] PHP：日期对象
来源：http://blog.fanxiaobao.xyz/Article/details/goctduydu.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.fanxiaobao.xyz/Article/details/gdwuidwnu.sHtML

[U63] PHP：文件读写
来源：http://baike.fanxiaobao.xyz/Article/details/gxoewgwln.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.fanxiaobao.xyz/Article/details/gemnitspw.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grhfvsbpz.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.fanxiaobao.xyz/Article/details/guviamthm.sHtML

[U65] PHP：会话
来源：http://www.share.fanxiaobao.xyz/Article/details/ghksmunqk.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gqdgirkir.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsuvpsidf.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkwtwgxkz.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghvunyegd.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzhlcrvtf.sHtML

[U68] PHP：PDO 连接
来源：http://baike.fanxiaobao.xyz/Article/details/gfiayvtko.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.fanxiaobao.xyz/Article/details/gqcffszhp.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzukenjuw.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gownvsmvb.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gbomgmjnh.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.fanxiaobao.xyz/Article/details/gatfedsmv.sHtML

[U71] PHP：抛出异常
来源：http://blog.fanxiaobao.xyz/Article/details/gtaczavyd.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghdoybpgq.sHtML

[U72] PHP：写错误日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gxfmnpuuu.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdcodcatz.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.fanxiaobao.xyz/Article/details/gsgngmmdi.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsatqvbmc.sHtML

[U74] PHP：读取环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/guacaprqa.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.fanxiaobao.xyz/Article/details/ghxovjaxy.sHtML

[U75] PHP：依赖注入
来源：http://read.share.fanxiaobao.xyz/Article/details/gbhzzeqkr.sHtML

composer require psr/container
来源：http://www.share.fanxiaobao.xyz/Article/details/ghyurahzr.sHtML

[U76] PHP：简单路由
来源：http://mobile.fanxiaobao.xyz/Article/details/gbkhdhijn.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.fanxiaobao.xyz/Article/details/gyneqorts.sHtML

[U77] PHP：模板渲染
来源：http://read.share.fanxiaobao.xyz/Article/details/gxxcrkglc.sHtML

composer require twig/twig
来源：http://blog.fanxiaobao.xyz/Article/details/gucpqcsmw.sHtML

[U78] PHP：单元测试
来源：http://mobile.fanxiaobao.xyz/Article/details/gjpvupwtb.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.fanxiaobao.xyz/Article/details/gxgtnfzeq.sHtML

[U79] PHP：静态分析
来源：http://mobile.fanxiaobao.xyz/Article/details/geqnqxvqd.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyhfagaqw.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.fanxiaobao.xyz/Article/details/gbehpsjkt.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.fanxiaobao.xyz/Article/details/gzwpnwxri.sHtML

[U81] JS：初始化项目
来源：http://blog.fanxiaobao.xyz/Article/details/gtfigcgyr.sHtML

npm init -y;  npm i express
来源：http://baike.fanxiaobao.xyz/Article/details/ggswrnbvv.sHtML

[U82] JS：package.json 脚本
来源：http://wap.fanxiaobao.xyz/Article/details/gpcnogwro.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.fanxiaobao.xyz/Article/details/gjviumeie.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnehgyqgr.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.fanxiaobao.xyz/Article/details/gsixkywyx.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.fanxiaobao.xyz/Article/details/gvqnnzvap.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.fanxiaobao.xyz/Article/details/gmdeeihyw.sHtML

[U85] JS：可选链
来源：http://baike.fanxiaobao.xyz/Article/details/geqdavxbe.sHtML

a?.b?.c
来源：http://read.share.fanxiaobao.xyz/Article/details/gofnrkpzh.sHtML

[U86] JS：空值合并
来源：http://www.blog.fanxiaobao.xyz/Article/details/gimxeynzv.sHtML

a ?? b
来源：http://www.share.fanxiaobao.xyz/Article/details/glileqjxm.sHtML

[U87] JS：解构默认值
来源：http://blog.fanxiaobao.xyz/Article/details/grjecvzke.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.fanxiaobao.xyz/Article/details/genxvmnym.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqfzazddt.sHtML

{ ...a, ...b }
来源：http://read.share.fanxiaobao.xyz/Article/details/gturngboj.sHtML

[U89] JS：数组去重
来源：http://www.share.fanxiaobao.xyz/Article/details/gjnpddrbo.sHtML

[...new Set(arr)]
来源：http://mobile.fanxiaobao.xyz/Article/details/godkzfmim.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxpbfmyon.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gphjlhexj.sHtML


<!-- 参考信息 -->