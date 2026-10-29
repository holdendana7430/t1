代发 wailian999

[U01] Py：创建虚拟环境
来源：http://m.share.hesvh.cn/Article/details/gzccrlwdb.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.fehbvm.com/Article/details/gxuswrhqm.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.fehbvm.com/Article/details/grykaimkc.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.zdbjq.cn/Article/details/glxsdoowp.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.fehbvm.com/Article/details/gebgzsciz.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.hesvh.cn/Article/details/gdwvsevmt.sHtML

[U04] Py：变量调试打印
来源：http://www.share.hesvh.cn/Article/details/gxgdaxgxy.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.fehbvm.com/Article/details/guzunmuvr.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.hesvh.cn/Article/details/gczakhwqy.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/gfwvhpswf.sHtML

[U06] Py：合并两个字典
来源：http://blog.hesvh.cn/Article/details/gonfjxseh.sHtML

{**a, **b}
来源：http://www.m.share.hesvh.cn/Article/details/geysyuwop.sHtML

[U07] Py：反转字典键值
来源：http://wap.zdbjq.cn/Article/details/gzgzuheab.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.hesvh.cn/Article/details/gptoomeuh.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.zdbjq.cn/Article/details/gjlvrxrvs.sHtML

[y for x in nested for y in x]
来源：http://3g.fehbvm.com/Article/details/glnqsyhbw.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.hesvh.cn/Article/details/gkiwebqpm.sHtML

max(d, key=d.get)
来源：http://read.share.zdbjq.cn/Article/details/glksjrdiv.sHtML

[U10] Py：按值排序字典
来源：http://m.share.fehbvm.com/Article/details/gjtcmlzjm.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.zdbjq.cn/Article/details/goecmprxz.sHtML

[U11] Py：生成器表达式
来源：http://mobile.hesvh.cn/Article/details/gorznmzce.sHtML

(x * 2 for x in arr)
来源：http://read.share.hesvh.cn/Article/details/gtcubwzqi.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.zdbjq.cn/Article/details/gfefiomdw.sHtML

Counter(arr).most_common(3)
来源：http://m.share.zdbjq.cn/Article/details/geksabdaa.sHtML

[U13] Py：固定长度队列
来源：http://www.share.zdbjq.cn/Article/details/gbmujsdph.sHtML

deque(maxlen=10)
来源：http://3g.fehbvm.com/Article/details/gfwejtbyp.sHtML

[U14] Py：分组收集到列表
来源：http://blog.fehbvm.com/Article/details/gjppfvlda.sHtML

defaultdict(list)
来源：http://mobile.hesvh.cn/Article/details/gggoktbve.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.hesvh.cn/Article/details/gnheycybv.sHtML

t = time.perf_counter()
来源：http://wap.zdbjq.cn/Article/details/gvmztpmng.sHtML

[U16] Py：命令行参数解析
来源：http://wap.fehbvm.com/Article/details/gwvgmqmmf.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.zdbjq.cn/Article/details/gbuvkyjzu.sHtML

[U17] Py：初始化日志
来源：http://mobile.fehbvm.com/Article/details/gktilehej.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.hesvh.cn/Article/details/gukkajeiy.sHtML

[U18] Py：预编译正则
来源：http://mobile.fehbvm.com/Article/details/gznalileg.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.zdbjq.cn/Article/details/gsuqogvpr.sHtML

[U19] Py：正则替换带回调
来源：http://blog.zdbjq.cn/Article/details/gsjfvicvz.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.zdbjq.cn/Article/details/gevzjirwi.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.fehbvm.com/Article/details/glkyfikbu.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.hesvh.cn/Article/details/gwknthgww.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.fehbvm.com/Article/details/gpdwjtauj.sHtML

@contextlib.contextmanager
来源：http://www.share.fehbvm.com/Article/details/gapicngiw.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.fehbvm.com/Article/details/glsaptjis.sHtML

list(zip(*m))
来源：http://blog.fehbvm.com/Article/details/ggtezevvs.sHtML

[U23] Py：分块读取大文件
来源：http://baike.zdbjq.cn/Article/details/gvbclmril.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.fehbvm.com/Article/details/grkzqzrpz.sHtML

[U24] Py：路径操作
来源：http://read.share.zdbjq.cn/Article/details/gzurhqans.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.hesvh.cn/Article/details/glgwlzmzd.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.hesvh.cn/Article/details/gnmlyuiwt.sHtML

