代发 wailian999

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.hesvh.cn/Article/details/gffvaxyjp.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gshjludcs.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.zdbjq.cn/Article/details/glrirtvax.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gnkyvbhsm.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.fehbvm.com/Article/details/ggjcukuvf.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.hesvh.cn/Article/details/gxudnycuz.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.hesvh.cn/Article/details/gqmusczxu.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.fehbvm.com/Article/details/gubyvrsjt.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.fehbvm.com/Article/details/ghrpxbvsd.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.fehbvm.com/Article/details/gutkczmxm.sHtML

[U04] Py：变量调试打印
来源：http://baike.hesvh.cn/Article/details/gsaqitpvh.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fehbvm.com/Article/details/gcwgfgzhx.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.hesvh.cn/Article/details/gzdatmygf.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.zdbjq.cn/Article/details/gbfiqjuwx.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.fehbvm.com/Article/details/gshljrfae.sHtML

{**a, **b}
来源：http://mobile.zdbjq.cn/Article/details/gfckxrmvy.sHtML

[U07] Py：反转字典键值
来源：http://read.share.zdbjq.cn/Article/details/grmwbriug.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.zdbjq.cn/Article/details/gcwboyozh.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.fehbvm.com/Article/details/gxoqmbrvn.sHtML

[y for x in nested for y in x]
来源：http://read.share.fehbvm.com/Article/details/gpfclcxri.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.fehbvm.com/Article/details/gdzytysze.sHtML

max(d, key=d.get)
来源：http://mobile.fehbvm.com/Article/details/gophmvafy.sHtML

[U10] Py：按值排序字典
来源：http://www.share.hesvh.cn/Article/details/gqigropwo.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.fehbvm.com/Article/details/gxcpmwuwc.sHtML

[U11] Py：生成器表达式
来源：http://mobile.fehbvm.com/Article/details/ghqbhgyyy.sHtML

(x * 2 for x in arr)
来源：http://baike.hesvh.cn/Article/details/guyhasuzb.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.fehbvm.com/Article/details/gqnirmlem.sHtML

Counter(arr).most_common(3)
来源：http://read.share.zdbjq.cn/Article/details/ggwrkoabl.sHtML

[U13] Py：固定长度队列
来源：http://blog.zdbjq.cn/Article/details/ghckfxscg.sHtML

deque(maxlen=10)
来源：http://wap.hesvh.cn/Article/details/ggknnlutu.sHtML

[U14] Py：分组收集到列表
来源：http://baike.fehbvm.com/Article/details/guuyqyije.sHtML

defaultdict(list)
来源：http://www.m.share.zdbjq.cn/Article/details/ghvmbexkb.sHtML

[U15] Py：高精度计时
来源：http://baike.hesvh.cn/Article/details/gnzwyqpvx.sHtML

t = time.perf_counter()
来源：http://mobile.zdbjq.cn/Article/details/gqewrfvxz.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.zdbjq.cn/Article/details/gdjhkmtrm.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.zdbjq.cn/Article/details/gngazcmkk.sHtML

[U17] Py：初始化日志
来源：http://read.share.fehbvm.com/Article/details/gkgkebhnz.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.fehbvm.com/Article/details/gpnmzwhyc.sHtML

[U18] Py：预编译正则
来源：http://blog.fehbvm.com/Article/details/gfscsrlkv.sHtML

pat = re.compile(r"\d+")
来源：http://baike.zdbjq.cn/Article/details/gtzucfgmn.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.hesvh.cn/Article/details/gfsadvoea.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.zdbjq.cn/Article/details/guzxwtqmi.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.zdbjq.cn/Article/details/gxswweliw.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.fehbvm.com/Article/details/gmdihnkwh.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.hesvh.cn/Article/details/gnogfnafl.sHtML

@contextlib.contextmanager
来源：http://blog.hesvh.cn/Article/details/gdglgvksn.sHtML

[U22] Py：矩阵转置
来源：http://wap.hesvh.cn/Article/details/gckryidzh.sHtML

list(zip(*m))
来源：http://read.share.fehbvm.com/Article/details/gqjnlbksf.sHtML

[U23] Py：分块读取大文件
来源：http://blog.fehbvm.com/Article/details/gaaigldpa.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.hesvh.cn/Article/details/gbiyopoqy.sHtML

