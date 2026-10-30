代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://baike.zdbjq.cn/Article/details/gktmvfgpt.sHtML

[T55] Scala：集合过滤
来源：http://wap.fehbvm.com/Article/details/gsfvkbjry.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.hesvh.cn/Article/details/gluzdruix.sHtML

[T56] Scala：样例类
来源：http://mobile.zdbjq.cn/Article/details/gkuewvopb.sHtML

case class User(name: String, age: Int)
来源：http://wap.zdbjq.cn/Article/details/gmsbjteyt.sHtML

[T57] Scala：模式匹配
来源：http://baike.hesvh.cn/Article/details/gongibaes.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.fehbvm.com/Article/details/grpeusgil.sHtML

[T58] Scala：函数定义
来源：http://baike.fehbvm.com/Article/details/gmykekxqe.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.zdbjq.cn/Article/details/gjytnobkm.sHtML

[T59] Scala：循环
来源：http://www.m.share.hesvh.cn/Article/details/gmvrmtyot.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/gidtaxnze.sHtML

[T60] Scala：折叠
来源：http://wap.fehbvm.com/Article/details/gtoedoxig.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.zdbjq.cn/Article/details/gsbvrxufq.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ggmorhpst.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.zdbjq.cn/Article/details/gycrjrqux.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gdncsruxz.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.fehbvm.com/Article/details/goyqdslue.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.hesvh.cn/Article/details/gxuwuoptu.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.fehbvm.com/Article/details/gxoxcicdq.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.fehbvm.com/Article/details/gelgbbfgl.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.fehbvm.com/Article/details/gqrvwwbkn.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.zdbjq.cn/Article/details/gojbjlsvl.sHtML

[U04] Py：变量调试打印
来源：http://baike.zdbjq.cn/Article/details/gcaloaojb.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.zdbjq.cn/Article/details/gtacxgmkx.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.hesvh.cn/Article/details/gkpdovlkg.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.hesvh.cn/Article/details/gbcfflslb.sHtML

[U06] Py：合并两个字典
来源：http://mobile.hesvh.cn/Article/details/gaurzsqyd.sHtML

{**a, **b}
来源：http://read.share.hesvh.cn/Article/details/gqrlczecd.sHtML

[U07] Py：反转字典键值
来源：http://read.share.zdbjq.cn/Article/details/gldnsunxb.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.zdbjq.cn/Article/details/guyfxbnxi.sHtML

[U08] Py：展平二维列表
来源：http://www.share.fehbvm.com/Article/details/gvejpbkmw.sHtML

[y for x in nested for y in x]
来源：http://3g.zdbjq.cn/Article/details/gfidrabch.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.zdbjq.cn/Article/details/gcnxwaitk.sHtML

max(d, key=d.get)
来源：http://www.m.share.fehbvm.com/Article/details/gdhsxakqr.sHtML

[U10] Py：按值排序字典
来源：http://blog.zdbjq.cn/Article/details/gteuptkwh.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.zdbjq.cn/Article/details/gsljdxzbv.sHtML

[U11] Py：生成器表达式
来源：http://blog.hesvh.cn/Article/details/gnwgubdaa.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.hesvh.cn/Article/details/gmlivigbu.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.fehbvm.com/Article/details/gyywvvccs.sHtML

Counter(arr).most_common(3)
来源：http://www.share.hesvh.cn/Article/details/gwmuzunyg.sHtML

[U13] Py：固定长度队列
来源：http://blog.fehbvm.com/Article/details/gwpmhqbhr.sHtML

deque(maxlen=10)
来源：http://wap.fehbvm.com/Article/details/glmtvddvm.sHtML

[U14] Py：分组收集到列表
来源：http://blog.hesvh.cn/Article/details/gspnnltbs.sHtML

defaultdict(list)
来源：http://www.m.share.zdbjq.cn/Article/details/gcdmfrkmg.sHtML

[U15] Py：高精度计时
来源：http://read.share.zdbjq.cn/Article/details/guqnyammk.sHtML

t = time.perf_counter()
来源：http://www.blog.zdbjq.cn/Article/details/gbstiuadf.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.hesvh.cn/Article/details/grdepgvze.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.zdbjq.cn/Article/details/gbcvqnxli.sHtML

[U17] Py：初始化日志
来源：http://www.blog.hesvh.cn/Article/details/gycokyhph.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fehbvm.com/Article/details/ghxqnnljl.sHtML

