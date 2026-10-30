代发 wailian999

[T03] Kotlin：字符串模板
来源：http://read.share.hesvh.cn/Article/details/gzudcdmea.sHtML

"值: $b"
来源：http://baike.hesvh.cn/Article/details/gxiemddjq.sHtML

[T04] Kotlin：空安全
来源：http://mobile.hesvh.cn/Article/details/gdlaeepcf.sHtML

val n: String? = null;  n?.length
来源：http://baike.fehbvm.com/Article/details/gxefzytle.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.hesvh.cn/Article/details/gvctuatta.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fehbvm.com/Article/details/gtvirrknf.sHtML

[T06] Kotlin：集合映射
来源：http://3g.hesvh.cn/Article/details/gsteourvg.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gjtndkfjs.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/gfzocnmmb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fehbvm.com/Article/details/gnwutyata.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.zdbjq.cn/Article/details/gqwklutnh.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fehbvm.com/Article/details/gddcsugtv.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.hesvh.cn/Article/details/gpdcxdlcc.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.hesvh.cn/Article/details/gtamdyexw.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.hesvh.cn/Article/details/ghxtrglnn.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fehbvm.com/Article/details/gsfbudkjh.sHtML

[T11] Kotlin：协程
来源：http://m.share.hesvh.cn/Article/details/gketnrphu.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.hesvh.cn/Article/details/gcegasafa.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.hesvh.cn/Article/details/gnntpdtof.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gceyitxvc.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.zdbjq.cn/Article/details/gzowiimda.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.hesvh.cn/Article/details/gxmcpijly.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.zdbjq.cn/Article/details/ggpupxoch.sHtML

for (i in 1..10) println(i)
来源：http://3g.fehbvm.com/Article/details/gwvceectt.sHtML

[T15] Kotlin：接口
来源：http://read.share.fehbvm.com/Article/details/gnvqupcdk.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fehbvm.com/Article/details/ggtomdmoi.sHtML

[T16] Swift：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gxpxmjnyq.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/gchbjlgsq.sHtML

[T17] Swift：变量与常量
来源：http://www.share.zdbjq.cn/Article/details/ghisrobaf.sHtML

var a = 1;  let b = 2
来源：http://m.share.hesvh.cn/Article/details/guvppmbds.sHtML

[T18] Swift：字符串插值
来源：http://mobile.hesvh.cn/Article/details/ghmexdbft.sHtML

"值: \(b)"
来源：http://baike.zdbjq.cn/Article/details/gldupxblg.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fehbvm.com/Article/details/ghhggindp.sHtML

if let n = opt { print(n) }
来源：http://3g.zdbjq.cn/Article/details/gwjyupzvg.sHtML

[T20] Swift：数组操作
来源：http://wap.hesvh.cn/Article/details/gntetprlb.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.zdbjq.cn/Article/details/gxvsaqwed.sHtML

[T21] Swift：遍历
来源：http://wap.fehbvm.com/Article/details/gakogdzys.sHtML

for x in a { print(x) }
来源：http://baike.fehbvm.com/Article/details/gvrvecndr.sHtML

[T22] Swift：字典
来源：http://mobile.fehbvm.com/Article/details/gtcomcela.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.zdbjq.cn/Article/details/gsadsucpb.sHtML

[T23] Swift：函数
来源：http://www.blog.fehbvm.com/Article/details/guiijaxjm.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.fehbvm.com/Article/details/gntfyggir.sHtML

[T24] Swift：闭包
来源：http://www.share.zdbjq.cn/Article/details/gbkutlfew.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.fehbvm.com/Article/details/gnpdrsywz.sHtML

[T25] Swift：结构体
来源：http://3g.fehbvm.com/Article/details/gbtegcyfv.sHtML

struct P { var x: Int }
来源：http://www.share.hesvh.cn/Article/details/ginivkiza.sHtML

[T26] Swift：类与重写
来源：http://www.share.fehbvm.com/Article/details/gaqatwcks.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fehbvm.com/Article/details/glgqzhmao.sHtML

[T27] Swift：错误处理
来源：http://www.blog.fehbvm.com/Article/details/gdhnegpux.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.hesvh.cn/Article/details/gnkcfwriw.sHtML

[T28] Swift：枚举
来源：http://baike.hesvh.cn/Article/details/gpydvvhqo.sHtML

