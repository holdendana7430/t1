代发 wailian999

[T03] Kotlin：字符串模板
来源：http://baike.fehbvm.com/Article/details/gnakaeiqo.sHtML

"值: $b"
来源：http://3g.hesvh.cn/Article/details/gcamdrxog.sHtML

[T04] Kotlin：空安全
来源：http://3g.hesvh.cn/Article/details/grkrdytkg.sHtML

val n: String? = null;  n?.length
来源：http://wap.fehbvm.com/Article/details/gbvccsles.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.zdbjq.cn/Article/details/gjbohgebc.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fehbvm.com/Article/details/gsnkvxkne.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fehbvm.com/Article/details/gainbbyzt.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/ghphininj.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.hesvh.cn/Article/details/gxnioeuxt.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fehbvm.com/Article/details/gbadtktfy.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.zdbjq.cn/Article/details/gicxcqvnw.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.hesvh.cn/Article/details/ganzdrson.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.zdbjq.cn/Article/details/gzgqgpafy.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.hesvh.cn/Article/details/gynmozqza.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.hesvh.cn/Article/details/gwnkevijt.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fehbvm.com/Article/details/gahuqtlya.sHtML

[T11] Kotlin：协程
来源：http://mobile.zdbjq.cn/Article/details/gxqgbfsrx.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.zdbjq.cn/Article/details/guzopzeqy.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.zdbjq.cn/Article/details/ghixvhmul.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/ggnsofdox.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.zdbjq.cn/Article/details/guueklbcw.sHtML

val m = mapOf("a" to 1)
来源：http://wap.hesvh.cn/Article/details/gkvlwgcih.sHtML

[T14] Kotlin：循环
来源：http://mobile.hesvh.cn/Article/details/gqlzvflbd.sHtML

for (i in 1..10) println(i)
来源：http://3g.fehbvm.com/Article/details/geuzhyxgl.sHtML

[T15] Kotlin：接口
来源：http://3g.hesvh.cn/Article/details/gcmmzjish.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.zdbjq.cn/Article/details/guxveankc.sHtML

[T16] Swift：Hello World
来源：http://3g.hesvh.cn/Article/details/gswkuuryu.sHtML

print("Hello")
来源：http://baike.hesvh.cn/Article/details/gngvhuipl.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fehbvm.com/Article/details/gdldtutzz.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.hesvh.cn/Article/details/glixadrci.sHtML

[T18] Swift：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gclfhwgfw.sHtML

"值: \(b)"
来源：http://wap.zdbjq.cn/Article/details/gperhrmfw.sHtML

[T19] Swift：可选绑定
来源：http://read.share.zdbjq.cn/Article/details/gyocmhnfg.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.fehbvm.com/Article/details/gccmfgxop.sHtML

[T20] Swift：数组操作
来源：http://baike.fehbvm.com/Article/details/gihjhdcpv.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.zdbjq.cn/Article/details/gxsodpswg.sHtML

[T21] Swift：遍历
来源：http://www.blog.hesvh.cn/Article/details/gjbhxpscx.sHtML

for x in a { print(x) }
来源：http://www.m.share.fehbvm.com/Article/details/gmkdtemzg.sHtML

[T22] Swift：字典
来源：http://www.share.zdbjq.cn/Article/details/gqoprtdbp.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fehbvm.com/Article/details/gsulozlxp.sHtML

[T23] Swift：函数
来源：http://m.share.zdbjq.cn/Article/details/grljdmwtr.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.fehbvm.com/Article/details/gpmwdqdlg.sHtML

[T24] Swift：闭包
来源：http://blog.fehbvm.com/Article/details/gsspgezfy.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.hesvh.cn/Article/details/gjwmghkbt.sHtML

[T25] Swift：结构体
来源：http://m.share.hesvh.cn/Article/details/gnrvooobt.sHtML