[U18] Py：预编译正则
来源：http://baike.hesvh.cn/Article/details/gxmswezsq.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.zdbjq.cn/Article/details/giswjipua.sHtML

[U19] Py：正则替换带回调
来源：http://3g.hesvh.cn/Article/details/glncezgpx.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.fehbvm.com/Article/details/gdadvforh.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.fehbvm.com/Article/details/gzsadheji.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.zdbjq.cn/Article/details/gtfxfmybw.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.hesvh.cn/Article/details/gokhghlal.sHtML

@contextlib.contextmanager
来源：http://m.share.fehbvm.com/Article/details/gevmfaspq.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.fehbvm.com/Article/details/gcdfimoel.sHtML

list(zip(*m))
来源：http://blog.zdbjq.cn/Article/details/gjgwrutwc.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.zdbjq.cn/Article/details/gkhklpomd.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.fehbvm.com/Article/details/gvcfqldkz.sHtML

[U24] Py：路径操作
来源：http://www.m.share.zdbjq.cn/Article/details/gcipqewyi.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.hesvh.cn/Article/details/gzyleebii.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.zdbjq.cn/Article/details/gwhtahrcr.sHtML

csv.DictReader(f)
来源：http://blog.hesvh.cn/Article/details/grhsgdtdw.sHtML

[U26] Py：并发下载
来源：http://www.blog.hesvh.cn/Article/details/gfhfcohpp.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.fehbvm.com/Article/details/gfihsigln.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.zdbjq.cn/Article/details/gmxxbfuwf.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.zdbjq.cn/Article/details/gfcdqzgpy.sHtML

[U28] Py：类型别名
来源：http://www.share.hesvh.cn/Article/details/ggdtbctis.sHtML

UserId = int
来源：http://blog.zdbjq.cn/Article/details/gmqdqwlin.sHtML

[U29] Py：属性校验
来源：http://www.share.zdbjq.cn/Article/details/gqjbwaswn.sHtML

@property 与 @x.setter 配合
来源：http://mobile.hesvh.cn/Article/details/gfycmxxnk.sHtML

[U30] Py：数据类
来源：http://baike.zdbjq.cn/Article/details/gvlbpgvyv.sHtML

@dataclass(slots=True)
来源：http://read.share.zdbjq.cn/Article/details/grnterwbz.sHtML

[U31] Py：单测
来源：http://read.share.zdbjq.cn/Article/details/gvlcegwju.sHtML

python -m pytest -q
来源：http://mobile.hesvh.cn/Article/details/gqkbqtgnn.sHtML

[U32] Py：代码格式化
来源：http://blog.hesvh.cn/Article/details/ginxqhiri.sHtML

ruff format . && ruff check --fix .
来源：http://baike.fehbvm.com/Article/details/ggblslknv.sHtML

[U33] Py：打包发布
来源：http://mobile.fehbvm.com/Article/details/gmificnnr.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.zdbjq.cn/Article/details/gjbhxzrbf.sHtML

[U34] Py：判断编码
来源：http://3g.fehbvm.com/Article/details/gcdijxxfh.sHtML

chardet.detect(raw)
来源：http://mobile.hesvh.cn/Article/details/gylanbrhe.sHtML

[U35] Py：发送邮件
来源：http://read.share.hesvh.cn/Article/details/gevmldkfv.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.fehbvm.com/Article/details/giwcfuakr.sHtML

[U36] Py：定时任务
来源：http://www.blog.zdbjq.cn/Article/details/galtkondf.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.fehbvm.com/Article/details/gujwbduol.sHtML

[U37] Py：读写 Excel
来源：http://baike.hesvh.cn/Article/details/gtnjzkugd.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.fehbvm.com/Article/details/gmyiavxmo.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.fehbvm.com/Article/details/ggaezeisc.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.fehbvm.com/Article/details/gnfarscmo.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.hesvh.cn/Article/details/gmsmhsudy.sHtML

sys.stdout.isatty()
来源：http://wap.zdbjq.cn/Article/details/gxxzesbxj.sHtML

[U40] Py：打印到标准错误
来源：http://baike.fehbvm.com/Article/details/gqmeboqkn.sHtML

