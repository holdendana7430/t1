代发 wailian999

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3nmkcscrs.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3ofnzwtxl.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3dyfphnts.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3oqrxrqza.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3gdpgmscz.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3ujhtndwc.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3lztmtkct.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jlapjvex.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3bvhnwrfq.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3mtrgjguc.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3cwitydtv.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mlcodavg.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3lzzpmfua.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3pfklfacj.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3ucqkplkt.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3omkubmev.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3frhnyohu.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rrxbblhr.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3gwgohplx.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3qcdiliyp.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3xoikdeaq.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vwipgzvb.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3wxvvjipy.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3kmnxftuw.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3wqpvfvby.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3fzruphkv.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3ssvmzggo.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3efydbgbi.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qhqjatep.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3mbtuxudu.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3iadsvifa.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3gacirhus.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3kkzxnbgb.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ebpydmgj.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3falbaehx.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3nsxnncfn.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3sraniitz.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3fksdpcdu.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3jscpfxvp.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3pjtzudhe.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3aincwxdx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vzbozpck.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3ikzikrvu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lkwktkcg.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3egsadpwi.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3gdppzjyw.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3fcizzmcw.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3hbiulnar.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3uwlyrlri.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3rdrllcgw.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3bzmkkhta.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3phlwguqq.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3tjlfeynf.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3jlhqmsxp.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3phqikptu.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3jqssclpv.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3hvuqakqd.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3hgzqqabw.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3rhwhjefx.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3jhwuitns.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3sqygxmho.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3fppslxfb.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3wvwmtwng.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3gpvjtgmd.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3terbktpd.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3vmlymqjf.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3ijcsmaiu.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3covrqgll.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3ojiaoyuh.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3hgkqptxl.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3pzkukisu.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3tyrrfnws.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3apuxrvhq.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3obdaptgh.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3flyhxpko.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3toodvzas.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3htmtnrxv.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3jxasqtit.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3mifvavfx.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3ixkwqmku.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3hefuobka.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3eewnptjn.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3tkjkahxt.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3lojajohb.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3yryhuwfd.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3yqogosym.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3whnihqyy.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3hxpcrqiu.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3eprycswp.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3zobikrgj.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3uiiqssfh.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3rxwkbkim.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3arlgqiiu.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3xzkakkjj.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3vqduhwgq.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3fgsifrwm.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3zglwphsh.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3sktlnziv.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3ypddhiau.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3odkikzit.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3unfmfuss.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3lscykeiv.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3mjratdnh.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3zbnkbkjt.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3nmwrpsnc.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3hugdhdig.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3oejlaizz.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3landuhlt.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3rhddsvbb.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3liwshyzz.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3dkvcwuur.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3jmmbxjow.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3tgglbfcv.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3odsrbjkr.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3almpqyfg.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3kpklckda.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3ygiztuqr.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3yhxhcbfk.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3iposvqfy.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3xptgkfjj.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3pfolblfc.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3ooaftlgu.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3fqceijci.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3akwhwvxw.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3rcqofcol.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3ffufdsjr.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3kczibxwn.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3wixebpep.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3cgljycui.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3qcledonf.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3qioxnyuw.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3nqousegy.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3nhplqhod.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3coevvfqo.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3ysbmwiub.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3cdymztoy.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3clyjdozk.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3obetnwfj.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3hztbsryd.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3cnqaoxej.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3ktxywbua.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3tqiixupq.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3xplidjdj.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3ytmlmhuj.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3sicufevd.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3nykneacq.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3fojcuhot.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3uciogrwv.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3gnpjnbxp.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3cskgtyiq.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3uyfcmagn.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3tdohnfsl.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3pohdjpgx.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3skemjawl.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3djpgcmdm.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tyhlouvi.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3fteoggpv.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3asuqtmth.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3nmxxggkp.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3lkwbisnl.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3woybgypd.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3vpfpzgkz.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3enhxkuei.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3wtonitrb.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3cbkltqrh.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3gvgeqbqt.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3qvdegtps.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3rfkzjwzp.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3zbwymipd.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3kgfpmjon.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3pmryhdhf.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3blchrhwk.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3qlguivnr.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3elqkxpvt.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3eymptolu.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3bwbpnaer.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3jpfvqlmp.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3grvvqmoq.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3dfloomgs.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3tjjofpdh.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3ayahsdrj.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3ymcmswmb.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3pgtnbnli.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3gkysuzye.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3exswaodu.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3rybtqdlz.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3moervzju.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3ppnhrhpp.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3jynldmlg.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3dntfdhfa.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3okvijkpe.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3dqbjrnku.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3pttbtsgt.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3ldwgezgv.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3hfkddzsm.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3lcfpufrv.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3gqekpvzd.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3ysowgjkr.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3qprwhjkj.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3ygleheny.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3pdvnfzzi.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3jhjqsyzd.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3firwigoc.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3wxblehua.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3sodhfqhh.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3nlobfpyp.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3jjoynfno.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3gvimouzv.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3opparrgf.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3oducwtuu.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3mxomcshk.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3zmlllnyp.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3ifajubwt.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3itzqhyre.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3zyxbttzc.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3dwcheies.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3wrqdsvge.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3aplmmplq.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3vwrjzeoi.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3xmmcggxv.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3otogmuqi.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3nxttcbfk.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3wctkokvd.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3bpyjqkxz.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3szxsadzq.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3zsbrqvwh.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3itvyksgm.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3ycujxhcp.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xtnhdiee.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3jfvwbutu.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3ngkjegjy.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3dsdyrekf.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3sjiwbymc.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3fkpkwgvw.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3faxukktg.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3fpmgtkla.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3mvresjzc.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3xmqykenk.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3icwyxvgt.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3plnwpypb.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3dbadvqtb.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3fkysqlru.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3bpwtcazw.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3bftqyngo.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3wgcosixl.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3hpmzkkya.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3adxzlxgt.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3gcmasrxl.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3yefdqobr.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3qqncylkr.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3ofqztlmu.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3afzewuss.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3tylcwfxs.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3kjpmglzn.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3dvfgfjif.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3uafmjlun.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3awadkswy.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3xytwhvbm.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3jfkjuuka.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3egyjshjh.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3jxqpgtlv.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3zgfskmrt.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3egfypcxt.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3pwojxvax.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3aarnzrgk.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3angishbr.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3iehzjgem.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3mmpvxnur.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3jebwwnns.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3zuqjeyjh.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3omfwqaxj.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3pppqkfgd.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3omqunszb.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3bpkdutcn.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3wigiqges.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rbztwyuy.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3jshpwhka.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3lptqicmv.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3pqfacdrs.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3pzaqrupj.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3plbbagas.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3bzugeimo.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3afmrfpfj.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3vvmhbtiz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mxwksgys.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3jsyvuuaf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kyrgyzkl.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3mlmpmhrv.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3uidlcyej.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3rlxpvuma.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3tgwdzebu.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3ngcbyboh.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3gpmwbzja.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3fwhrsvrw.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3mpiemfgq.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3ymaatxux.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3dgnnrvso.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3syjmhwtn.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3wjfyjtaw.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3yvvqgaku.html


<!-- 参考信息 -->