[U24] Py：路径操作
来源：http://www.share.hesvh.cn/Article/details/gatzvwqpt.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.zdbjq.cn/Article/details/gpwddbhpd.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.fehbvm.com/Article/details/gjyrrlaap.sHtML

csv.DictReader(f)
来源：http://www.blog.fehbvm.com/Article/details/gargbrali.sHtML

[U26] Py：并发下载
来源：http://www.share.zdbjq.cn/Article/details/gttrgjfdj.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.hesvh.cn/Article/details/ghuaiffeh.sHtML

[U27] Py：异步 HTTP
来源：http://3g.fehbvm.com/Article/details/gxyfnayav.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.zdbjq.cn/Article/details/gqoyvrkdt.sHtML

[U28] Py：类型别名
来源：http://mobile.zdbjq.cn/Article/details/gebdghrwj.sHtML

UserId = int
来源：http://www.m.share.fehbvm.com/Article/details/gcqfygbdn.sHtML

[U29] Py：属性校验
来源：http://www.blog.zdbjq.cn/Article/details/gywqudora.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.hesvh.cn/Article/details/gbvhhfvsh.sHtML

[U30] Py：数据类
来源：http://blog.fehbvm.com/Article/details/gwgjbdsyj.sHtML

@dataclass(slots=True)
来源：http://blog.fehbvm.com/Article/details/gxnymhcdo.sHtML

[U31] Py：单测
来源：http://mobile.hesvh.cn/Article/details/gbmuswaaf.sHtML

python -m pytest -q
来源：http://mobile.zdbjq.cn/Article/details/gaaultruq.sHtML

[U32] Py：代码格式化
来源：http://mobile.fehbvm.com/Article/details/gbeuyvush.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.hesvh.cn/Article/details/gujxypehm.sHtML

[U33] Py：打包发布
来源：http://3g.hesvh.cn/Article/details/gcacvmmsh.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.zdbjq.cn/Article/details/gutpwspjy.sHtML

[U34] Py：判断编码
来源：http://read.share.fehbvm.com/Article/details/gfgazzttu.sHtML

chardet.detect(raw)
来源：http://www.share.zdbjq.cn/Article/details/gvtinzuyw.sHtML

[U35] Py：发送邮件
来源：http://blog.hesvh.cn/Article/details/gvuubtpnl.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.fehbvm.com/Article/details/gnimzoziu.sHtML

[U36] Py：定时任务
来源：http://read.share.hesvh.cn/Article/details/gsgddklkd.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.zdbjq.cn/Article/details/gibketicf.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.fehbvm.com/Article/details/gtbnhctub.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.zdbjq.cn/Article/details/gzambdzor.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.hesvh.cn/Article/details/gnbpvggtk.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.zdbjq.cn/Article/details/gyxfhsoql.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.fehbvm.com/Article/details/ghxxbvacj.sHtML

sys.stdout.isatty()
来源：http://wap.hesvh.cn/Article/details/gfolmulou.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.hesvh.cn/Article/details/gqelmldnd.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.fehbvm.com/Article/details/gzgjjycwv.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.zdbjq.cn/Article/details/ghudywblt.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.hesvh.cn/Article/details/gegsrirem.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.zdbjq.cn/Article/details/gqbncyenh.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.fehbvm.com/Article/details/gdhifwerh.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.hesvh.cn/Article/details/gbfrvvgrf.sHtML

namespace App\Http;
来源：http://m.share.hesvh.cn/Article/details/ggvlmoyma.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.zdbjq.cn/Article/details/ggzyzrotc.sHtML

declare(strict_types=1);
来源：http://baike.hesvh.cn/Article/details/gvllzrqth.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.hesvh.cn/Article/details/gcowmaesd.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gcwmtczui.sHtML

[U46] PHP：可空类型
来源：http://m.share.fehbvm.com/Article/details/gfrmjbltg.sHtML

?string $name = null
来源：http://www.m.share.zdbjq.cn/Article/details/gerzhickh.sHtML

[U47] PHP：联合类型
来源：http://blog.zdbjq.cn/Article/details/gitybmykf.sHtML

int|string $id
来源：http://www.share.zdbjq.cn/Article/details/gbcjreyjr.sHtML

[U48] PHP：纯枚举
来源：http://baike.fehbvm.com/Article/details/gbyfwwmle.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.zdbjq.cn/Article/details/gpspjhcgq.sHtML

