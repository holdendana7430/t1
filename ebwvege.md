代发 wailian999

[U01] Py：创建虚拟环境
来源：http://read.share.fanxiaobao.xyz/Article/details/glkvlbpcw.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxowuznzy.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.fanxiaobao.xyz/Article/details/gcrskucks.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/grtwejrxw.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.fanxiaobao.xyz/Article/details/gfbjwtmhp.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.fanxiaobao.xyz/Article/details/glflysabz.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxxuvoikz.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.fanxiaobao.xyz/Article/details/gidiakrqb.sHtML

[U05] Py：列表去重且保序
来源：http://blog.fanxiaobao.xyz/Article/details/gvwjfdryi.sHtML

list(dict.fromkeys(arr))
来源：http://baike.fanxiaobao.xyz/Article/details/gfthwyoni.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gdvkzccad.sHtML

{**a, **b}
来源：http://3g.fanxiaobao.xyz/Article/details/ghhkvrdnc.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmuurdzva.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fanxiaobao.xyz/Article/details/gypujfhfe.sHtML

[U08] Py：展平二维列表
来源：http://www.share.fanxiaobao.xyz/Article/details/gbmpdwiwx.sHtML

[y for x in nested for y in x]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjkijpxyp.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.fanxiaobao.xyz/Article/details/gkhrqwvra.sHtML

max(d, key=d.get)
来源：http://mobile.fanxiaobao.xyz/Article/details/gknninqzt.sHtML

[U10] Py：按值排序字典
来源：http://blog.fanxiaobao.xyz/Article/details/gidoueptd.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwqfizubt.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsnpxavgd.sHtML

(x * 2 for x in arr)
来源：http://wap.fanxiaobao.xyz/Article/details/gltypvihc.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.fanxiaobao.xyz/Article/details/gbbgkllwj.sHtML

Counter(arr).most_common(3)
来源：http://blog.fanxiaobao.xyz/Article/details/gycnjbdzh.sHtML

[U13] Py：固定长度队列
来源：http://3g.fanxiaobao.xyz/Article/details/gzddgjirk.sHtML

deque(maxlen=10)
来源：http://mobile.fanxiaobao.xyz/Article/details/gufxwhluy.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggjptjnlh.sHtML

defaultdict(list)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guxscxzvx.sHtML

[U15] Py：高精度计时
来源：http://blog.fanxiaobao.xyz/Article/details/gecuueacp.sHtML

t = time.perf_counter()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqlslnxr.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fanxiaobao.xyz/Article/details/gbyatvcea.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gedijmyvj.sHtML

[U17] Py：初始化日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtahpisad.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.fanxiaobao.xyz/Article/details/gdycufnrq.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnqxaosff.sHtML

pat = re.compile(r"\d+")
来源：http://wap.fanxiaobao.xyz/Article/details/gvujozlup.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.fanxiaobao.xyz/Article/details/gzplvaiwe.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnbbmohpy.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.fanxiaobao.xyz/Article/details/gzyvnxouq.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfsntnnor.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxvoglxbb.sHtML

@contextlib.contextmanager
来源：http://blog.fanxiaobao.xyz/Article/details/glsnyvcbr.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtnaenciu.sHtML

list(zip(*m))
来源：http://baike.fanxiaobao.xyz/Article/details/ggrwbwqua.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gluypmser.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvixcwpni.sHtML

[U24] Py：路径操作
来源：http://3g.fanxiaobao.xyz/Article/details/gyilbwmkp.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.fanxiaobao.xyz/Article/details/gqouxniad.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.fanxiaobao.xyz/Article/details/gujphofii.sHtML

csv.DictReader(f)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghxsvoptg.sHtML

[U26] Py：并发下载
来源：http://blog.fanxiaobao.xyz/Article/details/ghfekxlaw.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.fanxiaobao.xyz/Article/details/gkrwuvglw.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwdlmbhye.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grtblxhzf.sHtML

[U28] Py：类型别名
来源：http://m.share.fanxiaobao.xyz/Article/details/gwrplrcuk.sHtML

