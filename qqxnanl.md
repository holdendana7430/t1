代发 wailian999

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.fehbvm.com/Article/details/gyhihhoch.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gcexmoayl.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fehbvm.com/Article/details/gphbwixjn.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gnnzidqyo.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.hesvh.cn/Article/details/giifgnteu.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.hesvh.cn/Article/details/goyqzwbub.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.fehbvm.com/Article/details/goyvfejaf.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.fehbvm.com/Article/details/gsteiqfrt.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.hesvh.cn/Article/details/gnztmbcfg.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.hesvh.cn/Article/details/gfetwxuqj.sHtML

[U04] Py：变量调试打印
来源：http://wap.fehbvm.com/Article/details/gyltgjcxb.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.zdbjq.cn/Article/details/gvkmauges.sHtML

[U05] Py：列表去重且保序
来源：http://wap.fehbvm.com/Article/details/gnhobzitk.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.zdbjq.cn/Article/details/gxkeslmos.sHtML

[U06] Py：合并两个字典
来源：http://baike.zdbjq.cn/Article/details/guznofvts.sHtML

{**a, **b}
来源：http://read.share.fehbvm.com/Article/details/gjkqmzmdx.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.zdbjq.cn/Article/details/gkfqmjjuu.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.hesvh.cn/Article/details/gmqamlwra.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.hesvh.cn/Article/details/gdomnocsa.sHtML

[y for x in nested for y in x]
来源：http://wap.zdbjq.cn/Article/details/gnmvezcio.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.zdbjq.cn/Article/details/gujxlespp.sHtML

max(d, key=d.get)
来源：http://read.share.hesvh.cn/Article/details/gtzcpwoxk.sHtML

[U10] Py：按值排序字典
来源：http://www.share.zdbjq.cn/Article/details/grrnfojyu.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.zdbjq.cn/Article/details/gsabqlzbc.sHtML

[U11] Py：生成器表达式
来源：http://m.share.hesvh.cn/Article/details/grfydbvxr.sHtML

(x * 2 for x in arr)
来源：http://m.share.zdbjq.cn/Article/details/geksksxyg.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.fehbvm.com/Article/details/gmmtbragu.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gipwajsat.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.hesvh.cn/Article/details/giadraows.sHtML

deque(maxlen=10)
来源：http://www.blog.zdbjq.cn/Article/details/grklxevzp.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.fehbvm.com/Article/details/gddffvprk.sHtML

defaultdict(list)
来源：http://read.share.hesvh.cn/Article/details/gdlljenwm.sHtML

[U15] Py：高精度计时
来源：http://m.share.zdbjq.cn/Article/details/gxggrtapo.sHtML

t = time.perf_counter()
来源：http://mobile.fehbvm.com/Article/details/gluyizmdh.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.fehbvm.com/Article/details/gdlvjksuk.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.zdbjq.cn/Article/details/gzqffmmqy.sHtML

[U17] Py：初始化日志
来源：http://www.blog.zdbjq.cn/Article/details/ggqcldwmv.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.fehbvm.com/Article/details/gdyudipqe.sHtML

[U18] Py：预编译正则
来源：http://mobile.zdbjq.cn/Article/details/gmihovmec.sHtML

pat = re.compile(r"\d+")
来源：http://wap.fehbvm.com/Article/details/gbntljgem.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.hesvh.cn/Article/details/gogwvgqqk.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.fehbvm.com/Article/details/gbdrwodau.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.hesvh.cn/Article/details/gujxglcav.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.fehbvm.com/Article/details/glwnrmdct.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.zdbjq.cn/Article/details/gipjjgpqu.sHtML

@contextlib.contextmanager
来源：http://3g.zdbjq.cn/Article/details/gdpktlxqc.sHtML

[U22] Py：矩阵转置
来源：http://m.share.zdbjq.cn/Article/details/gvegnbyag.sHtML

list(zip(*m))
来源：http://www.m.share.fehbvm.com/Article/details/gnexvhvrh.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.zdbjq.cn/Article/details/gyinrmigc.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.fehbvm.com/Article/details/gplgclmwp.sHtML

[U24] Py：路径操作
来源：http://3g.fehbvm.com/Article/details/gjeevuvwc.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.fehbvm.com/Article/details/gsyjshxto.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.fehbvm.com/Article/details/gvoemrlqs.sHtML