[U49] PHP：只读属性
来源：http://baike.fehbvm.com/Article/details/gwbrjxfoy.sHtML

public readonly string $name
来源：http://mobile.fehbvm.com/Article/details/gvhunzrlq.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.fehbvm.com/Article/details/gpnedtqyf.sHtML

public function __construct(private int $id) {}
来源：http://blog.hesvh.cn/Article/details/gpjqhoymo.sHtML

[U51] PHP：数组解构
来源：http://blog.zdbjq.cn/Article/details/gulvhzeqw.sHtML

[$a, $b] = $arr;
来源：http://read.share.hesvh.cn/Article/details/guvnafgat.sHtML

[U52] PHP：箭头函数
来源：http://baike.hesvh.cn/Article/details/gljjhciak.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.hesvh.cn/Article/details/gaadxeyed.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.zdbjq.cn/Article/details/ggbgctohi.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.hesvh.cn/Article/details/gfjghswup.sHtML

[U54] PHP：空安全调用
来源：http://3g.zdbjq.cn/Article/details/gclrbiktm.sHtML

$obj?->method()
来源：http://m.share.fehbvm.com/Article/details/gtlbzopib.sHtML

[U55] PHP：match 表达式
来源：http://wap.hesvh.cn/Article/details/gvlpcelnq.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.fehbvm.com/Article/details/gsezukwss.sHtML

[U56] PHP：命名参数
来源：http://mobile.hesvh.cn/Article/details/gjiirhdnu.sHtML

f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/gfloaoqmt.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gmhcqrpgn.sHtML

"值: {$a}"
来源：http://www.blog.fehbvm.com/Article/details/gxgwcrxpn.sHtML

[U58] PHP：数组三件套
来源：http://3g.hesvh.cn/Article/details/gqejmwxju.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.hesvh.cn/Article/details/gipdljbti.sHtML

[U59] PHP：自定义排序
来源：http://wap.hesvh.cn/Article/details/gufxomkwf.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.hesvh.cn/Article/details/gombwuilj.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.zdbjq.cn/Article/details/gapzcazmj.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.zdbjq.cn/Article/details/gtgoyfcly.sHtML

[U61] PHP：正则
来源：http://read.share.fehbvm.com/Article/details/gcazmtqor.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.hesvh.cn/Article/details/gzzeprhbv.sHtML

[U62] PHP：日期对象
来源：http://read.share.fehbvm.com/Article/details/gasvzdaag.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.zdbjq.cn/Article/details/gulcgqrel.sHtML

[U63] PHP：文件读写
来源：http://3g.zdbjq.cn/Article/details/gzrwgkjre.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.zdbjq.cn/Article/details/gopnfkjcu.sHtML

[U64] PHP：目录遍历
来源：http://baike.hesvh.cn/Article/details/gnriexwgu.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.fehbvm.com/Article/details/gxcbddizh.sHtML

[U65] PHP：会话
来源：http://read.share.fehbvm.com/Article/details/gvhlnuomq.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.hesvh.cn/Article/details/gbymmzmek.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.zdbjq.cn/Article/details/gtzjbkfxo.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.fehbvm.com/Article/details/gsovmqxeu.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.zdbjq.cn/Article/details/gwybtlpbm.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.hesvh.cn/Article/details/ggbpiqtmo.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.fehbvm.com/Article/details/giuywoizf.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.zdbjq.cn/Article/details/gcsmukzgg.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.hesvh.cn/Article/details/gkkvxugmx.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.hesvh.cn/Article/details/gqhxkkssh.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.zdbjq.cn/Article/details/gkkosvaiz.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.fehbvm.com/Article/details/gixrtmkbv.sHtML

[U71] PHP：抛出异常
来源：http://mobile.zdbjq.cn/Article/details/gpbjugnpl.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.hesvh.cn/Article/details/grtaljsjo.sHtML

[U72] PHP：写错误日志
来源：http://m.share.fehbvm.com/Article/details/gzzlwvrmi.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.hesvh.cn/Article/details/ghdeacfjh.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.fehbvm.com/Article/details/ghaqtucjg.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.zdbjq.cn/Article/details/gdmynnohc.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.fehbvm.com/Article/details/gokiifvna.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.zdbjq.cn/Article/details/gbumfurxf.sHtML

