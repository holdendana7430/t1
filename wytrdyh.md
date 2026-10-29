代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.zdbjq.cn/Article/details/ghdkzbtaq.sHtML

[T59] Scala：循环
来源：http://read.share.zdbjq.cn/Article/details/gbmcrogfm.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.zdbjq.cn/Article/details/gsficbdjy.sHtML

[T60] Scala：折叠
来源：http://mobile.fehbvm.com/Article/details/grtaxrhzp.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.zdbjq.cn/Article/details/grefmtqkx.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gpwophotz.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.hesvh.cn/Article/details/gexjjvrpm.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/guynqcvyn.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.hesvh.cn/Article/details/gdyeyotel.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.fehbvm.com/Article/details/giedsctss.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.zdbjq.cn/Article/details/gaxcgpbfi.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.hesvh.cn/Article/details/garzemcrx.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.fehbvm.com/Article/details/guzmolngp.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.hesvh.cn/Article/details/gsenkovbc.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.hesvh.cn/Article/details/gutkavyix.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fehbvm.com/Article/details/gawnxthea.sHtML

[U05] Py：列表去重且保序
来源：http://3g.zdbjq.cn/Article/details/gzpltulcv.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.hesvh.cn/Article/details/gldomfkcp.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fehbvm.com/Article/details/gtdkuangk.sHtML

{**a, **b}
来源：http://read.share.zdbjq.cn/Article/details/gtqhuuxly.sHtML

[U07] Py：反转字典键值
来源：http://read.share.zdbjq.cn/Article/details/gpazyjwlz.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.fehbvm.com/Article/details/gpbzfdfbt.sHtML

[U08] Py：展平二维列表
来源：http://wap.zdbjq.cn/Article/details/glfrnjtnu.sHtML

[y for x in nested for y in x]
来源：http://mobile.hesvh.cn/Article/details/gehoezxbi.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.hesvh.cn/Article/details/gupyhhlrj.sHtML

max(d, key=d.get)
来源：http://baike.fehbvm.com/Article/details/gvgdeuccz.sHtML

[U10] Py：按值排序字典
来源：http://baike.fehbvm.com/Article/details/gpllokuxr.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.zdbjq.cn/Article/details/gespibght.sHtML

[U11] Py：生成器表达式
来源：http://www.share.hesvh.cn/Article/details/glxpijlcp.sHtML

(x * 2 for x in arr)
来源：http://read.share.hesvh.cn/Article/details/gyytsadmx.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.hesvh.cn/Article/details/gvatqqqfo.sHtML

Counter(arr).most_common(3)
来源：http://read.share.fehbvm.com/Article/details/glzjpgnxm.sHtML

[U13] Py：固定长度队列
来源：http://baike.hesvh.cn/Article/details/gofgzmiyw.sHtML

deque(maxlen=10)
来源：http://www.m.share.hesvh.cn/Article/details/gafrxrczs.sHtML

[U14] Py：分组收集到列表
来源：http://wap.zdbjq.cn/Article/details/gpjkgzzvi.sHtML

defaultdict(list)
来源：http://read.share.hesvh.cn/Article/details/gxtlmgahy.sHtML

[U15] Py：高精度计时
来源：http://www.share.zdbjq.cn/Article/details/gzozvhovy.sHtML

t = time.perf_counter()
来源：http://blog.hesvh.cn/Article/details/gpbmjdwjf.sHtML

[U16] Py：命令行参数解析
来源：http://blog.fehbvm.com/Article/details/glwlivozg.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.fehbvm.com/Article/details/gwugxrxwj.sHtML

[U17] Py：初始化日志
来源：http://blog.zdbjq.cn/Article/details/gxpvsybin.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.zdbjq.cn/Article/details/gqxmjuysp.sHtML

[U18] Py：预编译正则
来源：http://wap.hesvh.cn/Article/details/ggmqwaisv.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.zdbjq.cn/Article/details/gkxjfxpwr.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.zdbjq.cn/Article/details/gckyijivc.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.fehbvm.com/Article/details/gtgtsitmb.sHtML

[U20] Py：缓存函数结果
来源：http://baike.hesvh.cn/Article/details/gpcvectov.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.hesvh.cn/Article/details/guoawjqhw.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.hesvh.cn/Article/details/ghqdvflou.sHtML

