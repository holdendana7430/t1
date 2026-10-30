代发 wailian999

[U01] Py：创建虚拟环境
来源：http://www.blog.fanxiaobao.xyz/Article/details/gletzgjkn.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.fanxiaobao.xyz/Article/details/gpywudrwl.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.fanxiaobao.xyz/Article/details/gvtubpjny.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/galoyvybu.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmyjlpfit.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.fanxiaobao.xyz/Article/details/gukbykjyj.sHtML

[U04] Py：变量调试打印
来源：http://read.share.fanxiaobao.xyz/Article/details/gqqjxgvhb.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.fanxiaobao.xyz/Article/details/glerdgofd.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gubbdwhns.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.fanxiaobao.xyz/Article/details/gndpwxnhg.sHtML

[U06] Py：合并两个字典
来源：http://wap.fanxiaobao.xyz/Article/details/gfszbbuey.sHtML

{**a, **b}
来源：http://blog.fanxiaobao.xyz/Article/details/gwtofmzrj.sHtML

[U07] Py：反转字典键值
来源：http://mobile.fanxiaobao.xyz/Article/details/gcqzizifd.sHtML

{v: k for k, v in d.items()}
来源：http://baike.fanxiaobao.xyz/Article/details/gffgeigoh.sHtML

[U08] Py：展平二维列表
来源：http://blog.fanxiaobao.xyz/Article/details/gulnkkuen.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfzaqlwmm.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.fanxiaobao.xyz/Article/details/gbnztrkek.sHtML

max(d, key=d.get)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzucwvzps.sHtML

[U10] Py：按值排序字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gohamhxur.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.fanxiaobao.xyz/Article/details/ghqzokvsy.sHtML

[U11] Py：生成器表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gdjxpqssv.sHtML

