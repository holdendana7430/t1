代发 wailian999

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2aywtgizo.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2owpiilyz.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2xskrskub.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2jpoosnqh.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2zaiaklqu.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2xouxspdy.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2dfteunry.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2watgwaow.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2fbcgppsr.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2hcpxkehy.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2vwenblix.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2rxxxayni.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2wubmchgb.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2ekqbauzq.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2ncjfwvek.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2knuetokk.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2yiuuydsq.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2ltbyhiqh.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2lhjbfiae.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2aentczhf.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2eolqogzp.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2dciqnbdg.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2zlqrcgcl.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2tuvntbtz.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2iituromi.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2uvxbnccl.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2yqmnclbs.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2auwbrozg.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2rwhcropb.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2rxrwkjtx.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2mfcrmupz.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2sphppwoo.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2hvtxlhla.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2lulxuoyj.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2cpxswhzs.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2egdggfyi.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2kcjrlxnr.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2fkhsebvx.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2dvrbdoor.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2htkceolq.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2icnpygcv.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2jzfvytfo.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2unaydxmz.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2uweocrxj.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2jdjbevge.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2ewvdxjcr.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2kiyjupwz.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2kysjpezj.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2veyabliv.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2pfddweez.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2tikkoute.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2jghuxitu.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2ozkkjtuo.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2itwzknfm.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2kbfteabv.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2oxmtdtnf.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2siiewbch.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2fbtrhuto.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2qitgkdio.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2obgcavpr.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2kgfovugb.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2ipkyqynt.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2xiznogpp.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2nodbinak.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2lwgsasxq.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2uskhplzm.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2zpuzzeff.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2djfthgav.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2ybjfahhj.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2nrgryhdk.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2aoloxflr.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2eedxjlgy.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2wuwgtupu.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2kpyungdd.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2twdtilnc.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2tsnralzf.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2nnxvwohz.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2vpbdckvj.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2uiolwycz.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2vzcweqfr.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2hcruythl.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2lziqtvfc.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2ezotypyy.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2vpcopwzk.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xzqpwusg.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2byrrycoa.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2xsumczad.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2foprbeyu.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2bqlwmbet.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2qvwinkjj.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2ynjbnmdi.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2ervqdsbj.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2cuemaguc.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2itubirns.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2bacuykff.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2qhoemjpg.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2kpezwjvw.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jfcfemcs.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2nkxghakx.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2fskhkdyh.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2crerdbdn.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ayrnrkjd.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2giyvejvd.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2oksqplod.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2ztmqaadn.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2jzjgipdt.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2epjiwwhf.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2dvafjrjx.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2slugrdef.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2edpgvscw.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2mebqanok.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2volcjsoj.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2tzfdnwdk.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2zabsfxip.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2eqqjnceo.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2mcxgukne.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2zgocaaif.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ktixcjof.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2idwpijod.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2whqkumdr.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2flbgccvc.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2hcoquypo.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2hayzitph.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2trdahkmq.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2tintgixb.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2tewndmbl.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2bdfxomwl.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2ryrjxmic.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2dilnmtey.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2uctzcjtn.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2rbblnain.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2fbndcfsn.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2uyvfxkdd.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2bqawjrqx.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2vdemhhkp.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2mungmphj.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2rtdmmksq.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2hackpkbp.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2ihmqdxtb.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2romdgjqn.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2ghyamsbt.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fylcyvow.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2aexpyoji.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2ipxnxtml.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2cxzvbggi.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2shhhvabw.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2zppgdewo.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2yoxnezba.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2bainprld.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2mwlddech.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2gugblntm.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2dcrsovex.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2tukyogpg.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2lucbfqbn.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2glkmlhly.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2czujbvrs.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2pquvfvkk.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2oiruzodm.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2pwmrxokd.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2ichmokdu.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2vjgvrdys.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2wrnvurqp.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2ocbeklxq.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2jicvjjrw.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2hziowjst.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2eibgvhhm.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2chqxbhqo.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2fhcwhmrd.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2itmgwygt.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2vqsupbib.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2qclwxclt.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2ipvxiuuy.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2kltfgoej.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2mthizubn.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2yivvekpa.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2ytzcnqjn.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2neumbqou.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2kyqyyzwc.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2nznepfgb.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2ngzbvbgx.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2llsocgjn.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2pvpywica.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2artkzkuo.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2twjcjyvn.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2yorwzoll.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2yyhqvfdj.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2kygblqkk.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2gwvawtnr.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2vgekwnrc.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2eztabqkt.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2lixfpjss.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2lpcpmtxg.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2parotffj.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2auzwlmsy.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2xvyyqkud.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2zjdnphbu.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2taiwfslp.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2eliwfsmn.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2eemytiep.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2mgulfmzk.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2oipwktdx.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2zpeikquh.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2kpektlwe.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2xzketaxd.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2yquecrte.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2ycoqxble.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2ianqkzlk.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2oragvmew.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2bpufjpqa.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2aqzuoiob.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2tldymqar.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2lnppdkcs.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2nuqremxm.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2ovbvdjvv.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2hicgynjk.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2jkktzrma.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2vczslanb.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2cqjhszgh.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2hrrsrpaa.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2jbpzodby.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2lnuadcaf.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2duiysnrv.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2tgujbhhs.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2gostpaxb.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2ozlogcgw.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2ayhcemyj.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2ejosahvq.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2xhyyrucq.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2jvononmz.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2dalplwaz.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2datpfdsn.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pbjyvafo.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2hnzjxfvs.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2tgpccujm.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2vtsxldvk.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2uitfmmsr.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2ofypbits.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2fjfcviqh.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2bcbknxoa.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2dzxgmlhc.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2blmfphpv.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2zbtihzmn.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2yvpxegsi.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2cisnttin.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2ulyutvqi.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2qpujejlt.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2utrihszt.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2yzsbvegg.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2lwsbnwfe.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2eqrssqnq.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2nlitwsnq.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2qcsvpzdq.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2durvcorz.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2ptogscrk.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2xwlpsmiy.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2ugzfnrdi.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2ejntdbsw.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2ktqrfzwf.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2ihuwzgwc.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2ejzgqvir.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2uooboric.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2nzhwpmyj.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2clwgorsb.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2omqtcfjo.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2hjqpwdth.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2jwczefre.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2obyrsixp.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2ymyzofhd.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2ejdkaddz.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2prvklloq.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2dqutsgst.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2vrzxhiiz.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2iwqgniwg.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2oobtalhi.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2mprwkrde.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2sgempxtu.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2pjsmjgkw.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2slkzraml.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2iewmfqmv.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2mmumfcan.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2kzqjzaif.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2atnpqfoy.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2qvfrlbzq.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2ckrderfs.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2snivrcil.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2odztxpsv.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2jtbhmpfv.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2byjozqfu.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2znybhghs.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2qupjidbr.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2uytpdnhy.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2sllnpvxx.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2uwdroieu.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2yprqvcje.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2oqokrvwj.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2dvjoxzgv.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2qjepxhwp.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2rgxbeqzd.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2jbxgsmgj.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2bjawwxta.html


<!-- 参考信息 -->