struct P { var x: Int }
来源：http://m.share.hesvh.cn/Article/details/gsprrnrsj.sHtML

[T26] Swift：类与重写
来源：http://www.share.hesvh.cn/Article/details/ghtvpcmwh.sHtML

class A: Base { override func f() {} }
来源：http://baike.zdbjq.cn/Article/details/gwfbldqnm.sHtML

[T27] Swift：错误处理
来源：http://m.share.fehbvm.com/Article/details/gedqxrsrz.sHtML

do { try f() } catch { print(error) }
来源：http://3g.hesvh.cn/Article/details/gkmdwbfhc.sHtML

[T28] Swift：枚举
来源：http://blog.hesvh.cn/Article/details/gcwukieaz.sHtML

enum Color { case red, green }
来源：http://www.m.share.zdbjq.cn/Article/details/ghwqypbpe.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.hesvh.cn/Article/details/gcavimdqr.sHtML

guard let x = opt else { return }
来源：http://www.blog.hesvh.cn/Article/details/grtbqudwr.sHtML

[T30] Swift：协议
来源：http://3g.zdbjq.cn/Article/details/gtisrenky.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fehbvm.com/Article/details/gfatiyxxt.sHtML

[T31] Lua：Hello World
来源：http://m.share.hesvh.cn/Article/details/gjggwsdeu.sHtML

print("Hello")
来源：http://www.share.hesvh.cn/Article/details/gtmmpxhbx.sHtML

[T32] Lua：局部变量
来源：http://www.blog.hesvh.cn/Article/details/gjywluysj.sHtML

local a = 1
来源：http://read.share.hesvh.cn/Article/details/gasjnvpuh.sHtML

[T33] Lua：表（数组）
来源：http://m.share.zdbjq.cn/Article/details/gpwlupqtr.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.zdbjq.cn/Article/details/gdfyyplzg.sHtML

[T34] Lua：遍历表
来源：http://read.share.hesvh.cn/Article/details/gjlsbjgjr.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.fehbvm.com/Article/details/gvapzscwa.sHtML

[T35] Lua：字典表
来源：http://read.share.hesvh.cn/Article/details/ghevdiyvw.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.fehbvm.com/Article/details/gjhhwnwfh.sHtML

[T36] Lua：函数
来源：http://www.blog.zdbjq.cn/Article/details/ggiytbieo.sHtML

function add(a, b) return a + b end
来源：http://read.share.hesvh.cn/Article/details/gzsiqjzqk.sHtML

[T37] Lua：字符串拼接
来源：http://wap.hesvh.cn/Article/details/gmknlelwg.sHtML

"a" .. "b"
来源：http://wap.fehbvm.com/Article/details/gwxcgifmp.sHtML

[T38] Lua：条件
来源：http://wap.hesvh.cn/Article/details/ghyynqiet.sHtML

if x > 0 then print("正") end
来源：http://www.share.zdbjq.cn/Article/details/geekuvzhe.sHtML

[T39] Lua：模式匹配
来源：http://blog.fehbvm.com/Article/details/gotytbcxx.sHtML

string.find(s, "%d+")
来源：http://3g.zdbjq.cn/Article/details/gqcfqxzbc.sHtML

[T40] Lua：元表
来源：http://www.m.share.hesvh.cn/Article/details/gdttpklll.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fehbvm.com/Article/details/guxtyozzk.sHtML

[T41] Perl：Hello World
来源：http://blog.zdbjq.cn/Article/details/gfhdgvxsz.sHtML

print "Hello\n";
来源：http://www.blog.fehbvm.com/Article/details/giaqymthu.sHtML

[T42] Perl：变量类型
来源：http://www.share.zdbjq.cn/Article/details/gxfndjkrc.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.fehbvm.com/Article/details/gqvuyxqcy.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gmjhzwtjh.sHtML

"值: $a"
来源：http://baike.hesvh.cn/Article/details/gtbovdzre.sHtML

