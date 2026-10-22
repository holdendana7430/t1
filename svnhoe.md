代发 wailian999

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2faaztysg.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2dvuvppyv.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2mjxunhlh.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2lpszunjp.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2aogyixqg.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2nvjlkrni.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2kwrpgyjd.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2wdkgueup.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2rwdajerr.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2mplfqpmi.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2wvylcobl.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2uhanhabk.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2sprjcjfb.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2gtmhfwmw.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2uhratfol.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2tljjxqhp.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2tyiyqerl.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2vucnumon.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2ysbijsjl.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2xhlucxan.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wyfkaefn.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2xozqaqqu.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2cxsdpcbe.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2jnsnzbmc.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2aewaxtet.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2paibqewj.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2ruhuyksu.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2hduqzlqh.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2lrkawbxu.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2tllixxlr.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2mrprkumt.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2bisxvdvs.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2kzavocyu.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2koymsina.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2vhdrdcnd.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2foruehvw.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2mwglylbg.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2tlyqhwpi.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2qvfbfuxu.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2gaecxzsd.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2dlimrfak.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2gueowgde.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2nkghjfpm.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2pciiqmfu.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2hgknyuwc.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2xxcqzqzw.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2nxbhnihk.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2veuciwai.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qymididz.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2sscnucjt.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2qoepyujg.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rkhmlgjc.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2qyelgcld.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2fgthnphs.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2clxskhuz.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2gkayoivq.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2idsqhrjo.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ncqogdwh.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2hresgnrq.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2saziflkd.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2etqlvekw.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2zdyzcuke.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2akhhints.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2vzewuxts.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2zdtvirxq.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2hxrahngf.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2boaivfdx.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2thswrnuj.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pclyagxb.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2oawvmgto.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2pqjtsjgf.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2hekanerz.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2mezzeocl.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2yphonnpe.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2zbwlgjvg.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2islegeli.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2epdgnbdr.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2lslsaskt.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2qyxdqhyf.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2zwfnqtkn.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2wdaksops.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bwobdxrd.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2tdkxxdlx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2slfztefu.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2zftfyhkb.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2vkgplzkz.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2kkfzvojg.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tloelzfc.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2pkcbzjyl.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2qggxsgno.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2ujcyqsjw.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2vegtjchh.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2vntwyozk.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2wvbaydeh.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2pdycuias.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2tgvbfmuw.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2bvafzakt.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2mnozmtqj.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2tuewpozr.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2evysuees.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2ufkbtbyk.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2yebrczan.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2txwobgcp.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2uakmicyv.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2inxtuqkg.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2kdgtoips.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2eosjiqun.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2amfrafeh.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2pxkfiykg.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2oefaatau.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2heyyieyi.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2dyfbnhkm.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2yplxbmbs.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2dfnfzijo.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2fovtduuk.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2sutjunqv.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2nwqtffml.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2mfboazjh.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2renutrfv.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2pahaddrf.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2hujxeplo.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2zpoxwrgk.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2agbhlwjm.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2dtdxcswn.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2nabzkima.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2ohehebvu.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2addodiyn.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2gtenyyor.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2gaupbkpd.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2qrgrsvve.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2tmmlaaoc.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2nfyipbzd.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2zcmsqxsa.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2nrkpjxwx.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2xyfwwjen.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2pwbnhihg.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2ftussqtp.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2jczadstn.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2thbkuxzm.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2vhumcrgq.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2qqplzyqa.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2gabgvkie.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2jrdixoyl.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2xmhanjed.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2fqqicwwu.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2idozsxlb.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2graeassk.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2htvilthv.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2lwzuoyes.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2itsgbaml.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2agvgrnxq.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2smqsrxpy.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2iulvwpbb.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2qorjblcg.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2ttzydjbf.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2lbmomufz.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2qjdfwxpg.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2zgvnizmf.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2occfyazz.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2zaeujbht.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2wzosqcyc.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2djnmzawr.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2sccgkxqe.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2fxtoyrkr.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2ubbvbyxs.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2ysfpwzoi.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2jlexhepx.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2kbjkqkmx.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2hkwtsavs.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2mvxjkrzq.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2mtlbumjm.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2ouicchsq.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2ikflpxhu.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2enphmazl.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2lhgojdom.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2mydffcyc.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2bxstrncf.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2hmrkezoo.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2fzexdvgx.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bmbnmfgb.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2mzitzzzk.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2nwmxslsp.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2kzljzshj.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2csruaxlm.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2udgdrlqb.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2sajploiw.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2crdtnfmx.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2joookrqs.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2fpoewkub.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2aoshszub.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2aohwbntb.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2atwcijwl.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2hqypbiel.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2zdgjxcdk.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2pidvevvj.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mdtnxjdj.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2somgahjw.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2ckqmflvm.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2gwadborq.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2nvlvjthg.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2msspraok.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2lbkzssyr.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2eisymuff.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2nsrjbdlm.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2cnqzcstt.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2wkrnvfqa.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2liytajer.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2hharrmvc.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2iqkwpvov.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2jydpqmje.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jbfzrakw.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2hfafzmkl.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2qtaiugmm.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2obmyykwx.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2ginqawpa.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2fyygjaki.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2njkscjqe.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2lrthzmpn.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2xqwjirlr.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2azbpzxxm.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2iwzyuewi.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2mmbvpnhr.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2znjecysv.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2guoxfrfd.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2inpkuigd.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2txhfqmao.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2zwzghuln.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2soatpsnv.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2zweipvve.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2qrstcfhg.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2upceciiz.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2ubitdply.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2lhcmemhi.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2adexdlkn.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2lyionoxi.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2pvmvjbao.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2gzzgxwep.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2tlyuvnha.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2porhkgwo.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2ziuqizub.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2mexpbuzc.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2tuqemiek.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2aaedclqz.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2ntxhfdrx.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2dxkhtdwu.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2fggbabve.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2acjjjudn.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2qqikbjbr.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2qvtbkiyc.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2vmnhwcjy.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2bjqcseya.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2qhvpghjz.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2ssngrmka.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2kxkuybdo.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2fdttvonn.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2rfahjdgk.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2fttsgxyb.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2qwjxesoq.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2pepbceic.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2zdkibnes.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2lmhxrurz.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2xuahxbgc.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2hsswjpsg.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2sfsfzjrw.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2oypqsblm.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2hgakaclk.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2rjnufeve.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2ktqzmoob.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2hhtepeqi.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2qcbjwbxz.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2olfwasfs.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2msxnyolt.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2rsmhmzvv.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2kyylihmw.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2bwpuplrr.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2ohbngfyi.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2pdivubki.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2binxvubk.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2lkvnfkcq.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2xgopslsx.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2fmbxdkbg.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2wbyogzkj.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2xqgsrqgr.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2vptjvoew.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2gavrgqqs.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2sthaicxz.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2anyhcooi.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2amyzqqde.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2xkojqhhk.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2gmzvpwnw.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2onbzmhah.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2zheuopyg.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2tipfvckp.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2ufoadjmh.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ksnizdto.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2pjjvjshz.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2jfvbozdo.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2hywqiwtv.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2wftyldwj.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2vjutbphf.html


<!-- 参考信息 -->