enum Color { case red, green }
来源：http://read.share.hesvh.cn/Article/details/gbosbsljl.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.fehbvm.com/Article/details/gtgwwuiyh.sHtML

guard let x = opt else { return }
来源：http://www.share.fehbvm.com/Article/details/gahwixztm.sHtML

[T30] Swift：协议
来源：http://www.share.fehbvm.com/Article/details/gcnlivbwg.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.zdbjq.cn/Article/details/gfbomcofh.sHtML

[T31] Lua：Hello World
来源：http://blog.fehbvm.com/Article/details/goxyusprx.sHtML

print("Hello")
来源：http://wap.fehbvm.com/Article/details/gxhhiimug.sHtML

[T32] Lua：局部变量
来源：http://3g.fehbvm.com/Article/details/gnhkkzqzk.sHtML

local a = 1
来源：http://baike.fehbvm.com/Article/details/gkbznktjf.sHtML

[T33] Lua：表（数组）
来源：http://www.share.fehbvm.com/Article/details/gewrkxuez.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.fehbvm.com/Article/details/gwglkroks.sHtML

[T34] Lua：遍历表
来源：http://mobile.hesvh.cn/Article/details/gxfdsohhk.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.zdbjq.cn/Article/details/ghdhdwvvq.sHtML

[T35] Lua：字典表
来源：http://mobile.zdbjq.cn/Article/details/gdsrfdgji.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fehbvm.com/Article/details/guuqotsui.sHtML

[T36] Lua：函数
来源：http://m.share.zdbjq.cn/Article/details/gbeowogtq.sHtML

function add(a, b) return a + b end
来源：http://3g.hesvh.cn/Article/details/gnujqcpcj.sHtML

[T37] Lua：字符串拼接
来源：http://baike.zdbjq.cn/Article/details/gtidrxfgy.sHtML

"a" .. "b"
来源：http://read.share.hesvh.cn/Article/details/gzeqbmebr.sHtML

[T38] Lua：条件
来源：http://blog.fehbvm.com/Article/details/guhexjjgf.sHtML

if x > 0 then print("正") end
来源：http://www.share.hesvh.cn/Article/details/gaqzjgfxs.sHtML

[T39] Lua：模式匹配
来源：http://blog.hesvh.cn/Article/details/giajzfcjp.sHtML

string.find(s, "%d+")
来源：http://wap.fehbvm.com/Article/details/gchnhgjzu.sHtML

[T40] Lua：元表
来源：http://www.blog.fehbvm.com/Article/details/gjumgqnxb.sHtML

setmetatable({}, { __index = base })
来源：http://baike.hesvh.cn/Article/details/gozsvhztl.sHtML

[T41] Perl：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gdtzqruxx.sHtML

print "Hello\n";
来源：http://mobile.zdbjq.cn/Article/details/gkyflhefu.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.fehbvm.com/Article/details/gbzkebdfs.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.zdbjq.cn/Article/details/gikiicxjg.sHtML

[T43] Perl：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gqscfhimk.sHtML

"值: $a"
来源：http://m.share.hesvh.cn/Article/details/gthnmteva.sHtML

[T44] Perl：条件
来源：http://m.share.hesvh.cn/Article/details/gsgkkheef.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.zdbjq.cn/Article/details/gekzzggqt.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.zdbjq.cn/Article/details/gbnvyirno.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.zdbjq.cn/Article/details/gevxywptt.sHtML

[T46] Perl：哈希操作
来源：http://baike.zdbjq.cn/Article/details/gxripkzsf.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.hesvh.cn/Article/details/gpnwshzsq.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.zdbjq.cn/Article/details/gnitvidcr.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.zdbjq.cn/Article/details/gohtlnrwr.sHtML

[T48] Perl：正则替换
来源：http://wap.hesvh.cn/Article/details/gvovbocem.sHtML

$s =~ s/old/new/g;
来源：http://wap.fehbvm.com/Article/details/gxlnwnjxn.sHtML

[T49] Perl：函数
来源：http://mobile.hesvh.cn/Article/details/giaizuqro.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gorwlbnje.sHtML

[T50] Perl：逐行读文件
来源：http://wap.hesvh.cn/Article/details/ggvnuuezb.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.fehbvm.com/Article/details/gaeefmeds.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.hesvh.cn/Article/details/glvnliaeg.sHtML

[T51] Scala：Hello World
来源：http://www.share.hesvh.cn/Article/details/gvwvmljnn.sHtML

