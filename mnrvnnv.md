代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwnnaqys.sHtML

[T55] Scala：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gbwurtfrf.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gioesfowo.sHtML

[T56] Scala：样例类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsmkwcnkg.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gghaztzat.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfsdhuekd.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.fanxiaobao.xyz/Article/details/giimcqzwc.sHtML

[T58] Scala：函数定义
来源：http://blog.fanxiaobao.xyz/Article/details/gzokknaav.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gosjukedp.sHtML

[T59] Scala：循环
来源：http://read.share.fanxiaobao.xyz/Article/details/goemwhnmp.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggayxrufo.sHtML

[T60] Scala：折叠
来源：http://m.share.fanxiaobao.xyz/Article/details/gevaqvetq.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.fanxiaobao.xyz/Article/details/gnhvwfkyy.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gtyazytsu.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gqfrgfocg.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gbjwyoffw.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.fanxiaobao.xyz/Article/details/ghzsaquwc.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.fanxiaobao.xyz/Article/details/guigogmzc.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.fanxiaobao.xyz/Article/details/gsehszmey.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gdjesyfmf.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.fanxiaobao.xyz/Article/details/gwfxodhok.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.fanxiaobao.xyz/Article/details/gajgdkcfm.sHtML

[U04] Py：变量调试打印
来源：http://read.share.fanxiaobao.xyz/Article/details/grzdbfnay.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fanxiaobao.xyz/Article/details/gykdvjwsh.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxlmpzizb.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghpstzwto.sHtML

[U06] Py：合并两个字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gzulhrpse.sHtML

{**a, **b}
来源：http://www.share.fanxiaobao.xyz/Article/details/gxdoaoudy.sHtML

[U07] Py：反转字典键值
来源：http://www.share.fanxiaobao.xyz/Article/details/gbdzwdlwr.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fanxiaobao.xyz/Article/details/gtcweimbm.sHtML

[U08] Py：展平二维列表
来源：http://blog.fanxiaobao.xyz/Article/details/gebpctbmk.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grlhrybeg.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.fanxiaobao.xyz/Article/details/gmbcklvpc.sHtML

max(d, key=d.get)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjjnybrqt.sHtML

[U10] Py：按值排序字典
来源：http://m.share.fanxiaobao.xyz/Article/details/glxkgvkou.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbrqxlhnp.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtwziwlcv.sHtML