@contextlib.contextmanager
来源：http://www.blog.fehbvm.com/Article/details/glsmmxjyi.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.zdbjq.cn/Article/details/gdxfhunet.sHtML

list(zip(*m))
来源：http://read.share.zdbjq.cn/Article/details/ghudjkjxn.sHtML

[U23] Py：分块读取大文件
来源：http://wap.hesvh.cn/Article/details/gwunjdbpj.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.fehbvm.com/Article/details/ghjekjjfa.sHtML

[U24] Py：路径操作
来源：http://blog.fehbvm.com/Article/details/gcacihaop.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.hesvh.cn/Article/details/gmnkzeayv.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.zdbjq.cn/Article/details/glnzregvg.sHtML

csv.DictReader(f)
来源：http://baike.hesvh.cn/Article/details/gyefvipfc.sHtML

[U26] Py：并发下载
来源：http://3g.zdbjq.cn/Article/details/gxslfcmyv.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.zdbjq.cn/Article/details/gfetsxcbe.sHtML

[U27] Py：异步 HTTP
来源：http://3g.hesvh.cn/Article/details/glydqzfvt.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.hesvh.cn/Article/details/gdevbxqle.sHtML

[U28] Py：类型别名
来源：http://wap.hesvh.cn/Article/details/gfhdonjwo.sHtML

UserId = int
来源：http://wap.hesvh.cn/Article/details/gqwkasqlt.sHtML

[U29] Py：属性校验
来源：http://www.share.zdbjq.cn/Article/details/gddfsepok.sHtML

@property 与 @x.setter 配合
来源：http://mobile.fehbvm.com/Article/details/gksqryvsv.sHtML

[U30] Py：数据类
来源：http://mobile.hesvh.cn/Article/details/gjovgmbsn.sHtML

@dataclass(slots=True)
来源：http://read.share.hesvh.cn/Article/details/gbsxsuocx.sHtML

[U31] Py：单测
来源：http://mobile.zdbjq.cn/Article/details/gppsfawuc.sHtML

python -m pytest -q
来源：http://blog.hesvh.cn/Article/details/ghazudmde.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.fehbvm.com/Article/details/ghbwjdupq.sHtML

ruff format . && ruff check --fix .
来源：http://blog.hesvh.cn/Article/details/gvuwsnufr.sHtML

[U33] Py：打包发布
来源：http://read.share.zdbjq.cn/Article/details/gghsfwnvd.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.fehbvm.com/Article/details/gjspsdiye.sHtML

[U34] Py：判断编码
来源：http://wap.fehbvm.com/Article/details/gmpkgslse.sHtML

chardet.detect(raw)
来源：http://www.blog.fehbvm.com/Article/details/gkhsmoowq.sHtML

[U35] Py：发送邮件
来源：http://mobile.zdbjq.cn/Article/details/gycnfjqqw.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.fehbvm.com/Article/details/gkducyqgz.sHtML

[U36] Py：定时任务
来源：http://read.share.hesvh.cn/Article/details/gqljlwxjj.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.hesvh.cn/Article/details/gpfmlggjv.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.fehbvm.com/Article/details/gkedbacfp.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.fehbvm.com/Article/details/goqbdmsbu.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fehbvm.com/Article/details/gipfbhfdx.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.zdbjq.cn/Article/details/grqrvktsi.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.fehbvm.com/Article/details/gojhkqrac.sHtML

sys.stdout.isatty()
来源：http://m.share.fehbvm.com/Article/details/gdlovbeng.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.hesvh.cn/Article/details/gngwykkuk.sHtML

print("err", file=sys.stderr)
来源：http://m.share.zdbjq.cn/Article/details/gzffmdknv.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.zdbjq.cn/Article/details/gzafksovx.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.hesvh.cn/Article/details/gndkgwgal.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.fehbvm.com/Article/details/gyqzcelfx.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.fehbvm.com/Article/details/gtfmylgvk.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.zdbjq.cn/Article/details/gwdhpabrr.sHtML

namespace App\Http;
来源：http://3g.zdbjq.cn/Article/details/gsebplvim.sHtML

[U44] PHP：开启严格类型
来源：http://baike.fehbvm.com/Article/details/gylbgtjbp.sHtML

declare(strict_types=1);
来源：http://blog.hesvh.cn/Article/details/gturknudy.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.hesvh.cn/Article/details/gbdjeoijg.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gqnvqlzrk.sHtML

