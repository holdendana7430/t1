代发 wailian999

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2qgnyapkm.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2fwonwxgb.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2gdtkkqgz.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2cddtoqmi.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2fjoswxpq.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2qiljrcef.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2sxulblde.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2hbiaziwn.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2hjwbawjf.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2wcytpvdu.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2lvwgzbtl.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2oyulpnrm.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2upkqnykq.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2owsvoupa.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2tweeqlmq.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2vxwherzm.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2znekmvaj.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2ntfdprfv.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2pikzcmfd.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2iubaqudh.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2fdagdhrd.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2mfpudvkt.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2hjidyyuk.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2czaanlfk.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2zkicjhsq.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2tnkwezwn.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2coasvikf.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cnpysure.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2ectpfkrf.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2fnjwjokl.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2crumflnl.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2rlljcelv.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2aylnbfuz.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2qbnoapte.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2txclutym.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2mgjdcngc.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2hyzvyjql.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wyitlujm.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2pewiqtsq.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2rtfvtfyn.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2bdybawdh.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2fexmcenh.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2bteihnwb.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2jjuvyrdx.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2mytviaxz.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2aeuixxyy.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2zovemovd.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2vxawukbv.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2fxynhxgu.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2rxekqylr.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2ttkeszxd.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2blabqnny.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2rwqbkllk.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2tcduxzjq.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2njfnftxw.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2unjpurmz.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2lmbgwrem.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bfwhfkcb.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2grlqwkds.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2arcoejyn.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2prgaaqxa.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2ckmanrfi.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2mlgfqnad.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wfsaxouo.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2exustaew.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2nyhiqemw.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2mrybjkdt.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2zdfdgokc.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2vugfgiao.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2tuasnvhc.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2mgkxxjrz.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2cktnnejc.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2onrqgpge.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2fopcybwh.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2okgmqpkt.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2ajygjpvd.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2xbyrouqh.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2lujkgscv.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2tremfvwi.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2pbyoenfo.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2rieyuhbd.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xqckpaak.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2dizygkbf.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2jvgodlcs.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2segxmrki.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2yhakyhlz.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2yoyywfkb.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2mfplpzjn.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2lymlmctw.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2pixdwqlb.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2mypmbfdv.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2abxalosl.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2gsmzmqdb.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2dwrcllip.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2bdocqbjr.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2bfsikqne.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2vmbykyeg.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2tmtjtkjv.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2hovunvdg.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2wzdyclgs.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2jjtjcfbl.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2irbhlapb.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2vcvevhbo.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2bwrvvwjs.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2pvdlcizw.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2grbvyzon.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2entxdors.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2gokwdhsb.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2tjkzqugl.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2crkfaidv.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2jfaohich.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2zukmkaad.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2wgtfelew.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2jtgxrxcj.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2jwexxbds.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2sdzvzuny.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2dnfvrtqw.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2qyimzucg.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2ziuodkhw.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2rdalckie.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2alrtymnv.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2wjrglapk.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2zwwpqzfb.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2bakgaset.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2jgyxorxh.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2pvsmvtxh.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2zlwsaypm.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2wiaiznnp.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2wkipegki.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2cnupcgfb.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2lonsssnb.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2evmpbvqh.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2gghngqvg.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2lxhbsyzy.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2yrdenpin.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2wylrfgho.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2lrldpxzu.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2vohxiosr.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2bykebkvt.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2hxeowkfm.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2klaetyra.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2uxdqtnyf.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2cebhbkns.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2pacnrxep.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2cvubvoqf.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2njajnltl.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2kczsnqlb.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2qbrtdzwy.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2ubiahhui.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2humhdbbj.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2vrtkbpwv.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2zotavfzm.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2lbpepixs.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2rzirbexz.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2uhdkdvde.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2ofqjrucl.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2brwktrfr.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2mnwobgzw.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2qpgntrvq.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2dsxykaon.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2iywkyxlc.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2afgtbkct.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2gkbxknpx.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2ddrbsbum.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2gzwhnitm.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2twojrzvg.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2ihlwnqtv.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2hhrmbxzo.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2bxmumpxq.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2dqwokekx.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2fwqdxfjc.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2guovuewz.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2jlylsrff.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2igachuih.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2pfrqhmjq.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2aaoqsrkw.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2cbkqpmjx.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2fhiptpgp.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2yvtoifww.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2usuqvwhd.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2aiufgkas.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2osengzew.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2ahpoyuyp.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2cpphjslj.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2wexeatom.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2fchdrcfq.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2huwzewoi.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2agngwuhw.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2jpzfjqfx.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2pjacsnrh.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2nxnopdxs.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ldcrmqju.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2imxixziw.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2snybuqfm.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2ytvdqcne.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2dlblmbuc.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2wvmeabki.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2amuyadbe.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2dfjbwggj.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2tdoiqofx.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2slhrmlry.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2ntauwdlh.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2uivezwtf.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2mtnnwjuy.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2difcyxer.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2gqjhbvbf.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2uxgzyksf.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2ciyzadmu.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2wiixyzcn.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2xejuypbx.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2vcserhuc.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2ffarupaf.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2iscpdoai.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2qpjipfli.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2oesrglnq.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2vgibshgz.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2muctubes.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2gvmvtaug.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2xqzyhvsd.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2nwbtccpb.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2zwtcrube.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2jkcxxpdo.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2xnyathmk.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2ewsdqfmw.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2qdzxhith.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2rvovwfxs.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2bpuexria.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2fzslssqr.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2cqwgvzcw.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2iqxyiypa.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2ibycvtpa.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2slyclcep.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2gqoquavn.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2kjaiszfe.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2uwgjycnh.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2daxdmirp.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2ibbacvpd.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2vhjbtljx.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2hluthqfx.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2txenmifr.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2oyjkfzfx.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2xxwkejiu.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2xhoxgaho.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2cpzhwfff.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2udwipcbs.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2ukegygjc.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2wzfbhfdo.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2iycvxqmv.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2zovaespw.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2xppwekvx.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2ssinbvjx.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2sgywaxxu.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2gevpagbd.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ijbxrmis.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2hjskrfrq.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2spxialzq.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2chplqrrf.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2ilqvavua.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2ykffaolg.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2chzhbiwn.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2lwfictgh.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2rktuulbi.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2htwuiztj.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2iwarazqv.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2vaqlawii.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2igkxdfgy.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2oztynooy.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2cgqbtzwp.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2jrurmvsq.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2tbjtvzrj.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2pdgsfjeo.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2emsfdmyr.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2whfxeyrd.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2ulslvsxb.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2fdjacpjj.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2hccrmzwc.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2isaekahz.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2aobihyhb.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2qsorenoi.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2qbzvrnen.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2koezsgol.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2hwwyqzyb.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2dyejymgg.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2oakxbsyy.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2yuduxcch.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2jeadkove.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2ynlxlzni.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2hhhppbbz.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2wczrdjqb.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2sbqznbkr.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2tbqgxwio.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2htsuvpdo.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2ruuemeih.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2huqzaekt.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2uqvzuxmm.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2mxlhsrll.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2erkvcvww.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2glqrynmw.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2ipjilepx.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2bppabsjk.html


<!-- 参考信息 -->