csv.DictReader(f)
来源：http://www.m.share.hesvh.cn/Article/details/gbtqytkat.sHtML

[U26] Py：并发下载
来源：http://read.share.zdbjq.cn/Article/details/gseildwxg.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.hesvh.cn/Article/details/gbfgqlgdf.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.hesvh.cn/Article/details/gkuaawtja.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.zdbjq.cn/Article/details/gnmnjbeiu.sHtML

[U28] Py：类型别名
来源：http://m.share.fehbvm.com/Article/details/gdlgozvxg.sHtML

UserId = int
来源：http://wap.zdbjq.cn/Article/details/gkdhvzqln.sHtML

[U29] Py：属性校验
来源：http://www.blog.zdbjq.cn/Article/details/gjchpiqwm.sHtML

@property 与 @x.setter 配合
来源：http://read.share.fehbvm.com/Article/details/gklohgnxg.sHtML

[U30] Py：数据类
来源：http://blog.fehbvm.com/Article/details/gaqiftyhe.sHtML

@dataclass(slots=True)
来源：http://www.share.hesvh.cn/Article/details/glvpgjliz.sHtML

[U31] Py：单测
来源：http://wap.hesvh.cn/Article/details/gqlflxoaf.sHtML

python -m pytest -q
来源：http://www.m.share.fehbvm.com/Article/details/gzeihepwg.sHtML

[U32] Py：代码格式化
来源：http://www.share.fehbvm.com/Article/details/gigfxsiql.sHtML

ruff format . && ruff check --fix .
来源：http://baike.hesvh.cn/Article/details/gbrxkmqcw.sHtML

[U33] Py：打包发布
来源：http://m.share.fehbvm.com/Article/details/gaqeubdwy.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.zdbjq.cn/Article/details/gapuxekwl.sHtML

[U34] Py：判断编码
来源：http://read.share.hesvh.cn/Article/details/gfuuszdvf.sHtML

chardet.detect(raw)
来源：http://3g.fehbvm.com/Article/details/gxctoqrgt.sHtML

[U35] Py：发送邮件
来源：http://m.share.fehbvm.com/Article/details/gywrafwpn.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.hesvh.cn/Article/details/gfczieevs.sHtML

[U36] Py：定时任务
来源：http://baike.fehbvm.com/Article/details/gdtonhbwm.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.fehbvm.com/Article/details/giuufjoot.sHtML

[U37] Py：读写 Excel
来源：http://baike.fehbvm.com/Article/details/gpnpddduj.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.zdbjq.cn/Article/details/ggzyddkxj.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.hesvh.cn/Article/details/gwthevuhu.sHtML

Path(__file__).resolve().parent
来源：http://mobile.hesvh.cn/Article/details/gsloffuuz.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.hesvh.cn/Article/details/gcrzvbzib.sHtML

sys.stdout.isatty()
来源：http://read.share.hesvh.cn/Article/details/gjmghpcif.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.zdbjq.cn/Article/details/glgeqhnqt.sHtML

print("err", file=sys.stderr)
来源：http://baike.fehbvm.com/Article/details/gbgbgduvk.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.zdbjq.cn/Article/details/gyyrfxfwi.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.zdbjq.cn/Article/details/ghuvedgmz.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.hesvh.cn/Article/details/gchdkagbz.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.hesvh.cn/Article/details/ghlqaryfi.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.fehbvm.com/Article/details/geaebtlpn.sHtML

namespace App\Http;
来源：http://blog.hesvh.cn/Article/details/grzaecwel.sHtML

[U44] PHP：开启严格类型
来源：http://3g.fehbvm.com/Article/details/ginehhega.sHtML

declare(strict_types=1);
来源：http://3g.hesvh.cn/Article/details/gfnuujzzk.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.hesvh.cn/Article/details/gpynzulut.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gijhgicrq.sHtML

[U46] PHP：可空类型
来源：http://read.share.hesvh.cn/Article/details/guzqhllbw.sHtML

?string $name = null
来源：http://www.share.fehbvm.com/Article/details/gmdksajam.sHtML

[U47] PHP：联合类型
来源：http://3g.zdbjq.cn/Article/details/gclaleyka.sHtML

int|string $id
来源：http://read.share.zdbjq.cn/Article/details/goglxgsol.sHtML

[U48] PHP：纯枚举
来源：http://wap.fehbvm.com/Article/details/gxnovarft.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.zdbjq.cn/Article/details/gicsfcybd.sHtML

