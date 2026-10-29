代发 wailian999

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.fehbvm.com/Article/details/gpfjtzyzg.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gnuhiyqmn.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fehbvm.com/Article/details/gqmqarcrm.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gtjddyiyo.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.hesvh.cn/Article/details/gixnnuoip.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.zdbjq.cn/Article/details/gpuvyhksx.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.hesvh.cn/Article/details/grhjcfott.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.hesvh.cn/Article/details/gdjklnrfb.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.hesvh.cn/Article/details/gjjjmgklq.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.zdbjq.cn/Article/details/gkafxxuht.sHtML

[U04] Py：变量调试打印
来源：http://blog.hesvh.cn/Article/details/gdolutddz.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.hesvh.cn/Article/details/gwlvuhzbw.sHtML

[U05] Py：列表去重且保序
来源：http://blog.zdbjq.cn/Article/details/ggtdivqil.sHtML

list(dict.fromkeys(arr))
来源：http://blog.zdbjq.cn/Article/details/gcrvqfogm.sHtML

[U06] Py：合并两个字典
来源：http://3g.hesvh.cn/Article/details/gluwbeczg.sHtML

{**a, **b}
来源：http://www.blog.hesvh.cn/Article/details/gkkimpvfm.sHtML

[U07] Py：反转字典键值
来源：http://read.share.fehbvm.com/Article/details/gpjrhnyzu.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.zdbjq.cn/Article/details/guvwaqhwh.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.zdbjq.cn/Article/details/gkvvenjay.sHtML

[y for x in nested for y in x]
来源：http://www.share.fehbvm.com/Article/details/gkezxwfpr.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.fehbvm.com/Article/details/guowoefub.sHtML

max(d, key=d.get)
来源：http://m.share.fehbvm.com/Article/details/gakbsrdva.sHtML

[U10] Py：按值排序字典
来源：http://mobile.zdbjq.cn/Article/details/gwbqmvlnn.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.hesvh.cn/Article/details/gsweadwhd.sHtML

[U11] Py：生成器表达式
来源：http://mobile.fehbvm.com/Article/details/gawiulwaz.sHtML

(x * 2 for x in arr)
来源：http://3g.fehbvm.com/Article/details/gxefmeycy.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.fehbvm.com/Article/details/gsqxxozdj.sHtML

Counter(arr).most_common(3)
来源：http://blog.zdbjq.cn/Article/details/gmsvjbdiv.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.hesvh.cn/Article/details/gjhdbxzvd.sHtML

deque(maxlen=10)
来源：http://www.blog.hesvh.cn/Article/details/ghjajucmw.sHtML

[U14] Py：分组收集到列表
来源：http://baike.fehbvm.com/Article/details/gljyfwysj.sHtML

defaultdict(list)
来源：http://www.m.share.zdbjq.cn/Article/details/gqvdzjsgn.sHtML

[U15] Py：高精度计时
来源：http://blog.fehbvm.com/Article/details/gwndotkdt.sHtML

t = time.perf_counter()
来源：http://www.m.share.hesvh.cn/Article/details/gzvpatrnc.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.hesvh.cn/Article/details/glsvdzocs.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.fehbvm.com/Article/details/govrlfvhw.sHtML

[U17] Py：初始化日志
来源：http://mobile.hesvh.cn/Article/details/gjgkaxgmy.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.fehbvm.com/Article/details/gsodundga.sHtML

[U18] Py：预编译正则
来源：http://www.share.fehbvm.com/Article/details/gryryhvau.sHtML

pat = re.compile(r"\d+")
来源：http://wap.fehbvm.com/Article/details/gbnkghhhu.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.zdbjq.cn/Article/details/gnwsdpnyp.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.hesvh.cn/Article/details/gxerhfxxz.sHtML

[U20] Py：缓存函数结果
来源：http://wap.fehbvm.com/Article/details/gidgttunq.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.hesvh.cn/Article/details/gdgsjsqdh.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.zdbjq.cn/Article/details/givfgtahn.sHtML

@contextlib.contextmanager
来源：http://read.share.zdbjq.cn/Article/details/gsekxvuoy.sHtML

[U22] Py：矩阵转置
来源：http://m.share.fehbvm.com/Article/details/grlvjqqvb.sHtML

list(zip(*m))
来源：http://baike.hesvh.cn/Article/details/gbosxcqfx.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.fehbvm.com/Article/details/gkaagoggw.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.hesvh.cn/Article/details/gszvdpifw.sHtML

