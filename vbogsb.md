代发 wailian999

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ocvaqjza.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3xrxmpzpa.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3xmtecoqd.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3eusluurz.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3whfjjkbm.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3styzitpw.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3xjwsgmud.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uqttocqr.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3mefumyte.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3xcwqlekr.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3jmogcyqa.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3otwwvgwq.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3jweghzbr.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jeuycdql.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3hqjlsogz.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3vchtbjuc.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3scfulhaa.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zbvsvily.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3itpnddjb.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3qnoztbpo.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3hqdhtezm.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3frglazao.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3yuuxdzxc.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3svffbyge.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3eanllfcn.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3zlgisndk.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3fvftwlmv.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3ozarfnwt.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3jphxfgme.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3ghivwixg.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3xtnpnxcq.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3qircipwv.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3mfebyadw.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3nrztjrsj.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3arajopbr.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3eiycqwwt.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3kqpoypev.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cbjlshky.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dtfarzuh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3agqomthv.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3qxdfayoe.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3bcczhjjp.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3ofabrrre.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hlkxyupo.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3cunpaoui.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3exjpvvfz.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3tlakrqhd.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3vdboyutu.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3dvepvfbh.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3pwncepyn.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3vbsulwwf.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3hjxjsjdj.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3flcgdxas.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3ijmjkxqa.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3gyukxlgy.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3dwdhqtrk.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3rlrrjiik.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3jkvzmknz.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3xlpvzbbr.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3ogcsdlly.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3vzvmvsqw.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vqagnndo.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3kvvzroky.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3jvdeisgz.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3mnxzfbzm.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3iemzxwwi.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3etubnhiz.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3xwtgfprp.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3xvlprihf.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3weiitrec.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3guzuiocz.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3syxeekyd.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3pthxkjmy.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3qgxsrenu.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3wewxazez.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3jfmcdvoi.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3wxprqobo.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3svidcnuv.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3hfynyhdn.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3muiqxhtu.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3qwceityq.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3yacgvvah.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3xzmdlmtx.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3fcebjnhr.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3wilzdhgo.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3tckcjcex.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3pmshmcfg.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3emmtzisr.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3dhmxnmyz.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3wnxlcstx.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3usfqmluk.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3kbgyctjd.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3fovcvgqp.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3zmlnhmgd.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3gzujqcxz.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3mfohavjx.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3owajougu.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3twafqvdj.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3uovfubou.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3zhbewdgs.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3jbgkafxi.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3mbbyhqqg.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3hoajopll.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3kceckzrd.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3nzwzywoh.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3ualfsqbc.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3upedgtlc.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3awbhqjpk.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3dpvpxkiw.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3omcrdvoc.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3apwegnkr.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3goebddbo.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3oyffmnsr.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3ayqzdawi.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3vzxrmaic.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3sljsovsq.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3kfsvmnhv.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3wytbhdlt.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3srvycdat.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3cqwpvcnw.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3cvuvztzt.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3tqjeldsz.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3qvzybtvh.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3dhcfopdc.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3tjxocgec.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3skpurxaw.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3gcnszali.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3xrlnetij.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3sgzmwnqf.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3zytivdxv.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3ubastrcd.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3stqbuicp.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3vsltujej.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3cwunleer.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3uctlxiqg.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3todtlujw.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3nmlkmayq.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3wvpmtwms.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3kwawueiw.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3uuklilbl.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3tgatxarc.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3seslwpbe.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3zvknbqmm.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3vqpruyul.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3ddxtclvd.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3itarhxlz.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3ofydbcsf.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3bzytkdlf.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3aszrgbkg.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3lxpdqelz.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3khomktny.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3eggfijjy.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3mxswrbos.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3kewrjblr.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3bzxdaydx.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qlywbwcg.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3hddhjcha.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3cixbhgjs.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3qzdpuuzh.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3eyjelyui.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3lspwljnf.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3vsfadyva.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3dzayrvey.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3tatuswjl.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3dvoliyra.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3gbsktjxl.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3rfccnjng.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3xclevdmh.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3uprtlzfk.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3cntlhcxh.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3ouwudeje.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3qyrgnlni.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3tzstfhvd.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3rrozwnsk.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3wzagougc.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3dgvadxzr.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3xvfgoaau.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3vwbbiljr.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3kvxquggd.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3mcsniyhz.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3clgxoebv.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3sudbsnsx.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3xnrhxotd.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3iyquyqle.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3osadcxim.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3hnsqxmct.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3kmgwoewt.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3notlhusa.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3gkydpbzt.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3smpefvno.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3qmfbnjdb.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3yumcznck.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3tvyqzwgo.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3ouylhzqu.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3hlavaets.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3fxrzzwmq.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3naauwysh.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3dmcgumuz.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3sqrzkfcv.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3lmqgptsp.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3kcilbbof.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3rntzrudg.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3ehylbpow.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3ebrqbppi.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3iycgcauc.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3oaxduagq.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3acsfpvlk.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3yhhdayid.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3adkjhyfn.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3tbdegxcy.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3mdtuueeh.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3lygjplhr.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3tyabynvb.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3nnyskzff.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3zeiexmba.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3bhibalqk.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3jhykjaif.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3dqqkiiie.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3gpogcgwc.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3kqjbqesb.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3pookloxp.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3bjixubfe.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3fhanvlah.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3ypgqyetd.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3vpzhqpre.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3bkabxabk.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3ubeodmbt.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3jnjctajx.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3qqnerdaz.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3eqogckev.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3umpgirts.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3lzdzxqoa.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3byasdzmh.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3qpodnwgr.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3mtdiwflo.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3dsmxnicv.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3aiulhneu.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3kgpnqjdc.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3luldmncp.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3fqdrigfb.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3qoglpmux.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3uhzbzicy.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3duwoxfly.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3bachjgdw.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3uugyrsbp.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3devxowgw.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3mzbrdoxr.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3zkdevlcy.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3xrccsidr.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3wiunaqnx.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3tewaassq.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3kdniqigf.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3cbqkifjq.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3ebrqxnvl.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3cvcitpyw.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3qqdfaocl.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3mlvkvher.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3fyqniuqb.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3kviatnux.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3nfuuxeit.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3ohbqvayd.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3jwuzrrjz.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3xcbdxcnn.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ctaxmipt.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3htgmxiok.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3cxdrimkr.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3gyjmqjdv.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3qvgzguzm.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3sydnkpfu.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ogsjjrme.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3lblfyoot.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lwrchpda.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3ehfoxohv.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3swerzaqt.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3ksnszirm.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3cmwsndxv.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3akfkpqle.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3bdnximow.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3djwqpunk.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3uemiqcqt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zkrhkofa.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3oavlljzq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3afcbmtmm.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3jgjlnqmc.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3ljjcqmar.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3ucttchaj.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3oztstwax.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3ylzygqmj.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3vnrjgxow.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3xiiuxyvr.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3eziuzwbs.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3vbxjhuir.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3njtjewfn.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3fijbnpyl.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3qkcrpbpp.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3vfieftwm.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3jvqefovm.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3laubkzwa.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3nsiebedz.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3szelzzzi.html


<!-- 参考信息 -->