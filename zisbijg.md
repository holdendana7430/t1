代发 wailian999

[T05] Kotlin：when 表达式
来源：http://mobile.zdbjq.cn/Article/details/gouckqxph.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.zdbjq.cn/Article/details/gulsgehxy.sHtML

[T06] Kotlin：集合映射
来源：http://wap.hesvh.cn/Article/details/gmhoombcp.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.zdbjq.cn/Article/details/gyewyqmmx.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.hesvh.cn/Article/details/gaahvkfks.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.hesvh.cn/Article/details/ggmsmxwwu.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fehbvm.com/Article/details/givsbcpgf.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.hesvh.cn/Article/details/gzqvdsyba.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fehbvm.com/Article/details/gboungeeg.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.zdbjq.cn/Article/details/gzxzmsaqq.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.hesvh.cn/Article/details/gijplmjyt.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fehbvm.com/Article/details/gezwgzjvh.sHtML

[T11] Kotlin：协程
来源：http://www.blog.hesvh.cn/Article/details/gvthirxxc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.zdbjq.cn/Article/details/gdzvydnwg.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.zdbjq.cn/Article/details/gmlckgypo.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.hesvh.cn/Article/details/gvlmnlxrx.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fehbvm.com/Article/details/gnkvwzany.sHtML

val m = mapOf("a" to 1)
来源：http://3g.zdbjq.cn/Article/details/gukjafkrn.sHtML

[T14] Kotlin：循环
来源：http://baike.zdbjq.cn/Article/details/glqfwggxd.sHtML

for (i in 1..10) println(i)
来源：http://read.share.hesvh.cn/Article/details/gxckxhwrf.sHtML

[T15] Kotlin：接口
来源：http://wap.fehbvm.com/Article/details/gyamumryu.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fehbvm.com/Article/details/gxspyhewy.sHtML

[T16] Swift：Hello World
来源：http://www.share.fehbvm.com/Article/details/gnbbtzrkp.sHtML

