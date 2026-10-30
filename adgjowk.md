代发 wailian999

[U03] Py：加载 .env 配置
来源：http://3g.fanxiaobao.xyz/Article/details/gydbtlnxk.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.fanxiaobao.xyz/Article/details/gtjurgeet.sHtML

[U04] Py：变量调试打印
来源：http://www.share.fanxiaobao.xyz/Article/details/gagxemnfv.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.fanxiaobao.xyz/Article/details/gswtjgqvq.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.fanxiaobao.xyz/Article/details/gbqxtjmfn.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.fanxiaobao.xyz/Article/details/gkdfhlkkd.sHtML

[U06] Py：合并两个字典
来源：http://blog.fanxiaobao.xyz/Article/details/ghszlpblp.sHtML

{**a, **b}
来源：http://read.share.fanxiaobao.xyz/Article/details/gvudipnat.sHtML

[U07] Py：反转字典键值
来源：http://www.share.fanxiaobao.xyz/Article/details/ghenbzutl.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.fanxiaobao.xyz/Article/details/gbvkfgcxt.sHtML

[U08] Py：展平二维列表
来源：http://3g.fanxiaobao.xyz/Article/details/gphpbcrxv.sHtML

[y for x in nested for y in x]
来源：http://3g.fanxiaobao.xyz/Article/details/gssglziag.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.fanxiaobao.xyz/Article/details/gyqqxyrbk.sHtML

max(d, key=d.get)
来源：http://read.share.fanxiaobao.xyz/Article/details/grpblzbqb.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmvutkxsf.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfrhgvesr.sHtML

[U11] Py：生成器表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gdfozyfya.sHtML

(x * 2 for x in arr)
来源：http://3g.fanxiaobao.xyz/Article/details/ghbzfcpqa.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.fanxiaobao.xyz/Article/details/gzkxgtjlz.sHtML

Counter(arr).most_common(3)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggwybbnse.sHtML

[U13] Py：固定长度队列
来源：http://read.share.fanxiaobao.xyz/Article/details/gzdqgavre.sHtML

deque(maxlen=10)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkzbpdapb.sHtML

[U14] Py：分组收集到列表
来源：http://wap.fanxiaobao.xyz/Article/details/gzrjmlffw.sHtML

defaultdict(list)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvgmrlhqz.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbczbqsbc.sHtML

t = time.perf_counter()
来源：http://baike.fanxiaobao.xyz/Article/details/gforvopee.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxrqjmbas.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.fanxiaobao.xyz/Article/details/gfurwgxxz.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gveadckif.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.fanxiaobao.xyz/Article/details/gibzkvkrp.sHtML

[U18] Py：预编译正则
来源：http://mobile.fanxiaobao.xyz/Article/details/gqaoodoni.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/galmxpijq.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gczjcufks.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcnjhvwvp.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.fanxiaobao.xyz/Article/details/grglstkjg.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.fanxiaobao.xyz/Article/details/gitoszilu.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.fanxiaobao.xyz/Article/details/gkdhqvuhk.sHtML

@contextlib.contextmanager
来源：http://baike.fanxiaobao.xyz/Article/details/gjgsiwrci.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.fanxiaobao.xyz/Article/details/grtfedrir.sHtML

list(zip(*m))
来源：http://baike.fanxiaobao.xyz/Article/details/godytthgv.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggzxaibak.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.fanxiaobao.xyz/Article/details/glskwncnb.sHtML

[U24] Py：路径操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gmshxploz.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.fanxiaobao.xyz/Article/details/grcegwuqp.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.fanxiaobao.xyz/Article/details/gtdsgkykx.sHtML

csv.DictReader(f)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gplosfylu.sHtML

[U26] Py：并发下载
来源：http://www.share.fanxiaobao.xyz/Article/details/gbextxwss.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxfsdfrhh.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gezalyzds.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.fanxiaobao.xyz/Article/details/gvardfobt.sHtML

