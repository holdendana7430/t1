代发 wailian999

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2dejrqccb.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2dratcvob.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2ybpjhabj.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2tprjfcue.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2gxbbovms.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2pnqchioe.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2ytswofno.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2mpsikoqj.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2faepjutm.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2iwcalreg.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2wbligxrt.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2mismsgwl.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2trydsnrm.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xiihyrdx.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2unexjvly.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2dscvjwug.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2haxvogmc.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2azsxjypt.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2digulejr.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2qbaighzt.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2edzimvqw.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2dgscetyz.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2bpvceiee.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2rqdjqprz.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2tmacvoas.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2vilxlswi.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2aivluphj.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2wwkbdorz.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2scxkahhf.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2ynwieytx.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2eqeyvmmj.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2smbhcyfa.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2apsmqkzu.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2hqjiqasw.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2dvpheskt.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2quutmzjc.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2omfeinno.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2lhfzrxtt.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2uedtswzv.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2bgkfsqct.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2paojjcxj.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2ajbfmtyg.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2zmohrsdm.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2mvquuupp.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2qzodyplf.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2ffxqhfpq.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2bnirgzrg.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2ejxredbw.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2pvgxbdrb.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2txvkrgag.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2yfjymwjw.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2xxscpfop.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2dbaouhdq.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2clpenuvk.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2ngxojosu.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2akzrvsmm.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2qjtzjuie.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2vemganik.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2bifpkotb.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2eketvvls.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2vgwlskac.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2hfnwcjjv.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2tdgbfskf.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2qccjidal.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2oyjudczf.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2mfsyabst.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2bdgkwuxp.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2flvhdrhe.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qwzkjbkq.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2jcqnpwez.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2vzgqyomr.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2vkklzyla.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2eqrgmlwc.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2nfgwmhak.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2chjycknx.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2oaccbnqj.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2klzflchq.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2exgzjadp.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2fdctrbcm.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jylxpasp.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2ckxeszjc.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2wkcouees.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2anodgtlx.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2cmhhpqsd.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2vthuniow.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wpticdun.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2oooeotza.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2sljrqjxo.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2oonwgfah.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ebjutxuu.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2mbhcnotz.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2zcatzciw.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2jrdgvdmz.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ynxggdke.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2obtaxnnm.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2qxgyqfax.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hdtytele.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2kkcmvroj.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2anirkeip.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2yfvlzgzh.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2hseqdhgg.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2sxgogwgp.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2rsnggrxx.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2wkpwrhim.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2hmutranc.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2fmvrcqmw.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2voipjyps.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2jyypjqdg.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2paleziyo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xgiuvydy.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ldlmlrym.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kbxamwpm.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2ccdcctlm.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2pjqjyzhh.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2qhxvqysy.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2iziwngcz.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2irtrivxh.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2hfnivhxm.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2dzsibrcv.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2filtsjak.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2qqbuhcvk.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ugfatupr.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2ivzuafsn.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2cywnrpmt.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2ptxexhxr.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2zmrwvwzt.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2qqmizsme.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2gdawupll.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2mywnthmp.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2jnjrrqze.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2fxpfgtzc.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2iwgoqtpg.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2yqdfmmcx.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vryhbjgf.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2kjzwlcir.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2wwjpcbof.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2diptylwq.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2pzuwvmzc.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2tlramlwv.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2dpxbersl.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2ckecarmq.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2yynkmwxj.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2qdhgufjm.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2btgprilq.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2uxeeygkt.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2wjbbgqkx.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2wfhcruqq.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2wvwpbpzp.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2knaxvonf.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2laqmiiwd.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2pclvmbjx.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2hxuwokod.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2ocgagcts.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2tutgjqqz.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2xivywtst.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2axqqeznf.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2gkognase.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2ixrujrtb.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2cnhpjebt.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ogswkfbn.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2ikjcknhs.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2uhdedadv.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2trddxbmb.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2zthxuybw.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2lzfytfsz.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2nmyqoqxl.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2vgpzytpo.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2yxtrtjap.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2habqqzkb.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2xxskioap.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2gkcfwqyg.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2dpsqpbos.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2bzcvpccu.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2askevkdw.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2lolinmts.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2qslqzxsm.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2nrgrqtvx.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2xxakfgnv.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2qsjwwity.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2ecerkhoe.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2lgfzahhe.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2jkqpdbpz.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2hoikhicd.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2kksdutzq.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2mzpgwlhv.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2dkyzynqs.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2elipvweb.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2apxooekb.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2qmgmnrsj.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2dcysnywr.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2hldholwt.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2yafdunvu.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2vddhuafd.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2yfmksnzd.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2cwejikky.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2xrkqfrmo.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2vbyqrqko.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2lpcmvhfd.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2bpacrsfn.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2slyyffyn.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2wuxxqoyt.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2gdquijxy.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2ncdtqaag.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2qpvirxuf.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2gpjbxvpb.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2wcktwlzi.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2rtsjgysg.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jizuuepw.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2vjigzyzm.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2lecomrrl.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2uqnzomzy.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2czgismpb.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2ogaqojor.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2fflqmxao.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2tewecxcu.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2yqbzrywm.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2zykelxsq.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2wfhssmiq.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2prhpfolo.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2khmkjodd.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2chmcjjzb.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2emyoedcb.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2krrlrpru.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2efdubhsk.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2uczhxevf.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2ayegobiu.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2qmbrpvbn.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2focfjnxb.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2tqxtartc.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2zvhkimfi.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2fyjrscfb.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2gtmvqjcd.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2bunzpdoo.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mjssyvxc.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2cngdmeun.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2znbmigjo.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2jhkzwjcq.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2evmkaqsy.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2tpidvlkx.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2johsijmj.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2uzqjdtvm.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2pzvkqtjr.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2etkfozsk.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2mnmumeva.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2khfosfte.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2adexuymr.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2xcwaoauh.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2bdjluwll.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2uwrdpskj.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2ofdgpttr.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2zoohkjht.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2hmitzhvq.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2safzmvcy.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2oevynfht.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2zncdmigw.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2qbvqlxdb.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2agxpmwrs.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2jpneuwgd.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2puhdgtzt.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2vhwmvtli.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2odwrohre.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2rwwfuiew.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2oscjxpbq.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2agnavaau.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2ragunvzc.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2tcyjuqnw.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2okugkltx.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2hnmylsip.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2tojvvutx.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2cqdabqxu.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2qqthgvet.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2ekyyhyew.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2swxszmhr.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2lsytcist.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2zeffztmi.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2faqskwmu.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2dnvgizeq.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2higwrtjw.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2zmigqngv.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2fwbrsnnl.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2qtflwnhm.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2rswfkfmc.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2dzcfbzvm.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2bqphhkas.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2ldhrmlwv.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2lzxwmxlh.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2dacmxtik.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2gjkfzxcn.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2cjcqqizb.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2nxomvely.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2dcrslrdy.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2dctkuomx.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2pytuxgzw.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2mskburnw.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2gclmfsaz.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zatnchsl.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2etcpizgg.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2ellnfize.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2iliqmfhg.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2eezkvvti.html


<!-- 参考信息 -->