[U24] Py：路径操作
来源：http://www.share.fehbvm.com/Article/details/grufdijxd.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.hesvh.cn/Article/details/gdiegkhoq.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.zdbjq.cn/Article/details/gzpfstipj.sHtML

csv.DictReader(f)
来源：http://mobile.hesvh.cn/Article/details/glxnuqjzu.sHtML

[U26] Py：并发下载
来源：http://www.share.zdbjq.cn/Article/details/ggmqbalri.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.fehbvm.com/Article/details/guhrkfqcy.sHtML

[U27] Py：异步 HTTP
来源：http://wap.hesvh.cn/Article/details/gaoqazcbw.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.hesvh.cn/Article/details/gglzkpnbb.sHtML

[U28] Py：类型别名
来源：http://read.share.hesvh.cn/Article/details/guqdnvuoo.sHtML

UserId = int
来源：http://blog.fehbvm.com/Article/details/gsocmrpdv.sHtML

[U29] Py：属性校验
来源：http://www.m.share.fehbvm.com/Article/details/gzwinidxp.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.hesvh.cn/Article/details/gznylmrdf.sHtML

[U30] Py：数据类
来源：http://mobile.zdbjq.cn/Article/details/gelpbmcry.sHtML

@dataclass(slots=True)
来源：http://www.m.share.fehbvm.com/Article/details/gacuatcty.sHtML

[U31] Py：单测
来源：http://baike.zdbjq.cn/Article/details/gnrmqwbrs.sHtML

python -m pytest -q
来源：http://read.share.hesvh.cn/Article/details/gcuhoacpj.sHtML

[U32] Py：代码格式化
来源：http://wap.zdbjq.cn/Article/details/gwbkueujr.sHtML

ruff format . && ruff check --fix .
来源：http://3g.hesvh.cn/Article/details/gftfvhppg.sHtML

[U33] Py：打包发布
来源：http://blog.zdbjq.cn/Article/details/gxpwlwtbn.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.hesvh.cn/Article/details/gglpfezpc.sHtML

[U34] Py：判断编码
来源：http://www.share.fehbvm.com/Article/details/gvuyqlden.sHtML

chardet.detect(raw)
来源：http://3g.hesvh.cn/Article/details/goyttdqwx.sHtML

[U35] Py：发送邮件
来源：http://mobile.hesvh.cn/Article/details/gktakaapt.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.fehbvm.com/Article/details/gystdrcfp.sHtML

[U36] Py：定时任务
来源：http://www.m.share.hesvh.cn/Article/details/ghsczzdox.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.fehbvm.com/Article/details/ghmjzqwta.sHtML

[U37] Py：读写 Excel
来源：http://blog.zdbjq.cn/Article/details/gsliafpko.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.hesvh.cn/Article/details/gcuflojvr.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.fehbvm.com/Article/details/gprainvfc.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.hesvh.cn/Article/details/gxvpumelm.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.fehbvm.com/Article/details/gtnqrjtmf.sHtML

sys.stdout.isatty()
来源：http://baike.zdbjq.cn/Article/details/gbzeujbzb.sHtML

[U40] Py：打印到标准错误
来源：http://3g.fehbvm.com/Article/details/ggwazdjzn.sHtML

print("err", file=sys.stderr)
来源：http://m.share.hesvh.cn/Article/details/guuehseuh.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.zdbjq.cn/Article/details/gwjocgmfj.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.fehbvm.com/Article/details/gcohnjgii.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.fehbvm.com/Article/details/gubonijoc.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.zdbjq.cn/Article/details/ggngeccdw.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.hesvh.cn/Article/details/gtbcahqsf.sHtML

namespace App\Http;
来源：http://baike.zdbjq.cn/Article/details/gzabtdyug.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.hesvh.cn/Article/details/gmufeotgh.sHtML

declare(strict_types=1);
来源：http://www.m.share.hesvh.cn/Article/details/guxxnhzqj.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.zdbjq.cn/Article/details/gdkzcftlg.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gpgsdgnji.sHtML

[U46] PHP：可空类型
来源：http://www.share.fehbvm.com/Article/details/gpsrtnsje.sHtML

?string $name = null
来源：http://blog.hesvh.cn/Article/details/gbuejmlhe.sHtML

