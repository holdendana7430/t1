代发 wailian999

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ldalivbg.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3ffzzccaj.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3dkkrecoz.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3trqhckip.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3laxfydzw.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3cjguuslc.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3spovulyt.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mgqazvfv.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3uxaanmdo.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ihniapvj.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3egpcapli.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3qywkokbd.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3aoljndva.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3xpoxnacj.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3ckygdycj.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3ftciiuft.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3zrxtijmf.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tdihdyyu.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3zsciskct.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3upivdvce.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3wopubhqq.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3amuwhbzy.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3zcvahccx.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3muabvmab.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3cjsgrpym.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3mmglsjon.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3duabbdyu.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3irgrdhlz.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3mrqeosgw.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3qrxlmrga.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3bwpzqobv.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3gbqqlhjn.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3jpezlcfu.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3clnbvkpg.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3ejwzqzul.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3kmdcrxvv.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3zvirihem.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3rmljttcx.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3hjebkktt.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3tscannor.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3kfitvavc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yfwvsgma.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3twpfrdrm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nwvwcfdn.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3oxysolne.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3haflbuld.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3oeweqsef.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3ucfhhcvs.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3lrtcvvla.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3mlhvgmbs.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3gpuozsnx.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3derxsayn.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3ymmmpfyp.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3onudredw.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3yyqzjnok.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3qjagzqzy.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3wvppyqjh.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3xitbjfdt.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3lqnnafli.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3hembzjoj.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3optittdk.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3codibmci.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3sbfhqygl.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3ximjwoqx.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3epdhdbdr.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3nxtbvnxc.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3xkbwwxfz.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3mpddhhvk.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3uwtknjty.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3phoayjub.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3dfdnialk.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3rcxspjpt.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3jzvmotgg.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3xmxxianh.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3zeiqqosy.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3xdbwxahp.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3nxeoebko.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3umcuyase.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3zqgnrgya.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3onpdkuqk.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3qsldgvdf.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3ypbidjbo.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3ggvdrneo.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3rrqaeurf.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3yvenqzfm.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3sdrifikf.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3eoeyyhxf.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3fyvukodn.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3llwzpzgo.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3trpmscof.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3nqyldoqv.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3pvrcdksx.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3zksttfoj.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3fvrrcnfe.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3oblflqyq.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3iyjciuvp.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3twnspces.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3wwnlcoad.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3owipccvi.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3vkhrqufx.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3twdquqvb.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3xyiykext.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3zusupjrr.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3geytzxgg.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3mbqtpkmt.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3whkpzgia.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3leebbihx.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3bajjeaqx.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3nerqozbe.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3nreabfry.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3xpbqloig.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3oyvtcptr.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3ijdwlamj.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3yjjxmpsv.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3rjymkmdb.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3kcvehtex.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3ornyjasj.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3ljbirqrf.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3scbpajbd.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3xjvcylqp.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3dnjzvxhh.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3cfzldrxk.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3choeteah.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3rhbceeje.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3sfvkruyt.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3ogjisscu.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3sbbadewh.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3ayeqcajy.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3mitswkxv.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3ctzjevbk.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3jfjbzqjb.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3hhqfravt.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3emntxzyl.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3gzxibcgn.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3vpunzlqr.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3wwsvmmqf.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3pnlikvxw.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3viupvfly.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3asvjortl.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zcveqjgy.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3ubzzuucp.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3buksykdq.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3fpdwgqfr.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aefmlczh.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3vvmgfwqt.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3tirzdmpo.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3asaqjcus.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3zzfahtoc.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3urambayy.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3zmyeyeoz.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3pxzlrywr.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3fdqtramv.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3zuipuohu.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3vlbmxnkb.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3zzybpwjz.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3qfvvadoa.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3slxpdkhj.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3xnlfhbwq.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3lygqxtjo.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3hxmjcwae.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3mkenbfuo.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3oocpzflz.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3vfvjmszs.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3phgjlxpl.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3iijoazun.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3bywxvcmj.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3arzfvpoi.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3mwoptdqz.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3oucjoaun.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3nhckravu.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3vqdevnbk.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3gfeckmey.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3rxgliuyd.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3esncphlq.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3cyqmvqgv.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3eapciddx.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3fxpgtghh.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3jejewguk.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3bdmyrmrj.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3kdsvdbvj.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3ttfpaxnt.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3ncbaoobe.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3gnnhomjw.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3kzftjdzz.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3ijmvvmjn.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3vpaoohkp.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3qxwwuysh.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3ntysqsvb.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3nwifehsy.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3dctpotlg.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3txmzeykm.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3iqnojeme.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3omqrdscb.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3hxbshibo.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3uqegmbgm.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3gzujssre.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3takfzdzv.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3fcvhxzdo.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3lmklbxvv.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3lgfhxtvu.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3fywctlig.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3dlrrgags.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3tijjlhhs.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3fnkgxgav.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3pjetzhdf.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3wpygxfgi.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3rygvispe.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3wvfjxwkg.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3qtqxqwfw.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3wlsldtfq.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3mgbjwtss.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3icpcfumu.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3hasbbegi.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3hjcpobod.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3rpfradgz.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3uzlgjozn.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3mvoxsqon.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3vzjvffyc.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3krizsvqm.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3levbfaip.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3ntdddqka.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3fddmoltn.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3lyqexhip.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3wrpbtsuc.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qymkauxy.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3hsioqamp.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3dgoftlsm.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3upbwasuo.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3czwvaiwc.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3haqzojnx.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3myezqqdr.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3uqcldene.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3mxmyqdhv.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3nvmcdhsz.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3byuwryal.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3rzrbywof.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3yppxyrhm.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3utdkqxul.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ntdbyktd.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3wvggwkqx.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3thtagfcc.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3ymozzdtt.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3rkhgilby.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3pdcqfurc.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3cpyhcikw.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3bpguwflj.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3zgpbzjie.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3lawbcirl.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3qvlerlfi.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3qqjiynxi.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3ybjmnlhj.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3wowccuga.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3ggkpjvnz.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3jwrhzlfn.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3syvtxqec.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3oqnzolxn.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3txzhuhyr.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3arokyvae.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3kxaxnfel.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3pwzddiqj.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3rhnmybip.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3ujtkogje.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3ihdoyxji.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3aqavsszs.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3ffogfgnz.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3xnmaemsd.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3wxghfxzb.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3quuegqyg.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3ezndccid.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3sbwoicek.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3yoruadnv.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3tztymvgd.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3utluynoi.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3wvdhonwv.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3hykrwucb.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3newcsycj.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3wqcibmre.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3sgbicuip.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3quorgmop.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3jusfubnj.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3jtodbdzu.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3yohitcab.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3egfwvejk.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3rvyqmexr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ssjwmoqu.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3cpcbokuc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gvlxitnn.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3haazorwc.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3ybpfnfni.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3menwnbkh.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3phnvghqn.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3lajpnswn.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3ghakdhhw.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3jaaizusw.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3zalrrwta.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3bflyvqgi.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3qrcsaspy.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3pancpvvk.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3akltywck.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3gsqbhjoh.html


<!-- 参考信息 -->