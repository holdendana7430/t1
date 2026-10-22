代发 wailian999

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2ufedutzw.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2wgfwbuzi.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2qxhceblg.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2pbzjzvzq.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2aqwgewfe.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2qctcemru.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2aicdztgu.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2kbbfkjdr.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2kapdseit.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2xpivzwdb.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2dpunpdew.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2drilumsc.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2bbfyioqk.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ibrqgcrl.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2vreizoav.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ggdhciqg.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2ewlzgmiq.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2uiilachi.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2gqgkolik.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2dfnorqqt.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2atqjuloj.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cquixuhn.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2gojuuvfp.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2sbipccjm.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2mndwmqhs.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rqjhcpcs.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ospptnbl.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2anqxbylv.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2iaokkhyz.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2zkhwyekn.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2pvqstjmj.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2pocntinb.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2ihovvwwd.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2dazjawcf.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2maanlexw.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2qbfmwitr.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2cwekxafc.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2ufrqikxl.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2yozrxait.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2ttubqkfw.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2zprbpuql.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2wcknivxa.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2uirsefue.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2eppurzde.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2bwkiaseu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qlwbpkvs.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gzoqedrl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fovxrsiw.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2czwifhgg.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2eibgqkjv.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2biqznxch.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2gcneadhe.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2btsjbqiw.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2tuvzsjec.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2hxhsugjw.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2ziuhqsov.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2wufukbut.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2wxsbvzob.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2mmdhcdxx.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2fasrttjs.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2gobmmbdz.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2jybayqwn.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2mbanobei.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2amjsldzy.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2kfmepjai.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2nobyffra.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2uiufvekn.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2wxzkvgld.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2ixjjvzwb.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rblhsfii.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2ufbqyjpw.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2kaiyrrtu.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2jliatcaq.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2wdrckcon.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2gcohpkgh.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2gfexwprb.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2lrhitrog.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2cfnnpjpu.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2hpkgmudo.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2okvokdqg.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2adnicgqy.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2wexicvsu.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2obuuygpz.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2ecioiiej.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2pceyasgm.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2kqztyvzp.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2ojldhuca.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2zhtglxxb.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2xnomkjaq.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2ovubxhpd.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2qqvsdxay.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2buoqbstx.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2ldhqkoan.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2nfajwwgz.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2bhtjfjhu.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2qhgionyi.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2kgcyimud.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2irbsdyjq.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2moztxcbn.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2wjigtemw.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2ixfucbvp.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2fqmenznm.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2okxputuz.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2sqamuwmb.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2jztuwmte.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2ougryskw.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2rcpuvlph.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2geblxmnx.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2zebpprrw.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2hjqthlbm.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2aroicpbq.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2quwerxje.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2ugdhwblm.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2gtgapgyh.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2hrhwfils.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2ucrzsnrl.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2drzwxgcn.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2nlhjhcic.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2xmdfdhlb.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2dpgoercx.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2kmkkldnb.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2ndeiltjy.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2lvzpzfkr.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2fueaejtm.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2fujjjier.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2wrrajbap.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2czixhixk.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2lrsjtzaf.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2jvgsitth.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2jorjhxpj.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2aadkydko.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2qblsggha.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2peavpfsi.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2obrnjanm.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2zogsrref.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2shsziwph.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2qlnoerip.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2najtytjj.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2dpemsacu.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2tjpesvdb.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2oxkottzk.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2yfephkka.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2mgmnwlpk.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2owhmfaxg.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2fcngdmvu.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2qxvwvmvz.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2czxusltr.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2sassfqyy.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2irdurbld.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2jzhvnywe.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2ruselpit.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2dyjylxiv.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2odmxfhsu.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2sxncwbxr.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2jfjsakbr.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2ocjqopil.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2honvrtht.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2pbaagrdn.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2koaukbfp.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2dssauxkm.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2wfcwhuvj.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2qiatghiv.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2vkbgexhm.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2ijdqjmyb.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2kbqngnlt.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2mlnpygdc.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2ebfsyopr.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2mjtfiebi.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2bokjksvm.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2cnykmbes.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2cdatfudf.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2hkaolzzm.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2gviturbu.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2dgjpgbmr.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wgwqvhnd.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2frrwvqkz.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2gavbfwfv.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2cfzrrrkl.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2xzazjsub.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ucabixjp.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2lakxpmdl.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2rrcvqgib.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2fsnvwqhq.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2wfipoabi.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2newupkvp.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2lkuvmeqs.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2tlxszmfv.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2dqvktdhf.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2hdwadfrj.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2toiregzd.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2aldxcjha.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2tneheqsh.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2pedslynf.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2yrqmkklb.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2zrnegtxz.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2twexyslr.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2zjfvhtik.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2jdsoymnv.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2klhgqasa.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2tqxaoobj.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2dejnotxs.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2icfnwujf.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2wqvmwsul.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2mgoynykm.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2mfnzlgos.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2bwzltjnn.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2jzodovtd.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2nnyclsdd.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2wwnacvrv.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2uqppwleq.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2quleujih.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2kxucplwu.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2xdohjvsi.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2ioqwnehf.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2scghkszi.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2higynxeo.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2nskedufh.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2gfvxbhou.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2wcspzvhm.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2yzyvhbsq.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2yodxhgti.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2vhbmanpt.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2qdfyjaxu.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2cnazqvgx.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2hbibdzbp.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2diqrmhji.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2mpikzapb.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2xtkbmjco.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rvnodkys.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2roucmpvl.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2kqaskjag.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tfxrwaac.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2aoagijtk.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2wqqibxgw.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2pxjdxjwm.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2zwqegsgv.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2jyoivesb.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2mzzladty.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2ajmwendn.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2vcunkpjc.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2cmiomsen.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ngtcvioe.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2pequraek.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2thswyuvb.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2mgyngery.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2dhwbjcri.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2ueulildx.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2ylnojkpe.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2pflhosjt.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2vykpoqdd.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2czbisaui.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2zqlrbbjs.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2iytrevzg.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2ytpscyft.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2vxodwvel.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2bybcngsg.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2dlwrmfij.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2luymbpig.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2jlfileke.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2nrmsahlx.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2ancoanqv.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2xtwachsj.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2xuqgtmyv.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2chcvlwgk.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2ljxprtua.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2lasrecky.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2uscdazpg.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2sjfrapik.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2tktsrijf.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2ejeeyjbe.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2xozzhemd.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2qqxxhema.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2davuubcf.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2yypqtyuo.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2rhcqakkl.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2rmhzwwyf.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2gqehtlob.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2kdqkioda.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2amupqtca.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xqgjyvzv.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2wvadojbo.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2nivhajau.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2bvmqoeld.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2kzgihasp.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2eafvhlry.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2ckjfdvlk.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2nqqwkzwe.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2pphesezz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mtbjaejz.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2rybddrga.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2crgvhhmj.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2ckejvvlk.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2lrjbvmai.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2bpvlcnjn.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2sksregrt.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2ksfugevu.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2goqllbro.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2mccbqxev.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2aftkndvs.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2xmbkjucu.html


<!-- 参考信息 -->