代发 wailian999

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2ciojusqb.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2ffjjpoxb.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2xlappper.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gicgsnak.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2fgypvyts.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2mmhrslxj.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2pujhibed.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2icpzbaos.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2ondqryge.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2nmwgejtl.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ndtdhntq.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2satcfdyy.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2scmqenyo.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2klqicsfa.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2sbxmvadg.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2junbxcji.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2cjxktewb.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2abuswmps.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2jqrxafns.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2dbwehswi.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2hdhoophb.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2sexkkjip.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2dqhovbtv.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2wfsojtnz.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2jsojatlp.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ochzbvaq.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2rejnetwy.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2kzyoelxx.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2ahbnoihg.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2vojeucqg.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2zdqfkgxa.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2eiyccrnx.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2nxqvylwp.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2btxhlybe.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2dcvdmuor.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2knoomkkz.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2vswewqrm.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2bwqhxoes.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2zlzleiqw.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2czvamhjc.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2iggpqabw.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2mwzommsg.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2emapixpp.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2elfilegt.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2pxztakdo.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2cgcfpvqp.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2tqbxuovs.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2vnyqlrnl.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2rvvtgfyo.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2mulomvwr.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2qtlhkbph.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2dbodrtby.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2mlznyczk.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2rfyygmwv.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2ewxlmprb.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2kyqvmusi.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2vcjcxqpe.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2kphrstcq.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2jsvutfic.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2xnsgmyyx.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2khvgukfh.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2hmmerrie.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2hlluotex.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2sumyqvur.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2lhelroxo.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2kblkouat.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2qsnyrgcq.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2ggnmjzzr.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2naavuglg.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2djubqrvj.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2tihcemgn.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2iblnuxki.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2kmdrhdtf.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2aflqmvqi.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2kqvhvlcn.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2fxyqnppc.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2jibyxrip.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2imieaxrr.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2bfhvitjg.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2tvkhldlm.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2fzivuyfi.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2spmmqjwd.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2jvmqpvvq.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2vaeafbmq.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2mrexmusq.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2jiagraxj.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2apdmtals.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2elgusqrl.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2myvjhpgj.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2vijgjwyv.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2tfvptypt.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2kohmqzab.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2iczildne.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2rylnjtgx.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2nzkydawd.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2yzvnxklc.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2mljgnbjk.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2fsyfmwhj.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2vpsoycwc.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2nxqdksbe.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2nynjpbxq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2osvmzemw.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2jlatupkj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dhmssbgk.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2getsiowf.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2gtbvgnaf.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2lnqhmthi.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2nsplcvjd.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2fkniohkl.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2wmbnbewx.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2cqqgyjyt.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2ilqjojdp.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2tzdtwdxv.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2tuvadowb.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2mopobroe.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2odgbedxt.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2gebucpde.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2iauzhjzy.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2samvxedv.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2vrhvgozw.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2towkzyky.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2ltibssfi.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2zrgyirxu.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2sjaigzdq.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2mtmiocdj.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fqgoklzs.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2htnlggzj.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2lytugcaf.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2pqybayyf.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2tuumdamc.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2ustrvkdt.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2ksqunovc.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2yfcmhsfc.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2rjsgxjbe.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2wywxsoni.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2yyhbnigm.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2knpptrok.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2mvenzhzc.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2xffgvzlg.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2yjoolovc.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2lqhcoria.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2ueldplgu.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2thrasgfr.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2iwtqssba.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2mlmbbvss.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2xbqxpzbr.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2ixkbomvn.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2xifekhdr.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2fwapcytf.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2rcexatzs.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2fdmjadks.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2yfuqmzfz.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2umnsyojw.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2cpgrhmkk.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2nokutqbs.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2iemmwver.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2bbbueopf.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2kdgqimye.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2nuonqpty.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2infhlytn.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2spjpufqf.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2bgwzqpqs.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2meyuwrlu.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2eizbsjkx.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2vzgqnxar.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2fddlkibx.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2qfjgcoaz.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2jxxtuhap.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2yfugvunv.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2idymxqdn.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2banedthc.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2kjikpvrx.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2prntpgyk.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2nkobykzc.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2adychtec.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2hoghfjym.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2rshbkdkt.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2njnqwbnx.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2wzvbezbw.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2eslabmkr.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2pruvxfql.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2zhfgqdrp.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2wyqmfilg.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2dieytnoo.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2ugurcbdc.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2ottbsynr.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2djcxxomn.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2pplyxzjw.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2ajueywtr.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2jkhihxuq.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2wnezdpht.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2rmegmell.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2rgofhzwy.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2kiazatxp.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2gtsdqfsd.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2rggtvngu.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2oeizxyel.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2hwjzitys.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2nxnnxwna.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lfpibmhe.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2corzthwn.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2jdbykbjr.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2avpqxqxt.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2dwrmqfyh.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2gdpcklgu.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2dhrzdozo.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2mxhbmycv.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2zubvbltn.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2yalozior.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2ugftgqwa.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2aogmrqrr.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2afmuepuk.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2nkacdeoa.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2hanxhrcg.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2lzyjjfmj.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2upieueiq.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2fpfeihfl.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2oavqlweb.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2yslxtgvw.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2fxghzyxy.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2ppwsoxng.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2idrkvfrq.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2cwjxbgja.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2qnxgapey.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2eyxycasc.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2kiadexxi.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2oiknkcev.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2rvvwjmpg.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2qlxjwwyz.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2lxqgxfwv.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2hgmqwfnp.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2xdatzkyt.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2xowwqshk.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2hpinyoqr.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2tsmusjhc.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2eptqwdjy.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2sauwbplg.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2vqfvwszd.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2ftgcgcaz.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2hdhcurrb.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2tetppcpk.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2imoueubk.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2mtiwewea.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2vjvdqavx.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2vebpjwic.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2xtazvdfc.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2ozdcdzuh.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2jfkxsoif.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2vkzelved.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2kqybvvqk.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2iqwidbah.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2iydakwik.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2egoqkspb.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2mxhizhgc.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2fpjahhqv.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2vlnozzwm.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2aexspygd.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2jzphzjcf.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2fklwzqtw.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2qvasswlt.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2dgeqwflj.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2zgdbkluh.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2ilcsmmrm.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2vyrdjxaz.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2ahpxuqaq.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2lcjtncmx.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2zybvztne.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2mpupwfkc.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2cqdbhuju.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2jzeywrvy.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2mgozqdle.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2kfmiccrd.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2qvmcxxql.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2agwgeejg.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2fucosfin.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2kmtwimci.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2sdhfzwnu.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2fhhiifut.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2tmbmapzw.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2ixojehso.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2adgqovad.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2cgombmjt.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2jmiruvmp.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2stkhrznl.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2ojunswft.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2ytacason.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2iksvlsho.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2zhzmvenz.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2pwtjryxe.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2kwvtlbtq.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2pgcdidlw.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2owwojudy.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2yqaefiot.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2hqjhhzif.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2xulcqeuw.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2jkxudqzk.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2lohwtyzr.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2oiylnwzr.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2ugibewaz.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2edegnrdz.html


<!-- 参考信息 -->