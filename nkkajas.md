代发 wailian999

case class User(name: String, age: Int)
来源：http://wap.fehbvm.com/Article/details/ghjycykex.sHtML

[T57] Scala：模式匹配
来源：http://3g.fehbvm.com/Article/details/gxislwypv.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.fehbvm.com/Article/details/guhjlwtwr.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.fehbvm.com/Article/details/gclbyxews.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.zdbjq.cn/Article/details/gzaqkqphq.sHtML

[T59] Scala：循环
来源：http://wap.zdbjq.cn/Article/details/gkqyvrdow.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.fehbvm.com/Article/details/grlomcvtj.sHtML

[T60] Scala：折叠
来源：http://www.share.zdbjq.cn/Article/details/gvqygwbqp.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.zdbjq.cn/Article/details/geiynxuxy.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ghjctnzdr.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.zdbjq.cn/Article/details/ginkfiitc.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gtbmjcuwh.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.zdbjq.cn/Article/details/gwotsqjli.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.zdbjq.cn/Article/details/gdygzmylq.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.zdbjq.cn/Article/details/grnxqdqsy.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.hesvh.cn/Article/details/gkcctdrtl.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.zdbjq.cn/Article/details/gtarptuoc.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.fehbvm.com/Article/details/gdtdtjwod.sHtML

[U04] Py：变量调试打印
来源：http://mobile.fehbvm.com/Article/details/gxbecgjou.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.fehbvm.com/Article/details/gxhojxair.sHtML

[U05] Py：列表去重且保序
来源：http://3g.zdbjq.cn/Article/details/gspqrgssg.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/geubzpcgf.sHtML

[U06] Py：合并两个字典
来源：http://wap.zdbjq.cn/Article/details/gyvqvemuo.sHtML

{**a, **b}
来源：http://read.share.fehbvm.com/Article/details/gesxubqri.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.hesvh.cn/Article/details/gfyydabzx.sHtML

{v: k for k, v in d.items()}
来源：http://baike.zdbjq.cn/Article/details/gpbdisrpf.sHtML

[U08] Py：展平二维列表
来源：http://3g.fehbvm.com/Article/details/gspuwqgwt.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.hesvh.cn/Article/details/gasuwnqfq.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.hesvh.cn/Article/details/gmbonjafr.sHtML

max(d, key=d.get)
来源：http://m.share.fehbvm.com/Article/details/gbmbnrzpt.sHtML

[U10] Py：按值排序字典
来源：http://www.share.zdbjq.cn/Article/details/gktrmkjxk.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.fehbvm.com/Article/details/gfoqhojkr.sHtML

[U11] Py：生成器表达式
来源：http://m.share.fehbvm.com/Article/details/gklsctrnm.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.hesvh.cn/Article/details/glxchrruc.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.zdbjq.cn/Article/details/gxkmpwmwv.sHtML

Counter(arr).most_common(3)
来源：http://read.share.zdbjq.cn/Article/details/gqyhrrbqb.sHtML

[U13] Py：固定长度队列
来源：http://blog.zdbjq.cn/Article/details/goyzmyvpg.sHtML

deque(maxlen=10)
来源：http://m.share.hesvh.cn/Article/details/ghhuqlgzk.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.fehbvm.com/Article/details/gkjqyyrcg.sHtML

defaultdict(list)
来源：http://wap.fehbvm.com/Article/details/gsptjbsag.sHtML

[U15] Py：高精度计时
来源：http://m.share.hesvh.cn/Article/details/gqnbysins.sHtML

t = time.perf_counter()
来源：http://3g.fehbvm.com/Article/details/gmezcgynm.sHtML

[U16] Py：命令行参数解析
来源：http://wap.zdbjq.cn/Article/details/gvimyoxhw.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.fehbvm.com/Article/details/gngywhgmc.sHtML

[U17] Py：初始化日志
来源：http://read.share.zdbjq.cn/Article/details/gcwjeazpf.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.zdbjq.cn/Article/details/gzwhtejjy.sHtML

[U18] Py：预编译正则
来源：http://blog.fehbvm.com/Article/details/gxpsbmmwc.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.fehbvm.com/Article/details/glcswviad.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.fehbvm.com/Article/details/ginaspqjz.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.hesvh.cn/Article/details/gzihzzkrr.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.fehbvm.com/Article/details/gmsknthgb.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.fehbvm.com/Article/details/gkxqngncx.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.zdbjq.cn/Article/details/gseqotrrl.sHtML