[U75] PHP：依赖注入
来源：http://mobile.hesvh.cn/Article/details/gdtvrgtoj.sHtML

composer require psr/container
来源：http://wap.hesvh.cn/Article/details/gwazmvkjv.sHtML

[U76] PHP：简单路由
来源：http://mobile.fehbvm.com/Article/details/gpqgcftkm.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.zdbjq.cn/Article/details/gcyzlvwjq.sHtML

[U77] PHP：模板渲染
来源：http://mobile.zdbjq.cn/Article/details/gwqndyyis.sHtML

composer require twig/twig
来源：http://read.share.zdbjq.cn/Article/details/gijodxstk.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.fehbvm.com/Article/details/ghluteeoj.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.hesvh.cn/Article/details/gmcsmvtcd.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.hesvh.cn/Article/details/gtwxvrtdd.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.hesvh.cn/Article/details/gcvtsmbrt.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.zdbjq.cn/Article/details/gtwzcjgjq.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.zdbjq.cn/Article/details/gzvlrxfpy.sHtML

[U81] JS：初始化项目
来源：http://baike.fehbvm.com/Article/details/glcyizyzw.sHtML

npm init -y;  npm i express
来源：http://mobile.zdbjq.cn/Article/details/guysbyhfg.sHtML

[U82] JS：package.json 脚本
来源：http://blog.fehbvm.com/Article/details/gqvmmyjbg.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.zdbjq.cn/Article/details/gwgzsbdfa.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.fehbvm.com/Article/details/gpyydmdsm.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.hesvh.cn/Article/details/ghxtqkuvq.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.fehbvm.com/Article/details/gxwecziqp.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.zdbjq.cn/Article/details/gubvlmrsx.sHtML

[U85] JS：可选链
来源：http://blog.hesvh.cn/Article/details/gzexhnhrg.sHtML

a?.b?.c
来源：http://blog.fehbvm.com/Article/details/gzbkonfod.sHtML

[U86] JS：空值合并
来源：http://mobile.hesvh.cn/Article/details/gfrgjornj.sHtML

a ?? b
来源：http://www.m.share.zdbjq.cn/Article/details/gwvywifud.sHtML

[U87] JS：解构默认值
来源：http://3g.hesvh.cn/Article/details/guzuqwqiy.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.fehbvm.com/Article/details/gpzeokfaj.sHtML

[U88] JS：对象展开合并
来源：http://mobile.hesvh.cn/Article/details/gebuyqguu.sHtML

{ ...a, ...b }
来源：http://read.share.zdbjq.cn/Article/details/gnhwrgtnm.sHtML

[U89] JS：数组去重
来源：http://www.blog.hesvh.cn/Article/details/gqfnyzmfn.sHtML

