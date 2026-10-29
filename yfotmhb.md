代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://www.share.hesvh.cn/Article/details/guljskgzo.sHtML

[T55] Scala：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/gzrxwpjer.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.zdbjq.cn/Article/details/gjfobcmjr.sHtML

[T56] Scala：样例类
来源：http://mobile.zdbjq.cn/Article/details/gwvjpbpja.sHtML

case class User(name: String, age: Int)
来源：http://baike.fehbvm.com/Article/details/gbkyjtrid.sHtML

[T57] Scala：模式匹配
来源：http://m.share.fehbvm.com/Article/details/gejbocvxi.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.fehbvm.com/Article/details/gfjwrxbco.sHtML

[T58] Scala：函数定义
来源：http://m.share.hesvh.cn/Article/details/gxfrvvvly.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.zdbjq.cn/Article/details/gllhhgngx.sHtML

[T59] Scala：循环
来源：http://mobile.hesvh.cn/Article/details/gucnbikdc.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.hesvh.cn/Article/details/glctjkxlu.sHtML

[T60] Scala：折叠
来源：http://blog.fehbvm.com/Article/details/gqfiqhdkp.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.fehbvm.com/Article/details/goeeeayus.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gihsueaqb.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.hesvh.cn/Article/details/guyaljoxa.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gvlsmfoyd.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.zdbjq.cn/Article/details/gqqxcvxro.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.zdbjq.cn/Article/details/gnbmyptuo.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.zdbjq.cn/Article/details/glnchswmv.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.hesvh.cn/Article/details/gdxmvjcla.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.hesvh.cn/Article/details/glpyfqtoe.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.fehbvm.com/Article/details/gbojfmenw.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.zdbjq.cn/Article/details/gxsaxwynz.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.fehbvm.com/Article/details/gzfduaqnm.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.zdbjq.cn/Article/details/gxxirpdba.sHtML

list(dict.fromkeys(arr))
来源：http://wap.hesvh.cn/Article/details/gyknkqypm.sHtML

[U06] Py：合并两个字典
来源：http://mobile.hesvh.cn/Article/details/gvdwheqwl.sHtML

{**a, **b}
来源：http://read.share.hesvh.cn/Article/details/gvkdwbojg.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.fehbvm.com/Article/details/gdphfvuan.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.hesvh.cn/Article/details/gkjjluymc.sHtML

[U08] Py：展平二维列表
来源：http://3g.hesvh.cn/Article/details/gdschhzdk.sHtML

[y for x in nested for y in x]
来源：http://mobile.hesvh.cn/Article/details/gisliyafk.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.zdbjq.cn/Article/details/gmnmqrapx.sHtML

max(d, key=d.get)
来源：http://3g.fehbvm.com/Article/details/gzajopmmp.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.zdbjq.cn/Article/details/gnlnkyywr.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.zdbjq.cn/Article/details/gvgkqklpw.sHtML

[U11] Py：生成器表达式
来源：http://mobile.hesvh.cn/Article/details/gvfcfrdru.sHtML

(x * 2 for x in arr)
来源：http://baike.fehbvm.com/Article/details/gctxnoicu.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.hesvh.cn/Article/details/gggnjiekj.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gavuuphif.sHtML

[U13] Py：固定长度队列
来源：http://read.share.fehbvm.com/Article/details/gcpoqdfoh.sHtML

deque(maxlen=10)
来源：http://baike.hesvh.cn/Article/details/gooohvnjv.sHtML

[U14] Py：分组收集到列表
来源：http://wap.fehbvm.com/Article/details/gkryxydsp.sHtML

defaultdict(list)
来源：http://baike.fehbvm.com/Article/details/gcmvpawot.sHtML

[U15] Py：高精度计时
来源：http://wap.zdbjq.cn/Article/details/gzwfzuhme.sHtML

t = time.perf_counter()
来源：http://www.share.zdbjq.cn/Article/details/gsydwcgjg.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.hesvh.cn/Article/details/gxaafrvsi.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.hesvh.cn/Article/details/gbzzwtvze.sHtML

[U17] Py：初始化日志
来源：http://baike.hesvh.cn/Article/details/gtboqlwfz.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fehbvm.com/Article/details/gqzwctvwv.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fehbvm.com/Article/details/gwwmaajza.sHtML

pat = re.compile(r"\d+")
来源：http://wap.fehbvm.com/Article/details/gshhnezak.sHtML

