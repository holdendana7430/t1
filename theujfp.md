代发 wailian999

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.fanxiaobao.xyz/Article/details/gcligoitp.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gdpazlcnf.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdalxwntg.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gxkysbxfl.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.fanxiaobao.xyz/Article/details/gpbkiyvia.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.fanxiaobao.xyz/Article/details/gvouamllo.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.fanxiaobao.xyz/Article/details/gucpmbdbx.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/ghugzdzap.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.fanxiaobao.xyz/Article/details/ghjgnhnzs.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.fanxiaobao.xyz/Article/details/gnkpyxapb.sHtML

[U04] Py：变量调试打印
来源：http://wap.fanxiaobao.xyz/Article/details/gyvahwypi.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.fanxiaobao.xyz/Article/details/ghdcxfsnn.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.fanxiaobao.xyz/Article/details/gyewreodp.sHtML

list(dict.fromkeys(arr))
来源：http://3g.fanxiaobao.xyz/Article/details/giytmggmf.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gqbvrthdv.sHtML

{**a, **b}
来源：http://baike.fanxiaobao.xyz/Article/details/gnqlctttx.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gohnjorbf.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjntkyufk.sHtML

[U08] Py：展平二维列表
来源：http://baike.fanxiaobao.xyz/Article/details/geduecqci.sHtML

[y for x in nested for y in x]
来源：http://3g.fanxiaobao.xyz/Article/details/gjswkfqvn.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.fanxiaobao.xyz/Article/details/gaczvfrjn.sHtML

max(d, key=d.get)
来源：http://3g.fanxiaobao.xyz/Article/details/glracncwp.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsntumghd.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grgykxchn.sHtML

[U11] Py：生成器表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gzzhctxkk.sHtML

