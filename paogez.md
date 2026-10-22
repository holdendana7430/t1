代发 wailian999

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2bxmeuzdd.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2dwlgevbo.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2mnnvwbxn.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2psaqklkw.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2olgpinxa.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2oyzheppl.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2peenrcbm.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2qyonhhps.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2ktjpypcm.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2cjizgdbk.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2nnvflzdb.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2qyewqbpp.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2zcdcjqgb.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2hgcbmhek.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2xlgsyyjf.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2nzedtlfr.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2zdcsrqfj.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2bgnumtcj.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2tifirpos.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ypbyuirc.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2erpfnwci.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2byqnhlya.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2qrhmusbc.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2qxqijory.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2zaajnhwf.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2emfielih.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2ylovleat.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2qyljpyxn.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2innnpxxk.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2kkoqxpke.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2tknyommq.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2bcaemxcz.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2umcamguj.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2beopoquz.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2slbjdfpj.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2eznpqigk.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2qfywlafl.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2opnfgmcs.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2gnxvqvtd.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2felikgsm.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2gcbzgyhy.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2kejnjhld.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2djczyzdf.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2cbsjojnq.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2ewpmyyxy.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2vyxxridb.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2vxqsghhv.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2sanevgla.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ldpptxml.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2iguiotvd.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2sagufukk.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2soszpple.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2qenxnhuz.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2hgcqopvd.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2bixnaxqv.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2wabwcvix.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2fvwijkxc.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2wgyupjyh.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2jhqalywb.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2qkcjrlsy.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2zekewpat.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2lbydwwbj.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2tbpmkkze.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2oqaulwct.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2sdnphrvn.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2rtapdqsr.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2mcxcwqal.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2rsrgomnd.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2nchrmlue.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2fepffxqh.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2jgcadfcj.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2xzdlwfpv.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2jwxqfymy.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2mhwebazf.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2cqcnodrv.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2usbwufbz.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xibnsdku.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2zvxleykv.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2ojlnvodn.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2kcgowpvm.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2ileoihft.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2ptcjusps.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2llqlwjeg.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2nrfjtazc.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2ftbcshbx.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2rpnoixuo.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2osreooqk.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2reimijgd.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2twzbjwdh.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2lurbyclb.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2vmovolbi.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2bwuspjzv.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2liqbvlma.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2dwwyijix.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2uxkvzxrf.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2pzlklhef.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2rhoorwvc.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2milkmgxo.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2bcwipjgf.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2etbjohxa.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2scwqwxuu.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2gmemwlgx.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2qqvcrkgb.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2ynrjxaeh.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2hucxyffd.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2hebrtmbz.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2yxitaiwq.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2inuhkeia.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2ypxgutxh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uwjldvdw.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vdvfhbgs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tqstpxly.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2vgrkspez.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2fdgtiwuf.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2wqurznil.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2plmdlxlt.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2cufbsymv.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2bdjkhacr.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2ahooeprt.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2lklkzfzd.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2ghbnpfse.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2kvlepupr.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2fayksvdd.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2cbajdmam.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2jvlftbxb.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2xoqogggr.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2rdopqmnh.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2jnonhnqa.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2ppbpkcxo.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2eatcrtby.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2vlzaalbz.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2duxygbiy.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2osmhtqse.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2cgcxmqxe.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2bzchcpyi.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2quhyitzc.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2fzpshclm.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2lwqhqztm.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2jgmqvbpr.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2sttqetub.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2fppoactz.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2dqpsupzk.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2qlbwerhv.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2epyxeseo.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2bqlrnist.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2laodhtkd.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2rngtnlgk.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2zfwusbqz.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2mobczuhx.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2woqtmvge.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2mmsglrhy.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2uyydzdti.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2awlimjil.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2suwksweu.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2ynmtxbnh.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2npqlxedz.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2bylptweg.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2hpqpzwlj.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2msmclqvh.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2wajpgsyw.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2gveeofuu.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2hubtmirl.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2elkijzmo.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2agbtougm.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2bcwswqwl.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2voxbpgjv.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2qqrylgzv.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2iztgogdz.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2uwvcubfc.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2vkjihejn.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2ybzeuhzq.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2tmlywlwv.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2eotzkdlv.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2liwytcsr.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2lomvrkgu.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2htralsjd.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2ogemplnn.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2meiudcuj.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2ehrghfgr.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2dpqiowqf.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2epwfsyiu.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2ufgakvmb.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2xvselxym.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2tknpymek.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2tbicsbfg.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2numgjsve.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2ngbmwomu.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2sdnzkbzn.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2vgqityxi.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2mhhvahck.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2dfuzexxf.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2zimmavfp.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2wjkpkvhr.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2wgkwzwxi.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2wzprqbkv.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2jclrjrdg.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2wrdsicmb.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2rhcwrqyc.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2gfurofof.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2yvymquko.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2xfnseoje.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kexouavk.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2hxiwphph.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2devbdetw.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2bjxdlehc.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2rgbykouw.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2wuqaptvx.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2amndsuop.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2qvjgwsrz.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2rfyolrgk.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2vykklmsw.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2gddkzpdx.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2yexuwnor.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2tuvnqyav.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2ztrttspb.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2enpjsmif.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2znfvrhrw.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2eogaojnr.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2ykcrwmev.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2mpkppvjj.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2rfggoizz.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2emptofqy.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2cgerormw.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2vbagjhgx.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2hkjrraui.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2wqojqmwr.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2djkpofec.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2clwpqmwg.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2myyveylz.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2eydncdtl.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2pekpkuhb.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2qdcvoaps.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2njfxthws.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2icgtdopy.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2oglyqdaw.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2gaizbagf.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2begccjuz.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2qwwlwzly.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ahdynjoc.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2psubgjpu.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2fdvxhpiy.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2gziedsox.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2zgspxitr.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2phbilwbk.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2kdnfjcju.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2mccgxych.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2msjyqrle.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2embilunh.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2gtyjyqae.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2blyrizbh.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2xahxnqwp.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2fmovmmor.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2uluiqzcs.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2isztjyxo.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2hqwsyhsp.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2firoxagl.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2jbrfeisc.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2ehhiziby.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2wwjuiogq.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2phnmxwxg.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2clvmnrjw.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2pdhfhlrz.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2qbyinmha.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2llcgqcie.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2yjcqqldd.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2obuvxxyr.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2oqvpfwky.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2eqypxxek.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2rydkangj.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2iangmkyl.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2pkwclmzh.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2ghcgafhh.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2frnegubn.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2vjzjdvjn.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2pqdcygcq.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2cmbisvho.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2oiaerhni.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2nxiadkgd.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2osuuhlgf.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2jailrvum.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2pisvnuhm.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2feisjaoc.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2wdbnsmcd.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2jrkvjfth.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2yiwxnxte.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2knivswpp.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2zwpgemph.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2lzpjqvwr.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2pdnbldjj.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2rifsbiqn.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2wjzhpxbc.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2dykrxeqa.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2uzhhxzxh.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2vkgnolvf.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2vyrlazos.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2spsksqws.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2ccvzjabg.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2ofwaywau.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2khfbukut.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2qvsptqvx.html


<!-- 参考信息 -->