csv.DictReader(f)
来源：http://www.share.zdbjq.cn/Article/details/gbfgmzgmp.sHtML

[U26] Py：并发下载
来源：http://baike.hesvh.cn/Article/details/gkbkyhhhf.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.zdbjq.cn/Article/details/gpallrrmt.sHtML

[U27] Py：异步 HTTP
来源：http://blog.fehbvm.com/Article/details/gexdwsmsg.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.hesvh.cn/Article/details/ggkfromzk.sHtML

[U28] Py：类型别名
来源：http://baike.fehbvm.com/Article/details/gakbhdfyo.sHtML

UserId = int
来源：http://blog.hesvh.cn/Article/details/gtanhgdzn.sHtML

[U29] Py：属性校验
来源：http://blog.zdbjq.cn/Article/details/gnckaengd.sHtML

@property 与 @x.setter 配合
来源：http://baike.zdbjq.cn/Article/details/gsgsottxm.sHtML

[U30] Py：数据类
来源：http://baike.hesvh.cn/Article/details/gvwqtczma.sHtML

@dataclass(slots=True)
来源：http://wap.zdbjq.cn/Article/details/gccigdypu.sHtML

[U31] Py：单测
来源：http://wap.fehbvm.com/Article/details/gvxyyjbfa.sHtML

python -m pytest -q
来源：http://blog.zdbjq.cn/Article/details/glcsqyerw.sHtML

[U32] Py：代码格式化
来源：http://3g.zdbjq.cn/Article/details/grrovuqod.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.hesvh.cn/Article/details/gqmqroczh.sHtML

[U33] Py：打包发布
来源：http://mobile.zdbjq.cn/Article/details/gkzxikqeb.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.hesvh.cn/Article/details/gjcrmkurd.sHtML

[U34] Py：判断编码
来源：http://blog.hesvh.cn/Article/details/ggwltnfjc.sHtML

chardet.detect(raw)
来源：http://www.m.share.fehbvm.com/Article/details/gdycdkzgk.sHtML

[U35] Py：发送邮件
来源：http://read.share.zdbjq.cn/Article/details/ghpvyszgg.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.hesvh.cn/Article/details/ghykroymw.sHtML

[U36] Py：定时任务
来源：http://mobile.zdbjq.cn/Article/details/gfnhieqdv.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.zdbjq.cn/Article/details/ggklsbler.sHtML

[U37] Py：读写 Excel
来源：http://wap.fehbvm.com/Article/details/glvjyiwng.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.fehbvm.com/Article/details/gyzmffxmr.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.zdbjq.cn/Article/details/gryigemoz.sHtML

Path(__file__).resolve().parent
来源：http://m.share.hesvh.cn/Article/details/gcixlabno.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.zdbjq.cn/Article/details/gvzywckcc.sHtML

sys.stdout.isatty()
来源：http://3g.fehbvm.com/Article/details/gyqxtxnpq.sHtML

[U40] Py：打印到标准错误
来源：http://wap.zdbjq.cn/Article/details/ggoqriaak.sHtML

print("err", file=sys.stderr)
来源：http://blog.fehbvm.com/Article/details/gxwofysui.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.zdbjq.cn/Article/details/grrakkukg.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.zdbjq.cn/Article/details/gslckrywr.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.fehbvm.com/Article/details/gnpgrcznd.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.zdbjq.cn/Article/details/gnheutodn.sHtML

[U43] PHP：声明命名空间
来源：http://3g.zdbjq.cn/Article/details/gfbkyqthc.sHtML

namespace App\Http;
来源：http://www.share.hesvh.cn/Article/details/gjlqhzppo.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.zdbjq.cn/Article/details/gpxarnsks.sHtML

declare(strict_types=1);
来源：http://3g.zdbjq.cn/Article/details/gtuhpgskd.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.fehbvm.com/Article/details/grkzybrdi.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gtzsyxcyn.sHtML

[U46] PHP：可空类型
来源：http://3g.zdbjq.cn/Article/details/gogvrkaeg.sHtML

?string $name = null
来源：http://baike.hesvh.cn/Article/details/gylbpnkjv.sHtML

[U47] PHP：联合类型
来源：http://blog.zdbjq.cn/Article/details/gpndrmsmj.sHtML

