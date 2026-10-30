代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://3g.fehbvm.com/Article/details/gdiluzgds.sHtML

[T59] Scala：循环
来源：http://3g.hesvh.cn/Article/details/geekdbwdf.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.zdbjq.cn/Article/details/ggqbexklj.sHtML

[T60] Scala：折叠
来源：http://3g.zdbjq.cn/Article/details/gcvyjvkeo.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.zdbjq.cn/Article/details/gwbceikmc.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gxhaybuii.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fehbvm.com/Article/details/gbbbjnuuq.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gnbgtrlrt.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.zdbjq.cn/Article/details/gqcaawirg.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.hesvh.cn/Article/details/gvtvldqix.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.fehbvm.com/Article/details/gqfadjmer.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.hesvh.cn/Article/details/gkgvpjedu.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.zdbjq.cn/Article/details/gptpxvssc.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.hesvh.cn/Article/details/gtxekdoia.sHtML

[U04] Py：变量调试打印
来源：http://m.share.hesvh.cn/Article/details/gvulbadzb.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.hesvh.cn/Article/details/gbsitukgt.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.hesvh.cn/Article/details/gtgfobmez.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/gxtaxhgct.sHtML

[U06] Py：合并两个字典
来源：http://blog.fehbvm.com/Article/details/gwerpfyil.sHtML

{**a, **b}
来源：http://read.share.zdbjq.cn/Article/details/gokaxdfpu.sHtML

[U07] Py：反转字典键值
来源：http://3g.fehbvm.com/Article/details/gnotocwpf.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.hesvh.cn/Article/details/gkmkljsec.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.hesvh.cn/Article/details/gvklisgmy.sHtML

[y for x in nested for y in x]
来源：http://mobile.hesvh.cn/Article/details/gliocyhaz.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.fehbvm.com/Article/details/gszgbzzli.sHtML

max(d, key=d.get)
来源：http://blog.hesvh.cn/Article/details/gdeqiytpc.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.zdbjq.cn/Article/details/gtomgfmqm.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.fehbvm.com/Article/details/gdhuimaif.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.hesvh.cn/Article/details/gknnicyfo.sHtML

(x * 2 for x in arr)
来源：http://m.share.zdbjq.cn/Article/details/ggczuhhvb.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.hesvh.cn/Article/details/gtykcjkzf.sHtML

Counter(arr).most_common(3)
来源：http://baike.hesvh.cn/Article/details/gyfkxrcbx.sHtML

[U13] Py：固定长度队列
来源：http://read.share.zdbjq.cn/Article/details/gwwlecvaq.sHtML

deque(maxlen=10)
来源：http://blog.zdbjq.cn/Article/details/gqmwhrnny.sHtML

[U14] Py：分组收集到列表
来源：http://baike.hesvh.cn/Article/details/gtsdnzlcy.sHtML

defaultdict(list)
来源：http://baike.hesvh.cn/Article/details/grvsxkdvr.sHtML

[U15] Py：高精度计时
来源：http://www.blog.fehbvm.com/Article/details/gndeknghg.sHtML

t = time.perf_counter()
来源：http://m.share.fehbvm.com/Article/details/ghqlhabid.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.zdbjq.cn/Article/details/giqdeixvt.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.zdbjq.cn/Article/details/gtjszcrjo.sHtML

[U17] Py：初始化日志
来源：http://wap.zdbjq.cn/Article/details/gwkinzqbh.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.zdbjq.cn/Article/details/gjlnsgcve.sHtML

[U18] Py：预编译正则
来源：http://www.share.zdbjq.cn/Article/details/gmazqrudv.sHtML

pat = re.compile(r"\d+")
来源：http://3g.zdbjq.cn/Article/details/grfahvrwg.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.fehbvm.com/Article/details/gngmkvhgv.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.fehbvm.com/Article/details/gprbwtphn.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.fehbvm.com/Article/details/gexhiuqri.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.hesvh.cn/Article/details/geymixzjf.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.zdbjq.cn/Article/details/gisjosyhm.sHtML

@contextlib.contextmanager
来源：http://mobile.fehbvm.com/Article/details/ghzmnjaxb.sHtML

[U22] Py：矩阵转置
来源：http://wap.fehbvm.com/Article/details/gkuihisnb.sHtML

list(zip(*m))
来源：http://www.m.share.hesvh.cn/Article/details/gcjcdutrk.sHtML

