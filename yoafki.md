代发 wailian999

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2lcgkqewf.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2eojezzhi.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2kxuwsxwl.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2flymeocl.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2vdpyvkcn.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2jxyqwuey.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2tgbpmrch.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2qkqascju.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2lpdzgxja.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2oldbmxmz.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2hyegefbh.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2nivctxgj.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2ulkolqiq.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2oobqiscv.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2jempktnv.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2yuyjpoex.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2voothmsp.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2ebsgdeqk.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2yjffzcdg.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2oxivlhrx.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2psfeahuk.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2sryfpihi.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2ndukfegv.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ddfmcrdg.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2oablwpqu.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2knznbxnk.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2kfprefza.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2tequggzq.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2bpmpdpqt.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2flqwogre.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ymeixjuk.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2mrgaugkh.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2dkhkdrmp.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2vtbvafpr.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2bifetxrx.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2qwtkfxhu.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2fjgkqzhh.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2sezvwijn.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2hadeggpn.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2ggbesdfg.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2wecbmhqc.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2cbbzahqv.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2zqflezpo.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2upepeczy.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2xprlvoew.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2bbamblwn.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2herazbbr.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2zimfemad.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2irnvdvwl.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2emvudgzu.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2aqifzpwe.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2hehslkoo.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2stnbowwf.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2hjhohiqn.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2kflqnwum.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2zxmutwjk.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2pwprpdzt.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2rdfxhboh.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2hynwdnpp.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2dgiqncrd.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2tyclqisl.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2sysjrlua.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2fmuawkyb.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2ortdsyar.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2imlwnbtf.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2lzrawpnh.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2lwnqqcua.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2scysibkj.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2yxnklplg.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2yiuqpqym.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2bvrqxnua.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2lwyxpaqb.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2lwcavjvq.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2zdswqbxd.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2yfjxvfsp.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2ituccalo.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vcnliuow.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2qncgussd.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2gycmmwzy.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2hwglbojl.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2kakbyosm.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2ybdpzfei.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2pgqhlavv.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ycbtweac.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2wbebyldp.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2ihujtctf.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2uwbvjiva.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2zosmbgoe.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2gxobkqne.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2rrojvzxg.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2cmqjvgqj.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2tpyrtqiw.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2lfghgeqk.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2osfzdtiq.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2oabezrtr.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2faxwlbqi.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2imkiuxua.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2iyfbqthl.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2yvlwmjyv.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2djpwiiyx.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2frdrmgkc.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ymmnpbca.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2uvfsjdmu.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2edajuonq.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zeqspqhd.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2dusefvhf.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vjalglap.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2xtynyohc.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2utiaapcb.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2lwanfgov.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2mtrqyfrx.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2xrcktgyb.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2peolitai.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2hzqsfxpz.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2uyucjvmh.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2mqfauxqc.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2xfacynli.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hrobuuib.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2tzpiohes.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2derzkmmp.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2prvmrpjw.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2ytnwozja.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2xfcrpzwu.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2fawdxszb.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2nstmgids.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2nqjddevy.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2glagpape.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2wcecvthv.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2hzyonkdx.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2lxvltiix.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2clybslcx.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2qmudlrpp.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2azpigpii.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2qsexgwen.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2dlrxcrpq.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2bnvpddhj.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2kzjhwuuv.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2bhejxeuz.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2dnfwviti.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2mkaklqdv.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2tuzicpuu.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wfkfhfbf.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2untopcoh.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2jgyhdaoc.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2pmzcfqzi.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2kqsqouir.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2zhmzpqnj.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2fncgbniv.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2pbvafltj.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2xtihaurc.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2kbnatvlb.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2nwkchlkr.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2bbtgixui.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2ryqmtoqo.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2vzvzngaz.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2mnajwnhk.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2xdfdnroy.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2trbfnwou.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2ovptgffb.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2wglfilah.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2vfgbnocu.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2ubteegww.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2yfjfbkof.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2dxyftyle.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2epttxkqr.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2hjnoybzx.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2fcpuwuaq.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2gfogdcsu.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2clbhyanw.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2myyylrdk.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2nqfkmajd.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2bbvvtqen.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2frkborcj.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2lshypawc.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2indvhoav.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2mlgnvmrb.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2jzrafabp.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2zuznbryq.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2iblohjiy.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2tspycfyf.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2mozfuomt.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2pqxtcmng.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2owglhexl.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2intvqnde.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2drdkxebq.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2hdkaoont.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2hxlepaem.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2vgzqyozh.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2myizxsjo.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2xxdacjxm.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2gwteygjg.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2bwntanba.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2kzaspjjt.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2ucxycula.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2iqpbufox.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2uzdyuneu.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2iyoliypc.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2varztqvk.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2lznhyquf.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2zmkjtznt.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2apyyjsnv.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2wlixjvll.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2yiowdkeg.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2biplrhib.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2mrhsgvsu.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2gsomgtna.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2udtnrlvf.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2dnrkicuu.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2eijyqdah.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dwdaahcb.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2cadrogbr.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2nokskrra.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2tjdfjcgo.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2eujcnvox.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2krovvxqb.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zbvtnkxo.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2pmtpjcej.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2obwhwbgb.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2mlbtutnc.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2cfqcswzr.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2zgomfnrb.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2gzzwljwz.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2ubavbggj.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2wwnxalxa.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2xcaiikef.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2cftjhfvy.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2zmwiticg.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2wmrcaxbx.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2lraipjsq.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2smqnfmps.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2ozpvueit.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2fvqtmbyd.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2outcbtlv.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2bhdupnxl.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2nhrzikzb.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2qnxrwksx.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2ldzymjlg.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ebxymxcj.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2ghlulepo.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2jbvmzled.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2mgmuejek.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2rfndtlpm.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2bskkxprw.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2cvqdbcqc.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2rkelnfrp.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2wmjoeboz.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2cnmlpwnn.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2ynhmyykh.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2tetoxreu.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2gqmiqkbn.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2czreuoyb.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2vmlsabef.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2fkncvhqe.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2fqztbjrd.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2xyvftkli.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2wgqfgehd.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2phczakvq.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2qijksnfp.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2mlzgjlva.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2ixazfexy.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2ektrtuob.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2mwbvzlox.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2fhwhunka.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2wccywqli.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2qigiiyeb.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2lhosilld.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2ztcwflkq.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2nfhdtrxf.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2ezddgdtf.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2ezytsqsz.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2kuzzntrm.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2omgbbnef.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2lpdcaptm.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2xjkqdkhw.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2pcdpyapu.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2lpqnlbuw.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2dmyydqxj.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2umjveatc.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2quyiahnz.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2ecqmbfpb.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2bxholees.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2aijzbjvq.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2iycsvhlc.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2bufurzly.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2wodipaos.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2bchqlysg.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2uwavwwvk.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2cuunausg.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2lnzsouow.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2akhkgwkz.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2bccvuhed.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2lcygwjpz.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2usvawoty.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2epkmgwbv.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2srtkwgds.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2bpzfxglw.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2tefocfjk.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ksgedjjj.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2hdzysvlw.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2hpzmxkph.html


<!-- 参考信息 -->