[U19] Py：正则替换带回调
来源：http://baike.zdbjq.cn/Article/details/gcnkpmxzd.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.zdbjq.cn/Article/details/ghggldibu.sHtML

[U20] Py：缓存函数结果
来源：http://baike.zdbjq.cn/Article/details/gpnbuektj.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.fehbvm.com/Article/details/gykkqikty.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.fehbvm.com/Article/details/gegzrjobm.sHtML

@contextlib.contextmanager
来源：http://www.m.share.hesvh.cn/Article/details/gniuoeoyt.sHtML

[U22] Py：矩阵转置
来源：http://baike.zdbjq.cn/Article/details/gnknyqbzx.sHtML

list(zip(*m))
来源：http://read.share.fehbvm.com/Article/details/gfmganxhx.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.hesvh.cn/Article/details/gvmqsdsrq.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.fehbvm.com/Article/details/gpdtrwvru.sHtML

[U24] Py：路径操作
来源：http://m.share.hesvh.cn/Article/details/gzwsnkbqf.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.fehbvm.com/Article/details/gqubzmaob.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.hesvh.cn/Article/details/gfkpkhkvi.sHtML

csv.DictReader(f)
来源：http://read.share.fehbvm.com/Article/details/gwklcqxzc.sHtML

[U26] Py：并发下载
来源：http://m.share.hesvh.cn/Article/details/getwzxadd.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.zdbjq.cn/Article/details/ginnyrlak.sHtML

[U27] Py：异步 HTTP
来源：http://wap.hesvh.cn/Article/details/gplhofxaa.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.zdbjq.cn/Article/details/gjasujcwf.sHtML

[U28] Py：类型别名
来源：http://www.m.share.zdbjq.cn/Article/details/gjnkcnejf.sHtML

UserId = int
来源：http://read.share.zdbjq.cn/Article/details/gqlziyyqk.sHtML

[U29] Py：属性校验
来源：http://wap.zdbjq.cn/Article/details/gehsmisys.sHtML

@property 与 @x.setter 配合
来源：http://3g.zdbjq.cn/Article/details/gasgnisgo.sHtML

[U30] Py：数据类
来源：http://www.m.share.hesvh.cn/Article/details/gtktpwkte.sHtML

@dataclass(slots=True)
来源：http://baike.hesvh.cn/Article/details/gakrpwxkp.sHtML

[U31] Py：单测
来源：http://www.share.zdbjq.cn/Article/details/gdqesurgc.sHtML

python -m pytest -q
来源：http://baike.zdbjq.cn/Article/details/gspuwgekh.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gfwyzjkfj.sHtML

ruff format . && ruff check --fix .
来源：http://baike.zdbjq.cn/Article/details/gfnuzgvxf.sHtML

[U33] Py：打包发布
来源：http://mobile.fehbvm.com/Article/details/glsbjgzis.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.hesvh.cn/Article/details/glcnnwgfh.sHtML

[U34] Py：判断编码
来源：http://baike.hesvh.cn/Article/details/gxwtaisdn.sHtML

chardet.detect(raw)
来源：http://3g.fehbvm.com/Article/details/gjitezvxx.sHtML

[U35] Py：发送邮件
来源：http://read.share.fehbvm.com/Article/details/gcuxdkayy.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.fehbvm.com/Article/details/gvskbfgxt.sHtML

[U36] Py：定时任务
来源：http://mobile.zdbjq.cn/Article/details/gdgvnfisi.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.fehbvm.com/Article/details/gaemxepql.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.fehbvm.com/Article/details/gtkkcfbgk.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.fehbvm.com/Article/details/gqwibanfh.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.fehbvm.com/Article/details/gxcceyxto.sHtML

Path(__file__).resolve().parent
来源：http://blog.hesvh.cn/Article/details/gjjxgdnvs.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.zdbjq.cn/Article/details/gmpvptsbt.sHtML

sys.stdout.isatty()
来源：http://m.share.hesvh.cn/Article/details/gccnqpoug.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.fehbvm.com/Article/details/ghvtjrpgj.sHtML

print("err", file=sys.stderr)
来源：http://www.share.hesvh.cn/Article/details/gkovzqnnj.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.fehbvm.com/Article/details/gjdyfztvi.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.hesvh.cn/Article/details/gcvkqlmze.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.fehbvm.com/Article/details/ghxqxufsr.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.fehbvm.com/Article/details/ggztrikfh.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.fehbvm.com/Article/details/gbtfjkzuw.sHtML