[U46] PHP：可空类型
来源：http://www.blog.fehbvm.com/Article/details/gdevccvnr.sHtML

?string $name = null
来源：http://baike.fehbvm.com/Article/details/gmixsubby.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.zdbjq.cn/Article/details/gaqdpqapl.sHtML

int|string $id
来源：http://mobile.zdbjq.cn/Article/details/gjrlwkktp.sHtML

[U48] PHP：纯枚举
来源：http://3g.fehbvm.com/Article/details/grxxefxki.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.fehbvm.com/Article/details/gnoktaimp.sHtML

[U49] PHP：只读属性
来源：http://www.share.hesvh.cn/Article/details/gmyhavlln.sHtML

public readonly string $name
来源：http://baike.zdbjq.cn/Article/details/gwgfgrahl.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.fehbvm.com/Article/details/grwnwcxhi.sHtML

public function __construct(private int $id) {}
来源：http://read.share.hesvh.cn/Article/details/gwfipmamd.sHtML

[U51] PHP：数组解构
来源：http://3g.fehbvm.com/Article/details/ggrwqhoog.sHtML

[$a, $b] = $arr;
来源：http://wap.hesvh.cn/Article/details/ghgzqxnuu.sHtML

[U52] PHP：箭头函数
来源：http://read.share.fehbvm.com/Article/details/gkjivncjq.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.zdbjq.cn/Article/details/gbsmasjkd.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.zdbjq.cn/Article/details/ggnpsxzyi.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.zdbjq.cn/Article/details/gpjcsxghq.sHtML

[U54] PHP：空安全调用
来源：http://wap.hesvh.cn/Article/details/ghrrdmqrn.sHtML

$obj?->method()
来源：http://3g.fehbvm.com/Article/details/gmiiqxgil.sHtML

[U55] PHP：match 表达式
来源：http://read.share.zdbjq.cn/Article/details/gzcwvplui.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.zdbjq.cn/Article/details/gvcyfvxyh.sHtML

[U56] PHP：命名参数
来源：http://read.share.hesvh.cn/Article/details/gpzxchdef.sHtML

f(a: 1, b: 2)
来源：http://mobile.hesvh.cn/Article/details/gsnmqrmtm.sHtML

[U57] PHP：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gksgonjtp.sHtML

"值: {$a}"
来源：http://blog.zdbjq.cn/Article/details/ggfjravhn.sHtML

[U58] PHP：数组三件套
来源：http://www.share.zdbjq.cn/Article/details/gmkcdfqqh.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.fehbvm.com/Article/details/gueqngbrg.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.fehbvm.com/Article/details/gwufvjhih.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.zdbjq.cn/Article/details/gwenydtkj.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.fehbvm.com/Article/details/gczttiidq.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.zdbjq.cn/Article/details/gshrcfqmz.sHtML

[U61] PHP：正则
来源：http://read.share.hesvh.cn/Article/details/goazsmfdy.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.hesvh.cn/Article/details/gflxejkby.sHtML

[U62] PHP：日期对象
来源：http://m.share.hesvh.cn/Article/details/gyoeoeokg.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.hesvh.cn/Article/details/gpxiftyuz.sHtML

[U63] PHP：文件读写
来源：http://m.share.fehbvm.com/Article/details/grswndrdw.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.fehbvm.com/Article/details/gkgxhwkua.sHtML

[U64] PHP：目录遍历
来源：http://read.share.fehbvm.com/Article/details/gnrtvgkew.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.hesvh.cn/Article/details/gdbpzabss.sHtML

[U65] PHP：会话
来源：http://blog.hesvh.cn/Article/details/ghlvgbynb.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gheutkkeh.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.zdbjq.cn/Article/details/gjzmojdww.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.fehbvm.com/Article/details/gtmhbjbpw.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.zdbjq.cn/Article/details/gnqwcvmyb.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.hesvh.cn/Article/details/gpkhbuzpx.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.fehbvm.com/Article/details/glkekubas.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.fehbvm.com/Article/details/gkutraljn.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.hesvh.cn/Article/details/gzxashvkk.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.zdbjq.cn/Article/details/gtfvnvlls.sHtML

[U70] PHP：PDO 事务
来源：http://blog.fehbvm.com/Article/details/gpnqztcdx.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.fehbvm.com/Article/details/gveolqsqj.sHtML