@contextlib.contextmanager
来源：http://mobile.hesvh.cn/Article/details/gojigixnr.sHtML

[U22] Py：矩阵转置
来源：http://3g.hesvh.cn/Article/details/gnqqnorcu.sHtML

list(zip(*m))
来源：http://read.share.fehbvm.com/Article/details/gegllqpxd.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.hesvh.cn/Article/details/ghjishxgs.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.hesvh.cn/Article/details/gjabslnxx.sHtML

[U24] Py：路径操作
来源：http://read.share.zdbjq.cn/Article/details/gyigjnrfo.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.hesvh.cn/Article/details/gjwtgluwd.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.fehbvm.com/Article/details/ghwbokdyl.sHtML

csv.DictReader(f)
来源：http://mobile.zdbjq.cn/Article/details/gkkslmjih.sHtML

[U26] Py：并发下载
来源：http://3g.fehbvm.com/Article/details/gsprmlcdp.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.hesvh.cn/Article/details/gqqjqjmgm.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.fehbvm.com/Article/details/gsvdefhst.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.hesvh.cn/Article/details/gtwwzwkln.sHtML

[U28] Py：类型别名
来源：http://3g.fehbvm.com/Article/details/ghxfmocrs.sHtML

UserId = int
来源：http://mobile.hesvh.cn/Article/details/gchscaxhr.sHtML

[U29] Py：属性校验
来源：http://read.share.zdbjq.cn/Article/details/gxsigvzih.sHtML

@property 与 @x.setter 配合
来源：http://mobile.hesvh.cn/Article/details/gctykmndw.sHtML

[U30] Py：数据类
来源：http://www.share.hesvh.cn/Article/details/gcutvgenm.sHtML

@dataclass(slots=True)
来源：http://3g.hesvh.cn/Article/details/ghmjxhgya.sHtML

[U31] Py：单测
来源：http://m.share.zdbjq.cn/Article/details/gtmceqoqa.sHtML

python -m pytest -q
来源：http://3g.hesvh.cn/Article/details/godkuazui.sHtML

[U32] Py：代码格式化
来源：http://www.blog.zdbjq.cn/Article/details/gtxppzjwr.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.hesvh.cn/Article/details/gtkvyzpim.sHtML

[U33] Py：打包发布
来源：http://blog.zdbjq.cn/Article/details/gmoehlfxn.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.hesvh.cn/Article/details/gmphyrvjk.sHtML

[U34] Py：判断编码
来源：http://3g.fehbvm.com/Article/details/gaeukzdei.sHtML

chardet.detect(raw)
来源：http://blog.fehbvm.com/Article/details/gmpbwdfps.sHtML

[U35] Py：发送邮件
来源：http://m.share.zdbjq.cn/Article/details/gdiinxgzm.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.fehbvm.com/Article/details/gavnwptta.sHtML

[U36] Py：定时任务
来源：http://mobile.fehbvm.com/Article/details/glxfrjjlg.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.hesvh.cn/Article/details/gtmgjlpei.sHtML

[U37] Py：读写 Excel
来源：http://m.share.zdbjq.cn/Article/details/grbbuvlsz.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.hesvh.cn/Article/details/gtoemcekt.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.fehbvm.com/Article/details/gekjlpxmh.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.fehbvm.com/Article/details/gduztzanc.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.zdbjq.cn/Article/details/gbvbyicxt.sHtML

sys.stdout.isatty()
来源：http://mobile.fehbvm.com/Article/details/gjgnqvfoo.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.zdbjq.cn/Article/details/gvtwczmng.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.fehbvm.com/Article/details/gkxfyocee.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.zdbjq.cn/Article/details/gzffjjxgy.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.fehbvm.com/Article/details/gtxawjkuw.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.hesvh.cn/Article/details/gaufoudys.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.zdbjq.cn/Article/details/gyuohruqv.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.fehbvm.com/Article/details/gmcgzncny.sHtML

namespace App\Http;
来源：http://read.share.fehbvm.com/Article/details/gtrstvkyg.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.hesvh.cn/Article/details/gsscvmfrl.sHtML