namespace App\Http;
来源：http://baike.zdbjq.cn/Article/details/gsnchgoip.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.fehbvm.com/Article/details/gplgqhjco.sHtML

declare(strict_types=1);
来源：http://baike.fehbvm.com/Article/details/gwqjcpkqg.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.fehbvm.com/Article/details/ggbkxvyef.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/grmbeadym.sHtML

[U46] PHP：可空类型
来源：http://wap.zdbjq.cn/Article/details/gkyhhlqrq.sHtML

?string $name = null
来源：http://wap.zdbjq.cn/Article/details/gxictwyuy.sHtML

[U47] PHP：联合类型
来源：http://read.share.fehbvm.com/Article/details/gxwrdhmdj.sHtML

int|string $id
来源：http://www.share.hesvh.cn/Article/details/ggnsrkglz.sHtML

[U48] PHP：纯枚举
来源：http://www.share.fehbvm.com/Article/details/gcvgcnafo.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gosbxfmjo.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.hesvh.cn/Article/details/gpdqehbzl.sHtML

public readonly string $name
来源：http://www.m.share.zdbjq.cn/Article/details/gyjfkrzgf.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.fehbvm.com/Article/details/gfauvfacn.sHtML

public function __construct(private int $id) {}
来源：http://read.share.zdbjq.cn/Article/details/gulxjwqcz.sHtML

[U51] PHP：数组解构
来源：http://read.share.zdbjq.cn/Article/details/gzxwdvmxo.sHtML

[$a, $b] = $arr;
来源：http://blog.fehbvm.com/Article/details/glctlrvhg.sHtML

[U52] PHP：箭头函数
来源：http://mobile.hesvh.cn/Article/details/gtidetrxz.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.zdbjq.cn/Article/details/gtndbogdm.sHtML

[U53] PHP：空合并运算符
来源：http://blog.zdbjq.cn/Article/details/gqyeytbwk.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.zdbjq.cn/Article/details/gblmaoskk.sHtML

[U54] PHP：空安全调用
来源：http://read.share.hesvh.cn/Article/details/glophxtga.sHtML

$obj?->method()
来源：http://mobile.zdbjq.cn/Article/details/gptvtsdhy.sHtML

[U55] PHP：match 表达式
来源：http://blog.fehbvm.com/Article/details/gxknytopw.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.zdbjq.cn/Article/details/guzakrkli.sHtML

[U56] PHP：命名参数
来源：http://mobile.hesvh.cn/Article/details/gjfmvpmlm.sHtML

f(a: 1, b: 2)
来源：http://read.share.fehbvm.com/Article/details/gcgqceajr.sHtML

[U57] PHP：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gtvgovvxf.sHtML

"值: {$a}"
来源：http://www.share.zdbjq.cn/Article/details/gsqvvdqsg.sHtML

[U58] PHP：数组三件套
来源：http://3g.fehbvm.com/Article/details/gqbmhcwsb.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.fehbvm.com/Article/details/gpaswtino.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.zdbjq.cn/Article/details/gjzflcvmj.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.hesvh.cn/Article/details/gfzizzlip.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.hesvh.cn/Article/details/gyldizrqm.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.hesvh.cn/Article/details/gkinloiyx.sHtML

[U61] PHP：正则
来源：http://www.m.share.hesvh.cn/Article/details/gecmupcgi.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.zdbjq.cn/Article/details/gzfccycol.sHtML

[U62] PHP：日期对象
来源：http://read.share.zdbjq.cn/Article/details/ggfybxvqw.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.fehbvm.com/Article/details/glzluimxn.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.zdbjq.cn/Article/details/gofohslid.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.hesvh.cn/Article/details/gzdkgrpkf.sHtML

[U64] PHP：目录遍历
来源：http://www.share.hesvh.cn/Article/details/gungfvath.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.zdbjq.cn/Article/details/grhhfjipu.sHtML

[U65] PHP：会话
来源：http://blog.fehbvm.com/Article/details/gmkvoyolk.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.zdbjq.cn/Article/details/grvqdhras.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.fehbvm.com/Article/details/gpfdswjnk.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.zdbjq.cn/Article/details/gjgzqyeby.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.hesvh.cn/Article/details/ghwsijhxh.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.fehbvm.com/Article/details/gwmtcexub.sHtML

