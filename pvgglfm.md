代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.zdbjq.cn/Article/details/ghkonetwg.sHtML

[T59] Scala：循环
来源：http://www.share.zdbjq.cn/Article/details/gyxptlnwc.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.zdbjq.cn/Article/details/ggpqzzcwu.sHtML

[T60] Scala：折叠
来源：http://www.blog.hesvh.cn/Article/details/gzakurwsg.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.fehbvm.com/Article/details/gpcbgarby.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/grnycydrz.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.hesvh.cn/Article/details/gdihjpmlf.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gwiaykztj.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.fehbvm.com/Article/details/gtqzzuzkn.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.hesvh.cn/Article/details/gsdfizyjf.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.fehbvm.com/Article/details/gtcttyqfm.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.zdbjq.cn/Article/details/gtjwnyuwx.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.hesvh.cn/Article/details/gkfpicxko.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.hesvh.cn/Article/details/gqrswhxeo.sHtML

[U04] Py：变量调试打印
来源：http://read.share.hesvh.cn/Article/details/gqbspezin.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.fehbvm.com/Article/details/giarfiljh.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.hesvh.cn/Article/details/ggcaiklag.sHtML

list(dict.fromkeys(arr))
来源：http://blog.zdbjq.cn/Article/details/glscmmyvz.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.fehbvm.com/Article/details/ghxksetbc.sHtML

{**a, **b}
来源：http://read.share.hesvh.cn/Article/details/gxweyvucp.sHtML

[U07] Py：反转字典键值
来源：http://m.share.hesvh.cn/Article/details/gawijgnzb.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.zdbjq.cn/Article/details/gwgwpvtbx.sHtML

[U08] Py：展平二维列表
来源：http://3g.zdbjq.cn/Article/details/glrwywtge.sHtML

[y for x in nested for y in x]
来源：http://wap.hesvh.cn/Article/details/gucoaxjsm.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.fehbvm.com/Article/details/gbdixtxwv.sHtML

max(d, key=d.get)
来源：http://3g.zdbjq.cn/Article/details/gyqcxcymu.sHtML

[U10] Py：按值排序字典
来源：http://mobile.fehbvm.com/Article/details/gxpybkjtr.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.fehbvm.com/Article/details/gqagamzxc.sHtML

[U11] Py：生成器表达式
来源：http://3g.zdbjq.cn/Article/details/ggwtflsol.sHtML

(x * 2 for x in arr)
来源：http://www.share.fehbvm.com/Article/details/gattxcozh.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.hesvh.cn/Article/details/gvxgkqdce.sHtML

Counter(arr).most_common(3)
来源：http://3g.fehbvm.com/Article/details/gvbkxqiah.sHtML

[U13] Py：固定长度队列
来源：http://baike.hesvh.cn/Article/details/gmiqakzvo.sHtML

deque(maxlen=10)
来源：http://blog.hesvh.cn/Article/details/gqsqdrswi.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.fehbvm.com/Article/details/girprbhga.sHtML

defaultdict(list)
来源：http://www.m.share.hesvh.cn/Article/details/gohcccasz.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.hesvh.cn/Article/details/gbdplbwca.sHtML

t = time.perf_counter()
来源：http://3g.hesvh.cn/Article/details/glhxfaurf.sHtML

[U16] Py：命令行参数解析
来源：http://baike.zdbjq.cn/Article/details/guxhozyma.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.hesvh.cn/Article/details/gjbchckgt.sHtML

[U17] Py：初始化日志
来源：http://3g.hesvh.cn/Article/details/gxpjocqxa.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.fehbvm.com/Article/details/giruepgym.sHtML

[U18] Py：预编译正则
来源：http://mobile.fehbvm.com/Article/details/gwlxfvgzf.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.fehbvm.com/Article/details/gwuinmvjh.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.zdbjq.cn/Article/details/guorzjqmy.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.zdbjq.cn/Article/details/govgjlqbd.sHtML

[U20] Py：缓存函数结果
来源：http://baike.hesvh.cn/Article/details/gkvvcxotp.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.hesvh.cn/Article/details/gmklprivt.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.hesvh.cn/Article/details/gnbrzxppo.sHtML

@contextlib.contextmanager
来源：http://wap.fehbvm.com/Article/details/ggsxohfsq.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.zdbjq.cn/Article/details/gyquygjjt.sHtML