[U49] PHP：只读属性
来源：http://blog.zdbjq.cn/Article/details/gbntyaorm.sHtML

public readonly string $name
来源：http://www.blog.hesvh.cn/Article/details/gfieeqtsn.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.hesvh.cn/Article/details/gxzmxwsfu.sHtML

public function __construct(private int $id) {}
来源：http://read.share.zdbjq.cn/Article/details/gbhqmrtqa.sHtML

[U51] PHP：数组解构
来源：http://baike.zdbjq.cn/Article/details/gjuygbsjo.sHtML

[$a, $b] = $arr;
来源：http://www.share.fehbvm.com/Article/details/gyqfnhtnx.sHtML

[U52] PHP：箭头函数
来源：http://wap.zdbjq.cn/Article/details/gpcycestd.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.hesvh.cn/Article/details/gjqntcxfz.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.hesvh.cn/Article/details/grnlsonyx.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.fehbvm.com/Article/details/giesmbfkr.sHtML

[U54] PHP：空安全调用
来源：http://mobile.fehbvm.com/Article/details/gkxggnivp.sHtML

$obj?->method()
来源：http://www.blog.zdbjq.cn/Article/details/gjlcntabx.sHtML

[U55] PHP：match 表达式
来源：http://mobile.hesvh.cn/Article/details/garycvuul.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.zdbjq.cn/Article/details/gsrxwjzmp.sHtML

[U56] PHP：命名参数
来源：http://read.share.fehbvm.com/Article/details/govutzcxq.sHtML

f(a: 1, b: 2)
来源：http://3g.zdbjq.cn/Article/details/ghgyzstel.sHtML

[U57] PHP：字符串插值
来源：http://wap.fehbvm.com/Article/details/gszkpdisg.sHtML

"值: {$a}"
来源：http://wap.fehbvm.com/Article/details/gzuhgwkgn.sHtML

[U58] PHP：数组三件套
来源：http://m.share.hesvh.cn/Article/details/gnpzugaxc.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.zdbjq.cn/Article/details/gbslcvdrv.sHtML

[U59] PHP：自定义排序
来源：http://3g.fehbvm.com/Article/details/gchxvkldf.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.hesvh.cn/Article/details/gpaeruotk.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.zdbjq.cn/Article/details/gutdwqfpe.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.fehbvm.com/Article/details/gxglyqbgd.sHtML

[U61] PHP：正则
来源：http://m.share.zdbjq.cn/Article/details/gbxjjvpeq.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.fehbvm.com/Article/details/gexozltlh.sHtML

[U62] PHP：日期对象
来源：http://3g.fehbvm.com/Article/details/geuhudlbt.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.zdbjq.cn/Article/details/gfrhbagkl.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.zdbjq.cn/Article/details/gqoykmpks.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.hesvh.cn/Article/details/gdftjsldr.sHtML

[U64] PHP：目录遍历
来源：http://blog.fehbvm.com/Article/details/gaptnumam.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.zdbjq.cn/Article/details/gpepmfytb.sHtML

[U65] PHP：会话
来源：http://www.blog.hesvh.cn/Article/details/gkdsfwjbe.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.hesvh.cn/Article/details/glmklqudx.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.fehbvm.com/Article/details/glfomzekk.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.fehbvm.com/Article/details/ghitqebhz.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.fehbvm.com/Article/details/ghzoeruft.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.hesvh.cn/Article/details/grjlrvbfb.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.fehbvm.com/Article/details/gzfoonpyf.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.fehbvm.com/Article/details/gqeldmnci.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.fehbvm.com/Article/details/gucxggjgg.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.zdbjq.cn/Article/details/gixzgkjxf.sHtML

[U70] PHP：PDO 事务
来源：http://3g.hesvh.cn/Article/details/gezisegec.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.hesvh.cn/Article/details/glmaundoh.sHtML

[U71] PHP：抛出异常
来源：http://mobile.fehbvm.com/Article/details/giuehcchz.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.fehbvm.com/Article/details/gsldwnddm.sHtML

[U72] PHP：写错误日志
来源：http://mobile.zdbjq.cn/Article/details/gpakabusx.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.hesvh.cn/Article/details/gedwpdfaw.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.hesvh.cn/Article/details/gouxgcsxs.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.zdbjq.cn/Article/details/gohalavte.sHtML

