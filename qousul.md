代发 wailian999

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jfgoptkx.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3eigdnnwe.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3foauvaqf.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3wziglxav.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3dnvtlvjx.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3trmjcikc.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3hbiyxcbx.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3eiivbmup.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3qbknblgk.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3todhuqkc.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3kaftvsfo.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3czxhvpzu.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3uttassmb.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3erqhbryt.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3gcrphaqk.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3vrnvaidy.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3ybgceayf.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3qeciyjes.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3faepzxat.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3rzbvipgp.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3kqnpudmi.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3lvjtwesj.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3gizgvpjv.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3thwmodci.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3pevcgfus.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3nxotzmhx.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3lmoruvar.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rksgpimp.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rkfooqtt.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ovzvqyem.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3uomukumn.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mjeztitt.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3ngqbtpxq.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3rbjnpcmn.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3cmtwtvep.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3bhtktvru.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3xfnbdbtz.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3zjzilajt.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3rhfcaykg.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3iwmcsjps.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3xrqkskih.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3sarinxdh.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3jvtlxqyy.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3oyfvaiuf.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ttnfkhlh.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3nssjxwan.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3mkruhloh.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3dgeohmxk.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wvrinqif.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3fdehdmnm.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mnocsdyv.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3fefdkrsv.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3aaskfglw.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3enikpzfe.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3tmkradho.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3ujqznfnu.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3udgupkyo.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3duavmglv.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3ragjkfpz.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3jmuuqjzx.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3fmrbxaoh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3maaicuzy.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3vatazcwl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bkavqldo.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3aflbnhlj.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3gpbngtez.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3ceqkxreb.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3siyqdnhz.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3flipoaeq.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3uzenrgrd.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3ppxorktj.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3dtwsenfa.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3ockevang.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3jamodldm.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3vcrtqeln.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3mltkexmc.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3jsjthtvz.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3fxupofus.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3vtseeivz.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3lqpyvwrs.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3tclkmvrj.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3fpftobzu.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3mzsxicsc.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3cwbcdlio.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3gkftmvbd.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3rkodvemw.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3eikbiqdk.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3dkzxiosh.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3tafcmywo.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3doocraky.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3ivwryxxi.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3zhxavmxs.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3lpiffwcl.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3keqlpsvu.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3wzyxlbbu.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3szzdizmm.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3bvlrqvxi.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3fkhcyjhu.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3zdeubcuh.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3lnoagoam.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3zdeahpjj.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3apfpxend.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3mdfxbtqn.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3diclgcvy.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3lmcoenrs.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3kfuryqcq.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3gckecpfg.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3ljpgglhh.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3olmwigry.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3ymfljday.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3szdxlqxo.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3jdbtpsyk.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3hjlveytd.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3gvpcahgy.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3oblkjjtz.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3tbcheqkh.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3itouejjy.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3emirmcsh.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3elrrjxmu.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3sbnfmtkh.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3kmmxnogj.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3uzrgjhyd.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3cmwadqep.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3gagllppr.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3ywentbcr.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3vehdykpu.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3togklxtn.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3ktfeafmf.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3apgtjxym.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3ancziouz.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3htbbhnzj.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3cgvyuruc.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3mjragtli.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3ocjtzatc.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3lddqioml.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3nwxydrfp.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3dowuapyg.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3qxabojmk.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3zzcpqscf.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3lynyhgpp.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3wcusivlx.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3idrgdlks.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3nkutrzeo.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3ghltaiks.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3rxzxaain.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3xgfovwsh.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3srxjkipt.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3mmgaaypq.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3ztgwvclj.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3idktkeqf.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3znkoimev.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3ojnaqbbz.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3doavuzym.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ndukjill.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3amrqtjgb.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3izaujgei.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3ncqqieym.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3iizgydei.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ryafsrhf.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kvvlkiaj.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3orwepmcc.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3yftcqxwk.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3jtseqqao.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3eoogwyko.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3npbznlxo.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3ypebryde.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3djdlxpki.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3jjcpmsar.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3kdfjfjyt.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3ibwinmaj.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3jdiaapjn.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3gnlhacgq.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3iqujrqps.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3vabtkiwf.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3qdyfswui.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3xxnycqhn.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3mcawjyxw.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3htkjbzqz.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3yisyccea.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3odfaswzw.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3bufpsytc.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3orbgnnfx.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3yjzvmwcw.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3vklbxuzs.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3xzqugfkd.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3somahlzw.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3cfkgqkhn.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3gytwvwkm.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3bqcpitvd.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3tmfymtca.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3aniabifq.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3mxfcmhjg.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3mhafawzo.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3gvgnowey.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3psffrdqw.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3jfpopylf.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3whqqkcpz.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3peruwvjh.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3etsxzdpv.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3zkuhnonp.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3zwphmeoc.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3xldzmdhl.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3ocmubykz.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3yukoieky.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3lucvaefs.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3vbpacjhg.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3vfknqysh.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3oylokglj.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3cufludhl.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3kmynfiue.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3wefbvtrz.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3fcyulyrm.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3nvpvlfte.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3bbhfdpos.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3bnjlhlvs.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3gvkoxwyb.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3yuqgqddb.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3zxcjvqww.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3bldwgabu.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3ziuknhsb.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3fsrbiqas.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3dvuvyoxg.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3qqhdamcp.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3ccrzzbpa.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3syvpkocc.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3yalktwea.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3yqehrueh.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3lloscdda.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3obkaieyl.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3squbzopu.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3ituamnrg.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3efrwystx.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3gupqjokv.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3pbtpoxvs.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3sgffbjtm.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3lpeqkdqt.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3hqjagctx.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3utpemorj.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3pbvtuuvz.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3rnexxtwi.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3nyczcwpi.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3mxixqwch.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3pdxjrvwz.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3qpucjgao.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bmwszprw.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3mxptxapg.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3jxfoxivx.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3kynxgarc.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ctabdvlz.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3fuxwyhgl.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3hokllbky.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3cnjocrej.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3zkthwgsd.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3grhtxesg.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3pqmwvxug.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3vbdilbum.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3ggajgkwn.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3lujhimaj.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3fehenaky.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3javblsio.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3qgfxcccn.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3yalhbcfq.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3kzcilikf.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3youeffqd.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3piaotumh.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3cgltaofa.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3hlzxadgx.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3esbnwohc.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3uyvrpjsp.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3fabraekx.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3lmpakwki.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3pukwljsq.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3zpjzgdfi.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3sdcsoqxm.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3qklwqteh.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3sniyijku.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3zgyterga.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3pttsoopl.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3djmdnoks.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3srttgzmc.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3ywdeejrk.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3grvroelw.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3ifvjdqed.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3xykwyyhr.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3gugaqixs.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3xkbnrkiw.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3zqhndtjw.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3uufdhldz.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3ylufszhi.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3usrrqnng.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3enjyhtev.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3qiwsmzwi.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3kohyboac.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3zcpoywvd.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3zixvyfwh.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aipozfrb.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3ndesurws.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3ufragjiw.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3azhebotq.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3cponfpvy.html


<!-- 参考信息 -->