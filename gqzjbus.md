代发 wailian999

[T03] Kotlin：字符串模板
来源：http://www.m.share.fehbvm.com/Article/details/gtidpbisk.sHtML

"值: $b"
来源：http://3g.hesvh.cn/Article/details/gndetgagk.sHtML

[T04] Kotlin：空安全
来源：http://baike.zdbjq.cn/Article/details/ggadnxbxm.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fehbvm.com/Article/details/gzlunfesm.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fehbvm.com/Article/details/gqcnribvi.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.hesvh.cn/Article/details/gtslggrma.sHtML

[T06] Kotlin：集合映射
来源：http://blog.zdbjq.cn/Article/details/gohhvqryb.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.hesvh.cn/Article/details/gwzioajvn.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/gxciasrzr.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.zdbjq.cn/Article/details/gmnczomos.sHtML

[T08] Kotlin：数据类
来源：http://wap.hesvh.cn/Article/details/geycsxewn.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.hesvh.cn/Article/details/gtbhmdrch.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.hesvh.cn/Article/details/gzhtupwov.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fehbvm.com/Article/details/gqyxoxrjx.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fehbvm.com/Article/details/gqhxvkmiq.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.hesvh.cn/Article/details/gkdlodkfp.sHtML

[T11] Kotlin：协程
来源：http://read.share.hesvh.cn/Article/details/guzxeickj.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.zdbjq.cn/Article/details/gvzsrssjm.sHtML

[T12] Kotlin：解构声明
来源：http://blog.zdbjq.cn/Article/details/guxxcqdea.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/gmqjiepxn.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.zdbjq.cn/Article/details/gzjscbkyc.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.hesvh.cn/Article/details/gmtsbdbea.sHtML

[T14] Kotlin：循环
来源：http://m.share.hesvh.cn/Article/details/gcimqpytm.sHtML

for (i in 1..10) println(i)
来源：http://m.share.hesvh.cn/Article/details/gvrnspffb.sHtML

[T15] Kotlin：接口
来源：http://www.blog.zdbjq.cn/Article/details/gqcejmepl.sHtML

interface Shape { fun area(): Double }
来源：http://blog.hesvh.cn/Article/details/gdjuthsod.sHtML

[T16] Swift：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gwluahrae.sHtML

print("Hello")
来源：http://wap.hesvh.cn/Article/details/ggucaqsps.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.zdbjq.cn/Article/details/gugkvphmn.sHtML

var a = 1;  let b = 2
来源：http://wap.zdbjq.cn/Article/details/gnmxkbxnw.sHtML

[T18] Swift：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gjzwoeyqw.sHtML

"值: \(b)"
来源：http://baike.fehbvm.com/Article/details/gmfjpmlef.sHtML

[T19] Swift：可选绑定
来源：http://read.share.hesvh.cn/Article/details/gbhqhluhw.sHtML

if let n = opt { print(n) }
来源：http://www.blog.zdbjq.cn/Article/details/gyrrybibm.sHtML

[T20] Swift：数组操作
来源：http://3g.zdbjq.cn/Article/details/gssvdmjun.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fehbvm.com/Article/details/gkmnhdueb.sHtML

[T21] Swift：遍历
来源：http://www.blog.zdbjq.cn/Article/details/gdtttrmod.sHtML

for x in a { print(x) }
来源：http://read.share.fehbvm.com/Article/details/guysatego.sHtML

[T22] Swift：字典
来源：http://3g.fehbvm.com/Article/details/ghkpsklsw.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fehbvm.com/Article/details/grgqzsvpa.sHtML

[T23] Swift：函数
来源：http://blog.zdbjq.cn/Article/details/gbkmwbcsc.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.hesvh.cn/Article/details/gwmmiyesr.sHtML

[T24] Swift：闭包
来源：http://baike.fehbvm.com/Article/details/gkxjrefvh.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gpstegcam.sHtML

[T25] Swift：结构体
来源：http://m.share.zdbjq.cn/Article/details/gofrxjaqz.sHtML

struct P { var x: Int }
来源：http://blog.fehbvm.com/Article/details/galperugq.sHtML

[T26] Swift：类与重写
来源：http://wap.hesvh.cn/Article/details/gcqnpdopn.sHtML

class A: Base { override func f() {} }
来源：http://wap.fehbvm.com/Article/details/gkyqqepfq.sHtML

