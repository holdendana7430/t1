代发 wailian999

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2msinlwpf.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2xnasdayu.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2vyfttuky.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2zncuwyeb.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2tlqbzaiz.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2egkicjpd.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2zoihmtwd.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2gxnepkfe.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2tmkozsbx.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2enorkqor.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2nodlyrbz.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2ldcfllku.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2ewejcbzv.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2ctuehuii.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2yyxwbmtr.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2gjjmnsuo.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2hxtglmns.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2nzqzwfbi.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2rmvqmxhq.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ilahxxyt.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2yhgsaydi.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2guteiwkr.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2jgkztafx.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2vmvfgwtr.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2kpochcan.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2cafrygza.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xddavadm.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2bjouihnb.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2njyaxxod.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2obrxoohj.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ecyrzjuq.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2cviqpivt.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2flteiwtt.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2wetsjpfu.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2azwuuhie.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2sbofclke.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2cqdsphiy.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2ucomzebo.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2euypbtro.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2gjwthahh.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2spaxrpty.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2rjltdbxf.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2gvsnfrur.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2rwpeoera.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2znqldshh.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2nnnssyrt.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2mhayerum.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2vcuoxbtg.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2tufcczjo.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2bfwliyta.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2dnsavyen.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2cqgcvioi.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2ubpbdrdx.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2ytkyuxtz.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2ywetdigi.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2ytlfuqaz.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2uqiszyfe.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ykzxryjq.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2fesoxegb.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2sefpilci.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2zeceifgv.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2aogyajgc.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2qjjbmlzg.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2okkddvgz.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2vsyqednh.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2ehoutesu.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2vgqwvhqo.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2ltodcftf.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2sfkgyobi.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2cgvgudnk.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2qvttsoye.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2lacnqxtu.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2ksayqewn.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2ctolwftu.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2jtaeoamf.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2zzbdhuzk.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2boucxkwa.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2pwqrsuof.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2opgooxjr.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2wjocokri.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2vlynrbza.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2cnbdxtjx.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2fllmnste.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vemkhule.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2rjeewgdm.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2zmyrqnaa.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2ymsxvftk.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2znqaxsei.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2hqimnchb.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2cugsuuts.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2xynablef.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2juqsziwj.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2ubgxmkny.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2pciwiqpc.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ejfhufvp.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2ioqhdxvi.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2pggqjokl.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2pnhktlyd.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ceyhcaxr.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2aqfyvaro.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2zpvjaanf.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2qfkwgoik.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2hnymrbiw.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2xiccgwap.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2buakzcfh.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2lrbintdp.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qmrvlytu.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2kaqudcpm.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2fgghuqhs.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2weqmmpmo.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2lzoqazki.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2kgjemvbo.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2adzbawcj.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2rppvjsye.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2bhddqdzg.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2uiqroxji.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2hijwvvuf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ffnjfhun.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2iofnvzsv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2clusybwz.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2vfzcfwcv.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2nsnllmrt.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2ppbxcamk.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2xqbcdtgt.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2xniunwmd.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2vxzklcul.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2shboyqut.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2dhbotviy.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2saymahet.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2jgkuokns.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2eswczmlr.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2phrjsysd.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2usgcozro.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2qpucjywa.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2dtaipnxk.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2tievzeva.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2xynjysnr.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2neqdistg.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2fgjzgmrd.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2gozhlqaa.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2iucyljmn.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2xpmxpzkf.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2isyzshft.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2nckirpyj.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2hycagcep.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2kqlqgfzz.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2vcidbtke.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2yukripdd.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2kpalzaxi.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2ulyiiupw.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2pefcvojg.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2pnvdzimq.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2sxnwrlqc.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2fxhfojdv.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2nkpvgdju.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2rmghqhmr.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2yijpotje.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2dzaaxyql.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2phjcrspp.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2olgzudup.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2zklmexut.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2rswlyqjf.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2wqbrfwip.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2gnpjcxlz.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2wgivyxkm.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2yqmhjdtd.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2vvukeyds.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2rdrlfxci.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2xwksnwyw.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2lqpslvuy.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2nuozayqa.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2tnssmtvu.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2ntukjiap.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2swbdfnwr.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2lwzjzazs.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2ljkexqfz.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2viumzuie.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2ywgqxrmp.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2xkveacdp.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2cocwbnke.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2eltzniai.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2fnowccny.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2cohqaujc.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2ohbhctmf.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2idgfdlqk.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2ycvbjpyu.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2xwftgdry.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2pcjdyvxz.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2dfhsuujw.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2fbwwvkxw.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2hlpkrqir.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2bzmhbrce.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2rutkatox.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2apsbrpmh.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2tqlnjfkz.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2gghvstfz.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2lbkrctjx.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2qjtrulxm.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2jiadavmr.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2rcbrmsqh.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2saoibrgh.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2ikilktey.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2calhbknp.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2deobuqmn.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2gjatmdgy.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2wnnokfrj.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2bskmanei.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2rmqhzpdv.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2freqnmmu.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2edqerysx.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2uxupnujd.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2pnlszohq.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2myykgogp.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2pehnfujt.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2fizaruhi.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uppgbqcc.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2pqhwsckd.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2luoomtup.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2btlnrapt.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2swomztan.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2iadyaejv.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2fhujuknb.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2fkllfpmg.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2ntukljoj.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2jmzxfdih.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2wrzetcie.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2rnpefnuo.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2cfkewqam.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2qofjgchf.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2xrsqhvbz.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2qdscnlpt.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cujisasr.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2wuvuvsmf.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2vszhonlu.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2egajfuuq.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2lhqrowfm.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2btrunshi.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2idmzarmg.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2yhyjvynj.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2qxeakzje.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2cbxsluzb.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2gvulzdgd.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2yhoombve.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2craadfei.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2ndgwjuqt.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2mulajxpe.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2vajgomyi.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2exdpcqdp.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2lyitmszc.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wflvmptx.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2psgzduin.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2sejwmsxq.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2mxspkbtz.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2eeqykcln.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2orsbevnh.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2tczmtwqg.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2xyzwceyc.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2rkfasjat.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2rsgflzpz.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2utwcmfzk.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2eymgkqpt.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2vzsmngrv.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2apxtfsoz.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2wboykngd.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2ftysjmdr.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2hdbcyysk.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ccikvgwo.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2qiomgaiq.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2qstqushy.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2eigeypcu.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2fozjfqgv.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2ajesbets.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2kjsfrbzv.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2sdkgyviv.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2krjhygmu.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2vuhuwmgr.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2zxrysddq.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2sewlqukg.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2mppxupta.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2ftgrfyvm.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2ljipeqsn.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2zljgoucf.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2ajrvacer.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2ysudwemn.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2bjkmlsfl.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2szspegqi.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2xvfsunlm.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2nqqonaut.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2hedtbbpl.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2lcqywdwn.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2phparueb.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2zucpaebz.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2mxeloonm.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2umdtwvvb.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2nfjprzvb.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2xevxxspz.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2mzgmltml.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2wndbfndp.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2eoismcus.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2otlefqug.html


<!-- 参考信息 -->