[T44] Perl：条件
来源：http://read.share.zdbjq.cn/Article/details/gzorpomfv.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.fehbvm.com/Article/details/gzpdxngce.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.fehbvm.com/Article/details/glsuewozt.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.fehbvm.com/Article/details/ggbzvvozb.sHtML

[T46] Perl：哈希操作
来源：http://mobile.hesvh.cn/Article/details/gxlkdqgph.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.fehbvm.com/Article/details/gxlukzkju.sHtML

[T47] Perl：正则捕获
来源：http://3g.hesvh.cn/Article/details/gueilgpre.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.zdbjq.cn/Article/details/gewupxgad.sHtML

[T48] Perl：正则替换
来源：http://3g.zdbjq.cn/Article/details/gttbaugbz.sHtML

$s =~ s/old/new/g;
来源：http://read.share.zdbjq.cn/Article/details/gvoowfhbh.sHtML

[T49] Perl：函数
来源：http://read.share.fehbvm.com/Article/details/gymabhxjr.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/ggoxyxkvz.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gmqqoxuvh.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.hesvh.cn/Article/details/gmyrhuxek.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.hesvh.cn/Article/details/gmxazucyp.sHtML

[T51] Scala：Hello World
来源：http://wap.fehbvm.com/Article/details/gdbwsjkur.sHtML

println("Hello")
来源：http://blog.zdbjq.cn/Article/details/gzyqhxwqf.sHtML

[T52] Scala：变量
来源：http://baike.fehbvm.com/Article/details/gbusqchxc.sHtML

val a = 1;  var b = 2
来源：http://www.share.zdbjq.cn/Article/details/gpkneftym.sHtML

[T53] Scala：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gtpkxfegf.sHtML

s"值: $b"
来源：http://m.share.zdbjq.cn/Article/details/ghatsgmqc.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.fehbvm.com/Article/details/gtntkyrrr.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.fehbvm.com/Article/details/gzsdhwesq.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gtfjdbgch.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.fehbvm.com/Article/details/gbrjuruto.sHtML

[T56] Scala：样例类
来源：http://mobile.hesvh.cn/Article/details/gtscswgbk.sHtML

case class User(name: String, age: Int)
来源：http://read.share.zdbjq.cn/Article/details/genllrfvz.sHtML

[T57] Scala：模式匹配
来源：http://mobile.fehbvm.com/Article/details/gjkbqyago.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.fehbvm.com/Article/details/gdcrkxocn.sHtML

[T58] Scala：函数定义
来源：http://baike.fehbvm.com/Article/details/gvbturlqi.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.hesvh.cn/Article/details/gfrcdmyvz.sHtML

[T59] Scala：循环
来源：http://www.m.share.fehbvm.com/Article/details/gnducqicp.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.hesvh.cn/Article/details/gwyjzlrlw.sHtML

[T60] Scala：折叠
来源：http://3g.zdbjq.cn/Article/details/gxwpjybpn.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.fehbvm.com/Article/details/gisxmiofy.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gktfnfeih.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.hesvh.cn/Article/details/geyjjhtqm.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gndvkdkxx.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.hesvh.cn/Article/details/gwijiyonq.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.hesvh.cn/Article/details/giwzlfsma.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.hesvh.cn/Article/details/ghoawcecx.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.hesvh.cn/Article/details/gnnpenlns.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.zdbjq.cn/Article/details/gacbfiufl.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.fehbvm.com/Article/details/gmnnrntmo.sHtML

[U04] Py：变量调试打印
来源：http://wap.fehbvm.com/Article/details/gifhxcccj.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.hesvh.cn/Article/details/gosrafcyw.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.fehbvm.com/Article/details/gbodhvmgw.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.fehbvm.com/Article/details/gvazmxovp.sHtML

[U06] Py：合并两个字典
来源：http://wap.hesvh.cn/Article/details/gwcbyclqz.sHtML