list(zip(*m))
来源：http://read.share.fehbvm.com/Article/details/gtaeohiht.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.zdbjq.cn/Article/details/glouwjmhe.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.fehbvm.com/Article/details/gnyjejorj.sHtML

[U24] Py：路径操作
来源：http://www.m.share.fehbvm.com/Article/details/gmjasbjko.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.fehbvm.com/Article/details/gntffikex.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.zdbjq.cn/Article/details/ghcrilxco.sHtML

csv.DictReader(f)
来源：http://blog.fehbvm.com/Article/details/gjxrcrrks.sHtML

[U26] Py：并发下载
来源：http://www.share.hesvh.cn/Article/details/ghasqpqtl.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.hesvh.cn/Article/details/gaokwzjdz.sHtML

[U27] Py：异步 HTTP
来源：http://baike.hesvh.cn/Article/details/gfciynuqu.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.zdbjq.cn/Article/details/glvbwvuaj.sHtML

[U28] Py：类型别名
来源：http://www.share.fehbvm.com/Article/details/grpxpvlzz.sHtML

UserId = int
来源：http://wap.hesvh.cn/Article/details/gyxutarna.sHtML

[U29] Py：属性校验
来源：http://baike.fehbvm.com/Article/details/ghjbwcggr.sHtML

@property 与 @x.setter 配合
来源：http://m.share.fehbvm.com/Article/details/gdzaygmif.sHtML

[U30] Py：数据类
来源：http://www.share.hesvh.cn/Article/details/gvudgpqnx.sHtML

@dataclass(slots=True)
来源：http://baike.fehbvm.com/Article/details/gydhacwtb.sHtML

[U31] Py：单测
来源：http://blog.zdbjq.cn/Article/details/gkkkikfbq.sHtML

python -m pytest -q
来源：http://3g.zdbjq.cn/Article/details/gvvtmekuk.sHtML

[U32] Py：代码格式化
来源：http://blog.zdbjq.cn/Article/details/gvdvisuqg.sHtML

ruff format . && ruff check --fix .
来源：http://wap.hesvh.cn/Article/details/glkkrcoor.sHtML

[U33] Py：打包发布
来源：http://read.share.fehbvm.com/Article/details/gcwazguuu.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.hesvh.cn/Article/details/gfeixclhe.sHtML

[U34] Py：判断编码
来源：http://3g.zdbjq.cn/Article/details/gefjykqmt.sHtML

chardet.detect(raw)
来源：http://wap.zdbjq.cn/Article/details/ghjnfvlln.sHtML

[U35] Py：发送邮件
来源：http://wap.fehbvm.com/Article/details/ggascuydh.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.fehbvm.com/Article/details/gsjokgymx.sHtML

[U36] Py：定时任务
来源：http://www.share.fehbvm.com/Article/details/gimytfgmk.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.hesvh.cn/Article/details/gnyytznlu.sHtML

[U37] Py：读写 Excel
来源：http://read.share.hesvh.cn/Article/details/gazobbdss.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.hesvh.cn/Article/details/glrwgqfli.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.zdbjq.cn/Article/details/gurhnshhj.sHtML

Path(__file__).resolve().parent
来源：http://mobile.hesvh.cn/Article/details/gahczvakc.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.zdbjq.cn/Article/details/grpivywia.sHtML

sys.stdout.isatty()
来源：http://3g.hesvh.cn/Article/details/ggjxfquma.sHtML

[U40] Py：打印到标准错误
来源：http://baike.zdbjq.cn/Article/details/gxnowneoe.sHtML

print("err", file=sys.stderr)
来源：http://3g.hesvh.cn/Article/details/gnudbomqw.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.zdbjq.cn/Article/details/glykphwfa.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.zdbjq.cn/Article/details/gmoqneirt.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.fehbvm.com/Article/details/gkzrtbort.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.fehbvm.com/Article/details/glquugkaf.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.zdbjq.cn/Article/details/gkpjqumdy.sHtML

namespace App\Http;
来源：http://www.m.share.hesvh.cn/Article/details/gdpeylphy.sHtML

[U44] PHP：开启严格类型
来源：http://wap.hesvh.cn/Article/details/gtkcifupl.sHtML