print("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gojyjcgkv.sHtML

[T17] Swift：变量与常量
来源：http://www.share.zdbjq.cn/Article/details/glviaupxe.sHtML

var a = 1;  let b = 2
来源：http://m.share.hesvh.cn/Article/details/goppkelch.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gtfakjqir.sHtML

"值: \(b)"
来源：http://wap.hesvh.cn/Article/details/gsewehcxx.sHtML

[T19] Swift：可选绑定
来源：http://blog.fehbvm.com/Article/details/gdvkwsvlq.sHtML

if let n = opt { print(n) }
来源：http://baike.zdbjq.cn/Article/details/gncdtdsto.sHtML

[T20] Swift：数组操作
来源：http://wap.hesvh.cn/Article/details/guwvewvmr.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.hesvh.cn/Article/details/gpbctlhzj.sHtML

[T21] Swift：遍历
来源：http://baike.zdbjq.cn/Article/details/ggqrkbnhg.sHtML

for x in a { print(x) }
来源：http://www.m.share.fehbvm.com/Article/details/gbapaxexo.sHtML

[T22] Swift：字典
来源：http://www.share.hesvh.cn/Article/details/gssdsbhwg.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fehbvm.com/Article/details/gfjqsmvrh.sHtML

[T23] Swift：函数
来源：http://m.share.zdbjq.cn/Article/details/gabqqzopx.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gldwjyjec.sHtML

[T24] Swift：闭包
来源：http://baike.hesvh.cn/Article/details/gbpciqhia.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/ggwivdvah.sHtML

[T25] Swift：结构体
来源：http://m.share.hesvh.cn/Article/details/gbmntacio.sHtML

struct P { var x: Int }
来源：http://read.share.fehbvm.com/Article/details/gjbjsnuep.sHtML

[T26] Swift：类与重写
来源：http://3g.zdbjq.cn/Article/details/gpchjwpsn.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fehbvm.com/Article/details/gchijykbb.sHtML

[T27] Swift：错误处理
来源：http://m.share.fehbvm.com/Article/details/gqrulwlug.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.fehbvm.com/Article/details/gcwuknxnx.sHtML

[T28] Swift：枚举
来源：http://read.share.hesvh.cn/Article/details/ghlprskrw.sHtML

enum Color { case red, green }
来源：http://m.share.fehbvm.com/Article/details/gmwlrcwzx.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.hesvh.cn/Article/details/gplbrycqf.sHtML

guard let x = opt else { return }
来源：http://mobile.zdbjq.cn/Article/details/gyzdexatl.sHtML

[T30] Swift：协议
来源：http://m.share.hesvh.cn/Article/details/gpjmsnwwl.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fehbvm.com/Article/details/gdmtsabql.sHtML

[T31] Lua：Hello World
来源：http://m.share.hesvh.cn/Article/details/gnvtsyjmd.sHtML

print("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gflunlphf.sHtML

[T32] Lua：局部变量
来源：http://3g.fehbvm.com/Article/details/gvzjsxtal.sHtML

local a = 1
来源：http://3g.fehbvm.com/Article/details/gxhojcvry.sHtML

[T33] Lua：表（数组）
来源：http://m.share.hesvh.cn/Article/details/gceacqjqi.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.hesvh.cn/Article/details/gftjdomry.sHtML

[T34] Lua：遍历表
来源：http://mobile.hesvh.cn/Article/details/gzhtfwpet.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.hesvh.cn/Article/details/gfpczyutk.sHtML

[T35] Lua：字典表
来源：http://m.share.zdbjq.cn/Article/details/gdlpobjfn.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.fehbvm.com/Article/details/gwrwqvlty.sHtML

[T36] Lua：函数
来源：http://wap.fehbvm.com/Article/details/gwjvyiusb.sHtML

function add(a, b) return a + b end
来源：http://blog.hesvh.cn/Article/details/gfqctbhwy.sHtML

[T37] Lua：字符串拼接
来源：http://blog.fehbvm.com/Article/details/gpuvezdnj.sHtML

"a" .. "b"
来源：http://blog.fehbvm.com/Article/details/ganeapoia.sHtML

[T38] Lua：条件
来源：http://www.blog.zdbjq.cn/Article/details/gusssjyjs.sHtML

if x > 0 then print("正") end
来源：http://wap.zdbjq.cn/Article/details/ggssopyuc.sHtML

[T39] Lua：模式匹配
来源：http://baike.fehbvm.com/Article/details/gzrbkebbl.sHtML

string.find(s, "%d+")
来源：http://mobile.fehbvm.com/Article/details/gyqmnzyxk.sHtML

[T40] Lua：元表
来源：http://read.share.zdbjq.cn/Article/details/gcrrbxrql.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.zdbjq.cn/Article/details/gkohlzgyp.sHtML

[T41] Perl：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gdcywmhds.sHtML

print "Hello\n";
来源：http://blog.fehbvm.com/Article/details/guhvsbwwx.sHtML

[T42] Perl：变量类型
来源：http://baike.hesvh.cn/Article/details/ghakqjfpm.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.zdbjq.cn/Article/details/gajbqiirz.sHtML

[T43] Perl：字符串插值
来源：http://baike.hesvh.cn/Article/details/gafycldnv.sHtML

"值: $a"
来源：http://wap.fehbvm.com/Article/details/griuglqdl.sHtML

[T44] Perl：条件
来源：http://baike.fehbvm.com/Article/details/gsuyetxhf.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.hesvh.cn/Article/details/gzaavazyz.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.fehbvm.com/Article/details/gkwbhepbe.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.fehbvm.com/Article/details/gdzyudqrk.sHtML

[T46] Perl：哈希操作
来源：http://m.share.fehbvm.com/Article/details/gclqalaav.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.hesvh.cn/Article/details/gnnmexxcr.sHtML

[T47] Perl：正则捕获
来源：http://baike.hesvh.cn/Article/details/gmefrmhoz.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.fehbvm.com/Article/details/gvowstgls.sHtML

[T48] Perl：正则替换
来源：http://blog.fehbvm.com/Article/details/gvbmrfywy.sHtML

$s =~ s/old/new/g;
来源：http://3g.zdbjq.cn/Article/details/grqdwqmrn.sHtML

[T49] Perl：函数
来源：http://www.m.share.fehbvm.com/Article/details/gutoqfktj.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/ggwkrzvik.sHtML

[T50] Perl：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gvaybydid.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.hesvh.cn/Article/details/gpsamjkqv.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.zdbjq.cn/Article/details/grvzzboyn.sHtML

[T51] Scala：Hello World
来源：http://mobile.hesvh.cn/Article/details/gcooqnzum.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/gmduicszr.sHtML

[T52] Scala：变量
来源：http://mobile.zdbjq.cn/Article/details/gutawkxpc.sHtML

val a = 1;  var b = 2
来源：http://blog.fehbvm.com/Article/details/gdscfwmtu.sHtML

[T53] Scala：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gxogoxeps.sHtML

s"值: $b"
来源：http://www.blog.hesvh.cn/Article/details/gvejnxozn.sHtML

[T54] Scala：集合映射
来源：http://3g.hesvh.cn/Article/details/gjpgtraiy.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.zdbjq.cn/Article/details/gdyfnlmbb.sHtML

[T55] Scala：集合过滤
来源：http://read.share.zdbjq.cn/Article/details/gghnjiwwz.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.fehbvm.com/Article/details/gorhuiitr.sHtML

[T56] Scala：样例类
来源：http://mobile.fehbvm.com/Article/details/ghphglesn.sHtML

case class User(name: String, age: Int)
来源：http://read.share.hesvh.cn/Article/details/geyykcfes.sHtML

[T57] Scala：模式匹配
来源：http://blog.hesvh.cn/Article/details/goyjmnjsi.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.zdbjq.cn/Article/details/gfgemdfwa.sHtML

[T58] Scala：函数定义
来源：http://wap.hesvh.cn/Article/details/gkjkkxczn.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.hesvh.cn/Article/details/gfcuduvts.sHtML

[T59] Scala：循环
来源：http://www.share.fehbvm.com/Article/details/gdegjpjot.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.zdbjq.cn/Article/details/grjkejinv.sHtML

[T60] Scala：折叠
来源：http://3g.hesvh.cn/Article/details/gzgvgxbbo.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.zdbjq.cn/Article/details/gthzvhqmj.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gddglrswr.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.fehbvm.com/Article/details/gndxmuplc.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gqslsmdcx.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.fehbvm.com/Article/details/gfinkcrgp.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.zdbjq.cn/Article/details/glaebbzsq.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.hesvh.cn/Article/details/gywqojtkw.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.zdbjq.cn/Article/details/gzpopfksc.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.zdbjq.cn/Article/details/gvkxwpljp.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.zdbjq.cn/Article/details/gbrjslzgw.sHtML

[U04] Py：变量调试打印
来源：http://baike.hesvh.cn/Article/details/gzxueathl.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.hesvh.cn/Article/details/gpoqybcuo.sHtML

[U05] Py：列表去重且保序
来源：http://baike.fehbvm.com/Article/details/gosfifiah.sHtML

list(dict.fromkeys(arr))
来源：http://wap.fehbvm.com/Article/details/gbgpyzxuv.sHtML

[U06] Py：合并两个字典
来源：http://3g.hesvh.cn/Article/details/gqwekbrst.sHtML

{**a, **b}
来源：http://wap.zdbjq.cn/Article/details/gjawcjhoe.sHtML

[U07] Py：反转字典键值
来源：http://m.share.zdbjq.cn/Article/details/gkepeqnhq.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.fehbvm.com/Article/details/gjwottrmk.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.fehbvm.com/Article/details/gkvemiiri.sHtML

[y for x in nested for y in x]
来源：http://www.blog.hesvh.cn/Article/details/gpoyagjcf.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.hesvh.cn/Article/details/gzwesviih.sHtML

max(d, key=d.get)
来源：http://baike.zdbjq.cn/Article/details/grhtqyqlh.sHtML

[U10] Py：按值排序字典
来源：http://read.share.zdbjq.cn/Article/details/gdczzwbgx.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.fehbvm.com/Article/details/gudztkjmc.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.hesvh.cn/Article/details/gtdzwntnh.sHtML

(x * 2 for x in arr)
来源：http://wap.hesvh.cn/Article/details/gddnfpkkh.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.zdbjq.cn/Article/details/gfexhprda.sHtML

Counter(arr).most_common(3)
来源：http://read.share.fehbvm.com/Article/details/gkewcwxpr.sHtML

[U13] Py：固定长度队列
来源：http://www.share.fehbvm.com/Article/details/gvszdeoxv.sHtML

deque(maxlen=10)
来源：http://www.blog.zdbjq.cn/Article/details/gbrnecfqv.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.fehbvm.com/Article/details/gqovwipke.sHtML

defaultdict(list)
来源：http://www.share.fehbvm.com/Article/details/gypmtdeku.sHtML

[U15] Py：高精度计时
来源：http://www.share.fehbvm.com/Article/details/gwwgvwiox.sHtML

t = time.perf_counter()
来源：http://3g.hesvh.cn/Article/details/goaeylvgf.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.fehbvm.com/Article/details/gjdfcxsbh.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.zdbjq.cn/Article/details/guvsxibeb.sHtML

[U17] Py：初始化日志
来源：http://mobile.hesvh.cn/Article/details/gentdmfmn.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fehbvm.com/Article/details/geadycwqp.sHtML

[U18] Py：预编译正则
来源：http://m.share.fehbvm.com/Article/details/grjkyjcgw.sHtML

pat = re.compile(r"\d+")
来源：http://blog.zdbjq.cn/Article/details/gpjzqzwpw.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.zdbjq.cn/Article/details/ggvbhlknk.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.fehbvm.com/Article/details/ghqiisulk.sHtML

[U20] Py：缓存函数结果
来源：http://wap.zdbjq.cn/Article/details/gntkpykra.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.fehbvm.com/Article/details/gfymdstrh.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.hesvh.cn/Article/details/ghigfmdmo.sHtML

@contextlib.contextmanager
来源：http://www.share.fehbvm.com/Article/details/gkbmosynx.sHtML

[U22] Py：矩阵转置
来源：http://mobile.hesvh.cn/Article/details/gsjnnsvnf.sHtML

list(zip(*m))
来源：http://www.share.hesvh.cn/Article/details/gebfirvif.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.fehbvm.com/Article/details/gojyqpchn.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.zdbjq.cn/Article/details/gyaxiyfmn.sHtML

[U24] Py：路径操作
来源：http://m.share.fehbvm.com/Article/details/ggtmlvjcw.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.hesvh.cn/Article/details/gekxbajtf.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.fehbvm.com/Article/details/gdslfukse.sHtML

csv.DictReader(f)
来源：http://baike.zdbjq.cn/Article/details/gtxkdhogx.sHtML

[U26] Py：并发下载
来源：http://wap.hesvh.cn/Article/details/gjfleaxhx.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.hesvh.cn/Article/details/gffvxpdej.sHtML

[U27] Py：异步 HTTP
来源：http://wap.hesvh.cn/Article/details/gbhubssaw.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.hesvh.cn/Article/details/gwvkpotqb.sHtML

[U28] Py：类型别名
来源：http://baike.fehbvm.com/Article/details/gamcsbjwb.sHtML

UserId = int
来源：http://baike.hesvh.cn/Article/details/gytszrjbf.sHtML

[U29] Py：属性校验
来源：http://mobile.zdbjq.cn/Article/details/gbyozebwt.sHtML

@property 与 @x.setter 配合
来源：http://baike.zdbjq.cn/Article/details/gvljyxsjw.sHtML

[U30] Py：数据类
来源：http://www.share.zdbjq.cn/Article/details/guuensill.sHtML

@dataclass(slots=True)
来源：http://m.share.zdbjq.cn/Article/details/gbfpvccsd.sHtML

[U31] Py：单测
来源：http://www.blog.fehbvm.com/Article/details/gfiftrvne.sHtML

python -m pytest -q
来源：http://read.share.hesvh.cn/Article/details/gqesjaqla.sHtML

[U32] Py：代码格式化
来源：http://www.share.zdbjq.cn/Article/details/gkfqsrvcb.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.hesvh.cn/Article/details/gingwgate.sHtML

[U33] Py：打包发布
来源：http://www.m.share.hesvh.cn/Article/details/goesfojgs.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.hesvh.cn/Article/details/gjtaskzuq.sHtML

[U34] Py：判断编码
来源：http://wap.fehbvm.com/Article/details/grgoyjjpt.sHtML

chardet.detect(raw)
来源：http://blog.hesvh.cn/Article/details/gvcokdfjp.sHtML

[U35] Py：发送邮件
来源：http://mobile.fehbvm.com/Article/details/gbslhaobk.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.fehbvm.com/Article/details/gqmqbzxhr.sHtML

[U36] Py：定时任务
来源：http://m.share.fehbvm.com/Article/details/gqruyzutx.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.zdbjq.cn/Article/details/gjfsywxjf.sHtML

[U37] Py：读写 Excel
来源：http://m.share.zdbjq.cn/Article/details/gbvxmedyo.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.fehbvm.com/Article/details/gyblmalpn.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.zdbjq.cn/Article/details/gmaimjnze.sHtML

Path(__file__).resolve().parent
来源：http://3g.hesvh.cn/Article/details/gyhdypwfp.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.fehbvm.com/Article/details/gqpevrpdt.sHtML

sys.stdout.isatty()
来源：http://www.blog.zdbjq.cn/Article/details/gqmyjriml.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.fehbvm.com/Article/details/ggsgphyrf.sHtML

print("err", file=sys.stderr)
来源：http://m.share.zdbjq.cn/Article/details/gvdunlflx.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.zdbjq.cn/Article/details/gxrdvotkn.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.fehbvm.com/Article/details/gdjnibkvt.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.hesvh.cn/Article/details/gcgavfoeh.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.hesvh.cn/Article/details/gpvmiwuna.sHtML

[U43] PHP：声明命名空间
来源：http://3g.fehbvm.com/Article/details/gwiclxkmg.sHtML

namespace App\Http;
来源：http://read.share.zdbjq.cn/Article/details/gazydgceo.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.hesvh.cn/Article/details/gmrpokssa.sHtML

declare(strict_types=1);
来源：http://www.blog.hesvh.cn/Article/details/ggntaclgq.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.hesvh.cn/Article/details/gysxjriha.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/ggxdpjwqw.sHtML

[U46] PHP：可空类型
来源：http://m.share.fehbvm.com/Article/details/ghmfepmya.sHtML

?string $name = null
来源：http://www.blog.zdbjq.cn/Article/details/gzultvpcg.sHtML

[U47] PHP：联合类型
来源：http://www.share.fehbvm.com/Article/details/gsvuixizy.sHtML

int|string $id
来源：http://www.m.share.hesvh.cn/Article/details/gjuqlbvvl.sHtML

[U48] PHP：纯枚举
来源：http://wap.fehbvm.com/Article/details/gcnddllpx.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.hesvh.cn/Article/details/gvpsonidb.sHtML

[U49] PHP：只读属性
来源：http://blog.hesvh.cn/Article/details/gfmvamlge.sHtML

public readonly string $name
来源：http://read.share.zdbjq.cn/Article/details/glffofgrp.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.hesvh.cn/Article/details/grydwrvhz.sHtML

public function __construct(private int $id) {}
来源：http://read.share.hesvh.cn/Article/details/gznbbodjg.sHtML

[U51] PHP：数组解构
来源：http://blog.zdbjq.cn/Article/details/gyjvmnvjz.sHtML

[$a, $b] = $arr;
来源：http://wap.hesvh.cn/Article/details/gklfrxrmw.sHtML

[U52] PHP：箭头函数
来源：http://wap.fehbvm.com/Article/details/geymzliqu.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.zdbjq.cn/Article/details/gqqqncmjz.sHtML

[U53] PHP：空合并运算符
来源：http://blog.fehbvm.com/Article/details/gkgekhhmb.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.zdbjq.cn/Article/details/gfmtocpwa.sHtML

[U54] PHP：空安全调用
来源：http://www.share.zdbjq.cn/Article/details/gvfihsjcy.sHtML

$obj?->method()
来源：http://www.share.fehbvm.com/Article/details/gphbnbpwf.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.fehbvm.com/Article/details/gvjvigwze.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.zdbjq.cn/Article/details/gzpxhyvlu.sHtML

[U56] PHP：命名参数
来源：http://www.blog.fehbvm.com/Article/details/gbaofdbim.sHtML

f(a: 1, b: 2)
来源：http://www.share.zdbjq.cn/Article/details/gmevdkcjz.sHtML

[U57] PHP：字符串插值
来源：http://blog.fehbvm.com/Article/details/gyxqqhsro.sHtML

"值: {$a}"
来源：http://3g.zdbjq.cn/Article/details/gmhuuvfwg.sHtML

[U58] PHP：数组三件套
来源：http://wap.hesvh.cn/Article/details/grayximwj.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.zdbjq.cn/Article/details/gnvnghabg.sHtML

[U59] PHP：自定义排序
来源：http://mobile.zdbjq.cn/Article/details/gafvjwmsj.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.hesvh.cn/Article/details/gdvgtmdnj.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.fehbvm.com/Article/details/gokenphzb.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gbijrqpas.sHtML

[U61] PHP：正则
来源：http://3g.zdbjq.cn/Article/details/gvsmxjecg.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.hesvh.cn/Article/details/ghkoexmhz.sHtML

[U62] PHP：日期对象
来源：http://m.share.fehbvm.com/Article/details/gsuxpotqm.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.hesvh.cn/Article/details/gxfgrvtqo.sHtML

[U63] PHP：文件读写
来源：http://3g.hesvh.cn/Article/details/ghueajqja.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.fehbvm.com/Article/details/geiawwdzp.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.fehbvm.com/Article/details/gukawxdbc.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.zdbjq.cn/Article/details/ggzvqbler.sHtML

[U65] PHP：会话
来源：http://m.share.fehbvm.com/Article/details/grmeilcap.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gzsyrykml.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.zdbjq.cn/Article/details/gkwvbmcjk.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.zdbjq.cn/Article/details/gwnbjrwuh.sHtML

[U67] PHP：处理文件上传
来源：http://wap.zdbjq.cn/Article/details/gebyatfmb.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.fehbvm.com/Article/details/gfczdbfwb.sHtML

[U68] PHP：PDO 连接
来源：http://3g.hesvh.cn/Article/details/gtvtlmkdf.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.hesvh.cn/Article/details/gkeedlhqm.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.zdbjq.cn/Article/details/ggyrazban.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.zdbjq.cn/Article/details/gxbmuajmm.sHtML

[U70] PHP：PDO 事务
来源：http://baike.hesvh.cn/Article/details/gklqcrdjw.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.zdbjq.cn/Article/details/gdguhbjxc.sHtML

[U71] PHP：抛出异常
来源：http://3g.hesvh.cn/Article/details/gheojvmkv.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.hesvh.cn/Article/details/gytfratjv.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.zdbjq.cn/Article/details/girgeenzh.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.zdbjq.cn/Article/details/ggsxlbtep.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.zdbjq.cn/Article/details/gdhkvpzht.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.zdbjq.cn/Article/details/grbtqwqzs.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.hesvh.cn/Article/details/gawktbbna.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.fehbvm.com/Article/details/gwqkcvalm.sHtML

[U75] PHP：依赖注入
来源：http://www.share.hesvh.cn/Article/details/gmlwikkxf.sHtML

composer require psr/container
来源：http://www.blog.hesvh.cn/Article/details/gxrnlewbc.sHtML

[U76] PHP：简单路由
来源：http://wap.hesvh.cn/Article/details/gepfibwdu.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.hesvh.cn/Article/details/gwmtkyamg.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.zdbjq.cn/Article/details/gdskegxvy.sHtML

composer require twig/twig
来源：http://mobile.zdbjq.cn/Article/details/gwvjsoqmb.sHtML

[U78] PHP：单元测试
来源：http://baike.fehbvm.com/Article/details/gcwoycrzn.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.hesvh.cn/Article/details/ghsnknetn.sHtML

[U79] PHP：静态分析
来源：http://blog.zdbjq.cn/Article/details/grbjgkdaf.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.zdbjq.cn/Article/details/gjbatjozm.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.zdbjq.cn/Article/details/gciloeoik.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.fehbvm.com/Article/details/gvljgzmym.sHtML

[U81] JS：初始化项目
来源：http://mobile.zdbjq.cn/Article/details/gsvmfqcbn.sHtML

npm init -y;  npm i express
来源：http://www.share.fehbvm.com/Article/details/grqcyexhl.sHtML

[U82] JS：package.json 脚本
来源：http://wap.hesvh.cn/Article/details/gbwuzcwjb.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.zdbjq.cn/Article/details/gjjxznndh.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.hesvh.cn/Article/details/gepktzrkj.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.fehbvm.com/Article/details/gfiwpfece.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.fehbvm.com/Article/details/gnfqzjehx.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.hesvh.cn/Article/details/gjdkhhhjo.sHtML

[U85] JS：可选链
来源：http://www.share.fehbvm.com/Article/details/gmrvhssuq.sHtML

a?.b?.c
来源：http://baike.fehbvm.com/Article/details/gkltbmtst.sHtML

[U86] JS：空值合并
来源：http://www.blog.fehbvm.com/Article/details/gnacufnnk.sHtML

a ?? b
来源：http://www.share.hesvh.cn/Article/details/gqnbffdqw.sHtML

[U87] JS：解构默认值
来源：http://mobile.fehbvm.com/Article/details/gdyvixkac.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.zdbjq.cn/Article/details/grnlgwgis.sHtML

[U88] JS：对象展开合并
来源：http://baike.zdbjq.cn/Article/details/gnqufnyoj.sHtML

{ ...a, ...b }
来源：http://www.m.share.zdbjq.cn/Article/details/gbtdkawst.sHtML

[U89] JS：数组去重
来源：http://wap.fehbvm.com/Article/details/gasccltvi.sHtML

[...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/gxgphuzex.sHtML

[U90] JS：数字数组排序
来源：http://mobile.zdbjq.cn/Article/details/gcibyscdg.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/gnkmwznwl.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.fehbvm.com/Article/details/ghbvcises.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.fehbvm.com/Article/details/ggmgwpdcy.sHtML

[U92] JS：深拷贝
来源：http://wap.zdbjq.cn/Article/details/geclwfkqf.sHtML

structuredClone(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gsushrfff.sHtML


<!-- 参考信息 -->