[U71] PHP：抛出异常
来源：http://blog.hesvh.cn/Article/details/gctaxdzok.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.fehbvm.com/Article/details/ggogvqfkc.sHtML

[U72] PHP：写错误日志
来源：http://wap.hesvh.cn/Article/details/grxxfrysx.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.zdbjq.cn/Article/details/gohiiypgz.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.hesvh.cn/Article/details/gzvpbbyrp.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.hesvh.cn/Article/details/gjurweozl.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.zdbjq.cn/Article/details/gkkfzdakw.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.hesvh.cn/Article/details/gyltnljmj.sHtML

[U75] PHP：依赖注入
来源：http://blog.fehbvm.com/Article/details/gqjvpiysl.sHtML

composer require psr/container
来源：http://www.share.zdbjq.cn/Article/details/gtcvmludm.sHtML

[U76] PHP：简单路由
来源：http://mobile.fehbvm.com/Article/details/goypckfcy.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.zdbjq.cn/Article/details/grsbatkjr.sHtML

[U77] PHP：模板渲染
来源：http://mobile.zdbjq.cn/Article/details/gpgszosby.sHtML

composer require twig/twig
来源：http://www.share.hesvh.cn/Article/details/gdnutddew.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.hesvh.cn/Article/details/gzjetnjgd.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.fehbvm.com/Article/details/gdknpkvlw.sHtML

[U79] PHP：静态分析
来源：http://read.share.zdbjq.cn/Article/details/glorzxqdn.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.hesvh.cn/Article/details/gmpllgpho.sHtML

[U80] PHP：代码规范修复
来源：http://blog.zdbjq.cn/Article/details/gqqtkhohx.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.zdbjq.cn/Article/details/gvwqjiddt.sHtML

[U81] JS：初始化项目
来源：http://blog.zdbjq.cn/Article/details/gboyldelv.sHtML

npm init -y;  npm i express
来源：http://www.blog.fehbvm.com/Article/details/grhhujghy.sHtML

[U82] JS：package.json 脚本
来源：http://wap.zdbjq.cn/Article/details/gshdzuxxb.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.hesvh.cn/Article/details/gwkqgjkgq.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.hesvh.cn/Article/details/goxifcyzz.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.hesvh.cn/Article/details/gqyepfafr.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.hesvh.cn/Article/details/gayurqcgg.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.hesvh.cn/Article/details/gmcgshbwq.sHtML

[U85] JS：可选链
来源：http://wap.zdbjq.cn/Article/details/gyepprzgv.sHtML

a?.b?.c
来源：http://www.share.fehbvm.com/Article/details/gclwqmuhq.sHtML

[U86] JS：空值合并
来源：http://m.share.zdbjq.cn/Article/details/gcdsrrbyj.sHtML

a ?? b
来源：http://read.share.zdbjq.cn/Article/details/gbsjexhsi.sHtML

[U87] JS：解构默认值
来源：http://blog.fehbvm.com/Article/details/gyenzmmtc.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.fehbvm.com/Article/details/gcbtnvmbb.sHtML

[U88] JS：对象展开合并
来源：http://m.share.hesvh.cn/Article/details/gchcuvovr.sHtML

{ ...a, ...b }
来源：http://wap.zdbjq.cn/Article/details/gnksxuuow.sHtML

[U89] JS：数组去重
来源：http://m.share.zdbjq.cn/Article/details/grsvzjeis.sHtML

