代发 wailian999

[T03] Kotlin：字符串模板
来源：http://baike.hesvh.cn/Article/details/gsycjesuc.sHtML

"值: $b"
来源：http://m.share.hesvh.cn/Article/details/gkjmwazlk.sHtML

[T04] Kotlin：空安全
来源：http://baike.fehbvm.com/Article/details/gfbjsbuxc.sHtML

val n: String? = null;  n?.length
来源：http://m.share.zdbjq.cn/Article/details/genzxpimu.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fehbvm.com/Article/details/gayxxmtri.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.hesvh.cn/Article/details/gfslogiba.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.hesvh.cn/Article/details/gnmwkyseb.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gbevnnjpi.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.hesvh.cn/Article/details/gaflohkcb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.hesvh.cn/Article/details/gtxodfhbf.sHtML

[T08] Kotlin：数据类
来源：http://3g.hesvh.cn/Article/details/gxvxaeitl.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fehbvm.com/Article/details/gnbhuclzr.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fehbvm.com/Article/details/gwtvtwbsm.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fehbvm.com/Article/details/gttjizoyv.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.zdbjq.cn/Article/details/gvevrpgpl.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.zdbjq.cn/Article/details/grzwjnlzx.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fehbvm.com/Article/details/gymapvuhz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.fehbvm.com/Article/details/goisfskkp.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fehbvm.com/Article/details/gvtmothmq.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gsshspymm.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fehbvm.com/Article/details/gnisgabxk.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fehbvm.com/Article/details/gsdlmdahm.sHtML

[T14] Kotlin：循环
来源：http://www.share.hesvh.cn/Article/details/gbvxvqxyv.sHtML

for (i in 1..10) println(i)
来源：http://www.share.hesvh.cn/Article/details/gasywoqpc.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fehbvm.com/Article/details/gfgmrwaqn.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.hesvh.cn/Article/details/gdkhvtdsi.sHtML

[T16] Swift：Hello World
来源：http://wap.fehbvm.com/Article/details/gnfevfhkl.sHtML

print("Hello")
来源：http://3g.zdbjq.cn/Article/details/gttgrvxew.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fehbvm.com/Article/details/gukvrxnub.sHtML

var a = 1;  let b = 2
来源：http://baike.hesvh.cn/Article/details/gtiqggntf.sHtML

[T18] Swift：字符串插值
来源：http://wap.fehbvm.com/Article/details/gmsykzlgv.sHtML

"值: \(b)"
来源：http://www.share.zdbjq.cn/Article/details/gcwrhjqlk.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fehbvm.com/Article/details/gqhkvikyc.sHtML

if let n = opt { print(n) }
来源：http://read.share.zdbjq.cn/Article/details/gxygyyhhc.sHtML

[T20] Swift：数组操作
来源：http://baike.fehbvm.com/Article/details/gxjtobrey.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fehbvm.com/Article/details/gydxklipo.sHtML

[T21] Swift：遍历
来源：http://blog.fehbvm.com/Article/details/guayddioa.sHtML

for x in a { print(x) }
来源：http://blog.fehbvm.com/Article/details/gxdeqsohz.sHtML

[T22] Swift：字典
来源：http://www.m.share.zdbjq.cn/Article/details/gjekocctr.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.zdbjq.cn/Article/details/gquhrmdqy.sHtML

[T23] Swift：函数
来源：http://mobile.fehbvm.com/Article/details/gfqsminlg.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.hesvh.cn/Article/details/gcrrzoybm.sHtML

[T24] Swift：闭包
来源：http://baike.hesvh.cn/Article/details/gnurptpfn.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.hesvh.cn/Article/details/gzhhicuun.sHtML

[T25] Swift：结构体
来源：http://www.blog.zdbjq.cn/Article/details/gsbnlhsnk.sHtML

struct P { var x: Int }
来源：http://read.share.hesvh.cn/Article/details/gzsvqwxnb.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.zdbjq.cn/Article/details/gjiyagcfe.sHtML

class A: Base { override func f() {} }
来源：http://wap.fehbvm.com/Article/details/gxcwtlgyf.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fehbvm.com/Article/details/gzjlsuwmy.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.zdbjq.cn/Article/details/giyjoyhgy.sHtML

[T28] Swift：枚举
来源：http://www.blog.zdbjq.cn/Article/details/gugtqehnl.sHtML