[T27] Swift：错误处理
来源：http://m.share.fehbvm.com/Article/details/ghbjsazkq.sHtML

do { try f() } catch { print(error) }
来源：http://blog.zdbjq.cn/Article/details/greyjvbup.sHtML

[T28] Swift：枚举
来源：http://baike.hesvh.cn/Article/details/gccdnkeex.sHtML

enum Color { case red, green }
来源：http://read.share.fehbvm.com/Article/details/gtamfdolj.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.hesvh.cn/Article/details/gnjtggvxu.sHtML

guard let x = opt else { return }
来源：http://blog.fehbvm.com/Article/details/gcegbbuwl.sHtML

[T30] Swift：协议
来源：http://mobile.fehbvm.com/Article/details/gezceotsj.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.zdbjq.cn/Article/details/gmnxswous.sHtML

[T31] Lua：Hello World
来源：http://read.share.hesvh.cn/Article/details/gwumiiskx.sHtML

print("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gvmkbzedf.sHtML

[T32] Lua：局部变量
来源：http://read.share.fehbvm.com/Article/details/gwatvzyzj.sHtML

local a = 1
来源：http://mobile.fehbvm.com/Article/details/gwatdmrqv.sHtML

[T33] Lua：表（数组）
来源：http://blog.zdbjq.cn/Article/details/gcaamlfqs.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fehbvm.com/Article/details/gtbbhywcm.sHtML

[T34] Lua：遍历表
来源：http://wap.zdbjq.cn/Article/details/glaiymtmf.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.fehbvm.com/Article/details/grtvurfor.sHtML

[T35] Lua：字典表
来源：http://www.share.zdbjq.cn/Article/details/gqrrcwtua.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.hesvh.cn/Article/details/gczmtmhuv.sHtML

[T36] Lua：函数
来源：http://www.share.zdbjq.cn/Article/details/gjpklazui.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.fehbvm.com/Article/details/gnwzrkeig.sHtML

[T37] Lua：字符串拼接
来源：http://baike.fehbvm.com/Article/details/gfgkwkrlm.sHtML

"a" .. "b"
来源：http://3g.hesvh.cn/Article/details/gxlohysdv.sHtML

[T38] Lua：条件
来源：http://m.share.hesvh.cn/Article/details/gdmgyvjzo.sHtML

if x > 0 then print("正") end
来源：http://mobile.fehbvm.com/Article/details/gabawikoy.sHtML

[T39] Lua：模式匹配
来源：http://mobile.fehbvm.com/Article/details/gncfmdvzm.sHtML

string.find(s, "%d+")
来源：http://www.blog.fehbvm.com/Article/details/gxbgcudrv.sHtML

[T40] Lua：元表
来源：http://www.m.share.fehbvm.com/Article/details/guywpvylb.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.fehbvm.com/Article/details/gbwhhbhyp.sHtML

[T41] Perl：Hello World
来源：http://wap.fehbvm.com/Article/details/gstyivxad.sHtML

print "Hello\n";
来源：http://blog.hesvh.cn/Article/details/gdpamxfgx.sHtML

[T42] Perl：变量类型
来源：http://read.share.zdbjq.cn/Article/details/gajfcnaxy.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.hesvh.cn/Article/details/gbzsxwhjd.sHtML

[T43] Perl：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gardhrntg.sHtML

"值: $a"
来源：http://baike.hesvh.cn/Article/details/gynbrmyfm.sHtML

[T44] Perl：条件
来源：http://mobile.zdbjq.cn/Article/details/gtssrhyst.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.fehbvm.com/Article/details/gtsszksts.sHtML

[T45] Perl：数组遍历
来源：http://m.share.zdbjq.cn/Article/details/gbumabxje.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.hesvh.cn/Article/details/gepjahpxv.sHtML

[T46] Perl：哈希操作
来源：http://wap.fehbvm.com/Article/details/gjjypfldw.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.fehbvm.com/Article/details/gicmuxvgo.sHtML

[T47] Perl：正则捕获
来源：http://read.share.hesvh.cn/Article/details/gjeoqxmbf.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.fehbvm.com/Article/details/gqkrlbtyo.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.hesvh.cn/Article/details/ggufobcpl.sHtML

$s =~ s/old/new/g;
来源：http://www.share.zdbjq.cn/Article/details/gjvnmwblu.sHtML

[T49] Perl：函数
来源：http://baike.zdbjq.cn/Article/details/gomnxgruv.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gnrfvkggw.sHtML

[T50] Perl：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gviryeuip.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.fehbvm.com/Article/details/gccbnisty.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.fehbvm.com/Article/details/gpbrwbqbh.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gzcjcdjoz.sHtML

println("Hello")
来源：http://mobile.hesvh.cn/Article/details/ghleftonr.sHtML

[T52] Scala：变量
来源：http://wap.zdbjq.cn/Article/details/grqhebhpg.sHtML

val a = 1;  var b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gnjkjtubk.sHtML

[T53] Scala：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gqayhidma.sHtML

s"值: $b"
来源：http://read.share.fehbvm.com/Article/details/gzgumuviy.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.fehbvm.com/Article/details/gidwvpchb.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.hesvh.cn/Article/details/gisspsyxi.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.fehbvm.com/Article/details/gussdlikw.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.zdbjq.cn/Article/details/guvthpqey.sHtML

[T56] Scala：样例类
来源：http://mobile.zdbjq.cn/Article/details/gdzczsjyp.sHtML

case class User(name: String, age: Int)
来源：http://baike.hesvh.cn/Article/details/ggmupqeer.sHtML

[T57] Scala：模式匹配
来源：http://www.share.fehbvm.com/Article/details/gybogatye.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.fehbvm.com/Article/details/gvnrihpnp.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.hesvh.cn/Article/details/gxnlsxagz.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.hesvh.cn/Article/details/grtdvfhty.sHtML

[T59] Scala：循环
来源：http://mobile.hesvh.cn/Article/details/gqptmvtao.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.zdbjq.cn/Article/details/glcupcygo.sHtML

[T60] Scala：折叠
来源：http://read.share.hesvh.cn/Article/details/gukadglkx.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.hesvh.cn/Article/details/gknpiqdno.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gqvzwodsc.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.zdbjq.cn/Article/details/gpjhmuuly.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/garlqlytu.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.fehbvm.com/Article/details/gejqyofjw.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.fehbvm.com/Article/details/gssngbtye.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.fehbvm.com/Article/details/gzlozhdzb.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.zdbjq.cn/Article/details/gqfnxxirn.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.hesvh.cn/Article/details/gpisokurn.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.fehbvm.com/Article/details/gsmdyqayn.sHtML

[U04] Py：变量调试打印
来源：http://mobile.zdbjq.cn/Article/details/gfpqvqscr.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.zdbjq.cn/Article/details/gciwuinqz.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.hesvh.cn/Article/details/geubnfgce.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.fehbvm.com/Article/details/gahgiftcf.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fehbvm.com/Article/details/ggkvegbya.sHtML

{**a, **b}
来源：http://mobile.hesvh.cn/Article/details/gxqqzzyiu.sHtML

[U07] Py：反转字典键值
来源：http://mobile.fehbvm.com/Article/details/gjfpzgbvr.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.hesvh.cn/Article/details/gucmhjmtv.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.zdbjq.cn/Article/details/gmmxoqqog.sHtML

[y for x in nested for y in x]
来源：http://3g.fehbvm.com/Article/details/gqoaiqegb.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.hesvh.cn/Article/details/glmlkbuxv.sHtML

max(d, key=d.get)
来源：http://read.share.fehbvm.com/Article/details/gfultrrhq.sHtML

[U10] Py：按值排序字典
来源：http://m.share.hesvh.cn/Article/details/gfyxrjysq.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.fehbvm.com/Article/details/gkyvumjkr.sHtML

[U11] Py：生成器表达式
来源：http://wap.fehbvm.com/Article/details/gvrbqgoac.sHtML

(x * 2 for x in arr)
来源：http://m.share.zdbjq.cn/Article/details/gclvzobqt.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.fehbvm.com/Article/details/glryhuace.sHtML

Counter(arr).most_common(3)
来源：http://www.share.zdbjq.cn/Article/details/griqzjhdj.sHtML

[U13] Py：固定长度队列
来源：http://m.share.zdbjq.cn/Article/details/gczoptart.sHtML

deque(maxlen=10)
来源：http://m.share.zdbjq.cn/Article/details/gmgbzhwrb.sHtML

[U14] Py：分组收集到列表
来源：http://3g.fehbvm.com/Article/details/giaotbmyu.sHtML

defaultdict(list)
来源：http://www.blog.fehbvm.com/Article/details/glhdifzwh.sHtML

[U15] Py：高精度计时
来源：http://blog.zdbjq.cn/Article/details/gxuxltjdh.sHtML

t = time.perf_counter()
来源：http://wap.fehbvm.com/Article/details/goodovwlc.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.zdbjq.cn/Article/details/gnekiehtc.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.zdbjq.cn/Article/details/gybqarzui.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.zdbjq.cn/Article/details/grleohnyv.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.fehbvm.com/Article/details/giwndwqin.sHtML

[U18] Py：预编译正则
来源：http://3g.fehbvm.com/Article/details/gkmycwzcg.sHtML

pat = re.compile(r"\d+")
来源：http://3g.zdbjq.cn/Article/details/gxrithsox.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.zdbjq.cn/Article/details/gxjjusppd.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.fehbvm.com/Article/details/gjcdykutk.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.fehbvm.com/Article/details/gpszakksy.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.hesvh.cn/Article/details/gyccftaoy.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.fehbvm.com/Article/details/goduykyjh.sHtML

@contextlib.contextmanager
来源：http://read.share.zdbjq.cn/Article/details/ghhksrtww.sHtML

[U22] Py：矩阵转置
来源：http://blog.hesvh.cn/Article/details/gqelldggq.sHtML

list(zip(*m))
来源：http://3g.fehbvm.com/Article/details/gflhuszvd.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.hesvh.cn/Article/details/gmlxrivya.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.fehbvm.com/Article/details/gfgrymdot.sHtML

[U24] Py：路径操作
来源：http://www.blog.hesvh.cn/Article/details/gvimmpyeh.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.fehbvm.com/Article/details/gficnzdai.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.hesvh.cn/Article/details/gswpvijrc.sHtML

csv.DictReader(f)
来源：http://3g.hesvh.cn/Article/details/geqejfpwp.sHtML

[U26] Py：并发下载
来源：http://3g.hesvh.cn/Article/details/gxqfgueoy.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.hesvh.cn/Article/details/gcifzqelg.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fehbvm.com/Article/details/giahefgbv.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.hesvh.cn/Article/details/gtppwslst.sHtML

[U28] Py：类型别名
来源：http://www.blog.fehbvm.com/Article/details/gfndohthc.sHtML

UserId = int
来源：http://3g.zdbjq.cn/Article/details/gwecbskas.sHtML

[U29] Py：属性校验
来源：http://mobile.fehbvm.com/Article/details/gebpmyunv.sHtML

@property 与 @x.setter 配合
来源：http://blog.fehbvm.com/Article/details/gtbgdaaax.sHtML

[U30] Py：数据类
来源：http://www.blog.hesvh.cn/Article/details/gwoshlovc.sHtML

@dataclass(slots=True)
来源：http://www.blog.fehbvm.com/Article/details/gfbzklbco.sHtML

[U31] Py：单测
来源：http://3g.fehbvm.com/Article/details/grvlripox.sHtML

python -m pytest -q
来源：http://blog.zdbjq.cn/Article/details/gtnlzniaz.sHtML

[U32] Py：代码格式化
来源：http://www.blog.zdbjq.cn/Article/details/gcfodkqvv.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.fehbvm.com/Article/details/glbwthozm.sHtML

[U33] Py：打包发布
来源：http://www.m.share.zdbjq.cn/Article/details/gfflntdpt.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.zdbjq.cn/Article/details/gkimakhgk.sHtML

[U34] Py：判断编码
来源：http://www.blog.zdbjq.cn/Article/details/gidogetlc.sHtML

chardet.detect(raw)
来源：http://www.blog.zdbjq.cn/Article/details/gezedgqwc.sHtML

[U35] Py：发送邮件
来源：http://www.blog.zdbjq.cn/Article/details/gaolvxvpx.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.zdbjq.cn/Article/details/gaottkmnh.sHtML

[U36] Py：定时任务
来源：http://www.blog.hesvh.cn/Article/details/glbswfapn.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.fehbvm.com/Article/details/gwxftqrgn.sHtML

[U37] Py：读写 Excel
来源：http://wap.fehbvm.com/Article/details/gkmmusrnr.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.zdbjq.cn/Article/details/gjbselyay.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.hesvh.cn/Article/details/geloxpxqf.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.zdbjq.cn/Article/details/gxplhvjbg.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.fehbvm.com/Article/details/glkzebjot.sHtML

sys.stdout.isatty()
来源：http://mobile.zdbjq.cn/Article/details/gawgpjvmj.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.fehbvm.com/Article/details/gpcpmxilm.sHtML

print("err", file=sys.stderr)
来源：http://wap.zdbjq.cn/Article/details/gvldkbokh.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.hesvh.cn/Article/details/gtygozbkd.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.fehbvm.com/Article/details/gobgfivsf.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.zdbjq.cn/Article/details/gsxjfjndt.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.fehbvm.com/Article/details/gecesyadr.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.zdbjq.cn/Article/details/galqaqfnw.sHtML

namespace App\Http;
来源：http://www.m.share.zdbjq.cn/Article/details/ggogrwcoe.sHtML

[U44] PHP：开启严格类型
来源：http://blog.hesvh.cn/Article/details/gisyyiwqz.sHtML

declare(strict_types=1);
来源：http://www.share.hesvh.cn/Article/details/gqcggqotx.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.hesvh.cn/Article/details/gfefmyfap.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gguyfmpys.sHtML

[U46] PHP：可空类型
来源：http://wap.fehbvm.com/Article/details/gjilpuvvn.sHtML

?string $name = null
来源：http://www.blog.zdbjq.cn/Article/details/gflnakdkl.sHtML

[U47] PHP：联合类型
来源：http://m.share.fehbvm.com/Article/details/gwndxonxr.sHtML

int|string $id
来源：http://www.share.zdbjq.cn/Article/details/gamcdylli.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.fehbvm.com/Article/details/gzqugqfey.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.hesvh.cn/Article/details/gllsuqeyd.sHtML

[U49] PHP：只读属性
来源：http://mobile.zdbjq.cn/Article/details/gysgeawxe.sHtML

public readonly string $name
来源：http://read.share.zdbjq.cn/Article/details/gbyumtotk.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.zdbjq.cn/Article/details/gglgcikiv.sHtML

public function __construct(private int $id) {}
来源：http://read.share.fehbvm.com/Article/details/gjughpvrg.sHtML

[U51] PHP：数组解构
来源：http://m.share.zdbjq.cn/Article/details/gcgakgutn.sHtML

[$a, $b] = $arr;
来源：http://blog.fehbvm.com/Article/details/gxemfomxi.sHtML

[U52] PHP：箭头函数
来源：http://blog.zdbjq.cn/Article/details/gmqxvpyxg.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.hesvh.cn/Article/details/gxjvnfxvn.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.fehbvm.com/Article/details/gdzgzmbpa.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.fehbvm.com/Article/details/gffqjadld.sHtML

[U54] PHP：空安全调用
来源：http://www.share.fehbvm.com/Article/details/gdesldeyt.sHtML

$obj?->method()
来源：http://www.m.share.fehbvm.com/Article/details/gfmmuondh.sHtML

[U55] PHP：match 表达式
来源：http://mobile.hesvh.cn/Article/details/gbltptzqm.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.zdbjq.cn/Article/details/gpxmwzkaw.sHtML

[U56] PHP：命名参数
来源：http://baike.fehbvm.com/Article/details/ganontomv.sHtML

f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/gtogcbuux.sHtML

[U57] PHP：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gnimppvwt.sHtML

"值: {$a}"
来源：http://blog.hesvh.cn/Article/details/gfcamvzfl.sHtML

[U58] PHP：数组三件套
来源：http://3g.hesvh.cn/Article/details/gmbtbvdhs.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.fehbvm.com/Article/details/gheniqrva.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.zdbjq.cn/Article/details/gtlbgteyv.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fehbvm.com/Article/details/grwirtefn.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.fehbvm.com/Article/details/gwdhteklr.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.zdbjq.cn/Article/details/gtydbttmv.sHtML

[U61] PHP：正则
来源：http://read.share.hesvh.cn/Article/details/gzemmtkao.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.hesvh.cn/Article/details/gqiijffhp.sHtML

[U62] PHP：日期对象
来源：http://wap.zdbjq.cn/Article/details/gothhdltl.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.zdbjq.cn/Article/details/gzalvuwnf.sHtML

[U63] PHP：文件读写
来源：http://baike.hesvh.cn/Article/details/gdaawnfvi.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.hesvh.cn/Article/details/gzlorgeyk.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.fehbvm.com/Article/details/gbzurxzpw.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.hesvh.cn/Article/details/gzjfxfzsw.sHtML

[U65] PHP：会话
来源：http://3g.fehbvm.com/Article/details/ggdsxnnaw.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gjviolobv.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.fehbvm.com/Article/details/gmrwntxlx.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.hesvh.cn/Article/details/goymnudrm.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.hesvh.cn/Article/details/goqmjjfga.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.fehbvm.com/Article/details/gntaryess.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.fehbvm.com/Article/details/gsuoofsfx.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.zdbjq.cn/Article/details/gwrgacwwu.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.zdbjq.cn/Article/details/gptgrfuhe.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.hesvh.cn/Article/details/gfjcdqltm.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.hesvh.cn/Article/details/gghtsxzst.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.hesvh.cn/Article/details/gspqqrqzl.sHtML

[U71] PHP：抛出异常
来源：http://blog.fehbvm.com/Article/details/ggzravwjf.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.fehbvm.com/Article/details/gbfvhjddz.sHtML

[U72] PHP：写错误日志
来源：http://wap.hesvh.cn/Article/details/gulfttfyz.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.zdbjq.cn/Article/details/ggubnvqjm.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.hesvh.cn/Article/details/gpljjgvkx.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.fehbvm.com/Article/details/gqfgywawo.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.hesvh.cn/Article/details/gjvwpekvz.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.fehbvm.com/Article/details/gmhfjmjmr.sHtML

[U75] PHP：依赖注入
来源：http://read.share.fehbvm.com/Article/details/gvqbnzrem.sHtML

composer require psr/container
来源：http://blog.fehbvm.com/Article/details/gvyrnlsao.sHtML

[U76] PHP：简单路由
来源：http://read.share.zdbjq.cn/Article/details/gsgoiuwds.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.fehbvm.com/Article/details/gamyzbasw.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.fehbvm.com/Article/details/gwiomtavb.sHtML

composer require twig/twig
来源：http://baike.zdbjq.cn/Article/details/goelobzlb.sHtML

[U78] PHP：单元测试
来源：http://baike.hesvh.cn/Article/details/gsggohaos.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.zdbjq.cn/Article/details/ghvonqhds.sHtML

[U79] PHP：静态分析
来源：http://wap.fehbvm.com/Article/details/guvapfpmp.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.hesvh.cn/Article/details/gyeybahtr.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.zdbjq.cn/Article/details/gqnyiaczd.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.zdbjq.cn/Article/details/giebsjqtw.sHtML

[U81] JS：初始化项目
来源：http://m.share.zdbjq.cn/Article/details/gkfdrtohf.sHtML

npm init -y;  npm i express
来源：http://www.m.share.fehbvm.com/Article/details/guudqjiqw.sHtML

[U82] JS：package.json 脚本
来源：http://blog.fehbvm.com/Article/details/gbildekpk.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.fehbvm.com/Article/details/gaappuscj.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.zdbjq.cn/Article/details/ghzqnsvjy.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.hesvh.cn/Article/details/gacstrjlk.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.zdbjq.cn/Article/details/gyfqaaxwj.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.hesvh.cn/Article/details/gpvodmwxo.sHtML

[U85] JS：可选链
来源：http://3g.fehbvm.com/Article/details/gicbbppdp.sHtML

a?.b?.c
来源：http://www.m.share.hesvh.cn/Article/details/gdenovlal.sHtML

[U86] JS：空值合并
来源：http://www.blog.hesvh.cn/Article/details/gqrakzcdm.sHtML

a ?? b
来源：http://3g.fehbvm.com/Article/details/gczwtnvsr.sHtML

[U87] JS：解构默认值
来源：http://mobile.zdbjq.cn/Article/details/gvdhefvgf.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.zdbjq.cn/Article/details/gezoiuekt.sHtML

[U88] JS：对象展开合并
来源：http://www.share.hesvh.cn/Article/details/gjvqyimpm.sHtML

{ ...a, ...b }
来源：http://m.share.zdbjq.cn/Article/details/gzuxxcwtb.sHtML

[U89] JS：数组去重
来源：http://www.m.share.hesvh.cn/Article/details/gtsjfarpk.sHtML

[...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/gqezimhbn.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.zdbjq.cn/Article/details/glwzjjemk.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/geytxsggc.sHtML


<!-- 参考信息 -->