{**a, **b}
来源：http://baike.zdbjq.cn/Article/details/ghkwcxqbf.sHtML

[U07] Py：反转字典键值
来源：http://www.share.zdbjq.cn/Article/details/gleieukfe.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.hesvh.cn/Article/details/gxrglfifm.sHtML

[U08] Py：展平二维列表
来源：http://m.share.fehbvm.com/Article/details/gsemnoutz.sHtML

[y for x in nested for y in x]
来源：http://www.share.zdbjq.cn/Article/details/gfkygiyyt.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.fehbvm.com/Article/details/giybkccbq.sHtML

max(d, key=d.get)
来源：http://mobile.fehbvm.com/Article/details/gaddiygor.sHtML

[U10] Py：按值排序字典
来源：http://wap.zdbjq.cn/Article/details/gszudvoml.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.hesvh.cn/Article/details/gnxtdtakj.sHtML

[U11] Py：生成器表达式
来源：http://wap.hesvh.cn/Article/details/grqqzzizh.sHtML

(x * 2 for x in arr)
来源：http://www.share.zdbjq.cn/Article/details/gwmquwipj.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.hesvh.cn/Article/details/gcrjlishl.sHtML

Counter(arr).most_common(3)
来源：http://wap.hesvh.cn/Article/details/gskvqzkvj.sHtML

[U13] Py：固定长度队列
来源：http://3g.fehbvm.com/Article/details/gqjbeqtyf.sHtML

deque(maxlen=10)
来源：http://m.share.fehbvm.com/Article/details/gqxwpdowy.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.hesvh.cn/Article/details/gaxuihsie.sHtML

defaultdict(list)
来源：http://blog.fehbvm.com/Article/details/gubeizizo.sHtML

[U15] Py：高精度计时
来源：http://3g.hesvh.cn/Article/details/gxjjtyill.sHtML

t = time.perf_counter()
来源：http://www.blog.fehbvm.com/Article/details/gfnttdvtv.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fehbvm.com/Article/details/geeetwaed.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.zdbjq.cn/Article/details/gjtyqbtay.sHtML

[U17] Py：初始化日志
来源：http://www.share.zdbjq.cn/Article/details/gesldvcbp.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.zdbjq.cn/Article/details/ggfeksccb.sHtML

[U18] Py：预编译正则
来源：http://3g.zdbjq.cn/Article/details/gjjuevakt.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.zdbjq.cn/Article/details/gejjltzkg.sHtML

[U19] Py：正则替换带回调
来源：http://blog.fehbvm.com/Article/details/gubabolay.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.zdbjq.cn/Article/details/gqsoibymo.sHtML

[U20] Py：缓存函数结果
来源：http://3g.fehbvm.com/Article/details/gwgfuxofk.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.hesvh.cn/Article/details/gbmtpholm.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.hesvh.cn/Article/details/ghdokcspc.sHtML

@contextlib.contextmanager
来源：http://3g.fehbvm.com/Article/details/gnrkiudzk.sHtML

[U22] Py：矩阵转置
来源：http://baike.zdbjq.cn/Article/details/gbbqcnans.sHtML

list(zip(*m))
来源：http://3g.hesvh.cn/Article/details/gqsazewnx.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.zdbjq.cn/Article/details/gimrrybdw.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.zdbjq.cn/Article/details/grcmmkzdj.sHtML

[U24] Py：路径操作
来源：http://blog.hesvh.cn/Article/details/gwumvdbwu.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.zdbjq.cn/Article/details/gxaqspxfy.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.hesvh.cn/Article/details/gwupyohfc.sHtML

csv.DictReader(f)
来源：http://3g.hesvh.cn/Article/details/gkhgvvqrr.sHtML

[U26] Py：并发下载
来源：http://read.share.fehbvm.com/Article/details/gulcpnrhu.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.hesvh.cn/Article/details/gfnhesoby.sHtML