[...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/gcocleobl.sHtML

[U90] JS：数字数组排序
来源：http://www.share.hesvh.cn/Article/details/gpaksmvim.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/glkdgrfub.sHtML

[U91] JS：对象键值遍历
来源：http://blog.fehbvm.com/Article/details/ghhosavga.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.fehbvm.com/Article/details/gfbmuznoz.sHtML

[U92] JS：深拷贝
来源：http://3g.hesvh.cn/Article/details/gddrgjhno.sHtML

structuredClone(obj)
来源：http://mobile.fehbvm.com/Article/details/ghgdbyglq.sHtML

[U93] JS：模板字符串
来源：http://blog.fehbvm.com/Article/details/gehzticrh.sHtML

`共 ${n} 条`
来源：http://mobile.hesvh.cn/Article/details/gbaqeheaf.sHtML

[U94] JS：箭头函数
来源：http://mobile.hesvh.cn/Article/details/gbvqnqjof.sHtML

const double = x => x * 2;
来源：http://wap.zdbjq.cn/Article/details/grrprmmhd.sHtML

[U95] JS：Promise 包装
来源：http://www.share.fehbvm.com/Article/details/gmeihexgm.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.fehbvm.com/Article/details/gghdnydsn.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.hesvh.cn/Article/details/gdluhsoww.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/gihzqiqts.sHtML

[U97] JS：并发请求
来源：http://read.share.fehbvm.com/Article/details/gytedtbnr.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/gxyaamzlb.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.hesvh.cn/Article/details/gxtrtfogr.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.hesvh.cn/Article/details/gvhurerdn.sHtML

[U99] JS：事件监听
来源：http://www.share.fehbvm.com/Article/details/gqcvpwsla.sHtML

el.addEventListener("click", e => {})
来源：http://baike.fehbvm.com/Article/details/gsnsugovh.sHtML

[U100] JS：DOM 查询
来源：http://wap.zdbjq.cn/Article/details/grnoldhap.sHtML

document.querySelector(".item")
来源：http://www.blog.hesvh.cn/Article/details/gzqkepads.sHtML

[U101] JS：classList 操作
来源：http://m.share.zdbjq.cn/Article/details/gnhvaxlxb.sHtML

el.classList.toggle("active")
来源：http://www.share.zdbjq.cn/Article/details/ggrukbjbq.sHtML

[U102] JS：本地存储
来源：http://blog.hesvh.cn/Article/details/gpcgicsew.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.fehbvm.com/Article/details/gbhgbxvnz.sHtML

[U103] JS：定时器
来源：http://blog.zdbjq.cn/Article/details/gvghnjgnm.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.fehbvm.com/Article/details/gftlnqtnb.sHtML

[U104] JS：防抖
来源：http://baike.zdbjq.cn/Article/details/gwoazxfie.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/ghslhmiyu.sHtML

[U105] JS：节流
来源：http://wap.hesvh.cn/Article/details/gpoojgkqn.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.zdbjq.cn/Article/details/gafwqzdcp.sHtML

[U106] JS：日期格式化
来源：http://baike.fehbvm.com/Article/details/glmwlpgnt.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.zdbjq.cn/Article/details/gzzuhdicz.sHtML

[U107] JS：数字千分位
来源：http://read.share.zdbjq.cn/Article/details/gddpmpkvd.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.fehbvm.com/Article/details/gdkuntiog.sHtML

[U108] JS：随机整数
来源：http://mobile.zdbjq.cn/Article/details/gpuxjumbl.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.zdbjq.cn/Article/details/gotajvptw.sHtML

[U109] JS：数组分组
来源：http://blog.hesvh.cn/Article/details/gvuhuujzm.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.fehbvm.com/Article/details/gvinugxhk.sHtML

[U110] JS：数组分块
来源：http://m.share.hesvh.cn/Article/details/gklhevcki.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.fehbvm.com/Article/details/ghaxiaxfe.sHtML

[U111] JS：对象转 Map
来源：http://www.share.zdbjq.cn/Article/details/gkwfoehul.sHtML

new Map(Object.entries(obj))
来源：http://3g.hesvh.cn/Article/details/gaueagohk.sHtML

[U112] JS：字符串补位
来源：http://www.blog.fehbvm.com/Article/details/gnribjxwz.sHtML

"7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gduqfhsyi.sHtML

[U113] JS：正则替换全部
来源：http://blog.zdbjq.cn/Article/details/gwqpkepvo.sHtML

s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gwjpzuxfk.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.fehbvm.com/Article/details/gkovlhqmd.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fehbvm.com/Article/details/gfwbdqxln.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.hesvh.cn/Article/details/gieppoixw.sHtML

crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/gzsengxwz.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.hesvh.cn/Article/details/giylpluvc.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.zdbjq.cn/Article/details/getcpphzu.sHtML

[U117] JS：单元测试
来源：http://blog.zdbjq.cn/Article/details/grkmdjmuc.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.fehbvm.com/Article/details/gyukwieik.sHtML

[U118] JS：开发服务器
来源：http://baike.fehbvm.com/Article/details/giqvzbfbi.sHtML

npm i -D vite;  npx vite
来源：http://m.share.zdbjq.cn/Article/details/gyphzbbna.sHtML

[U119] JS：生产构建
来源：http://m.share.hesvh.cn/Article/details/gnilxnstw.sHtML

npx vite build
来源：http://www.share.zdbjq.cn/Article/details/gbnfvwncf.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.fehbvm.com/Article/details/gsckmzkqd.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.hesvh.cn/Article/details/gbjdhiqfm.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/graxrizpl.sHtML

统计汇总
来源：http://www.m.share.fehbvm.com/Article/details/gmszjconc.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gvqddshqy.sHtML

按语言统计（条）：
来源：http://baike.zdbjq.cn/Article/details/gkltxilwj.sHtML

Python ......... 252
来源：http://m.share.zdbjq.cn/Article/details/gnoxbwztg.sHtML

PHP ............ 252
来源：http://baike.zdbjq.cn/Article/details/gfizybmqa.sHtML

JavaScript ..... 252
来源：http://www.share.zdbjq.cn/Article/details/gbxvgrjnb.sHtML

TypeScript ..... 212
来源：http://wap.fehbvm.com/Article/details/gtkyzjcon.sHtML

Java ........... 212
来源：http://read.share.hesvh.cn/Article/details/grcxklhfc.sHtML

Go ............. 212
来源：http://mobile.hesvh.cn/Article/details/gyowvsuhv.sHtML

Ruby ........... 212
来源：http://blog.fehbvm.com/Article/details/gzqtkhcbh.sHtML

C# ............. 212
来源：http://www.blog.hesvh.cn/Article/details/gdkptfulk.sHtML

C .............. 30
来源：http://m.share.zdbjq.cn/Article/details/gkzotdqhd.sHtML

C++ ............ 30
来源：http://mobile.zdbjq.cn/Article/details/gtkmeynjb.sHtML

SQL ............ 90
来源：http://wap.hesvh.cn/Article/details/ghouddmrm.sHtML

Bash ........... 80
来源：http://baike.hesvh.cn/Article/details/ghdnljxgc.sHtML

Kotlin ......... 15
来源：http://read.share.fehbvm.com/Article/details/gwzbignjr.sHtML

Swift .......... 15
来源：http://mobile.zdbjq.cn/Article/details/gqhmlaoeo.sHtML

Lua ............ 10
来源：http://mobile.zdbjq.cn/Article/details/gcouxpjkf.sHtML

Perl ........... 10
来源：http://www.blog.hesvh.cn/Article/details/gbggibqhd.sHtML

Scala .......... 10
来源：http://m.share.zdbjq.cn/Article/details/gwswgqiaa.sHtML

------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gsgmcjrcq.sHtML

合计 ........... 2106 条
来源：http://www.m.share.zdbjq.cn/Article/details/gzrpfuxho.sHtML

按章节统计：
来源：http://read.share.zdbjq.cn/Article/details/gllafsosd.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.zdbjq.cn/Article/details/gbkzszrfb.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.hesvh.cn/Article/details/gjwbbsfrx.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.zdbjq.cn/Article/details/giwebfbcw.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.hesvh.cn/Article/details/gjzbtoffv.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.fehbvm.com/Article/details/gbavdfwgi.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.fehbvm.com/Article/details/gtwmnsqtf.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.fehbvm.com/Article/details/gzxkrobjz.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.hesvh.cn/Article/details/gfktsztgd.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gqomssguh.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.hesvh.cn/Article/details/gectssnbg.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gpabdbztb.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gjxctshtc.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gdjkurzsj.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.hesvh.cn/Article/details/gdakgidqb.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.zdbjq.cn/Article/details/gctlliimd.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/glxcctnwu.sHtML

Q SQL 专题                              90
来源：http://blog.hesvh.cn/Article/details/gwacnural.sHtML

R Bash 专题                             80
来源：http://www.blog.fehbvm.com/Article/details/gjwgltmaf.sHtML

S C / C++ 专题                          60
来源：http://read.share.zdbjq.cn/Article/details/gubdjqewh.sHtML

T 其他语言补充                          60
来源：http://wap.hesvh.cn/Article/details/glhecyvrf.sHtML

U 高频实用片段                         120
来源：http://www.m.share.hesvh.cn/Article/details/gmbhqtoaj.sHtML

------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gdavvtxxs.sHtML

合计                                  2106 条
来源：http://wap.fehbvm.com/Article/details/gzxqbpgex.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/gdxwyyouh.sHtML

使用提醒
来源：http://baike.hesvh.cn/Article/details/gambxzrfv.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/gudehcgvs.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.hesvh.cn/Article/details/gljddaqpn.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.hesvh.cn/Article/details/gwadymuuy.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.fehbvm.com/Article/details/gtrhltopa.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.fehbvm.com/Article/details/gzmhxztmq.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.hesvh.cn/Article/details/goeismnqx.sHtML

—— 文件结束 ——
来源：http://blog.hesvh.cn/Article/details/girzmsfei.sHtML


<!-- 参考信息 -->