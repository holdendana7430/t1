代发 wailian999

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3rewghhmn.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3xwxwdzxe.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3zhdwlcua.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3qathgzlu.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3kauewcsv.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3nevtmdjv.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3hzaonkqi.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3azgnhdms.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3umswuzyt.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3odzntxll.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3wxbsfrur.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bsctgcsk.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3oskjikyl.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3dycmoojo.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3pbmmohrn.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3bwkfxuiu.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3igzegxsr.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3dhpbmchm.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3zzynkbat.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3bqdmpmob.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3fxgcggly.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3fcbguooq.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3kbvtpwaa.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3wuqbnrsi.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3kovewuws.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3mgelsrov.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3gcnqwekb.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3vciboooj.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3amsptwte.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3zxxkqvnl.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3cchvhlut.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3envmkvah.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3iewgvboh.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3bfuofdyc.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3isdivgco.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3nsgyshyj.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3vroprfpm.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3fjskbyli.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3kpgjlxpv.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3vipwvlwa.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3sieziamv.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3gywiritu.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3znzwqlxu.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3exxipmuy.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3myyfoxkw.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3fpdxdybl.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3bstzdsdh.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3yvjhubgr.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3svgkaote.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3lwqabybx.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3vpohwygy.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3hmietzwq.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3siebmbuu.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3gdiphsod.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3fdjxkgoe.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3atgpilmp.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3ulwbiwzh.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ihsepkas.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3guamrhny.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3hlttgglp.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3rvtgnukk.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3giojkbew.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3elfiwdfq.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3qfmsrbas.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3bhwvjujx.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3kbqtbaih.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3nmlehgzl.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3orxkzmcz.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vywsecxf.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3ymeydtmg.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3qptrxcvt.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3zyycomfz.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3wwdmboab.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3dehrrgzs.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3wspilwnn.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dfrfooqc.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qvapohcs.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3slvelndd.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3lmerpzgd.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ojtihlky.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3xkzususj.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3lnukievd.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3tpswjrnn.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3yovojkof.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3bqbkddlc.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3fesjtmzf.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3sbkvhiqn.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3ficnelry.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3zvvnocma.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ivtnausf.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3hcqrgmhx.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3usojcejg.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3lvshgijl.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3cjpwonzv.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3marxjbhe.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3sauwnhka.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3ccmcdceg.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3buinevsx.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3wvlzktje.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3iadbhltn.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3llritjmu.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3vsovvzev.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3qxnoltdb.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3ptoiwlni.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3fhighest.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3egltfzeb.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3qhpmwcjh.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3bvryjucr.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3nyiikvik.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lchoglmq.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xxotgutu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3poxjqcmb.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3gewjkhpj.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3bhyjcvsh.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3knxxlagm.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3rtneruoo.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3nwgbfzxt.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3qmykfzjk.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3pgjldawj.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3chtohjsr.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3qjfzrtef.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3yqfvjkrj.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3pwzgyjrv.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3lumolfhr.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3pygtapkq.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3phkrthhd.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3xeceevtx.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3kmhirtri.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3tydcoicr.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3zqsfwtav.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3logyiphu.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3yaeedxnj.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3rzifpmqx.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bzfxaicn.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3admbnxvr.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3nnmyczag.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3lybaetod.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3bqpvpzev.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3orcxgail.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3arkxtnyy.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3cqcwlmaj.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3cwzefthj.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3ovuywlkh.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3xvknkwbw.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3zauzvemn.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3kffogubh.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3ppacmyff.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3halbeenq.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3aqgizgzh.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3xwkzeidx.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3gucckcvf.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3cgvoiqzr.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3sptxwkcl.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3huubwbfc.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3lvgclymn.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3dwctiugc.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3kbyzwbaq.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3nbyqznqt.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3pnfjrbkg.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3cfkkmimc.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3qokhagjn.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3vdxcfhkh.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3qrfdejaw.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3uejsxapk.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3gxedtjre.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3wuqokbur.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3jtduocii.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3gyjpoina.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3ildlteyo.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3shfhycqd.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3dsaxloaj.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3hvfkrnet.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3ixknirni.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3upirgbrv.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3btyrkimb.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3sxjyfqfr.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3krdxpkpj.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3dtrtzdmd.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3tbvmwvas.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3avostluz.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3lsibutqt.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3tuivpsia.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3girzlfmc.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3mdrbogav.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3xxcrcwmf.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3dmwznrpc.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3qhsqjabp.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3ktcfkcvl.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3sukusqoa.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3ewhplowd.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3ubwhjlbg.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3ulpmwxwn.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3csurwdej.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3yphhjfpo.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3xipdcevq.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3vcqfnqtd.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3nbxfdbsc.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3vwixgzir.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3kkufnajp.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3vwldksbx.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3erutvbbf.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3odmiwivs.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3lcnzzvqu.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3gmjncqmw.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3kergcewd.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3demhixvo.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3xmfuppae.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3uvcsahvd.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3kgcirqfu.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3tqwcefcb.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3janfssvu.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3ltpjuovc.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3xctoyjia.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3rwyyjrxf.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3swbdhunr.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3bpihxhbz.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3lvlurtuk.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3nagbttbe.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3awjqhzik.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3tazbxltb.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3dyqlpwoo.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3honlnocu.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3gyxcajob.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ktmeulql.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3diiobsas.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3xcfwiubd.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3zifizdku.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3kehwlnft.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3bkxqljkv.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3awsipwch.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3kzmkcnpz.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3cdlunhhx.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3vuthoqvx.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3zgbuanjv.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3eulayqmn.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3yjuorkkx.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3bvsklakb.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3gqykrrnw.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3vchvjrqy.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3mubbetsl.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3btiejoah.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3vbfedlhy.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3vsbnpyoz.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3vamaqqdx.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3uxmamquv.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3lgtcmfed.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3urhfsnjg.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3ajkthrmo.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3cjcvdaqd.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3ztabdvch.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3kdunwgeg.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3lekexgxq.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3iiwojbqk.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3bonowziq.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3zlwbjxfd.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3oiwbwbea.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3xwzqfnlu.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3jkvtdexw.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3dktypppj.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3qhzuebeq.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3ahqnwgzx.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3ejyitjai.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3mugwsink.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3qszlicaq.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3ixjnfitj.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3aieqpdye.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3vqgrzhho.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3wccplsoi.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3grmphcgg.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3haqkyepm.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3zrfekgmm.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3cggdrhsi.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3amrlwkzc.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3wyuogxue.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3xhdbwxqu.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3tmwyfnsw.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3pcdgjthk.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3ytlizedn.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3mlaqadkf.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3yeaebojz.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3vonygyua.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3mmynuywu.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3jcarwwmh.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3smmixgad.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3fdhhlvmy.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3pzoptaxd.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3gbethjxf.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3mzlvydcn.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3bournery.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3pgmcsjdi.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3chmdpefg.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3dasxyzpj.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3crvklxwl.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3jjiiwpml.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3deybgvhz.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3husarxrb.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zdtihsdm.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3txcqtosz.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3oefqzhat.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3xxajuotc.html


<!-- 参考信息 -->