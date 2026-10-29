代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.hesvh.cn/Article/details/gjsaumsin.sHtML

[T59] Scala：循环
来源：http://wap.hesvh.cn/Article/details/gixdtvmmy.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.fehbvm.com/Article/details/gignptedb.sHtML

[T60] Scala：折叠
来源：http://mobile.hesvh.cn/Article/details/gdefplvzt.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.zdbjq.cn/Article/details/gybniyafy.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gcyzpqdyb.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.hesvh.cn/Article/details/gylbaoujp.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gwzamgtjq.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.fehbvm.com/Article/details/grkbtipot.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.hesvh.cn/Article/details/gbcuexypu.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.hesvh.cn/Article/details/gxbnhhnye.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.zdbjq.cn/Article/details/gjrnqhwds.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.zdbjq.cn/Article/details/ghtdqgvsj.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.fehbvm.com/Article/details/gpxshfpzh.sHtML

[U04] Py：变量调试打印
来源：http://3g.zdbjq.cn/Article/details/glznuverf.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.zdbjq.cn/Article/details/geakzowab.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.hesvh.cn/Article/details/gufsenssd.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.fehbvm.com/Article/details/gmxhuzsre.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.zdbjq.cn/Article/details/gymvyoffw.sHtML

{**a, **b}
来源：http://blog.hesvh.cn/Article/details/georvnrzi.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.fehbvm.com/Article/details/gwikpmpdw.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.hesvh.cn/Article/details/giarhxmie.sHtML

[U08] Py：展平二维列表
来源：http://mobile.hesvh.cn/Article/details/gbpyjrfok.sHtML

[y for x in nested for y in x]
来源：http://baike.zdbjq.cn/Article/details/gfjswxicj.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.zdbjq.cn/Article/details/gryqpvezy.sHtML

max(d, key=d.get)
来源：http://3g.fehbvm.com/Article/details/gavrpakrc.sHtML

[U10] Py：按值排序字典
来源：http://wap.fehbvm.com/Article/details/gwxxsycpn.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.fehbvm.com/Article/details/gaxmhuqml.sHtML

[U11] Py：生成器表达式
来源：http://www.share.zdbjq.cn/Article/details/glibhnhyn.sHtML

(x * 2 for x in arr)
来源：http://www.blog.hesvh.cn/Article/details/gcsmopkrf.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.fehbvm.com/Article/details/gtkkzvdve.sHtML

Counter(arr).most_common(3)
来源：http://m.share.zdbjq.cn/Article/details/gutsotytg.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.zdbjq.cn/Article/details/giaqglpab.sHtML

deque(maxlen=10)
来源：http://www.share.fehbvm.com/Article/details/gojcikihz.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.fehbvm.com/Article/details/gfeurgwvb.sHtML

defaultdict(list)
来源：http://read.share.hesvh.cn/Article/details/gkvzeyhgp.sHtML

[U15] Py：高精度计时
来源：http://mobile.zdbjq.cn/Article/details/ggkpltuah.sHtML

t = time.perf_counter()
来源：http://www.blog.fehbvm.com/Article/details/giaddemcn.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.hesvh.cn/Article/details/grtjcypoc.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.fehbvm.com/Article/details/givdvpnbq.sHtML

[U17] Py：初始化日志
来源：http://mobile.hesvh.cn/Article/details/gupizdzfg.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fehbvm.com/Article/details/gpuhtjmih.sHtML

[U18] Py：预编译正则
来源：http://3g.zdbjq.cn/Article/details/gwezohkap.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.fehbvm.com/Article/details/gvieqkpns.sHtML

[U19] Py：正则替换带回调
来源：http://3g.zdbjq.cn/Article/details/gztyebwjj.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.zdbjq.cn/Article/details/gsobdoyng.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.hesvh.cn/Article/details/ghaostokt.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.fehbvm.com/Article/details/gvuvtvfhp.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.zdbjq.cn/Article/details/guqrlgvyq.sHtML

@contextlib.contextmanager
来源：http://m.share.hesvh.cn/Article/details/godrjouke.sHtML

[U22] Py：矩阵转置
来源：http://baike.hesvh.cn/Article/details/gfvynddhh.sHtML

list(zip(*m))
来源：http://read.share.hesvh.cn/Article/details/gzwdkvsec.sHtML