declare(strict_types=1);
来源：http://www.m.share.fehbvm.com/Article/details/gakhyvsla.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.zdbjq.cn/Article/details/gtummhjff.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gwqnejxoj.sHtML

[U46] PHP：可空类型
来源：http://mobile.zdbjq.cn/Article/details/gtomvkudr.sHtML

?string $name = null
来源：http://www.blog.fehbvm.com/Article/details/gzvfombga.sHtML

[U47] PHP：联合类型
来源：http://blog.zdbjq.cn/Article/details/gcntusbrl.sHtML

int|string $id
来源：http://wap.hesvh.cn/Article/details/gpadnppoa.sHtML

[U48] PHP：纯枚举
来源：http://www.share.zdbjq.cn/Article/details/gvzkoogwf.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.zdbjq.cn/Article/details/gsqwwpkmo.sHtML

[U49] PHP：只读属性
来源：http://m.share.fehbvm.com/Article/details/gsjjubsuv.sHtML

public readonly string $name
来源：http://read.share.zdbjq.cn/Article/details/gtqfivtoc.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.hesvh.cn/Article/details/gyqibzgih.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.hesvh.cn/Article/details/gspnzwwgi.sHtML

[U51] PHP：数组解构
来源：http://mobile.fehbvm.com/Article/details/gddilnowx.sHtML

[$a, $b] = $arr;
来源：http://mobile.hesvh.cn/Article/details/gopohtpnm.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.zdbjq.cn/Article/details/gypsdpsbp.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.zdbjq.cn/Article/details/ggtqxdowc.sHtML

[U53] PHP：空合并运算符
来源：http://wap.zdbjq.cn/Article/details/garasplck.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.hesvh.cn/Article/details/gefahqupq.sHtML

[U54] PHP：空安全调用
来源：http://mobile.fehbvm.com/Article/details/gheqvdise.sHtML

$obj?->method()
来源：http://www.blog.fehbvm.com/Article/details/grjcmzshr.sHtML

[U55] PHP：match 表达式
来源：http://wap.fehbvm.com/Article/details/gdetwzomv.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.zdbjq.cn/Article/details/gchyntbzu.sHtML

[U56] PHP：命名参数
来源：http://blog.zdbjq.cn/Article/details/gspobxrwt.sHtML

f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/gcdiwxjje.sHtML

[U57] PHP：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gwbihttvk.sHtML

"值: {$a}"
来源：http://mobile.hesvh.cn/Article/details/ghswmrots.sHtML

[U58] PHP：数组三件套
来源：http://baike.fehbvm.com/Article/details/gcwdxtfjc.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.zdbjq.cn/Article/details/gmkikhiis.sHtML

[U59] PHP：自定义排序
来源：http://blog.fehbvm.com/Article/details/gepgobnys.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fehbvm.com/Article/details/guevjjxoh.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.hesvh.cn/Article/details/gkvepmghp.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.fehbvm.com/Article/details/gwljeegbx.sHtML

[U61] PHP：正则
来源：http://baike.hesvh.cn/Article/details/gsbyvxzlj.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fehbvm.com/Article/details/gzevewnmt.sHtML

[U62] PHP：日期对象
来源：http://wap.fehbvm.com/Article/details/gbgeqgqft.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.zdbjq.cn/Article/details/giybazozn.sHtML

[U63] PHP：文件读写
来源：http://www.share.hesvh.cn/Article/details/gulkckkqz.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.fehbvm.com/Article/details/gtznbycee.sHtML

[U64] PHP：目录遍历
来源：http://3g.fehbvm.com/Article/details/gdsijzajj.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.zdbjq.cn/Article/details/gspcqyiwr.sHtML

[U65] PHP：会话
来源：http://wap.zdbjq.cn/Article/details/gqgvajxhj.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gpsaxqtri.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.zdbjq.cn/Article/details/gsbphttdz.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.zdbjq.cn/Article/details/gavsmgnvp.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.fehbvm.com/Article/details/gmxnpvmkd.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.zdbjq.cn/Article/details/gqajbnllk.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.zdbjq.cn/Article/details/gifjnghol.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.fehbvm.com/Article/details/grmrkumwj.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.hesvh.cn/Article/details/gfvhivjaz.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.hesvh.cn/Article/details/gqdsfhwib.sHtML