[U74] PHP：读取环境变量
来源：http://wap.fehbvm.com/Article/details/gxqkjgmrm.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.zdbjq.cn/Article/details/gnnunncus.sHtML

[U75] PHP：依赖注入
来源：http://www.share.hesvh.cn/Article/details/gkquhiyhz.sHtML

composer require psr/container
来源：http://baike.zdbjq.cn/Article/details/ggftbexvk.sHtML

[U76] PHP：简单路由
来源：http://www.share.hesvh.cn/Article/details/grcetfhpa.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.zdbjq.cn/Article/details/gkqawiymw.sHtML

[U77] PHP：模板渲染
来源：http://3g.hesvh.cn/Article/details/glgehpark.sHtML

composer require twig/twig
来源：http://blog.fehbvm.com/Article/details/gsqzsdbme.sHtML

[U78] PHP：单元测试
来源：http://3g.zdbjq.cn/Article/details/gqmcemyud.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.hesvh.cn/Article/details/gzmldzsyo.sHtML

[U79] PHP：静态分析
来源：http://blog.fehbvm.com/Article/details/gnspgollt.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.fehbvm.com/Article/details/gpsmseaeg.sHtML

[U80] PHP：代码规范修复
来源：http://blog.hesvh.cn/Article/details/gcgdshjiu.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.hesvh.cn/Article/details/gwwvzlbmv.sHtML

[U81] JS：初始化项目
来源：http://mobile.fehbvm.com/Article/details/gymcervdp.sHtML

npm init -y;  npm i express
来源：http://www.m.share.fehbvm.com/Article/details/gwghnzojk.sHtML

[U82] JS：package.json 脚本
来源：http://3g.fehbvm.com/Article/details/gqwyydedo.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.fehbvm.com/Article/details/gebfslsvb.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.hesvh.cn/Article/details/gbmoayeos.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.zdbjq.cn/Article/details/gxpclcncq.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.fehbvm.com/Article/details/gldlhtddf.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.hesvh.cn/Article/details/gosmfjvzi.sHtML

[U85] JS：可选链
来源：http://m.share.hesvh.cn/Article/details/gajeiworu.sHtML

a?.b?.c
来源：http://m.share.hesvh.cn/Article/details/glhajgjyj.sHtML

[U86] JS：空值合并
来源：http://www.share.zdbjq.cn/Article/details/gnwywtkjx.sHtML

a ?? b
来源：http://www.m.share.hesvh.cn/Article/details/guzdksuea.sHtML

[U87] JS：解构默认值
来源：http://blog.zdbjq.cn/Article/details/gznuhpmdf.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.hesvh.cn/Article/details/gbmikvklw.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.zdbjq.cn/Article/details/ghhvckluq.sHtML

{ ...a, ...b }
来源：http://m.share.zdbjq.cn/Article/details/gxdabrpea.sHtML

[U89] JS：数组去重
来源：http://blog.fehbvm.com/Article/details/gaxvmaxgh.sHtML