[U23] Py：分块读取大文件
来源：http://blog.fehbvm.com/Article/details/gspugynzd.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.fehbvm.com/Article/details/gvkmetvob.sHtML

[U24] Py：路径操作
来源：http://www.m.share.hesvh.cn/Article/details/giexflvoa.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/gaeggtbrb.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.zdbjq.cn/Article/details/gjvjgotqr.sHtML

csv.DictReader(f)
来源：http://baike.zdbjq.cn/Article/details/gdpapskyi.sHtML

[U26] Py：并发下载
来源：http://mobile.zdbjq.cn/Article/details/gutmovtvd.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.zdbjq.cn/Article/details/gqveneyzg.sHtML

[U27] Py：异步 HTTP
来源：http://blog.fehbvm.com/Article/details/gwffwpame.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.fehbvm.com/Article/details/glaemjovh.sHtML

[U28] Py：类型别名
来源：http://blog.fehbvm.com/Article/details/ggopkxehg.sHtML

UserId = int
来源：http://blog.hesvh.cn/Article/details/gohxepamd.sHtML

[U29] Py：属性校验
来源：http://read.share.hesvh.cn/Article/details/gwdbxohuh.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.hesvh.cn/Article/details/gntuvbjtg.sHtML

[U30] Py：数据类
来源：http://blog.hesvh.cn/Article/details/gfuuhmzzy.sHtML

@dataclass(slots=True)
来源：http://read.share.hesvh.cn/Article/details/gszkqgnrc.sHtML

[U31] Py：单测
来源：http://mobile.hesvh.cn/Article/details/gfbkwzsup.sHtML

python -m pytest -q
来源：http://www.share.hesvh.cn/Article/details/gmbivsuhs.sHtML

[U32] Py：代码格式化
来源：http://blog.fehbvm.com/Article/details/gnaiizkct.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.fehbvm.com/Article/details/gqchgnthr.sHtML

[U33] Py：打包发布
来源：http://baike.zdbjq.cn/Article/details/ghxbihnds.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.fehbvm.com/Article/details/gogodygyi.sHtML

[U34] Py：判断编码
来源：http://www.share.zdbjq.cn/Article/details/gjzkfxcjn.sHtML

chardet.detect(raw)
来源：http://m.share.zdbjq.cn/Article/details/gfclaxfjv.sHtML

[U35] Py：发送邮件
来源：http://mobile.fehbvm.com/Article/details/ghckkjmfi.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.zdbjq.cn/Article/details/gmmzthnid.sHtML

[U36] Py：定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/gcfigjruz.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.fehbvm.com/Article/details/gipjevqwn.sHtML

[U37] Py：读写 Excel
来源：http://3g.hesvh.cn/Article/details/gfuhwtjep.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.hesvh.cn/Article/details/gaayxhzre.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.zdbjq.cn/Article/details/gpuyvzvdb.sHtML

Path(__file__).resolve().parent
来源：http://www.share.hesvh.cn/Article/details/gqtldydyj.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.zdbjq.cn/Article/details/gbqklwwli.sHtML

sys.stdout.isatty()
来源：http://www.blog.fehbvm.com/Article/details/glvvdbdyv.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.fehbvm.com/Article/details/gwtolqxhj.sHtML

print("err", file=sys.stderr)
来源：http://mobile.hesvh.cn/Article/details/gmlomvbfq.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.fehbvm.com/Article/details/gjdywvcxh.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.zdbjq.cn/Article/details/gclaxqfdx.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.hesvh.cn/Article/details/ggrqbeqrx.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.fehbvm.com/Article/details/gwhhfsamz.sHtML

[U43] PHP：声明命名空间
来源：http://baike.hesvh.cn/Article/details/goslynuxn.sHtML

namespace App\Http;
来源：http://read.share.fehbvm.com/Article/details/greebkkrj.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.fehbvm.com/Article/details/gvzscrwsi.sHtML

declare(strict_types=1);
来源：http://www.share.fehbvm.com/Article/details/gmmjdxwrt.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.hesvh.cn/Article/details/gcpspqbkp.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gvsstjqnp.sHtML

[U46] PHP：可空类型
来源：http://m.share.zdbjq.cn/Article/details/gcvlxcqcu.sHtML

?string $name = null
来源：http://3g.zdbjq.cn/Article/details/gwcmnkdnk.sHtML