print("err", file=sys.stderr)
来源：http://3g.fehbvm.com/Article/details/gtcklqzlf.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.zdbjq.cn/Article/details/goducrdbz.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.fehbvm.com/Article/details/gpdadwhvo.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.zdbjq.cn/Article/details/gstyetmvi.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.fehbvm.com/Article/details/gokpnbedv.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.fehbvm.com/Article/details/gvkfsopqo.sHtML

namespace App\Http;
来源：http://3g.zdbjq.cn/Article/details/gatnquvsz.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.hesvh.cn/Article/details/gambtsnpx.sHtML

declare(strict_types=1);
来源：http://www.blog.fehbvm.com/Article/details/ghzhvjyvp.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.hesvh.cn/Article/details/gityhvpxz.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gxqdnibiy.sHtML

[U46] PHP：可空类型
来源：http://www.blog.fehbvm.com/Article/details/gdoxvhszp.sHtML

?string $name = null
来源：http://www.m.share.hesvh.cn/Article/details/gksshajre.sHtML

[U47] PHP：联合类型
来源：http://www.blog.fehbvm.com/Article/details/gkzyvdqxm.sHtML

int|string $id
来源：http://baike.hesvh.cn/Article/details/gxpxzotms.sHtML

[U48] PHP：纯枚举
来源：http://m.share.hesvh.cn/Article/details/gyiyupvio.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.fehbvm.com/Article/details/glsuvvnhb.sHtML

[U49] PHP：只读属性
来源：http://www.share.hesvh.cn/Article/details/gvqdpcdor.sHtML

public readonly string $name
来源：http://baike.hesvh.cn/Article/details/gxzkrsfla.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.zdbjq.cn/Article/details/gtxrnnvkz.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.zdbjq.cn/Article/details/gmwrhgifq.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.fehbvm.com/Article/details/gavqizhyz.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.zdbjq.cn/Article/details/gsnrdqztx.sHtML

[U52] PHP：箭头函数
来源：http://www.share.zdbjq.cn/Article/details/giekzxfyz.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.fehbvm.com/Article/details/gyrhryidr.sHtML

[U53] PHP：空合并运算符
来源：http://baike.zdbjq.cn/Article/details/govmmnnfo.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.fehbvm.com/Article/details/gjhyfqucg.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.hesvh.cn/Article/details/gkosmtqam.sHtML

$obj?->method()
来源：http://baike.hesvh.cn/Article/details/gongtvbmx.sHtML

[U55] PHP：match 表达式
来源：http://baike.hesvh.cn/Article/details/gewvbcwup.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.zdbjq.cn/Article/details/geonqglnk.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.fehbvm.com/Article/details/gkbijcgtq.sHtML

f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/gwlrnfgkt.sHtML

[U57] PHP：字符串插值
来源：http://3g.fehbvm.com/Article/details/gmfggfmrv.sHtML

"值: {$a}"
来源：http://3g.fehbvm.com/Article/details/gmvaewvns.sHtML

[U58] PHP：数组三件套
来源：http://mobile.zdbjq.cn/Article/details/gundatgut.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.fehbvm.com/Article/details/ggzkekvsn.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.fehbvm.com/Article/details/geloogwnw.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.hesvh.cn/Article/details/geijxctea.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.fehbvm.com/Article/details/ghzeleuju.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.fehbvm.com/Article/details/gkouwkogk.sHtML

[U61] PHP：正则
来源：http://www.share.fehbvm.com/Article/details/gjcufjkwu.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.zdbjq.cn/Article/details/gdcijghrf.sHtML

[U62] PHP：日期对象
来源：http://blog.fehbvm.com/Article/details/gmcfkwamp.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.hesvh.cn/Article/details/gxtcdhgsa.sHtML

[U63] PHP：文件读写
来源：http://wap.hesvh.cn/Article/details/ghtlloxbi.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.fehbvm.com/Article/details/gmgmtdutr.sHtML

[U64] PHP：目录遍历
来源：http://read.share.fehbvm.com/Article/details/gtznmkagf.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.hesvh.cn/Article/details/gklsbaoqu.sHtML

[U65] PHP：会话
来源：http://m.share.fehbvm.com/Article/details/gsnhsphnc.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gkelkbota.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.zdbjq.cn/Article/details/gyscttrty.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.zdbjq.cn/Article/details/grpkqwsrk.sHtML

