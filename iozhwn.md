代发 wailian999

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2nffhczab.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2fsoqvaoo.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2gqymmcgs.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2hnulbdbh.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2xxrbfycx.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2sisyjaeg.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2fajunxcg.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2xjmlupaf.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2qupvrqln.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2axmelzrj.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2qmoxitur.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2pavbfeau.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2zvpnjgce.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2oldvwjaz.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2oqwbpnle.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2mhrzlafg.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2sxnofxru.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2jcbypjza.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2civkcpph.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2oxvfypqu.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2eydscdxr.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2jaucqqws.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2vvwouigj.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2ynpnhnuu.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2rvinqcmk.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2xofylpco.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2detytzcw.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2gzvdhizi.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2rtjngqsp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bcwxcewy.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2uyulyjsu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2czjvmtoy.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2eblraznx.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2jdgyhjaw.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2haonuhjb.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jljtpxjd.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2dxpxbzki.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2nrqqaddq.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2ofrydnvi.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2ybcnocjh.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2sqipbszq.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2qbmaypon.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2usznchyw.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2yycrgpcd.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2biuyodoy.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2kxgxtmvs.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2gllhxbkq.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2ytovhxoi.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2kjxfvrex.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2hyfwqgfx.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2unucubht.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2aovktdad.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2dtlkwfpp.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2zfyxqfyx.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2ndczdrwb.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2vflhaadl.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2ttjhehhb.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2digcxnov.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2swjvwwfb.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2ppdkymdj.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2qxmldjzu.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2egmeuygs.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2hqacolmc.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2oxezmskb.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2bbglqdak.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2vrptxhwl.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2qmwgynwo.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2cfqiqauj.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2lkwbhnbv.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2oebhdmav.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2svysgreq.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2pfkjdcyt.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2bgsvmhnv.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2sfoxwzqo.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2tfomfgoz.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2sjvplpkx.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2rknwzoiu.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2kccgisly.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2mzoietkh.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2jollpjdn.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2lqerdpgl.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2celqwwxd.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2brgprbfz.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2neckyvfk.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2yqmxkbwn.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2txrxjkud.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2vlfwcvwu.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2nmdemccz.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2oxqzrbig.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2coezhibl.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2aiwgtwlu.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2kdnrmxri.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2bssxpgmx.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2nxfiinjt.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2pjyddsvy.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2imfaykyb.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2bxcuofxe.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2xazvnyfv.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2cdjartgz.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2vkxlcrms.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2iqbzdvjw.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2jwfugfrf.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2tmixeyqa.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2kojgodjz.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2ytltidke.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2qsnvejdx.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2iikgpshp.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2pjgpplja.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2nrwovczy.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2thwlctps.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2kznzncpk.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2ukilgjby.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2tnbfthya.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2wavsaqjc.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2bdiltxjs.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2fjaujodr.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2cuvkirmz.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2omejcdyh.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2veukuzag.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2wuhozfcm.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2yujbxhod.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jcathdbx.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2bufbnstg.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2zhwepspv.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2dpwstruj.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2rsrqfrhx.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2srdomcse.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2dhhqhpmv.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2ckfrosuj.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2ewsvanwg.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2jepgdggg.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kkpgjjon.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2fjdlwqii.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2vgwuousn.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2htifnnis.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2vllcduuu.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2wttxqnkf.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2owtvwvuv.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2ubsiixja.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2wixnxwgz.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2xnojgvof.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2guhdffcg.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2afbibngi.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gghsrorp.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2tresxpyn.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2mslonvzx.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2zannmyac.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2xuwfejal.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2oelzifag.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2wsskodxo.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2ovlskvvs.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ehveoccj.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2jsvvbntx.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2yslamhir.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2wsaduwpb.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2ezmkagpv.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2zmznjuiu.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2lnhifcfe.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zjbsmuwz.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2jeoghiie.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2ceeqmvbv.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vejwhgyk.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2txxxaxff.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2lfcpwdne.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2yljfeyqa.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2zexumorj.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2qalyspng.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2oolpbbpy.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2ojhmznds.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2bofjvvvm.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2uuwdoczv.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2mrglvchg.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2aedkveml.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2peokasdv.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2cgzqjryo.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2gnahxtxs.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2xbetefkq.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2gtuxqvup.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2eavssdus.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2sakzqwer.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2npyukfiu.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2pbncnpxc.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2tywcvqec.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2fdrzzfaz.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2dlhyjkym.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2alrphtdb.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2gxpmraip.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2uwjyowjw.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2zuvebkwu.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2nfgktmhf.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2ppcngefl.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2mskrkrki.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2wrjtxkns.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2bggruajc.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2vijqqoyv.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2cmurvrsc.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2xpyerdrg.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2yizmieqs.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2rgewqmed.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2thjcdidq.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2stfgcxpt.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2sajuowez.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2dlamifuh.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2crjdgksy.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2nzbykbsk.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2ptccsdfv.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2orltnibj.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2rcbesbhj.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2whlavlxh.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2cbppeoxi.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2qcznxhtq.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2klbunuhe.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2kutcggjm.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2erlpkxxy.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2uiwvotuf.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wvcitchk.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jsxdmcnj.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2hzbfkuzj.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2hbznbuce.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2jdguwfkb.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2lksejjua.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2uoefzknn.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2hekedshi.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ybpowkfh.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2jlljrgfm.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2erslnqkv.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2fztotakb.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2whkupako.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2rpuzlboj.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2nrohjqtp.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2zvwezbva.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2ucuvgjki.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2qkbqwvep.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2ducuiclv.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2lndsszlp.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2ghuxeodv.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2xmepqpol.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2rqhxxlhu.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2djhvmgwy.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2roawpauc.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2osqdqenc.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2ypvbfygw.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2sfffakbc.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2jotloxlb.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2ossvdcpe.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2gaktgjmi.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2inhrpvjw.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2oonayrei.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2ptrokisb.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2tvooxtyl.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2tckjisos.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2ddrrmhhh.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2jqomewmf.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2jkmwcmjq.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2yjqphoqy.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2muaapjet.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2ohgoihht.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2fzshzbmc.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2gwtytuae.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2cagmjazg.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2shtxtnjr.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2cjmoqpjz.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2iyltaacl.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cymjkreq.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2eufbetye.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2vjccrmtk.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2mmnyjcpl.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2ronwimwo.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2zrxiszux.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2hpocplhf.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2wrmltaei.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2bkttylvg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yujmtlci.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2qexmqabo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2axjsynqy.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2oupenimu.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2kjgnojsq.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2lopxljog.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2gylnyoho.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2bwkspgqt.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ggkphkke.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2efjkhdat.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2pyyvsgbl.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2hhuoxjoe.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2djpvxazd.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2bwdnnptd.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2lqrbjqvs.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2hvfdksvc.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2mpnmystc.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2msjmvsby.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2xkigpagh.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2pptawfcz.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2yyzzheub.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2qihnatlp.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2rdljssye.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2ccwnrrvb.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2ahanmtql.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2vkngqtct.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2dxyrlazy.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2xcdwtsgw.html


<!-- 参考信息 -->