int|string $id
来源：http://www.blog.fehbvm.com/Article/details/gfqawxxsl.sHtML

[U48] PHP：纯枚举
来源：http://blog.zdbjq.cn/Article/details/gfvrzaync.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.fehbvm.com/Article/details/gvrxcfglt.sHtML

[U49] PHP：只读属性
来源：http://m.share.zdbjq.cn/Article/details/gsbhbrhxp.sHtML

public readonly string $name
来源：http://m.share.fehbvm.com/Article/details/gkdwxcpoe.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.zdbjq.cn/Article/details/gqfrnwlio.sHtML

public function __construct(private int $id) {}
来源：http://m.share.hesvh.cn/Article/details/gsluspeok.sHtML

[U51] PHP：数组解构
来源：http://blog.fehbvm.com/Article/details/gsstsjygo.sHtML

[$a, $b] = $arr;
来源：http://3g.hesvh.cn/Article/details/glfjsocls.sHtML

[U52] PHP：箭头函数
来源：http://mobile.hesvh.cn/Article/details/gzdxiaveq.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.zdbjq.cn/Article/details/gdsgiqbwj.sHtML

[U53] PHP：空合并运算符
来源：http://baike.zdbjq.cn/Article/details/gczjokhpd.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.zdbjq.cn/Article/details/gdclkseop.sHtML

[U54] PHP：空安全调用
来源：http://www.share.fehbvm.com/Article/details/gjsmgxovy.sHtML

$obj?->method()
来源：http://www.blog.zdbjq.cn/Article/details/gjmnbpsnr.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.hesvh.cn/Article/details/gvxvaanje.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.hesvh.cn/Article/details/gosisorxd.sHtML

[U56] PHP：命名参数
来源：http://read.share.hesvh.cn/Article/details/gkjzkvcff.sHtML

f(a: 1, b: 2)
来源：http://www.share.zdbjq.cn/Article/details/goliwaiha.sHtML

[U57] PHP：字符串插值
来源：http://wap.hesvh.cn/Article/details/gxolvfwmq.sHtML

"值: {$a}"
来源：http://wap.zdbjq.cn/Article/details/gspgujcrm.sHtML

[U58] PHP：数组三件套
来源：http://3g.hesvh.cn/Article/details/gtowhcwcj.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.hesvh.cn/Article/details/gitnrnngj.sHtML

[U59] PHP：自定义排序
来源：http://blog.zdbjq.cn/Article/details/gpcsidogu.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.zdbjq.cn/Article/details/gbkipmynj.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.fehbvm.com/Article/details/gsqqwpsdj.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.hesvh.cn/Article/details/gabfpmtxa.sHtML

[U61] PHP：正则
来源：http://baike.zdbjq.cn/Article/details/gbauvsprp.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.zdbjq.cn/Article/details/gfokcwhta.sHtML

[U62] PHP：日期对象
来源：http://m.share.zdbjq.cn/Article/details/gqkpcphbe.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.zdbjq.cn/Article/details/gqfticwag.sHtML

[U63] PHP：文件读写
来源：http://wap.zdbjq.cn/Article/details/gkkueoojv.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.hesvh.cn/Article/details/gbnfkwygc.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.fehbvm.com/Article/details/gybfzyjxr.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.hesvh.cn/Article/details/gzxbmjqdo.sHtML

[U65] PHP：会话
来源：http://3g.fehbvm.com/Article/details/guiydkxjr.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/grokooews.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.fehbvm.com/Article/details/gdjxjdtks.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.hesvh.cn/Article/details/gnmznetic.sHtML

[U67] PHP：处理文件上传
来源：http://wap.hesvh.cn/Article/details/ghzlmhoyv.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.fehbvm.com/Article/details/gofvxnyhs.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.hesvh.cn/Article/details/gsmalstbv.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.fehbvm.com/Article/details/gjnohkfny.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.fehbvm.com/Article/details/gkgtelhsc.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.hesvh.cn/Article/details/gvdwforvt.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.fehbvm.com/Article/details/gkmbhhnfd.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.fehbvm.com/Article/details/gvwbkghna.sHtML

[U71] PHP：抛出异常
来源：http://blog.zdbjq.cn/Article/details/giuxulphh.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.fehbvm.com/Article/details/ghmyqbzeu.sHtML

