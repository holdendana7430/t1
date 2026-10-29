代发 wailian999

[T05] Kotlin：when 表达式
来源：http://wap.hesvh.cn/Article/details/gtswgyklp.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.zdbjq.cn/Article/details/gutzwdkzw.sHtML

[T06] Kotlin：集合映射
来源：http://3g.zdbjq.cn/Article/details/ghofdabnb.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.hesvh.cn/Article/details/gyhusdzya.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fehbvm.com/Article/details/gihmfmmjb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fehbvm.com/Article/details/gcsqblake.sHtML

[T08] Kotlin：数据类
来源：http://3g.fehbvm.com/Article/details/gmbanjado.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fehbvm.com/Article/details/gjucovpsz.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.zdbjq.cn/Article/details/gmbbaschz.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fehbvm.com/Article/details/ggarjyfhp.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fehbvm.com/Article/details/gbovxonen.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fehbvm.com/Article/details/gjtkdarpq.sHtML

[T11] Kotlin：协程
来源：http://mobile.hesvh.cn/Article/details/gmqpwcfez.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.hesvh.cn/Article/details/ggdjdhiom.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fehbvm.com/Article/details/gznqkvyrc.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.fehbvm.com/Article/details/ggskryrkv.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.zdbjq.cn/Article/details/gdxxvqccz.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.hesvh.cn/Article/details/gqvgmvbkw.sHtML

[T14] Kotlin：循环
来源：http://wap.hesvh.cn/Article/details/gevfbhiet.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.hesvh.cn/Article/details/gdkfadiaj.sHtML

[T15] Kotlin：接口
来源：http://mobile.fehbvm.com/Article/details/ghqjmnrqj.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.zdbjq.cn/Article/details/ggkkydfxr.sHtML

[T16] Swift：Hello World
来源：http://3g.hesvh.cn/Article/details/gickaltrw.sHtML