[U28] Py：类型别名
来源：http://www.share.fanxiaobao.xyz/Article/details/gehyvtlmh.sHtML

UserId = int
来源：http://www.share.fanxiaobao.xyz/Article/details/ghrxftxbc.sHtML

[U29] Py：属性校验
来源：http://blog.fanxiaobao.xyz/Article/details/gyfwngajc.sHtML

@property 与 @x.setter 配合
来源：http://mobile.fanxiaobao.xyz/Article/details/gcddmtrjd.sHtML

[U30] Py：数据类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gthxpkcpg.sHtML

@dataclass(slots=True)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdsdatahp.sHtML

[U31] Py：单测
来源：http://m.share.fanxiaobao.xyz/Article/details/gnodohicf.sHtML

python -m pytest -q
来源：http://wap.fanxiaobao.xyz/Article/details/gowdxdjrh.sHtML

[U32] Py：代码格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gbbntgrva.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.fanxiaobao.xyz/Article/details/gblgbdard.sHtML

[U33] Py：打包发布
来源：http://baike.fanxiaobao.xyz/Article/details/gjugbfsuc.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.fanxiaobao.xyz/Article/details/gbleipdvu.sHtML

[U34] Py：判断编码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqzcfviat.sHtML

chardet.detect(raw)
来源：http://read.share.fanxiaobao.xyz/Article/details/grgzxzfkt.sHtML

[U35] Py：发送邮件
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghfbpyasy.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.fanxiaobao.xyz/Article/details/gzpelfbbr.sHtML

[U36] Py：定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gobllsfsz.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/garxmxjnb.sHtML

[U37] Py：读写 Excel
来源：http://3g.fanxiaobao.xyz/Article/details/gsemwpwyw.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.fanxiaobao.xyz/Article/details/gaivbyglq.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.fanxiaobao.xyz/Article/details/gnbvcgzpg.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcdltgfkr.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.fanxiaobao.xyz/Article/details/gtyokiild.sHtML

sys.stdout.isatty()
来源：http://blog.fanxiaobao.xyz/Article/details/giwesmeik.sHtML

[U40] Py：打印到标准错误
来源：http://wap.fanxiaobao.xyz/Article/details/gjxvefdfx.sHtML

print("err", file=sys.stderr)
来源：http://wap.fanxiaobao.xyz/Article/details/gtdmptglg.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glrxcdled.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.fanxiaobao.xyz/Article/details/grapqspyp.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.fanxiaobao.xyz/Article/details/giibrfjia.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.fanxiaobao.xyz/Article/details/grygdlfru.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdwhknvun.sHtML

namespace App\Http;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmfjpckey.sHtML

[U44] PHP：开启严格类型
来源：http://baike.fanxiaobao.xyz/Article/details/gifosxsxd.sHtML

declare(strict_types=1);
来源：http://wap.fanxiaobao.xyz/Article/details/gblcbffgp.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.fanxiaobao.xyz/Article/details/ghtjoezgj.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gjshexzfe.sHtML

[U46] PHP：可空类型
来源：http://baike.fanxiaobao.xyz/Article/details/gsxgdtpmb.sHtML

?string $name = null
来源：http://m.share.fanxiaobao.xyz/Article/details/goevbzaxf.sHtML

[U47] PHP：联合类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gobgvosaa.sHtML

int|string $id
来源：http://mobile.fanxiaobao.xyz/Article/details/gdtjcyxbz.sHtML

[U48] PHP：纯枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gzdsetqcu.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gcwovywom.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guvcaipbd.sHtML

public readonly string $name
来源：http://baike.fanxiaobao.xyz/Article/details/glapqdbun.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvgmupofh.sHtML

public function __construct(private int $id) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gmnqejkcx.sHtML

[U51] PHP：数组解构
来源：http://blog.fanxiaobao.xyz/Article/details/gucfhaddn.sHtML

[$a, $b] = $arr;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfszqbkfw.sHtML

