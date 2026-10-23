代发 wailian999

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3arbozaiu.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3vtggtxby.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3jskkvwqd.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3uabxnvxx.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3gsajazek.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3hpgsjdlz.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3rrkbshjv.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3lprwstnk.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3kwergzqq.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3iodurinz.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3zwzlxlpf.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3ykfqhwfb.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3dwezywez.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3jhmgapqn.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vwicxxbp.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3vbnfddhe.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3ljyhwbro.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3qgczcvpa.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3mwzlxpht.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3fltnfwdf.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3qrwwuheg.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3ywhtfcob.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3wchiqjxn.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3ujueouwm.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3dabshuvb.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3knxoerlg.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3qcgmvwqg.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3hefurvpx.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3aqsdsuzd.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3kvzevbwv.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3onlpdjgb.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3mgyqnypo.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3vrjbkuvc.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3ctpxqlby.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3xgnriaml.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3mrtmbxpt.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3fvrgnwrt.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3kkawqjwc.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3rzldkgjj.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3zcuswhsx.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3sgfatbaj.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3hgzpmqmo.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3arvkvayi.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3kadpjong.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qcmzqeqj.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3anceuwda.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3dsxlfodz.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3ghzbfunm.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3srrxwskr.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3xokmkcty.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3phuugxtt.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3mlbbqjcb.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3juzeqrxe.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3ofpvhytt.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3wbfrgghn.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3ktmyakza.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3blxurxfi.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3yfuynpgd.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3lnuzwbxv.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3gewbaumn.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3qvfpuusi.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3oskjmoqv.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3xmlwrgxh.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3rbpsfqmk.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3wkskjdqg.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3dxpqwlbv.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3xjzkyoot.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3hgtenxvu.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3oxpcdgvr.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3xovgrphz.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3pzbdxgdv.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3ntarbkuz.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ktbulgkg.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3suhzxbmp.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3guzvlyhx.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rnauxaye.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3tbkefqzz.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3peuepijb.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3lnrwpknp.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3oozbtfzd.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3kjfnwwzb.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3djpvzpce.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ldbhyoqc.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3wdjchvod.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3qpqifcvo.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3rpqytvtx.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3rttjbjdo.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3iqrcipik.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3jzzwvger.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3qrttrslf.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3bvjfstof.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3bxggeemp.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3xshspafs.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3tvdxreoo.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3yqenquvg.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3clxzarhr.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3iezhdaio.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3sldwtktx.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3ssswsbrs.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3attyufyp.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3yjdcxkyg.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3bhscoedw.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3uuqikgqj.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3gstpcagi.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3rrpcvbxc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cewrbuxw.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3emoikbrb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uuloiilv.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3kwbzqqok.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3iulxkpft.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3gdzygitc.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jjtjjrbt.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3glpbuyst.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3qmnakarz.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3ayeiclbu.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3gfkuqevw.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3afpgyeqi.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ixorrixk.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3yyjlqewi.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3cymispfs.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3srsmzvan.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3holslxmk.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3tgpxrmfi.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3gsemqtrf.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3nqnkjbbs.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3cgdprlxz.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3tlhfazyx.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3kcgvdkoj.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3sinwpgqx.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3vqiihikn.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3eeoflhuy.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3nggrbalp.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3xfvesdtm.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3maqqpuni.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3mscukcvd.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3cszefsyo.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3jsdvjvim.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3qykhjvyw.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3zdftzqcy.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3khhgskbi.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3ssyclfkj.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3cuemzazg.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3yjtupovd.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3mfordjnz.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3cesjgskw.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3hysclkrl.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3ydbzvivq.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3drrnkhfv.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3xqijfwtq.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3akcvlkmm.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3wfsbyqcr.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3puapwizs.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3lpbkrzij.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3tfmtrpcd.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3upjmywqv.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3qxjhfino.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3sjhqajhn.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3xrunefly.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3fvcssdnl.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3ptjgncig.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3wwzceoge.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3imuxrias.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3vqboalts.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3lmowswxg.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3ldlbnnvc.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3zsypxskd.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3qxvrhjzf.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3maxavcbj.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3ffnqtzha.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3htrczjnz.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3rnjxznup.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3qjuxdwgj.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3ztguforn.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3iwbonskv.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3evuohnxj.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3hyazydmm.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3msqynksz.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3rsublrqn.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3prnarsdv.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3lvuskrxu.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3cbnbrkcg.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3vyajbfng.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3arrxqmlv.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3dgvpufxd.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3henfxdjk.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3wdrjhsif.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3wbdutvhu.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3wmpkdiuf.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3gqctsahi.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3shetlpqu.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3poxglyuo.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3ocyqysml.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3fyukzjip.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3yxotxjgd.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3nzulwxld.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3qghfglfa.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3ofzdmcbi.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3htfncmbk.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3pllxmhlf.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3xsmownzi.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3irkodyay.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3dissroqi.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3audufquj.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3pnrhuhqt.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3eylkidtu.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3vreybqcc.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3pwqebtfi.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ccowyukw.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3fbcxfknx.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3vsdhpnrk.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3trbnkjku.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3eyegpgiu.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3dkpwkltu.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3qwnkhrnr.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3tqkeascz.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3ypvcxpwr.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3kixopwxo.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3vewxmytf.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3ppfbitim.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xbevlkga.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3cnoimcxt.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3tllumkbt.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3mlyycjlg.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3wizontwa.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3kkpprgxb.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3pqduepcg.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3ozylcojx.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3dpjbqsox.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3ooitimuq.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3gjfnuexv.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3fdrvgqrk.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3pydtqzpu.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3rewhicll.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3cdcyuaez.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3prpaxmay.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3amvtwuio.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3jwjiahkp.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ivzgdntn.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3ftythgdd.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3bthevlad.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3kjgckxxt.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3ffysnlyx.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3nblbvowo.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3amegnmhk.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3lejapyhq.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3nuknkcjd.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3hanxctla.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3civcyvpd.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3fqkwgrfb.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3ieuichxa.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3wcgzyzqy.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3kkefhvvd.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3fsickjii.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3pnwynzjv.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3jwfvgelq.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3vfrgttxk.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3qizhvdro.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3fbtladxe.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3lzoddkgv.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3jkqbkrwg.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3hwwrrhkw.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3dccbvnzz.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3nvtxczei.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3qcmjtsog.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3qixakgef.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3hkfuorjp.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3tlbuhghv.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3ecvyenof.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3gvyczkcp.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3ksrdylgj.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3pyjyvmes.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3nvmxdihf.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3sargpigq.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3gzgcrkkh.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3xnausjdb.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3rwpuvgbt.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3qaljfgeb.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3moxuxqec.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3smnpvgfq.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3wegpddsx.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ijemcooz.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3qykaaoqk.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3gzgnpqie.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3mmafzolt.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3tsrkhxej.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3datzelcx.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3mrpawfix.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ulfsqdho.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3zeecvata.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3wgxxewzd.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3nepuotma.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wquksdse.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3vxcfvoss.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3oyupktub.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3ausxigrw.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3zriqnwag.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3gvytkyou.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3kldxvbff.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3anrijqjg.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ujgaymxx.html


<!-- 参考信息 -->