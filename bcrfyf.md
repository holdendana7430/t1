代发 wailian999

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2zwthazay.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2kifgvdcg.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2duahhxjj.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2wafetgkj.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2jdwohqrs.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2wnxofpdg.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2rlpwrqqc.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2yhzcvini.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2bhmlxpbw.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2zomvguhp.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2urtroisn.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2abzqgiep.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2zxhbdyfp.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2abgaejeq.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2ubqpnhgb.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2xhpkcsfd.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2wyervyxv.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2lenwbgvn.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2cgjbejdn.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2blmawcnd.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2pkqnuyva.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2cczrlspw.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2yevkhltt.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2mqkixwem.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2xyylaqmj.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2rasfktzj.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2oeebxxnp.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2cwgjkmye.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2ufyftyel.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2rfmkdosh.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2zaxpntha.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2gnhyfivu.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2euhmvodc.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2ezbexdjw.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2wgjpyqbk.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2evapxncl.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2ldilysew.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2hlqokxrf.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2augtkjpa.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2cvvioppo.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2kjycclpb.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2wyditxyy.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2weehvzga.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2kezgrnlm.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2jgfipzjc.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2nnvhzxjo.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2axtjcehn.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2govaeygv.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2jynngsaa.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2joeopsir.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2mkyqrror.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2rueafkda.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2qbsbjogg.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2vlnclzgl.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2zijrjvzj.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2rkzefoci.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2oloxcfle.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2psdojeff.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2xnlxknae.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2mkyttmff.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2lqfdlwve.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2nsjtcozh.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2ufgrdomf.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2dohftlfv.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2lefsioha.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2anvpfwti.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2kzmoymsg.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2vlqzggih.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2aeezavse.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2ugwznbkq.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2derdetjx.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2ugvggrtk.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2gxkajupy.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2vgxtioer.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2pubqgrrm.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2sefjzbct.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2dxnlboig.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2jgnvcmpr.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2gkzakgns.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2dvhiopgr.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2xlfrwyig.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2agqrdeqn.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2ahwtiepj.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2uydwnanq.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rvvppmux.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2noxplzcs.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2zlqjwwyf.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2shwzlbai.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2wnolwzlx.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2wkgsjyac.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2krtgnrtj.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2rahcdmkx.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2myegeowz.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dtqjivov.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ogcwiaof.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2rapqkqlq.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2hespnjme.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qewjvmsv.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2raeodtbs.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2zhtmhlnf.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2zqskusgb.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2rrglhxts.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2sfmcgbmp.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2ozhohtra.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mkqsamet.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2tpzjzpcu.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2qropsoff.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2mrompfpk.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2deujaxdt.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2swmfzxeo.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2vvmvzrnv.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2wafjkcxw.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2rimytwtq.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2sqvjpjtx.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2kbieaulc.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2jodfqbeh.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2txnrbleg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nvxfiexx.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ynwdxemn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ivdfixoy.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2tbsdfaqc.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2yslnwwgc.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2qseicdol.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2krmsirai.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2bgqskrwy.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2jdszjiwl.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2drejuybs.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2bsqnxukm.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2gwofzsxd.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2vkaywydn.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2emojhtdr.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2xpxqlxii.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2ezyvnngw.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2riabtwwv.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2jkqxajyz.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2dpxdpvmq.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2oujyhbbr.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2ijsdbksz.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2brhzmzap.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2icaqizmo.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2cnfmnhbs.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2qftqkjgj.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2sjqqecfg.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2yeixzlev.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2gvnhyycg.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2iyurtqum.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2macdzyyx.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2skippfct.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2aypqmzql.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2xsiiefrz.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2bepxabfl.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2bqpfvdwk.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2omrjqvot.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2lbvgnsqo.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2oqkyuyvl.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2ouzkqlhc.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2jkbekwfc.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2ziewwwrt.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2vtwuypnh.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2nnumcbvg.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2jhtsbxfd.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2qrkdsnny.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2hrygsszf.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2ndfaeivz.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2mrgernoh.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2gdofsgfp.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2xkgdnckj.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2xjjjgyhj.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2qevjsomq.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2pciftaak.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2mvlhsxyh.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2snajqkdr.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2lxsxvtxk.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2hdgyphve.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2vffbhixf.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2odmlgjbl.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2abfjaeys.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2xmeehpjd.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2gxudwufc.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2zfhjslvk.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2khteuwkk.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2rcuqawgk.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2xccoapnv.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2ytqwfdkb.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2vibhqzft.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2wjcohbck.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2tzwlxeyf.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2xpegwwue.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2rfizhzdv.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2yhxvifwu.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2wmvgukeb.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2ltogqybv.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2vrhoswoo.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2mikudnjw.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2wfyhhnny.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2iowscxui.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2zyfryoqt.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2qcntvmom.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2juxfmlhv.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2vcyhkwjo.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2itbzvwqg.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2cokumarq.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2apmnozwb.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2apnhtzzc.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2iyqcgiwy.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2heqhdyie.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2muwklbnv.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2oflokfhf.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2wnctiihf.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2bdppznhv.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2xqlmubxb.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2sfkinojo.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2ctgxfvpz.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2xovdeaac.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2rwjglyls.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kpvexsvx.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2olfaotgk.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2hpivylbf.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2mbdfnwfg.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2spoxdfcd.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2trjxkzxq.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2nybfzkbh.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2aoppzizs.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2djymvfmb.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2xjuqohyx.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2gtsljcau.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2isblqroc.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2pssptcpo.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2gicdsqgn.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2ygvnbpva.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2fmhquwjo.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qikmkctm.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2uwzmgocs.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2prfunkla.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2mgigyhqn.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2babigdqw.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2zepwgsrd.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2pascifkx.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2gbexpnja.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2hzobtsuj.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2htyvmiwv.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2fjhyknrm.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2xbwwrpbp.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2trhwkdql.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2rgmyncop.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2jmrtdkmr.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2mubfagym.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2daquvodp.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2ecapftqx.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2bwzmbcvt.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2hoghyinq.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2mkfhwdkd.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2mldshsdo.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2wyizbnsb.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2aygclxlk.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2ribhilrd.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2yfynvkon.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2wkajqnuv.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2gprdklgf.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2ifvzgmmi.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2ryycdlef.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2bliiqvgd.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2qdaeczim.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2awwflbew.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2couhjfyd.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2julgsipe.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2syozwesd.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2xwgfpmkc.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2wbjgfrip.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2scqfaacr.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2snyiugte.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2dqqrxvlr.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2dwcqagtk.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2wxvarcvs.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2ircnfonr.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2lvsehisj.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2ccwsfyso.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2ryzmjeae.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2wbvvaleg.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2fejtrfif.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2errjjusg.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2krhpgbvc.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2bbqsolfi.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2brrsjbnv.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2rvwmrmfh.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2ypdiyuve.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2mfvnklog.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2tsdlhyqe.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2xipgjwzz.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2ssbnlozd.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2hwrujdqr.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2cnqpkfpi.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2ymudgloj.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2ieajxilz.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2lvssnzsk.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2vtyhcygh.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2djhqpmpl.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2xdgxdcfo.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2hhuqyerw.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2hzjfoybx.html


<!-- 参考信息 -->