[U27] Py：异步 HTTP
来源：http://wap.zdbjq.cn/Article/details/giizvcpnx.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.hesvh.cn/Article/details/gxwfnvadv.sHtML

[U28] Py：类型别名
来源：http://www.share.hesvh.cn/Article/details/giinvxepu.sHtML

UserId = int
来源：http://read.share.zdbjq.cn/Article/details/guwworxwr.sHtML

[U29] Py：属性校验
来源：http://blog.fehbvm.com/Article/details/ggiixegxr.sHtML

@property 与 @x.setter 配合
来源：http://www.share.fehbvm.com/Article/details/gugdykfki.sHtML

[U30] Py：数据类
来源：http://read.share.zdbjq.cn/Article/details/gpefzouyi.sHtML

@dataclass(slots=True)
来源：http://read.share.fehbvm.com/Article/details/gawgqyyxj.sHtML

[U31] Py：单测
来源：http://mobile.fehbvm.com/Article/details/glrbgghoc.sHtML

python -m pytest -q
来源：http://baike.zdbjq.cn/Article/details/gqrgvmyrj.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.fehbvm.com/Article/details/gpafzhnkv.sHtML

ruff format . && ruff check --fix .
来源：http://3g.hesvh.cn/Article/details/gtgslqpem.sHtML

[U33] Py：打包发布
来源：http://wap.zdbjq.cn/Article/details/gdyaiqkhb.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.zdbjq.cn/Article/details/ggiwvyyty.sHtML

[U34] Py：判断编码
来源：http://www.share.fehbvm.com/Article/details/gxyizvtys.sHtML

chardet.detect(raw)
来源：http://3g.zdbjq.cn/Article/details/ghqpoznsb.sHtML

[U35] Py：发送邮件
来源：http://3g.fehbvm.com/Article/details/gkrsvomih.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.hesvh.cn/Article/details/gqpxuelra.sHtML

[U36] Py：定时任务
来源：http://blog.fehbvm.com/Article/details/gucjngmqz.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.hesvh.cn/Article/details/gvxwqbtgr.sHtML

[U37] Py：读写 Excel
来源：http://blog.zdbjq.cn/Article/details/ggynafnpm.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.zdbjq.cn/Article/details/genpewoug.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.fehbvm.com/Article/details/gjlhhhloz.sHtML

Path(__file__).resolve().parent
来源：http://m.share.fehbvm.com/Article/details/gnmbxscqd.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.zdbjq.cn/Article/details/gspydzldg.sHtML

sys.stdout.isatty()
来源：http://wap.zdbjq.cn/Article/details/gztbbwymu.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.zdbjq.cn/Article/details/gcltfoavo.sHtML

print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/grkrwhuon.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.fehbvm.com/Article/details/gilrqovid.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.zdbjq.cn/Article/details/ghnukifyb.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.fehbvm.com/Article/details/gnomrwnov.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.zdbjq.cn/Article/details/gpzlomsfd.sHtML

[U43] PHP：声明命名空间
来源：http://3g.zdbjq.cn/Article/details/gzxznbgwb.sHtML

namespace App\Http;
来源：http://blog.hesvh.cn/Article/details/gkwfmytra.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.fehbvm.com/Article/details/ggvnpoygo.sHtML

declare(strict_types=1);
来源：http://www.share.hesvh.cn/Article/details/gqmdhlfxh.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.hesvh.cn/Article/details/gzctezaem.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/ggndrfabw.sHtML

[U46] PHP：可空类型
来源：http://baike.hesvh.cn/Article/details/gbizowfyf.sHtML

?string $name = null
来源：http://baike.fehbvm.com/Article/details/ggtkfwnpc.sHtML

[U47] PHP：联合类型
来源：http://baike.fehbvm.com/Article/details/gcdvxkxpb.sHtML

int|string $id
来源：http://www.m.share.hesvh.cn/Article/details/ggyhdzjgu.sHtML

