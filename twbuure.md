代发 wailian999

[T05] Kotlin：when 表达式
来源：http://wap.fehbvm.com/Article/details/glqbgtuax.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fehbvm.com/Article/details/gadtkxmjl.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fehbvm.com/Article/details/gjrnwwuty.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.hesvh.cn/Article/details/gjezhoaep.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.zdbjq.cn/Article/details/gxatscozk.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.zdbjq.cn/Article/details/gqlcpwnyf.sHtML

[T08] Kotlin：数据类
来源：http://www.share.zdbjq.cn/Article/details/gqnkyofuz.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fehbvm.com/Article/details/guatcjmvv.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.zdbjq.cn/Article/details/gwhmrfytl.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.zdbjq.cn/Article/details/ggobaqcia.sHtML

[T10] Kotlin：默认参数
来源：http://baike.hesvh.cn/Article/details/gezcyltzj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.zdbjq.cn/Article/details/ggzvzjlcy.sHtML

[T11] Kotlin：协程
来源：http://read.share.hesvh.cn/Article/details/gomvvpqaa.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.zdbjq.cn/Article/details/gsblholnx.sHtML

[T12] Kotlin：解构声明
来源：http://blog.hesvh.cn/Article/details/gfmcedppd.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gdlumolcb.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.zdbjq.cn/Article/details/gvnqudeyf.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fehbvm.com/Article/details/gnbbqrxen.sHtML

[T14] Kotlin：循环
来源：http://mobile.zdbjq.cn/Article/details/gmvpeygap.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.zdbjq.cn/Article/details/gjiutqawm.sHtML

[T15] Kotlin：接口
来源：http://blog.fehbvm.com/Article/details/gavpxomib.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fehbvm.com/Article/details/giryteprd.sHtML

[T16] Swift：Hello World
来源：http://wap.zdbjq.cn/Article/details/gzsnpzkpz.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/gyhwlaiqq.sHtML

[T17] Swift：变量与常量
来源：http://baike.fehbvm.com/Article/details/gkpbwlcgp.sHtML

var a = 1;  let b = 2
来源：http://m.share.zdbjq.cn/Article/details/gzvoktshy.sHtML

[T18] Swift：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gvazkvkzd.sHtML

"值: \(b)"
来源：http://wap.fehbvm.com/Article/details/geecmnqze.sHtML

[T19] Swift：可选绑定
来源：http://blog.fehbvm.com/Article/details/gxdensaky.sHtML

if let n = opt { print(n) }
来源：http://baike.zdbjq.cn/Article/details/gjolfljsr.sHtML

[T20] Swift：数组操作
来源：http://www.share.fehbvm.com/Article/details/gfsshgyxt.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.zdbjq.cn/Article/details/gdsggrzag.sHtML

[T21] Swift：遍历
来源：http://www.m.share.hesvh.cn/Article/details/glrovpgju.sHtML

for x in a { print(x) }
来源：http://m.share.hesvh.cn/Article/details/ginablfmu.sHtML

[T22] Swift：字典
来源：http://baike.fehbvm.com/Article/details/gewfjlsdd.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.fehbvm.com/Article/details/geovvsibh.sHtML

[T23] Swift：函数
来源：http://www.share.fehbvm.com/Article/details/gcyixzyna.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fehbvm.com/Article/details/gwcownnaw.sHtML

[T24] Swift：闭包
来源：http://baike.hesvh.cn/Article/details/goucbxuce.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gbdumcgpf.sHtML

[T25] Swift：结构体
来源：http://baike.hesvh.cn/Article/details/glizbtofw.sHtML

struct P { var x: Int }
来源：http://read.share.zdbjq.cn/Article/details/gxbhxbkzz.sHtML

[T26] Swift：类与重写
来源：http://mobile.zdbjq.cn/Article/details/gqqprmeyl.sHtML

class A: Base { override func f() {} }
来源：http://mobile.hesvh.cn/Article/details/gmnnxoljj.sHtML

[T27] Swift：错误处理
来源：http://read.share.hesvh.cn/Article/details/gurxemajk.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.zdbjq.cn/Article/details/gavistxyo.sHtML

[T28] Swift：枚举
来源：http://www.share.zdbjq.cn/Article/details/giyrkxbix.sHtML

enum Color { case red, green }
来源：http://mobile.zdbjq.cn/Article/details/gojvuvkfq.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.hesvh.cn/Article/details/gmlrewexp.sHtML