enum Color { case red, green }
来源：http://www.blog.hesvh.cn/Article/details/gdtxdhzzz.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.hesvh.cn/Article/details/gesfozedg.sHtML

guard let x = opt else { return }
来源：http://www.m.share.zdbjq.cn/Article/details/gnpawklfh.sHtML

[T30] Swift：协议
来源：http://m.share.zdbjq.cn/Article/details/ghqskpwsj.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.hesvh.cn/Article/details/gvitthmiz.sHtML

[T31] Lua：Hello World
来源：http://wap.zdbjq.cn/Article/details/gnjluefld.sHtML

print("Hello")
来源：http://wap.fehbvm.com/Article/details/geiypwklb.sHtML

[T32] Lua：局部变量
来源：http://read.share.hesvh.cn/Article/details/gblngarnu.sHtML

local a = 1
来源：http://m.share.hesvh.cn/Article/details/gujsuowix.sHtML

[T33] Lua：表（数组）
来源：http://blog.fehbvm.com/Article/details/gzmrbpmql.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.fehbvm.com/Article/details/gaoybwawj.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.hesvh.cn/Article/details/gdhcrqhsg.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.fehbvm.com/Article/details/gsuqbafqc.sHtML

[T35] Lua：字典表
来源：http://3g.zdbjq.cn/Article/details/gotsszton.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/guririptd.sHtML

[T36] Lua：函数
来源：http://3g.fehbvm.com/Article/details/gsslviksj.sHtML

function add(a, b) return a + b end
来源：http://m.share.fehbvm.com/Article/details/gfxvecagq.sHtML

[T37] Lua：字符串拼接
来源：http://wap.fehbvm.com/Article/details/gbvkzxrgh.sHtML

"a" .. "b"
来源：http://blog.hesvh.cn/Article/details/gxnocrrdf.sHtML

[T38] Lua：条件
来源：http://read.share.zdbjq.cn/Article/details/gtmasycbv.sHtML

if x > 0 then print("正") end
来源：http://www.blog.fehbvm.com/Article/details/gsdwvzwnh.sHtML

[T39] Lua：模式匹配
来源：http://mobile.hesvh.cn/Article/details/guzflhuau.sHtML

string.find(s, "%d+")
来源：http://www.share.fehbvm.com/Article/details/gxeibniop.sHtML

[T40] Lua：元表
来源：http://blog.zdbjq.cn/Article/details/ggaztqdkl.sHtML

setmetatable({}, { __index = base })
来源：http://wap.zdbjq.cn/Article/details/galykctwu.sHtML

[T41] Perl：Hello World
来源：http://3g.fehbvm.com/Article/details/gtyuqjanv.sHtML

print "Hello\n";
来源：http://blog.zdbjq.cn/Article/details/gitfgehbn.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.zdbjq.cn/Article/details/gnhkntfjc.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.fehbvm.com/Article/details/gkaalzoyq.sHtML

[T43] Perl：字符串插值
来源：http://baike.fehbvm.com/Article/details/ggioujmoj.sHtML

"值: $a"
来源：http://m.share.zdbjq.cn/Article/details/gaeokueli.sHtML

[T44] Perl：条件
来源：http://m.share.hesvh.cn/Article/details/gelmfimzl.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.fehbvm.com/Article/details/gmrbnmyfm.sHtML

[T45] Perl：数组遍历
来源：http://blog.fehbvm.com/Article/details/gtqjjjdgs.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.hesvh.cn/Article/details/gbclqdudu.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.hesvh.cn/Article/details/gpsmhgwjy.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.fehbvm.com/Article/details/gcbyntxlc.sHtML

[T47] Perl：正则捕获
来源：http://mobile.fehbvm.com/Article/details/gxwzmgiku.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.fehbvm.com/Article/details/gharulwea.sHtML

[T48] Perl：正则替换
来源：http://mobile.zdbjq.cn/Article/details/gtyupcgvi.sHtML

$s =~ s/old/new/g;
来源：http://m.share.hesvh.cn/Article/details/gcrfimwch.sHtML

[T49] Perl：函数
来源：http://3g.fehbvm.com/Article/details/giixglzfy.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gsuqbqllb.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/ggpzisoaj.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.zdbjq.cn/Article/details/gbtuarcvh.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.zdbjq.cn/Article/details/ghhrtitrz.sHtML

[T51] Scala：Hello World
来源：http://wap.zdbjq.cn/Article/details/gnrpbhouo.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/gwfynzrbu.sHtML