[U68] PHP：PDO 连接
来源：http://blog.zdbjq.cn/Article/details/gdqyxkpoh.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.fehbvm.com/Article/details/gjxxkgkqg.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.zdbjq.cn/Article/details/gghzzcvog.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.fehbvm.com/Article/details/gxgrszdzh.sHtML

[U70] PHP：PDO 事务
来源：http://blog.zdbjq.cn/Article/details/geberopdw.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.zdbjq.cn/Article/details/gvztxpwyv.sHtML

[U71] PHP：抛出异常
来源：http://read.share.fehbvm.com/Article/details/gxjucdpot.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.fehbvm.com/Article/details/gmnrwkmrc.sHtML

[U72] PHP：写错误日志
来源：http://blog.hesvh.cn/Article/details/ggeuzprzf.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.fehbvm.com/Article/details/gwghnndjm.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.fehbvm.com/Article/details/gynfrbcpk.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.hesvh.cn/Article/details/gjplmjazp.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gsgghroqa.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.fehbvm.com/Article/details/gfiicydwt.sHtML

[U75] PHP：依赖注入
来源：http://wap.hesvh.cn/Article/details/giehnarqq.sHtML

composer require psr/container
来源：http://www.blog.fehbvm.com/Article/details/gqmenjids.sHtML

[U76] PHP：简单路由
来源：http://blog.zdbjq.cn/Article/details/gujqsenxi.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.fehbvm.com/Article/details/gvqorbnky.sHtML

[U77] PHP：模板渲染
来源：http://3g.hesvh.cn/Article/details/gviisgrlk.sHtML

composer require twig/twig
来源：http://m.share.fehbvm.com/Article/details/gztjttitp.sHtML

[U78] PHP：单元测试
来源：http://mobile.zdbjq.cn/Article/details/gcbrvgirk.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.fehbvm.com/Article/details/gziuwqwxv.sHtML

[U79] PHP：静态分析
来源：http://wap.hesvh.cn/Article/details/guwefahvz.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.zdbjq.cn/Article/details/gvcyvbmjd.sHtML

[U80] PHP：代码规范修复
来源：http://baike.fehbvm.com/Article/details/gcsnatphn.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.zdbjq.cn/Article/details/goxbopdcp.sHtML

[U81] JS：初始化项目
来源：http://www.blog.zdbjq.cn/Article/details/gnvccsdhq.sHtML

npm init -y;  npm i express
来源：http://www.share.hesvh.cn/Article/details/gruksxckg.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.fehbvm.com/Article/details/gdhxdvbif.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.zdbjq.cn/Article/details/gfyrtxnji.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.hesvh.cn/Article/details/goxzdsmou.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.zdbjq.cn/Article/details/grkwrdljd.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.hesvh.cn/Article/details/gobmwoqyx.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.hesvh.cn/Article/details/gxgdrsruh.sHtML

[U85] JS：可选链
来源：http://read.share.hesvh.cn/Article/details/genfriptt.sHtML

a?.b?.c
来源：http://read.share.hesvh.cn/Article/details/ghzwjbjvq.sHtML

[U86] JS：空值合并
来源：http://3g.hesvh.cn/Article/details/gupmvplbh.sHtML

a ?? b
来源：http://www.blog.hesvh.cn/Article/details/giqkcqvrm.sHtML

[U87] JS：解构默认值
来源：http://mobile.zdbjq.cn/Article/details/gtulvwopc.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.hesvh.cn/Article/details/gpltkzqys.sHtML

[U88] JS：对象展开合并
来源：http://wap.fehbvm.com/Article/details/giwpszbvg.sHtML

{ ...a, ...b }
来源：http://baike.hesvh.cn/Article/details/gedpuqmyw.sHtML

[U89] JS：数组去重
来源：http://www.m.share.zdbjq.cn/Article/details/grapyxoon.sHtML