declare(strict_types=1);
来源：http://www.share.zdbjq.cn/Article/details/gpxxttobn.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.fehbvm.com/Article/details/gyulcuafe.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gtswlvvej.sHtML

[U46] PHP：可空类型
来源：http://read.share.hesvh.cn/Article/details/gvmlritzy.sHtML

?string $name = null
来源：http://baike.hesvh.cn/Article/details/gelzskaxa.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.zdbjq.cn/Article/details/gwpwhcemo.sHtML

int|string $id
来源：http://mobile.zdbjq.cn/Article/details/gihdzxpgp.sHtML

[U48] PHP：纯枚举
来源：http://m.share.hesvh.cn/Article/details/gsqlxtkfp.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.hesvh.cn/Article/details/gkmmidiyf.sHtML

[U49] PHP：只读属性
来源：http://m.share.hesvh.cn/Article/details/ghcmhpoik.sHtML

public readonly string $name
来源：http://www.m.share.hesvh.cn/Article/details/gathpzqsx.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.fehbvm.com/Article/details/gftasvawu.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.hesvh.cn/Article/details/guwovickl.sHtML

[U51] PHP：数组解构
来源：http://blog.hesvh.cn/Article/details/gxfvblsyy.sHtML

[$a, $b] = $arr;
来源：http://www.blog.zdbjq.cn/Article/details/gwndwqwfp.sHtML

[U52] PHP：箭头函数
来源：http://mobile.zdbjq.cn/Article/details/gnpjjovjk.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.zdbjq.cn/Article/details/giqupzekp.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.zdbjq.cn/Article/details/gujebuifg.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.fehbvm.com/Article/details/gujmlomhj.sHtML

[U54] PHP：空安全调用
来源：http://read.share.hesvh.cn/Article/details/gboeinuxt.sHtML

$obj?->method()
来源：http://read.share.zdbjq.cn/Article/details/gghxezlxm.sHtML

[U55] PHP：match 表达式
来源：http://mobile.hesvh.cn/Article/details/gfirvmyfc.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.hesvh.cn/Article/details/gswwtmrlh.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.fehbvm.com/Article/details/gjitkvejw.sHtML

f(a: 1, b: 2)
来源：http://mobile.hesvh.cn/Article/details/gknzaqpto.sHtML

[U57] PHP：字符串插值
来源：http://wap.fehbvm.com/Article/details/gjnknephf.sHtML

"值: {$a}"
来源：http://baike.zdbjq.cn/Article/details/ggjxzajvk.sHtML

[U58] PHP：数组三件套
来源：http://mobile.zdbjq.cn/Article/details/gqaaadknp.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.fehbvm.com/Article/details/gvlnfwovu.sHtML

[U59] PHP：自定义排序
来源：http://mobile.zdbjq.cn/Article/details/gxgsfyqon.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.hesvh.cn/Article/details/geuiubhat.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.fehbvm.com/Article/details/gudebmugn.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.hesvh.cn/Article/details/gkwpgimhm.sHtML

[U61] PHP：正则
来源：http://www.m.share.zdbjq.cn/Article/details/gtusicpms.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fehbvm.com/Article/details/griibhirp.sHtML

[U62] PHP：日期对象
来源：http://3g.zdbjq.cn/Article/details/gisqmyazt.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.zdbjq.cn/Article/details/gfkzqerjg.sHtML

[U63] PHP：文件读写
来源：http://www.share.fehbvm.com/Article/details/guomqqfyf.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.hesvh.cn/Article/details/gfhhxqezm.sHtML

[U64] PHP：目录遍历
来源：http://baike.hesvh.cn/Article/details/gdwqaskxr.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.zdbjq.cn/Article/details/gcxmtykwb.sHtML

[U65] PHP：会话
来源：http://mobile.fehbvm.com/Article/details/gsergdcnz.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gbqonvrom.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.hesvh.cn/Article/details/gombhadnd.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.hesvh.cn/Article/details/gqxxholmf.sHtML

[U67] PHP：处理文件上传
来源：http://baike.hesvh.cn/Article/details/gljbhdexg.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.fehbvm.com/Article/details/gvonwiddf.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.hesvh.cn/Article/details/gzgkylpdn.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.hesvh.cn/Article/details/gythpkqtl.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.zdbjq.cn/Article/details/gvppnuenn.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.hesvh.cn/Article/details/gywxktzjm.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.fehbvm.com/Article/details/gzheqpzuf.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.zdbjq.cn/Article/details/gfdwlhvkz.sHtML