[U47] PHP：联合类型
来源：http://m.share.hesvh.cn/Article/details/gnlpwodnl.sHtML

int|string $id
来源：http://read.share.hesvh.cn/Article/details/gkelavgzf.sHtML

[U48] PHP：纯枚举
来源：http://read.share.hesvh.cn/Article/details/gecnnrrgz.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.fehbvm.com/Article/details/gmfteeuue.sHtML

[U49] PHP：只读属性
来源：http://wap.fehbvm.com/Article/details/glzibnnkf.sHtML

public readonly string $name
来源：http://m.share.hesvh.cn/Article/details/gwxzzpbnu.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.zdbjq.cn/Article/details/gigawywpc.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.hesvh.cn/Article/details/gjvsgibza.sHtML

[U51] PHP：数组解构
来源：http://read.share.fehbvm.com/Article/details/ghsrowzho.sHtML

[$a, $b] = $arr;
来源：http://mobile.fehbvm.com/Article/details/gbdxlbibs.sHtML

[U52] PHP：箭头函数
来源：http://m.share.hesvh.cn/Article/details/genkaerje.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.hesvh.cn/Article/details/gyfmaohuh.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.hesvh.cn/Article/details/glssfcruh.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.hesvh.cn/Article/details/gswatshrs.sHtML

[U54] PHP：空安全调用
来源：http://wap.hesvh.cn/Article/details/goxvrrvok.sHtML

$obj?->method()
来源：http://baike.fehbvm.com/Article/details/gbfgeickh.sHtML

[U55] PHP：match 表达式
来源：http://m.share.hesvh.cn/Article/details/gboccyzbq.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.fehbvm.com/Article/details/graalycqu.sHtML

[U56] PHP：命名参数
来源：http://baike.fehbvm.com/Article/details/gthulxkfu.sHtML

f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/glxrxsfhr.sHtML

[U57] PHP：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gfifatgpe.sHtML

"值: {$a}"
来源：http://www.share.zdbjq.cn/Article/details/gedrvmcjk.sHtML

[U58] PHP：数组三件套
来源：http://www.share.fehbvm.com/Article/details/guurivsvc.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.hesvh.cn/Article/details/gqubvkmci.sHtML

[U59] PHP：自定义排序
来源：http://mobile.zdbjq.cn/Article/details/glgqvvrua.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.hesvh.cn/Article/details/gzjkojtcn.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.hesvh.cn/Article/details/grsxrnuri.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.zdbjq.cn/Article/details/gyxiphhyl.sHtML

[U61] PHP：正则
来源：http://3g.fehbvm.com/Article/details/grodbsvih.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.fehbvm.com/Article/details/grqdqmrfk.sHtML

[U62] PHP：日期对象
来源：http://www.share.hesvh.cn/Article/details/gwnggrweq.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.hesvh.cn/Article/details/grddodtgk.sHtML

[U63] PHP：文件读写
来源：http://baike.fehbvm.com/Article/details/gedzmbabt.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.hesvh.cn/Article/details/gkcvsmruj.sHtML

[U64] PHP：目录遍历
来源：http://baike.fehbvm.com/Article/details/gguedsdyk.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.hesvh.cn/Article/details/gofjowlid.sHtML

[U65] PHP：会话
来源：http://m.share.zdbjq.cn/Article/details/gbjiuahxt.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gkiikuxpo.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.zdbjq.cn/Article/details/gewqhhkkn.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.zdbjq.cn/Article/details/gruplvvsr.sHtML

[U67] PHP：处理文件上传
来源：http://blog.zdbjq.cn/Article/details/glspocxcc.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.fehbvm.com/Article/details/gztzxiftr.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.fehbvm.com/Article/details/grlqpwemm.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.fehbvm.com/Article/details/gdecdobjz.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.fehbvm.com/Article/details/gldcjctzs.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.hesvh.cn/Article/details/gnhcestcr.sHtML

[U70] PHP：PDO 事务
来源：http://3g.zdbjq.cn/Article/details/gmbojxspx.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.zdbjq.cn/Article/details/gwaeqxhjh.sHtML

[U71] PHP：抛出异常
来源：http://m.share.fehbvm.com/Article/details/gmxjvacfg.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.fehbvm.com/Article/details/gmamhkmof.sHtML