println("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gfkvdvekt.sHtML

[T52] Scala：变量
来源：http://mobile.fehbvm.com/Article/details/gccruzgnu.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.hesvh.cn/Article/details/ggkxnqlfg.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fehbvm.com/Article/details/ggswpswtq.sHtML

s"值: $b"
来源：http://blog.hesvh.cn/Article/details/gjpdpqlxy.sHtML

[T54] Scala：集合映射
来源：http://www.share.hesvh.cn/Article/details/genixjasz.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.hesvh.cn/Article/details/gxkodsxzj.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gcljoyafv.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.fehbvm.com/Article/details/gpnrfrqpf.sHtML

[T56] Scala：样例类
来源：http://m.share.zdbjq.cn/Article/details/gdhcygiie.sHtML

case class User(name: String, age: Int)
来源：http://m.share.fehbvm.com/Article/details/ghrfgsnod.sHtML

[T57] Scala：模式匹配
来源：http://wap.fehbvm.com/Article/details/gywppfzwl.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fehbvm.com/Article/details/guootmdfd.sHtML

[T58] Scala：函数定义
来源：http://baike.fehbvm.com/Article/details/geradjstl.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.zdbjq.cn/Article/details/gxlyimcmm.sHtML

[T59] Scala：循环
来源：http://www.m.share.zdbjq.cn/Article/details/gjsaynvdi.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.zdbjq.cn/Article/details/gdjgcycka.sHtML

[T60] Scala：折叠
来源：http://wap.hesvh.cn/Article/details/gjyphzljs.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.hesvh.cn/Article/details/gjyiwfndx.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/grqlipdjd.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.zdbjq.cn/Article/details/gepsxvnrz.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gwqhibbap.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.fehbvm.com/Article/details/gtrlcjphp.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.zdbjq.cn/Article/details/ghrvjnflw.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.zdbjq.cn/Article/details/gdcqippes.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.fehbvm.com/Article/details/gnijwkzwa.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.zdbjq.cn/Article/details/gcwfktgsx.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.hesvh.cn/Article/details/gxyhcmgsa.sHtML

[U04] Py：变量调试打印
来源：http://m.share.hesvh.cn/Article/details/gyxunbfpp.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.zdbjq.cn/Article/details/gxufyapwu.sHtML

[U05] Py：列表去重且保序
来源：http://baike.fehbvm.com/Article/details/gyuzzelce.sHtML

list(dict.fromkeys(arr))
来源：http://baike.zdbjq.cn/Article/details/gfrwerfno.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.zdbjq.cn/Article/details/gzdhmeiiz.sHtML

{**a, **b}
来源：http://baike.fehbvm.com/Article/details/gowcozutd.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.fehbvm.com/Article/details/gyvapukuf.sHtML

{v: k for k, v in d.items()}
来源：http://baike.zdbjq.cn/Article/details/gqdbepksf.sHtML

[U08] Py：展平二维列表
来源：http://m.share.hesvh.cn/Article/details/gecmalefh.sHtML

[y for x in nested for y in x]
来源：http://3g.fehbvm.com/Article/details/gzjzjjhjp.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.hesvh.cn/Article/details/gkihtrgnn.sHtML

max(d, key=d.get)
来源：http://www.blog.zdbjq.cn/Article/details/ghxxdyveg.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.zdbjq.cn/Article/details/gxixaubuf.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.zdbjq.cn/Article/details/gcfkjeebz.sHtML

[U11] Py：生成器表达式
来源：http://mobile.fehbvm.com/Article/details/gwzzafnrr.sHtML

(x * 2 for x in arr)
来源：http://wap.fehbvm.com/Article/details/gewqbavbt.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.fehbvm.com/Article/details/gjjwjtjyl.sHtML

Counter(arr).most_common(3)
来源：http://baike.zdbjq.cn/Article/details/gtdcoqoua.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.hesvh.cn/Article/details/gtsxcgfcd.sHtML

deque(maxlen=10)
来源：http://www.m.share.hesvh.cn/Article/details/gwuzglfml.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.zdbjq.cn/Article/details/gyqwhgixt.sHtML

defaultdict(list)
来源：http://3g.fehbvm.com/Article/details/gwfsizxhm.sHtML

[U15] Py：高精度计时
来源：http://m.share.fehbvm.com/Article/details/gvzznrqxz.sHtML

t = time.perf_counter()
来源：http://3g.hesvh.cn/Article/details/glkwkbmxe.sHtML

[U16] Py：命令行参数解析
来源：http://wap.zdbjq.cn/Article/details/gxojfwwew.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.zdbjq.cn/Article/details/gpkztrssh.sHtML

[U17] Py：初始化日志
来源：http://baike.zdbjq.cn/Article/details/gendlikdr.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.fehbvm.com/Article/details/gipgjfthd.sHtML

[U18] Py：预编译正则
来源：http://blog.hesvh.cn/Article/details/gbkhnzepg.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.zdbjq.cn/Article/details/gcpogshqz.sHtML

[U19] Py：正则替换带回调
来源：http://wap.fehbvm.com/Article/details/gxldkxqju.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.zdbjq.cn/Article/details/gyabziqfz.sHtML

[U20] Py：缓存函数结果
来源：http://wap.hesvh.cn/Article/details/gkmhuxnfr.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.hesvh.cn/Article/details/geajtgvek.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.hesvh.cn/Article/details/gqxzlmwex.sHtML

@contextlib.contextmanager
来源：http://m.share.zdbjq.cn/Article/details/gygsskkwa.sHtML

[U22] Py：矩阵转置
来源：http://read.share.fehbvm.com/Article/details/gldcnuqrv.sHtML

list(zip(*m))
来源：http://wap.zdbjq.cn/Article/details/gpzqmradl.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.hesvh.cn/Article/details/grvuzgcoe.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.hesvh.cn/Article/details/gazjrqlxi.sHtML

[U24] Py：路径操作
来源：http://blog.hesvh.cn/Article/details/ggnakxoqp.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.zdbjq.cn/Article/details/gtllstvob.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.fehbvm.com/Article/details/gkygyaiaw.sHtML

csv.DictReader(f)
来源：http://read.share.zdbjq.cn/Article/details/glcqmumxd.sHtML

[U26] Py：并发下载
来源：http://blog.hesvh.cn/Article/details/gqgbbfpgf.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.fehbvm.com/Article/details/gmtvaxvqn.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.zdbjq.cn/Article/details/gsfztrxuw.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.fehbvm.com/Article/details/gyjzfqrfl.sHtML

[U28] Py：类型别名
来源：http://blog.hesvh.cn/Article/details/guklwhvdt.sHtML

UserId = int
来源：http://mobile.hesvh.cn/Article/details/gijpenjdw.sHtML

[U29] Py：属性校验
来源：http://www.share.fehbvm.com/Article/details/ghtpqsnyt.sHtML

@property 与 @x.setter 配合
来源：http://m.share.fehbvm.com/Article/details/gxhvwlgsw.sHtML

[U30] Py：数据类
来源：http://m.share.zdbjq.cn/Article/details/gduvehboz.sHtML

@dataclass(slots=True)
来源：http://blog.hesvh.cn/Article/details/gxkbobsps.sHtML

[U31] Py：单测
来源：http://3g.fehbvm.com/Article/details/gjoetqtbk.sHtML

python -m pytest -q
来源：http://read.share.fehbvm.com/Article/details/gvygsamjw.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gkyeaewsv.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.fehbvm.com/Article/details/gngooyggi.sHtML

[U33] Py：打包发布
来源：http://wap.fehbvm.com/Article/details/gfiwzpvgv.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.fehbvm.com/Article/details/gyizkzayi.sHtML

[U34] Py：判断编码
来源：http://www.share.fehbvm.com/Article/details/gkbcwxwbm.sHtML

chardet.detect(raw)
来源：http://m.share.zdbjq.cn/Article/details/ghesfvwbl.sHtML

[U35] Py：发送邮件
来源：http://3g.fehbvm.com/Article/details/gukdaiwnh.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.hesvh.cn/Article/details/gdwlkkuvr.sHtML

[U36] Py：定时任务
来源：http://baike.zdbjq.cn/Article/details/gecdstyfi.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.zdbjq.cn/Article/details/gobmnrlsf.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.zdbjq.cn/Article/details/goqwfkfbq.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.fehbvm.com/Article/details/gaambicwo.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fehbvm.com/Article/details/gobgszghs.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.zdbjq.cn/Article/details/gehmhicte.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.zdbjq.cn/Article/details/gtcxmxnhz.sHtML

sys.stdout.isatty()
来源：http://3g.hesvh.cn/Article/details/gdorekzim.sHtML

[U40] Py：打印到标准错误
来源：http://blog.hesvh.cn/Article/details/gqqgaoguh.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.zdbjq.cn/Article/details/gvjjutbip.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.zdbjq.cn/Article/details/guavowhvl.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.zdbjq.cn/Article/details/gbbwmzino.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.hesvh.cn/Article/details/gogimuodw.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.hesvh.cn/Article/details/gciprsbkl.sHtML

[U43] PHP：声明命名空间
来源：http://3g.fehbvm.com/Article/details/gkqaijvzc.sHtML

namespace App\Http;
来源：http://www.share.fehbvm.com/Article/details/gjmeybmby.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.fehbvm.com/Article/details/gnpfuhhji.sHtML

declare(strict_types=1);
来源：http://read.share.hesvh.cn/Article/details/gfmrndpeg.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.zdbjq.cn/Article/details/gsoaqwaxm.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gssfbojef.sHtML

[U46] PHP：可空类型
来源：http://m.share.hesvh.cn/Article/details/giwfvkurc.sHtML

?string $name = null
来源：http://www.share.fehbvm.com/Article/details/gktwypddr.sHtML

[U47] PHP：联合类型
来源：http://3g.zdbjq.cn/Article/details/ghzubudrk.sHtML

int|string $id
来源：http://baike.fehbvm.com/Article/details/gftwfdoyt.sHtML

[U48] PHP：纯枚举
来源：http://www.share.fehbvm.com/Article/details/gjjobbmxh.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.hesvh.cn/Article/details/gwqgrcpzx.sHtML

[U49] PHP：只读属性
来源：http://wap.hesvh.cn/Article/details/gxyoxpfhb.sHtML

public readonly string $name
来源：http://baike.zdbjq.cn/Article/details/giubuzzsk.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.hesvh.cn/Article/details/gahljgyic.sHtML

public function __construct(private int $id) {}
来源：http://read.share.zdbjq.cn/Article/details/gliyquert.sHtML

[U51] PHP：数组解构
来源：http://wap.zdbjq.cn/Article/details/gzbfyapse.sHtML

[$a, $b] = $arr;
来源：http://m.share.zdbjq.cn/Article/details/gpxqukcvk.sHtML

[U52] PHP：箭头函数
来源：http://mobile.fehbvm.com/Article/details/geauanxgy.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.zdbjq.cn/Article/details/gelgyybtq.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.fehbvm.com/Article/details/gfnpvkxeb.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.hesvh.cn/Article/details/gbpwmovoz.sHtML

[U54] PHP：空安全调用
来源：http://m.share.hesvh.cn/Article/details/gwkjsuixd.sHtML

$obj?->method()
来源：http://mobile.fehbvm.com/Article/details/gmdyfjxwc.sHtML

[U55] PHP：match 表达式
来源：http://m.share.fehbvm.com/Article/details/gekqrjbow.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.hesvh.cn/Article/details/gihnmebpp.sHtML

[U56] PHP：命名参数
来源：http://www.blog.hesvh.cn/Article/details/gilxlcdxn.sHtML

f(a: 1, b: 2)
来源：http://mobile.hesvh.cn/Article/details/ginsdkufj.sHtML

[U57] PHP：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gwqbsypsy.sHtML

"值: {$a}"
来源：http://3g.zdbjq.cn/Article/details/gfxpwcrji.sHtML

[U58] PHP：数组三件套
来源：http://wap.zdbjq.cn/Article/details/giqgitssp.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.hesvh.cn/Article/details/godafjfcv.sHtML

[U59] PHP：自定义排序
来源：http://3g.fehbvm.com/Article/details/gjskmfstv.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.hesvh.cn/Article/details/gpqbkjogf.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.zdbjq.cn/Article/details/grqkzinqv.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.fehbvm.com/Article/details/gsbpgzpss.sHtML

[U61] PHP：正则
来源：http://m.share.zdbjq.cn/Article/details/gamghxuvx.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.hesvh.cn/Article/details/gpuhoiavx.sHtML

[U62] PHP：日期对象
来源：http://read.share.hesvh.cn/Article/details/gyslcpedn.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.zdbjq.cn/Article/details/gfiyppqbz.sHtML

[U63] PHP：文件读写
来源：http://mobile.hesvh.cn/Article/details/godhxepbj.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.hesvh.cn/Article/details/gyulenpxb.sHtML

[U64] PHP：目录遍历
来源：http://blog.fehbvm.com/Article/details/grvlfeokk.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.hesvh.cn/Article/details/gogiowiqq.sHtML

[U65] PHP：会话
来源：http://3g.hesvh.cn/Article/details/gvmwmzrdq.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gfpaaqwjc.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.fehbvm.com/Article/details/gltyflvzd.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.fehbvm.com/Article/details/gigkewkin.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.hesvh.cn/Article/details/gktngdizg.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.hesvh.cn/Article/details/gztuthvka.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.hesvh.cn/Article/details/grgmafwya.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.hesvh.cn/Article/details/gtilmskag.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.zdbjq.cn/Article/details/gbsoyhysy.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.hesvh.cn/Article/details/gbzwaggru.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.hesvh.cn/Article/details/guvoiclxo.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.zdbjq.cn/Article/details/glcsjnfmv.sHtML

[U71] PHP：抛出异常
来源：http://mobile.fehbvm.com/Article/details/gsiwuyfkb.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.hesvh.cn/Article/details/gnayoutyq.sHtML

[U72] PHP：写错误日志
来源：http://baike.zdbjq.cn/Article/details/gusssmzna.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.zdbjq.cn/Article/details/gyegjjzpv.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.zdbjq.cn/Article/details/gllotacha.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.hesvh.cn/Article/details/ghijtlejv.sHtML

[U74] PHP：读取环境变量
来源：http://baike.zdbjq.cn/Article/details/grpvplorp.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.fehbvm.com/Article/details/gxnxyjili.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.zdbjq.cn/Article/details/givgoigqp.sHtML

composer require psr/container
来源：http://3g.hesvh.cn/Article/details/gcnhdtxfa.sHtML

[U76] PHP：简单路由
来源：http://www.blog.fehbvm.com/Article/details/grfsdoiem.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.zdbjq.cn/Article/details/gqlnmsfgy.sHtML

[U77] PHP：模板渲染
来源：http://read.share.fehbvm.com/Article/details/godnrkews.sHtML

composer require twig/twig
来源：http://baike.fehbvm.com/Article/details/gpzxuirdf.sHtML

[U78] PHP：单元测试
来源：http://blog.zdbjq.cn/Article/details/gvyifpxzp.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.hesvh.cn/Article/details/glxqzoldy.sHtML

[U79] PHP：静态分析
来源：http://wap.fehbvm.com/Article/details/gkmmmauxa.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.fehbvm.com/Article/details/gkkclioua.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.fehbvm.com/Article/details/gqvhpjgle.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.hesvh.cn/Article/details/ggrgvcfhn.sHtML

[U81] JS：初始化项目
来源：http://www.blog.hesvh.cn/Article/details/gesofryzi.sHtML

npm init -y;  npm i express
来源：http://m.share.hesvh.cn/Article/details/gioazhkfj.sHtML

[U82] JS：package.json 脚本
来源：http://wap.zdbjq.cn/Article/details/glzzbuytn.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.hesvh.cn/Article/details/gyadydydu.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.fehbvm.com/Article/details/gsamniyjl.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.hesvh.cn/Article/details/gulsqjluj.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.hesvh.cn/Article/details/goqpoumqp.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.zdbjq.cn/Article/details/ghmydzntm.sHtML

[U85] JS：可选链
来源：http://wap.fehbvm.com/Article/details/gtffeaxuy.sHtML

a?.b?.c
来源：http://www.share.hesvh.cn/Article/details/gsvsroazb.sHtML

[U86] JS：空值合并
来源：http://read.share.hesvh.cn/Article/details/gttjrshpf.sHtML

a ?? b
来源：http://m.share.zdbjq.cn/Article/details/grnavtmjn.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.hesvh.cn/Article/details/gjdqabpvo.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.hesvh.cn/Article/details/gvlvovoox.sHtML

[U88] JS：对象展开合并
来源：http://wap.hesvh.cn/Article/details/gbltqiufj.sHtML

{ ...a, ...b }
来源：http://www.blog.hesvh.cn/Article/details/guzazdznx.sHtML

[U89] JS：数组去重
来源：http://blog.hesvh.cn/Article/details/gvtnprezn.sHtML

[...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/gkgypryue.sHtML

[U90] JS：数字数组排序
来源：http://blog.zdbjq.cn/Article/details/gstjqftpi.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/gzqmdcqwv.sHtML


<!-- 参考信息 -->