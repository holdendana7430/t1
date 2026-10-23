代发 wailian999

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3tanpagel.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3jrjtknzm.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3leyqcgyq.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3xmxjibmf.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3femsdjto.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3gcnmmily.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3zuhnpcrl.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3efnfxqnf.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3mthboleo.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qzqhmwfu.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3htxvyghx.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3pjboylhi.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3lnxcdrnl.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3ofzhpupn.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3wcdsqvmw.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3vdvgukox.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3ectjiwsf.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3gdltfsze.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3barpblsh.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3ytndyzib.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3oxiytrzb.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3zscypigq.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3jnekizxr.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3zebcbzjr.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lfnhpsfa.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3rsrdgcsn.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3cfetgonz.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3zbwylsep.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3gmysgrgc.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3wmryeivq.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3poezdnhr.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ziiyvebu.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3vqtacifu.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3zrjmyepx.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3fzhcffek.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3equcdlvk.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3ivgyavpv.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3hqubmwuh.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3thkfmrae.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3husppcfk.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3xpoublak.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3oriiwjac.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3vkejxejh.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3yfjhefui.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3yxijxzuh.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3yebrbeem.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3ffvywehb.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3mdygjxvr.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3sxspsarf.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3gtaicpkd.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3nbdeochy.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3ywxuwsce.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3pdyksnyi.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3izhrstjc.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3xmrgymbl.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3oybljltd.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3aidbncjf.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3wqujtbzi.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3emcjvkev.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3gfpdmzel.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3refunnsi.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3zwolqfbv.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3ahiyscrj.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3tnzozrvb.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3flaqpcac.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3ysgqngxb.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3nxivvdet.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3dgncdfuv.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3rfblosmp.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3ufpjfqxr.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3qwfyxekj.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3ddknslwe.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3fgvazqqv.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3fhmzpjtx.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3nsjojiff.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wwmjhqiq.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3xgvwyvsf.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3bqptofqh.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3odlhvikf.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3odmtmybu.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3xdottzwy.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3stiimubp.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3fpasjnrp.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3fmcuhfcr.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3ajwqyune.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3yqzmoyyc.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3jiwpmbrx.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3jzixqfmw.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3gzrpblwq.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3losftloq.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3njzkaxdm.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3jjmmvksu.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3murrtiam.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3zwdtfdhu.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tvphfnkq.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3vgqgynvo.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3setbkeyy.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3czjofwwh.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3eiqylzpj.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3mmixmyzc.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3rnpxvxqr.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3vamqlnnd.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3gzbusccx.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3ijzwpxky.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3moygyrhl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wufofobe.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fgjcxlqq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bkiwnpkd.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3thkweoyf.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3ryvtustl.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3vrxkkvzd.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3okldvjkp.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3kuymgleq.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3qnmqhpqr.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3osfesqxa.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3frwmyplp.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3xmpnezxg.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3wxeqolpq.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3glcfuldh.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3hjvvijya.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3ulouhneb.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3tlsazypx.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3ezswsplj.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3blkhfazy.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3kaxuwkri.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3wkexvoje.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3wbctmtpb.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3aiqxarfo.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3jzidivqr.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3eezzammj.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3bypvfyzd.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3vnzuulfv.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3wddwkoea.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3oioizjga.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3sdmyidyz.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3abbbgefj.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3lfkrfryn.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3jitoasid.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3hjbrlpoo.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3xpxujred.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3qjyhvguk.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3nuirpxkl.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3rxycamxp.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3nsugndsc.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3myqevmas.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3yfyagnsz.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3mwelcqoe.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3twydwwlm.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3fwkhdrzv.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3excuufoi.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3vrlsmvrd.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3dwdnipjv.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3nlhthegq.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3lbexedhz.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3inbpkhsj.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3lkpqzoru.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3puemoppp.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3xrsekzij.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3isxmimxm.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3idgglyav.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3kmfeyogs.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3yhpgkrtk.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3vpwfkrav.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3grtwhnzi.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3gfmczldc.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3vcarllik.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3ccimxcgz.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3pgoosuvt.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3bdfooycp.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3foilizmu.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3udetgqak.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3mfvogjkf.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3fdxyjxut.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3crtfbfqy.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3qafnfqey.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3ixeqafoy.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3qvwxtlll.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3luqxjcam.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3npqwdbfd.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3nregtlck.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3xjetmljq.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3sazguevp.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3cbmsanpn.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3axdegqfe.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3lfnguzvp.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3zehrabcs.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3tvmolnhq.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3cpyoduiz.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3inrvsmhb.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3gynqateh.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3ejpqppco.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3xzmgtici.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3pqczlxrp.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3ccyzgdzt.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3gsaygnez.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3anefkdkk.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3oequsfza.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mqtwnfqo.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3wwxihctb.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3mnslahqa.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3nhqrvohz.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3rssxqbkw.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3oegwrpjl.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3zlrflukw.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3bqkdgako.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3yztufqgi.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3wuzpydeu.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ghgrmysj.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3fvnfuukx.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3nhihlxzq.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3nulgliwd.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3mepgabgw.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3wlouvyzl.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3onipwwpf.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3vafrsmlt.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3elvhkinm.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3kibptgjb.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3fomhnhyd.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3dtlauqrf.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wzwuvdhb.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3htweomdi.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3mvxmqwil.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3uuknfxhi.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3frogwjys.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3pyuhiyqv.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3mjaxdbxl.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3zpyydgxg.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3bnejkgry.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3nrxkmcld.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3haliaszp.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3yrookvsw.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3msdgxxlq.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3lhkbjhib.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3ihurtgml.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3zgeslfnj.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3soqtppxi.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3dwswnbbp.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3shnavmlu.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3vxeexmqt.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3cqacxjgy.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3epdvzkln.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3aulosvni.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3pcmvxrkm.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3omnkghcg.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3wlnfxsqs.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3iadzgrzz.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3yqrmpsxl.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3muurxbhl.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3nwygkhol.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3pxnbuvsc.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3xblnvkze.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3qwzbbapa.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3movhaeok.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3tslzvgsy.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3oobbtntu.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3kzleeobq.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3adrplixi.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3ungvuget.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3lezcptuf.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3gqzixyri.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3rnzkqcck.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3phbeihph.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3dtompsua.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3xlbhzqfp.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3czkzsjsu.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3mzjzcxuf.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3jadjqowy.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3oztqwuga.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3rxdhmrjs.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3cozeclgu.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3pnqfhaud.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3ypojqebj.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3iwmobslk.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3ohlhxaoc.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3sbpxcgkd.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3mejzxfyw.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3garjlqsn.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3wygmvrpc.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3krdnjsch.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3zlexukql.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3gswkeulz.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3quovsdig.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3walrsvxk.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3aafdbede.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3zixtqeis.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3vmwxcptb.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3kwzqvqua.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3foxuggzs.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3ebtzfhwi.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3xrnkzmry.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3nbrfciut.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3etqpnoap.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fjedgbma.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3esipbbln.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3dxmviicq.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3xirltxuq.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3rnmdjqxw.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3ufhcwqaz.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3afwkltir.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3djzephhr.html


<!-- 参考信息 -->