[T52] Scala：变量
来源：http://read.share.hesvh.cn/Article/details/gatwzlvtw.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gehgjzixi.sHtML

[T53] Scala：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gxkpraztu.sHtML

s"值: $b"
来源：http://3g.fehbvm.com/Article/details/gmqbzfnol.sHtML

[T54] Scala：集合映射
来源：http://www.share.hesvh.cn/Article/details/gvalwlvrz.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.zdbjq.cn/Article/details/gtxcftupq.sHtML

[T55] Scala：集合过滤
来源：http://baike.zdbjq.cn/Article/details/gzralvhay.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.hesvh.cn/Article/details/gpthjboie.sHtML

[T56] Scala：样例类
来源：http://m.share.fehbvm.com/Article/details/gtcflwgcq.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.zdbjq.cn/Article/details/gxjfbsyfs.sHtML

[T57] Scala：模式匹配
来源：http://m.share.zdbjq.cn/Article/details/gbrdudmxj.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.fehbvm.com/Article/details/gtaxgoeyf.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.hesvh.cn/Article/details/gkskqkyfi.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.fehbvm.com/Article/details/gtmdjbbyw.sHtML

[T59] Scala：循环
来源：http://read.share.hesvh.cn/Article/details/giwlmfxxz.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.zdbjq.cn/Article/details/ghqagdzkx.sHtML

[T60] Scala：折叠
来源：http://www.blog.hesvh.cn/Article/details/gqtlukwxf.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.hesvh.cn/Article/details/gomjbqgvb.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gfoandkyz.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fehbvm.com/Article/details/guxuwbqcj.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gjbkagwde.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.zdbjq.cn/Article/details/gzgkfdbfr.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.fehbvm.com/Article/details/glpgkucdp.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.hesvh.cn/Article/details/gijyskdks.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.fehbvm.com/Article/details/gmnutttaj.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.fehbvm.com/Article/details/gibtjayoo.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.fehbvm.com/Article/details/gwnfemwga.sHtML

[U04] Py：变量调试打印
来源：http://blog.hesvh.cn/Article/details/gmgpcstqu.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.zdbjq.cn/Article/details/gkjtsmuit.sHtML

[U05] Py：列表去重且保序
来源：http://blog.zdbjq.cn/Article/details/gulfsmltv.sHtML

list(dict.fromkeys(arr))
来源：http://baike.zdbjq.cn/Article/details/gmjjevuow.sHtML

[U06] Py：合并两个字典
来源：http://wap.hesvh.cn/Article/details/gbjhugski.sHtML

{**a, **b}
来源：http://3g.fehbvm.com/Article/details/gvlrshcep.sHtML

[U07] Py：反转字典键值
来源：http://blog.fehbvm.com/Article/details/gvsbmehgl.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fehbvm.com/Article/details/gsiqjivvm.sHtML

[U08] Py：展平二维列表
来源：http://mobile.fehbvm.com/Article/details/gpcvfidzk.sHtML

[y for x in nested for y in x]
来源：http://read.share.fehbvm.com/Article/details/gktxdkfnb.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.hesvh.cn/Article/details/gxubicrkl.sHtML

max(d, key=d.get)
来源：http://wap.zdbjq.cn/Article/details/gtwzfjkmb.sHtML

[U10] Py：按值排序字典
来源：http://3g.hesvh.cn/Article/details/gwpehseln.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.hesvh.cn/Article/details/gitwmnitg.sHtML

[U11] Py：生成器表达式
来源：http://www.share.zdbjq.cn/Article/details/gqddwicrq.sHtML

(x * 2 for x in arr)
来源：http://blog.zdbjq.cn/Article/details/gfxkgptiy.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.zdbjq.cn/Article/details/gbdqsbflm.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.hesvh.cn/Article/details/gqcuqutsh.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.zdbjq.cn/Article/details/gpzlebmax.sHtML

deque(maxlen=10)
来源：http://wap.fehbvm.com/Article/details/ggbmfvgev.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.fehbvm.com/Article/details/guvlydfcp.sHtML

defaultdict(list)
来源：http://baike.zdbjq.cn/Article/details/gbuanwjax.sHtML

[U15] Py：高精度计时
来源：http://mobile.hesvh.cn/Article/details/gkbgxwzrz.sHtML

t = time.perf_counter()
来源：http://www.share.hesvh.cn/Article/details/gbitgswfy.sHtML

