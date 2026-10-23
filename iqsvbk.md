代发 wailian999

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3tjioovqk.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3ycejiotz.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3bpsuyuvf.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3gvnrrdgb.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3gzzkhuem.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3qdhjyxqh.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3arsfvwzd.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3jllqaizi.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3atovguob.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3bjusotjm.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3vqowbdsc.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3sbwuoopb.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3yemhgmsl.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3mgddhxlz.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3ihhsqxng.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3pkvqbueh.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3pqrslxrx.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3lnniohiy.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3cmkuxoec.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ipoydsin.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3lemxzpfw.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wkeifhdq.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3hnlgochb.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3vptpxuqz.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3zctuhrhq.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3akvpidnv.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3oxrgljtp.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3cbsnnkvf.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3rgoiendj.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3vfsydbjq.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3evffqxgf.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3grrwjzos.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3dasdlpfg.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3bnsmepzw.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3ojvppzmk.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3hfvfidkv.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3uvtqeufm.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3yhunyjrz.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3vdqmkknr.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3hrondinu.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3mfrtzkgf.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3epgfnioj.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3kyryhsdh.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3nrmrnkbv.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3bugbqkze.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3pdmuwmsv.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3ncbxxhuj.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3zlnomfgh.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3nocsqhjf.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3lupjkdou.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3oevrgyyn.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3gqcpjlio.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3ksnewfzt.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3zpburmcc.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3ljwznwqv.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3sezfnjcy.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3feudykny.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3tmdnwiie.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3ukalfsie.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3dkgyghjh.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3zdkgxoba.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3lkxigjut.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3hgevoxof.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3ijzyuecm.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3zlsedesk.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3gvngsbfg.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3atupyhzg.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3iquijakh.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3gufzmuxk.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3dvmdzgjt.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3alynekyu.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3nfyypeyv.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3yvbqbfbx.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3hzppcfir.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3cpumievn.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3ghflgizz.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3rndpnaar.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3jjvithfc.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3yzzmrqkt.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3vkutaese.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3vfosffbf.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3hnukremr.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3fktceeup.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3oznxhans.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3zejifgsc.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3btdseaeo.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3oujbxcsm.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fufkffrl.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3xlyornsr.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3vcydzvqk.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3urlosynb.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3zdpyiono.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3gbrriaxd.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3yhtpukxy.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3amuclasy.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3chdfvrfo.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3hjpssjfq.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zgdfmabm.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3upmbvaxh.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3yqjoaqvh.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3gfcfhpzc.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3tfytamkj.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3fybxusuf.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3skihhhea.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xfbsqtyj.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3urmgsalp.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3tabktlmb.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3imunpbew.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3rxhjkjxl.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3mcfoglvj.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3hqkzpvlk.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3nytoyylc.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3sedjqfxu.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3xockeomz.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3ottviies.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3thjdklyd.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3sdmfhcbc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gxzexiyj.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3nkpsbjqe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jbqeghzh.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3colviyfw.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3unpnfryx.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3wxnzvtyl.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ivfsfipf.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3pnwvgbla.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3rkvuxjny.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3fpvfcnvb.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3ffdbvxfs.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3nztqjnsw.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3sdhgfumk.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3mmmcumiy.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3dupbncgh.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3dhtsefyn.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3qbiaavhx.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3lktworeq.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3iklzkgui.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3gajdeucp.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3rzsiofxy.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3dqlcdjnc.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3nhhewstw.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3xowazpqh.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3hfwofrap.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3cnbbvshd.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3skqyvbvn.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3hxtlcaoy.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3mqhynzbu.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3zywjxath.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3zuvcvlrz.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3vjwhtcvs.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3qcalmzro.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3wmwufhsk.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3nqnkufjh.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3fsepizvy.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3tmlpefyi.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3pwqtpgki.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3xfzfwrra.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3dthtxxnj.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3pqlpcbmm.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3ojptqepu.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3mqsxnfbg.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3nblfrcyr.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3ikqnpate.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3niahogrg.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3pihbitrs.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3hcnsvsmj.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3oooyrsis.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3ckdhwevz.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3gqvrpfbx.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3daonclti.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3otdlkjrx.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3otjnuiql.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3tjjkofij.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3zqooppti.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3fsieepdx.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3wwykikmp.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3ebmbcrnw.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3uhbooydg.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3uhulhxbw.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3fxwvzogn.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3abkuzgnm.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3kvsohiel.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3rowxwzsu.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3pcmkdngk.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3wquhmdna.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3quwkwsvv.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3nmylypsj.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3bbrhxumm.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3djelpyfb.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3ifzufddg.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3lczxkyec.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3korckytl.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3abptvgnf.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3zmpvugtd.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3xynjctqr.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3grjzfehk.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3seeytfcv.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3uywfnwef.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3dxecqqto.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3shzqalso.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3dawdhcaa.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3tvprhjea.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3ggumyksl.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3irxbjots.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3giflwuzy.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3lmdkgpzk.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3mmydrvbp.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3xcenccqj.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3arwsihca.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3vcirkyfo.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qiariitz.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3hroeyhwu.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3ioeqzzol.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3cqtjycci.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3dzbslklv.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3gcdlobtk.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3pwfcelfh.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3lcashgpb.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3jvwfnieb.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3njaqekmq.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3ipahxrcl.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3ggmqvzry.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3cxoqawbu.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3xjoedrzt.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3jbldrjlf.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3xypoyuip.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3ythtkkev.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3gfwozhdx.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3djpbeeuz.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ayilgytl.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3ixbkxwwv.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3msyyklas.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3yvwundzf.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3mjytcnmg.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3zgafoliz.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3tcxuwljn.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3byhdvdmw.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3kdsqaqun.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3dompaekn.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3bxgomqpq.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3klpbhynl.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3ugzydihv.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xzeevqfw.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3cvqbnijn.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3xdrgjsbb.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3hlbwbsam.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3soshlikm.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3znwkpgyt.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3icwsaqll.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3nnyzfnck.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3lwttmvvd.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3vqruvlvu.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3aqbnybeu.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3lqmqouix.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3cqibsaii.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3vwxqsfqm.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3gygrnabj.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3uwmfidcf.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3yfraxibo.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3ybpysons.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3mnriaysp.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3edzlkmov.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3kwqrktre.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3lmujfvtm.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3iqucsord.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3wmgkkgrb.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3luqxunzu.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3bwqwhqlr.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3vkszkjsx.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3hjragttm.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3gdpibhnp.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3gakricap.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3olqesost.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3lfcauhjb.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3mubsrbbl.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3taygmpbz.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3byvflspw.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3lrpaszdm.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3lymndbos.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3ezbicvll.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3mrtgujxl.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3gplyhtqe.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3palpklfl.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3jggaebza.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3vsffsacp.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3xewpbstm.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3hqbcofbu.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3xeqtpdht.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3zyupklfo.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3waazxrhg.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3jnumgaos.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3vcgowmoi.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3qthhrzoj.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3ptqplkzw.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3fffvivlk.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3eafvnjpj.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3nlbgecbd.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3qdmxnlgx.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3hbbttxqe.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3sgksscic.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3lpdomlgs.html


<!-- 参考信息 -->