[U72] PHP：写错误日志
来源：http://blog.hesvh.cn/Article/details/gqyjgufjf.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.hesvh.cn/Article/details/grapsxoda.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.fehbvm.com/Article/details/gxrgorokf.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.zdbjq.cn/Article/details/gvtltnmwa.sHtML

[U74] PHP：读取环境变量
来源：http://3g.zdbjq.cn/Article/details/ggbrhhgny.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.zdbjq.cn/Article/details/gnmspmyut.sHtML

[U75] PHP：依赖注入
来源：http://read.share.hesvh.cn/Article/details/gjdrrqqwx.sHtML

composer require psr/container
来源：http://wap.fehbvm.com/Article/details/gxlidyayv.sHtML

[U76] PHP：简单路由
来源：http://www.blog.hesvh.cn/Article/details/gzrfajkjc.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.zdbjq.cn/Article/details/gjrsbbpoj.sHtML

[U77] PHP：模板渲染
来源：http://www.share.zdbjq.cn/Article/details/ggzrsfqcd.sHtML

composer require twig/twig
来源：http://read.share.fehbvm.com/Article/details/gwrhgatgc.sHtML

[U78] PHP：单元测试
来源：http://mobile.zdbjq.cn/Article/details/gnhrxxrbk.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.fehbvm.com/Article/details/grqepohms.sHtML

[U79] PHP：静态分析
来源：http://www.blog.fehbvm.com/Article/details/gmeetjkcj.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.hesvh.cn/Article/details/gyfdoxynf.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.fehbvm.com/Article/details/gthrraxuu.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.fehbvm.com/Article/details/gulxfrkol.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.hesvh.cn/Article/details/gbhxtsbnt.sHtML

npm init -y;  npm i express
来源：http://baike.fehbvm.com/Article/details/gljlbenuz.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.fehbvm.com/Article/details/gxviuusqw.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.fehbvm.com/Article/details/gaobzyxhc.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.hesvh.cn/Article/details/gadwwyvap.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.zdbjq.cn/Article/details/gzikzhrud.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.hesvh.cn/Article/details/gausmfzls.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.fehbvm.com/Article/details/gaxvttcys.sHtML

[U85] JS：可选链
来源：http://m.share.zdbjq.cn/Article/details/gdgeywhuh.sHtML

a?.b?.c
来源：http://www.blog.fehbvm.com/Article/details/gaimarozg.sHtML

[U86] JS：空值合并
来源：http://wap.zdbjq.cn/Article/details/gkpbyewbq.sHtML

a ?? b
来源：http://read.share.fehbvm.com/Article/details/gcijqntnu.sHtML

[U87] JS：解构默认值
来源：http://3g.fehbvm.com/Article/details/gfinwrtji.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.hesvh.cn/Article/details/guifsqele.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.zdbjq.cn/Article/details/ghhdtyqgy.sHtML

{ ...a, ...b }
来源：http://3g.hesvh.cn/Article/details/gmjifjtcw.sHtML

[U89] JS：数组去重
来源：http://read.share.fehbvm.com/Article/details/gkmevulty.sHtML