[...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/grsxbxlra.sHtML

[U90] JS：数字数组排序
来源：http://baike.fehbvm.com/Article/details/gdalcszne.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/geqvqwvra.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.fehbvm.com/Article/details/gwcrqkzhp.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.zdbjq.cn/Article/details/grlxdkosb.sHtML

[U92] JS：深拷贝
来源：http://wap.zdbjq.cn/Article/details/gyqhccbio.sHtML

structuredClone(obj)
来源：http://www.share.hesvh.cn/Article/details/gaxhgdslh.sHtML

[U93] JS：模板字符串
来源：http://read.share.fehbvm.com/Article/details/gvkqgfggt.sHtML

`共 ${n} 条`
来源：http://www.m.share.fehbvm.com/Article/details/gbdgrtewn.sHtML

[U94] JS：箭头函数
来源：http://www.share.fehbvm.com/Article/details/gpbtoboqu.sHtML

const double = x => x * 2;
来源：http://blog.fehbvm.com/Article/details/gmgspiwyr.sHtML

[U95] JS：Promise 包装
来源：http://read.share.hesvh.cn/Article/details/gfyjvbmzj.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.zdbjq.cn/Article/details/gwymktcyy.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.hesvh.cn/Article/details/gplbuemwu.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gmgulgtrc.sHtML

[U97] JS：并发请求
来源：http://read.share.fehbvm.com/Article/details/ghotuazyw.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gaqkzelmr.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.fehbvm.com/Article/details/gwysftrqd.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.hesvh.cn/Article/details/gasubrale.sHtML

[U99] JS：事件监听
来源：http://blog.fehbvm.com/Article/details/gbdsmnfrx.sHtML

el.addEventListener("click", e => {})
来源：http://blog.zdbjq.cn/Article/details/glxnolfcx.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.fehbvm.com/Article/details/gwmxqttwf.sHtML

document.querySelector(".item")
来源：http://www.share.hesvh.cn/Article/details/gsmylmefd.sHtML

[U101] JS：classList 操作
来源：http://blog.fehbvm.com/Article/details/gptqdfdnc.sHtML

el.classList.toggle("active")
来源：http://blog.fehbvm.com/Article/details/gtxkaieea.sHtML

[U102] JS：本地存储
来源：http://www.share.hesvh.cn/Article/details/gwpjpujpv.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.zdbjq.cn/Article/details/gyrnzblqb.sHtML

[U103] JS：定时器
来源：http://wap.hesvh.cn/Article/details/gsleoowpr.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.zdbjq.cn/Article/details/gcagorlxf.sHtML

[U104] JS：防抖
来源：http://wap.hesvh.cn/Article/details/griioxhvy.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/gszqpswxn.sHtML

[U105] JS：节流
来源：http://www.m.share.fehbvm.com/Article/details/gbtgnxkdm.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.fehbvm.com/Article/details/gryefujhv.sHtML

[U106] JS：日期格式化
来源：http://3g.zdbjq.cn/Article/details/gwrpzjifg.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.fehbvm.com/Article/details/gmtaqxswh.sHtML

[U107] JS：数字千分位
来源：http://www.share.fehbvm.com/Article/details/gskrgfkwt.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.zdbjq.cn/Article/details/gsytpprbq.sHtML

[U108] JS：随机整数
来源：http://3g.zdbjq.cn/Article/details/gmeqyyfwc.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.zdbjq.cn/Article/details/gqbcirfis.sHtML

[U109] JS：数组分组
来源：http://read.share.fehbvm.com/Article/details/gzdgsyrng.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.fehbvm.com/Article/details/ghkzwdroz.sHtML

[U110] JS：数组分块
来源：http://www.share.zdbjq.cn/Article/details/gyhaacmhz.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.fehbvm.com/Article/details/gvtehpurq.sHtML

[U111] JS：对象转 Map
来源：http://mobile.fehbvm.com/Article/details/gpmawutov.sHtML

new Map(Object.entries(obj))
来源：http://baike.fehbvm.com/Article/details/ggrfdiace.sHtML

[U112] JS：字符串补位
来源：http://read.share.zdbjq.cn/Article/details/gupnnwoxa.sHtML

"7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gfxpeizpx.sHtML

[U113] JS：正则替换全部
来源：http://m.share.zdbjq.cn/Article/details/gejpbbkcg.sHtML

s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gvgirzaqa.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.zdbjq.cn/Article/details/gwqxkqvnd.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gkkmpwhli.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.zdbjq.cn/Article/details/gfwspmkii.sHtML

crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gvdenhdls.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.fehbvm.com/Article/details/gooxdrlld.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gxyiklgrl.sHtML

[U117] JS：单元测试
来源：http://blog.fehbvm.com/Article/details/gbibdwokq.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.zdbjq.cn/Article/details/gmyuuzxau.sHtML

[U118] JS：开发服务器
来源：http://3g.hesvh.cn/Article/details/gmzpuvffe.sHtML

npm i -D vite;  npx vite
来源：http://baike.hesvh.cn/Article/details/ggfoffuot.sHtML

[U119] JS：生产构建
来源：http://m.share.hesvh.cn/Article/details/gcrgrjjay.sHtML

npx vite build
来源：http://baike.hesvh.cn/Article/details/gngxnqiqt.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.hesvh.cn/Article/details/gebxqrjoe.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.zdbjq.cn/Article/details/gxpsuvylv.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gbldpgtnx.sHtML

统计汇总
来源：http://read.share.hesvh.cn/Article/details/gnjmpfoxh.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gakhjltgx.sHtML

按语言统计（条）：
来源：http://www.m.share.zdbjq.cn/Article/details/guuammrao.sHtML

Python ......... 252
来源：http://read.share.fehbvm.com/Article/details/gkcpinyyi.sHtML

PHP ............ 252
来源：http://mobile.fehbvm.com/Article/details/gbjfidkpz.sHtML

JavaScript ..... 252
来源：http://wap.zdbjq.cn/Article/details/gyqzzigai.sHtML

TypeScript ..... 212
来源：http://www.blog.hesvh.cn/Article/details/gdguswrgn.sHtML

Java ........... 212
来源：http://mobile.zdbjq.cn/Article/details/gvcnojegy.sHtML

Go ............. 212
来源：http://baike.fehbvm.com/Article/details/gnifphgem.sHtML

Ruby ........... 212
来源：http://m.share.fehbvm.com/Article/details/gatleehyb.sHtML

C# ............. 212
来源：http://wap.hesvh.cn/Article/details/gwqhksbmy.sHtML

C .............. 30
来源：http://blog.hesvh.cn/Article/details/giggcagaf.sHtML

C++ ............ 30
来源：http://read.share.fehbvm.com/Article/details/gkmshwiyu.sHtML

SQL ............ 90
来源：http://www.blog.zdbjq.cn/Article/details/gqcmbmhnc.sHtML

Bash ........... 80
来源：http://www.blog.hesvh.cn/Article/details/gmwyoplce.sHtML

Kotlin ......... 15
来源：http://www.m.share.hesvh.cn/Article/details/gzlojzvrp.sHtML

Swift .......... 15
来源：http://www.share.fehbvm.com/Article/details/gschdquvn.sHtML

Lua ............ 10
来源：http://www.share.zdbjq.cn/Article/details/glwfotqll.sHtML

Perl ........... 10
来源：http://m.share.zdbjq.cn/Article/details/gtpnfmmhq.sHtML

Scala .......... 10
来源：http://mobile.zdbjq.cn/Article/details/gtzbedxuf.sHtML

------------------------------------
来源：http://mobile.hesvh.cn/Article/details/givyybsrk.sHtML

合计 ........... 2106 条
来源：http://www.share.zdbjq.cn/Article/details/gntrgvljw.sHtML

按章节统计：
来源：http://www.m.share.fehbvm.com/Article/details/glwmnzisy.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.hesvh.cn/Article/details/gcvzcpdff.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/gwqaalmjm.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.hesvh.cn/Article/details/ggefvrviw.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.fehbvm.com/Article/details/gfhdnsrjt.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.zdbjq.cn/Article/details/gaobhpnus.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.zdbjq.cn/Article/details/gdzxsnrwi.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/gtrkscbia.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.fehbvm.com/Article/details/gyfazsagd.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gbmuhvdeb.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.fehbvm.com/Article/details/gxowngapi.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gccwzmrbj.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gzjetvysy.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gblsxpksu.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.hesvh.cn/Article/details/gnzlilqnn.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.fehbvm.com/Article/details/gzbuqbcjg.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gmgfekjym.sHtML

Q SQL 专题                              90
来源：http://www.blog.hesvh.cn/Article/details/guwynkcsv.sHtML

R Bash 专题                             80
来源：http://m.share.fehbvm.com/Article/details/gpfilcbao.sHtML

S C / C++ 专题                          60
来源：http://mobile.zdbjq.cn/Article/details/goykvorcg.sHtML

T 其他语言补充                          60
来源：http://mobile.fehbvm.com/Article/details/glririvkk.sHtML

U 高频实用片段                         120
来源：http://www.m.share.hesvh.cn/Article/details/gmihyjdlf.sHtML

------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gqmbqkmsz.sHtML

合计                                  2106 条
来源：http://read.share.fehbvm.com/Article/details/gtjsguqea.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gybxgzlpa.sHtML

使用提醒
来源：http://mobile.fehbvm.com/Article/details/gfipibzoh.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gqmabzngn.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.hesvh.cn/Article/details/gbtvhqrca.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.hesvh.cn/Article/details/gceqedulv.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.zdbjq.cn/Article/details/gcpkxgown.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.zdbjq.cn/Article/details/gobqmeppw.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.hesvh.cn/Article/details/grdsqqtqe.sHtML

—— 文件结束 ——
来源：http://3g.fehbvm.com/Article/details/gowzwbnvm.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/goejfqgba.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.fehbvm.com/Article/details/gxnexvgej.sHtML

Common Programming Examples Cheat Book
来源：http://wap.hesvh.cn/Article/details/gsgspunbm.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ggukabetq.sHtML


<!-- 参考信息 -->