[U16] Py：命令行参数解析
来源：http://wap.zdbjq.cn/Article/details/geifmmejd.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.zdbjq.cn/Article/details/gdtoltvxw.sHtML

[U17] Py：初始化日志
来源：http://baike.zdbjq.cn/Article/details/gxsjayxem.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.hesvh.cn/Article/details/gnkisyxvz.sHtML

[U18] Py：预编译正则
来源：http://read.share.hesvh.cn/Article/details/glkbgktkz.sHtML

pat = re.compile(r"\d+")
来源：http://3g.zdbjq.cn/Article/details/gvmgrwbjt.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.zdbjq.cn/Article/details/gwlvdsjhw.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.hesvh.cn/Article/details/gewvgrrvi.sHtML

[U20] Py：缓存函数结果
来源：http://baike.zdbjq.cn/Article/details/gzviucaoi.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.fehbvm.com/Article/details/gepjsartq.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.zdbjq.cn/Article/details/gucbngkih.sHtML

@contextlib.contextmanager
来源：http://m.share.zdbjq.cn/Article/details/guyqohmog.sHtML

[U22] Py：矩阵转置
来源：http://mobile.hesvh.cn/Article/details/grckhmnoc.sHtML

list(zip(*m))
来源：http://www.blog.zdbjq.cn/Article/details/gtlmdlxpg.sHtML

[U23] Py：分块读取大文件
来源：http://blog.zdbjq.cn/Article/details/gorpueamn.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.zdbjq.cn/Article/details/gexvfezji.sHtML

[U24] Py：路径操作
来源：http://blog.hesvh.cn/Article/details/gmepyslzg.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/ggnygedgf.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.hesvh.cn/Article/details/gwnaubrrc.sHtML

csv.DictReader(f)
来源：http://mobile.hesvh.cn/Article/details/gyqrhnnqk.sHtML

[U26] Py：并发下载
来源：http://mobile.zdbjq.cn/Article/details/grzimvila.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.hesvh.cn/Article/details/geacxcisw.sHtML

[U27] Py：异步 HTTP
来源：http://blog.hesvh.cn/Article/details/gzfdpnusv.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.zdbjq.cn/Article/details/gvndolrmu.sHtML

[U28] Py：类型别名
来源：http://baike.fehbvm.com/Article/details/gqenhffqn.sHtML

UserId = int
来源：http://www.blog.hesvh.cn/Article/details/ggmuwzaxi.sHtML

[U29] Py：属性校验
来源：http://mobile.hesvh.cn/Article/details/gmdfpenir.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.hesvh.cn/Article/details/gobmtzzyt.sHtML

[U30] Py：数据类
来源：http://3g.fehbvm.com/Article/details/gnbgxbvyf.sHtML

@dataclass(slots=True)
来源：http://www.blog.hesvh.cn/Article/details/grzlilzmw.sHtML

[U31] Py：单测
来源：http://m.share.zdbjq.cn/Article/details/gqnzmzsis.sHtML

python -m pytest -q
来源：http://read.share.hesvh.cn/Article/details/gxpdkctbb.sHtML

[U32] Py：代码格式化
来源：http://read.share.fehbvm.com/Article/details/gxawnskfl.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.zdbjq.cn/Article/details/gfjzqonbc.sHtML

[U33] Py：打包发布
来源：http://3g.hesvh.cn/Article/details/ghmthyjog.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.fehbvm.com/Article/details/gznduckpc.sHtML

[U34] Py：判断编码
来源：http://blog.fehbvm.com/Article/details/gnxiheeau.sHtML

chardet.detect(raw)
来源：http://mobile.hesvh.cn/Article/details/gzsfysvok.sHtML

[U35] Py：发送邮件
来源：http://baike.hesvh.cn/Article/details/gjjrbhgfd.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.hesvh.cn/Article/details/grfvcyyfi.sHtML

[U36] Py：定时任务
来源：http://www.blog.hesvh.cn/Article/details/goxyselax.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.hesvh.cn/Article/details/gizoffmpz.sHtML

[U37] Py：读写 Excel
来源：http://mobile.zdbjq.cn/Article/details/gglriwprf.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.hesvh.cn/Article/details/gcngrwpwz.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.fehbvm.com/Article/details/gppkkrrwd.sHtML

Path(__file__).resolve().parent
来源：http://blog.zdbjq.cn/Article/details/gtvyktvex.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.zdbjq.cn/Article/details/ggidondrg.sHtML