(x * 2 for x in arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gublcesml.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.fanxiaobao.xyz/Article/details/gusrkjjem.sHtML

Counter(arr).most_common(3)
来源：http://blog.fanxiaobao.xyz/Article/details/gwaywfuga.sHtML

[U13] Py：固定长度队列
来源：http://wap.fanxiaobao.xyz/Article/details/ghhevatbb.sHtML

deque(maxlen=10)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqqvkbkvw.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.fanxiaobao.xyz/Article/details/goepmhxee.sHtML

defaultdict(list)
来源：http://3g.fanxiaobao.xyz/Article/details/gdqjhzmdq.sHtML

[U15] Py：高精度计时
来源：http://baike.fanxiaobao.xyz/Article/details/gpgsasvjk.sHtML

t = time.perf_counter()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggvaanxwq.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.fanxiaobao.xyz/Article/details/gjsnrdinz.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.fanxiaobao.xyz/Article/details/gscxgpfpw.sHtML

[U17] Py：初始化日志
来源：http://wap.fanxiaobao.xyz/Article/details/gvqmroerv.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggmwgtjkl.sHtML

[U18] Py：预编译正则
来源：http://baike.fanxiaobao.xyz/Article/details/gbvqunvlj.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/girtnitbp.sHtML

[U19] Py：正则替换带回调
来源：http://blog.fanxiaobao.xyz/Article/details/govidaktl.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gluvatyks.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.fanxiaobao.xyz/Article/details/geknukbwg.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkeymfsmx.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsggmtmae.sHtML

@contextlib.contextmanager
来源：http://read.share.fanxiaobao.xyz/Article/details/gnnapfbai.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmdhgkwnp.sHtML

list(zip(*m))
来源：http://3g.fanxiaobao.xyz/Article/details/gxhrsjrbo.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjaitvzgo.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.fanxiaobao.xyz/Article/details/gcfzmmqxr.sHtML

[U24] Py：路径操作
来源：http://3g.fanxiaobao.xyz/Article/details/gybwjjdtc.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtkvdlmuy.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmwtptbwe.sHtML

csv.DictReader(f)
来源：http://blog.fanxiaobao.xyz/Article/details/gkqzfkdgq.sHtML

[U26] Py：并发下载
来源：http://3g.fanxiaobao.xyz/Article/details/ghpbheyjq.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gorfdncmm.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fanxiaobao.xyz/Article/details/gpjxdxujy.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.fanxiaobao.xyz/Article/details/ggiwabjkc.sHtML

[U28] Py：类型别名
来源：http://www.share.fanxiaobao.xyz/Article/details/gqaqgbsxl.sHtML

UserId = int
来源：http://www.blog.fanxiaobao.xyz/Article/details/grdpecvvh.sHtML

[U29] Py：属性校验
来源：http://3g.fanxiaobao.xyz/Article/details/grmkpzkdv.sHtML

@property 与 @x.setter 配合
来源：http://3g.fanxiaobao.xyz/Article/details/gojpunoxz.sHtML

[U30] Py：数据类
来源：http://m.share.fanxiaobao.xyz/Article/details/gwmctwdgn.sHtML

@dataclass(slots=True)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkylpozil.sHtML

[U31] Py：单测
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtjqveeks.sHtML

python -m pytest -q
来源：http://baike.fanxiaobao.xyz/Article/details/gsucspept.sHtML

[U32] Py：代码格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gnidyxhpk.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.fanxiaobao.xyz/Article/details/gijowjrzy.sHtML

[U33] Py：打包发布
来源：http://blog.fanxiaobao.xyz/Article/details/guwmspzow.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.fanxiaobao.xyz/Article/details/gpzgqacgo.sHtML

[U34] Py：判断编码
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghfyfmpue.sHtML

chardet.detect(raw)
来源：http://blog.fanxiaobao.xyz/Article/details/ghbmownsg.sHtML

[U35] Py：发送邮件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdvthxzoh.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmdtsdihx.sHtML

[U36] Py：定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gmsoawvef.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gljsormti.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.fanxiaobao.xyz/Article/details/gedjondis.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.fanxiaobao.xyz/Article/details/grbrrwyta.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.fanxiaobao.xyz/Article/details/gcznevlab.sHtML

Path(__file__).resolve().parent
来源：http://m.share.fanxiaobao.xyz/Article/details/gjrsmqfre.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.fanxiaobao.xyz/Article/details/gytraysuz.sHtML

sys.stdout.isatty()
来源：http://3g.fanxiaobao.xyz/Article/details/ggwvqontf.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfiaibfce.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcatyqack.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.fanxiaobao.xyz/Article/details/ggnalhlfu.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.fanxiaobao.xyz/Article/details/gievyvpaq.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.fanxiaobao.xyz/Article/details/ggqndrenu.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.fanxiaobao.xyz/Article/details/guhkinclo.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzmhtckbu.sHtML

namespace App\Http;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwythdlsh.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gnjfesbrn.sHtML

declare(strict_types=1);
来源：http://m.share.fanxiaobao.xyz/Article/details/grvhqpaiu.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.fanxiaobao.xyz/Article/details/ghhjumphf.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gjheetpww.sHtML

[U46] PHP：可空类型
来源：http://3g.fanxiaobao.xyz/Article/details/gngasqaeh.sHtML

?string $name = null
来源：http://baike.fanxiaobao.xyz/Article/details/gwcpsytei.sHtML

[U47] PHP：联合类型
来源：http://wap.fanxiaobao.xyz/Article/details/gbixjqlvb.sHtML

int|string $id
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpwxxzbqy.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gagqfyszx.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gtuqkjpfo.sHtML

[U49] PHP：只读属性
来源：http://blog.fanxiaobao.xyz/Article/details/gjhjuoscy.sHtML

public readonly string $name
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzhjitdsy.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.fanxiaobao.xyz/Article/details/gfypmtipu.sHtML

public function __construct(private int $id) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gelfwglnr.sHtML

[U51] PHP：数组解构
来源：http://wap.fanxiaobao.xyz/Article/details/gzkdglqoz.sHtML

[$a, $b] = $arr;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcueojwcu.sHtML

[U52] PHP：箭头函数
来源：http://baike.fanxiaobao.xyz/Article/details/gnjnmgzmn.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdyrmibxw.sHtML

[U53] PHP：空合并运算符
来源：http://wap.fanxiaobao.xyz/Article/details/gcvhdbpot.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.fanxiaobao.xyz/Article/details/gxhkoauth.sHtML

[U54] PHP：空安全调用
来源：http://www.share.fanxiaobao.xyz/Article/details/gzwfvijxc.sHtML

$obj?->method()
来源：http://read.share.fanxiaobao.xyz/Article/details/giuywngtb.sHtML

[U55] PHP：match 表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gkzbivjoy.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.fanxiaobao.xyz/Article/details/gsprmkeui.sHtML

[U56] PHP：命名参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gstkybcmh.sHtML

f(a: 1, b: 2)
来源：http://baike.fanxiaobao.xyz/Article/details/grvqthyzi.sHtML

[U57] PHP：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gvcqsrthr.sHtML

"值: {$a}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnlbgsgpv.sHtML

[U58] PHP：数组三件套
来源：http://www.share.fanxiaobao.xyz/Article/details/gnmvdyodg.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.fanxiaobao.xyz/Article/details/gbalxszmq.sHtML

[U59] PHP：自定义排序
来源：http://baike.fanxiaobao.xyz/Article/details/gtfsehmas.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxwaseexl.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.fanxiaobao.xyz/Article/details/gyayzxrpi.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.fanxiaobao.xyz/Article/details/gamlsgkue.sHtML

[U61] PHP：正则
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxwhtalxs.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gezsaosdb.sHtML

[U62] PHP：日期对象
来源：http://blog.fanxiaobao.xyz/Article/details/gctiekqkh.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gniqdlrjd.sHtML

[U63] PHP：文件读写
来源：http://mobile.fanxiaobao.xyz/Article/details/gihblwtli.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.fanxiaobao.xyz/Article/details/gotmrbklo.sHtML

[U64] PHP：目录遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gdnoyrkcb.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.fanxiaobao.xyz/Article/details/gbluwkhea.sHtML

[U65] PHP：会话
来源：http://www.share.fanxiaobao.xyz/Article/details/gbhbrkvvv.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gskjiliix.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.fanxiaobao.xyz/Article/details/gealyhwbj.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.fanxiaobao.xyz/Article/details/gptvooaca.sHtML

[U67] PHP：处理文件上传
来源：http://baike.fanxiaobao.xyz/Article/details/gpapknawj.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsjaglaiq.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gpejkzuqs.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.fanxiaobao.xyz/Article/details/gvefuhdvv.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfhtujzpr.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.fanxiaobao.xyz/Article/details/gmqwklrpv.sHtML

[U70] PHP：PDO 事务
来源：http://blog.fanxiaobao.xyz/Article/details/gibeasksw.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.fanxiaobao.xyz/Article/details/gppyutoen.sHtML

[U71] PHP：抛出异常
来源：http://blog.fanxiaobao.xyz/Article/details/gqionvair.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmtmzkjrc.sHtML

[U72] PHP：写错误日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gwhqhjuew.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.fanxiaobao.xyz/Article/details/gkqbkgvqc.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.fanxiaobao.xyz/Article/details/grptqfhpw.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.fanxiaobao.xyz/Article/details/gagmfibwp.sHtML

[U74] PHP：读取环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/gxzdekayy.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.fanxiaobao.xyz/Article/details/ghtjqblmz.sHtML

[U75] PHP：依赖注入
来源：http://read.share.fanxiaobao.xyz/Article/details/gsldmboaz.sHtML

composer require psr/container
来源：http://3g.fanxiaobao.xyz/Article/details/gccoqvcgz.sHtML

[U76] PHP：简单路由
来源：http://baike.fanxiaobao.xyz/Article/details/glatbmvic.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.fanxiaobao.xyz/Article/details/gjtdcrkdb.sHtML

[U77] PHP：模板渲染
来源：http://read.share.fanxiaobao.xyz/Article/details/gdqqffwcg.sHtML

composer require twig/twig
来源：http://blog.fanxiaobao.xyz/Article/details/gjjuzklte.sHtML

[U78] PHP：单元测试
来源：http://baike.fanxiaobao.xyz/Article/details/gtwgkmvjg.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.fanxiaobao.xyz/Article/details/gxjvjlewd.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gznkerbax.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkrxglpdx.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbydcujtn.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.fanxiaobao.xyz/Article/details/gfcfbdvru.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gidxkfojh.sHtML

npm init -y;  npm i express
来源：http://www.share.fanxiaobao.xyz/Article/details/gosuhewil.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.fanxiaobao.xyz/Article/details/gjxapywjk.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcdqaltru.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.fanxiaobao.xyz/Article/details/gfartqtnj.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.fanxiaobao.xyz/Article/details/gpdygjwik.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.fanxiaobao.xyz/Article/details/gfnxigcst.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.fanxiaobao.xyz/Article/details/gttxmzkxb.sHtML

[U85] JS：可选链
来源：http://baike.fanxiaobao.xyz/Article/details/gsahyiazg.sHtML

a?.b?.c
来源：http://blog.fanxiaobao.xyz/Article/details/ghwuvqywf.sHtML

[U86] JS：空值合并
来源：http://baike.fanxiaobao.xyz/Article/details/gfgulvqib.sHtML

a ?? b
来源：http://www.share.fanxiaobao.xyz/Article/details/gnxalwtle.sHtML

[U87] JS：解构默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/gqtlvizrn.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxazfojjj.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfzohcepw.sHtML

{ ...a, ...b }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gptqjwpbl.sHtML

[U89] JS：数组去重
来源：http://read.share.fanxiaobao.xyz/Article/details/gucjkmolr.sHtML

[...new Set(arr)]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gucstcvuf.sHtML

[U90] JS：数字数组排序
来源：http://3g.fanxiaobao.xyz/Article/details/gjoecwioa.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.fanxiaobao.xyz/Article/details/gkocjekdk.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gikeekluo.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.fanxiaobao.xyz/Article/details/gehkmdpui.sHtML

[U92] JS：深拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gqiunplor.sHtML

structuredClone(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdyvosqhf.sHtML

[U93] JS：模板字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gohgoagek.sHtML

`共 ${n} 条`
来源：http://m.share.fanxiaobao.xyz/Article/details/gtcsqtrbq.sHtML

[U94] JS：箭头函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gneoiaumj.sHtML

const double = x => x * 2;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggwivsaic.sHtML

[U95] JS：Promise 包装
来源：http://3g.fanxiaobao.xyz/Article/details/gqsfrgngj.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.fanxiaobao.xyz/Article/details/gwvahitdg.sHtML

[U96] JS：async/await 与异常
来源：http://blog.fanxiaobao.xyz/Article/details/glmtifwlh.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmxvjcrbj.sHtML

[U97] JS：并发请求
来源：http://m.share.fanxiaobao.xyz/Article/details/guubfetsn.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fanxiaobao.xyz/Article/details/gylmgrktz.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfqmsvzcy.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvqgxeoup.sHtML

[U99] JS：事件监听
来源：http://m.share.fanxiaobao.xyz/Article/details/gzruqwkbb.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.fanxiaobao.xyz/Article/details/gvzcnrkuw.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gifnsfpbk.sHtML

document.querySelector(".item")
来源：http://3g.fanxiaobao.xyz/Article/details/ggkbdxnqn.sHtML

[U101] JS：classList 操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gvsycwmyz.sHtML

el.classList.toggle("active")
来源：http://blog.fanxiaobao.xyz/Article/details/gisgkpuqs.sHtML

[U102] JS：本地存储
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtksnwdpb.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.fanxiaobao.xyz/Article/details/gttoqdazc.sHtML

[U103] JS：定时器
来源：http://m.share.fanxiaobao.xyz/Article/details/gaujlquoy.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gumqfufof.sHtML

[U104] JS：防抖
来源：http://mobile.fanxiaobao.xyz/Article/details/gzacqhiqn.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fanxiaobao.xyz/Article/details/gjfbyjjbk.sHtML

[U105] JS：节流
来源：http://3g.fanxiaobao.xyz/Article/details/gamtiqjix.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gpxbtnpit.sHtML

[U106] JS：日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/giqhrvjoi.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.fanxiaobao.xyz/Article/details/gczbasvwa.sHtML

[U107] JS：数字千分位
来源：http://www.share.fanxiaobao.xyz/Article/details/gvvjukclx.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.fanxiaobao.xyz/Article/details/gdgngjltp.sHtML

[U108] JS：随机整数
来源：http://blog.fanxiaobao.xyz/Article/details/gkreyijlv.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.fanxiaobao.xyz/Article/details/genuyeuuk.sHtML

[U109] JS：数组分组
来源：http://wap.fanxiaobao.xyz/Article/details/gecwpngjm.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.fanxiaobao.xyz/Article/details/giidphgfj.sHtML

[U110] JS：数组分块
来源：http://baike.fanxiaobao.xyz/Article/details/gvltdlkax.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.fanxiaobao.xyz/Article/details/gcynrkwnd.sHtML

[U111] JS：对象转 Map
来源：http://mobile.fanxiaobao.xyz/Article/details/ggrvcjndc.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdxktcagv.sHtML

[U112] JS：字符串补位
来源：http://blog.fanxiaobao.xyz/Article/details/gvtkfjhij.sHtML

"7".padStart(3, "0")
来源：http://3g.fanxiaobao.xyz/Article/details/gaosfzsgg.sHtML

[U113] JS：正则替换全部
来源：http://blog.fanxiaobao.xyz/Article/details/gygcjyxdg.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gadswnqog.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmgebxyru.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gupceprib.sHtML

[U115] JS：生成 UUID
来源：http://blog.fanxiaobao.xyz/Article/details/gsqedhzoz.sHtML

crypto.randomUUID()
来源：http://read.share.fanxiaobao.xyz/Article/details/ghcajcazi.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.fanxiaobao.xyz/Article/details/grcuegizu.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gmeuzbgce.sHtML

[U117] JS：单元测试
来源：http://baike.fanxiaobao.xyz/Article/details/gjmeajidh.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggqdnibdb.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtkmlriaf.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grijhrxfd.sHtML

[U119] JS：生产构建
来源：http://www.share.fanxiaobao.xyz/Article/details/gpztytcxb.sHtML

npx vite build
来源：http://www.share.fanxiaobao.xyz/Article/details/gxksugegq.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.fanxiaobao.xyz/Article/details/gleuoqobk.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.fanxiaobao.xyz/Article/details/gvdvrgqjp.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/ghzlpkbts.sHtML

统计汇总
来源：http://blog.fanxiaobao.xyz/Article/details/gshwmfqkl.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gzuutftyy.sHtML

按语言统计（条）：
来源：http://baike.fanxiaobao.xyz/Article/details/gotdwewyy.sHtML

Python ......... 252
来源：http://blog.fanxiaobao.xyz/Article/details/gwuhhzeli.sHtML

PHP ............ 252
来源：http://read.share.fanxiaobao.xyz/Article/details/gjwrgitiq.sHtML

JavaScript ..... 252
来源：http://m.share.fanxiaobao.xyz/Article/details/grimrqini.sHtML

TypeScript ..... 212
来源：http://blog.fanxiaobao.xyz/Article/details/gwuktkftr.sHtML

Java ........... 212
来源：http://blog.fanxiaobao.xyz/Article/details/gbbdogwzx.sHtML

Go ............. 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gnpllhgfw.sHtML

Ruby ........... 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gxqwyenjn.sHtML

C# ............. 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/getxjjcms.sHtML

C .............. 30
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwuiommlk.sHtML

C++ ............ 30
来源：http://3g.fanxiaobao.xyz/Article/details/gqblraeqv.sHtML

SQL ............ 90
来源：http://m.share.fanxiaobao.xyz/Article/details/gsrcnbimg.sHtML

Bash ........... 80
来源：http://m.share.fanxiaobao.xyz/Article/details/gbbfhjxgm.sHtML

Kotlin ......... 15
来源：http://3g.fanxiaobao.xyz/Article/details/gmqwhgmbk.sHtML

Swift .......... 15
来源：http://mobile.fanxiaobao.xyz/Article/details/gzhsfswbj.sHtML

Lua ............ 10
来源：http://blog.fanxiaobao.xyz/Article/details/gipbadipw.sHtML

Perl ........... 10
来源：http://3g.fanxiaobao.xyz/Article/details/gwyfbypbw.sHtML

Scala .......... 10
来源：http://blog.fanxiaobao.xyz/Article/details/gxzjlxoyc.sHtML

------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/giaciqnob.sHtML

合计 ........... 2106 条
来源：http://m.share.fanxiaobao.xyz/Article/details/gabtzhzno.sHtML

按章节统计：
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwzyyeanc.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.fanxiaobao.xyz/Article/details/geqyhtans.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gasoznjri.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmgdvjvdb.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdkqgqkmj.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.fanxiaobao.xyz/Article/details/gaujztrxl.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.fanxiaobao.xyz/Article/details/gfvwkiunn.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.fanxiaobao.xyz/Article/details/gjvqjswcr.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.fanxiaobao.xyz/Article/details/grrqetljg.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/gpyvkwavx.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.fanxiaobao.xyz/Article/details/gratizbuy.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/gzsahflsg.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/ghqpumvzh.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/gjqxuiuap.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.fanxiaobao.xyz/Article/details/gjbyxrnsi.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.fanxiaobao.xyz/Article/details/gebbjncjn.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gmwawmjkm.sHtML

Q SQL 专题                              90
来源：http://wap.fanxiaobao.xyz/Article/details/gudronbyb.sHtML

R Bash 专题                             80
来源：http://3g.fanxiaobao.xyz/Article/details/ggabmszge.sHtML

S C / C++ 专题                          60
来源：http://wap.fanxiaobao.xyz/Article/details/gjtfjaiez.sHtML

T 其他语言补充                          60
来源：http://mobile.fanxiaobao.xyz/Article/details/gcnrymcvu.sHtML

U 高频实用片段                         120
来源：http://3g.fanxiaobao.xyz/Article/details/gumgroipz.sHtML

------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvhfholgz.sHtML

合计                                  2106 条
来源：http://blog.fanxiaobao.xyz/Article/details/gvanlnudt.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guvmoelje.sHtML

使用提醒
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzkdepssv.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/goyzxriiw.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.fanxiaobao.xyz/Article/details/gojeurmie.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.fanxiaobao.xyz/Article/details/gxjqbuwse.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.fanxiaobao.xyz/Article/details/gqqqhinld.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.fanxiaobao.xyz/Article/details/gaomxataq.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.fanxiaobao.xyz/Article/details/gbkibggzc.sHtML

—— 文件结束 ——
来源：http://mobile.fanxiaobao.xyz/Article/details/gzoqcyzeu.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfeztdmup.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.fanxiaobao.xyz/Article/details/guwsofwrv.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.fanxiaobao.xyz/Article/details/grkzlccdw.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gsbelvrxz.sHtML


<!-- 参考信息 -->