[U72] PHP：写错误日志
来源：http://www.share.fehbvm.com/Article/details/gyprvbzhl.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.fehbvm.com/Article/details/gyxmngzjk.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.zdbjq.cn/Article/details/gxtgerfaj.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.zdbjq.cn/Article/details/gbwjfbqoa.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.hesvh.cn/Article/details/givqftsgp.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.fehbvm.com/Article/details/gduwjsdoh.sHtML

[U75] PHP：依赖注入
来源：http://www.share.hesvh.cn/Article/details/gxihlgafv.sHtML

composer require psr/container
来源：http://www.blog.hesvh.cn/Article/details/gbygyibdl.sHtML

[U76] PHP：简单路由
来源：http://read.share.fehbvm.com/Article/details/gevkrzglm.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.hesvh.cn/Article/details/gmgibmpgh.sHtML

[U77] PHP：模板渲染
来源：http://m.share.zdbjq.cn/Article/details/gmeamqwne.sHtML

composer require twig/twig
来源：http://baike.fehbvm.com/Article/details/gawqtaqsb.sHtML

[U78] PHP：单元测试
来源：http://blog.hesvh.cn/Article/details/gxluikhhn.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.hesvh.cn/Article/details/gdjdfyssb.sHtML

[U79] PHP：静态分析
来源：http://read.share.fehbvm.com/Article/details/gfinqnefk.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.hesvh.cn/Article/details/ggdltfaun.sHtML

[U80] PHP：代码规范修复
来源：http://wap.hesvh.cn/Article/details/ghrfjxwud.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.hesvh.cn/Article/details/glejgcqrv.sHtML

[U81] JS：初始化项目
来源：http://www.blog.zdbjq.cn/Article/details/gnicrbnya.sHtML

npm init -y;  npm i express
来源：http://wap.fehbvm.com/Article/details/gtugphmhw.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.fehbvm.com/Article/details/gfkeiowpk.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.zdbjq.cn/Article/details/gzxlxxbmd.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.fehbvm.com/Article/details/gerhwjwec.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.hesvh.cn/Article/details/gjjafzrxl.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.hesvh.cn/Article/details/gutqzsifr.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.zdbjq.cn/Article/details/gknfkqtjc.sHtML

[U85] JS：可选链
来源：http://www.share.zdbjq.cn/Article/details/gwcjiqzmc.sHtML

a?.b?.c
来源：http://www.m.share.fehbvm.com/Article/details/gkqjfzlnn.sHtML

[U86] JS：空值合并
来源：http://blog.hesvh.cn/Article/details/govyjugfu.sHtML

a ?? b
来源：http://baike.hesvh.cn/Article/details/gjpalxvne.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.hesvh.cn/Article/details/gdljsemcq.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.hesvh.cn/Article/details/geafvpdpt.sHtML

[U88] JS：对象展开合并
来源：http://blog.hesvh.cn/Article/details/gxrgvoxvu.sHtML

{ ...a, ...b }
来源：http://www.m.share.fehbvm.com/Article/details/gyyomjwxo.sHtML

[U89] JS：数组去重
来源：http://m.share.fehbvm.com/Article/details/ggysopmpb.sHtML

