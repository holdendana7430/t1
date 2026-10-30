代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gpcaalplq.sHtML

[T55] Scala：集合过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gspcrwwnu.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.fanxiaobao.xyz/Article/details/geqaaugsk.sHtML

[T56] Scala：样例类
来源：http://mobile.fanxiaobao.xyz/Article/details/gkiedsoyx.sHtML

case class User(name: String, age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/gweibxrgh.sHtML

[T57] Scala：模式匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gzywlwraj.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.fanxiaobao.xyz/Article/details/gewilyixp.sHtML

[T58] Scala：函数定义
来源：http://3g.fanxiaobao.xyz/Article/details/gtlsqqmcd.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fanxiaobao.xyz/Article/details/gmmsanwlg.sHtML

[T59] Scala：循环
来源：http://baike.fanxiaobao.xyz/Article/details/ggiyukldm.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.fanxiaobao.xyz/Article/details/ggpkwktxi.sHtML

[T60] Scala：折叠
来源：http://wap.fanxiaobao.xyz/Article/details/gpdctpedq.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fanxiaobao.xyz/Article/details/gngjhvotg.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gzhhrsvst.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gkgxquobr.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gbuzfwbgx.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.fanxiaobao.xyz/Article/details/goqheelpl.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.fanxiaobao.xyz/Article/details/gyatnfsqs.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.fanxiaobao.xyz/Article/details/grcfkhcwo.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwvgoiznb.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.fanxiaobao.xyz/Article/details/gdkpbjdxu.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.fanxiaobao.xyz/Article/details/glscjmlqo.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmgvrguxg.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.fanxiaobao.xyz/Article/details/gndblkbkj.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.fanxiaobao.xyz/Article/details/gpihwwjvx.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.fanxiaobao.xyz/Article/details/gcviihmgy.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gokwegciq.sHtML

{**a, **b}
来源：http://mobile.fanxiaobao.xyz/Article/details/gmsjbrdew.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxalxiwts.sHtML

{v: k for k, v in d.items()}
来源：http://blog.fanxiaobao.xyz/Article/details/gqaredssh.sHtML

[U08] Py：展平二维列表
来源：http://3g.fanxiaobao.xyz/Article/details/gnebfryic.sHtML

[y for x in nested for y in x]
来源：http://m.share.fanxiaobao.xyz/Article/details/gimxhdtwb.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.fanxiaobao.xyz/Article/details/gnsqgjevw.sHtML

max(d, key=d.get)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwbyorowi.sHtML

[U10] Py：按值排序字典
来源：http://3g.fanxiaobao.xyz/Article/details/gxpcttpif.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.fanxiaobao.xyz/Article/details/gojzbnwze.sHtML

[U11] Py：生成器表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gnlwxdmct.sHtML

(x * 2 for x in arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbwcqbwmi.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gyfsnidhb.sHtML

Counter(arr).most_common(3)
来源：http://m.share.fanxiaobao.xyz/Article/details/gaanjfbju.sHtML

[U13] Py：固定长度队列
来源：http://baike.fanxiaobao.xyz/Article/details/ghmprelje.sHtML

deque(maxlen=10)
来源：http://3g.fanxiaobao.xyz/Article/details/guhbrzgby.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.fanxiaobao.xyz/Article/details/gvgbsnxrn.sHtML

defaultdict(list)
来源：http://blog.fanxiaobao.xyz/Article/details/giichpfvm.sHtML

[U15] Py：高精度计时
来源：http://baike.fanxiaobao.xyz/Article/details/ggkmkvtyg.sHtML

t = time.perf_counter()
来源：http://read.share.fanxiaobao.xyz/Article/details/gncalgmhy.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwghphpkk.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.fanxiaobao.xyz/Article/details/gpiknyhap.sHtML

[U17] Py：初始化日志
来源：http://baike.fanxiaobao.xyz/Article/details/gywigqcvb.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.fanxiaobao.xyz/Article/details/grwewesta.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnwfvgsxd.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfbmhhwnm.sHtML

[U19] Py：正则替换带回调
来源：http://blog.fanxiaobao.xyz/Article/details/gqmbaiojw.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.fanxiaobao.xyz/Article/details/goovffjtl.sHtML

[U20] Py：缓存函数结果
来源：http://baike.fanxiaobao.xyz/Article/details/gaagjvjmu.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwrjwvwbb.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.fanxiaobao.xyz/Article/details/gloqbymbl.sHtML

@contextlib.contextmanager
来源：http://www.share.fanxiaobao.xyz/Article/details/ggxktimjo.sHtML

[U22] Py：矩阵转置
来源：http://m.share.fanxiaobao.xyz/Article/details/gurnyritk.sHtML

list(zip(*m))
来源：http://read.share.fanxiaobao.xyz/Article/details/gqncguqpl.sHtML

[U23] Py：分块读取大文件
来源：http://wap.fanxiaobao.xyz/Article/details/gbzqyduza.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.fanxiaobao.xyz/Article/details/ggmhiiqzc.sHtML

[U24] Py：路径操作
来源：http://wap.fanxiaobao.xyz/Article/details/gvypajkqf.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxkxuyejp.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.fanxiaobao.xyz/Article/details/gegjderae.sHtML

csv.DictReader(f)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gacmtkanj.sHtML

[U26] Py：并发下载
来源：http://read.share.fanxiaobao.xyz/Article/details/gxxivzfhk.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjcvifmua.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.fanxiaobao.xyz/Article/details/gevwxmkuv.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.fanxiaobao.xyz/Article/details/gundtzrdd.sHtML

[U28] Py：类型别名
来源：http://baike.fanxiaobao.xyz/Article/details/gfpfcnetk.sHtML

UserId = int
来源：http://baike.fanxiaobao.xyz/Article/details/gjzdhfqql.sHtML

[U29] Py：属性校验
来源：http://baike.fanxiaobao.xyz/Article/details/ghfkdpwym.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggxzkhvst.sHtML

[U30] Py：数据类
来源：http://baike.fanxiaobao.xyz/Article/details/gvzyglyfk.sHtML

@dataclass(slots=True)
来源：http://wap.fanxiaobao.xyz/Article/details/grxymmjyn.sHtML

[U31] Py：单测
来源：http://3g.fanxiaobao.xyz/Article/details/gavukvsyi.sHtML

python -m pytest -q
来源：http://blog.fanxiaobao.xyz/Article/details/gucfsfloa.sHtML

[U32] Py：代码格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gswcwxqiy.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.fanxiaobao.xyz/Article/details/gzbojvvmk.sHtML

[U33] Py：打包发布
来源：http://read.share.fanxiaobao.xyz/Article/details/giwjrrnua.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqdeiubo.sHtML

[U34] Py：判断编码
来源：http://m.share.fanxiaobao.xyz/Article/details/gepvjxiyr.sHtML

chardet.detect(raw)
来源：http://read.share.fanxiaobao.xyz/Article/details/guprrhtms.sHtML

[U35] Py：发送邮件
来源：http://baike.fanxiaobao.xyz/Article/details/gdliudawk.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.fanxiaobao.xyz/Article/details/gbixlkwrf.sHtML

[U36] Py：定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/gzfdckjtl.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.fanxiaobao.xyz/Article/details/gvthyyaxg.sHtML

[U37] Py：读写 Excel
来源：http://wap.fanxiaobao.xyz/Article/details/ghxozamgk.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.fanxiaobao.xyz/Article/details/gzphmetjh.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.fanxiaobao.xyz/Article/details/gsfhfefxz.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghnyvdzwo.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.fanxiaobao.xyz/Article/details/gwaelzeje.sHtML

sys.stdout.isatty()
来源：http://blog.fanxiaobao.xyz/Article/details/gwefgxypb.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqnwodkjd.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvebqhmmf.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.fanxiaobao.xyz/Article/details/gykvuxvfk.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.fanxiaobao.xyz/Article/details/gfeezlxkp.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.fanxiaobao.xyz/Article/details/gosaozlvf.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfffwkczt.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjelmryfr.sHtML

namespace App\Http;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gljzawqdu.sHtML

[U44] PHP：开启严格类型
来源：http://blog.fanxiaobao.xyz/Article/details/gymbckrjh.sHtML

declare(strict_types=1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/guydlwgzg.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.fanxiaobao.xyz/Article/details/gznehvahq.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gsenpqdrp.sHtML

[U46] PHP：可空类型
来源：http://read.share.fanxiaobao.xyz/Article/details/grrmgsoac.sHtML

?string $name = null
来源：http://blog.fanxiaobao.xyz/Article/details/grqykbghi.sHtML

[U47] PHP：联合类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gtbifbznf.sHtML

int|string $id
来源：http://wap.fanxiaobao.xyz/Article/details/gmdqfilsz.sHtML

[U48] PHP：纯枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/glqqminrf.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gevlvhjph.sHtML

[U49] PHP：只读属性
来源：http://m.share.fanxiaobao.xyz/Article/details/gerwhglsz.sHtML

public readonly string $name
来源：http://blog.fanxiaobao.xyz/Article/details/gnwyqucms.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.fanxiaobao.xyz/Article/details/gyupjrhnk.sHtML

public function __construct(private int $id) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gbwcutevz.sHtML

[U51] PHP：数组解构
来源：http://blog.fanxiaobao.xyz/Article/details/gplzovocv.sHtML

[$a, $b] = $arr;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzarhuqwo.sHtML

[U52] PHP：箭头函数
来源：http://baike.fanxiaobao.xyz/Article/details/gxfewgojn.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.fanxiaobao.xyz/Article/details/gstdxxkhz.sHtML

[U53] PHP：空合并运算符
来源：http://blog.fanxiaobao.xyz/Article/details/gzfwgsftx.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gswirzoei.sHtML

[U54] PHP：空安全调用
来源：http://3g.fanxiaobao.xyz/Article/details/gxxgooqhv.sHtML

$obj?->method()
来源：http://3g.fanxiaobao.xyz/Article/details/gmhqyvmjd.sHtML

[U55] PHP：match 表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gctzjyrwm.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghdnotgzg.sHtML

[U56] PHP：命名参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gnxqtrsyt.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjacmxeid.sHtML

[U57] PHP：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/ghnliceeu.sHtML

"值: {$a}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gysscvece.sHtML

[U58] PHP：数组三件套
来源：http://3g.fanxiaobao.xyz/Article/details/gyrelfllv.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.fanxiaobao.xyz/Article/details/giflobnya.sHtML

[U59] PHP：自定义排序
来源：http://wap.fanxiaobao.xyz/Article/details/gerpplwez.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fanxiaobao.xyz/Article/details/ghviudbjn.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.fanxiaobao.xyz/Article/details/gnymprfgb.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giwtxytyr.sHtML

[U61] PHP：正则
来源：http://wap.fanxiaobao.xyz/Article/details/gxrleybru.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxakvazur.sHtML

[U62] PHP：日期对象
来源：http://wap.fanxiaobao.xyz/Article/details/gatkihgei.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.fanxiaobao.xyz/Article/details/gkopwjttc.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guhxwifhl.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.fanxiaobao.xyz/Article/details/gdrtszrlt.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/geyjxiutt.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.fanxiaobao.xyz/Article/details/gzqnfzzbj.sHtML

[U65] PHP：会话
来源：http://baike.fanxiaobao.xyz/Article/details/ghvmgdbxm.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsnozbquz.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghqjykufx.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gztyqusqj.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.fanxiaobao.xyz/Article/details/guqtsxhod.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.fanxiaobao.xyz/Article/details/gkcxkwlis.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gpvuhgfjf.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.fanxiaobao.xyz/Article/details/gecqabtmu.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gvicgtdrj.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.fanxiaobao.xyz/Article/details/gngwgviyl.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gizraytqr.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.fanxiaobao.xyz/Article/details/gcbdserzk.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaufrgkhu.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.fanxiaobao.xyz/Article/details/gpcwwitwf.sHtML

[U72] PHP：写错误日志
来源：http://baike.fanxiaobao.xyz/Article/details/gytgdrmts.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbrqoksoi.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.fanxiaobao.xyz/Article/details/ghwsasvky.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.fanxiaobao.xyz/Article/details/gcqwuajki.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/guxnfeugt.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.fanxiaobao.xyz/Article/details/gsokjgccx.sHtML

[U75] PHP：依赖注入
来源：http://baike.fanxiaobao.xyz/Article/details/gqrgrheiw.sHtML

composer require psr/container
来源：http://wap.fanxiaobao.xyz/Article/details/gjefnocpx.sHtML

[U76] PHP：简单路由
来源：http://3g.fanxiaobao.xyz/Article/details/gwvxfpkhg.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.fanxiaobao.xyz/Article/details/gfcvliedg.sHtML

[U77] PHP：模板渲染
来源：http://m.share.fanxiaobao.xyz/Article/details/gmzdbitwl.sHtML

composer require twig/twig
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpshpihty.sHtML

[U78] PHP：单元测试
来源：http://m.share.fanxiaobao.xyz/Article/details/gktegvtez.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.fanxiaobao.xyz/Article/details/gkotuoqku.sHtML

[U79] PHP：静态分析
来源：http://m.share.fanxiaobao.xyz/Article/details/gnbmwziwc.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.fanxiaobao.xyz/Article/details/gfdrzowyj.sHtML

[U80] PHP：代码规范修复
来源：http://blog.fanxiaobao.xyz/Article/details/gdwkhtakz.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.fanxiaobao.xyz/Article/details/gzrfilrdt.sHtML

[U81] JS：初始化项目
来源：http://blog.fanxiaobao.xyz/Article/details/gusljydjg.sHtML

npm init -y;  npm i express
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gapkyzldf.sHtML

[U82] JS：package.json 脚本
来源：http://wap.fanxiaobao.xyz/Article/details/grhsmmmlo.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmaqbutwt.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.fanxiaobao.xyz/Article/details/gkjnwlhut.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.fanxiaobao.xyz/Article/details/gkgmgiobf.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmbbkhhxi.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.fanxiaobao.xyz/Article/details/gszezbsug.sHtML

[U85] JS：可选链
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfjhpdysi.sHtML

a?.b?.c
来源：http://wap.fanxiaobao.xyz/Article/details/gabbruckv.sHtML

[U86] JS：空值合并
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyonztfdx.sHtML

a ?? b
来源：http://blog.fanxiaobao.xyz/Article/details/gnvmbdqcq.sHtML

[U87] JS：解构默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/goncxwhdd.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.fanxiaobao.xyz/Article/details/ggoyblbec.sHtML

[U88] JS：对象展开合并
来源：http://mobile.fanxiaobao.xyz/Article/details/gqlmkumlr.sHtML

{ ...a, ...b }
来源：http://wap.fanxiaobao.xyz/Article/details/gbbhgizmy.sHtML

[U89] JS：数组去重
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glgxkiide.sHtML

[...new Set(arr)]
来源：http://wap.fanxiaobao.xyz/Article/details/giuhjblcq.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gklldmbup.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gemdyecgq.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gybdxplyn.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.fanxiaobao.xyz/Article/details/gpioypxrc.sHtML

[U92] JS：深拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gqizycvyk.sHtML

structuredClone(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfwjabcef.sHtML

[U93] JS：模板字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gakveempg.sHtML

`共 ${n} 条`
来源：http://m.share.fanxiaobao.xyz/Article/details/gjablwjjv.sHtML

[U94] JS：箭头函数
来源：http://wap.fanxiaobao.xyz/Article/details/gzufcmmnu.sHtML

const double = x => x * 2;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbdgmemqb.sHtML

[U95] JS：Promise 包装
来源：http://3g.fanxiaobao.xyz/Article/details/gotebzigp.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.fanxiaobao.xyz/Article/details/gwulfaqgf.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.fanxiaobao.xyz/Article/details/gqxdkhnee.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.fanxiaobao.xyz/Article/details/gpkygvgbl.sHtML

[U97] JS：并发请求
来源：http://baike.fanxiaobao.xyz/Article/details/guhynlhww.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fanxiaobao.xyz/Article/details/gjabppbnl.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.fanxiaobao.xyz/Article/details/gyjaxzcqe.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.fanxiaobao.xyz/Article/details/gbrgavate.sHtML

[U99] JS：事件监听
来源：http://baike.fanxiaobao.xyz/Article/details/gqvsqfuzb.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.fanxiaobao.xyz/Article/details/gbdieyvde.sHtML

[U100] JS：DOM 查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gvlogopns.sHtML

document.querySelector(".item")
来源：http://baike.fanxiaobao.xyz/Article/details/gpsfhdiou.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghbgdonlz.sHtML

el.classList.toggle("active")
来源：http://blog.fanxiaobao.xyz/Article/details/gvuwtlsty.sHtML

[U102] JS：本地存储
来源：http://www.share.fanxiaobao.xyz/Article/details/gratvyeus.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.fanxiaobao.xyz/Article/details/gfmyrvtwc.sHtML

[U103] JS：定时器
来源：http://mobile.fanxiaobao.xyz/Article/details/gseqwwphz.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.fanxiaobao.xyz/Article/details/garlcluaq.sHtML

[U104] JS：防抖
来源：http://www.share.fanxiaobao.xyz/Article/details/gktbkssqp.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fanxiaobao.xyz/Article/details/gmexwoadx.sHtML

[U105] JS：节流
来源：http://read.share.fanxiaobao.xyz/Article/details/gokcdwvtb.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gndxgquzi.sHtML

[U106] JS：日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gowbsrpze.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.fanxiaobao.xyz/Article/details/gfbzwdeah.sHtML

[U107] JS：数字千分位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvjgvlqai.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.fanxiaobao.xyz/Article/details/gmeiuoqyk.sHtML

[U108] JS：随机整数
来源：http://blog.fanxiaobao.xyz/Article/details/gapvhaikj.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.fanxiaobao.xyz/Article/details/glqvojivm.sHtML

[U109] JS：数组分组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyaiduzuo.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.fanxiaobao.xyz/Article/details/gqxnmzqlk.sHtML

[U110] JS：数组分块
来源：http://www.blog.fanxiaobao.xyz/Article/details/glxcrfjdx.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.fanxiaobao.xyz/Article/details/gklccsbvx.sHtML

[U111] JS：对象转 Map
来源：http://wap.fanxiaobao.xyz/Article/details/gtbtdlnmt.sHtML

new Map(Object.entries(obj))
来源：http://read.share.fanxiaobao.xyz/Article/details/gvfdcwymf.sHtML

[U112] JS：字符串补位
来源：http://www.share.fanxiaobao.xyz/Article/details/gjpefnyvv.sHtML

"7".padStart(3, "0")
来源：http://www.share.fanxiaobao.xyz/Article/details/gvoawhrni.sHtML

[U113] JS：正则替换全部
来源：http://wap.fanxiaobao.xyz/Article/details/gsbhzwlee.sHtML

s.replaceAll("a", "b")
来源：http://www.share.fanxiaobao.xyz/Article/details/gysurggmm.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gsxtjtnhi.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghxfxjquf.sHtML

[U115] JS：生成 UUID
来源：http://3g.fanxiaobao.xyz/Article/details/gzelminis.sHtML

crypto.randomUUID()
来源：http://3g.fanxiaobao.xyz/Article/details/gelhfygje.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.fanxiaobao.xyz/Article/details/ghbvucdub.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjcehatgq.sHtML

[U117] JS：单元测试
来源：http://www.blog.fanxiaobao.xyz/Article/details/gugdlnjya.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.fanxiaobao.xyz/Article/details/gjmpacqgk.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxdpvurpp.sHtML

npm i -D vite;  npx vite
来源：http://blog.fanxiaobao.xyz/Article/details/gqimgqtvp.sHtML

[U119] JS：生产构建
来源：http://www.share.fanxiaobao.xyz/Article/details/gpqgluhoq.sHtML

npx vite build
来源：http://mobile.fanxiaobao.xyz/Article/details/gasynxzwt.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.fanxiaobao.xyz/Article/details/gvwaoywdg.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.fanxiaobao.xyz/Article/details/grscfmdrs.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gqxpiztsb.sHtML

统计汇总
来源：http://mobile.fanxiaobao.xyz/Article/details/gvxelyjmi.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gkinorxwo.sHtML

按语言统计（条）：
来源：http://read.share.fanxiaobao.xyz/Article/details/guwuqylha.sHtML

Python ......... 252
来源：http://m.share.fanxiaobao.xyz/Article/details/gubzohtjh.sHtML

PHP ............ 252
来源：http://read.share.fanxiaobao.xyz/Article/details/gamukskbj.sHtML

JavaScript ..... 252
来源：http://baike.fanxiaobao.xyz/Article/details/gshmuthow.sHtML

TypeScript ..... 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gseluqlqb.sHtML

Java ........... 212
来源：http://baike.fanxiaobao.xyz/Article/details/gxqluuybu.sHtML

Go ............. 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gsahdqxml.sHtML

Ruby ........... 212
来源：http://mobile.fanxiaobao.xyz/Article/details/ghaqwchty.sHtML

C# ............. 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gszhhorss.sHtML

C .............. 30
来源：http://3g.fanxiaobao.xyz/Article/details/glsfbkmwh.sHtML

C++ ............ 30
来源：http://m.share.fanxiaobao.xyz/Article/details/gyfnfzhfh.sHtML

SQL ............ 90
来源：http://www.blog.fanxiaobao.xyz/Article/details/gprqibixv.sHtML

Bash ........... 80
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwpbrvxia.sHtML

Kotlin ......... 15
来源：http://mobile.fanxiaobao.xyz/Article/details/gtmmzyszj.sHtML

Swift .......... 15
来源：http://read.share.fanxiaobao.xyz/Article/details/gdrjjxicn.sHtML

Lua ............ 10
来源：http://blog.fanxiaobao.xyz/Article/details/gmcwfibpp.sHtML

Perl ........... 10
来源：http://3g.fanxiaobao.xyz/Article/details/guydpedmd.sHtML

Scala .......... 10
来源：http://mobile.fanxiaobao.xyz/Article/details/gffrymovx.sHtML

------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjdesqhyh.sHtML

合计 ........... 2106 条
来源：http://wap.fanxiaobao.xyz/Article/details/glxqwykkd.sHtML

按章节统计：
来源：http://mobile.fanxiaobao.xyz/Article/details/gepmuoenh.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.fanxiaobao.xyz/Article/details/gexexyvcy.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.fanxiaobao.xyz/Article/details/gdlbbxgqe.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.fanxiaobao.xyz/Article/details/gvagudfyr.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.fanxiaobao.xyz/Article/details/gpfmhitwm.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.fanxiaobao.xyz/Article/details/geulqtrqc.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.fanxiaobao.xyz/Article/details/gsfuzjywk.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.fanxiaobao.xyz/Article/details/gyerocyos.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.fanxiaobao.xyz/Article/details/gnvmwbzvk.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/gleraqhrk.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.fanxiaobao.xyz/Article/details/gpdalaxga.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/gszgfqtwl.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/gibvhebmw.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/gatztfzfw.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.fanxiaobao.xyz/Article/details/gomeubirb.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.fanxiaobao.xyz/Article/details/gczrdigiw.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gtvwlchvg.sHtML

Q SQL 专题                              90
来源：http://blog.fanxiaobao.xyz/Article/details/gwervubyp.sHtML

R Bash 专题                             80
来源：http://mobile.fanxiaobao.xyz/Article/details/gkrqixzva.sHtML

S C / C++ 专题                          60
来源：http://3g.fanxiaobao.xyz/Article/details/gcdncoaxh.sHtML

T 其他语言补充                          60
来源：http://www.blog.fanxiaobao.xyz/Article/details/govclotqi.sHtML


<!-- 参考信息 -->