[U71] PHP：抛出异常
来源：http://baike.fehbvm.com/Article/details/govognmde.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.fehbvm.com/Article/details/gxpokbute.sHtML

[U72] PHP：写错误日志
来源：http://mobile.hesvh.cn/Article/details/gryisvhsv.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.zdbjq.cn/Article/details/gfbpszmdj.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.zdbjq.cn/Article/details/gomtfuzvh.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.fehbvm.com/Article/details/gjxjexujp.sHtML

[U74] PHP：读取环境变量
来源：http://baike.fehbvm.com/Article/details/grascadzd.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.hesvh.cn/Article/details/gmijatzio.sHtML

[U75] PHP：依赖注入
来源：http://read.share.hesvh.cn/Article/details/gpjkzhyom.sHtML

composer require psr/container
来源：http://baike.zdbjq.cn/Article/details/grwacqnux.sHtML

[U76] PHP：简单路由
来源：http://blog.zdbjq.cn/Article/details/goxpsetld.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.hesvh.cn/Article/details/gfmccwhgu.sHtML

[U77] PHP：模板渲染
来源：http://blog.zdbjq.cn/Article/details/gwgjzlrop.sHtML

composer require twig/twig
来源：http://blog.hesvh.cn/Article/details/gjaqjnakw.sHtML

[U78] PHP：单元测试
来源：http://3g.fehbvm.com/Article/details/gslqwrilo.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.hesvh.cn/Article/details/gnokflukl.sHtML

[U79] PHP：静态分析
来源：http://baike.hesvh.cn/Article/details/gepfxtvrp.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.hesvh.cn/Article/details/gthodkyqx.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.hesvh.cn/Article/details/gspiyfuvo.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.fehbvm.com/Article/details/gbezbsnil.sHtML

[U81] JS：初始化项目
来源：http://wap.hesvh.cn/Article/details/grhvggpfm.sHtML

npm init -y;  npm i express
来源：http://read.share.zdbjq.cn/Article/details/guxkbmdpj.sHtML

[U82] JS：package.json 脚本
来源：http://3g.hesvh.cn/Article/details/gwehtgixe.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.fehbvm.com/Article/details/gyxoffnre.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.zdbjq.cn/Article/details/gwziojkyj.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.hesvh.cn/Article/details/gfccdiqic.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.fehbvm.com/Article/details/gvvbrzuxg.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.fehbvm.com/Article/details/gadsdckaz.sHtML

[U85] JS：可选链
来源：http://read.share.hesvh.cn/Article/details/gdyvognuu.sHtML

a?.b?.c
来源：http://www.blog.zdbjq.cn/Article/details/gjoghyhwh.sHtML

[U86] JS：空值合并
来源：http://www.blog.fehbvm.com/Article/details/ghbgaykpy.sHtML

a ?? b
来源：http://read.share.hesvh.cn/Article/details/geutwthpu.sHtML

[U87] JS：解构默认值
来源：http://3g.hesvh.cn/Article/details/gbkroirbs.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.hesvh.cn/Article/details/geqhqfcvy.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.zdbjq.cn/Article/details/gyctpcwsz.sHtML

{ ...a, ...b }
来源：http://www.share.hesvh.cn/Article/details/gqqqhvbnz.sHtML

[U89] JS：数组去重
来源：http://mobile.zdbjq.cn/Article/details/gbckulgfm.sHtML