guard let x = opt else { return }
来源：http://baike.fehbvm.com/Article/details/gcxrgywkb.sHtML

[T30] Swift：协议
来源：http://www.share.zdbjq.cn/Article/details/gesqkejvb.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.zdbjq.cn/Article/details/gnrzntuyy.sHtML

[T31] Lua：Hello World
来源：http://3g.hesvh.cn/Article/details/gdtusmkey.sHtML

print("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/guphqpuwu.sHtML

[T32] Lua：局部变量
来源：http://www.share.zdbjq.cn/Article/details/gvplvbuzk.sHtML

local a = 1
来源：http://3g.zdbjq.cn/Article/details/gssfiivzc.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.zdbjq.cn/Article/details/gprgfmvws.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.zdbjq.cn/Article/details/gynaaaprd.sHtML

[T34] Lua：遍历表
来源：http://blog.hesvh.cn/Article/details/ghxcyaipq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fehbvm.com/Article/details/gjyrjjzrh.sHtML

[T35] Lua：字典表
来源：http://3g.fehbvm.com/Article/details/gueqfymiv.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.zdbjq.cn/Article/details/gxcdksuac.sHtML

[T36] Lua：函数
来源：http://read.share.hesvh.cn/Article/details/gatcjluaz.sHtML

function add(a, b) return a + b end
来源：http://www.blog.zdbjq.cn/Article/details/grxkeqnra.sHtML

[T37] Lua：字符串拼接
来源：http://baike.hesvh.cn/Article/details/gljbwejao.sHtML

"a" .. "b"
来源：http://wap.zdbjq.cn/Article/details/gezqewonx.sHtML

[T38] Lua：条件
来源：http://m.share.hesvh.cn/Article/details/gecgifvnr.sHtML

if x > 0 then print("正") end
来源：http://www.share.fehbvm.com/Article/details/gengtkdyf.sHtML

[T39] Lua：模式匹配
来源：http://blog.hesvh.cn/Article/details/gielklsmh.sHtML

string.find(s, "%d+")
来源：http://wap.hesvh.cn/Article/details/gmowmoywa.sHtML

[T40] Lua：元表
来源：http://wap.hesvh.cn/Article/details/gvoqrnhic.sHtML

setmetatable({}, { __index = base })
来源：http://3g.fehbvm.com/Article/details/gkdvcqxtj.sHtML

[T41] Perl：Hello World
来源：http://m.share.zdbjq.cn/Article/details/ghrjstzpm.sHtML

print "Hello\n";
来源：http://www.m.share.hesvh.cn/Article/details/gpzgpkoyo.sHtML

[T42] Perl：变量类型
来源：http://baike.zdbjq.cn/Article/details/gsuycxbgw.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.zdbjq.cn/Article/details/gvnqplgue.sHtML

[T43] Perl：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gvroovhcs.sHtML

"值: $a"
来源：http://read.share.fehbvm.com/Article/details/gbewvhfka.sHtML

[T44] Perl：条件
来源：http://www.blog.hesvh.cn/Article/details/gfsyhqtug.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.hesvh.cn/Article/details/gaccdgzgw.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.zdbjq.cn/Article/details/ggzkbdmua.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.hesvh.cn/Article/details/gqklbfrtm.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.fehbvm.com/Article/details/gulpcseha.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.fehbvm.com/Article/details/gzsemyhaz.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.fehbvm.com/Article/details/gwmgyyvmj.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.zdbjq.cn/Article/details/gpapfozyt.sHtML

[T48] Perl：正则替换
来源：http://wap.zdbjq.cn/Article/details/gxohtaavh.sHtML

$s =~ s/old/new/g;
来源：http://mobile.zdbjq.cn/Article/details/ghjyavvcu.sHtML

[T49] Perl：函数
来源：http://read.share.hesvh.cn/Article/details/gubluljys.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gfdzlxnvj.sHtML

[T50] Perl：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gadizejee.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.hesvh.cn/Article/details/gygdmqxzw.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.zdbjq.cn/Article/details/giiobjadt.sHtML

[T51] Scala：Hello World
来源：http://m.share.hesvh.cn/Article/details/gcikxrzjk.sHtML

println("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gdbmxfsds.sHtML

[T52] Scala：变量
来源：http://3g.fehbvm.com/Article/details/gyziwbihx.sHtML

val a = 1;  var b = 2
来源：http://m.share.hesvh.cn/Article/details/gqfgkqulp.sHtML

[T53] Scala：字符串插值
来源：http://blog.hesvh.cn/Article/details/ghogyepaw.sHtML

s"值: $b"
来源：http://baike.fehbvm.com/Article/details/gfuclhuqz.sHtML

[T54] Scala：集合映射
来源：http://www.share.zdbjq.cn/Article/details/gqelgxuhq.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.fehbvm.com/Article/details/gneuksirl.sHtML

[T55] Scala：集合过滤
来源：http://3g.hesvh.cn/Article/details/gcgbbvjrx.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.hesvh.cn/Article/details/gwaxuqwco.sHtML

[T56] Scala：样例类
来源：http://m.share.fehbvm.com/Article/details/gayalywai.sHtML

case class User(name: String, age: Int)
来源：http://wap.zdbjq.cn/Article/details/gsljsjrjl.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fehbvm.com/Article/details/gdcvloxjb.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.zdbjq.cn/Article/details/ggpfnqvec.sHtML

[T58] Scala：函数定义
来源：http://m.share.fehbvm.com/Article/details/gvqirblnv.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.hesvh.cn/Article/details/ghrcrrgtt.sHtML

[T59] Scala：循环
来源：http://blog.fehbvm.com/Article/details/gpxgklmik.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.hesvh.cn/Article/details/gxpyjlvbh.sHtML

[T60] Scala：折叠
来源：http://www.m.share.zdbjq.cn/Article/details/gokgkkzkw.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.hesvh.cn/Article/details/glwmklqii.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gpvvsubeh.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fehbvm.com/Article/details/glenkeilz.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gtiqwjzte.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.hesvh.cn/Article/details/goxdlkvor.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.hesvh.cn/Article/details/ghpgohhmf.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.fehbvm.com/Article/details/gnmcikdmm.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.hesvh.cn/Article/details/ggsswybom.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.zdbjq.cn/Article/details/gyyzaklpg.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.zdbjq.cn/Article/details/gvlxhxvpx.sHtML

[U04] Py：变量调试打印
来源：http://www.share.fehbvm.com/Article/details/gjvigjudo.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.fehbvm.com/Article/details/gjkwicycw.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.fehbvm.com/Article/details/gsyhygesj.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.fehbvm.com/Article/details/ghlnbpqnt.sHtML

[U06] Py：合并两个字典
来源：http://m.share.fehbvm.com/Article/details/grktysleh.sHtML

{**a, **b}
来源：http://baike.zdbjq.cn/Article/details/gtcwqrqds.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.hesvh.cn/Article/details/gxovbvadf.sHtML

{v: k for k, v in d.items()}
来源：http://blog.zdbjq.cn/Article/details/geblvykkz.sHtML

[U08] Py：展平二维列表
来源：http://www.share.zdbjq.cn/Article/details/gwkxfncbb.sHtML

[y for x in nested for y in x]
来源：http://m.share.zdbjq.cn/Article/details/gcxdmiopl.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.hesvh.cn/Article/details/goollubmk.sHtML

max(d, key=d.get)
来源：http://www.blog.hesvh.cn/Article/details/gyeafoaua.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.zdbjq.cn/Article/details/gmacrdety.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.fehbvm.com/Article/details/gozcryypd.sHtML

[U11] Py：生成器表达式
来源：http://mobile.fehbvm.com/Article/details/grqgkfjka.sHtML

(x * 2 for x in arr)
来源：http://www.share.fehbvm.com/Article/details/glcpwtjls.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.hesvh.cn/Article/details/gxdcetnxt.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.hesvh.cn/Article/details/gcgtztxxj.sHtML

[U13] Py：固定长度队列
来源：http://mobile.zdbjq.cn/Article/details/gzvsatjby.sHtML

deque(maxlen=10)
来源：http://baike.zdbjq.cn/Article/details/gpwoozpfk.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.zdbjq.cn/Article/details/gsvdksenx.sHtML

defaultdict(list)
来源：http://mobile.fehbvm.com/Article/details/gsxrcckqx.sHtML

[U15] Py：高精度计时
来源：http://mobile.hesvh.cn/Article/details/grligcxyx.sHtML

t = time.perf_counter()
来源：http://blog.zdbjq.cn/Article/details/gwkzinygm.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.zdbjq.cn/Article/details/gvfjkevzp.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.zdbjq.cn/Article/details/gwruwlrwi.sHtML

[U17] Py：初始化日志
来源：http://read.share.fehbvm.com/Article/details/gryqxeifa.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.zdbjq.cn/Article/details/gpdzpmkil.sHtML

[U18] Py：预编译正则
来源：http://blog.zdbjq.cn/Article/details/gbuhzxicw.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.zdbjq.cn/Article/details/gkrqjhoiz.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.hesvh.cn/Article/details/gzxadbods.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.hesvh.cn/Article/details/galjwngmj.sHtML

[U20] Py：缓存函数结果
来源：http://3g.hesvh.cn/Article/details/gcsnyeokz.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.fehbvm.com/Article/details/gkhbeekjc.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.hesvh.cn/Article/details/gkvarmafi.sHtML

@contextlib.contextmanager
来源：http://www.m.share.zdbjq.cn/Article/details/gkrtnagso.sHtML

[U22] Py：矩阵转置
来源：http://mobile.fehbvm.com/Article/details/gvvediatq.sHtML

list(zip(*m))
来源：http://blog.fehbvm.com/Article/details/gkhovmiqg.sHtML

[U23] Py：分块读取大文件
来源：http://baike.zdbjq.cn/Article/details/gjjhllktm.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.hesvh.cn/Article/details/gbrodcfax.sHtML

[U24] Py：路径操作
来源：http://www.share.hesvh.cn/Article/details/ghqfuwifx.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.zdbjq.cn/Article/details/glylssvhi.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.fehbvm.com/Article/details/gqixzweow.sHtML

csv.DictReader(f)
来源：http://www.share.fehbvm.com/Article/details/gavloogcs.sHtML

[U26] Py：并发下载
来源：http://3g.hesvh.cn/Article/details/gzguqgtso.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.zdbjq.cn/Article/details/ghvyqjzpr.sHtML

[U27] Py：异步 HTTP
来源：http://wap.zdbjq.cn/Article/details/ggufurrbi.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.hesvh.cn/Article/details/gyyeesmzo.sHtML

[U28] Py：类型别名
来源：http://wap.fehbvm.com/Article/details/glaoimqmh.sHtML

UserId = int
来源：http://www.blog.zdbjq.cn/Article/details/gqslrlhpp.sHtML

[U29] Py：属性校验
来源：http://www.share.hesvh.cn/Article/details/glpotivim.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.zdbjq.cn/Article/details/grosmcrla.sHtML

[U30] Py：数据类
来源：http://mobile.fehbvm.com/Article/details/gyghmciwk.sHtML

@dataclass(slots=True)
来源：http://read.share.zdbjq.cn/Article/details/gveeowysd.sHtML

[U31] Py：单测
来源：http://wap.hesvh.cn/Article/details/gcbyfdegr.sHtML

python -m pytest -q
来源：http://www.share.hesvh.cn/Article/details/gijretczs.sHtML

[U32] Py：代码格式化
来源：http://www.blog.fehbvm.com/Article/details/gewxqmipe.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.hesvh.cn/Article/details/gydekkygq.sHtML

[U33] Py：打包发布
来源：http://www.m.share.zdbjq.cn/Article/details/gumzkstff.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.hesvh.cn/Article/details/grlnumkut.sHtML

[U34] Py：判断编码
来源：http://3g.fehbvm.com/Article/details/ggjkqaxlo.sHtML

chardet.detect(raw)
来源：http://3g.hesvh.cn/Article/details/ghickwzmd.sHtML

[U35] Py：发送邮件
来源：http://wap.hesvh.cn/Article/details/grinzcjhu.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.hesvh.cn/Article/details/gfjzfbgkv.sHtML

[U36] Py：定时任务
来源：http://m.share.fehbvm.com/Article/details/gococjhra.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.zdbjq.cn/Article/details/gnxbpfzbi.sHtML

[U37] Py：读写 Excel
来源：http://blog.hesvh.cn/Article/details/gmyiamfsq.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.fehbvm.com/Article/details/gkkrpizad.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.fehbvm.com/Article/details/ghkywpknv.sHtML

Path(__file__).resolve().parent
来源：http://blog.fehbvm.com/Article/details/gxrlgihps.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.hesvh.cn/Article/details/gsakumsnu.sHtML

sys.stdout.isatty()
来源：http://read.share.zdbjq.cn/Article/details/gahvqmqte.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.fehbvm.com/Article/details/gcsibulhh.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.hesvh.cn/Article/details/gxgjlruif.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.hesvh.cn/Article/details/gtdayvwug.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.fehbvm.com/Article/details/gzwdpmoig.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.zdbjq.cn/Article/details/gzennvmbb.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.hesvh.cn/Article/details/gzrbbaisg.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.hesvh.cn/Article/details/ginmojooy.sHtML

namespace App\Http;
来源：http://blog.hesvh.cn/Article/details/gkhiqzdza.sHtML

[U44] PHP：开启严格类型
来源：http://baike.fehbvm.com/Article/details/gcardbcuj.sHtML

declare(strict_types=1);
来源：http://mobile.zdbjq.cn/Article/details/gdrmghlks.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.hesvh.cn/Article/details/gnhsvsccf.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/ghzncnkei.sHtML

[U46] PHP：可空类型
来源：http://m.share.zdbjq.cn/Article/details/gwdilaiqf.sHtML

?string $name = null
来源：http://blog.hesvh.cn/Article/details/gyybdcxqj.sHtML

[U47] PHP：联合类型
来源：http://read.share.zdbjq.cn/Article/details/ghiudrxtz.sHtML

int|string $id
来源：http://www.share.fehbvm.com/Article/details/gixnxqxqe.sHtML

[U48] PHP：纯枚举
来源：http://read.share.hesvh.cn/Article/details/gwebsyiyq.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.hesvh.cn/Article/details/gomibrbpg.sHtML

[U49] PHP：只读属性
来源：http://m.share.hesvh.cn/Article/details/gmilznoiv.sHtML

public readonly string $name
来源：http://wap.fehbvm.com/Article/details/gldbcrvpf.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.fehbvm.com/Article/details/gdcuwgzoa.sHtML

public function __construct(private int $id) {}
来源：http://blog.hesvh.cn/Article/details/gpdsbbcyr.sHtML

[U51] PHP：数组解构
来源：http://3g.hesvh.cn/Article/details/gaisewjhf.sHtML

[$a, $b] = $arr;
来源：http://www.blog.fehbvm.com/Article/details/gjplapzup.sHtML

[U52] PHP：箭头函数
来源：http://baike.hesvh.cn/Article/details/glolbbcws.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.hesvh.cn/Article/details/gvwqwfizj.sHtML

[U53] PHP：空合并运算符
来源：http://baike.hesvh.cn/Article/details/gkcanpfqr.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.hesvh.cn/Article/details/gydgsjdns.sHtML

[U54] PHP：空安全调用
来源：http://blog.hesvh.cn/Article/details/gkbefdian.sHtML

$obj?->method()
来源：http://www.share.zdbjq.cn/Article/details/gtkyvpicu.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gaminqhdf.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.hesvh.cn/Article/details/gwkikuivp.sHtML

[U56] PHP：命名参数
来源：http://m.share.fehbvm.com/Article/details/gckjpoekl.sHtML

f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/gbtpuvykt.sHtML

[U57] PHP：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gurewsscb.sHtML

"值: {$a}"
来源：http://wap.hesvh.cn/Article/details/gitvrqjpx.sHtML

[U58] PHP：数组三件套
来源：http://m.share.hesvh.cn/Article/details/gmewicwsy.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.zdbjq.cn/Article/details/gzeqijoch.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.fehbvm.com/Article/details/grnnlfxim.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fehbvm.com/Article/details/gifscnntj.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.hesvh.cn/Article/details/gfqhrxujs.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.fehbvm.com/Article/details/gbngngwrt.sHtML

[U61] PHP：正则
来源：http://3g.fehbvm.com/Article/details/gzysmjyvk.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.zdbjq.cn/Article/details/gffoqeftc.sHtML

[U62] PHP：日期对象
来源：http://www.share.hesvh.cn/Article/details/gyjxmsjdv.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.fehbvm.com/Article/details/gqkbspsis.sHtML

[U63] PHP：文件读写
来源：http://wap.fehbvm.com/Article/details/gqpftwabm.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.fehbvm.com/Article/details/gtxzedzmz.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.hesvh.cn/Article/details/gjidiysyb.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.hesvh.cn/Article/details/gqaeobgyo.sHtML

[U65] PHP：会话
来源：http://3g.hesvh.cn/Article/details/gwlhukkyf.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gecmnblvt.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.fehbvm.com/Article/details/goshrnjka.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.zdbjq.cn/Article/details/gyfhlcrlb.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.fehbvm.com/Article/details/gsupldhat.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.zdbjq.cn/Article/details/gkphkiqio.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.hesvh.cn/Article/details/geixxafzj.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.zdbjq.cn/Article/details/gllciuaxk.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.fehbvm.com/Article/details/gyffbwtxi.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.fehbvm.com/Article/details/gfumflarm.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.hesvh.cn/Article/details/gmhcjrusq.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.zdbjq.cn/Article/details/gcsrnquxw.sHtML

[U71] PHP：抛出异常
来源：http://m.share.hesvh.cn/Article/details/gjwtzkepe.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.fehbvm.com/Article/details/gllnonyyz.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.hesvh.cn/Article/details/gqlgxjwez.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.zdbjq.cn/Article/details/gqvcypdrv.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.fehbvm.com/Article/details/gkbamjwam.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.fehbvm.com/Article/details/gnitgarcb.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/ghiafbszp.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.hesvh.cn/Article/details/gwmnbtcrt.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.zdbjq.cn/Article/details/guggssfli.sHtML

composer require psr/container
来源：http://www.blog.hesvh.cn/Article/details/guywypumc.sHtML

[U76] PHP：简单路由
来源：http://blog.zdbjq.cn/Article/details/gjobnswcd.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.fehbvm.com/Article/details/gkeyjtckr.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.fehbvm.com/Article/details/giewpssyb.sHtML

composer require twig/twig
来源：http://blog.fehbvm.com/Article/details/ggorjhnuz.sHtML

[U78] PHP：单元测试
来源：http://www.share.hesvh.cn/Article/details/gjaoprnwp.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.zdbjq.cn/Article/details/gzddcixlx.sHtML

[U79] PHP：静态分析
来源：http://www.share.hesvh.cn/Article/details/gclmtsafe.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.zdbjq.cn/Article/details/grobfnyqw.sHtML

[U80] PHP：代码规范修复
来源：http://blog.hesvh.cn/Article/details/gwewxatsx.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.fehbvm.com/Article/details/gtowdnlbo.sHtML

[U81] JS：初始化项目
来源：http://read.share.zdbjq.cn/Article/details/gsuebkaoq.sHtML

npm init -y;  npm i express
来源：http://www.share.fehbvm.com/Article/details/gtrucwjjj.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.zdbjq.cn/Article/details/gqrmxfefc.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.hesvh.cn/Article/details/glrloeden.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.hesvh.cn/Article/details/gnmvtoxyl.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.hesvh.cn/Article/details/godkjhytu.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.hesvh.cn/Article/details/ggglcljoe.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.fehbvm.com/Article/details/gjnhhdalt.sHtML

[U85] JS：可选链
来源：http://mobile.hesvh.cn/Article/details/gbsjbkohg.sHtML

a?.b?.c
来源：http://mobile.hesvh.cn/Article/details/ghtvmsezi.sHtML

[U86] JS：空值合并
来源：http://www.share.zdbjq.cn/Article/details/gbeuywbnr.sHtML

a ?? b
来源：http://3g.fehbvm.com/Article/details/gyhdfkowt.sHtML

[U87] JS：解构默认值
来源：http://read.share.zdbjq.cn/Article/details/giqjgkfaz.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.fehbvm.com/Article/details/ggwullwhi.sHtML

[U88] JS：对象展开合并
来源：http://m.share.zdbjq.cn/Article/details/gybivvybs.sHtML

{ ...a, ...b }
来源：http://read.share.zdbjq.cn/Article/details/gyodxfivp.sHtML

[U89] JS：数组去重
来源：http://wap.fehbvm.com/Article/details/gcssxjzcb.sHtML

[...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gkxsjwkqb.sHtML

[U90] JS：数字数组排序
来源：http://3g.zdbjq.cn/Article/details/gltskdscw.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/ggqlcxgrp.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.hesvh.cn/Article/details/gricjrzuh.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.fehbvm.com/Article/details/gyqdqlcnx.sHtML

[U92] JS：深拷贝
来源：http://mobile.zdbjq.cn/Article/details/gkmkunbjx.sHtML

structuredClone(obj)
来源：http://read.share.zdbjq.cn/Article/details/grkrmqaik.sHtML


<!-- 参考信息 -->