[...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/gizfpjorm.sHtML

[U90] JS：数字数组排序
来源：http://read.share.fehbvm.com/Article/details/ggitdfxof.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gezmavhbc.sHtML

[U91] JS：对象键值遍历
来源：http://blog.zdbjq.cn/Article/details/gqlaiwkpy.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.fehbvm.com/Article/details/gvrhqccpg.sHtML

[U92] JS：深拷贝
来源：http://blog.zdbjq.cn/Article/details/gzgkgsknz.sHtML

structuredClone(obj)
来源：http://wap.fehbvm.com/Article/details/gigdxkmxx.sHtML

[U93] JS：模板字符串
来源：http://www.share.hesvh.cn/Article/details/ggyymxgrn.sHtML

`共 ${n} 条`
来源：http://blog.hesvh.cn/Article/details/gzcerkacm.sHtML

[U94] JS：箭头函数
来源：http://3g.zdbjq.cn/Article/details/giajuxtzf.sHtML

const double = x => x * 2;
来源：http://3g.hesvh.cn/Article/details/gtbbgzxci.sHtML

[U95] JS：Promise 包装
来源：http://wap.zdbjq.cn/Article/details/gqzksoitk.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.zdbjq.cn/Article/details/gobpiboyr.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.zdbjq.cn/Article/details/gxdmqzoys.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/geugpsxol.sHtML

[U97] JS：并发请求
来源：http://3g.zdbjq.cn/Article/details/gvygccyaf.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/gaccmudvv.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.zdbjq.cn/Article/details/gjtfdgyyv.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.fehbvm.com/Article/details/gbndozvzj.sHtML

[U99] JS：事件监听
来源：http://mobile.zdbjq.cn/Article/details/gnbdsjoyr.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.hesvh.cn/Article/details/gmckwcrdc.sHtML

[U100] JS：DOM 查询
来源：http://www.share.fehbvm.com/Article/details/giwmcbtby.sHtML

document.querySelector(".item")
来源：http://3g.hesvh.cn/Article/details/gjabtdfvm.sHtML

[U101] JS：classList 操作
来源：http://blog.hesvh.cn/Article/details/ghbucmwso.sHtML

el.classList.toggle("active")
来源：http://blog.zdbjq.cn/Article/details/gnnaahzsg.sHtML

[U102] JS：本地存储
来源：http://read.share.fehbvm.com/Article/details/giximlfip.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.zdbjq.cn/Article/details/gpjiweuoo.sHtML

[U103] JS：定时器
来源：http://3g.hesvh.cn/Article/details/gjunqwweb.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.zdbjq.cn/Article/details/grvlybjyx.sHtML

[U104] JS：防抖
来源：http://www.blog.zdbjq.cn/Article/details/gwutyucwb.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/gjunfqtdr.sHtML

[U105] JS：节流
来源：http://www.m.share.fehbvm.com/Article/details/gzwohybmd.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.fehbvm.com/Article/details/gkqkhbdaa.sHtML

[U106] JS：日期格式化
来源：http://3g.zdbjq.cn/Article/details/gioqfdlwl.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.zdbjq.cn/Article/details/gbtgxznpv.sHtML

[U107] JS：数字千分位
来源：http://wap.zdbjq.cn/Article/details/gpykrdbvb.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.fehbvm.com/Article/details/gtxqumvza.sHtML

[U108] JS：随机整数
来源：http://blog.hesvh.cn/Article/details/gljfihtvj.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.hesvh.cn/Article/details/gwcxdqcja.sHtML

[U109] JS：数组分组
来源：http://www.blog.fehbvm.com/Article/details/gficrydef.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.hesvh.cn/Article/details/gzrintpyi.sHtML

[U110] JS：数组分块
来源：http://www.m.share.fehbvm.com/Article/details/glgrbayad.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.hesvh.cn/Article/details/gmluqmanf.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.fehbvm.com/Article/details/gmkbznblp.sHtML

new Map(Object.entries(obj))
来源：http://mobile.zdbjq.cn/Article/details/gtohffizk.sHtML

[U112] JS：字符串补位
来源：http://blog.zdbjq.cn/Article/details/giyjdqzao.sHtML

"7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/ghgktkokb.sHtML

[U113] JS：正则替换全部
来源：http://blog.hesvh.cn/Article/details/glffkwytx.sHtML

s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gysjliyuk.sHtML

[U114] JS：JSON 深比较
来源：http://3g.hesvh.cn/Article/details/gjblksoce.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.zdbjq.cn/Article/details/gqfotjkwl.sHtML

[U115] JS：生成 UUID
来源：http://3g.zdbjq.cn/Article/details/goafltpxs.sHtML

crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/grlltfkhh.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.zdbjq.cn/Article/details/gukfnbcak.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.fehbvm.com/Article/details/ghupdpris.sHtML

[U117] JS：单元测试
来源：http://www.share.zdbjq.cn/Article/details/guesjntga.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.zdbjq.cn/Article/details/gexjizesm.sHtML

[U118] JS：开发服务器
来源：http://mobile.hesvh.cn/Article/details/ghkwqambz.sHtML

npm i -D vite;  npx vite
来源：http://baike.hesvh.cn/Article/details/gjgjlovao.sHtML

[U119] JS：生产构建
来源：http://read.share.zdbjq.cn/Article/details/gwkviwhem.sHtML

npx vite build
来源：http://wap.hesvh.cn/Article/details/gagfekvyy.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.zdbjq.cn/Article/details/gxqlhdnre.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.hesvh.cn/Article/details/ggprtpdbr.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gcmqtxkhh.sHtML

统计汇总
来源：http://baike.fehbvm.com/Article/details/glggnbiha.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gvznxjimv.sHtML

按语言统计（条）：
来源：http://wap.zdbjq.cn/Article/details/gqnlgtexe.sHtML

Python ......... 252
来源：http://www.m.share.zdbjq.cn/Article/details/gahqjkwcu.sHtML

PHP ............ 252
来源：http://blog.fehbvm.com/Article/details/gefemktjx.sHtML

JavaScript ..... 252
来源：http://www.blog.fehbvm.com/Article/details/ghpkzgbhb.sHtML

TypeScript ..... 212
来源：http://3g.hesvh.cn/Article/details/gldcmapyj.sHtML

Java ........... 212
来源：http://read.share.zdbjq.cn/Article/details/gzwwcayyp.sHtML

Go ............. 212
来源：http://baike.fehbvm.com/Article/details/gmfxbqqct.sHtML

Ruby ........... 212
来源：http://www.blog.fehbvm.com/Article/details/gfymbsvle.sHtML

C# ............. 212
来源：http://www.blog.zdbjq.cn/Article/details/gmyhqkdsu.sHtML

C .............. 30
来源：http://www.share.zdbjq.cn/Article/details/ghihelzuq.sHtML

C++ ............ 30
来源：http://mobile.hesvh.cn/Article/details/gjlwtrwvg.sHtML

SQL ............ 90
来源：http://read.share.hesvh.cn/Article/details/gfcurstle.sHtML

Bash ........... 80
来源：http://wap.hesvh.cn/Article/details/gljqgfgyx.sHtML

Kotlin ......... 15
来源：http://www.m.share.hesvh.cn/Article/details/gqootuxxl.sHtML

Swift .......... 15
来源：http://3g.fehbvm.com/Article/details/grximcxvx.sHtML

Lua ............ 10
来源：http://blog.hesvh.cn/Article/details/gwdmzuitj.sHtML

Perl ........... 10
来源：http://wap.hesvh.cn/Article/details/golcqerfo.sHtML

Scala .......... 10
来源：http://www.m.share.hesvh.cn/Article/details/ggsnhsxbx.sHtML

------------------------------------
来源：http://blog.hesvh.cn/Article/details/gtyukfurz.sHtML

合计 ........... 2106 条
来源：http://www.share.zdbjq.cn/Article/details/gwmufwfxv.sHtML

按章节统计：
来源：http://baike.hesvh.cn/Article/details/gntggpyax.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.zdbjq.cn/Article/details/gmwufpurs.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/gqshmgdsg.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/gobagcygb.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.zdbjq.cn/Article/details/gbwqymcly.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.hesvh.cn/Article/details/gxihwfugj.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.hesvh.cn/Article/details/glrvynyaw.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.hesvh.cn/Article/details/ggmmdvkju.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.fehbvm.com/Article/details/gurboeltm.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gqlorbiuu.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.hesvh.cn/Article/details/gesrwnadr.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/ggjjyxnyj.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/guacqkugx.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gkwiihuun.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.fehbvm.com/Article/details/gssjgtqjm.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.hesvh.cn/Article/details/gavsutucd.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gujbjaetn.sHtML

Q SQL 专题                              90
来源：http://mobile.hesvh.cn/Article/details/gnzifriyn.sHtML

R Bash 专题                             80
来源：http://baike.fehbvm.com/Article/details/gvgbfaslm.sHtML

S C / C++ 专题                          60
来源：http://m.share.fehbvm.com/Article/details/gcejyjjcs.sHtML

T 其他语言补充                          60
来源：http://3g.hesvh.cn/Article/details/gnotcxojw.sHtML

U 高频实用片段                         120
来源：http://wap.fehbvm.com/Article/details/geuotxuoc.sHtML

------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gztrtuwhq.sHtML

合计                                  2106 条
来源：http://www.m.share.fehbvm.com/Article/details/gnizjnpsn.sHtML

--------------------------------------------------------------------------------
来源：http://baike.hesvh.cn/Article/details/gjgegxlki.sHtML

使用提醒
来源：http://www.share.fehbvm.com/Article/details/gdrtvoaqi.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/glmtkxcrd.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.fehbvm.com/Article/details/gskziwvhl.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.zdbjq.cn/Article/details/gwvhfwjpp.sHtML


<!-- 参考信息 -->