[...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/gawcdutmd.sHtML

[U90] JS：数字数组排序
来源：http://read.share.hesvh.cn/Article/details/gzabhhgiz.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gxzybfykj.sHtML

[U91] JS：对象键值遍历
来源：http://baike.hesvh.cn/Article/details/gphhgbedv.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.hesvh.cn/Article/details/gfkssikbk.sHtML

[U92] JS：深拷贝
来源：http://baike.fehbvm.com/Article/details/gggzblird.sHtML

structuredClone(obj)
来源：http://mobile.fehbvm.com/Article/details/gbucicokd.sHtML

[U93] JS：模板字符串
来源：http://www.blog.zdbjq.cn/Article/details/gzlkiauop.sHtML

`共 ${n} 条`
来源：http://read.share.fehbvm.com/Article/details/ghtboafzo.sHtML

[U94] JS：箭头函数
来源：http://www.blog.fehbvm.com/Article/details/gikjdsoqm.sHtML

const double = x => x * 2;
来源：http://mobile.zdbjq.cn/Article/details/gnbcmulyr.sHtML

[U95] JS：Promise 包装
来源：http://blog.fehbvm.com/Article/details/gwqalhoej.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.zdbjq.cn/Article/details/gzmahmhnc.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.fehbvm.com/Article/details/gghaddhhs.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gmhvbygwz.sHtML

[U97] JS：并发请求
来源：http://blog.hesvh.cn/Article/details/gqihcupfz.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/gewqohmph.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.fehbvm.com/Article/details/gzfrbnuul.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.zdbjq.cn/Article/details/gnszixyeh.sHtML

[U99] JS：事件监听
来源：http://baike.fehbvm.com/Article/details/gldvtkvpr.sHtML

el.addEventListener("click", e => {})
来源：http://3g.zdbjq.cn/Article/details/glizogdsb.sHtML

[U100] JS：DOM 查询
来源：http://mobile.hesvh.cn/Article/details/gfexfqkju.sHtML

document.querySelector(".item")
来源：http://blog.hesvh.cn/Article/details/gisyffrnd.sHtML

[U101] JS：classList 操作
来源：http://www.share.fehbvm.com/Article/details/gifjeytne.sHtML

el.classList.toggle("active")
来源：http://wap.hesvh.cn/Article/details/ghnjjwylf.sHtML

[U102] JS：本地存储
来源：http://read.share.zdbjq.cn/Article/details/gvpilfyzk.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.hesvh.cn/Article/details/gadtsaztt.sHtML

[U103] JS：定时器
来源：http://baike.zdbjq.cn/Article/details/gbnwdalcx.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.hesvh.cn/Article/details/gvtzyzxyl.sHtML

[U104] JS：防抖
来源：http://www.blog.hesvh.cn/Article/details/gkizvfwss.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gffpeoaxe.sHtML

[U105] JS：节流
来源：http://blog.fehbvm.com/Article/details/gniltocsm.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.zdbjq.cn/Article/details/gybbhwznv.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/ghftugzil.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.fehbvm.com/Article/details/gztifzvak.sHtML

[U107] JS：数字千分位
来源：http://m.share.hesvh.cn/Article/details/gnsvqarkg.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.zdbjq.cn/Article/details/gztzefpmh.sHtML

[U108] JS：随机整数
来源：http://m.share.fehbvm.com/Article/details/gvrfkdtwq.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.zdbjq.cn/Article/details/geapzdfdi.sHtML

[U109] JS：数组分组
来源：http://www.m.share.hesvh.cn/Article/details/glazcissw.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.fehbvm.com/Article/details/gpmttryeo.sHtML

[U110] JS：数组分块
来源：http://read.share.fehbvm.com/Article/details/gxjuknpoz.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.fehbvm.com/Article/details/gsdgkboog.sHtML

[U111] JS：对象转 Map
来源：http://blog.fehbvm.com/Article/details/gboxhcqur.sHtML

new Map(Object.entries(obj))
来源：http://read.share.zdbjq.cn/Article/details/guuerfmov.sHtML

[U112] JS：字符串补位
来源：http://mobile.fehbvm.com/Article/details/gkculgvbn.sHtML

"7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gvlpxizof.sHtML

[U113] JS：正则替换全部
来源：http://www.share.fehbvm.com/Article/details/gkogmawkk.sHtML

s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gieeesawl.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.fehbvm.com/Article/details/gchmvxitr.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.zdbjq.cn/Article/details/gkzpxmyrt.sHtML

[U115] JS：生成 UUID
来源：http://blog.fehbvm.com/Article/details/gderqqwtx.sHtML

crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gibetfngn.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.fehbvm.com/Article/details/gloabcoey.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.zdbjq.cn/Article/details/gjcexmvrx.sHtML

[U117] JS：单元测试
来源：http://read.share.hesvh.cn/Article/details/gkocbxflc.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.zdbjq.cn/Article/details/gxmspeqlp.sHtML

[U118] JS：开发服务器
来源：http://m.share.hesvh.cn/Article/details/guwefxyjz.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.zdbjq.cn/Article/details/gezqjaifv.sHtML

[U119] JS：生产构建
来源：http://mobile.zdbjq.cn/Article/details/gjyaxtagx.sHtML

npx vite build
来源：http://wap.fehbvm.com/Article/details/girjuosdv.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.fehbvm.com/Article/details/gfgwgytyw.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.fehbvm.com/Article/details/grzbenohp.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gcgavfwbe.sHtML

统计汇总
来源：http://baike.hesvh.cn/Article/details/gitmsztic.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gwviqpvbg.sHtML

按语言统计（条）：
来源：http://read.share.zdbjq.cn/Article/details/gwbklbbwb.sHtML

Python ......... 252
来源：http://www.blog.zdbjq.cn/Article/details/gbhtnqmpg.sHtML

PHP ............ 252
来源：http://3g.zdbjq.cn/Article/details/gyyebkhjd.sHtML

JavaScript ..... 252
来源：http://mobile.zdbjq.cn/Article/details/gwrydyyqe.sHtML

TypeScript ..... 212
来源：http://www.blog.zdbjq.cn/Article/details/gwvxmudwr.sHtML

Java ........... 212
来源：http://baike.fehbvm.com/Article/details/giayomnae.sHtML

Go ............. 212
来源：http://www.blog.hesvh.cn/Article/details/guavuvcpf.sHtML

Ruby ........... 212
来源：http://m.share.zdbjq.cn/Article/details/gvvyojtct.sHtML

C# ............. 212
来源：http://mobile.fehbvm.com/Article/details/gyqmfolhn.sHtML

C .............. 30
来源：http://m.share.hesvh.cn/Article/details/gsmuluefd.sHtML

C++ ............ 30
来源：http://blog.fehbvm.com/Article/details/gfzycjdmh.sHtML

SQL ............ 90
来源：http://www.m.share.fehbvm.com/Article/details/guclxnkem.sHtML

Bash ........... 80
来源：http://3g.zdbjq.cn/Article/details/ggnuohslx.sHtML

Kotlin ......... 15
来源：http://www.share.hesvh.cn/Article/details/gtbyrvygi.sHtML

Swift .......... 15
来源：http://mobile.zdbjq.cn/Article/details/guxzaxiju.sHtML

Lua ............ 10
来源：http://www.m.share.zdbjq.cn/Article/details/gxwpidalo.sHtML

Perl ........... 10
来源：http://read.share.fehbvm.com/Article/details/grdmebkff.sHtML

Scala .......... 10
来源：http://m.share.hesvh.cn/Article/details/gjmyrkpog.sHtML

------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gokpfszfa.sHtML

合计 ........... 2106 条
来源：http://wap.zdbjq.cn/Article/details/gxovvpbtq.sHtML

按章节统计：
来源：http://blog.fehbvm.com/Article/details/gwblcevpc.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.zdbjq.cn/Article/details/gekaxwgnl.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.hesvh.cn/Article/details/ghmuiowoz.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/gbtxodtlu.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.fehbvm.com/Article/details/gprjvhnbj.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.hesvh.cn/Article/details/gzptbkbda.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.hesvh.cn/Article/details/gfxyzbbdg.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.hesvh.cn/Article/details/gcdyjmmnq.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.zdbjq.cn/Article/details/gkkvuxgzp.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gwcsyibnf.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.hesvh.cn/Article/details/gndlugkva.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gqzbzvkar.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gmkepewga.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gzmleoyrn.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.hesvh.cn/Article/details/gpckrpyws.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.zdbjq.cn/Article/details/gkrxicscw.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/ghuqekxxc.sHtML

Q SQL 专题                              90
来源：http://m.share.fehbvm.com/Article/details/geqxjeccw.sHtML

R Bash 专题                             80
来源：http://www.m.share.zdbjq.cn/Article/details/gojubfjts.sHtML

S C / C++ 专题                          60
来源：http://blog.zdbjq.cn/Article/details/glgqodjmt.sHtML

T 其他语言补充                          60
来源：http://www.blog.fehbvm.com/Article/details/gkkbhqmga.sHtML

U 高频实用片段                         120
来源：http://blog.zdbjq.cn/Article/details/gxzrusrxx.sHtML

------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/ghinkdaqu.sHtML

合计                                  2106 条
来源：http://www.blog.fehbvm.com/Article/details/gvcfpkemz.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gvxapjlix.sHtML


<!-- 参考信息 -->