print("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gtgidtsqc.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.hesvh.cn/Article/details/gywvlnrfs.sHtML

var a = 1;  let b = 2
来源：http://blog.fehbvm.com/Article/details/gnkehhywc.sHtML

[T18] Swift：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gugxwecoe.sHtML

"值: \(b)"
来源：http://baike.fehbvm.com/Article/details/gvqpquddh.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.zdbjq.cn/Article/details/gwwaxhxvw.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fehbvm.com/Article/details/gmxcrjjky.sHtML

[T20] Swift：数组操作
来源：http://baike.fehbvm.com/Article/details/ggpwngrjs.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.zdbjq.cn/Article/details/gdfmdbest.sHtML

[T21] Swift：遍历
来源：http://www.m.share.fehbvm.com/Article/details/gwqfvnrii.sHtML

for x in a { print(x) }
来源：http://www.blog.hesvh.cn/Article/details/gjmchpurf.sHtML

[T22] Swift：字典
来源：http://www.m.share.hesvh.cn/Article/details/gdxnjuaza.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fehbvm.com/Article/details/gnejxtcim.sHtML

[T23] Swift：函数
来源：http://wap.zdbjq.cn/Article/details/godgfbzsd.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fehbvm.com/Article/details/goexzdlpa.sHtML

[T24] Swift：闭包
来源：http://www.m.share.hesvh.cn/Article/details/gqmcryztn.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.fehbvm.com/Article/details/gfspweher.sHtML

[T25] Swift：结构体
来源：http://blog.hesvh.cn/Article/details/gremaeyxh.sHtML

struct P { var x: Int }
来源：http://blog.fehbvm.com/Article/details/gxombpnxu.sHtML

[T26] Swift：类与重写
来源：http://wap.fehbvm.com/Article/details/ghxhbfubk.sHtML

class A: Base { override func f() {} }
来源：http://read.share.zdbjq.cn/Article/details/gyezjexio.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fehbvm.com/Article/details/ggjajgtpw.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fehbvm.com/Article/details/gpuzqgqvz.sHtML

[T28] Swift：枚举
来源：http://baike.zdbjq.cn/Article/details/gbvlqbrsz.sHtML

enum Color { case red, green }
来源：http://read.share.hesvh.cn/Article/details/grurtkvab.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.zdbjq.cn/Article/details/gzkthmbjx.sHtML

guard let x = opt else { return }
来源：http://www.m.share.fehbvm.com/Article/details/glojdizdr.sHtML

[T30] Swift：协议
来源：http://www.m.share.hesvh.cn/Article/details/gkehyxwvg.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fehbvm.com/Article/details/gsnkgsdol.sHtML

[T31] Lua：Hello World
来源：http://3g.zdbjq.cn/Article/details/gnsjmmbzi.sHtML

print("Hello")
来源：http://blog.zdbjq.cn/Article/details/gmiuqtxmk.sHtML

[T32] Lua：局部变量
来源：http://m.share.fehbvm.com/Article/details/gmrfuxgnt.sHtML

local a = 1
来源：http://blog.fehbvm.com/Article/details/gsrnufrwo.sHtML

[T33] Lua：表（数组）
来源：http://3g.fehbvm.com/Article/details/gjonrfmzx.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fehbvm.com/Article/details/glutazauy.sHtML

[T34] Lua：遍历表
来源：http://m.share.zdbjq.cn/Article/details/gbaxmjjeu.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.hesvh.cn/Article/details/gvbvqlrji.sHtML

[T35] Lua：字典表
来源：http://www.blog.fehbvm.com/Article/details/gucgezzgq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.zdbjq.cn/Article/details/gtosedhdd.sHtML

[T36] Lua：函数
来源：http://baike.hesvh.cn/Article/details/gypoqkfrw.sHtML

function add(a, b) return a + b end
来源：http://wap.hesvh.cn/Article/details/gfhrgluqp.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.hesvh.cn/Article/details/ghzokacdj.sHtML

"a" .. "b"
来源：http://www.blog.zdbjq.cn/Article/details/gpghtabeo.sHtML

[T38] Lua：条件
来源：http://blog.fehbvm.com/Article/details/gfeopeuun.sHtML

if x > 0 then print("正") end
来源：http://baike.zdbjq.cn/Article/details/gutadpflg.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.hesvh.cn/Article/details/gqqbsbads.sHtML

string.find(s, "%d+")
来源：http://www.blog.hesvh.cn/Article/details/gikhqewsi.sHtML

[T40] Lua：元表
来源：http://blog.zdbjq.cn/Article/details/gmbxbcymv.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.hesvh.cn/Article/details/gitxkycwt.sHtML

[T41] Perl：Hello World
来源：http://baike.zdbjq.cn/Article/details/gqfglwpom.sHtML

print "Hello\n";
来源：http://read.share.hesvh.cn/Article/details/gqfklpfvl.sHtML

[T42] Perl：变量类型
来源：http://www.blog.zdbjq.cn/Article/details/gfvmjpxvj.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.zdbjq.cn/Article/details/gwbkgcqsg.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gowouemsd.sHtML

"值: $a"
来源：http://blog.zdbjq.cn/Article/details/gfzqalqjm.sHtML

[T44] Perl：条件
来源：http://www.blog.fehbvm.com/Article/details/grrobloyi.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.zdbjq.cn/Article/details/gayrwczgd.sHtML

[T45] Perl：数组遍历
来源：http://blog.hesvh.cn/Article/details/gzuhrpjfs.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.zdbjq.cn/Article/details/gwsrekbyv.sHtML

[T46] Perl：哈希操作
来源：http://m.share.hesvh.cn/Article/details/gwjffjztj.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.hesvh.cn/Article/details/gxashqljh.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.fehbvm.com/Article/details/gzfbypewv.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fehbvm.com/Article/details/gqevoxcrg.sHtML

[T48] Perl：正则替换
来源：http://read.share.zdbjq.cn/Article/details/gvmsexlwx.sHtML

$s =~ s/old/new/g;
来源：http://mobile.zdbjq.cn/Article/details/glkjvkioh.sHtML

[T49] Perl：函数
来源：http://wap.zdbjq.cn/Article/details/gxivunncz.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gwsvgcrip.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gvaovxtas.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.zdbjq.cn/Article/details/gbovhisjg.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.fehbvm.com/Article/details/gmetdwoyp.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/glcrauhol.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/gxldhkccf.sHtML

[T52] Scala：变量
来源：http://baike.hesvh.cn/Article/details/gxvjirxbx.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.hesvh.cn/Article/details/gstyexvzo.sHtML

[T53] Scala：字符串插值
来源：http://wap.hesvh.cn/Article/details/gctejdqwz.sHtML

s"值: $b"
来源：http://3g.hesvh.cn/Article/details/goncnalwr.sHtML

[T54] Scala：集合映射
来源：http://wap.fehbvm.com/Article/details/gnmmnclhg.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gnzredvye.sHtML

[T55] Scala：集合过滤
来源：http://wap.fehbvm.com/Article/details/gbkyfwkjj.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.fehbvm.com/Article/details/gfueyplpf.sHtML

[T56] Scala：样例类
来源：http://wap.zdbjq.cn/Article/details/gerztkmlw.sHtML

case class User(name: String, age: Int)
来源：http://www.share.zdbjq.cn/Article/details/gmbjfowde.sHtML

[T57] Scala：模式匹配
来源：http://baike.fehbvm.com/Article/details/gffxalusi.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.fehbvm.com/Article/details/gfzshnswu.sHtML

[T58] Scala：函数定义
来源：http://m.share.zdbjq.cn/Article/details/gwvommred.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.fehbvm.com/Article/details/gsjpoapbc.sHtML

[T59] Scala：循环
来源：http://mobile.zdbjq.cn/Article/details/giuptimlp.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.zdbjq.cn/Article/details/gbdradnbc.sHtML

[T60] Scala：折叠
来源：http://read.share.zdbjq.cn/Article/details/gjvhtlndo.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.fehbvm.com/Article/details/gsrclteme.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gnbfooljh.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.hesvh.cn/Article/details/gqjcqzmoh.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/geenghbhw.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.hesvh.cn/Article/details/gcgcbnbyb.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.zdbjq.cn/Article/details/gftgdgied.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.fehbvm.com/Article/details/gekolaoey.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.hesvh.cn/Article/details/giflydasv.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.hesvh.cn/Article/details/ggfhrrici.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.zdbjq.cn/Article/details/galwtksyo.sHtML

[U04] Py：变量调试打印
来源：http://blog.zdbjq.cn/Article/details/gjqermohu.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.hesvh.cn/Article/details/gzfvwmeky.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.fehbvm.com/Article/details/ggoqdnqkd.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.hesvh.cn/Article/details/gctlieiaz.sHtML

[U06] Py：合并两个字典
来源：http://mobile.zdbjq.cn/Article/details/gityqfmuf.sHtML

{**a, **b}
来源：http://3g.zdbjq.cn/Article/details/glizbprxu.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.hesvh.cn/Article/details/gmmnrmnhs.sHtML

{v: k for k, v in d.items()}
来源：http://3g.zdbjq.cn/Article/details/gpdbwomsf.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.hesvh.cn/Article/details/gpmosmdtu.sHtML

[y for x in nested for y in x]
来源：http://blog.zdbjq.cn/Article/details/ghhfrhgeb.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.fehbvm.com/Article/details/goemurbmj.sHtML

max(d, key=d.get)
来源：http://baike.hesvh.cn/Article/details/gxcdqkowl.sHtML

[U10] Py：按值排序字典
来源：http://wap.hesvh.cn/Article/details/glyyagvrc.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.fehbvm.com/Article/details/gtvprkpux.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.fehbvm.com/Article/details/gsasbwayq.sHtML

(x * 2 for x in arr)
来源：http://www.share.fehbvm.com/Article/details/gaunxkict.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.hesvh.cn/Article/details/goqculemk.sHtML

Counter(arr).most_common(3)
来源：http://wap.zdbjq.cn/Article/details/gaskshnkz.sHtML

[U13] Py：固定长度队列
来源：http://baike.fehbvm.com/Article/details/glfuptgcm.sHtML

deque(maxlen=10)
来源：http://mobile.zdbjq.cn/Article/details/gtddszsna.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.zdbjq.cn/Article/details/grxjkuvdu.sHtML

defaultdict(list)
来源：http://www.share.zdbjq.cn/Article/details/gdeyngcho.sHtML

[U15] Py：高精度计时
来源：http://wap.fehbvm.com/Article/details/gnoyjugze.sHtML

t = time.perf_counter()
来源：http://read.share.zdbjq.cn/Article/details/gfrrcsjpa.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.zdbjq.cn/Article/details/goiwdhxxw.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.hesvh.cn/Article/details/gjshdqqyd.sHtML

[U17] Py：初始化日志
来源：http://www.blog.zdbjq.cn/Article/details/ggekmyamx.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.hesvh.cn/Article/details/ggsihvwkr.sHtML

[U18] Py：预编译正则
来源：http://wap.hesvh.cn/Article/details/gwwwmocac.sHtML

pat = re.compile(r"\d+")
来源：http://blog.hesvh.cn/Article/details/gbhtnlozz.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.fehbvm.com/Article/details/gfnfkaihr.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.zdbjq.cn/Article/details/gesjzlhyx.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.hesvh.cn/Article/details/gljgmxouk.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.zdbjq.cn/Article/details/gemgmjkjw.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.fehbvm.com/Article/details/gktsobxkw.sHtML

@contextlib.contextmanager
来源：http://baike.zdbjq.cn/Article/details/guwjktrnz.sHtML

[U22] Py：矩阵转置
来源：http://wap.fehbvm.com/Article/details/gyqgiphqk.sHtML

list(zip(*m))
来源：http://www.m.share.hesvh.cn/Article/details/goukyvjuu.sHtML

[U23] Py：分块读取大文件
来源：http://3g.zdbjq.cn/Article/details/gzeqwoxon.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.zdbjq.cn/Article/details/gjvknfoqr.sHtML

[U24] Py：路径操作
来源：http://www.blog.hesvh.cn/Article/details/giunzcbwe.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.zdbjq.cn/Article/details/gftayywme.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.hesvh.cn/Article/details/gzfdvkkqr.sHtML

csv.DictReader(f)
来源：http://3g.hesvh.cn/Article/details/ghrbtyptx.sHtML

[U26] Py：并发下载
来源：http://3g.zdbjq.cn/Article/details/gxipmzokt.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.zdbjq.cn/Article/details/gatoethkb.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.fehbvm.com/Article/details/grpccvmpa.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.hesvh.cn/Article/details/gpgavlovv.sHtML

[U28] Py：类型别名
来源：http://m.share.zdbjq.cn/Article/details/gexzscjkv.sHtML

UserId = int
来源：http://blog.hesvh.cn/Article/details/gkfpfhwme.sHtML

[U29] Py：属性校验
来源：http://m.share.hesvh.cn/Article/details/gileajhqf.sHtML

@property 与 @x.setter 配合
来源：http://baike.fehbvm.com/Article/details/gzbcywytx.sHtML

[U30] Py：数据类
来源：http://www.share.hesvh.cn/Article/details/guhajrjjx.sHtML

@dataclass(slots=True)
来源：http://baike.zdbjq.cn/Article/details/gjdcehsan.sHtML

[U31] Py：单测
来源：http://www.m.share.zdbjq.cn/Article/details/gxzcwmhdt.sHtML

python -m pytest -q
来源：http://www.share.zdbjq.cn/Article/details/gslzdcwpu.sHtML

[U32] Py：代码格式化
来源：http://read.share.zdbjq.cn/Article/details/guisvyosi.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.fehbvm.com/Article/details/gwpylekhc.sHtML

[U33] Py：打包发布
来源：http://www.m.share.fehbvm.com/Article/details/gtpfoyjny.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.fehbvm.com/Article/details/gosbpeqrw.sHtML

[U34] Py：判断编码
来源：http://read.share.fehbvm.com/Article/details/gofsnkapl.sHtML

chardet.detect(raw)
来源：http://3g.fehbvm.com/Article/details/gzpwknrko.sHtML

[U35] Py：发送邮件
来源：http://www.blog.fehbvm.com/Article/details/ggwgtvqhy.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.fehbvm.com/Article/details/gpnywecsr.sHtML

[U36] Py：定时任务
来源：http://blog.hesvh.cn/Article/details/ghufmeffn.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.hesvh.cn/Article/details/gqzgwncoj.sHtML

[U37] Py：读写 Excel
来源：http://baike.zdbjq.cn/Article/details/gchzbvvjw.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.hesvh.cn/Article/details/gydhwctyi.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.hesvh.cn/Article/details/gurezkxez.sHtML

Path(__file__).resolve().parent
来源：http://wap.zdbjq.cn/Article/details/gwkxwommt.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.hesvh.cn/Article/details/gjfiqvbxu.sHtML

sys.stdout.isatty()
来源：http://wap.hesvh.cn/Article/details/gryndqqht.sHtML

[U40] Py：打印到标准错误
来源：http://wap.fehbvm.com/Article/details/greofikpz.sHtML

print("err", file=sys.stderr)
来源：http://3g.fehbvm.com/Article/details/gzfsceabc.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.hesvh.cn/Article/details/grqlukzwj.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.hesvh.cn/Article/details/gkhbpjeya.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.fehbvm.com/Article/details/gjxgcepcu.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.hesvh.cn/Article/details/girytelgc.sHtML

[U43] PHP：声明命名空间
来源：http://baike.hesvh.cn/Article/details/gvjtvivat.sHtML

namespace App\Http;
来源：http://www.share.hesvh.cn/Article/details/gjkkvapyw.sHtML

[U44] PHP：开启严格类型
来源：http://blog.hesvh.cn/Article/details/gpukekcdy.sHtML

declare(strict_types=1);
来源：http://wap.zdbjq.cn/Article/details/gbzplegny.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.fehbvm.com/Article/details/grflypxep.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gbjfbitqg.sHtML

[U46] PHP：可空类型
来源：http://read.share.fehbvm.com/Article/details/gmgrucjks.sHtML

?string $name = null
来源：http://www.m.share.zdbjq.cn/Article/details/gcsynpotv.sHtML

[U47] PHP：联合类型
来源：http://baike.hesvh.cn/Article/details/gizmvweyz.sHtML

int|string $id
来源：http://read.share.zdbjq.cn/Article/details/gotdbwtwo.sHtML

[U48] PHP：纯枚举
来源：http://blog.fehbvm.com/Article/details/gavvozzyy.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.hesvh.cn/Article/details/gtlqprgjm.sHtML

[U49] PHP：只读属性
来源：http://mobile.zdbjq.cn/Article/details/goyvqkggq.sHtML

public readonly string $name
来源：http://mobile.hesvh.cn/Article/details/gltjrlwpk.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.fehbvm.com/Article/details/geahcmmzq.sHtML

public function __construct(private int $id) {}
来源：http://baike.zdbjq.cn/Article/details/gdveynvrc.sHtML

[U51] PHP：数组解构
来源：http://3g.fehbvm.com/Article/details/geueqiamk.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.hesvh.cn/Article/details/ghpavhpxj.sHtML

[U52] PHP：箭头函数
来源：http://m.share.zdbjq.cn/Article/details/gopjnndut.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.hesvh.cn/Article/details/gjjpyooou.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.zdbjq.cn/Article/details/gacxjuhzf.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.zdbjq.cn/Article/details/ggsxpzcdj.sHtML

[U54] PHP：空安全调用
来源：http://3g.fehbvm.com/Article/details/gcehcqjmo.sHtML

$obj?->method()
来源：http://3g.zdbjq.cn/Article/details/gfandblqw.sHtML

[U55] PHP：match 表达式
来源：http://blog.fehbvm.com/Article/details/grznujouu.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.zdbjq.cn/Article/details/gzwgssnzo.sHtML

[U56] PHP：命名参数
来源：http://blog.hesvh.cn/Article/details/gpyorljmc.sHtML

f(a: 1, b: 2)
来源：http://read.share.hesvh.cn/Article/details/gvunquwnf.sHtML

[U57] PHP：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gkowuaiow.sHtML

"值: {$a}"
来源：http://www.share.zdbjq.cn/Article/details/gbwulcoyt.sHtML

[U58] PHP：数组三件套
来源：http://read.share.zdbjq.cn/Article/details/gyljkiyfw.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.hesvh.cn/Article/details/gyxumsdir.sHtML

[U59] PHP：自定义排序
来源：http://3g.zdbjq.cn/Article/details/ghtjenozf.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fehbvm.com/Article/details/ghccgmjwy.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.zdbjq.cn/Article/details/gybsggylg.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.zdbjq.cn/Article/details/ghfewewxr.sHtML

[U61] PHP：正则
来源：http://baike.zdbjq.cn/Article/details/gexcxbsda.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/girjgmqdh.sHtML

[U62] PHP：日期对象
来源：http://wap.fehbvm.com/Article/details/gptviaxwn.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.fehbvm.com/Article/details/glzisrgyc.sHtML

[U63] PHP：文件读写
来源：http://www.share.hesvh.cn/Article/details/gmepqvnis.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.fehbvm.com/Article/details/gxcpbcvcb.sHtML

[U64] PHP：目录遍历
来源：http://read.share.zdbjq.cn/Article/details/gwyoeasuy.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.zdbjq.cn/Article/details/gduknvjyi.sHtML

[U65] PHP：会话
来源：http://mobile.zdbjq.cn/Article/details/gjzqavjta.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.fehbvm.com/Article/details/gnvznkudw.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.hesvh.cn/Article/details/gdthdzmpn.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.fehbvm.com/Article/details/gjexmnezq.sHtML

[U67] PHP：处理文件上传
来源：http://3g.fehbvm.com/Article/details/gyhihuorm.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.zdbjq.cn/Article/details/gtyxultvn.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.hesvh.cn/Article/details/gkflpqxnh.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.zdbjq.cn/Article/details/guzgakztm.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.hesvh.cn/Article/details/gwljewwqt.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.fehbvm.com/Article/details/gicffjxcj.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.zdbjq.cn/Article/details/govxsbwtd.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.zdbjq.cn/Article/details/gjhkegpbl.sHtML

[U71] PHP：抛出异常
来源：http://wap.hesvh.cn/Article/details/ghfrwthhk.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.fehbvm.com/Article/details/gczswqlzf.sHtML

[U72] PHP：写错误日志
来源：http://baike.zdbjq.cn/Article/details/ggsjtitcf.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.fehbvm.com/Article/details/gyeyghtbz.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.fehbvm.com/Article/details/gmokrbofw.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.hesvh.cn/Article/details/gtzvgffqa.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.fehbvm.com/Article/details/gcvopvery.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.zdbjq.cn/Article/details/gqcygtdph.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.zdbjq.cn/Article/details/gifjqbbzg.sHtML

composer require psr/container
来源：http://wap.fehbvm.com/Article/details/gosplzsge.sHtML

[U76] PHP：简单路由
来源：http://3g.zdbjq.cn/Article/details/gtuyijqai.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.hesvh.cn/Article/details/gleuyxlfc.sHtML

[U77] PHP：模板渲染
来源：http://blog.zdbjq.cn/Article/details/gsudyefst.sHtML

composer require twig/twig
来源：http://www.m.share.fehbvm.com/Article/details/ganlrwwjb.sHtML

[U78] PHP：单元测试
来源：http://baike.zdbjq.cn/Article/details/gfdwfjbuv.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.hesvh.cn/Article/details/giwlzpzlj.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.fehbvm.com/Article/details/gtovpuuct.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.hesvh.cn/Article/details/glrvlhiij.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.zdbjq.cn/Article/details/gdbtefahw.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.hesvh.cn/Article/details/gstvtojxn.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.hesvh.cn/Article/details/gcqoatcfl.sHtML

npm init -y;  npm i express
来源：http://mobile.fehbvm.com/Article/details/gxqzkhqby.sHtML

[U82] JS：package.json 脚本
来源：http://baike.fehbvm.com/Article/details/gyhetxhxl.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.zdbjq.cn/Article/details/gajtcztsd.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.zdbjq.cn/Article/details/gulnlgbku.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.hesvh.cn/Article/details/gplsrxqje.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.fehbvm.com/Article/details/gdpmrlgah.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.zdbjq.cn/Article/details/gsyvagyef.sHtML

[U85] JS：可选链
来源：http://blog.fehbvm.com/Article/details/geucgbxze.sHtML

a?.b?.c
来源：http://blog.fehbvm.com/Article/details/gjgdqhmjv.sHtML

[U86] JS：空值合并
来源：http://mobile.fehbvm.com/Article/details/glzdzhceg.sHtML

a ?? b
来源：http://read.share.zdbjq.cn/Article/details/giwcicpsf.sHtML

[U87] JS：解构默认值
来源：http://www.blog.zdbjq.cn/Article/details/gftinibiy.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.zdbjq.cn/Article/details/gznrpsegh.sHtML

[U88] JS：对象展开合并
来源：http://baike.hesvh.cn/Article/details/gemeerjwl.sHtML

{ ...a, ...b }
来源：http://read.share.hesvh.cn/Article/details/giilkfwpi.sHtML

[U89] JS：数组去重
来源：http://wap.hesvh.cn/Article/details/gjknifisb.sHtML

[...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/gxttzcvbs.sHtML

[U90] JS：数字数组排序
来源：http://www.share.fehbvm.com/Article/details/gsgxcnisc.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gslomwkns.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.fehbvm.com/Article/details/ggqgxbavc.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.hesvh.cn/Article/details/gmzpweenk.sHtML

[U92] JS：深拷贝
来源：http://m.share.zdbjq.cn/Article/details/gpwompxrp.sHtML

structuredClone(obj)
来源：http://baike.zdbjq.cn/Article/details/gatfzosrj.sHtML


<!-- 参考信息 -->