[U47] PHP：联合类型
来源：http://3g.fehbvm.com/Article/details/gdhrkvrzz.sHtML

int|string $id
来源：http://baike.hesvh.cn/Article/details/gdpbycpkf.sHtML

[U48] PHP：纯枚举
来源：http://blog.zdbjq.cn/Article/details/gejsnqbzd.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.hesvh.cn/Article/details/gqzgavqbv.sHtML

[U49] PHP：只读属性
来源：http://blog.fehbvm.com/Article/details/ggrzddwht.sHtML

public readonly string $name
来源：http://read.share.hesvh.cn/Article/details/gaukxfhdy.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.zdbjq.cn/Article/details/gkbxnfejd.sHtML

public function __construct(private int $id) {}
来源：http://baike.zdbjq.cn/Article/details/geyrppayt.sHtML

[U51] PHP：数组解构
来源：http://blog.fehbvm.com/Article/details/gwhapjckq.sHtML

[$a, $b] = $arr;
来源：http://mobile.hesvh.cn/Article/details/gtzztmzsf.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.hesvh.cn/Article/details/gxvonqkpq.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.hesvh.cn/Article/details/gpcdmgjdp.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.fehbvm.com/Article/details/gphpraubp.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.fehbvm.com/Article/details/gquusydkw.sHtML

[U54] PHP：空安全调用
来源：http://read.share.hesvh.cn/Article/details/ghwuyfuyr.sHtML

$obj?->method()
来源：http://read.share.zdbjq.cn/Article/details/gkngyoakw.sHtML

[U55] PHP：match 表达式
来源：http://mobile.fehbvm.com/Article/details/gzrkjklcr.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.hesvh.cn/Article/details/gmsjmizas.sHtML

[U56] PHP：命名参数
来源：http://read.share.hesvh.cn/Article/details/gputvkxia.sHtML

f(a: 1, b: 2)
来源：http://read.share.hesvh.cn/Article/details/gdnhxldbd.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gxtxrsnsi.sHtML

"值: {$a}"
来源：http://www.blog.hesvh.cn/Article/details/gtgntpysw.sHtML

[U58] PHP：数组三件套
来源：http://mobile.hesvh.cn/Article/details/giinxfrnv.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.zdbjq.cn/Article/details/gebzlqzmb.sHtML

[U59] PHP：自定义排序
来源：http://baike.fehbvm.com/Article/details/gnmbqujkn.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fehbvm.com/Article/details/ggpuqwqja.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.fehbvm.com/Article/details/gevltjhlg.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.fehbvm.com/Article/details/gucjwakoe.sHtML

[U61] PHP：正则
来源：http://3g.hesvh.cn/Article/details/gdcpnlubo.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.fehbvm.com/Article/details/gvcciavwo.sHtML

[U62] PHP：日期对象
来源：http://mobile.fehbvm.com/Article/details/gydxaddie.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.fehbvm.com/Article/details/gwwewofro.sHtML

[U63] PHP：文件读写
来源：http://www.blog.hesvh.cn/Article/details/gavgiszbd.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.zdbjq.cn/Article/details/gpujtddcg.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.zdbjq.cn/Article/details/gvcnsfbrj.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.zdbjq.cn/Article/details/gqkfdxwux.sHtML

[U65] PHP：会话
来源：http://www.m.share.hesvh.cn/Article/details/gqpjfgwqy.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/ggukflria.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.zdbjq.cn/Article/details/gwjyhecue.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.fehbvm.com/Article/details/gaugigugr.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.zdbjq.cn/Article/details/grhwwjcmo.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.hesvh.cn/Article/details/gkxxbetrx.sHtML

[U68] PHP：PDO 连接
来源：http://3g.hesvh.cn/Article/details/gixedrraj.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.hesvh.cn/Article/details/gijqqssld.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.hesvh.cn/Article/details/gfyfxsqqj.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.fehbvm.com/Article/details/gyskrwihu.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.hesvh.cn/Article/details/griapqyas.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.zdbjq.cn/Article/details/gafmrdtzt.sHtML

[U71] PHP：抛出异常
来源：http://www.share.zdbjq.cn/Article/details/gmhsqtoza.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.zdbjq.cn/Article/details/gtisgigno.sHtML