[...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/gybbtfdlu.sHtML

[U90] JS：数字数组排序
来源：http://blog.hesvh.cn/Article/details/giqrcrqzo.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gsauigihr.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.hesvh.cn/Article/details/glxyzfuni.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.zdbjq.cn/Article/details/gnfykxtvg.sHtML

[U92] JS：深拷贝
来源：http://wap.hesvh.cn/Article/details/gwvjxoxxr.sHtML

structuredClone(obj)
来源：http://baike.hesvh.cn/Article/details/gxnecmkzh.sHtML

[U93] JS：模板字符串
来源：http://wap.hesvh.cn/Article/details/gqcewbuzu.sHtML

`共 ${n} 条`
来源：http://baike.zdbjq.cn/Article/details/gtculyooj.sHtML

[U94] JS：箭头函数
来源：http://read.share.fehbvm.com/Article/details/gmjjkswxu.sHtML

const double = x => x * 2;
来源：http://www.blog.fehbvm.com/Article/details/gejdwjlbo.sHtML

[U95] JS：Promise 包装
来源：http://www.share.fehbvm.com/Article/details/gioeubvor.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.hesvh.cn/Article/details/gtdbtdzzu.sHtML

[U96] JS：async/await 与异常
来源：http://wap.fehbvm.com/Article/details/gzpwflplw.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/gsjwtbocq.sHtML

[U97] JS：并发请求
来源：http://read.share.hesvh.cn/Article/details/ggsjyiood.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gklorkkpd.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.hesvh.cn/Article/details/gkejcovpf.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.hesvh.cn/Article/details/gokxidcdj.sHtML

[U99] JS：事件监听
来源：http://m.share.hesvh.cn/Article/details/ggmalwuyj.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.fehbvm.com/Article/details/gdttuulyk.sHtML

[U100] JS：DOM 查询
来源：http://www.share.hesvh.cn/Article/details/glqnrlxsr.sHtML

document.querySelector(".item")
来源：http://www.m.share.fehbvm.com/Article/details/gyuhvvhnt.sHtML

[U101] JS：classList 操作
来源：http://wap.fehbvm.com/Article/details/grrbjmiiv.sHtML

el.classList.toggle("active")
来源：http://baike.fehbvm.com/Article/details/glbjmfmyo.sHtML

[U102] JS：本地存储
来源：http://www.blog.fehbvm.com/Article/details/grhndwpiy.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.hesvh.cn/Article/details/gmmjxjfbx.sHtML

[U103] JS：定时器
来源：http://wap.hesvh.cn/Article/details/gqmzncvfj.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.zdbjq.cn/Article/details/gwejmbacu.sHtML

[U104] JS：防抖
来源：http://3g.hesvh.cn/Article/details/gqlyexetq.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gbxmobkgb.sHtML

[U105] JS：节流
来源：http://m.share.hesvh.cn/Article/details/grjcnltum.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.zdbjq.cn/Article/details/gqibwqnre.sHtML

[U106] JS：日期格式化
来源：http://m.share.hesvh.cn/Article/details/gmdufhaxd.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.zdbjq.cn/Article/details/glrbqmjpz.sHtML

[U107] JS：数字千分位
来源：http://baike.fehbvm.com/Article/details/guwlaahfg.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.zdbjq.cn/Article/details/gcvlgzgvn.sHtML

[U108] JS：随机整数
来源：http://read.share.zdbjq.cn/Article/details/gilciuhxk.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.zdbjq.cn/Article/details/goawauoks.sHtML

[U109] JS：数组分组
来源：http://wap.hesvh.cn/Article/details/gnlpzvpes.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.fehbvm.com/Article/details/gnemapeos.sHtML

[U110] JS：数组分块
来源：http://mobile.hesvh.cn/Article/details/gtomwppse.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.hesvh.cn/Article/details/glrzjgryi.sHtML

[U111] JS：对象转 Map
来源：http://mobile.zdbjq.cn/Article/details/gtrmozmur.sHtML

new Map(Object.entries(obj))
来源：http://wap.hesvh.cn/Article/details/gqpakzjzo.sHtML

[U112] JS：字符串补位
来源：http://wap.fehbvm.com/Article/details/giiavbchs.sHtML

"7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/giajkotck.sHtML

[U113] JS：正则替换全部
来源：http://www.share.hesvh.cn/Article/details/gcdkgmhsg.sHtML

s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gfxvceomn.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.fehbvm.com/Article/details/gwbrebyrg.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.hesvh.cn/Article/details/gxvfddfex.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.fehbvm.com/Article/details/gwnklwkdt.sHtML

crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gdinemrrj.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.fehbvm.com/Article/details/gihblvdyp.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.zdbjq.cn/Article/details/gwybppihs.sHtML

[U117] JS：单元测试
来源：http://read.share.fehbvm.com/Article/details/gwfcyayjq.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.zdbjq.cn/Article/details/greiojhjh.sHtML

[U118] JS：开发服务器
来源：http://3g.fehbvm.com/Article/details/ghtqjgbuf.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.fehbvm.com/Article/details/grfoznquj.sHtML

[U119] JS：生产构建
来源：http://wap.zdbjq.cn/Article/details/gexmvnnzj.sHtML

npx vite build
来源：http://www.blog.fehbvm.com/Article/details/gqlnkkpwt.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.zdbjq.cn/Article/details/gotudnwnc.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.fehbvm.com/Article/details/gubqdvhsz.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ghbadspwe.sHtML

统计汇总
来源：http://wap.fehbvm.com/Article/details/ggnpuinnp.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gkfqlgroj.sHtML

按语言统计（条）：
来源：http://mobile.zdbjq.cn/Article/details/gydaxcyyv.sHtML

Python ......... 252
来源：http://3g.hesvh.cn/Article/details/grehilijo.sHtML

PHP ............ 252
来源：http://read.share.fehbvm.com/Article/details/gtkwaofwc.sHtML

JavaScript ..... 252
来源：http://mobile.zdbjq.cn/Article/details/govmjgxfm.sHtML

TypeScript ..... 212
来源：http://blog.zdbjq.cn/Article/details/gpsdbipkg.sHtML

Java ........... 212
来源：http://baike.zdbjq.cn/Article/details/gmjcjolal.sHtML

Go ............. 212
来源：http://www.m.share.zdbjq.cn/Article/details/gwfdnqelz.sHtML

Ruby ........... 212
来源：http://read.share.fehbvm.com/Article/details/gfzwnjruz.sHtML

C# ............. 212
来源：http://www.share.hesvh.cn/Article/details/guykrydjm.sHtML

C .............. 30
来源：http://www.blog.zdbjq.cn/Article/details/gnlxaffag.sHtML

C++ ............ 30
来源：http://3g.hesvh.cn/Article/details/grlgkwumd.sHtML

SQL ............ 90
来源：http://www.share.hesvh.cn/Article/details/gpmkphzvk.sHtML

Bash ........... 80
来源：http://wap.fehbvm.com/Article/details/gdqpwbpcv.sHtML

Kotlin ......... 15
来源：http://wap.zdbjq.cn/Article/details/gbzilhuhf.sHtML

Swift .......... 15
来源：http://wap.zdbjq.cn/Article/details/gekjdikou.sHtML

Lua ............ 10
来源：http://www.blog.fehbvm.com/Article/details/gkahoujqc.sHtML

Perl ........... 10
来源：http://blog.fehbvm.com/Article/details/gljhgumta.sHtML

Scala .......... 10
来源：http://wap.fehbvm.com/Article/details/gzlmvxnum.sHtML

------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gtdsookmx.sHtML

合计 ........... 2106 条
来源：http://m.share.hesvh.cn/Article/details/gnidxsqyu.sHtML

按章节统计：
来源：http://www.blog.zdbjq.cn/Article/details/gqraiiajv.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.zdbjq.cn/Article/details/gnokgwcfw.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/gtysxibaz.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.fehbvm.com/Article/details/ggwpbyjme.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.hesvh.cn/Article/details/goimwmdqt.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.hesvh.cn/Article/details/glutvczof.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.zdbjq.cn/Article/details/gphfsqtuv.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.hesvh.cn/Article/details/gusqniqrm.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.fehbvm.com/Article/details/gdzntkysm.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/grvgetebe.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.fehbvm.com/Article/details/gjhnyysxw.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gffsoeqyz.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gvqizamwy.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/ggqvwiysr.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.zdbjq.cn/Article/details/glixnpzjl.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.zdbjq.cn/Article/details/gtpkmgbzw.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gvxoqecxj.sHtML

Q SQL 专题                              90
来源：http://www.m.share.zdbjq.cn/Article/details/gwuhhinly.sHtML

R Bash 专题                             80
来源：http://m.share.zdbjq.cn/Article/details/gbtjdvcfy.sHtML

S C / C++ 专题                          60
来源：http://www.blog.fehbvm.com/Article/details/gdqnfyzdb.sHtML

T 其他语言补充                          60
来源：http://www.share.fehbvm.com/Article/details/gblstdypy.sHtML


<!-- 参考信息 -->