[U52] PHP：箭头函数
来源：http://blog.fanxiaobao.xyz/Article/details/gbfhplrre.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.fanxiaobao.xyz/Article/details/grkgssbsm.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.fanxiaobao.xyz/Article/details/guxpqetdq.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.fanxiaobao.xyz/Article/details/gzgdsaskl.sHtML

[U54] PHP：空安全调用
来源：http://baike.fanxiaobao.xyz/Article/details/gzgnzmuze.sHtML

$obj?->method()
来源：http://mobile.fanxiaobao.xyz/Article/details/gtcxtsswq.sHtML

[U55] PHP：match 表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/ggqmvzawv.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.fanxiaobao.xyz/Article/details/gfgofgmqg.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gedysdmaj.sHtML

f(a: 1, b: 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gsdeiivpg.sHtML

[U57] PHP：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/giaopjxbx.sHtML

"值: {$a}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzkpjqtvq.sHtML

[U58] PHP：数组三件套
来源：http://m.share.fanxiaobao.xyz/Article/details/gcfkglbsg.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.fanxiaobao.xyz/Article/details/gmaelwnsg.sHtML

[U59] PHP：自定义排序
来源：http://3g.fanxiaobao.xyz/Article/details/gmcbcskok.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fanxiaobao.xyz/Article/details/grlwpkoxi.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.fanxiaobao.xyz/Article/details/gmyhpvtai.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.fanxiaobao.xyz/Article/details/gfcgbkwzo.sHtML

[U61] PHP：正则
来源：http://www.share.fanxiaobao.xyz/Article/details/gdxnuittb.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtjjeuchm.sHtML

[U62] PHP：日期对象
来源：http://mobile.fanxiaobao.xyz/Article/details/gvyiorion.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqunbskm.sHtML

[U63] PHP：文件读写
来源：http://mobile.fanxiaobao.xyz/Article/details/gpzzayqsu.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.fanxiaobao.xyz/Article/details/gljmfdvlj.sHtML

[U64] PHP：目录遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gkcqfncar.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.fanxiaobao.xyz/Article/details/gbumcinaa.sHtML

[U65] PHP：会话
来源：http://read.share.fanxiaobao.xyz/Article/details/gulamlyao.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbhqurxby.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.fanxiaobao.xyz/Article/details/gwkjkdheu.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbaywsnos.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.fanxiaobao.xyz/Article/details/gyedylzep.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.fanxiaobao.xyz/Article/details/grpofuzxu.sHtML

[U68] PHP：PDO 连接
来源：http://baike.fanxiaobao.xyz/Article/details/gfukhwbwh.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.fanxiaobao.xyz/Article/details/gltmhbott.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.fanxiaobao.xyz/Article/details/glniusiig.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtrdfzmmq.sHtML

[U70] PHP：PDO 事务
来源：http://blog.fanxiaobao.xyz/Article/details/gvzlbqlzx.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.fanxiaobao.xyz/Article/details/gmywviedd.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzrntxihv.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.fanxiaobao.xyz/Article/details/gqmwnrzmw.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqgrirqcm.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbckymvqi.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.fanxiaobao.xyz/Article/details/giiaqefni.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.fanxiaobao.xyz/Article/details/gmuhoomfr.sHtML

[U74] PHP：读取环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/gsgcytfck.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.fanxiaobao.xyz/Article/details/gdrhozodq.sHtML

[U75] PHP：依赖注入
来源：http://m.share.fanxiaobao.xyz/Article/details/gdcxghxci.sHtML

composer require psr/container
来源：http://wap.fanxiaobao.xyz/Article/details/gwauhbhnb.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggazqtyye.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.fanxiaobao.xyz/Article/details/gkeccquou.sHtML

[U77] PHP：模板渲染
来源：http://baike.fanxiaobao.xyz/Article/details/gdqusjftq.sHtML

composer require twig/twig
来源：http://m.share.fanxiaobao.xyz/Article/details/gioueqwdp.sHtML

[U78] PHP：单元测试
来源：http://mobile.fanxiaobao.xyz/Article/details/gyaxgygmx.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.fanxiaobao.xyz/Article/details/guytbrfrv.sHtML

[U79] PHP：静态分析
来源：http://www.blog.fanxiaobao.xyz/Article/details/guodladgd.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.fanxiaobao.xyz/Article/details/gmhlbujgw.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.fanxiaobao.xyz/Article/details/gnmnzmosr.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.fanxiaobao.xyz/Article/details/gogcxncry.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giolyyxvj.sHtML

npm init -y;  npm i express
来源：http://mobile.fanxiaobao.xyz/Article/details/gnzegvzlk.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.fanxiaobao.xyz/Article/details/gcdwfabny.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.fanxiaobao.xyz/Article/details/gbmbwcmnm.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.fanxiaobao.xyz/Article/details/gisywdgoz.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.fanxiaobao.xyz/Article/details/gabltclkb.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.fanxiaobao.xyz/Article/details/gvuowadcj.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.fanxiaobao.xyz/Article/details/ghoxpykfc.sHtML

[U85] JS：可选链
来源：http://www.share.fanxiaobao.xyz/Article/details/gvqcrfnid.sHtML

a?.b?.c
来源：http://read.share.fanxiaobao.xyz/Article/details/gnhpgvuul.sHtML

[U86] JS：空值合并
来源：http://www.share.fanxiaobao.xyz/Article/details/glmuuyama.sHtML

a ?? b
来源：http://wap.fanxiaobao.xyz/Article/details/gsmuidxse.sHtML

[U87] JS：解构默认值
来源：http://3g.fanxiaobao.xyz/Article/details/gbzqznncn.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqwsqygik.sHtML

[U88] JS：对象展开合并
来源：http://blog.fanxiaobao.xyz/Article/details/gubjirkba.sHtML

{ ...a, ...b }
来源：http://baike.fanxiaobao.xyz/Article/details/gfblrkmhf.sHtML

[U89] JS：数组去重
来源：http://m.share.fanxiaobao.xyz/Article/details/gyxkzfuep.sHtML

[...new Set(arr)]
来源：http://mobile.fanxiaobao.xyz/Article/details/ghtymrnoo.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwudrbsdo.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.fanxiaobao.xyz/Article/details/gmrrnrbre.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/guzgvcuga.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.fanxiaobao.xyz/Article/details/gafkkoqur.sHtML

[U92] JS：深拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gdartzqwa.sHtML

structuredClone(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/geuhwnrdx.sHtML

[U93] JS：模板字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gcqpbgqjt.sHtML

`共 ${n} 条`
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtglrlljg.sHtML

[U94] JS：箭头函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gojarsyir.sHtML

const double = x => x * 2;
来源：http://wap.fanxiaobao.xyz/Article/details/gknohqxwe.sHtML

[U95] JS：Promise 包装
来源：http://www.share.fanxiaobao.xyz/Article/details/gqichihav.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.fanxiaobao.xyz/Article/details/gspabgjod.sHtML

[U96] JS：async/await 与异常
来源：http://wap.fanxiaobao.xyz/Article/details/gddvivims.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gibyreoae.sHtML

[U97] JS：并发请求
来源：http://www.share.fanxiaobao.xyz/Article/details/gvkadgsre.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fanxiaobao.xyz/Article/details/gcouxusul.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/gezycvgfp.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.fanxiaobao.xyz/Article/details/gerfqzaxr.sHtML

[U99] JS：事件监听
来源：http://baike.fanxiaobao.xyz/Article/details/gsfoynsst.sHtML

el.addEventListener("click", e => {})
来源：http://blog.fanxiaobao.xyz/Article/details/gleryzlae.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gczskgrtq.sHtML

document.querySelector(".item")
来源：http://www.share.fanxiaobao.xyz/Article/details/gtuzzrati.sHtML

[U101] JS：classList 操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gvredcolv.sHtML

el.classList.toggle("active")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gktelivim.sHtML

[U102] JS：本地存储
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjqwbneig.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.fanxiaobao.xyz/Article/details/gdjliikpl.sHtML

[U103] JS：定时器
来源：http://mobile.fanxiaobao.xyz/Article/details/goqnfmazr.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzlwfaubu.sHtML

[U104] JS：防抖
来源：http://blog.fanxiaobao.xyz/Article/details/gbyyaivzl.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gcnjolsng.sHtML

[U105] JS：节流
来源：http://baike.fanxiaobao.xyz/Article/details/givudjmxe.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.fanxiaobao.xyz/Article/details/gnfivhure.sHtML

[U106] JS：日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gjfvnnhyr.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.fanxiaobao.xyz/Article/details/glqrnlzbs.sHtML

[U107] JS：数字千分位
来源：http://www.blog.fanxiaobao.xyz/Article/details/glmhgmsus.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.fanxiaobao.xyz/Article/details/gvgsrdhzr.sHtML

[U108] JS：随机整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsifostlu.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.fanxiaobao.xyz/Article/details/gqybtnrxk.sHtML

[U109] JS：数组分组
来源：http://wap.fanxiaobao.xyz/Article/details/geveyexca.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.fanxiaobao.xyz/Article/details/glykctscc.sHtML

[U110] JS：数组分块
来源：http://blog.fanxiaobao.xyz/Article/details/gncxqszeg.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggcucezwt.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gawuhoeie.sHtML

new Map(Object.entries(obj))
来源：http://wap.fanxiaobao.xyz/Article/details/gwegptjwb.sHtML

[U112] JS：字符串补位
来源：http://blog.fanxiaobao.xyz/Article/details/gsihmhkxj.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdmtqhxtm.sHtML

[U113] JS：正则替换全部
来源：http://mobile.fanxiaobao.xyz/Article/details/gunbgpvdp.sHtML

s.replaceAll("a", "b")
来源：http://www.share.fanxiaobao.xyz/Article/details/gghytvnrh.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.fanxiaobao.xyz/Article/details/ghwmzpkew.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggaqiubms.sHtML

[U115] JS：生成 UUID
来源：http://mobile.fanxiaobao.xyz/Article/details/gbvsrzphz.sHtML

crypto.randomUUID()
来源：http://mobile.fanxiaobao.xyz/Article/details/gauuzuvwq.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.fanxiaobao.xyz/Article/details/gbxmmtaeo.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gbywifxcu.sHtML

[U117] JS：单元测试
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gurslfmyu.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.fanxiaobao.xyz/Article/details/gyypdwzwt.sHtML

[U118] JS：开发服务器
来源：http://3g.fanxiaobao.xyz/Article/details/gkvemultj.sHtML

npm i -D vite;  npx vite
来源：http://m.share.fanxiaobao.xyz/Article/details/gaatkdtcd.sHtML

[U119] JS：生产构建
来源：http://blog.fanxiaobao.xyz/Article/details/giinoqvgn.sHtML

npx vite build
来源：http://blog.fanxiaobao.xyz/Article/details/ggzwsblhy.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxqyulziz.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpzfpxlkw.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gwrpeazjl.sHtML

统计汇总
来源：http://3g.fanxiaobao.xyz/Article/details/gkejmlmkk.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gksptgspo.sHtML

按语言统计（条）：
来源：http://read.share.fanxiaobao.xyz/Article/details/govupecfz.sHtML

Python ......... 252
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzryiegvp.sHtML

PHP ............ 252
来源：http://mobile.fanxiaobao.xyz/Article/details/gkzmvijhv.sHtML

JavaScript ..... 252
来源：http://www.share.fanxiaobao.xyz/Article/details/gectwzzhw.sHtML

TypeScript ..... 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbnfkjkqv.sHtML

Java ........... 212
来源：http://3g.fanxiaobao.xyz/Article/details/gwvxixsfp.sHtML

Go ............. 212
来源：http://m.share.fanxiaobao.xyz/Article/details/ggbiwjril.sHtML

Ruby ........... 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gxmmzvdwn.sHtML

C# ............. 212
来源：http://baike.fanxiaobao.xyz/Article/details/gynvbscwj.sHtML

C .............. 30
来源：http://m.share.fanxiaobao.xyz/Article/details/gkxhwlgdm.sHtML

C++ ............ 30
来源：http://mobile.fanxiaobao.xyz/Article/details/gvoxxsoiz.sHtML

SQL ............ 90
来源：http://baike.fanxiaobao.xyz/Article/details/gehemhili.sHtML

Bash ........... 80
来源：http://wap.fanxiaobao.xyz/Article/details/guulttggv.sHtML

Kotlin ......... 15
来源：http://read.share.fanxiaobao.xyz/Article/details/goeeeyeon.sHtML

Swift .......... 15
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjbqrydej.sHtML

Lua ............ 10
来源：http://read.share.fanxiaobao.xyz/Article/details/grqwahjpz.sHtML

Perl ........... 10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtsgbdxek.sHtML

Scala .......... 10
来源：http://m.share.fanxiaobao.xyz/Article/details/gwfefsghi.sHtML

------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/gapdajaak.sHtML

合计 ........... 2106 条
来源：http://www.share.fanxiaobao.xyz/Article/details/gnetfnkki.sHtML

按章节统计：
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giatqcyaj.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.fanxiaobao.xyz/Article/details/gnzejyied.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.fanxiaobao.xyz/Article/details/gshkqlsly.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grczokgvk.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaaxeifsf.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggkyradrw.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.fanxiaobao.xyz/Article/details/gnugbonvj.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdudvjxht.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpgihssed.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/guxqtvldw.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.fanxiaobao.xyz/Article/details/gkzamdcsw.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gadmydsil.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/gidtqibce.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/geztiwtzv.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.fanxiaobao.xyz/Article/details/gpgibtwkj.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.fanxiaobao.xyz/Article/details/gblcimvla.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gwajqzfwe.sHtML

Q SQL 专题                              90
来源：http://mobile.fanxiaobao.xyz/Article/details/grrjzbfft.sHtML

R Bash 专题                             80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gohpfqpcv.sHtML

S C / C++ 专题                          60
来源：http://read.share.fanxiaobao.xyz/Article/details/gsxrzbfib.sHtML

T 其他语言补充                          60
来源：http://baike.fanxiaobao.xyz/Article/details/gpqwfhgkc.sHtML

U 高频实用片段                         120
来源：http://baike.fanxiaobao.xyz/Article/details/geepksvtm.sHtML

------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gtjyamrlw.sHtML

合计                                  2106 条
来源：http://3g.fanxiaobao.xyz/Article/details/gjkvumdll.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/ghqkmifzz.sHtML

使用提醒
来源：http://www.share.fanxiaobao.xyz/Article/details/gkcfqesuz.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkkkevcac.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.fanxiaobao.xyz/Article/details/gxaovcmke.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.fanxiaobao.xyz/Article/details/gfeppzwqv.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.fanxiaobao.xyz/Article/details/griqtaneu.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.fanxiaobao.xyz/Article/details/gyjdihzpf.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.fanxiaobao.xyz/Article/details/gwwhcavnf.sHtML

—— 文件结束 ——
来源：http://3g.fanxiaobao.xyz/Article/details/ganjeeefo.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gfuygjlwp.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnponwzqb.sHtML

Common Programming Examples Cheat Book
来源：http://blog.fanxiaobao.xyz/Article/details/gqnllbdge.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gdlhncmeg.sHtML

【收录内容】
来源：http://www.share.fanxiaobao.xyz/Article/details/gcyfalrof.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.fanxiaobao.xyz/Article/details/gasbxkwat.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtzvtgbnv.sHtML

SQL · Bash · C · C++
来源：http://www.blog.fanxiaobao.xyz/Article/details/grptmntlt.sHtML


<!-- 参考信息 -->