UserId = int
来源：http://baike.fanxiaobao.xyz/Article/details/grtlvloqt.sHtML

[U29] Py：属性校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxjirbtjv.sHtML

@property 与 @x.setter 配合
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjjkjtte.sHtML

[U30] Py：数据类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmvgnebnf.sHtML

@dataclass(slots=True)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqxhxsfht.sHtML

[U31] Py：单测
来源：http://baike.fanxiaobao.xyz/Article/details/gocorflho.sHtML

python -m pytest -q
来源：http://mobile.fanxiaobao.xyz/Article/details/gbeqgyfvy.sHtML

[U32] Py：代码格式化
来源：http://blog.fanxiaobao.xyz/Article/details/ghnognrpt.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.fanxiaobao.xyz/Article/details/gbzmiuihr.sHtML

[U33] Py：打包发布
来源：http://3g.fanxiaobao.xyz/Article/details/giekhzaof.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.fanxiaobao.xyz/Article/details/gbgfqmhcf.sHtML

[U34] Py：判断编码
来源：http://www.share.fanxiaobao.xyz/Article/details/gnjbajgsw.sHtML

chardet.detect(raw)
来源：http://blog.fanxiaobao.xyz/Article/details/gvwvgisku.sHtML

[U35] Py：发送邮件
来源：http://m.share.fanxiaobao.xyz/Article/details/gdcmagoix.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.fanxiaobao.xyz/Article/details/goysnhnwy.sHtML

[U36] Py：定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmsfurjgn.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.fanxiaobao.xyz/Article/details/gslqajmvs.sHtML

[U37] Py：读写 Excel
来源：http://wap.fanxiaobao.xyz/Article/details/goprclubn.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.fanxiaobao.xyz/Article/details/gpxcippui.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fanxiaobao.xyz/Article/details/gvmssvxre.sHtML

Path(__file__).resolve().parent
来源：http://read.share.fanxiaobao.xyz/Article/details/gbnvumhyh.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.fanxiaobao.xyz/Article/details/gylwjpzue.sHtML

sys.stdout.isatty()
来源：http://blog.fanxiaobao.xyz/Article/details/gdwswwyto.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gldqczgdd.sHtML

print("err", file=sys.stderr)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghqavuyif.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdqhwmven.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.fanxiaobao.xyz/Article/details/ghdilkijh.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfmavthtu.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.fanxiaobao.xyz/Article/details/gwjjyubhx.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grwpksnly.sHtML

namespace App\Http;
来源：http://www.share.fanxiaobao.xyz/Article/details/gugtgmcyg.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpviaodhr.sHtML

declare(strict_types=1);
来源：http://3g.fanxiaobao.xyz/Article/details/gpfwbuzsi.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gnxygalko.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gwdzwjeoj.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghrfuiidp.sHtML

?string $name = null
来源：http://m.share.fanxiaobao.xyz/Article/details/gxjoqsvuh.sHtML

[U47] PHP：联合类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsnnlwshz.sHtML

int|string $id
来源：http://mobile.fanxiaobao.xyz/Article/details/ghapixzhm.sHtML

[U48] PHP：纯枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gxdpcaeov.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gkatbvgre.sHtML

[U49] PHP：只读属性
来源：http://mobile.fanxiaobao.xyz/Article/details/gsjxxomgq.sHtML

public readonly string $name
来源：http://read.share.fanxiaobao.xyz/Article/details/glzjkgifu.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.fanxiaobao.xyz/Article/details/gutigbcgp.sHtML

public function __construct(private int $id) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gldzhhsvc.sHtML

[U51] PHP：数组解构
来源：http://blog.fanxiaobao.xyz/Article/details/graytrsyy.sHtML

[$a, $b] = $arr;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbdlaluwd.sHtML

[U52] PHP：箭头函数
来源：http://baike.fanxiaobao.xyz/Article/details/goqfjstym.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkcnchkac.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.fanxiaobao.xyz/Article/details/gnzygjasg.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnszvtmhz.sHtML