[U72] PHP：写错误日志
来源：http://baike.hesvh.cn/Article/details/gskkmdhnq.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.hesvh.cn/Article/details/gezjxgnru.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.fehbvm.com/Article/details/gcnwkixhb.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.fehbvm.com/Article/details/gqizvlhnf.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.hesvh.cn/Article/details/gvqzdeopc.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.zdbjq.cn/Article/details/gtxmgmgnt.sHtML

[U75] PHP：依赖注入
来源：http://mobile.zdbjq.cn/Article/details/gpmipfljg.sHtML

composer require psr/container
来源：http://3g.zdbjq.cn/Article/details/gnsimzjwp.sHtML

[U76] PHP：简单路由
来源：http://www.share.fehbvm.com/Article/details/ggqmecsmn.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.fehbvm.com/Article/details/ghoccymrz.sHtML

[U77] PHP：模板渲染
来源：http://blog.zdbjq.cn/Article/details/gydywaiqz.sHtML

composer require twig/twig
来源：http://www.blog.hesvh.cn/Article/details/gpclflphy.sHtML

[U78] PHP：单元测试
来源：http://www.blog.zdbjq.cn/Article/details/guhwgmrej.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.fehbvm.com/Article/details/ghzphdglw.sHtML

[U79] PHP：静态分析
来源：http://www.blog.hesvh.cn/Article/details/grhgwwdxq.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.fehbvm.com/Article/details/ggybhwyzn.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.zdbjq.cn/Article/details/giuzzalnh.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.hesvh.cn/Article/details/gpzknwedk.sHtML

[U81] JS：初始化项目
来源：http://m.share.fehbvm.com/Article/details/gynyxdgzu.sHtML

npm init -y;  npm i express
来源：http://www.share.zdbjq.cn/Article/details/gdyxpdqzz.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.hesvh.cn/Article/details/gnamkcttb.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.zdbjq.cn/Article/details/gbganenmk.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.hesvh.cn/Article/details/goybkecfy.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.zdbjq.cn/Article/details/ggdcrhlfo.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.zdbjq.cn/Article/details/griopkaum.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.fehbvm.com/Article/details/glvcdukrh.sHtML

[U85] JS：可选链
来源：http://www.m.share.fehbvm.com/Article/details/goyjqxsdy.sHtML

a?.b?.c
来源：http://www.share.fehbvm.com/Article/details/gghadedbb.sHtML

[U86] JS：空值合并
来源：http://wap.hesvh.cn/Article/details/gzmytxwqb.sHtML

a ?? b
来源：http://wap.fehbvm.com/Article/details/gsnitsxgk.sHtML

[U87] JS：解构默认值
来源：http://wap.hesvh.cn/Article/details/geteqacck.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.fehbvm.com/Article/details/gsawxbotj.sHtML

[U88] JS：对象展开合并
来源：http://www.share.fehbvm.com/Article/details/giuelfout.sHtML

{ ...a, ...b }
来源：http://wap.hesvh.cn/Article/details/gvwmfyybm.sHtML

[U89] JS：数组去重
来源：http://read.share.hesvh.cn/Article/details/gpuykwlsh.sHtML