[U48] PHP：纯枚举
来源：http://3g.hesvh.cn/Article/details/gknxlnqnf.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.hesvh.cn/Article/details/goteaetwt.sHtML

[U49] PHP：只读属性
来源：http://read.share.hesvh.cn/Article/details/gxficqeig.sHtML

public readonly string $name
来源：http://www.share.hesvh.cn/Article/details/gfyoetpsc.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.zdbjq.cn/Article/details/gycpedmyc.sHtML

public function __construct(private int $id) {}
来源：http://blog.zdbjq.cn/Article/details/gfxdfhefn.sHtML

[U51] PHP：数组解构
来源：http://baike.zdbjq.cn/Article/details/gbccrudeo.sHtML

[$a, $b] = $arr;
来源：http://blog.fehbvm.com/Article/details/grmupcxuk.sHtML

[U52] PHP：箭头函数
来源：http://www.share.fehbvm.com/Article/details/gkyapazpv.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.fehbvm.com/Article/details/gunolsccy.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.hesvh.cn/Article/details/gwvppjxpg.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.zdbjq.cn/Article/details/gxnsobwgw.sHtML

[U54] PHP：空安全调用
来源：http://www.share.hesvh.cn/Article/details/gqbtxzyxd.sHtML

$obj?->method()
来源：http://www.blog.hesvh.cn/Article/details/gcgkilgva.sHtML

[U55] PHP：match 表达式
来源：http://mobile.fehbvm.com/Article/details/gwhqebvcg.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.fehbvm.com/Article/details/gxhmdrzhu.sHtML

[U56] PHP：命名参数
来源：http://blog.zdbjq.cn/Article/details/gwlursegd.sHtML

f(a: 1, b: 2)
来源：http://mobile.zdbjq.cn/Article/details/gxmtvipqf.sHtML

[U57] PHP：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/ghvsgxwho.sHtML

"值: {$a}"
来源：http://wap.zdbjq.cn/Article/details/gcibidtuv.sHtML

[U58] PHP：数组三件套
来源：http://www.share.zdbjq.cn/Article/details/glsfqnhfv.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.fehbvm.com/Article/details/gmrscshby.sHtML

[U59] PHP：自定义排序
来源：http://wap.zdbjq.cn/Article/details/gtrogymuh.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fehbvm.com/Article/details/ggeiudgzg.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.hesvh.cn/Article/details/gusaifwlb.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.hesvh.cn/Article/details/gbodegrnm.sHtML

[U61] PHP：正则
来源：http://baike.hesvh.cn/Article/details/glbpxbgha.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.fehbvm.com/Article/details/gyopyrddu.sHtML

[U62] PHP：日期对象
来源：http://m.share.zdbjq.cn/Article/details/gkqpumbwf.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.zdbjq.cn/Article/details/ggfuudomz.sHtML

[U63] PHP：文件读写
来源：http://wap.hesvh.cn/Article/details/gzkxaikcp.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.zdbjq.cn/Article/details/gotdabqqg.sHtML

[U64] PHP：目录遍历
来源：http://wap.hesvh.cn/Article/details/ghliiifhk.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.zdbjq.cn/Article/details/ghaqcmkfy.sHtML

[U65] PHP：会话
来源：http://www.m.share.hesvh.cn/Article/details/gzdicwgva.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.fehbvm.com/Article/details/gywxkpaob.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.zdbjq.cn/Article/details/gupunatqo.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.fehbvm.com/Article/details/goubtaath.sHtML

[U67] PHP：处理文件上传
来源：http://3g.fehbvm.com/Article/details/gssumvqdp.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.fehbvm.com/Article/details/gadixujkw.sHtML

[U68] PHP：PDO 连接
来源：http://baike.zdbjq.cn/Article/details/gdmcwvuji.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.hesvh.cn/Article/details/gukbwpvco.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.fehbvm.com/Article/details/gumtnjesd.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.fehbvm.com/Article/details/gkvkyhwtb.sHtML