[U23] Py：分块读取大文件
来源：http://blog.fehbvm.com/Article/details/gkioxlhes.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.zdbjq.cn/Article/details/geurexvex.sHtML

[U24] Py：路径操作
来源：http://read.share.zdbjq.cn/Article/details/gjbkjmydb.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.fehbvm.com/Article/details/gqnvofugn.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.fehbvm.com/Article/details/gfcmntqsr.sHtML

csv.DictReader(f)
来源：http://www.m.share.zdbjq.cn/Article/details/gukkdkwfs.sHtML

[U26] Py：并发下载
来源：http://3g.hesvh.cn/Article/details/gosqlxupc.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.hesvh.cn/Article/details/gxypxkedv.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.zdbjq.cn/Article/details/gysmiubcf.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.fehbvm.com/Article/details/gymsabzqi.sHtML

[U28] Py：类型别名
来源：http://www.m.share.zdbjq.cn/Article/details/goummwsut.sHtML

UserId = int
来源：http://www.blog.zdbjq.cn/Article/details/grbejgamw.sHtML

[U29] Py：属性校验
来源：http://m.share.hesvh.cn/Article/details/grmnjlzep.sHtML

@property 与 @x.setter 配合
来源：http://mobile.hesvh.cn/Article/details/ggarfcthu.sHtML

[U30] Py：数据类
来源：http://www.share.zdbjq.cn/Article/details/gubqslsmh.sHtML

@dataclass(slots=True)
来源：http://m.share.zdbjq.cn/Article/details/gpkbccqii.sHtML

[U31] Py：单测
来源：http://3g.fehbvm.com/Article/details/gyxbrvikp.sHtML

python -m pytest -q
来源：http://m.share.hesvh.cn/Article/details/gwhbzlssx.sHtML

[U32] Py：代码格式化
来源：http://read.share.hesvh.cn/Article/details/gcgucwnop.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.hesvh.cn/Article/details/gxndjkkjv.sHtML

[U33] Py：打包发布
来源：http://blog.hesvh.cn/Article/details/gebromxxz.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.zdbjq.cn/Article/details/gtmxxgqjt.sHtML

[U34] Py：判断编码
来源：http://www.m.share.fehbvm.com/Article/details/grveuerab.sHtML

chardet.detect(raw)
来源：http://baike.fehbvm.com/Article/details/gzeoflghu.sHtML

[U35] Py：发送邮件
来源：http://m.share.zdbjq.cn/Article/details/gwwrrovit.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.fehbvm.com/Article/details/gqfcuflsj.sHtML

[U36] Py：定时任务
来源：http://wap.fehbvm.com/Article/details/gvezpxetr.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.hesvh.cn/Article/details/gepgguqkg.sHtML

[U37] Py：读写 Excel
来源：http://baike.hesvh.cn/Article/details/goysrdtap.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.fehbvm.com/Article/details/gtuogjezj.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.hesvh.cn/Article/details/gshrqacjn.sHtML

Path(__file__).resolve().parent
来源：http://mobile.fehbvm.com/Article/details/gduoprxbl.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.hesvh.cn/Article/details/gxvcbismm.sHtML

sys.stdout.isatty()
来源：http://wap.hesvh.cn/Article/details/ghotsnbyp.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.fehbvm.com/Article/details/godegtzfu.sHtML

print("err", file=sys.stderr)
来源：http://m.share.zdbjq.cn/Article/details/gvqphyzyv.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.zdbjq.cn/Article/details/grsqhygds.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.fehbvm.com/Article/details/golbkbeoi.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.zdbjq.cn/Article/details/gsgwjcnfz.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.fehbvm.com/Article/details/gjkhlcosk.sHtML

[U43] PHP：声明命名空间
来源：http://blog.hesvh.cn/Article/details/gbryqlemq.sHtML

namespace App\Http;
来源：http://wap.zdbjq.cn/Article/details/gvxjymyuz.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.hesvh.cn/Article/details/ghyffqddm.sHtML

declare(strict_types=1);
来源：http://mobile.fehbvm.com/Article/details/gxfjzzdcu.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.zdbjq.cn/Article/details/gaooqijwn.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/grwejvhrl.sHtML

[U46] PHP：可空类型
来源：http://read.share.hesvh.cn/Article/details/gavkmyomr.sHtML