(x * 2 for x in arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghxfjzxji.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqzeekgct.sHtML

Counter(arr).most_common(3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqqrolrsu.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcopbboil.sHtML

deque(maxlen=10)
来源：http://mobile.fanxiaobao.xyz/Article/details/gohtpbupq.sHtML

[U14] Py：分组收集到列表
来源：http://baike.fanxiaobao.xyz/Article/details/gatguqfkq.sHtML

defaultdict(list)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gixqohwky.sHtML

[U15] Py：高精度计时
来源：http://m.share.fanxiaobao.xyz/Article/details/gzjjhvcvq.sHtML

t = time.perf_counter()
来源：http://baike.fanxiaobao.xyz/Article/details/gkcsylawb.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.fanxiaobao.xyz/Article/details/grsieskaj.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.fanxiaobao.xyz/Article/details/geflzsrbf.sHtML

[U17] Py：初始化日志
来源：http://www.share.fanxiaobao.xyz/Article/details/ggkqcupid.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjdvufnfa.sHtML

[U18] Py：预编译正则
来源：http://wap.fanxiaobao.xyz/Article/details/gvyyvtopc.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/gsgjkccns.sHtML

[U19] Py：正则替换带回调
来源：http://blog.fanxiaobao.xyz/Article/details/gwewfmnyp.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gesegoyac.sHtML

[U20] Py：缓存函数结果
来源：http://baike.fanxiaobao.xyz/Article/details/gdlcrqqca.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.fanxiaobao.xyz/Article/details/gixdxgywp.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.fanxiaobao.xyz/Article/details/gygdtgmoz.sHtML

@contextlib.contextmanager
来源：http://mobile.fanxiaobao.xyz/Article/details/gcylmgpxm.sHtML

[U22] Py：矩阵转置
来源：http://www.share.fanxiaobao.xyz/Article/details/giaoayuzq.sHtML

list(zip(*m))
来源：http://blog.fanxiaobao.xyz/Article/details/gqdwridvj.sHtML

[U23] Py：分块读取大文件
来源：http://blog.fanxiaobao.xyz/Article/details/gdimchclz.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.fanxiaobao.xyz/Article/details/gpwxvujtg.sHtML

[U24] Py：路径操作
来源：http://baike.fanxiaobao.xyz/Article/details/gxjshpasq.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.fanxiaobao.xyz/Article/details/gzwhyjvuo.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.fanxiaobao.xyz/Article/details/gkizxanmy.sHtML

csv.DictReader(f)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghlqbcldk.sHtML

[U26] Py：并发下载
来源：http://wap.fanxiaobao.xyz/Article/details/gqngmnrqj.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.fanxiaobao.xyz/Article/details/gjnzepcfj.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnggzxzhe.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.fanxiaobao.xyz/Article/details/gxdjvnsnu.sHtML

[U28] Py：类型别名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpbeqxtso.sHtML

UserId = int
来源：http://read.share.fanxiaobao.xyz/Article/details/gblkjfvjk.sHtML

[U29] Py：属性校验
来源：http://mobile.fanxiaobao.xyz/Article/details/gloealjga.sHtML

@property 与 @x.setter 配合
来源：http://wap.fanxiaobao.xyz/Article/details/gmdcmsizt.sHtML

[U30] Py：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/gteondrhr.sHtML

@dataclass(slots=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggqennsxc.sHtML

[U31] Py：单测
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvaixnmjm.sHtML

python -m pytest -q
来源：http://blog.fanxiaobao.xyz/Article/details/ggadrxcnu.sHtML

[U32] Py：代码格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gkpdjqgvw.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxgklmll.sHtML

[U33] Py：打包发布
来源：http://www.share.fanxiaobao.xyz/Article/details/gglxacrog.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.fanxiaobao.xyz/Article/details/gizyocfti.sHtML

[U34] Py：判断编码
来源：http://m.share.fanxiaobao.xyz/Article/details/gvqqyjapv.sHtML

chardet.detect(raw)
来源：http://blog.fanxiaobao.xyz/Article/details/gcebpjlor.sHtML

[U35] Py：发送邮件
来源：http://read.share.fanxiaobao.xyz/Article/details/godinzhng.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.fanxiaobao.xyz/Article/details/gklkjaqmx.sHtML

[U36] Py：定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gushifmyg.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghgxffxjm.sHtML

[U37] Py：读写 Excel
来源：http://m.share.fanxiaobao.xyz/Article/details/gtaaztgja.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnplbglam.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fanxiaobao.xyz/Article/details/grehwolya.sHtML

Path(__file__).resolve().parent
来源：http://read.share.fanxiaobao.xyz/Article/details/ghwqxltso.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.fanxiaobao.xyz/Article/details/gazuohhjg.sHtML

sys.stdout.isatty()
来源：http://baike.fanxiaobao.xyz/Article/details/gitiyzjmy.sHtML

[U40] Py：打印到标准错误
来源：http://blog.fanxiaobao.xyz/Article/details/ghzttkega.sHtML

print("err", file=sys.stderr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtnjyagzu.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.fanxiaobao.xyz/Article/details/ggkqwzmbr.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqwczkctj.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.fanxiaobao.xyz/Article/details/gdarhbhzg.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gsxhgjxap.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/gzsbqjmov.sHtML

namespace App\Http;
来源：http://blog.fanxiaobao.xyz/Article/details/gbwqkfyrk.sHtML

[U44] PHP：开启严格类型
来源：http://blog.fanxiaobao.xyz/Article/details/gbxpvbomk.sHtML

declare(strict_types=1);
来源：http://m.share.fanxiaobao.xyz/Article/details/gyxboibax.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.fanxiaobao.xyz/Article/details/ggmoitjap.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gddgrolnc.sHtML

[U46] PHP：可空类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gnymbsleq.sHtML

?string $name = null
来源：http://read.share.fanxiaobao.xyz/Article/details/gyvvefjqn.sHtML

[U47] PHP：联合类型
来源：http://blog.fanxiaobao.xyz/Article/details/gumtxncum.sHtML

int|string $id
来源：http://read.share.fanxiaobao.xyz/Article/details/gwygjbtwt.sHtML

[U48] PHP：纯枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gpvqufofd.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqghwhrra.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghmtkkbwt.sHtML

public readonly string $name
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grhgjehtr.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.fanxiaobao.xyz/Article/details/gsviymsdr.sHtML

public function __construct(private int $id) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gtimladpf.sHtML

[U51] PHP：数组解构
来源：http://www.share.fanxiaobao.xyz/Article/details/gliasfcev.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpemgbqpn.sHtML

[U52] PHP：箭头函数
来源：http://blog.fanxiaobao.xyz/Article/details/gxwexjivh.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.fanxiaobao.xyz/Article/details/gdxfupaob.sHtML

[U53] PHP：空合并运算符
来源：http://blog.fanxiaobao.xyz/Article/details/gcedvoqzz.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.fanxiaobao.xyz/Article/details/goffgvauw.sHtML

[U54] PHP：空安全调用
来源：http://3g.fanxiaobao.xyz/Article/details/galcmegck.sHtML

$obj?->method()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcsihmplc.sHtML

[U55] PHP：match 表达式
来源：http://blog.fanxiaobao.xyz/Article/details/grlqystiu.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqetnkjzf.sHtML

[U56] PHP：命名参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gupdksevb.sHtML

f(a: 1, b: 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghgttazrl.sHtML

[U57] PHP：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gombezjlg.sHtML

"值: {$a}"
来源：http://3g.fanxiaobao.xyz/Article/details/gafxpuptn.sHtML

[U58] PHP：数组三件套
来源：http://read.share.fanxiaobao.xyz/Article/details/gbvhvmwne.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxetfmrtc.sHtML

[U59] PHP：自定义排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjplfjle.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fanxiaobao.xyz/Article/details/geqhzkpth.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.fanxiaobao.xyz/Article/details/gmlvcorlg.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.fanxiaobao.xyz/Article/details/gascthotv.sHtML

[U61] PHP：正则
来源：http://3g.fanxiaobao.xyz/Article/details/gmcyozzsv.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzzijdzhk.sHtML

[U62] PHP：日期对象
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxlroueum.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.fanxiaobao.xyz/Article/details/gscrdihwo.sHtML

[U63] PHP：文件读写
来源：http://blog.fanxiaobao.xyz/Article/details/gjojrmdzc.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.fanxiaobao.xyz/Article/details/grpbjmnsw.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goiybbsiy.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.fanxiaobao.xyz/Article/details/gyxyyncjg.sHtML

[U65] PHP：会话
来源：http://www.blog.fanxiaobao.xyz/Article/details/glpjhcnpz.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcejemryp.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.fanxiaobao.xyz/Article/details/gtawakmst.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnlhbvwwz.sHtML

[U67] PHP：处理文件上传
来源：http://baike.fanxiaobao.xyz/Article/details/gorlqdltr.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.fanxiaobao.xyz/Article/details/gibclbnoc.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gfihsnpba.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.fanxiaobao.xyz/Article/details/guxgjeixr.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.fanxiaobao.xyz/Article/details/gjvwcfuxp.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.fanxiaobao.xyz/Article/details/glnsfqueb.sHtML

[U70] PHP：PDO 事务
来源：http://3g.fanxiaobao.xyz/Article/details/gfujodant.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyhjwrpbq.sHtML

[U71] PHP：抛出异常
来源：http://read.share.fanxiaobao.xyz/Article/details/gofoojlnv.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.fanxiaobao.xyz/Article/details/gbdgxjgxe.sHtML

[U72] PHP：写错误日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gmtkndqpt.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.fanxiaobao.xyz/Article/details/ggebsuqix.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.fanxiaobao.xyz/Article/details/gdnrbrnun.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.fanxiaobao.xyz/Article/details/gvxqumzuo.sHtML

[U74] PHP：读取环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/gyejcatno.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gevbxkbor.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyzzpkfpv.sHtML

composer require psr/container
来源：http://www.blog.fanxiaobao.xyz/Article/details/gljvtotfz.sHtML

[U76] PHP：简单路由
来源：http://mobile.fanxiaobao.xyz/Article/details/geoasxnxl.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.fanxiaobao.xyz/Article/details/gxfwstsmn.sHtML

[U77] PHP：模板渲染
来源：http://3g.fanxiaobao.xyz/Article/details/gzwfuseso.sHtML

composer require twig/twig
来源：http://read.share.fanxiaobao.xyz/Article/details/geeragqzc.sHtML

[U78] PHP：单元测试
来源：http://www.share.fanxiaobao.xyz/Article/details/gotayljgt.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.fanxiaobao.xyz/Article/details/gxckwsixt.sHtML

[U79] PHP：静态分析
来源：http://3g.fanxiaobao.xyz/Article/details/goacvsqit.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.fanxiaobao.xyz/Article/details/gxpkatpvl.sHtML

[U80] PHP：代码规范修复
来源：http://blog.fanxiaobao.xyz/Article/details/glxuwwtin.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.fanxiaobao.xyz/Article/details/gqapzdfck.sHtML

[U81] JS：初始化项目
来源：http://m.share.fanxiaobao.xyz/Article/details/gfjvtvpwh.sHtML

npm init -y;  npm i express
来源：http://baike.fanxiaobao.xyz/Article/details/gdxsfoemq.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.fanxiaobao.xyz/Article/details/gvclaybyk.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.fanxiaobao.xyz/Article/details/gmjzbrdjd.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.fanxiaobao.xyz/Article/details/ghpdhtrej.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdfhahqwk.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.fanxiaobao.xyz/Article/details/gquphelgd.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.fanxiaobao.xyz/Article/details/gowcldlbt.sHtML

[U85] JS：可选链
来源：http://read.share.fanxiaobao.xyz/Article/details/gaddmssfg.sHtML

a?.b?.c
来源：http://3g.fanxiaobao.xyz/Article/details/gqpaduydu.sHtML

[U86] JS：空值合并
来源：http://www.share.fanxiaobao.xyz/Article/details/gexgfnqvf.sHtML

a ?? b
来源：http://3g.fanxiaobao.xyz/Article/details/gasmubxrk.sHtML

[U87] JS：解构默认值
来源：http://baike.fanxiaobao.xyz/Article/details/gksbsovwy.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghnqznmvk.sHtML

[U88] JS：对象展开合并
来源：http://blog.fanxiaobao.xyz/Article/details/gcorfpcju.sHtML

{ ...a, ...b }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxkntxhqo.sHtML

[U89] JS：数组去重
来源：http://wap.fanxiaobao.xyz/Article/details/gwxcxfkjh.sHtML

[...new Set(arr)]
来源：http://read.share.fanxiaobao.xyz/Article/details/gptnafddb.sHtML

[U90] JS：数字数组排序
来源：http://3g.fanxiaobao.xyz/Article/details/gssmrhnam.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbedlkqng.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gldmhgxtl.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.fanxiaobao.xyz/Article/details/gqikmfnzy.sHtML

[U92] JS：深拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gasnfoppy.sHtML

structuredClone(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gibbvjlbv.sHtML

[U93] JS：模板字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwrivnes.sHtML

`共 ${n} 条`
来源：http://3g.fanxiaobao.xyz/Article/details/gahvaalmm.sHtML

[U94] JS：箭头函数
来源：http://wap.fanxiaobao.xyz/Article/details/gdcqnfeij.sHtML

const double = x => x * 2;
来源：http://wap.fanxiaobao.xyz/Article/details/gotwpzifo.sHtML

[U95] JS：Promise 包装
来源：http://read.share.fanxiaobao.xyz/Article/details/groiocfav.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvhwsacer.sHtML

[U96] JS：async/await 与异常
来源：http://wap.fanxiaobao.xyz/Article/details/gbokmkolu.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpezahksx.sHtML

[U97] JS：并发请求
来源：http://3g.fanxiaobao.xyz/Article/details/gtctmxbhr.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fanxiaobao.xyz/Article/details/gwcjcukdx.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/getzonxnr.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyoscqfha.sHtML

[U99] JS：事件监听
来源：http://www.share.fanxiaobao.xyz/Article/details/grlxakijz.sHtML

el.addEventListener("click", e => {})
来源：http://baike.fanxiaobao.xyz/Article/details/gddlosaup.sHtML

[U100] JS：DOM 查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gisoktkpv.sHtML

document.querySelector(".item")
来源：http://baike.fanxiaobao.xyz/Article/details/gjftvhbzj.sHtML

[U101] JS：classList 操作
来源：http://3g.fanxiaobao.xyz/Article/details/gkssslfzl.sHtML

el.classList.toggle("active")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glkfbinpe.sHtML

[U102] JS：本地存储
来源：http://baike.fanxiaobao.xyz/Article/details/gmhdhnkyc.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.fanxiaobao.xyz/Article/details/gzwvtgost.sHtML

[U103] JS：定时器
来源：http://m.share.fanxiaobao.xyz/Article/details/gnnnoouzq.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.fanxiaobao.xyz/Article/details/gffqyhdbh.sHtML

[U104] JS：防抖
来源：http://baike.fanxiaobao.xyz/Article/details/gbhbkuqke.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gavemxuuk.sHtML

[U105] JS：节流
来源：http://www.blog.fanxiaobao.xyz/Article/details/gltwizjue.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmrwqlynx.sHtML

[U106] JS：日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/giokadxdv.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.fanxiaobao.xyz/Article/details/gvqbzqlna.sHtML

[U107] JS：数字千分位
来源：http://wap.fanxiaobao.xyz/Article/details/gqxutkvdr.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.fanxiaobao.xyz/Article/details/gunhlayqk.sHtML

[U108] JS：随机整数
来源：http://read.share.fanxiaobao.xyz/Article/details/gzaxbpmvz.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.fanxiaobao.xyz/Article/details/ghfqexqxm.sHtML

[U109] JS：数组分组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkmsnbrjk.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggbcjnzpn.sHtML

[U110] JS：数组分块
来源：http://www.share.fanxiaobao.xyz/Article/details/gotkaxioz.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.fanxiaobao.xyz/Article/details/giyisdaej.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghspgxsak.sHtML

new Map(Object.entries(obj))
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjmijojx.sHtML

[U112] JS：字符串补位
来源：http://m.share.fanxiaobao.xyz/Article/details/gngsgkgwz.sHtML

"7".padStart(3, "0")
来源：http://www.share.fanxiaobao.xyz/Article/details/gdjbctqhl.sHtML

[U113] JS：正则替换全部
来源：http://wap.fanxiaobao.xyz/Article/details/gswcoogij.sHtML

s.replaceAll("a", "b")
来源：http://wap.fanxiaobao.xyz/Article/details/gubfrfzql.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjvmjghko.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fanxiaobao.xyz/Article/details/gdpwyyvpr.sHtML

[U115] JS：生成 UUID
来源：http://3g.fanxiaobao.xyz/Article/details/ggglhoypy.sHtML

crypto.randomUUID()
来源：http://wap.fanxiaobao.xyz/Article/details/gvajwitzu.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.fanxiaobao.xyz/Article/details/gvgdlxnom.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.fanxiaobao.xyz/Article/details/goekvqetk.sHtML

[U117] JS：单元测试
来源：http://www.blog.fanxiaobao.xyz/Article/details/grrejtnvb.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.fanxiaobao.xyz/Article/details/gpkmthupt.sHtML

[U118] JS：开发服务器
来源：http://m.share.fanxiaobao.xyz/Article/details/gjvnzrnum.sHtML

npm i -D vite;  npx vite
来源：http://read.share.fanxiaobao.xyz/Article/details/gcgtoybel.sHtML

[U119] JS：生产构建
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkmmzlpyw.sHtML

npx vite build
来源：http://m.share.fanxiaobao.xyz/Article/details/gbkimoiam.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.fanxiaobao.xyz/Article/details/gnbmegdmv.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjeygmsmh.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gvlhhpwrt.sHtML

统计汇总
来源：http://wap.fanxiaobao.xyz/Article/details/grnszqzzn.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gfjnvzgkw.sHtML

按语言统计（条）：
来源：http://www.share.fanxiaobao.xyz/Article/details/gyomoahgk.sHtML

Python ......... 252
来源：http://blog.fanxiaobao.xyz/Article/details/gneuqcxjj.sHtML

PHP ............ 252
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdegajsju.sHtML

JavaScript ..... 252
来源：http://baike.fanxiaobao.xyz/Article/details/golslqfgy.sHtML

TypeScript ..... 212
来源：http://3g.fanxiaobao.xyz/Article/details/gxzlkxdrc.sHtML

Java ........... 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghqaepsix.sHtML

Go ............. 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gppkddryc.sHtML

Ruby ........... 212
来源：http://3g.fanxiaobao.xyz/Article/details/gxrqdcktt.sHtML

C# ............. 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gjmnwtbwy.sHtML

C .............. 30
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gekbvhofw.sHtML

C++ ............ 30
来源：http://baike.fanxiaobao.xyz/Article/details/gpepbspxp.sHtML

SQL ............ 90
来源：http://3g.fanxiaobao.xyz/Article/details/gkjklqflw.sHtML

Bash ........... 80
来源：http://read.share.fanxiaobao.xyz/Article/details/gmfpbsbbo.sHtML

Kotlin ......... 15
来源：http://www.blog.fanxiaobao.xyz/Article/details/gphkyykmx.sHtML

Swift .......... 15
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gztopygro.sHtML

Lua ............ 10
来源：http://www.share.fanxiaobao.xyz/Article/details/gcqdnspov.sHtML

Perl ........... 10
来源：http://wap.fanxiaobao.xyz/Article/details/gftbgerua.sHtML

Scala .......... 10
来源：http://3g.fanxiaobao.xyz/Article/details/gzhcnqmqb.sHtML

------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/ghnuygmke.sHtML

合计 ........... 2106 条
来源：http://3g.fanxiaobao.xyz/Article/details/gnvbertug.sHtML

按章节统计：
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyzcyogso.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqyghcxtz.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwbzsdsw.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkjtbfnld.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.fanxiaobao.xyz/Article/details/gihpmbdln.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.fanxiaobao.xyz/Article/details/gihjeulia.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.fanxiaobao.xyz/Article/details/gvngxdbzr.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.fanxiaobao.xyz/Article/details/gcaurnjfh.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.fanxiaobao.xyz/Article/details/guvghyrkq.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/goxbzzfjv.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.fanxiaobao.xyz/Article/details/gfwndilfh.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/gwvgphodl.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/guzfwwsgz.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/grrykfjju.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.fanxiaobao.xyz/Article/details/gunmqgoso.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.fanxiaobao.xyz/Article/details/gwmrlvbgx.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/gbiuedlrh.sHtML

Q SQL 专题                              90
来源：http://mobile.fanxiaobao.xyz/Article/details/gyaohlivn.sHtML

R Bash 专题                             80
来源：http://m.share.fanxiaobao.xyz/Article/details/grsszhfdo.sHtML

S C / C++ 专题                          60
来源：http://blog.fanxiaobao.xyz/Article/details/gmspkblgs.sHtML

T 其他语言补充                          60
来源：http://baike.fanxiaobao.xyz/Article/details/gqirvjbaz.sHtML

U 高频实用片段                         120
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqhnbnnqt.sHtML

------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/gnmetiwxa.sHtML

合计                                  2106 条
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbbnjcqod.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtxbygafm.sHtML

使用提醒
来源：http://wap.fanxiaobao.xyz/Article/details/gghcvouqm.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/gyzqcovpc.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.fanxiaobao.xyz/Article/details/grdrfvcgt.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtwmawaco.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.fanxiaobao.xyz/Article/details/goxjbobhy.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gojoasuwu.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.fanxiaobao.xyz/Article/details/gcietzafj.sHtML

—— 文件结束 ——
来源：http://read.share.fanxiaobao.xyz/Article/details/gprzbnhid.sHtML


<!-- 参考信息 -->