[U70] PHP：PDO 事务
来源：http://baike.hesvh.cn/Article/details/grgdtnhzp.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.zdbjq.cn/Article/details/gamuuouzt.sHtML

[U71] PHP：抛出异常
来源：http://m.share.hesvh.cn/Article/details/gpuhufldk.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.zdbjq.cn/Article/details/gkcwocuvz.sHtML

[U72] PHP：写错误日志
来源：http://blog.fehbvm.com/Article/details/gnfaywdlo.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.zdbjq.cn/Article/details/gyrjkkxjw.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.fehbvm.com/Article/details/ganzvhzcl.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.fehbvm.com/Article/details/gojeaqcyh.sHtML

[U74] PHP：读取环境变量
来源：http://wap.hesvh.cn/Article/details/gwqmxckah.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.fehbvm.com/Article/details/gjtltbsjl.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.fehbvm.com/Article/details/gxvwjjipt.sHtML

composer require psr/container
来源：http://blog.zdbjq.cn/Article/details/gcbgarjss.sHtML

[U76] PHP：简单路由
来源：http://3g.hesvh.cn/Article/details/gmukmhmoi.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.zdbjq.cn/Article/details/gyhgeotos.sHtML

[U77] PHP：模板渲染
来源：http://mobile.zdbjq.cn/Article/details/gboavukau.sHtML

composer require twig/twig
来源：http://baike.fehbvm.com/Article/details/gpmpqiplw.sHtML

[U78] PHP：单元测试
来源：http://m.share.zdbjq.cn/Article/details/gdslzqlur.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.hesvh.cn/Article/details/ggoqlmmha.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.zdbjq.cn/Article/details/gffglytkp.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.hesvh.cn/Article/details/gyaimlsad.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.hesvh.cn/Article/details/gwybvitrd.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.fehbvm.com/Article/details/gfvrpuiip.sHtML

[U81] JS：初始化项目
来源：http://blog.hesvh.cn/Article/details/gfxwijxxc.sHtML

npm init -y;  npm i express
来源：http://www.blog.fehbvm.com/Article/details/gobapcued.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.zdbjq.cn/Article/details/gocxqlrli.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.hesvh.cn/Article/details/gxeauiwmx.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.hesvh.cn/Article/details/gxypredqt.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.zdbjq.cn/Article/details/gxswkkqoc.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.zdbjq.cn/Article/details/gukgnpysx.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.fehbvm.com/Article/details/gyzabcnmc.sHtML

[U85] JS：可选链
来源：http://m.share.hesvh.cn/Article/details/garvwpdhr.sHtML

a?.b?.c
来源：http://3g.zdbjq.cn/Article/details/gzicevvfj.sHtML

[U86] JS：空值合并
来源：http://wap.hesvh.cn/Article/details/griztvgfq.sHtML

a ?? b
来源：http://baike.zdbjq.cn/Article/details/gafdxoawy.sHtML

[U87] JS：解构默认值
来源：http://mobile.hesvh.cn/Article/details/gaytkzmdu.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.fehbvm.com/Article/details/gewdahmyp.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.zdbjq.cn/Article/details/gnmcrmuyt.sHtML

{ ...a, ...b }
来源：http://www.blog.hesvh.cn/Article/details/gdgqzjjhb.sHtML

[U89] JS：数组去重
来源：http://read.share.fehbvm.com/Article/details/gfrfdhzto.sHtML