?string $name = null
来源：http://read.share.fehbvm.com/Article/details/gihskkxvf.sHtML

[U47] PHP：联合类型
来源：http://www.share.hesvh.cn/Article/details/gpdqqupdc.sHtML

int|string $id
来源：http://blog.zdbjq.cn/Article/details/gcoiveobo.sHtML

[U48] PHP：纯枚举
来源：http://3g.fehbvm.com/Article/details/gswmovzev.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.zdbjq.cn/Article/details/gupvtoxle.sHtML

[U49] PHP：只读属性
来源：http://mobile.fehbvm.com/Article/details/gxpegkbbs.sHtML

public readonly string $name
来源：http://m.share.hesvh.cn/Article/details/gmmsmxucn.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.zdbjq.cn/Article/details/genqxxfuk.sHtML

public function __construct(private int $id) {}
来源：http://read.share.fehbvm.com/Article/details/ghflgghsd.sHtML

[U51] PHP：数组解构
来源：http://blog.zdbjq.cn/Article/details/gjfchvyaq.sHtML

[$a, $b] = $arr;
来源：http://www.blog.hesvh.cn/Article/details/gabcyvnnk.sHtML

[U52] PHP：箭头函数
来源：http://blog.zdbjq.cn/Article/details/gyvtgnxjn.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.fehbvm.com/Article/details/ghzdiejqk.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.fehbvm.com/Article/details/griloqmdy.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.fehbvm.com/Article/details/grthsyhko.sHtML

[U54] PHP：空安全调用
来源：http://blog.hesvh.cn/Article/details/giztmdpxm.sHtML

$obj?->method()
来源：http://blog.hesvh.cn/Article/details/gtsswvuau.sHtML

[U55] PHP：match 表达式
来源：http://mobile.zdbjq.cn/Article/details/grbvsbgxp.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.fehbvm.com/Article/details/gcmxlfwtt.sHtML

[U56] PHP：命名参数
来源：http://www.blog.hesvh.cn/Article/details/gvmpfuouz.sHtML

f(a: 1, b: 2)
来源：http://baike.hesvh.cn/Article/details/gnoprmfsk.sHtML

[U57] PHP：字符串插值
来源：http://read.share.hesvh.cn/Article/details/grzetkubi.sHtML

"值: {$a}"
来源：http://www.m.share.zdbjq.cn/Article/details/gfjuxdesi.sHtML

[U58] PHP：数组三件套
来源：http://www.share.fehbvm.com/Article/details/gvyqfpgfq.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.fehbvm.com/Article/details/gvkjvhhtp.sHtML

[U59] PHP：自定义排序
来源：http://blog.zdbjq.cn/Article/details/gquuxudje.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.hesvh.cn/Article/details/gqlluofqg.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.hesvh.cn/Article/details/gaaklmytp.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.fehbvm.com/Article/details/gbokkhbum.sHtML

[U61] PHP：正则
来源：http://mobile.zdbjq.cn/Article/details/gntpjvsxh.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.hesvh.cn/Article/details/gosgtlowc.sHtML

[U62] PHP：日期对象
来源：http://wap.hesvh.cn/Article/details/gahhllhch.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.fehbvm.com/Article/details/gtelrtkyl.sHtML

[U63] PHP：文件读写
来源：http://blog.hesvh.cn/Article/details/ggkbpwiji.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.hesvh.cn/Article/details/gxkzpoxdg.sHtML

[U64] PHP：目录遍历
来源：http://m.share.hesvh.cn/Article/details/gwspysuia.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.fehbvm.com/Article/details/gruajdzrr.sHtML

[U65] PHP：会话
来源：http://read.share.zdbjq.cn/Article/details/gbhkmntpc.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/glepappwx.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.fehbvm.com/Article/details/gldcchdek.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.zdbjq.cn/Article/details/gezsbqyce.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.zdbjq.cn/Article/details/gadcpqqcg.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.hesvh.cn/Article/details/gprmcqulw.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.fehbvm.com/Article/details/grmsrphvb.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.fehbvm.com/Article/details/gbhxphcjc.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.hesvh.cn/Article/details/gzkmvghwm.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.zdbjq.cn/Article/details/ghivzwdne.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.fehbvm.com/Article/details/gghjdvypp.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.hesvh.cn/Article/details/ghsdvcfbt.sHtML

