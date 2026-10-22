代发 wailian999

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2kodbnlkw.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2uygqrdhp.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2lkjxusan.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2bdqpxeuh.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2kuumavfd.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2kxebupom.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2tpxmcafn.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2sjppqmun.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2lctyjubq.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2rlqqgvhm.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2treucfff.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2rydtcskr.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2ucphiist.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2xfavwyjh.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2qiuauokm.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gienzktp.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2xagckmas.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2azpbfcnh.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2epghgtfa.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2mtjcibyl.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2qoqjhkmc.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2quadqqoh.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2otwqquzb.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ymxkkgmp.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2lxeuqvcm.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2mkgeegoh.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2qeywwqih.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2itdzrpef.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2jezxmamt.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2mxwhggtj.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2ohdqkqdd.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2niqumesv.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2nfswzqnz.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2txorcswz.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2krqqrjdz.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2iachngit.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2coyoivpu.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2nghcewua.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2pioflzqm.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2qdlqfyrx.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2wdhspntg.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2pcgmikhk.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2uymomxuc.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2jnezedsi.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2opesypyx.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2tuhibveh.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2csrexyvq.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2zvctftmc.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2qkbnvnlg.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2hlzspqqf.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2pyqrorde.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2coqoyzji.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2doehcrmj.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2sidknxcx.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2egmqcaox.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2uvlaejse.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2czsldjec.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2aisudfhe.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2akskguot.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2fvlomnii.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2grtencvu.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2lftrhafv.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2kefawxjk.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2cqirwdly.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2tkmokblq.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2ntxhybkf.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2bbeliysw.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2cvxjjzhd.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2ofoxjkwk.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2wexmjolv.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2xifzwuhx.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2xdfudxzc.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2kobewbmz.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2exrzkkhc.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2yhbaztis.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2xbppiezm.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2wugdsfxm.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2iczdyliu.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2sxgjiavl.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2qbupydpy.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2eoqufzww.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2vbrwnjeh.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2mjhfkrcg.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2qvhwutaz.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2wcozxdut.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2aqxyixyp.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2oborrpzj.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2wayiamrv.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2nnlcfnme.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2hipzmaah.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2twmhuobp.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2nzlcgzqu.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2nobsdoyy.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2moonmtbs.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2wcvmrttx.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2cavnhppx.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2qjinvzxv.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2oeflppbh.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2ncekhqgr.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2pgpljlwi.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ktbjdjxx.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2gwumgweo.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2muwkevqo.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2qdtatpmd.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2vtpbqpqd.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2vzptastd.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2ujjiuqcl.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2tipguqpr.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2xiruauhl.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2asxrrmcd.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2ltwmtlgq.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2ztusovzw.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2sdkowitr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hmluaxoe.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2mvuoehuq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lptqefgw.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2lrhivqgn.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2pintknka.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2xznhplcl.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rebbqqgl.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2tztbhzqa.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2razxtspf.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2xaodwbzg.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2ewlcdjcs.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2orzqvcjh.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2ocsafxej.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2iymzxmij.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2vohumaps.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2lygwtxzs.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2gbpgnots.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2ealjntal.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2sszuxsbh.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2kbsfcjab.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2aivtxhjf.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2fjwhilbj.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2gvosfpmx.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2mhknmqka.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2tprtgfbj.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2vfuwwwuo.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2djwabgge.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2whuhmykc.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2fduooxvk.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2yfedldrk.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2tfmethvf.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2zikkmfwd.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2gasfgpeu.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2sonojtpo.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2rnzytknp.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2xlulvoif.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2eedsovzc.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2tfjljzhe.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2jtrhrlhk.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2vwylbqog.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2ngjgypjx.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2rcpwfesc.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2cgyoguuk.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2qoqrzqdi.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2xwyeodga.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2ynhmnthc.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2tikljhqd.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2zrknvxwc.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2eknlhjfo.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2vxqxajts.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2viutuxce.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2ldnjemlg.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2hxtqiswy.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2maoqgyif.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2rswzjado.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2vyjgjymk.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2agzapfis.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2tdmnxlbd.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2orgomydl.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2ozsfguib.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2mdxdamxl.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2fizgqacd.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2fmuqxfct.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2rtosnhrp.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2jgzmthse.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2zvrgjexb.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2ihwldpov.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2fzoffoga.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2orkcsuuf.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2gomdgwkd.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2vetrdyzk.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2cmeurbll.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2jnnoeiyb.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2dbjyfuqr.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2iqleopzz.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2jcksntja.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2ptoovkst.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2gkftkanq.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2dywjwnot.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2ibkwvddf.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2urkiknqh.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2kzxrayds.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2yupvdeui.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2geisnvnb.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2buhuliou.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2gmxyyyad.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2ydkirxjw.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2nkdfqdsm.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2jittfcuf.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2kzwenmqw.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2wzvobgtz.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2lhxkbxqo.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2mzugggno.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2itklpxei.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2ctjibnbq.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2mubskxpu.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2khractyf.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2oofoziqw.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rnfcacck.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2zfqpoafa.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2qkdbhofg.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2zezsxxci.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zbmlecez.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2tuyolsif.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2fjyeirvg.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2wcegdral.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2hgpgzkls.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2qoblmbwu.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2ymoqwmej.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2mstxiikw.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2txmqojut.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2illgvmty.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2uctnvygn.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2unniztpa.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2sikulewe.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2vgyrgcoi.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2gbzazrmu.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2xltkyctw.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2vzoxtoqc.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2gypgemlz.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2hcfsrqio.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2otpxwjif.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2eqozkjxm.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2faqgychu.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2mxdnpgob.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2fuwyzodm.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2xezrnbnc.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2fadmegsq.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2cpntlasz.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2mxvvsqly.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2pvenntmy.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2wrrkubeo.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jaqgenej.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2ipixuznb.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ysazekcc.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2kyxqltsd.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2pglxjklw.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2dlbdysyf.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2lrwxzdid.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2bcfsivga.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2btdcihqv.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2nufqzfop.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2ztkfviwf.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2hblpklxh.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2thhuitqx.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2iwbryxto.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2fehbkuov.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2mwqzuowc.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2fdtvzmyr.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2xrbtcozc.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2jzrchwsr.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2unayhvjf.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2fnxzeuha.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2rvraefjq.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2eegkkptv.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2houaeoex.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2nglvsxie.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2athvqipn.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2qgtdncrp.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2cxpxqtdx.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2lpsgaxzm.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2edowztuh.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2uxnbeprw.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2lbtqgdky.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2excmmilx.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2qzdasund.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2nujzwymf.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2irknyhub.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2jwbodcki.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2ykemapjp.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2gpegmwzw.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2cusxvgei.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2nehivyrb.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2pxhamktj.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2ocjvlryk.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2amvqjzzj.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2bwhbwsck.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2hiilexok.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2pxlwhlye.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2lkiqgaos.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ddkesehd.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2szeordyh.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2hohmqmkj.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2kkxejuvi.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2hhdcyrgc.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2imgfmqlh.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2swskeblr.html


<!-- 参考信息 -->