[U54] PHP：空安全调用
来源：http://www.share.fanxiaobao.xyz/Article/details/gxkwlowex.sHtML

$obj?->method()
来源：http://3g.fanxiaobao.xyz/Article/details/gcnfnwzlm.sHtML

[U55] PHP：match 表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gqcbccljf.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.fanxiaobao.xyz/Article/details/gzhzmzvjk.sHtML

[U56] PHP：命名参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxrdxmtly.sHtML

f(a: 1, b: 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/geuhybuqc.sHtML

[U57] PHP：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/glmkbaesq.sHtML

"值: {$a}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gnkfmwgzf.sHtML

[U58] PHP：数组三件套
来源：http://3g.fanxiaobao.xyz/Article/details/gwhzhwewd.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbrogazyh.sHtML

[U59] PHP：自定义排序
来源：http://3g.fanxiaobao.xyz/Article/details/gqbzbrbmm.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fanxiaobao.xyz/Article/details/gpzaqgpcf.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.fanxiaobao.xyz/Article/details/gntplxtvh.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.fanxiaobao.xyz/Article/details/gvvmanita.sHtML

[U61] PHP：正则
来源：http://mobile.fanxiaobao.xyz/Article/details/gidfluhis.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gfjhvkxhk.sHtML

[U62] PHP：日期对象
来源：http://baike.fanxiaobao.xyz/Article/details/gbmrskeca.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.fanxiaobao.xyz/Article/details/gksupwsyw.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqzlwcdhd.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gesmhamzo.sHtML

[U64] PHP：目录遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gfjpwaztf.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.fanxiaobao.xyz/Article/details/ggdzatbgb.sHtML

[U65] PHP：会话
来源：http://www.share.fanxiaobao.xyz/Article/details/gkeyvxrep.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gomhocshk.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gftgvprzb.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.fanxiaobao.xyz/Article/details/ghntuicpu.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.fanxiaobao.xyz/Article/details/ggsxttzog.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.fanxiaobao.xyz/Article/details/gcaipezgz.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjdcrhevz.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.fanxiaobao.xyz/Article/details/gqnpdcftn.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.fanxiaobao.xyz/Article/details/gwexumzuv.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.fanxiaobao.xyz/Article/details/guxfocqkj.sHtML

[U70] PHP：PDO 事务
来源：http://blog.fanxiaobao.xyz/Article/details/gavpxzupy.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.fanxiaobao.xyz/Article/details/gexpakeoi.sHtML

[U71] PHP：抛出异常
来源：http://baike.fanxiaobao.xyz/Article/details/girntgyld.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.fanxiaobao.xyz/Article/details/giuqotdit.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpnbyvrcu.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.fanxiaobao.xyz/Article/details/grcgpybsz.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.fanxiaobao.xyz/Article/details/gjybnyfwq.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.fanxiaobao.xyz/Article/details/grjydbjru.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggtkxrejv.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.fanxiaobao.xyz/Article/details/gmmqjtqqd.sHtML

[U75] PHP：依赖注入
来源：http://baike.fanxiaobao.xyz/Article/details/gpwmgpdjw.sHtML

composer require psr/container
来源：http://3g.fanxiaobao.xyz/Article/details/gbwnbmleh.sHtML

[U76] PHP：简单路由
来源：http://m.share.fanxiaobao.xyz/Article/details/gczckjfhz.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxngegvad.sHtML

[U77] PHP：模板渲染
来源：http://mobile.fanxiaobao.xyz/Article/details/ghbmcdsaf.sHtML

composer require twig/twig
来源：http://read.share.fanxiaobao.xyz/Article/details/gaxpebujx.sHtML

[U78] PHP：单元测试
来源：http://www.share.fanxiaobao.xyz/Article/details/gbtgkqiyh.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.fanxiaobao.xyz/Article/details/geeqogvim.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaaucyndl.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.fanxiaobao.xyz/Article/details/gjxyjutej.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.fanxiaobao.xyz/Article/details/gjifllmsl.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.fanxiaobao.xyz/Article/details/gqfrgccuq.sHtML

[U81] JS：初始化项目
来源：http://blog.fanxiaobao.xyz/Article/details/gshshmcxi.sHtML

npm init -y;  npm i express
来源：http://read.share.fanxiaobao.xyz/Article/details/gztkifcds.sHtML

[U82] JS：package.json 脚本
来源：http://blog.fanxiaobao.xyz/Article/details/gcohtjwda.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.fanxiaobao.xyz/Article/details/grgaqbucc.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.fanxiaobao.xyz/Article/details/gcgdyidxk.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.fanxiaobao.xyz/Article/details/gcfmzmywf.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.fanxiaobao.xyz/Article/details/gnzzbjbyv.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.fanxiaobao.xyz/Article/details/gnhqrpxkn.sHtML

[U85] JS：可选链
来源：http://m.share.fanxiaobao.xyz/Article/details/guyjczawn.sHtML

a?.b?.c
来源：http://m.share.fanxiaobao.xyz/Article/details/gxcynowng.sHtML

[U86] JS：空值合并
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqnwsxvri.sHtML

a ?? b
来源：http://3g.fanxiaobao.xyz/Article/details/gldrkhtrv.sHtML

[U87] JS：解构默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/gwugsylyg.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxieapdds.sHtML

[U88] JS：对象展开合并
来源：http://m.share.fanxiaobao.xyz/Article/details/gaoojqtmz.sHtML

{ ...a, ...b }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdewisgaj.sHtML

[U89] JS：数组去重
来源：http://3g.fanxiaobao.xyz/Article/details/gcbphyrim.sHtML

[...new Set(arr)]
来源：http://3g.fanxiaobao.xyz/Article/details/gqytcodyh.sHtML

[U90] JS：数字数组排序
来源：http://blog.fanxiaobao.xyz/Article/details/gsgcltmvu.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.fanxiaobao.xyz/Article/details/ggyaedvww.sHtML

[U91] JS：对象键值遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gxsxjvtvn.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.fanxiaobao.xyz/Article/details/gqntcbbrz.sHtML

[U92] JS：深拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gysjwdvpz.sHtML

structuredClone(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdokkdmxs.sHtML

[U93] JS：模板字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxrxadhcn.sHtML

`共 ${n} 条`
来源：http://read.share.fanxiaobao.xyz/Article/details/gmcbtpepd.sHtML

[U94] JS：箭头函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gaqsyejwl.sHtML

const double = x => x * 2;
来源：http://3g.fanxiaobao.xyz/Article/details/gqidlhdec.sHtML

[U95] JS：Promise 包装
来源：http://3g.fanxiaobao.xyz/Article/details/ghstjtgej.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.fanxiaobao.xyz/Article/details/gfkojtica.sHtML

[U96] JS：async/await 与异常
来源：http://3g.fanxiaobao.xyz/Article/details/gsecdjyzj.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvidspxqp.sHtML

[U97] JS：并发请求
来源：http://wap.fanxiaobao.xyz/Article/details/ghzwehvsj.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fanxiaobao.xyz/Article/details/giuvkorsi.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.fanxiaobao.xyz/Article/details/gkfskowqu.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxavujhfz.sHtML

[U99] JS：事件监听
来源：http://baike.fanxiaobao.xyz/Article/details/gfsqlsayv.sHtML

el.addEventListener("click", e => {})
来源：http://blog.fanxiaobao.xyz/Article/details/guewkucni.sHtML

[U100] JS：DOM 查询
来源：http://wap.fanxiaobao.xyz/Article/details/gppccnlwl.sHtML

document.querySelector(".item")
来源：http://m.share.fanxiaobao.xyz/Article/details/gtqcwsyuw.sHtML

[U101] JS：classList 操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gyiwsaojt.sHtML

el.classList.toggle("active")
来源：http://mobile.fanxiaobao.xyz/Article/details/gcpojktrg.sHtML

[U102] JS：本地存储
来源：http://www.blog.fanxiaobao.xyz/Article/details/glddwtiwm.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.fanxiaobao.xyz/Article/details/gsvyybujs.sHtML

[U103] JS：定时器
来源：http://www.share.fanxiaobao.xyz/Article/details/gcegdfuwk.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.fanxiaobao.xyz/Article/details/gnzejdgtv.sHtML

[U104] JS：防抖
来源：http://wap.fanxiaobao.xyz/Article/details/gdrdpohnf.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggphppbuc.sHtML

[U105] JS：节流
来源：http://wap.fanxiaobao.xyz/Article/details/gwomzhycp.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gzauvdnuu.sHtML

[U106] JS：日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gnvayjusz.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.fanxiaobao.xyz/Article/details/gwenhlnbu.sHtML

[U107] JS：数字千分位
来源：http://3g.fanxiaobao.xyz/Article/details/gxrtbklyv.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcdyorpmn.sHtML

[U108] JS：随机整数
来源：http://baike.fanxiaobao.xyz/Article/details/gcfvjkdew.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.fanxiaobao.xyz/Article/details/gkuofqqde.sHtML

[U109] JS：数组分组
来源：http://blog.fanxiaobao.xyz/Article/details/gltjhjsqk.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.fanxiaobao.xyz/Article/details/gxrsqdemh.sHtML

[U110] JS：数组分块
来源：http://www.share.fanxiaobao.xyz/Article/details/glxqfapmn.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.fanxiaobao.xyz/Article/details/gxqueeiay.sHtML

[U111] JS：对象转 Map
来源：http://wap.fanxiaobao.xyz/Article/details/gcbydpsvd.sHtML

new Map(Object.entries(obj))
来源：http://wap.fanxiaobao.xyz/Article/details/gjtzhklbw.sHtML

[U112] JS：字符串补位
来源：http://3g.fanxiaobao.xyz/Article/details/gshsnhpcs.sHtML

"7".padStart(3, "0")
来源：http://blog.fanxiaobao.xyz/Article/details/gyresgxkb.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.fanxiaobao.xyz/Article/details/gniqshked.sHtML

s.replaceAll("a", "b")
来源：http://m.share.fanxiaobao.xyz/Article/details/gbhobnong.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwewsrhfn.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fanxiaobao.xyz/Article/details/ghtumbmqm.sHtML

[U115] JS：生成 UUID
来源：http://wap.fanxiaobao.xyz/Article/details/ghcfzcppy.sHtML

crypto.randomUUID()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gotxyrdhf.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.fanxiaobao.xyz/Article/details/gsxxunvph.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gvqcudaki.sHtML

[U117] JS：单元测试
来源：http://wap.fanxiaobao.xyz/Article/details/ggwlxqhuw.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.fanxiaobao.xyz/Article/details/gjaqaqohi.sHtML

[U118] JS：开发服务器
来源：http://m.share.fanxiaobao.xyz/Article/details/glqyltqov.sHtML

npm i -D vite;  npx vite
来源：http://wap.fanxiaobao.xyz/Article/details/grjsnitby.sHtML

[U119] JS：生产构建
来源：http://read.share.fanxiaobao.xyz/Article/details/gtbvycnht.sHtML

npx vite build
来源：http://mobile.fanxiaobao.xyz/Article/details/gvuocgzfs.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.fanxiaobao.xyz/Article/details/gdipssfcl.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.fanxiaobao.xyz/Article/details/gurhqvoob.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gbkqjsmmr.sHtML

统计汇总
来源：http://blog.fanxiaobao.xyz/Article/details/gxczssdzu.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gjvwtzvdd.sHtML

按语言统计（条）：
来源：http://m.share.fanxiaobao.xyz/Article/details/gyzgwmxtk.sHtML

Python ......... 252
来源：http://www.share.fanxiaobao.xyz/Article/details/gbljdhvbh.sHtML

PHP ............ 252
来源：http://blog.fanxiaobao.xyz/Article/details/gbhduoxve.sHtML

JavaScript ..... 252
来源：http://blog.fanxiaobao.xyz/Article/details/gtabrptvl.sHtML

TypeScript ..... 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gcnrbqgee.sHtML

Java ........... 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtmsfzoci.sHtML

Go ............. 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gmsgrttdp.sHtML

Ruby ........... 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gpgjclajv.sHtML

C# ............. 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gmudwfsxm.sHtML

C .............. 30
来源：http://wap.fanxiaobao.xyz/Article/details/gfwqgqdfa.sHtML

C++ ............ 30
来源：http://read.share.fanxiaobao.xyz/Article/details/grgdpizus.sHtML

SQL ............ 90
来源：http://read.share.fanxiaobao.xyz/Article/details/grnozoaab.sHtML

Bash ........... 80
来源：http://www.share.fanxiaobao.xyz/Article/details/gudsxsmvv.sHtML

Kotlin ......... 15
来源：http://baike.fanxiaobao.xyz/Article/details/gvzsifimu.sHtML

Swift .......... 15
来源：http://baike.fanxiaobao.xyz/Article/details/gtbymaszw.sHtML

Lua ............ 10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnbgouger.sHtML

Perl ........... 10
来源：http://read.share.fanxiaobao.xyz/Article/details/gyelothih.sHtML

Scala .......... 10
来源：http://baike.fanxiaobao.xyz/Article/details/gfjfrtewn.sHtML

------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkvolewbs.sHtML

合计 ........... 2106 条
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnxxkejjo.sHtML

按章节统计：
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjpiszenl.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjzlocet.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.fanxiaobao.xyz/Article/details/gyufaxkyl.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.fanxiaobao.xyz/Article/details/galakhnfw.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.fanxiaobao.xyz/Article/details/ginpmclpu.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnoyswevd.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.fanxiaobao.xyz/Article/details/gtyciljid.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.fanxiaobao.xyz/Article/details/gvftvrayd.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.fanxiaobao.xyz/Article/details/gzalzobwq.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gykgjoseu.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.fanxiaobao.xyz/Article/details/gadzcgyqs.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/ghrnwvyho.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gftetdzeg.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdzyxdbvt.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.fanxiaobao.xyz/Article/details/gfyfbefdh.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.fanxiaobao.xyz/Article/details/gwytdyrtw.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/gleeluiec.sHtML

Q SQL 专题                              90
来源：http://m.share.fanxiaobao.xyz/Article/details/gdepmffmu.sHtML

R Bash 专题                             80
来源：http://read.share.fanxiaobao.xyz/Article/details/gvjrpngni.sHtML

S C / C++ 专题                          60
来源：http://blog.fanxiaobao.xyz/Article/details/gyieesjpm.sHtML

T 其他语言补充                          60
来源：http://read.share.fanxiaobao.xyz/Article/details/gesadsqia.sHtML

U 高频实用片段                         120
来源：http://www.share.fanxiaobao.xyz/Article/details/gzqbcrrau.sHtML

------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/gfpomwxnc.sHtML

合计                                  2106 条
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqshbgchf.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/gvbsphgrr.sHtML

使用提醒
来源：http://read.share.fanxiaobao.xyz/Article/details/gtlqdcwxa.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gophgysfx.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.fanxiaobao.xyz/Article/details/gdrrzglcy.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.fanxiaobao.xyz/Article/details/gvcyxivez.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.fanxiaobao.xyz/Article/details/gtjyeumqy.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqrhqehys.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.fanxiaobao.xyz/Article/details/gtzzaioxe.sHtML

—— 文件结束 ——
来源：http://www.blog.fanxiaobao.xyz/Article/details/gueuwjyiz.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gbvjazqde.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.fanxiaobao.xyz/Article/details/gkluncvji.sHtML

Common Programming Examples Cheat Book
来源：http://blog.fanxiaobao.xyz/Article/details/gajfynitr.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gcchwvtzh.sHtML


<!-- 参考信息 -->