[U71] PHP：抛出异常
来源：http://read.share.zdbjq.cn/Article/details/gcfybdlcw.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.hesvh.cn/Article/details/gudjdetlc.sHtML

[U72] PHP：写错误日志
来源：http://wap.hesvh.cn/Article/details/gvfueycyj.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.fehbvm.com/Article/details/ggcsgvjpl.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.fehbvm.com/Article/details/gdzzphxlz.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.fehbvm.com/Article/details/gxjkffndz.sHtML

[U74] PHP：读取环境变量
来源：http://3g.fehbvm.com/Article/details/gxagubtgl.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.hesvh.cn/Article/details/gmpoctwsw.sHtML

[U75] PHP：依赖注入
来源：http://read.share.fehbvm.com/Article/details/gpqbrcjve.sHtML

composer require psr/container
来源：http://m.share.zdbjq.cn/Article/details/gkasiudnn.sHtML

[U76] PHP：简单路由
来源：http://mobile.zdbjq.cn/Article/details/ggnywhrls.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.hesvh.cn/Article/details/gjhqrnipw.sHtML

[U77] PHP：模板渲染
来源：http://baike.hesvh.cn/Article/details/gucqjjfrs.sHtML

composer require twig/twig
来源：http://www.share.fehbvm.com/Article/details/gfvbhweef.sHtML

[U78] PHP：单元测试
来源：http://wap.hesvh.cn/Article/details/gkielfpdu.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.zdbjq.cn/Article/details/gqhptsnba.sHtML

[U79] PHP：静态分析
来源：http://m.share.fehbvm.com/Article/details/ggsrohwap.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.hesvh.cn/Article/details/gwrulirwb.sHtML

[U80] PHP：代码规范修复
来源：http://wap.hesvh.cn/Article/details/gvicomowy.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.zdbjq.cn/Article/details/gzhwjdfdn.sHtML

[U81] JS：初始化项目
来源：http://wap.zdbjq.cn/Article/details/gylbblbkd.sHtML

npm init -y;  npm i express
来源：http://www.blog.hesvh.cn/Article/details/gqjwweopo.sHtML

[U82] JS：package.json 脚本
来源：http://blog.hesvh.cn/Article/details/gxekfkknb.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.fehbvm.com/Article/details/goqzijvys.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.hesvh.cn/Article/details/gnedzqola.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.fehbvm.com/Article/details/gnoofpwpu.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.zdbjq.cn/Article/details/gwcynvebw.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.fehbvm.com/Article/details/gsdyhjxod.sHtML

[U85] JS：可选链
来源：http://www.blog.fehbvm.com/Article/details/gyqpcanxz.sHtML

a?.b?.c
来源：http://3g.zdbjq.cn/Article/details/gnhgmxhee.sHtML

[U86] JS：空值合并
来源：http://www.share.zdbjq.cn/Article/details/gayxhejka.sHtML

a ?? b
来源：http://www.share.hesvh.cn/Article/details/gpthnhlun.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.zdbjq.cn/Article/details/gfakbtakq.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.fehbvm.com/Article/details/gskcfwioi.sHtML

[U88] JS：对象展开合并
来源：http://blog.fehbvm.com/Article/details/gbgbmcnth.sHtML

{ ...a, ...b }
来源：http://blog.hesvh.cn/Article/details/giirsbrot.sHtML

[U89] JS：数组去重
来源：http://www.blog.hesvh.cn/Article/details/gpsuhvizg.sHtML