[U70] PHP：PDO 事务
来源：http://baike.hesvh.cn/Article/details/gbtxegtgt.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.zdbjq.cn/Article/details/gffiaatgq.sHtML

[U71] PHP：抛出异常
来源：http://m.share.fehbvm.com/Article/details/gscdiqzff.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.fehbvm.com/Article/details/guyaccmws.sHtML

[U72] PHP：写错误日志
来源：http://mobile.fehbvm.com/Article/details/gozxjatod.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.zdbjq.cn/Article/details/gzhqyfdsb.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.hesvh.cn/Article/details/gnjsrucau.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.zdbjq.cn/Article/details/geouhfdti.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.hesvh.cn/Article/details/ghshlubbi.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.fehbvm.com/Article/details/gwqtacuhh.sHtML

[U75] PHP：依赖注入
来源：http://www.share.fehbvm.com/Article/details/gmnoatiyb.sHtML

composer require psr/container
来源：http://m.share.hesvh.cn/Article/details/gjzmxdbjx.sHtML

[U76] PHP：简单路由
来源：http://read.share.hesvh.cn/Article/details/gtdfrkbvn.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.hesvh.cn/Article/details/gfuisjulv.sHtML

[U77] PHP：模板渲染
来源：http://wap.fehbvm.com/Article/details/glvjmofpr.sHtML

composer require twig/twig
来源：http://www.share.fehbvm.com/Article/details/gxsnlzsru.sHtML

[U78] PHP：单元测试
来源：http://m.share.zdbjq.cn/Article/details/gbpfjvzjx.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.fehbvm.com/Article/details/gourlchtm.sHtML

[U79] PHP：静态分析
来源：http://mobile.fehbvm.com/Article/details/gcznblhhg.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.fehbvm.com/Article/details/glfkgwccn.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.hesvh.cn/Article/details/gsaebtbef.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.zdbjq.cn/Article/details/gumkoetxu.sHtML

[U81] JS：初始化项目
来源：http://3g.fehbvm.com/Article/details/gldtowfwi.sHtML

npm init -y;  npm i express
来源：http://www.blog.fehbvm.com/Article/details/grqeqveqe.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.zdbjq.cn/Article/details/gdcylofac.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.zdbjq.cn/Article/details/glnyhiorf.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.hesvh.cn/Article/details/gfiubthtz.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.zdbjq.cn/Article/details/ghapmrkvt.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.fehbvm.com/Article/details/gmiwnbdbo.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.fehbvm.com/Article/details/gkjgjkqzl.sHtML

[U85] JS：可选链
来源：http://mobile.hesvh.cn/Article/details/gfkzjydmx.sHtML

a?.b?.c
来源：http://read.share.hesvh.cn/Article/details/gkxhgtwdl.sHtML

[U86] JS：空值合并
来源：http://mobile.fehbvm.com/Article/details/ginvihzog.sHtML

a ?? b
来源：http://baike.fehbvm.com/Article/details/gipfslmbm.sHtML

[U87] JS：解构默认值
来源：http://m.share.hesvh.cn/Article/details/gdykwdlas.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.hesvh.cn/Article/details/gnppgpgjj.sHtML

[U88] JS：对象展开合并
来源：http://mobile.hesvh.cn/Article/details/gcuzurnfr.sHtML

{ ...a, ...b }
来源：http://baike.zdbjq.cn/Article/details/gasfqomxe.sHtML

[U89] JS：数组去重
来源：http://wap.zdbjq.cn/Article/details/gwotlytvc.sHtML

[...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/gnknkplbr.sHtML

[U90] JS：数字数组排序
来源：http://www.share.hesvh.cn/Article/details/gkmuplvyu.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gxllfmmsl.sHtML


<!-- 参考信息 -->