[U67] PHP：处理文件上传
来源：http://blog.zdbjq.cn/Article/details/gdqkthuid.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.zdbjq.cn/Article/details/gsvxosaeq.sHtML

[U68] PHP：PDO 连接
来源：http://3g.hesvh.cn/Article/details/ggjcxwyec.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.fehbvm.com/Article/details/gcelemrka.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.zdbjq.cn/Article/details/gxdeqmkeo.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.zdbjq.cn/Article/details/gpttwasqk.sHtML

[U70] PHP：PDO 事务
来源：http://3g.fehbvm.com/Article/details/ghxejskxi.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.hesvh.cn/Article/details/gdlgqoomy.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.hesvh.cn/Article/details/grotzbzyd.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.fehbvm.com/Article/details/gihucmtti.sHtML

[U72] PHP：写错误日志
来源：http://mobile.zdbjq.cn/Article/details/grjchfmhm.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.hesvh.cn/Article/details/gfntdnztf.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.fehbvm.com/Article/details/gxekjizsb.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.hesvh.cn/Article/details/gquxyqhii.sHtML

[U74] PHP：读取环境变量
来源：http://blog.fehbvm.com/Article/details/ggdmwozgb.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.hesvh.cn/Article/details/giknsepzl.sHtML

[U75] PHP：依赖注入
来源：http://3g.hesvh.cn/Article/details/gbgonqbzn.sHtML

composer require psr/container
来源：http://3g.hesvh.cn/Article/details/gzhycpvov.sHtML

[U76] PHP：简单路由
来源：http://mobile.hesvh.cn/Article/details/gzomttrkc.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.fehbvm.com/Article/details/gwmjlijjh.sHtML

[U77] PHP：模板渲染
来源：http://wap.fehbvm.com/Article/details/gzegbvbls.sHtML

composer require twig/twig
来源：http://3g.fehbvm.com/Article/details/ggncbikfk.sHtML

[U78] PHP：单元测试
来源：http://mobile.hesvh.cn/Article/details/gsgxcdmio.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.fehbvm.com/Article/details/gssucctzv.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.zdbjq.cn/Article/details/gpxjtrdik.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.zdbjq.cn/Article/details/gnmibxzjz.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.fehbvm.com/Article/details/gmrwpfyfj.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.hesvh.cn/Article/details/gucwqssth.sHtML

[U81] JS：初始化项目
来源：http://3g.hesvh.cn/Article/details/gicnsvqpt.sHtML

npm init -y;  npm i express
来源：http://www.m.share.zdbjq.cn/Article/details/gseexsltv.sHtML

[U82] JS：package.json 脚本
来源：http://blog.fehbvm.com/Article/details/gfaecjqha.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.fehbvm.com/Article/details/gsriodpxz.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.hesvh.cn/Article/details/gejcbmott.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.zdbjq.cn/Article/details/gczeoyubb.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.fehbvm.com/Article/details/gkrnqfpho.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.hesvh.cn/Article/details/gvlmkuasa.sHtML

[U85] JS：可选链
来源：http://baike.fehbvm.com/Article/details/gelkpwnnc.sHtML

a?.b?.c
来源：http://wap.zdbjq.cn/Article/details/ghaolozro.sHtML

[U86] JS：空值合并
来源：http://www.m.share.fehbvm.com/Article/details/gvfaqbhby.sHtML

a ?? b
来源：http://wap.hesvh.cn/Article/details/gwrfwgwma.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.hesvh.cn/Article/details/gnbbclato.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.hesvh.cn/Article/details/goasafkuy.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.fehbvm.com/Article/details/gfcztvwwl.sHtML

{ ...a, ...b }
来源：http://mobile.zdbjq.cn/Article/details/geoadtexy.sHtML

[U89] JS：数组去重
来源：http://blog.hesvh.cn/Article/details/gmybdvyoe.sHtML