[...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/gtvvzueus.sHtML

[U90] JS：数字数组排序
来源：http://wap.zdbjq.cn/Article/details/gzvbwuvyj.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/glbaksrze.sHtML

[U91] JS：对象键值遍历
来源：http://blog.hesvh.cn/Article/details/gaoljfcgo.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.fehbvm.com/Article/details/ggsghxbck.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gptptvxrq.sHtML

structuredClone(obj)
来源：http://read.share.zdbjq.cn/Article/details/gjuschdov.sHtML

[U93] JS：模板字符串
来源：http://blog.zdbjq.cn/Article/details/gxiriqrgq.sHtML

`共 ${n} 条`
来源：http://m.share.fehbvm.com/Article/details/gwbopjmdl.sHtML

[U94] JS：箭头函数
来源：http://3g.hesvh.cn/Article/details/gbgdpxtoa.sHtML

const double = x => x * 2;
来源：http://mobile.fehbvm.com/Article/details/ghavqlnil.sHtML

[U95] JS：Promise 包装
来源：http://wap.hesvh.cn/Article/details/gnrtebpoq.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.zdbjq.cn/Article/details/gabgtsrzw.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.fehbvm.com/Article/details/gtmfaydzf.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/gjgrsbpop.sHtML

[U97] JS：并发请求
来源：http://mobile.hesvh.cn/Article/details/gqofiqmfo.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/gqaeybafz.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.fehbvm.com/Article/details/gtbuhxooo.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.zdbjq.cn/Article/details/grbpxdeiq.sHtML

[U99] JS：事件监听
来源：http://3g.fehbvm.com/Article/details/gtbvhcbdx.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.fehbvm.com/Article/details/gshmpjuwr.sHtML

[U100] JS：DOM 查询
来源：http://3g.zdbjq.cn/Article/details/gnbudrxdd.sHtML

document.querySelector(".item")
来源：http://wap.fehbvm.com/Article/details/gzfrjvind.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.zdbjq.cn/Article/details/glzxgztuc.sHtML

el.classList.toggle("active")
来源：http://www.share.hesvh.cn/Article/details/gplaisuve.sHtML

[U102] JS：本地存储
来源：http://read.share.fehbvm.com/Article/details/galhmhvmo.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.zdbjq.cn/Article/details/gkhexyhjz.sHtML

[U103] JS：定时器
来源：http://www.m.share.zdbjq.cn/Article/details/gsswdgjno.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.hesvh.cn/Article/details/gijktapvt.sHtML

[U104] JS：防抖
来源：http://m.share.zdbjq.cn/Article/details/gynjzbwqa.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/ghdjpgvcz.sHtML

[U105] JS：节流
来源：http://www.m.share.hesvh.cn/Article/details/gzpevidrd.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.hesvh.cn/Article/details/gyygerqut.sHtML

[U106] JS：日期格式化
来源：http://baike.fehbvm.com/Article/details/gffzugibt.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.fehbvm.com/Article/details/ghohlykox.sHtML

[U107] JS：数字千分位
来源：http://3g.hesvh.cn/Article/details/gndvjbvdd.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.zdbjq.cn/Article/details/gabdqldwf.sHtML

[U108] JS：随机整数
来源：http://baike.hesvh.cn/Article/details/gdiqaafja.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.fehbvm.com/Article/details/gvjopddmo.sHtML

[U109] JS：数组分组
来源：http://www.share.hesvh.cn/Article/details/gbbixjtok.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.zdbjq.cn/Article/details/gcwkypbxk.sHtML

[U110] JS：数组分块
来源：http://read.share.fehbvm.com/Article/details/glqnqbzfi.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.hesvh.cn/Article/details/glfxohilc.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.hesvh.cn/Article/details/gtcqxjydo.sHtML

new Map(Object.entries(obj))
来源：http://read.share.zdbjq.cn/Article/details/gyrngpuqm.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.zdbjq.cn/Article/details/gqbwsgtex.sHtML

"7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/guzzhkjel.sHtML

[U113] JS：正则替换全部
来源：http://3g.hesvh.cn/Article/details/gxhyvuepv.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gghhtwsus.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.zdbjq.cn/Article/details/gquubveeb.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fehbvm.com/Article/details/glshbyqoc.sHtML

[U115] JS：生成 UUID
来源：http://mobile.hesvh.cn/Article/details/gmrwdupiu.sHtML

crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/gvmictrrm.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.hesvh.cn/Article/details/gfzjqawhs.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.fehbvm.com/Article/details/gjgxpcctp.sHtML

[U117] JS：单元测试
来源：http://mobile.hesvh.cn/Article/details/gbhphwuls.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.hesvh.cn/Article/details/ghhmgglji.sHtML

[U118] JS：开发服务器
来源：http://www.share.hesvh.cn/Article/details/gwotdsjro.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.fehbvm.com/Article/details/gyzjuxvas.sHtML

[U119] JS：生产构建
来源：http://wap.fehbvm.com/Article/details/gnaojsejd.sHtML

npx vite build
来源：http://www.blog.hesvh.cn/Article/details/gnxyzhilb.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.zdbjq.cn/Article/details/gplycmsmb.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.fehbvm.com/Article/details/gnzynbrfx.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gwblouphb.sHtML

统计汇总
来源：http://www.m.share.fehbvm.com/Article/details/grhthuipo.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gjwdrlcte.sHtML

按语言统计（条）：
来源：http://www.m.share.fehbvm.com/Article/details/gmtcaygqh.sHtML

Python ......... 252
来源：http://3g.hesvh.cn/Article/details/gjcyksqct.sHtML

PHP ............ 252
来源：http://blog.zdbjq.cn/Article/details/gtkffkaoz.sHtML

JavaScript ..... 252
来源：http://blog.zdbjq.cn/Article/details/glezyyfzw.sHtML

TypeScript ..... 212
来源：http://wap.fehbvm.com/Article/details/ggcogmfru.sHtML

Java ........... 212
来源：http://www.blog.zdbjq.cn/Article/details/gmqjocare.sHtML

Go ............. 212
来源：http://3g.hesvh.cn/Article/details/gdsaqmkgy.sHtML

Ruby ........... 212
来源：http://blog.fehbvm.com/Article/details/gswecjogd.sHtML

C# ............. 212
来源：http://m.share.hesvh.cn/Article/details/gwrziwtbs.sHtML

C .............. 30
来源：http://3g.zdbjq.cn/Article/details/gvdkgzlka.sHtML

C++ ............ 30
来源：http://wap.zdbjq.cn/Article/details/ggocvalmy.sHtML

SQL ............ 90
来源：http://m.share.fehbvm.com/Article/details/gebjiiuxv.sHtML

Bash ........... 80
来源：http://blog.hesvh.cn/Article/details/gdmjvxuid.sHtML

Kotlin ......... 15
来源：http://read.share.zdbjq.cn/Article/details/ghngyfldw.sHtML

Swift .......... 15
来源：http://www.share.hesvh.cn/Article/details/gbltlyxos.sHtML

Lua ............ 10
来源：http://www.share.hesvh.cn/Article/details/grwnkpyor.sHtML

Perl ........... 10
来源：http://m.share.zdbjq.cn/Article/details/gkwscuedg.sHtML

Scala .......... 10
来源：http://blog.fehbvm.com/Article/details/gczckpner.sHtML

------------------------------------
来源：http://wap.hesvh.cn/Article/details/guyecuthc.sHtML

合计 ........... 2106 条
来源：http://wap.zdbjq.cn/Article/details/gqcicxeql.sHtML

按章节统计：
来源：http://read.share.zdbjq.cn/Article/details/gfjgpodfo.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.hesvh.cn/Article/details/gkjqirltt.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/ggipvrhms.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.hesvh.cn/Article/details/gykxdliuu.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.hesvh.cn/Article/details/gvrqchavi.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.zdbjq.cn/Article/details/goliewxng.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.fehbvm.com/Article/details/giiyoyifl.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.hesvh.cn/Article/details/gjreiiddc.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.fehbvm.com/Article/details/glkvwmrfb.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gczxgxeoc.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.zdbjq.cn/Article/details/gylwoaels.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gkdwwifxg.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gtvxpmhae.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gyjzdkzsk.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.hesvh.cn/Article/details/giregjyeh.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.fehbvm.com/Article/details/gzxgqffjt.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gxpmvwoim.sHtML

Q SQL 专题                              90
来源：http://blog.fehbvm.com/Article/details/gvtfqqdko.sHtML

R Bash 专题                             80
来源：http://3g.fehbvm.com/Article/details/gyhjlprzw.sHtML

S C / C++ 专题                          60
来源：http://www.share.zdbjq.cn/Article/details/gvqmpgpyb.sHtML

T 其他语言补充                          60
来源：http://wap.hesvh.cn/Article/details/gfntorrig.sHtML

U 高频实用片段                         120
来源：http://wap.zdbjq.cn/Article/details/gjlqxsjvo.sHtML

------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gdqsezvbe.sHtML

合计                                  2106 条
来源：http://wap.zdbjq.cn/Article/details/gtumecajf.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/gpjftghfg.sHtML

使用提醒
来源：http://mobile.fehbvm.com/Article/details/gngwvqgxj.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/glbvwquvt.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.fehbvm.com/Article/details/gcmyvceql.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.zdbjq.cn/Article/details/gicznvigb.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.zdbjq.cn/Article/details/gwrziqmux.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.hesvh.cn/Article/details/glrgixovl.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.zdbjq.cn/Article/details/ggkvrvhlb.sHtML

—— 文件结束 ——
来源：http://mobile.zdbjq.cn/Article/details/gvybgjhko.sHtML


<!-- 参考信息 -->