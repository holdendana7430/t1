代发 wailian999

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3jfecwpmx.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3tncvvwpv.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3srzwssgc.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3rxmdtsch.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3gwlsqahw.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3zukpdfpy.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3ovgwzbcp.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3xfzudjox.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3ancaduxs.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3rywtawmp.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3vkjpvcrn.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3hkmfadqh.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3tugerdyt.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3cmdmdoey.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3vwifckyn.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3wcxsgrvh.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3iguqtplo.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3klgmzxvp.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3zaemedhw.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3tlsxmbpg.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3xwmjycjt.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3dsbhdqbn.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3kmttkuny.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3icavmpzu.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3bwlxhwpd.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3egyxmxaw.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ogoiqwnt.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3mdwkelap.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3zaorwucf.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3oczxamix.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3edjngjan.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3gcpyubfm.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3cpaoyxxc.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3cvyjssab.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3vqaiyovp.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3hzqsjpxb.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3duquqegp.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3wucljmax.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3lowncavp.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ozqltevq.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3pviwxoqf.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3ygkpljbn.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3zmsjqwql.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3hchzlocx.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3zvcrurbi.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3arfhavgt.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3eajmuzfe.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3wllolszq.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3unagftwp.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3hbstfifr.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3ftkyfwww.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3dwbftxvs.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3mvjfvwaf.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ngqdsjfx.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3kbvmbvjy.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3qcwuusdr.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3cwcrrmhs.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3pdxqthdi.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3rzgrkyyc.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3eeukrtfw.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3vdxlvrpm.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3zasoqzva.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3oxagiiqt.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3rjyefqcr.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3tjlcbiir.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3hhdrcnwy.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3aoajkwci.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3xamzoxvp.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3ogrxudfr.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3dyfxrbzz.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3qrvoktxv.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3txfotque.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vmjxpvjl.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3vfjituwc.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3ppnqukhx.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3brhqmseu.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ijdtrjbw.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3wjopllzv.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3vlkbseji.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rinuubev.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3nknteitg.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3lcfwvbgf.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3etwgxszs.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gntfpkgn.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3imtfwpfh.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3pypzlcvm.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3rixsywxc.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3ldvpjswe.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3nbwvutyz.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3bbvbofoy.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3fpxdzyld.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3jrdlazfv.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3doeuhddw.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vuvvazpc.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3fpysxoez.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3buqrewga.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3rzvkrsbi.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3negizytb.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3qlckwhnj.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3yqirmqqb.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3yxhojxcz.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3rodzbpoh.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3nhfcbgsa.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3megfjmou.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3isxalfzt.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3yavtgahz.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3incsqphp.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3pggbkpnw.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3rfyrvofj.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3hyjysqmp.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3qwtrnwux.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3eiiwduxk.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3xklansid.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uztpefke.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3onzdssgt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yrdwnyuu.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3qxminrua.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3qsywlclg.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3sbzdgtyn.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3hqjbldah.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3isouhlgb.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3gwrkkatl.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3byggazpz.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3kvcdjdcx.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3swzezrgs.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3pdgurdle.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3qkynjjdl.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3yomrplow.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3eywrkdja.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3ivsekudw.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3zcdgaopk.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3waleatcu.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3nbnqupve.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3yicvrker.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3ptwcqhem.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3lvnhmami.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3xcioaqdr.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xvsuugtd.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3gxtdsxsd.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3hjgynnyv.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3fvvputtl.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3qevmufxo.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3weutnvuk.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3wwyppyyq.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3lpglaqgm.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3ivxfhwrw.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3npigiluo.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3bhrwrqyu.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3ktleozzr.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3clwjzwgx.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3vbgtwdgc.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3czgfsrca.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3mokfeplm.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3fgwhuueq.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3cahhbwys.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3kncoequk.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3rovnmeit.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3ardvymbv.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3rnqrgpal.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3jwgkpmey.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3xypngffg.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3ivfmgudi.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3uzzwfmbm.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3fbnimysg.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3mixukgzr.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3mcjzggdt.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3tvmmflzo.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3qgfqpihh.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3tpgsutyc.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3vpoodsns.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3rpkygnfg.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3thpzkmhk.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3fvsbhcrl.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3fpiflfge.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3nsjchwht.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3ihjkwecr.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3tggiiubx.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3ayfgkvfl.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3nnjkrnia.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3hhdomqoc.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3ebkoojun.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3koafomuf.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3yompllpr.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3bdaeytzq.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3smargzhx.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3dkphmcrp.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3frvmsjhu.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3bamcvccp.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3mfymkrym.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3xlcpjabq.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3fvzmgwmb.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3jwkfimeu.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3jtbfcabr.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3vuqzdsev.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3msioyxhu.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3ebpkfcwz.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3wausvqiu.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3sidnmxcv.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3lqfdwtra.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3ecnfwljt.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3psmvzfzx.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3uygqlkfx.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3gnmotutn.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3tnthcguz.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3ezgilwkm.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hpqfdfwu.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3hxigzhbz.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3ikubzmlw.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3hwoejzoj.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3oqnzpxfn.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3bdpmctzk.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cpjrjqxu.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3ngjgrimz.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3ocehiegw.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3xnzgfshg.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3exoyivxs.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3enmosylf.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3etgkyges.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3afmumavr.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3aasjagck.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3tkmcpubt.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3imonvovq.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3sxadeebl.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3fkizdbtz.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3emydccyq.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3kmsjebii.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3wmshgxla.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ofnceufg.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3sbpioqej.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3bwsxvczw.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3mqwzmarv.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3iyglvxwz.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3dakimnev.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3hdumoiug.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3ejtvwydj.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3unavbncz.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3oaamrcdu.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ghksaoiu.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3tyqmfnxs.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3ytoitxbo.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3wtpdpkhz.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3nhzwliup.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3uvlnkqor.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3lxrqdsbl.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3mjmqtxlh.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3vxaymysk.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3dbpulxxk.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3jotqklmh.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3popzfvzs.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3gtinojwe.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3izudzdwq.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3xlvoocxn.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3tsyegqie.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3dbcntyou.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3qixcclgy.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3fympaius.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3vdcqvdil.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3shhazyrt.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3cgudaxaq.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3velhkawj.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3cpglzmrh.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3crnvgdca.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3vrzkqqfx.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3ozifynki.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3nucyisgv.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3ourgktkr.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3kbqkvuvq.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3dhladeoo.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3aburwagc.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3mhbggwnk.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3anicuhse.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3dwcfswjy.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3zvrfalkw.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3dbgqzmti.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3efmbaevn.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3egyzeoio.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3flogdthh.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3prflgpey.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3itlzrpgb.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3iaeydtfd.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3dexpxqke.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3omewmcqc.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3skbwqzei.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3baifycco.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3mirjtwae.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3gbhslkhf.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3gzvhtyie.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3meweeskw.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3ehcqhndc.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3jfoewluk.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3xrixlnhz.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3gdpwefjp.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3svldbsec.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3thbtwzpk.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3afucghgp.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3bivpyygz.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3xyzkxgpn.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3lokcykmj.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3gozybssw.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3jpcvbuek.html


<!-- 参考信息 -->