(x * 2 for x in arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghkcqlmxe.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.fanxiaobao.xyz/Article/details/gewrfngcx.sHtML

Counter(arr).most_common(3)
来源：http://3g.fanxiaobao.xyz/Article/details/gldoztahj.sHtML

[U13] Py：固定长度队列
来源：http://read.share.fanxiaobao.xyz/Article/details/gnqtnffih.sHtML

deque(maxlen=10)
来源：http://blog.fanxiaobao.xyz/Article/details/ghyfmfrhu.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gprmwipqn.sHtML

defaultdict(list)
来源：http://3g.fanxiaobao.xyz/Article/details/gwsixqfme.sHtML

[U15] Py：高精度计时
来源：http://mobile.fanxiaobao.xyz/Article/details/gcyrdbcoi.sHtML

t = time.perf_counter()
来源：http://baike.fanxiaobao.xyz/Article/details/gvcrpvkzb.sHtML

[U16] Py：命令行参数解析
来源：http://3g.fanxiaobao.xyz/Article/details/gtpivybrt.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.fanxiaobao.xyz/Article/details/gutpincvf.sHtML

[U17] Py：初始化日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gmundbpaw.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.fanxiaobao.xyz/Article/details/gouxeofkr.sHtML

[U18] Py：预编译正则
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvmahavrp.sHtML

pat = re.compile(r"\d+")
来源：http://blog.fanxiaobao.xyz/Article/details/ggvjgzamu.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.fanxiaobao.xyz/Article/details/gwpiswecj.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.fanxiaobao.xyz/Article/details/gqgnxscxt.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkeigrfsg.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.fanxiaobao.xyz/Article/details/grjtjpjxe.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.fanxiaobao.xyz/Article/details/gnkmeffyw.sHtML

@contextlib.contextmanager
来源：http://blog.fanxiaobao.xyz/Article/details/gvepvhqrd.sHtML

[U22] Py：矩阵转置
来源：http://blog.fanxiaobao.xyz/Article/details/gtndkrnvs.sHtML

list(zip(*m))
来源：http://blog.fanxiaobao.xyz/Article/details/ghvjgazea.sHtML

[U23] Py：分块读取大文件
来源：http://blog.fanxiaobao.xyz/Article/details/gxqzvdpzj.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.fanxiaobao.xyz/Article/details/gfbcoythe.sHtML

[U24] Py：路径操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/godmaqcgu.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.fanxiaobao.xyz/Article/details/glyveapin.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.fanxiaobao.xyz/Article/details/gwoccrtxl.sHtML

csv.DictReader(f)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsoivwlyx.sHtML

[U26] Py：并发下载
来源：http://blog.fanxiaobao.xyz/Article/details/gjnutxuww.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggdaewuly.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.fanxiaobao.xyz/Article/details/gjauepfvz.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.fanxiaobao.xyz/Article/details/grwwbqbht.sHtML

[U28] Py：类型别名
来源：http://read.share.fanxiaobao.xyz/Article/details/gopbmdbpu.sHtML

UserId = int
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghirnaqvh.sHtML

[U29] Py：属性校验
来源：http://mobile.fanxiaobao.xyz/Article/details/gzhhmbads.sHtML

@property 与 @x.setter 配合
来源：http://3g.fanxiaobao.xyz/Article/details/gukpdkygl.sHtML

[U30] Py：数据类
来源：http://mobile.fanxiaobao.xyz/Article/details/gtzaznvke.sHtML

@dataclass(slots=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvqfagqbg.sHtML

[U31] Py：单测
来源：http://read.share.fanxiaobao.xyz/Article/details/gewfpqrwb.sHtML

python -m pytest -q
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guxgwteyc.sHtML

[U32] Py：代码格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gfvvguhvc.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.fanxiaobao.xyz/Article/details/geepyzsrv.sHtML

[U33] Py：打包发布
来源：http://baike.fanxiaobao.xyz/Article/details/gtvqcowmx.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.fanxiaobao.xyz/Article/details/glrhrwdfo.sHtML

[U34] Py：判断编码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gffqhmfol.sHtML

chardet.detect(raw)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghboitube.sHtML

[U35] Py：发送邮件
来源：http://baike.fanxiaobao.xyz/Article/details/gjjzqyfwd.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.fanxiaobao.xyz/Article/details/gjhxlazwd.sHtML

[U36] Py：定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gsaulhctd.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gthilkqhz.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtsghqptk.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.fanxiaobao.xyz/Article/details/gbvmprklf.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.fanxiaobao.xyz/Article/details/gszgkaoop.sHtML

Path(__file__).resolve().parent
来源：http://blog.fanxiaobao.xyz/Article/details/gmgneagxt.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbnckbpvt.sHtML

sys.stdout.isatty()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfioptymp.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gmzobdjsc.sHtML

print("err", file=sys.stderr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmsvvdymj.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.fanxiaobao.xyz/Article/details/gxzhisihs.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.fanxiaobao.xyz/Article/details/givmmfojt.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.fanxiaobao.xyz/Article/details/gxnidkdds.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.fanxiaobao.xyz/Article/details/gtzjtkgfe.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.fanxiaobao.xyz/Article/details/gjskvgzfz.sHtML

namespace App\Http;
来源：http://mobile.fanxiaobao.xyz/Article/details/geldnnzog.sHtML

[U44] PHP：开启严格类型
来源：http://blog.fanxiaobao.xyz/Article/details/gxkafiywn.sHtML

declare(strict_types=1);
来源：http://baike.fanxiaobao.xyz/Article/details/gvqabepkb.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gavkwqwyh.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjkueignz.sHtML

[U46] PHP：可空类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gjyslbral.sHtML

?string $name = null
来源：http://3g.fanxiaobao.xyz/Article/details/gvrgyowqw.sHtML

[U47] PHP：联合类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdcqamoca.sHtML

int|string $id
来源：http://www.share.fanxiaobao.xyz/Article/details/gqbrmbyqz.sHtML

[U48] PHP：纯枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gecujrrmc.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gsxsynmae.sHtML

[U49] PHP：只读属性
来源：http://wap.fanxiaobao.xyz/Article/details/ggndzudsv.sHtML

public readonly string $name
来源：http://blog.fanxiaobao.xyz/Article/details/gnfgbeake.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.fanxiaobao.xyz/Article/details/gtzbhlrfc.sHtML

public function __construct(private int $id) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gbyeynfnm.sHtML

[U51] PHP：数组解构
来源：http://baike.fanxiaobao.xyz/Article/details/gmyposfhc.sHtML

[$a, $b] = $arr;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwcnriwja.sHtML

[U52] PHP：箭头函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gnygueocj.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkktiocpb.sHtML

[U53] PHP：空合并运算符
来源：http://wap.fanxiaobao.xyz/Article/details/ginvkjdav.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.fanxiaobao.xyz/Article/details/gpqsuhcna.sHtML

[U54] PHP：空安全调用
来源：http://read.share.fanxiaobao.xyz/Article/details/ghszvwtqi.sHtML

$obj?->method()
来源：http://mobile.fanxiaobao.xyz/Article/details/glgvkylfc.sHtML

[U55] PHP：match 表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gbdzgpyas.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.fanxiaobao.xyz/Article/details/ggmezqvua.sHtML

[U56] PHP：命名参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/grxankjtf.sHtML

f(a: 1, b: 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/grtxdkjym.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gduqtskfu.sHtML

"值: {$a}"
来源：http://blog.fanxiaobao.xyz/Article/details/gskgxaoqj.sHtML

[U58] PHP：数组三件套
来源：http://m.share.fanxiaobao.xyz/Article/details/glzkglfkc.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.fanxiaobao.xyz/Article/details/gonuplsdy.sHtML

[U59] PHP：自定义排序
来源：http://mobile.fanxiaobao.xyz/Article/details/giyunfofv.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fanxiaobao.xyz/Article/details/gbvvvqeek.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.fanxiaobao.xyz/Article/details/gicgkznkt.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.fanxiaobao.xyz/Article/details/gfeciltgp.sHtML

[U61] PHP：正则
来源：http://baike.fanxiaobao.xyz/Article/details/gijonqoiw.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.fanxiaobao.xyz/Article/details/geydejles.sHtML

[U62] PHP：日期对象
来源：http://blog.fanxiaobao.xyz/Article/details/gsslaixib.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfjprdufb.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqowabsyy.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkjttvznl.sHtML

[U64] PHP：目录遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gdxbimrsc.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.fanxiaobao.xyz/Article/details/gandddouc.sHtML

[U65] PHP：会话
来源：http://mobile.fanxiaobao.xyz/Article/details/gtzhjpqte.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyymtwjhb.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtusgxqce.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.fanxiaobao.xyz/Article/details/ggycnlkxv.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.fanxiaobao.xyz/Article/details/gykeitckp.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.fanxiaobao.xyz/Article/details/gknyexrat.sHtML

[U68] PHP：PDO 连接
来源：http://3g.fanxiaobao.xyz/Article/details/gbwatzxgb.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.fanxiaobao.xyz/Article/details/gyvacwugw.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjlnvgqno.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/giqftxbcw.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkfsstksb.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggwonxiwx.sHtML

[U71] PHP：抛出异常
来源：http://mobile.fanxiaobao.xyz/Article/details/gvwjttntc.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjtzbsumr.sHtML

[U72] PHP：写错误日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gkfyccfep.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.fanxiaobao.xyz/Article/details/gqkuixonj.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.fanxiaobao.xyz/Article/details/gbbastxhc.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.fanxiaobao.xyz/Article/details/gciikpnxk.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/giudetfhb.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.fanxiaobao.xyz/Article/details/gbcxoabal.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/garpqgrgu.sHtML

composer require psr/container
来源：http://wap.fanxiaobao.xyz/Article/details/gczglcyyn.sHtML

[U76] PHP：简单路由
来源：http://baike.fanxiaobao.xyz/Article/details/gclhsqafs.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.fanxiaobao.xyz/Article/details/gggopdidd.sHtML

[U77] PHP：模板渲染
来源：http://m.share.fanxiaobao.xyz/Article/details/gliyomeja.sHtML

composer require twig/twig
来源：http://m.share.fanxiaobao.xyz/Article/details/gkxcshoqv.sHtML

[U78] PHP：单元测试
来源：http://wap.fanxiaobao.xyz/Article/details/gufdlimuk.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.fanxiaobao.xyz/Article/details/gdzjrkhet.sHtML

[U79] PHP：静态分析
来源：http://mobile.fanxiaobao.xyz/Article/details/gojzmrwix.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.fanxiaobao.xyz/Article/details/gvvvzxazr.sHtML

[U80] PHP：代码规范修复
来源：http://wap.fanxiaobao.xyz/Article/details/gwievyhkg.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.fanxiaobao.xyz/Article/details/gmaspfjit.sHtML

[U81] JS：初始化项目
来源：http://baike.fanxiaobao.xyz/Article/details/ghjjuddci.sHtML

npm init -y;  npm i express
来源：http://read.share.fanxiaobao.xyz/Article/details/gyibydwiq.sHtML

[U82] JS：package.json 脚本
来源：http://blog.fanxiaobao.xyz/Article/details/gyclgqwpt.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.fanxiaobao.xyz/Article/details/glasujcqc.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.fanxiaobao.xyz/Article/details/gnpmvcauj.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.fanxiaobao.xyz/Article/details/gmocogmym.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxzzgigid.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gorgicvuk.sHtML

[U85] JS：可选链
来源：http://www.blog.fanxiaobao.xyz/Article/details/gndfeepkf.sHtML

a?.b?.c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsggtjbzy.sHtML

[U86] JS：空值合并
来源：http://blog.fanxiaobao.xyz/Article/details/gbjycdveq.sHtML

a ?? b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbayvkygb.sHtML

[U87] JS：解构默认值
来源：http://read.share.fanxiaobao.xyz/Article/details/gcrayxlji.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkaezjicd.sHtML

[U88] JS：对象展开合并
来源：http://blog.fanxiaobao.xyz/Article/details/gykkyussn.sHtML

{ ...a, ...b }
来源：http://wap.fanxiaobao.xyz/Article/details/gersxgbvs.sHtML

[U89] JS：数组去重
来源：http://m.share.fanxiaobao.xyz/Article/details/gdnyttzfp.sHtML

[...new Set(arr)]
来源：http://blog.fanxiaobao.xyz/Article/details/gaknwtosh.sHtML

[U90] JS：数字数组排序
来源：http://baike.fanxiaobao.xyz/Article/details/gtvsfzhhi.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmgcsmulg.sHtML

[U91] JS：对象键值遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gmkvymvut.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.fanxiaobao.xyz/Article/details/gflrkuzjl.sHtML

[U92] JS：深拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gnrqmggir.sHtML

structuredClone(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwebrcxaq.sHtML

[U93] JS：模板字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gcewoizum.sHtML

`共 ${n} 条`
来源：http://read.share.fanxiaobao.xyz/Article/details/ggazuysvl.sHtML

[U94] JS：箭头函数
来源：http://baike.fanxiaobao.xyz/Article/details/glbfdtcie.sHtML

const double = x => x * 2;
来源：http://wap.fanxiaobao.xyz/Article/details/gfoqkmzab.sHtML

[U95] JS：Promise 包装
来源：http://mobile.fanxiaobao.xyz/Article/details/gwxlisxwr.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.fanxiaobao.xyz/Article/details/gkfjmtkqk.sHtML

[U96] JS：async/await 与异常
来源：http://wap.fanxiaobao.xyz/Article/details/gbqszukqa.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdfzizioi.sHtML

[U97] JS：并发请求
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzejjlkcl.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtbikitco.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/guhmxfwdc.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.fanxiaobao.xyz/Article/details/gtkwezzdr.sHtML

[U99] JS：事件监听
来源：http://blog.fanxiaobao.xyz/Article/details/gujllxwhc.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.fanxiaobao.xyz/Article/details/gewxogika.sHtML

[U100] JS：DOM 查询
来源：http://blog.fanxiaobao.xyz/Article/details/geapcatuq.sHtML

document.querySelector(".item")
来源：http://www.share.fanxiaobao.xyz/Article/details/gywhvoumv.sHtML

[U101] JS：classList 操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gfdswuiuh.sHtML

el.classList.toggle("active")
来源：http://www.share.fanxiaobao.xyz/Article/details/gvgemgdfb.sHtML

[U102] JS：本地存储
来源：http://mobile.fanxiaobao.xyz/Article/details/gczwtxoqx.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.fanxiaobao.xyz/Article/details/guziuzjru.sHtML

[U103] JS：定时器
来源：http://www.blog.fanxiaobao.xyz/Article/details/gydvbeoil.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.fanxiaobao.xyz/Article/details/gbchkobcu.sHtML

[U104] JS：防抖
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjcygnkny.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gatozivkg.sHtML

[U105] JS：节流
来源：http://baike.fanxiaobao.xyz/Article/details/gavatfjzd.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.fanxiaobao.xyz/Article/details/gtgraelpn.sHtML

[U106] JS：日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gtphwgqca.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.fanxiaobao.xyz/Article/details/gkwixoene.sHtML

[U107] JS：数字千分位
来源：http://wap.fanxiaobao.xyz/Article/details/gukwpmqiu.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcnyspbvf.sHtML

[U108] JS：随机整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghksduhmc.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.fanxiaobao.xyz/Article/details/gugqyrtgt.sHtML

[U109] JS：数组分组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcljsutag.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtzztnzjl.sHtML

[U110] JS：数组分块
来源：http://wap.fanxiaobao.xyz/Article/details/gcdpypzvl.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.fanxiaobao.xyz/Article/details/gqyzjrhda.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaomxxktm.sHtML

new Map(Object.entries(obj))
来源：http://3g.fanxiaobao.xyz/Article/details/gytohauup.sHtML

[U112] JS：字符串补位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtlzbukun.sHtML

"7".padStart(3, "0")
来源：http://wap.fanxiaobao.xyz/Article/details/gwsvixsvs.sHtML

[U113] JS：正则替换全部
来源：http://blog.fanxiaobao.xyz/Article/details/gecsnhdoq.sHtML

s.replaceAll("a", "b")
来源：http://www.share.fanxiaobao.xyz/Article/details/gubzpreqp.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.fanxiaobao.xyz/Article/details/galezcodx.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fanxiaobao.xyz/Article/details/gbnvrclgh.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdgvxehds.sHtML

crypto.randomUUID()
来源：http://3g.fanxiaobao.xyz/Article/details/gmdsgowwk.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.fanxiaobao.xyz/Article/details/gqahqteyk.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gpzffyvlq.sHtML

[U117] JS：单元测试
来源：http://www.blog.fanxiaobao.xyz/Article/details/gurvtepjb.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.fanxiaobao.xyz/Article/details/gusfgconf.sHtML

[U118] JS：开发服务器
来源：http://mobile.fanxiaobao.xyz/Article/details/gpeqhywgt.sHtML

npm i -D vite;  npx vite
来源：http://blog.fanxiaobao.xyz/Article/details/gssqrkdiu.sHtML

[U119] JS：生产构建
来源：http://3g.fanxiaobao.xyz/Article/details/glbtasvfr.sHtML

npx vite build
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdjtoyvvx.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.fanxiaobao.xyz/Article/details/gkmdnjcxg.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.fanxiaobao.xyz/Article/details/gvggamajg.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gsbgkexnq.sHtML

统计汇总
来源：http://3g.fanxiaobao.xyz/Article/details/gkmqxzbzt.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gtduikrxl.sHtML

按语言统计（条）：
来源：http://3g.fanxiaobao.xyz/Article/details/gfsubumlt.sHtML

Python ......... 252
来源：http://www.share.fanxiaobao.xyz/Article/details/ggwpizgyj.sHtML

PHP ............ 252
来源：http://www.share.fanxiaobao.xyz/Article/details/gmqsaktkp.sHtML

JavaScript ..... 252
来源：http://m.share.fanxiaobao.xyz/Article/details/gxgifvmkq.sHtML

TypeScript ..... 212
来源：http://blog.fanxiaobao.xyz/Article/details/gzqjgjzsi.sHtML

Java ........... 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gloyrtegl.sHtML

Go ............. 212
来源：http://baike.fanxiaobao.xyz/Article/details/gtmpgweng.sHtML

Ruby ........... 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjgrjanof.sHtML

C# ............. 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gqitseimj.sHtML

C .............. 30
来源：http://www.blog.fanxiaobao.xyz/Article/details/giyqagjjy.sHtML

C++ ............ 30
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjyqtjtia.sHtML

SQL ............ 90
来源：http://www.share.fanxiaobao.xyz/Article/details/gxouxttcl.sHtML

Bash ........... 80
来源：http://m.share.fanxiaobao.xyz/Article/details/gdiypokva.sHtML

Kotlin ......... 15
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gldhqkqfx.sHtML

Swift .......... 15
来源：http://3g.fanxiaobao.xyz/Article/details/gjmvkcvkw.sHtML

Lua ............ 10
来源：http://3g.fanxiaobao.xyz/Article/details/gczysibsp.sHtML

Perl ........... 10
来源：http://wap.fanxiaobao.xyz/Article/details/gamlzauso.sHtML

Scala .......... 10
来源：http://wap.fanxiaobao.xyz/Article/details/girrekpaz.sHtML

------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/gfhqjrrgs.sHtML

合计 ........... 2106 条
来源：http://blog.fanxiaobao.xyz/Article/details/gobgfgqew.sHtML

按章节统计：
来源：http://wap.fanxiaobao.xyz/Article/details/girrgwizy.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghqwpxuub.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.fanxiaobao.xyz/Article/details/gpvlqgyqg.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsylamqqh.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.fanxiaobao.xyz/Article/details/glctgdedh.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.fanxiaobao.xyz/Article/details/gsceqgctg.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.fanxiaobao.xyz/Article/details/gyxlkissz.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.fanxiaobao.xyz/Article/details/gvvparzkf.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.fanxiaobao.xyz/Article/details/gzzljayfn.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/giqrkidcm.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.fanxiaobao.xyz/Article/details/gimoqceey.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gaqblhjcv.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gjuyvsusv.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/gqpvgstby.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.fanxiaobao.xyz/Article/details/gzdczaewh.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghmbuzpsb.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtfigazym.sHtML

Q SQL 专题                              90
来源：http://blog.fanxiaobao.xyz/Article/details/gsdvrgsbu.sHtML

R Bash 专题                             80
来源：http://read.share.fanxiaobao.xyz/Article/details/ggxcnpypm.sHtML

S C / C++ 专题                          60
来源：http://www.blog.fanxiaobao.xyz/Article/details/gphowwpun.sHtML

T 其他语言补充                          60
来源：http://mobile.fanxiaobao.xyz/Article/details/gcmoxyfyf.sHtML


<!-- 参考信息 -->