[...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gicxokdek.sHtML

[U90] JS：数字数组排序
来源：http://3g.hesvh.cn/Article/details/gmmzridrc.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/gkdjxduaw.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.fehbvm.com/Article/details/gdwbnzksi.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.zdbjq.cn/Article/details/gywjaenkg.sHtML

[U92] JS：深拷贝
来源：http://wap.zdbjq.cn/Article/details/gqpakdnxx.sHtML

structuredClone(obj)
来源：http://blog.hesvh.cn/Article/details/goxqfrrqn.sHtML

[U93] JS：模板字符串
来源：http://m.share.zdbjq.cn/Article/details/gkszcnggi.sHtML

`共 ${n} 条`
来源：http://3g.hesvh.cn/Article/details/grtynimkf.sHtML

[U94] JS：箭头函数
来源：http://www.share.hesvh.cn/Article/details/ghlhlbsrz.sHtML

const double = x => x * 2;
来源：http://www.share.zdbjq.cn/Article/details/gccqciatq.sHtML

[U95] JS：Promise 包装
来源：http://m.share.hesvh.cn/Article/details/giutaxmyp.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.hesvh.cn/Article/details/gahsijona.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.hesvh.cn/Article/details/gyusjauwn.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/gobdikhvy.sHtML

[U97] JS：并发请求
来源：http://www.m.share.hesvh.cn/Article/details/gyyahxkvj.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/gmhorvnec.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.fehbvm.com/Article/details/gedntiwxg.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.hesvh.cn/Article/details/gxrmkggdz.sHtML

[U99] JS：事件监听
来源：http://www.share.zdbjq.cn/Article/details/gcstfyfav.sHtML

el.addEventListener("click", e => {})
来源：http://wap.hesvh.cn/Article/details/gvsghhmzs.sHtML

[U100] JS：DOM 查询
来源：http://blog.zdbjq.cn/Article/details/gwbjpsulf.sHtML

document.querySelector(".item")
来源：http://baike.zdbjq.cn/Article/details/gyogszhhp.sHtML

[U101] JS：classList 操作
来源：http://www.blog.fehbvm.com/Article/details/grlxaouwg.sHtML

el.classList.toggle("active")
来源：http://m.share.hesvh.cn/Article/details/gvweqdnwd.sHtML

[U102] JS：本地存储
来源：http://m.share.zdbjq.cn/Article/details/ggegutjad.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.fehbvm.com/Article/details/gwlhcevfk.sHtML

[U103] JS：定时器
来源：http://3g.fehbvm.com/Article/details/gxxvhaloz.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.fehbvm.com/Article/details/gixcxfdsr.sHtML

[U104] JS：防抖
来源：http://mobile.fehbvm.com/Article/details/gaedhlfgi.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/gmvhgqund.sHtML

[U105] JS：节流
来源：http://m.share.zdbjq.cn/Article/details/goglseefc.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.hesvh.cn/Article/details/glluwpugs.sHtML

[U106] JS：日期格式化
来源：http://mobile.hesvh.cn/Article/details/gkdqicfzg.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.hesvh.cn/Article/details/gyxnqlrrp.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.fehbvm.com/Article/details/gywiavgsv.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.zdbjq.cn/Article/details/gyykpnzxm.sHtML

[U108] JS：随机整数
来源：http://www.share.hesvh.cn/Article/details/gzdswgkch.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.hesvh.cn/Article/details/gocxuubzd.sHtML

[U109] JS：数组分组
来源：http://blog.hesvh.cn/Article/details/gyyzdtjkv.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.hesvh.cn/Article/details/gacsebzzd.sHtML

[U110] JS：数组分块
来源：http://m.share.zdbjq.cn/Article/details/gmtesglbo.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.hesvh.cn/Article/details/gfxhwzgou.sHtML

[U111] JS：对象转 Map
来源：http://blog.fehbvm.com/Article/details/gvfxlohjv.sHtML

new Map(Object.entries(obj))
来源：http://m.share.zdbjq.cn/Article/details/gijaahgdo.sHtML

[U112] JS：字符串补位
来源：http://www.blog.hesvh.cn/Article/details/gjdiobulb.sHtML

"7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gqntehjul.sHtML

[U113] JS：正则替换全部
来源：http://www.share.fehbvm.com/Article/details/gidxvmldt.sHtML

s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/grvyeroix.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.fehbvm.com/Article/details/gqncoepsj.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.hesvh.cn/Article/details/googyajmi.sHtML

[U115] JS：生成 UUID
来源：http://mobile.fehbvm.com/Article/details/gahpmzyrp.sHtML

crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/gjerjglxw.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.zdbjq.cn/Article/details/gcfatgxde.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.hesvh.cn/Article/details/gmcbfuxep.sHtML

[U117] JS：单元测试
来源：http://www.m.share.zdbjq.cn/Article/details/gujtxahyr.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.zdbjq.cn/Article/details/gjmahroap.sHtML

[U118] JS：开发服务器
来源：http://m.share.zdbjq.cn/Article/details/gpjxcdhat.sHtML

npm i -D vite;  npx vite
来源：http://wap.hesvh.cn/Article/details/ghcnuipxw.sHtML

[U119] JS：生产构建
来源：http://www.share.fehbvm.com/Article/details/gbxqqhwfb.sHtML

npx vite build
来源：http://3g.fehbvm.com/Article/details/gcxdnqhsp.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.zdbjq.cn/Article/details/glxlelthi.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.zdbjq.cn/Article/details/gjxfdtbva.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/godlwvcbh.sHtML

统计汇总
来源：http://baike.hesvh.cn/Article/details/gnrwuqcof.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gowdumheo.sHtML

按语言统计（条）：
来源：http://mobile.hesvh.cn/Article/details/ghawxlbge.sHtML

Python ......... 252
来源：http://blog.fehbvm.com/Article/details/gxmghpofx.sHtML

PHP ............ 252
来源：http://3g.fehbvm.com/Article/details/gesbqbttu.sHtML

JavaScript ..... 252
来源：http://www.share.zdbjq.cn/Article/details/gjrrcrbsg.sHtML

TypeScript ..... 212
来源：http://wap.zdbjq.cn/Article/details/gmvwtwczf.sHtML

Java ........... 212
来源：http://www.blog.fehbvm.com/Article/details/gsehwdlzm.sHtML

Go ............. 212
来源：http://www.blog.hesvh.cn/Article/details/gfooehfam.sHtML

Ruby ........... 212
来源：http://wap.zdbjq.cn/Article/details/gepxoohsi.sHtML

C# ............. 212
来源：http://www.share.fehbvm.com/Article/details/gezvlaldn.sHtML

C .............. 30
来源：http://blog.hesvh.cn/Article/details/gpgsswbmz.sHtML

C++ ............ 30
来源：http://www.blog.fehbvm.com/Article/details/gwjskivbx.sHtML

SQL ............ 90
来源：http://m.share.hesvh.cn/Article/details/gqqxzmysq.sHtML

Bash ........... 80
来源：http://www.m.share.zdbjq.cn/Article/details/glyknnvvi.sHtML

Kotlin ......... 15
来源：http://3g.hesvh.cn/Article/details/glytpgcxc.sHtML

Swift .......... 15
来源：http://3g.zdbjq.cn/Article/details/gpcfaoyql.sHtML

Lua ............ 10
来源：http://wap.hesvh.cn/Article/details/ggbxtglqk.sHtML

Perl ........... 10
来源：http://www.blog.hesvh.cn/Article/details/gqauqqycb.sHtML

Scala .......... 10
来源：http://www.blog.fehbvm.com/Article/details/gyssftblu.sHtML

------------------------------------
来源：http://mobile.fehbvm.com/Article/details/ggbifautd.sHtML

合计 ........... 2106 条
来源：http://m.share.hesvh.cn/Article/details/gmrfdwmrv.sHtML

按章节统计：
来源：http://blog.hesvh.cn/Article/details/gnpsuqykg.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.hesvh.cn/Article/details/gkprqmwmm.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/gfmucykou.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.fehbvm.com/Article/details/gqewuqusy.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.hesvh.cn/Article/details/grubngeej.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.zdbjq.cn/Article/details/gqxitvrem.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.fehbvm.com/Article/details/gjodycqyk.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/gnowrkrxo.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.zdbjq.cn/Article/details/gqpuxdgys.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gopvyzhkz.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.zdbjq.cn/Article/details/gpzceuxqr.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gocnrxhye.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/ggxqnipdo.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gthxfjkil.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.zdbjq.cn/Article/details/gmuipolqb.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.fehbvm.com/Article/details/gpyfrtrte.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gkdjkzsxl.sHtML

Q SQL 专题                              90
来源：http://www.blog.fehbvm.com/Article/details/gqaksazph.sHtML

R Bash 专题                             80
来源：http://www.share.zdbjq.cn/Article/details/gszsbqrqa.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.zdbjq.cn/Article/details/grvtopkxl.sHtML

T 其他语言补充                          60
来源：http://www.share.fehbvm.com/Article/details/gfiiwscbo.sHtML


<!-- 参考信息 -->