[...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/ggaauqkfa.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.fehbvm.com/Article/details/gjdzyfmtn.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gvdponqav.sHtML

[U91] JS：对象键值遍历
来源：http://3g.hesvh.cn/Article/details/gjoktbayh.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.fehbvm.com/Article/details/glihuwltt.sHtML

[U92] JS：深拷贝
来源：http://m.share.hesvh.cn/Article/details/gmtjxnqgo.sHtML

structuredClone(obj)
来源：http://read.share.fehbvm.com/Article/details/goqwvdfpp.sHtML

[U93] JS：模板字符串
来源：http://read.share.hesvh.cn/Article/details/gjqrnbmbr.sHtML

`共 ${n} 条`
来源：http://www.m.share.fehbvm.com/Article/details/grtzjmfsp.sHtML

[U94] JS：箭头函数
来源：http://wap.fehbvm.com/Article/details/gomtjhqpm.sHtML

const double = x => x * 2;
来源：http://mobile.hesvh.cn/Article/details/guqonifer.sHtML

[U95] JS：Promise 包装
来源：http://www.share.zdbjq.cn/Article/details/ggslelhjm.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.fehbvm.com/Article/details/gxfcanjvg.sHtML

[U96] JS：async/await 与异常
来源：http://wap.zdbjq.cn/Article/details/gmeqxcgie.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/gqtrpegcq.sHtML

[U97] JS：并发请求
来源：http://blog.zdbjq.cn/Article/details/gpzghhryh.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/gdekwjnjk.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.hesvh.cn/Article/details/gxskbrdlc.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.hesvh.cn/Article/details/ghvmwbuvf.sHtML

[U99] JS：事件监听
来源：http://blog.fehbvm.com/Article/details/gckxaqbqz.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.hesvh.cn/Article/details/ghqmswkll.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.zdbjq.cn/Article/details/gnnvwatgt.sHtML

document.querySelector(".item")
来源：http://baike.fehbvm.com/Article/details/gxyfwmjkf.sHtML

[U101] JS：classList 操作
来源：http://mobile.hesvh.cn/Article/details/grrlhqugk.sHtML

el.classList.toggle("active")
来源：http://wap.zdbjq.cn/Article/details/grekdzifs.sHtML

[U102] JS：本地存储
来源：http://mobile.fehbvm.com/Article/details/gnzxxgzag.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.fehbvm.com/Article/details/gimbnipdr.sHtML

[U103] JS：定时器
来源：http://www.m.share.zdbjq.cn/Article/details/gfskefxik.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.zdbjq.cn/Article/details/gqxrfvfzs.sHtML

[U104] JS：防抖
来源：http://m.share.zdbjq.cn/Article/details/gbeaqknhx.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/ggbzjczwb.sHtML

[U105] JS：节流
来源：http://www.share.hesvh.cn/Article/details/gpbuvutgu.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.fehbvm.com/Article/details/giqnphrao.sHtML

[U106] JS：日期格式化
来源：http://mobile.hesvh.cn/Article/details/gnnrjvllp.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.fehbvm.com/Article/details/glskjrlcr.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.fehbvm.com/Article/details/gulweiqqm.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.hesvh.cn/Article/details/grsrgyrta.sHtML

[U108] JS：随机整数
来源：http://mobile.hesvh.cn/Article/details/gfqkrevvh.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.fehbvm.com/Article/details/gxtwdlylc.sHtML

[U109] JS：数组分组
来源：http://blog.hesvh.cn/Article/details/ghxykmigk.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.fehbvm.com/Article/details/gbbkifjls.sHtML

[U110] JS：数组分块
来源：http://www.m.share.hesvh.cn/Article/details/ghhhyykmy.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.hesvh.cn/Article/details/gbdurjckj.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.fehbvm.com/Article/details/gytbuivxv.sHtML

new Map(Object.entries(obj))
来源：http://baike.zdbjq.cn/Article/details/gzsvbfkhd.sHtML

[U112] JS：字符串补位
来源：http://wap.fehbvm.com/Article/details/gtrylypgg.sHtML

"7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/gjfccjnil.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.hesvh.cn/Article/details/ggcaojiul.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gkkuhcccz.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.hesvh.cn/Article/details/ginmzpsud.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gxcgfissk.sHtML

[U115] JS：生成 UUID
来源：http://3g.hesvh.cn/Article/details/gktpmfamd.sHtML

crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gqwgcqhxn.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.hesvh.cn/Article/details/gsuudepgm.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.zdbjq.cn/Article/details/gfneixwmz.sHtML

[U117] JS：单元测试
来源：http://m.share.fehbvm.com/Article/details/gyzcensnv.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.zdbjq.cn/Article/details/gnceczeck.sHtML

[U118] JS：开发服务器
来源：http://www.share.fehbvm.com/Article/details/gluxronek.sHtML

npm i -D vite;  npx vite
来源：http://www.share.hesvh.cn/Article/details/goyuaoptb.sHtML

[U119] JS：生产构建
来源：http://m.share.fehbvm.com/Article/details/gytwonlgt.sHtML

npx vite build
来源：http://www.m.share.zdbjq.cn/Article/details/gzcuhyokv.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.fehbvm.com/Article/details/gyndvsojt.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.hesvh.cn/Article/details/grnruxhpi.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gxupjltfz.sHtML

统计汇总
来源：http://www.share.hesvh.cn/Article/details/gewgkjcta.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gbstdqnpw.sHtML

按语言统计（条）：
来源：http://blog.hesvh.cn/Article/details/gwnmqneet.sHtML

Python ......... 252
来源：http://blog.zdbjq.cn/Article/details/ghiigpjnk.sHtML

PHP ............ 252
来源：http://blog.zdbjq.cn/Article/details/gkwrsxnst.sHtML

JavaScript ..... 252
来源：http://mobile.fehbvm.com/Article/details/gupnpxsnq.sHtML

TypeScript ..... 212
来源：http://baike.hesvh.cn/Article/details/gezqedhvk.sHtML

Java ........... 212
来源：http://www.share.hesvh.cn/Article/details/grwsmnshf.sHtML

Go ............. 212
来源：http://3g.hesvh.cn/Article/details/gvhmcikfd.sHtML

Ruby ........... 212
来源：http://baike.hesvh.cn/Article/details/gahuujtlq.sHtML

C# ............. 212
来源：http://baike.fehbvm.com/Article/details/gfnjgdkib.sHtML

C .............. 30
来源：http://baike.hesvh.cn/Article/details/gjhctfngq.sHtML

C++ ............ 30
来源：http://www.blog.fehbvm.com/Article/details/gspurnqjr.sHtML

SQL ............ 90
来源：http://read.share.hesvh.cn/Article/details/gxbtuktqi.sHtML

Bash ........... 80
来源：http://mobile.zdbjq.cn/Article/details/glstdmrcy.sHtML

Kotlin ......... 15
来源：http://www.share.hesvh.cn/Article/details/gmjrnlmqf.sHtML

Swift .......... 15
来源：http://wap.zdbjq.cn/Article/details/gixzmsves.sHtML

Lua ............ 10
来源：http://www.share.fehbvm.com/Article/details/gropdtvra.sHtML

Perl ........... 10
来源：http://blog.hesvh.cn/Article/details/giwpjptss.sHtML

Scala .......... 10
来源：http://blog.fehbvm.com/Article/details/gfygpzuro.sHtML

------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gbblimwcy.sHtML

合计 ........... 2106 条
来源：http://mobile.zdbjq.cn/Article/details/gioxmlpuf.sHtML

按章节统计：
来源：http://read.share.hesvh.cn/Article/details/gpxihmlst.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.fehbvm.com/Article/details/ggndchorc.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.fehbvm.com/Article/details/gmixiymug.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/gfdtpwgap.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.zdbjq.cn/Article/details/gtgtaczls.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.zdbjq.cn/Article/details/ghosrjdut.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.zdbjq.cn/Article/details/gkbyeqxib.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.fehbvm.com/Article/details/gysdgnsmp.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.hesvh.cn/Article/details/gzufohezy.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/ggrawhquz.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.fehbvm.com/Article/details/gzpxibkft.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gtnbzbqhd.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/ghpwzugyq.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gchnxzgxy.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.fehbvm.com/Article/details/gxfocdntk.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.zdbjq.cn/Article/details/gclaqprmv.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gvtojaaoz.sHtML

Q SQL 专题                              90
来源：http://mobile.fehbvm.com/Article/details/gmkjbvgnf.sHtML

R Bash 专题                             80
来源：http://www.blog.fehbvm.com/Article/details/gcoxvgzgt.sHtML

S C / C++ 专题                          60
来源：http://blog.fehbvm.com/Article/details/gzybmkwxz.sHtML

T 其他语言补充                          60
来源：http://www.m.share.fehbvm.com/Article/details/gichkcojf.sHtML

U 高频实用片段                         120
来源：http://www.share.hesvh.cn/Article/details/gmfqajszz.sHtML

------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/ggaqalddn.sHtML

合计                                  2106 条
来源：http://wap.zdbjq.cn/Article/details/gkfcotiww.sHtML

--------------------------------------------------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gjxipsuio.sHtML

使用提醒
来源：http://mobile.fehbvm.com/Article/details/giffrqpkk.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gdovlujdn.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.zdbjq.cn/Article/details/gybvwhjoq.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.zdbjq.cn/Article/details/guliyhpto.sHtML


<!-- 参考信息 -->