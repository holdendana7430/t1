代发 wailian999

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3bztvkklt.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3miufcqjq.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3befeiuki.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3utxnfphe.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3eregqlwu.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3dnzvdfty.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3yfwqyqnu.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3irsjphet.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3ydhsmybt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yrfuzjwu.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wdrihjjq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3matabbjw.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3ajuewvil.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3uejraoad.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3zopapvvt.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3zzopdzux.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3xkgrnvhk.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3pevhpkra.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3hwfmclyz.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3jrizewks.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3whkdbyvz.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3qylfjwhf.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3edexvqek.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3ivrbywfx.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3ipmuizmx.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3rwqucnph.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3ppddiaav.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3dmskifwr.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3tqjrnmwu.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3ffbrhngh.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3pmixfsfn.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3uwahrwho.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3exalijoc.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3xrfyjhwz.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3tlnwtuqo.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3ffyvznrd.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3nzljxinw.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3bchidoeu.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3yokcdckh.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3tkotabab.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3vljzvamp.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3fqwqjlox.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3adrpddtq.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3zmjlcpbk.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3vmdkiuoq.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3mxubmkmw.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3ybhbkbrl.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3njfbaqhh.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3hrfabvvh.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3dkiwgjfh.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3cihgoqhi.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3cqasrygi.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3nrpeweqc.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3wzdmwpyt.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3etdbyfir.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3rnbsgjra.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3nmihfcrs.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3qdfdmujz.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3lepzahlq.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3iipfpyld.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3whilkotn.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3mdeedulb.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3hlcofhkt.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3bmqdpfun.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3yeuyvhqo.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3bpgroovu.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3ljeabdhg.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3twcxotex.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3cfmidpqc.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3gwwoydsl.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3xqkkxktl.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3gqhxwgdd.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3tzdrrspm.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3xwrbdsmn.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3mtalqmle.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3nwbaqoai.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3eclxdujs.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3avixnlfb.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3drhrvlnv.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3wdnfyvia.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3xtanusox.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3xtalfpul.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3qwiyqpew.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3uxuaknfb.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3fhmphscy.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3eydjorqw.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3bvlvjkqx.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3fpaoxctz.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3vtwwssqr.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3idejmsjz.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3rqajsexe.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3druscuxr.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3mpvjlaqs.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3ntdxrnhz.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3ijqbmgkj.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3hwodntgm.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3wnpttqbk.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3kyagtjig.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3hbhkrigr.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3epjdjhhi.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3ytnyjanu.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3xwgpcdfj.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3dfjbusyx.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3fcwmkxbv.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3huavyvzi.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3vtugkkgy.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3yeqngjab.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3yfpxzqde.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3grutbqtu.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3jqrlzxlt.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3qexlpafy.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3phzgfcbt.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3rqtyuqbp.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3mbzzctrn.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3cgivzgzw.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3tteijdvd.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3vuitmoqz.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3kvrfjawc.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3lvwmvylk.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3lxvkxhsz.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3bdfcbgnn.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3uyfftcdr.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3wukhfgko.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xogvvqsx.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3iuqiswqt.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3hmkwdahw.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3zoujmhhx.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3pcdfwadt.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3zvbtnxea.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3eoyqqsyf.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3bowmldoq.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3nfektnzx.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3uheqrfxl.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3fcwasprt.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3ivhbnteu.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3bdenvnnx.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3augcyqpx.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3ihtmmrxl.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3lhurnysr.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3pjktegee.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3loglaetn.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xezcpftn.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3tqielqyt.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3hnxthzzq.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3nevivqwl.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3ehswdsjn.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3gpmrabov.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3uucdlild.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3evopxuua.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3htcvzzyi.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3fqhppofm.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3ryxwhepu.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3mabsdbdc.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3wzxsaqpj.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3fvtwmurl.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3ercfvtge.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3wazxlser.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3wtjlplfr.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3ykxqeknz.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3jthscowk.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3jgybfzkm.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3ilptechv.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3mmapoofv.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3kfomeybr.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3jmgvfaxd.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3fafejbmq.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3owcvumoj.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3ozovizmx.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3ozkwbzxu.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3hehdzxru.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3xatdwgsx.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3peqdhvta.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3venjruqt.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3socribrq.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3aodgvadp.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3yyblqpvq.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3lvemheof.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3ateeelxp.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3sktnyoxa.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3smekaysn.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3hhyagwtt.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3xnepeypr.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3ifwhnmmv.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3miwsftgz.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3wonkfqch.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3qdhkvzcg.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3tvxojkie.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3hetnijwd.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3qpdcfznb.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3dduakbfc.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3zzqczzod.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3smwplqth.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3igbnepmd.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3gpubvsrg.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3pdmpevog.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3uifvktsw.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fonajuzp.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3ecdeqhdg.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3mgrbjtie.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3hrzkvoxb.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3qzqtupwd.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3nscrsnst.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3bxtpjnjo.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3hwxnhljm.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3ofxkesbo.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3heqfoppr.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3tbyamawz.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3eviitwru.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3ojpkqpvt.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3xsrntlfj.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3gprcewmr.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3ehaoufst.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3bwsfefrn.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3ruywolba.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3zrvcrlms.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3jskiafre.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3hnygifut.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3iqwxvwvt.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3hidsufua.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3brnpwxdg.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3marcqchz.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3osmfrhun.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3bqoqvdgv.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3wjhxloqq.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3ikwhnggh.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3pnwbzwyj.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3rbmqizti.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3ntxsfdvh.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3crzghvee.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3tvgttahu.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3nmazbzfx.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3pjmwhgci.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3wymsbjlx.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3nhzwdfza.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3yrxunsay.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3alicfpda.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3bsxtinxl.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ssgxjzhg.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3ecqglmvh.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3keajryku.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3ucnhzbkv.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3yvwwqrrx.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3blqhxgtn.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rzrkschd.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3btoyzjmh.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3boycxrhh.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3zsreywzm.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3iemrbvix.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3iufohmpa.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3aqlisfqc.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3fswjtsaz.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3ppkarhsu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3phlswozk.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3ryfontag.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eoluvwgt.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3sixezsdk.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3kxgxjcus.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3xluszhzs.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3hzbxpiiu.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3ppdcbdsx.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3sdhjahub.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3shcvwyoq.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3atsxnzsa.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3ouenclps.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3rnjpchcl.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3bmdymobz.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3imfsjdxs.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3ddoibstw.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3zonblhkn.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3gktneowz.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3jfnuvbli.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3xnzryfrd.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3mzbehdyb.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3sdglvnvt.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3vlojzquh.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3lgejnfdp.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3usfjgbzl.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3cpceodfx.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3vnrnxxgw.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3rravjcum.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3shzsijui.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3jwohfuad.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3pzdcbuqg.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3kbvqxghc.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3qkzlyycn.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3yrcphbsr.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3nhdkjeld.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3kfmikmdo.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3sixomtlw.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3myaxjedp.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3viobevld.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ffsdaqup.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3afygzsvp.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3ykpxambd.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3xzgskahh.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3drbglmbu.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3glmmslpl.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3voprdcbp.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3qmmezxzg.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ttubtqhs.html


<!-- 参考信息 -->