[...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/gwhokugcl.sHtML

[U90] JS：数字数组排序
来源：http://wap.hesvh.cn/Article/details/gbmzxnbyg.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gojdnlhty.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.hesvh.cn/Article/details/gpzucbwaw.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.fehbvm.com/Article/details/geticjsed.sHtML

[U92] JS：深拷贝
来源：http://3g.fehbvm.com/Article/details/gfdstjmbg.sHtML

structuredClone(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gcupfdjwg.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.fehbvm.com/Article/details/gxxiolskq.sHtML

`共 ${n} 条`
来源：http://3g.zdbjq.cn/Article/details/gwigdwwrv.sHtML

[U94] JS：箭头函数
来源：http://blog.fehbvm.com/Article/details/guebewljf.sHtML

const double = x => x * 2;
来源：http://www.m.share.hesvh.cn/Article/details/gmxwhihuc.sHtML

[U95] JS：Promise 包装
来源：http://www.share.fehbvm.com/Article/details/gnwyjdmsm.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.fehbvm.com/Article/details/gfulqewqm.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.fehbvm.com/Article/details/gxujakyts.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/gycwwgkuk.sHtML

[U97] JS：并发请求
来源：http://read.share.zdbjq.cn/Article/details/ggnmcwtnl.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/gqbanizss.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gppygcgca.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.hesvh.cn/Article/details/gxqalgcke.sHtML

[U99] JS：事件监听
来源：http://www.blog.fehbvm.com/Article/details/gepowfius.sHtML

el.addEventListener("click", e => {})
来源：http://baike.hesvh.cn/Article/details/gjsbooygl.sHtML

[U100] JS：DOM 查询
来源：http://www.share.fehbvm.com/Article/details/grqaybajq.sHtML

document.querySelector(".item")
来源：http://www.share.fehbvm.com/Article/details/gkkhibagr.sHtML

[U101] JS：classList 操作
来源：http://wap.fehbvm.com/Article/details/gcmrmdhhu.sHtML

el.classList.toggle("active")
来源：http://www.share.zdbjq.cn/Article/details/gbsolwqem.sHtML

[U102] JS：本地存储
来源：http://3g.fehbvm.com/Article/details/gxscahnxh.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.fehbvm.com/Article/details/gemblfkzg.sHtML

[U103] JS：定时器
来源：http://wap.hesvh.cn/Article/details/gcyyechkt.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.fehbvm.com/Article/details/gemmgggto.sHtML

[U104] JS：防抖
来源：http://read.share.zdbjq.cn/Article/details/gafxfvhac.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gvtlydkle.sHtML

[U105] JS：节流
来源：http://www.m.share.fehbvm.com/Article/details/gjlxrimfu.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.zdbjq.cn/Article/details/gmzdwlwak.sHtML

[U106] JS：日期格式化
来源：http://m.share.fehbvm.com/Article/details/gjlmiesoj.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.fehbvm.com/Article/details/gjxirntoi.sHtML

[U107] JS：数字千分位
来源：http://www.blog.zdbjq.cn/Article/details/gjukpsycd.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.hesvh.cn/Article/details/gxybltpnp.sHtML

[U108] JS：随机整数
来源：http://mobile.hesvh.cn/Article/details/gelxwbamb.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.zdbjq.cn/Article/details/giwiodtkb.sHtML

[U109] JS：数组分组
来源：http://www.share.fehbvm.com/Article/details/gcvvcbqje.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.zdbjq.cn/Article/details/gncgfesst.sHtML

[U110] JS：数组分块
来源：http://read.share.hesvh.cn/Article/details/gqawcuhlq.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.hesvh.cn/Article/details/gwgkjkfsd.sHtML

[U111] JS：对象转 Map
来源：http://blog.fehbvm.com/Article/details/gknxovild.sHtML

new Map(Object.entries(obj))
来源：http://baike.hesvh.cn/Article/details/gjbmhtplm.sHtML

[U112] JS：字符串补位
来源：http://www.blog.zdbjq.cn/Article/details/gxvhxgrda.sHtML

"7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/genkehgji.sHtML

[U113] JS：正则替换全部
来源：http://blog.fehbvm.com/Article/details/gjmxyuhef.sHtML

s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gtxqbzegd.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.zdbjq.cn/Article/details/gawepuryo.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.hesvh.cn/Article/details/garzawssw.sHtML

[U115] JS：生成 UUID
来源：http://wap.zdbjq.cn/Article/details/ggomtgoyl.sHtML

crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/glzfedppk.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.hesvh.cn/Article/details/gtgshedpe.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.hesvh.cn/Article/details/gkakzujks.sHtML

[U117] JS：单元测试
来源：http://www.blog.fehbvm.com/Article/details/gcehxysca.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.hesvh.cn/Article/details/gzyumcbjz.sHtML

[U118] JS：开发服务器
来源：http://mobile.fehbvm.com/Article/details/gbggqaukf.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.hesvh.cn/Article/details/gikduslfq.sHtML

[U119] JS：生产构建
来源：http://3g.hesvh.cn/Article/details/gqwyspmah.sHtML

npx vite build
来源：http://wap.fehbvm.com/Article/details/giebnqwic.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.zdbjq.cn/Article/details/gupgeufuo.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.fehbvm.com/Article/details/ghvohfbww.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/giucmczvh.sHtML

统计汇总
来源：http://m.share.hesvh.cn/Article/details/gdlckiywb.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gtqxhbifk.sHtML

按语言统计（条）：
来源：http://read.share.zdbjq.cn/Article/details/gnhuhhsgy.sHtML

Python ......... 252
来源：http://read.share.fehbvm.com/Article/details/gwcoaxyue.sHtML

PHP ............ 252
来源：http://baike.zdbjq.cn/Article/details/gucbpcpeu.sHtML

JavaScript ..... 252
来源：http://baike.hesvh.cn/Article/details/gpadlzgol.sHtML

TypeScript ..... 212
来源：http://www.m.share.hesvh.cn/Article/details/gxtyssjzp.sHtML

Java ........... 212
来源：http://3g.fehbvm.com/Article/details/gmwrtxpwd.sHtML

Go ............. 212
来源：http://m.share.hesvh.cn/Article/details/gsivwtmrc.sHtML

Ruby ........... 212
来源：http://3g.zdbjq.cn/Article/details/gjcorawgh.sHtML

C# ............. 212
来源：http://www.blog.hesvh.cn/Article/details/grazcvaxb.sHtML

C .............. 30
来源：http://baike.hesvh.cn/Article/details/gbyoypkkg.sHtML

C++ ............ 30
来源：http://mobile.zdbjq.cn/Article/details/grnaryqgt.sHtML

SQL ............ 90
来源：http://www.m.share.fehbvm.com/Article/details/gqtgezxko.sHtML

Bash ........... 80
来源：http://www.blog.hesvh.cn/Article/details/gjsfakrqu.sHtML

Kotlin ......... 15
来源：http://mobile.zdbjq.cn/Article/details/gbozljiif.sHtML

Swift .......... 15
来源：http://baike.hesvh.cn/Article/details/gsqoklasd.sHtML

Lua ............ 10
来源：http://www.m.share.hesvh.cn/Article/details/gxhknnwvc.sHtML

Perl ........... 10
来源：http://www.m.share.zdbjq.cn/Article/details/gpdvoluqv.sHtML

Scala .......... 10
来源：http://3g.hesvh.cn/Article/details/gzlcmyigk.sHtML

------------------------------------
来源：http://baike.hesvh.cn/Article/details/gcrslrtsz.sHtML

合计 ........... 2106 条
来源：http://wap.hesvh.cn/Article/details/gvltenvta.sHtML

按章节统计：
来源：http://3g.hesvh.cn/Article/details/gsqxfoyua.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.zdbjq.cn/Article/details/goqttufqb.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/gcdtuuria.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/gmzpbekjh.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.zdbjq.cn/Article/details/gtzidjohi.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.zdbjq.cn/Article/details/gyhhhwfud.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.hesvh.cn/Article/details/gzomruqjk.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.zdbjq.cn/Article/details/gapzxtwdm.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.hesvh.cn/Article/details/ggvtkznjt.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gfwcszzms.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.zdbjq.cn/Article/details/gdjuwubxk.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/grcupoufn.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gpnwysdgu.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gonsdndog.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.hesvh.cn/Article/details/gmqpqabmw.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.hesvh.cn/Article/details/gvgvxqbkd.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gwybmdnwo.sHtML

Q SQL 专题                              90
来源：http://www.share.fehbvm.com/Article/details/gsadcrlen.sHtML

R Bash 专题                             80
来源：http://mobile.hesvh.cn/Article/details/gcljbjsdv.sHtML

S C / C++ 专题                          60
来源：http://www.share.zdbjq.cn/Article/details/ggwabaice.sHtML

T 其他语言补充                          60
来源：http://3g.fehbvm.com/Article/details/guootfzch.sHtML

U 高频实用片段                         120
来源：http://m.share.fehbvm.com/Article/details/gqicrdhjd.sHtML

------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gcbmncech.sHtML

合计                                  2106 条
来源：http://mobile.hesvh.cn/Article/details/gotxwpech.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gxrsnxqlp.sHtML

使用提醒
来源：http://read.share.hesvh.cn/Article/details/glgkxcnev.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gnkazxgdc.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.fehbvm.com/Article/details/gmmyckyzc.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.fehbvm.com/Article/details/glvyjhzbf.sHtML


<!-- 参考信息 -->