sys.stdout.isatty()
来源：http://www.blog.fehbvm.com/Article/details/gzhwtdcpi.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.hesvh.cn/Article/details/ggexhvnho.sHtML

print("err", file=sys.stderr)
来源：http://m.share.hesvh.cn/Article/details/gtxqbmrgi.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.zdbjq.cn/Article/details/goohkecds.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.fehbvm.com/Article/details/gpqaytjcd.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.fehbvm.com/Article/details/gbpoomkry.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.zdbjq.cn/Article/details/gnaysocch.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.zdbjq.cn/Article/details/gpljxblgj.sHtML

namespace App\Http;
来源：http://wap.fehbvm.com/Article/details/gbodhzdtc.sHtML

[U44] PHP：开启严格类型
来源：http://blog.zdbjq.cn/Article/details/gprytvyzb.sHtML

declare(strict_types=1);
来源：http://www.share.fehbvm.com/Article/details/gdkkolcwe.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.hesvh.cn/Article/details/gjygrhmdo.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/giqxiyehy.sHtML

[U46] PHP：可空类型
来源：http://www.blog.fehbvm.com/Article/details/gspoeyaou.sHtML

?string $name = null
来源：http://3g.hesvh.cn/Article/details/gxakpsvxd.sHtML

[U47] PHP：联合类型
来源：http://m.share.fehbvm.com/Article/details/gtewiikla.sHtML

int|string $id
来源：http://3g.hesvh.cn/Article/details/gcjuzshhj.sHtML

[U48] PHP：纯枚举
来源：http://wap.hesvh.cn/Article/details/ghjlrbcrk.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.zdbjq.cn/Article/details/gnuoelmbx.sHtML

[U49] PHP：只读属性
来源：http://read.share.hesvh.cn/Article/details/gpdgpcksr.sHtML

public readonly string $name
来源：http://www.m.share.fehbvm.com/Article/details/gqvixnmyn.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.fehbvm.com/Article/details/gazeazrvc.sHtML

public function __construct(private int $id) {}
来源：http://baike.fehbvm.com/Article/details/gutqbrmkn.sHtML

[U51] PHP：数组解构
来源：http://www.blog.fehbvm.com/Article/details/gjhkklpvz.sHtML

[$a, $b] = $arr;
来源：http://blog.fehbvm.com/Article/details/grneefmdt.sHtML

[U52] PHP：箭头函数
来源：http://blog.hesvh.cn/Article/details/gazbroatt.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.hesvh.cn/Article/details/gvufuplpk.sHtML

[U53] PHP：空合并运算符
来源：http://baike.hesvh.cn/Article/details/gwllczsti.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.hesvh.cn/Article/details/gshbjabrk.sHtML

[U54] PHP：空安全调用
来源：http://blog.zdbjq.cn/Article/details/gggxvxvhw.sHtML

$obj?->method()
来源：http://www.blog.fehbvm.com/Article/details/glvcgolow.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gwcmaolht.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.fehbvm.com/Article/details/gjqxfldbs.sHtML

[U56] PHP：命名参数
来源：http://baike.fehbvm.com/Article/details/gsuzjahev.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/gcdejjqlo.sHtML

[U57] PHP：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gaiocichx.sHtML

"值: {$a}"
来源：http://wap.zdbjq.cn/Article/details/gjfnlydok.sHtML

[U58] PHP：数组三件套
来源：http://baike.hesvh.cn/Article/details/gttnmbgmr.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.fehbvm.com/Article/details/gfkeseejq.sHtML

[U59] PHP：自定义排序
来源：http://blog.fehbvm.com/Article/details/gaexnmrgb.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fehbvm.com/Article/details/ghpmlcvkk.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.zdbjq.cn/Article/details/gmhceghvl.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.fehbvm.com/Article/details/gcxyzamzp.sHtML

[U61] PHP：正则
来源：http://www.m.share.fehbvm.com/Article/details/gcaeqdznj.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.hesvh.cn/Article/details/gpzsrayoc.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.fehbvm.com/Article/details/gyllyoaoz.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.fehbvm.com/Article/details/glaklwwrn.sHtML

[U63] PHP：文件读写
来源：http://blog.hesvh.cn/Article/details/gfxgtggeu.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.hesvh.cn/Article/details/gtxjflymg.sHtML

[U64] PHP：目录遍历
来源：http://3g.hesvh.cn/Article/details/gjyyhstxw.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.fehbvm.com/Article/details/gqnuplaex.sHtML