[...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gliywfxsy.sHtML

[U90] JS：数字数组排序
来源：http://baike.zdbjq.cn/Article/details/gezkjfwki.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gbkxqtdge.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.hesvh.cn/Article/details/gdkjbnmvh.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.fehbvm.com/Article/details/gdybtoird.sHtML

[U92] JS：深拷贝
来源：http://read.share.zdbjq.cn/Article/details/gffjjtned.sHtML

structuredClone(obj)
来源：http://www.blog.hesvh.cn/Article/details/gxwyrcvhw.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.fehbvm.com/Article/details/gdupgwbkn.sHtML

`共 ${n} 条`
来源：http://3g.zdbjq.cn/Article/details/gwcvdquba.sHtML

[U94] JS：箭头函数
来源：http://www.blog.fehbvm.com/Article/details/gdilnkxjq.sHtML

const double = x => x * 2;
来源：http://3g.zdbjq.cn/Article/details/gvrlfdaae.sHtML

[U95] JS：Promise 包装
来源：http://baike.hesvh.cn/Article/details/gamkqofcc.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.hesvh.cn/Article/details/goxtfoiwk.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.fehbvm.com/Article/details/gifixtfdh.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/grmttttvy.sHtML

[U97] JS：并发请求
来源：http://read.share.hesvh.cn/Article/details/gfykevukq.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/gesefjggd.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.zdbjq.cn/Article/details/gbzikrytq.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.zdbjq.cn/Article/details/ggfnfqfwk.sHtML

[U99] JS：事件监听
来源：http://3g.hesvh.cn/Article/details/gilwztytq.sHtML

el.addEventListener("click", e => {})
来源：http://3g.zdbjq.cn/Article/details/gsiszqyhl.sHtML

[U100] JS：DOM 查询
来源：http://m.share.zdbjq.cn/Article/details/gkgeykjeb.sHtML

document.querySelector(".item")
来源：http://wap.fehbvm.com/Article/details/gbbbywczf.sHtML

[U101] JS：classList 操作
来源：http://www.share.fehbvm.com/Article/details/gkbgcmspg.sHtML

el.classList.toggle("active")
来源：http://blog.zdbjq.cn/Article/details/gvhmcwnio.sHtML

[U102] JS：本地存储
来源：http://read.share.hesvh.cn/Article/details/gxgaipwwn.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.zdbjq.cn/Article/details/ghgnvbqkl.sHtML

[U103] JS：定时器
来源：http://m.share.zdbjq.cn/Article/details/gjalrurra.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.hesvh.cn/Article/details/goqgfrgtz.sHtML

[U104] JS：防抖
来源：http://3g.hesvh.cn/Article/details/gftbycmji.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/glxqoyfrn.sHtML

[U105] JS：节流
来源：http://m.share.hesvh.cn/Article/details/gapyisiop.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.fehbvm.com/Article/details/gzjrbhyxm.sHtML

[U106] JS：日期格式化
来源：http://baike.fehbvm.com/Article/details/gpizyolaa.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.hesvh.cn/Article/details/gnxgqplmr.sHtML

[U107] JS：数字千分位
来源：http://read.share.hesvh.cn/Article/details/gmasxskyd.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.hesvh.cn/Article/details/gjsdpwpkl.sHtML

[U108] JS：随机整数
来源：http://read.share.zdbjq.cn/Article/details/gpkpwenjn.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.zdbjq.cn/Article/details/gcjondelw.sHtML

[U109] JS：数组分组
来源：http://wap.hesvh.cn/Article/details/gclcjmrqe.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.fehbvm.com/Article/details/gkqxfeazz.sHtML

[U110] JS：数组分块
来源：http://blog.hesvh.cn/Article/details/gqvvfgvko.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.zdbjq.cn/Article/details/gjxoremue.sHtML

[U111] JS：对象转 Map
来源：http://3g.fehbvm.com/Article/details/gfhrwneqf.sHtML

new Map(Object.entries(obj))
来源：http://m.share.zdbjq.cn/Article/details/garztavad.sHtML

[U112] JS：字符串补位
来源：http://blog.zdbjq.cn/Article/details/gcqpbvhdp.sHtML

"7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/ggkmrayid.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.fehbvm.com/Article/details/ghckdadma.sHtML

s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/geeyrhpjs.sHtML

[U114] JS：JSON 深比较
来源：http://blog.zdbjq.cn/Article/details/gqbspkvww.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.zdbjq.cn/Article/details/gdlfdpjfn.sHtML

[U115] JS：生成 UUID
来源：http://www.share.hesvh.cn/Article/details/ghqvxmlue.sHtML

crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/guubudtez.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.hesvh.cn/Article/details/gbvnjhugl.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.fehbvm.com/Article/details/gqidxwbpn.sHtML

[U117] JS：单元测试
来源：http://www.share.zdbjq.cn/Article/details/gmlnnwziu.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.fehbvm.com/Article/details/gcauynebm.sHtML

[U118] JS：开发服务器
来源：http://3g.hesvh.cn/Article/details/ggtleuhvo.sHtML

npm i -D vite;  npx vite
来源：http://read.share.hesvh.cn/Article/details/gqlbabhie.sHtML

[U119] JS：生产构建
来源：http://read.share.zdbjq.cn/Article/details/gmxgnuepg.sHtML

npx vite build
来源：http://www.m.share.hesvh.cn/Article/details/gtemnyqil.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.hesvh.cn/Article/details/gwdtrdcea.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.fehbvm.com/Article/details/gigizyqee.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/grvdzvauz.sHtML

统计汇总
来源：http://read.share.fehbvm.com/Article/details/gqwextsdh.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gmcaoopoq.sHtML

按语言统计（条）：
来源：http://read.share.hesvh.cn/Article/details/ghwkasvpa.sHtML

Python ......... 252
来源：http://www.blog.hesvh.cn/Article/details/geniwblik.sHtML

PHP ............ 252
来源：http://blog.fehbvm.com/Article/details/gzhxsmaju.sHtML

JavaScript ..... 252
来源：http://blog.fehbvm.com/Article/details/gnzzbmekz.sHtML

TypeScript ..... 212
来源：http://wap.hesvh.cn/Article/details/gpqnjpjgg.sHtML

Java ........... 212
来源：http://mobile.fehbvm.com/Article/details/gbnfuibtl.sHtML

Go ............. 212
来源：http://3g.fehbvm.com/Article/details/groomxily.sHtML

Ruby ........... 212
来源：http://blog.fehbvm.com/Article/details/gjunwyhci.sHtML

C# ............. 212
来源：http://m.share.fehbvm.com/Article/details/gjlorvhzf.sHtML

C .............. 30
来源：http://mobile.zdbjq.cn/Article/details/gexenhrrs.sHtML

C++ ............ 30
来源：http://baike.fehbvm.com/Article/details/gfguopvvr.sHtML

SQL ............ 90
来源：http://www.share.hesvh.cn/Article/details/gtebqqvyb.sHtML

Bash ........... 80
来源：http://baike.hesvh.cn/Article/details/gyizksqzg.sHtML

Kotlin ......... 15
来源：http://wap.zdbjq.cn/Article/details/gcmurysed.sHtML

Swift .......... 15
来源：http://baike.zdbjq.cn/Article/details/gkqzpcfya.sHtML

Lua ............ 10
来源：http://mobile.hesvh.cn/Article/details/gbayzajky.sHtML

Perl ........... 10
来源：http://www.m.share.hesvh.cn/Article/details/gxgzqskhj.sHtML

Scala .......... 10
来源：http://3g.zdbjq.cn/Article/details/gnpdswkfq.sHtML

------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gotukyloe.sHtML

合计 ........... 2106 条
来源：http://read.share.hesvh.cn/Article/details/gznaujgly.sHtML

按章节统计：
来源：http://mobile.hesvh.cn/Article/details/gffckzdzh.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.hesvh.cn/Article/details/gwvwsqpca.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/grcoimjuy.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/grncjlowv.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.hesvh.cn/Article/details/gdtfunebx.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.fehbvm.com/Article/details/gfyvzzobc.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.zdbjq.cn/Article/details/giyhfnuzx.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.hesvh.cn/Article/details/goyoqazhy.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.fehbvm.com/Article/details/gfkkxlkky.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gtonmdlol.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.hesvh.cn/Article/details/gompvbgqq.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gaobdtacm.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gyhjkntim.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gdzrsdnup.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.hesvh.cn/Article/details/galicwisw.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.fehbvm.com/Article/details/gpavrxihl.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gywbrhszh.sHtML

Q SQL 专题                              90
来源：http://3g.fehbvm.com/Article/details/ghuamkwoh.sHtML

R Bash 专题                             80
来源：http://3g.fehbvm.com/Article/details/ghaswdqpv.sHtML

S C / C++ 专题                          60
来源：http://mobile.hesvh.cn/Article/details/gbfvigaoj.sHtML

T 其他语言补充                          60
来源：http://3g.zdbjq.cn/Article/details/gaunpokix.sHtML

U 高频实用片段                         120
来源：http://www.share.hesvh.cn/Article/details/gikkkrokn.sHtML

------------------------------------
来源：http://baike.fehbvm.com/Article/details/gtgxwcrfj.sHtML

合计                                  2106 条
来源：http://m.share.fehbvm.com/Article/details/gvmxsytlb.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/goumlanuj.sHtML

使用提醒
来源：http://blog.fehbvm.com/Article/details/geasnchpp.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/gfdlngdxh.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.fehbvm.com/Article/details/gsmgcouvv.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.zdbjq.cn/Article/details/gyqhxqfqk.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.hesvh.cn/Article/details/guiogxwnh.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.zdbjq.cn/Article/details/gigafdxjg.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.zdbjq.cn/Article/details/gflrfipwk.sHtML

—— 文件结束 ——
来源：http://www.blog.fehbvm.com/Article/details/gdiskmgfm.sHtML


<!-- 参考信息 -->