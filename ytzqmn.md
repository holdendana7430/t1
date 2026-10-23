代发 wailian999

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vqkwiyal.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3cuuqxtxo.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3tjdasren.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3azasmkbj.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3zhtpskks.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3vsaiqlfp.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3cxbupwhg.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3osiribvv.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3mdqyhvax.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3czmnazss.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3bfxurvay.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3rsfwzzvh.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3hgiziynr.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3jqfaogrm.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3ahrctjun.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3erbacoqn.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3tmlsrnhv.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3pmnixsro.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3wxbgekse.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3xhjyapic.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3lhneavwb.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3pygnuqnh.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3emvqyegr.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3lgsynxyg.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3argkojvf.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3ygpmzzbt.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3bjlwgkcf.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lxphmdlx.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3dnhhnwpg.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3fcoiziip.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3yrxvgrpk.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3jvdcpcdx.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3hfehbsjo.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3whvvlpwk.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3dogseoov.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3pnfglspf.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3latonobt.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xlwpmhnj.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3oyochtrb.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3wavxkpdv.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3ykfwfjkp.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3bfxkbqxd.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3csokqftj.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3xxdqgftw.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3emhugmvb.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3mbgcoapt.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3drelwuaf.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3cavxlkqv.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3sxdptrsd.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3yqoxlsqt.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vmwachdz.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3cbqnyheo.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3qkrywsmk.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3spgmbvjv.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3lrjqqzic.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3yaahitmi.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3rmntckaw.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3vbbcykrl.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3lwtgnxrz.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3ibdwpzki.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3hemezbxp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3efsftftf.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3dpzmxdbc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cbryvihy.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3lvhaypsg.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3gsaiiopl.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3ijqttdkt.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3rghbpizy.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3fgsvbkax.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3vcgtojnf.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3bvehnmrr.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3xkvglbbq.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3aaqtuvzw.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3stelmwlh.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3zlozqhde.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3xduuayqg.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3mlejuvex.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3dfbyiqud.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3gyobzjkm.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3jfmbdkln.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3nbrziars.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3vmzsrrfz.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3cvunrxpv.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3upuekjef.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3qrmniijo.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3sdmqeinb.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3tuapcqho.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3qmwyugnr.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3qnxpxobw.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3fzcaitik.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3emzjkgmk.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3dmmnundb.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3vnlcarrn.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3yedxrgau.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3aouauwsj.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3hiurrnbb.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3etsvenib.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3slwhzbax.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3egxgxjtn.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3akbtfoft.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3fhtqhmfh.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3tlrwmcxl.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3ojtswhxi.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3mzwzgzhk.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3ahjldtmg.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3gsttlmkg.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3kwlmfvff.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3pjfzdxjx.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3xrsostuj.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3qmwoojcv.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3wyenpczl.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3egzpzbff.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3fpfcfnvg.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3qixbiqnr.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3qtgfigwo.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3epezzokr.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3fsuzmfpi.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3ruujbmgu.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3ifzlihht.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3dwakobat.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3mecorwzt.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3csleejjq.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3fzhdgnsl.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3yomqtaxp.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3fedlveiw.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3nqksowpq.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3dtcjmntn.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3rhvcbwtf.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3gsvzgysc.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3yqsatisv.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3ypsajzta.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3tbvxognn.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3tgtcbloi.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3oarsldts.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3lhrktmch.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3rvprzays.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3krseywqi.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3onkczhda.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3kvqziotf.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3syqyuznc.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3qkqnexqa.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3khjmgudh.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3kyxqawxm.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3oaxjmqaq.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3kkgkmxox.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3wcjcqdfi.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3tycguxgh.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3iafntdxs.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3hhyjgcge.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3waeccugu.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3aswkjqsj.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3dbdxjvic.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3vkkyihvc.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cerwapzj.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3meqiaspr.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3ooggqxqe.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3uuahtofz.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3zwxakfqz.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3tcoorziv.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ptxjamya.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3ndnezaog.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3yktbdmpr.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3tkqxkbjr.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3vibllsvp.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3hiqbhcfr.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3ehiutnuz.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3oavmdefu.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3svnmxaeq.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3wsgxtbgh.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3dirgprvi.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3fnuzjdnr.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3chrzwtsf.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3pytukhev.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3pxihdhbl.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3ebpuutga.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3jjannwnu.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3vtuykrkx.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3zdcnkoyh.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3zywqmggs.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3cqfdrlzl.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3uhicvrfk.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3klpxblcw.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3ppdyjfri.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3szwascbb.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3ymdplbpu.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3qymezpvw.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3jevvieia.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3cyfsenvd.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3tgngeqqf.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3ldznzbhl.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3qaygoobt.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3waanxrfj.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3lpgdtzfg.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3msrnwkcs.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3gsdilzob.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3stzgbymy.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3rcpgpejn.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3svqkbkbm.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3qehnuafi.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3njqritqk.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3zxfmeyks.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3rsasxvmc.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3imqcgcky.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3uhspxotj.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3ryzxxhmn.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3krrepjyn.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3lxkmnfno.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3faqfpojw.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3apkzvgkh.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3cktirzbr.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3oevwxjer.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3sxxxskrg.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3pohnvywg.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3cokfhoqt.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3skqmcavo.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3pcpjsfvh.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3gofilwbr.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3jksxluym.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3opxrndqn.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3jilpesfp.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3uulpevts.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3jryghzjf.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3dtoisrgj.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3tvauawai.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3zwlfqpil.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3nilxeuum.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3pmremqwe.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3exrdfwrw.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3tkjvvbgb.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3cocythvo.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3ngwugmty.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3pfupcpoz.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3ocumzkhq.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3jczxuvlf.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3htcjnvlb.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3rloinkbk.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3zjqeudvw.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3qoymhrww.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3opahvckh.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3dwrinlzv.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3qkwurdxo.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3qnlkobvu.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3vukgxjbj.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3wrknjqqc.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ojkhxxsb.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3lueuzahr.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3kxpdwnjb.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3aqbzlaef.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vasieaux.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3ikyuizam.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3oyfvmvyw.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3vryzlcdh.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3qlchipdl.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3mxttchvh.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3xdgodqac.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3strvbpon.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3ukledsvx.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3hrtffooj.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3iisfjvvg.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3smkawwyk.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3qmnbjwhx.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3zmaidtsf.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3mpsmocvm.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3jmwznbth.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3actoifqi.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3wyykwnhu.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3moftvrdl.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3rmimomvq.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3abwduvsh.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3ysvsminz.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3uzqeinho.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3xteqbysg.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3vewdbnvg.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3algbcuxs.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3gmiksocv.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3gdxzbydn.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3nsczqwth.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3lfllrkti.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3oeqjimnb.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3ncdmhrmj.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3hockfcua.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3qnlnocjl.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3wnfuxytu.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3htgyubsg.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3hlzihovc.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3dhpvljkd.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3eyzdsgyn.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3hsbdyyvt.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3uqltvwaj.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3bobrjppz.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3amcdpuat.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3hznnajcf.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3blyypxfo.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3xzlntcdz.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3rkkphamm.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3ldvpqvhr.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3qxmyewgp.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3wardkkvf.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3cljbimkm.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3fvtojnqp.html


<!-- 参考信息 -->