[...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gdzoefvvb.sHtML

[U90] JS：数字数组排序
来源：http://wap.zdbjq.cn/Article/details/ggvtuekru.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/geuxgclft.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.fehbvm.com/Article/details/gihoxlcob.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.fehbvm.com/Article/details/gldchbgus.sHtML

[U92] JS：深拷贝
来源：http://wap.fehbvm.com/Article/details/gxtolahvb.sHtML

structuredClone(obj)
来源：http://mobile.fehbvm.com/Article/details/gaifnlmdg.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.hesvh.cn/Article/details/glvdpybdk.sHtML

`共 ${n} 条`
来源：http://3g.hesvh.cn/Article/details/gifxgrgqk.sHtML

[U94] JS：箭头函数
来源：http://baike.hesvh.cn/Article/details/gftdwzouz.sHtML

const double = x => x * 2;
来源：http://baike.zdbjq.cn/Article/details/gpgafcibf.sHtML

[U95] JS：Promise 包装
来源：http://baike.fehbvm.com/Article/details/gyjjeaqcu.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.fehbvm.com/Article/details/gfcnxjiub.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.fehbvm.com/Article/details/gpotwsjik.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/ghnhrfktl.sHtML

[U97] JS：并发请求
来源：http://read.share.zdbjq.cn/Article/details/gfoojrgix.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/gzvahtswz.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.hesvh.cn/Article/details/gpommtdcm.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.fehbvm.com/Article/details/ghqvsaekk.sHtML

[U99] JS：事件监听
来源：http://www.blog.hesvh.cn/Article/details/gmdsuvhts.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.hesvh.cn/Article/details/gsfzuxquq.sHtML

[U100] JS：DOM 查询
来源：http://m.share.zdbjq.cn/Article/details/gpiyillhj.sHtML

document.querySelector(".item")
来源：http://www.blog.zdbjq.cn/Article/details/glfxevecp.sHtML

[U101] JS：classList 操作
来源：http://www.share.zdbjq.cn/Article/details/gnrvjlvlf.sHtML

el.classList.toggle("active")
来源：http://m.share.fehbvm.com/Article/details/gdbwhhvdz.sHtML

[U102] JS：本地存储
来源：http://blog.zdbjq.cn/Article/details/guvvwamuy.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.zdbjq.cn/Article/details/gwnmysvds.sHtML

[U103] JS：定时器
来源：http://wap.zdbjq.cn/Article/details/gwbcnekik.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.fehbvm.com/Article/details/gvbhaqkgl.sHtML

[U104] JS：防抖
来源：http://www.blog.zdbjq.cn/Article/details/glrjfzcho.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gvrsyysza.sHtML

[U105] JS：节流
来源：http://mobile.fehbvm.com/Article/details/gklfojjpj.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.hesvh.cn/Article/details/gtjqnabsa.sHtML

[U106] JS：日期格式化
来源：http://m.share.fehbvm.com/Article/details/gtpuezwak.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.hesvh.cn/Article/details/gpkuojkek.sHtML

[U107] JS：数字千分位
来源：http://baike.fehbvm.com/Article/details/guqhrnzwo.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.zdbjq.cn/Article/details/gaqdrnnca.sHtML

[U108] JS：随机整数
来源：http://wap.hesvh.cn/Article/details/gwvepuyxb.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.zdbjq.cn/Article/details/ggvsdyzmq.sHtML

[U109] JS：数组分组
来源：http://blog.fehbvm.com/Article/details/gcatjhpyq.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.zdbjq.cn/Article/details/ghipfaggx.sHtML

[U110] JS：数组分块
来源：http://baike.fehbvm.com/Article/details/gijfyzfse.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.zdbjq.cn/Article/details/gcfkmooyh.sHtML

[U111] JS：对象转 Map
来源：http://blog.fehbvm.com/Article/details/galuwbyze.sHtML

new Map(Object.entries(obj))
来源：http://read.share.zdbjq.cn/Article/details/gmyghqaia.sHtML

[U112] JS：字符串补位
来源：http://mobile.hesvh.cn/Article/details/gjwyktyhb.sHtML

"7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/ghoiorapu.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.hesvh.cn/Article/details/gosbnslrj.sHtML

s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gddoibbul.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.fehbvm.com/Article/details/gajecblyz.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fehbvm.com/Article/details/gsffhapfv.sHtML

[U115] JS：生成 UUID
来源：http://blog.zdbjq.cn/Article/details/gzfkdagjx.sHtML

crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/gswxceiwf.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.zdbjq.cn/Article/details/gktrvgkpo.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.hesvh.cn/Article/details/gclerrvcv.sHtML

[U117] JS：单元测试
来源：http://www.m.share.fehbvm.com/Article/details/gqxasgzqj.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.zdbjq.cn/Article/details/gjpjsvkth.sHtML

[U118] JS：开发服务器
来源：http://read.share.zdbjq.cn/Article/details/gruwvvhqf.sHtML

npm i -D vite;  npx vite
来源：http://baike.hesvh.cn/Article/details/gqgooqtfv.sHtML

[U119] JS：生产构建
来源：http://read.share.hesvh.cn/Article/details/goxfqiadj.sHtML

npx vite build
来源：http://3g.fehbvm.com/Article/details/gphkoosmi.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.fehbvm.com/Article/details/ghrtwewzz.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.hesvh.cn/Article/details/gokcpbdlw.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ghngfxnez.sHtML

统计汇总
来源：http://blog.fehbvm.com/Article/details/gpvjmygbv.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gekhxyhoa.sHtML

按语言统计（条）：
来源：http://www.share.fehbvm.com/Article/details/gwhjhqhez.sHtML

Python ......... 252
来源：http://www.m.share.fehbvm.com/Article/details/gzsffjoir.sHtML

PHP ............ 252
来源：http://3g.hesvh.cn/Article/details/gexshhilz.sHtML

JavaScript ..... 252
来源：http://www.share.hesvh.cn/Article/details/gytfzatsa.sHtML

TypeScript ..... 212
来源：http://read.share.fehbvm.com/Article/details/gwrdnxtwl.sHtML

Java ........... 212
来源：http://www.blog.hesvh.cn/Article/details/gmexokmgr.sHtML

Go ............. 212
来源：http://www.m.share.hesvh.cn/Article/details/gquqtzstd.sHtML

Ruby ........... 212
来源：http://www.m.share.hesvh.cn/Article/details/gchjttgri.sHtML

C# ............. 212
来源：http://read.share.fehbvm.com/Article/details/gvmxsjrsh.sHtML

C .............. 30
来源：http://www.share.fehbvm.com/Article/details/gorehrvwg.sHtML

C++ ............ 30
来源：http://read.share.fehbvm.com/Article/details/gnstlcylx.sHtML

SQL ............ 90
来源：http://www.share.zdbjq.cn/Article/details/gadltdzly.sHtML

Bash ........... 80
来源：http://3g.zdbjq.cn/Article/details/gxspzcjod.sHtML

Kotlin ......... 15
来源：http://mobile.zdbjq.cn/Article/details/gcotnikzf.sHtML

Swift .......... 15
来源：http://m.share.fehbvm.com/Article/details/gwobvppal.sHtML

Lua ............ 10
来源：http://baike.zdbjq.cn/Article/details/gbhjplduj.sHtML

Perl ........... 10
来源：http://3g.zdbjq.cn/Article/details/gtsruvhyi.sHtML

Scala .......... 10
来源：http://3g.zdbjq.cn/Article/details/grqgbakqv.sHtML

------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gylaxkxct.sHtML

合计 ........... 2106 条
来源：http://www.share.fehbvm.com/Article/details/gqstjaulb.sHtML

按章节统计：
来源：http://www.share.zdbjq.cn/Article/details/guovgepli.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.hesvh.cn/Article/details/gzebaslvq.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/gyhdmbvet.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/gtcqgtoen.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.fehbvm.com/Article/details/ghuiwcnnk.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.hesvh.cn/Article/details/gicktsqmu.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.hesvh.cn/Article/details/gqgbiiyzo.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.fehbvm.com/Article/details/gglvbbgbj.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.hesvh.cn/Article/details/ggyuwptug.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gkxfltxym.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.hesvh.cn/Article/details/gvtsiejpj.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/guazwxchi.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gmybgfltn.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gycluteuu.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.hesvh.cn/Article/details/gsbclvfgy.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.fehbvm.com/Article/details/gqpafvtwj.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gmurtcbem.sHtML

Q SQL 专题                              90
来源：http://baike.hesvh.cn/Article/details/gvocatqxg.sHtML

R Bash 专题                             80
来源：http://read.share.fehbvm.com/Article/details/gpjfqyxoz.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.fehbvm.com/Article/details/gfgbcykxj.sHtML

T 其他语言补充                          60
来源：http://wap.hesvh.cn/Article/details/giulwlrbh.sHtML

U 高频实用片段                         120
来源：http://baike.fehbvm.com/Article/details/gofwxtlja.sHtML

------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gtncxalvn.sHtML

合计                                  2106 条
来源：http://m.share.zdbjq.cn/Article/details/gskzcollz.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gzjcsgvnk.sHtML

使用提醒
来源：http://www.blog.fehbvm.com/Article/details/gmjkkyrwg.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gebvappwg.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.fehbvm.com/Article/details/gmbxlwsqr.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.fehbvm.com/Article/details/gtiqdyqif.sHtML


<!-- 参考信息 -->