[U65] PHP：会话
来源：http://www.share.zdbjq.cn/Article/details/gskorjcyn.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.zdbjq.cn/Article/details/givhiunbs.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.hesvh.cn/Article/details/gdxxqxuoh.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.zdbjq.cn/Article/details/gmmtpjnzd.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.hesvh.cn/Article/details/gzeuutbyd.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.zdbjq.cn/Article/details/gtbvxsjuo.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.hesvh.cn/Article/details/gccdbnwax.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.hesvh.cn/Article/details/gmrmomfht.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.fehbvm.com/Article/details/ggeqlotya.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.zdbjq.cn/Article/details/gbkleeuff.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.fehbvm.com/Article/details/gwayvdgtn.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.hesvh.cn/Article/details/glsvhafss.sHtML

[U71] PHP：抛出异常
来源：http://baike.hesvh.cn/Article/details/gldjvtmsj.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.fehbvm.com/Article/details/gsvsdgror.sHtML

[U72] PHP：写错误日志
来源：http://m.share.fehbvm.com/Article/details/giizhvzzy.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.fehbvm.com/Article/details/gwoecbide.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.hesvh.cn/Article/details/gehxwlfuh.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.zdbjq.cn/Article/details/gjhswuojq.sHtML

[U74] PHP：读取环境变量
来源：http://3g.hesvh.cn/Article/details/ghaabezfl.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.zdbjq.cn/Article/details/gdzedwhsj.sHtML

[U75] PHP：依赖注入
来源：http://wap.fehbvm.com/Article/details/gmxvhufyr.sHtML

composer require psr/container
来源：http://www.m.share.hesvh.cn/Article/details/gcgpcqgth.sHtML

[U76] PHP：简单路由
来源：http://m.share.fehbvm.com/Article/details/gumibxtuv.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.fehbvm.com/Article/details/gsprwvclo.sHtML

[U77] PHP：模板渲染
来源：http://www.share.hesvh.cn/Article/details/gcxplixku.sHtML

composer require twig/twig
来源：http://m.share.zdbjq.cn/Article/details/gortqwxuy.sHtML

[U78] PHP：单元测试
来源：http://www.share.fehbvm.com/Article/details/gshluyiqh.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.fehbvm.com/Article/details/giltdhceb.sHtML

[U79] PHP：静态分析
来源：http://m.share.fehbvm.com/Article/details/gryzaehlh.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.fehbvm.com/Article/details/gylmipesi.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.fehbvm.com/Article/details/guvbzckfd.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.fehbvm.com/Article/details/gowuhhoeg.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.fehbvm.com/Article/details/gmancqujk.sHtML

npm init -y;  npm i express
来源：http://mobile.zdbjq.cn/Article/details/gzikddcjo.sHtML

[U82] JS：package.json 脚本
来源：http://wap.zdbjq.cn/Article/details/gbylfqael.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.fehbvm.com/Article/details/gbizdgsuf.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.fehbvm.com/Article/details/gdolsmifl.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.hesvh.cn/Article/details/gsypfzbuh.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.fehbvm.com/Article/details/gqmekleqe.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.fehbvm.com/Article/details/gbsrxfczh.sHtML

[U85] JS：可选链
来源：http://wap.hesvh.cn/Article/details/ghnltprfn.sHtML

a?.b?.c
来源：http://www.share.fehbvm.com/Article/details/gqyxqngua.sHtML

[U86] JS：空值合并
来源：http://baike.fehbvm.com/Article/details/gauhdfijw.sHtML

a ?? b
来源：http://mobile.fehbvm.com/Article/details/glkubcdxu.sHtML

[U87] JS：解构默认值
来源：http://www.share.fehbvm.com/Article/details/gtsyodnia.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.fehbvm.com/Article/details/glwycrxrk.sHtML

[U88] JS：对象展开合并
来源：http://www.share.zdbjq.cn/Article/details/gjkebbnhc.sHtML

{ ...a, ...b }
来源：http://baike.hesvh.cn/Article/details/glshxqyrm.sHtML

[U89] JS：数组去重
来源：http://www.share.zdbjq.cn/Article/details/gqxitlwvg.sHtML

[...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gynhtslje.sHtML

[U90] JS：数字数组排序
来源：http://wap.fehbvm.com/Article/details/ggocslidt.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/gjmpxucjj.sHtML


<!-- 参考信息 -->