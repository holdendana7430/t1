代发 wailian999

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.fehbvm.com/Article/details/gjpbzwrgc.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gxeuuddup.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.hesvh.cn/Article/details/gfpculfpj.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gpyxpdiqf.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.zdbjq.cn/Article/details/gsuzzbbkm.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.fehbvm.com/Article/details/gbxmhnfqj.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.fehbvm.com/Article/details/gaxucqcxp.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.fehbvm.com/Article/details/gxbkjrfap.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.zdbjq.cn/Article/details/gautnzhje.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.hesvh.cn/Article/details/gojjteiat.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.hesvh.cn/Article/details/gxculwveh.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.fehbvm.com/Article/details/gmkhhcmrv.sHtML

[U05] Py：列表去重且保序
来源：http://baike.zdbjq.cn/Article/details/gcseayusu.sHtML

list(dict.fromkeys(arr))
来源：http://baike.zdbjq.cn/Article/details/gimxzqdbo.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.zdbjq.cn/Article/details/gwismvjqr.sHtML

{**a, **b}
来源：http://wap.zdbjq.cn/Article/details/grjawdsjp.sHtML

[U07] Py：反转字典键值
来源：http://baike.zdbjq.cn/Article/details/gsdufovvr.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.zdbjq.cn/Article/details/gihmaqttv.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.fehbvm.com/Article/details/gdivqvwsp.sHtML

[y for x in nested for y in x]
来源：http://www.blog.fehbvm.com/Article/details/gmjhlhylw.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.hesvh.cn/Article/details/gshywlyvo.sHtML

max(d, key=d.get)
来源：http://mobile.fehbvm.com/Article/details/gtezahsoj.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.fehbvm.com/Article/details/gfeqbtphx.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.zdbjq.cn/Article/details/ghbotpxrp.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.hesvh.cn/Article/details/gqtmnkdlq.sHtML

(x * 2 for x in arr)
来源：http://blog.hesvh.cn/Article/details/gnfszkxpd.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.hesvh.cn/Article/details/gihjzusax.sHtML

Counter(arr).most_common(3)
来源：http://read.share.fehbvm.com/Article/details/gagbfahgp.sHtML

[U13] Py：固定长度队列
来源：http://m.share.hesvh.cn/Article/details/gcpfgsqgi.sHtML

deque(maxlen=10)
来源：http://baike.zdbjq.cn/Article/details/givraikkp.sHtML

[U14] Py：分组收集到列表
来源：http://3g.fehbvm.com/Article/details/galohsssl.sHtML

defaultdict(list)
来源：http://mobile.zdbjq.cn/Article/details/gplyjfzfo.sHtML

[U15] Py：高精度计时
来源：http://www.share.zdbjq.cn/Article/details/gyqhlsieb.sHtML

t = time.perf_counter()
来源：http://baike.hesvh.cn/Article/details/gfljeucff.sHtML

[U16] Py：命令行参数解析
来源：http://blog.fehbvm.com/Article/details/gwggggqwz.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.fehbvm.com/Article/details/gkzcunlha.sHtML

[U17] Py：初始化日志
来源：http://blog.fehbvm.com/Article/details/gdibtwnav.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.zdbjq.cn/Article/details/geklobgwn.sHtML

[U18] Py：预编译正则
来源：http://m.share.zdbjq.cn/Article/details/gekxcmxry.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.hesvh.cn/Article/details/gluybrbap.sHtML

[U19] Py：正则替换带回调
来源：http://blog.fehbvm.com/Article/details/gkczlhjpp.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.hesvh.cn/Article/details/gkebiqjmx.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.zdbjq.cn/Article/details/gcksysmoi.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.zdbjq.cn/Article/details/guazezfeu.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.fehbvm.com/Article/details/gheggrcgn.sHtML

@contextlib.contextmanager
来源：http://www.m.share.zdbjq.cn/Article/details/gdgithwlu.sHtML

[U22] Py：矩阵转置
来源：http://baike.zdbjq.cn/Article/details/gtljwabrj.sHtML

list(zip(*m))
来源：http://www.m.share.hesvh.cn/Article/details/gtflriwzv.sHtML

[U23] Py：分块读取大文件
来源：http://wap.hesvh.cn/Article/details/gqvjldfvw.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.hesvh.cn/Article/details/gpxgidyay.sHtML

[U24] Py：路径操作
来源：http://wap.fehbvm.com/Article/details/gvafaxcrq.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.hesvh.cn/Article/details/gxvpwpuve.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.zdbjq.cn/Article/details/golekujnp.sHtML

csv.DictReader(f)
来源：http://m.share.fehbvm.com/Article/details/gqabyfjtq.sHtML

[U26] Py：并发下载
来源：http://baike.zdbjq.cn/Article/details/gwonxabjh.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.hesvh.cn/Article/details/ghxrmyzbq.sHtML

[U27] Py：异步 HTTP
来源：http://wap.hesvh.cn/Article/details/gsabknozn.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.zdbjq.cn/Article/details/gfbtdpiua.sHtML

[U28] Py：类型别名
来源：http://www.m.share.zdbjq.cn/Article/details/gffmnyzoy.sHtML

UserId = int
来源：http://www.blog.fehbvm.com/Article/details/gtrgmmbhr.sHtML

[U29] Py：属性校验
来源：http://www.blog.fehbvm.com/Article/details/gqxnwbqew.sHtML

@property 与 @x.setter 配合
来源：http://mobile.zdbjq.cn/Article/details/gascrgpov.sHtML

[U30] Py：数据类
来源：http://baike.hesvh.cn/Article/details/gauahdyqv.sHtML

@dataclass(slots=True)
来源：http://www.m.share.fehbvm.com/Article/details/gutdrnxmh.sHtML

[U31] Py：单测
来源：http://3g.fehbvm.com/Article/details/gbyqybtql.sHtML

python -m pytest -q
来源：http://blog.zdbjq.cn/Article/details/gmohowpbm.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.fehbvm.com/Article/details/gcyavtlbb.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.hesvh.cn/Article/details/gfeusuzel.sHtML

[U33] Py：打包发布
来源：http://m.share.zdbjq.cn/Article/details/gbnxjjgoj.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.fehbvm.com/Article/details/gznzffdlx.sHtML

[U34] Py：判断编码
来源：http://read.share.fehbvm.com/Article/details/gdrpmcutw.sHtML

chardet.detect(raw)
来源：http://mobile.fehbvm.com/Article/details/gmkhmedfm.sHtML

[U35] Py：发送邮件
来源：http://blog.zdbjq.cn/Article/details/gboidfnzs.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.hesvh.cn/Article/details/gtxlppluh.sHtML

[U36] Py：定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/gjcqayukk.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.hesvh.cn/Article/details/gdoiexeak.sHtML

[U37] Py：读写 Excel
来源：http://www.share.fehbvm.com/Article/details/gmzyjqyat.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.zdbjq.cn/Article/details/gimoabyoo.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.hesvh.cn/Article/details/gyhqhgkyd.sHtML

Path(__file__).resolve().parent
来源：http://m.share.fehbvm.com/Article/details/gcuocnqje.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.hesvh.cn/Article/details/gyesrwvnr.sHtML

sys.stdout.isatty()
来源：http://mobile.fehbvm.com/Article/details/glxylwdwk.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.zdbjq.cn/Article/details/gnyuwmlhd.sHtML

print("err", file=sys.stderr)
来源：http://m.share.zdbjq.cn/Article/details/gdhzazaii.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.hesvh.cn/Article/details/gorenhjaj.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.zdbjq.cn/Article/details/gsemfptkt.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.zdbjq.cn/Article/details/gsfcoytmf.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.zdbjq.cn/Article/details/gqbrzhotf.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.fehbvm.com/Article/details/gfeldjfsj.sHtML

namespace App\Http;
来源：http://read.share.hesvh.cn/Article/details/gipiykzro.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.zdbjq.cn/Article/details/gyzmasgxm.sHtML

declare(strict_types=1);
来源：http://www.blog.zdbjq.cn/Article/details/gtfbhpkrf.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.fehbvm.com/Article/details/gmjpdbmhq.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gghrdfbpi.sHtML

[U46] PHP：可空类型
来源：http://mobile.fehbvm.com/Article/details/gbqucfdme.sHtML

?string $name = null
来源：http://m.share.zdbjq.cn/Article/details/gxtjhcxzx.sHtML

[U47] PHP：联合类型
来源：http://www.share.hesvh.cn/Article/details/gbamefrho.sHtML

int|string $id
来源：http://mobile.fehbvm.com/Article/details/gflzkferx.sHtML

[U48] PHP：纯枚举
来源：http://mobile.hesvh.cn/Article/details/gqnrrgdnx.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.fehbvm.com/Article/details/gvjpsccee.sHtML

[U49] PHP：只读属性
来源：http://www.share.hesvh.cn/Article/details/gywxzsfta.sHtML

public readonly string $name
来源：http://read.share.zdbjq.cn/Article/details/ggsdhmksq.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.fehbvm.com/Article/details/gyzshndum.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.zdbjq.cn/Article/details/ghvpbunqt.sHtML

[U51] PHP：数组解构
来源：http://www.blog.zdbjq.cn/Article/details/ginlrwxlv.sHtML

[$a, $b] = $arr;
来源：http://www.share.hesvh.cn/Article/details/gzrrdxezv.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.hesvh.cn/Article/details/gmaxrvmng.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.hesvh.cn/Article/details/gviposzfe.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.fehbvm.com/Article/details/gibhcpyuh.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.hesvh.cn/Article/details/gbioofskm.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.hesvh.cn/Article/details/gavbuzubi.sHtML

$obj?->method()
来源：http://baike.fehbvm.com/Article/details/gxfpfstfz.sHtML

[U55] PHP：match 表达式
来源：http://baike.zdbjq.cn/Article/details/gmfpsaaya.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.fehbvm.com/Article/details/glzwwbwsk.sHtML

[U56] PHP：命名参数
来源：http://baike.fehbvm.com/Article/details/ghjqhrjvn.sHtML

f(a: 1, b: 2)
来源：http://baike.zdbjq.cn/Article/details/gkpdywiln.sHtML

[U57] PHP：字符串插值
来源：http://3g.hesvh.cn/Article/details/gvbdwtpwc.sHtML

"值: {$a}"
来源：http://mobile.zdbjq.cn/Article/details/gdopvxcou.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.fehbvm.com/Article/details/gqewcoqqv.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.fehbvm.com/Article/details/gscmyifpf.sHtML

[U59] PHP：自定义排序
来源：http://mobile.hesvh.cn/Article/details/gnnwwtwhs.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fehbvm.com/Article/details/grnucaphf.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.zdbjq.cn/Article/details/gfmqibyrm.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.zdbjq.cn/Article/details/gbsczhotg.sHtML

[U61] PHP：正则
来源：http://3g.zdbjq.cn/Article/details/gxkrqnlfu.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.hesvh.cn/Article/details/gbzeuuuhw.sHtML

[U62] PHP：日期对象
来源：http://www.share.fehbvm.com/Article/details/giyuyfxrs.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.hesvh.cn/Article/details/gkcpwqhko.sHtML

[U63] PHP：文件读写
来源：http://3g.fehbvm.com/Article/details/gorsbrlii.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.fehbvm.com/Article/details/gnvwbroud.sHtML

[U64] PHP：目录遍历
来源：http://wap.zdbjq.cn/Article/details/gemfxgkvz.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.zdbjq.cn/Article/details/giyjsmloh.sHtML

[U65] PHP：会话
来源：http://www.blog.hesvh.cn/Article/details/ggjxzceer.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gndtedqxg.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.fehbvm.com/Article/details/gkaotzjdq.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.fehbvm.com/Article/details/gogtfgysr.sHtML

[U67] PHP：处理文件上传
来源：http://3g.zdbjq.cn/Article/details/gmqrkrbms.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.fehbvm.com/Article/details/gdpikogtq.sHtML

[U68] PHP：PDO 连接
来源：http://3g.zdbjq.cn/Article/details/gnodwmylu.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.fehbvm.com/Article/details/gwmijhkce.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.hesvh.cn/Article/details/gnikxlnmz.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.fehbvm.com/Article/details/gnlcksjnj.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.hesvh.cn/Article/details/gpqythqvv.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.hesvh.cn/Article/details/gucipbnbp.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.fehbvm.com/Article/details/gwcmijyoy.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.hesvh.cn/Article/details/gvytpemqw.sHtML

[U72] PHP：写错误日志
来源：http://www.share.zdbjq.cn/Article/details/gslgvlgrb.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.zdbjq.cn/Article/details/gwuhmpsvc.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.fehbvm.com/Article/details/gvxpughya.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.zdbjq.cn/Article/details/ggowtvfdh.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.fehbvm.com/Article/details/glcettlek.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.hesvh.cn/Article/details/guqgjxcvc.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.hesvh.cn/Article/details/gddqzdoej.sHtML

composer require psr/container
来源：http://blog.zdbjq.cn/Article/details/gogfkjgse.sHtML

[U76] PHP：简单路由
来源：http://3g.hesvh.cn/Article/details/gtbhxupvv.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.fehbvm.com/Article/details/gxwtbszxc.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.zdbjq.cn/Article/details/gunorblzd.sHtML

composer require twig/twig
来源：http://m.share.hesvh.cn/Article/details/gcppnmkuo.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.hesvh.cn/Article/details/gliagcsww.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.hesvh.cn/Article/details/gpyrwrxbk.sHtML

[U79] PHP：静态分析
来源：http://www.share.fehbvm.com/Article/details/gqbhplblg.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.zdbjq.cn/Article/details/gckcbkbrx.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.hesvh.cn/Article/details/gtflbbfqh.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.hesvh.cn/Article/details/gfydijvak.sHtML

[U81] JS：初始化项目
来源：http://blog.hesvh.cn/Article/details/gudplhwxk.sHtML

npm init -y;  npm i express
来源：http://wap.hesvh.cn/Article/details/geobebiyi.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.zdbjq.cn/Article/details/gomuqirsu.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.fehbvm.com/Article/details/gssrdkjto.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.fehbvm.com/Article/details/gcactnvua.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.fehbvm.com/Article/details/gmzgbjock.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.fehbvm.com/Article/details/gxspztvoj.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.hesvh.cn/Article/details/geihalbji.sHtML

[U85] JS：可选链
来源：http://www.blog.hesvh.cn/Article/details/gjhmwhcsy.sHtML

a?.b?.c
来源：http://blog.hesvh.cn/Article/details/gzzaocbja.sHtML

[U86] JS：空值合并
来源：http://blog.zdbjq.cn/Article/details/gvmwljcsd.sHtML

a ?? b
来源：http://3g.fehbvm.com/Article/details/glmjuzmip.sHtML

[U87] JS：解构默认值
来源：http://read.share.fehbvm.com/Article/details/gjctvjfui.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.fehbvm.com/Article/details/guxjvbrsn.sHtML

[U88] JS：对象展开合并
来源：http://read.share.hesvh.cn/Article/details/ggrhykuan.sHtML

{ ...a, ...b }
来源：http://www.m.share.hesvh.cn/Article/details/gddiuhytn.sHtML

[U89] JS：数组去重
来源：http://wap.hesvh.cn/Article/details/gbpjklias.sHtML

[...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/grdhkktes.sHtML

[U90] JS：数字数组排序
来源：http://baike.fehbvm.com/Article/details/gmcpulofj.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gwcjlhsto.sHtML

[U91] JS：对象键值遍历
来源：http://baike.zdbjq.cn/Article/details/gcseymowi.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.zdbjq.cn/Article/details/gaexkejfz.sHtML

[U92] JS：深拷贝
来源：http://mobile.fehbvm.com/Article/details/ghdqsjkjd.sHtML

structuredClone(obj)
来源：http://baike.hesvh.cn/Article/details/gmmsjnqfs.sHtML

[U93] JS：模板字符串
来源：http://mobile.zdbjq.cn/Article/details/gnxlhxcpc.sHtML

`共 ${n} 条`
来源：http://baike.zdbjq.cn/Article/details/grhsotpuo.sHtML

[U94] JS：箭头函数
来源：http://read.share.fehbvm.com/Article/details/gbyxageox.sHtML

const double = x => x * 2;
来源：http://3g.fehbvm.com/Article/details/glprypafz.sHtML

[U95] JS：Promise 包装
来源：http://mobile.hesvh.cn/Article/details/ggolpglza.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.zdbjq.cn/Article/details/ggiihnfkh.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.fehbvm.com/Article/details/gfsizterm.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/gzfktqipt.sHtML

[U97] JS：并发请求
来源：http://blog.zdbjq.cn/Article/details/grkxtuesj.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/gvocemjao.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.fehbvm.com/Article/details/ggvxgaoij.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.fehbvm.com/Article/details/gldbkgcub.sHtML

[U99] JS：事件监听
来源：http://3g.zdbjq.cn/Article/details/gfjolxgac.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.hesvh.cn/Article/details/guaxxoqlk.sHtML

[U100] JS：DOM 查询
来源：http://baike.fehbvm.com/Article/details/gduovbulg.sHtML

document.querySelector(".item")
来源：http://wap.zdbjq.cn/Article/details/gbskgzech.sHtML

[U101] JS：classList 操作
来源：http://wap.fehbvm.com/Article/details/giyhmquxk.sHtML

el.classList.toggle("active")
来源：http://m.share.hesvh.cn/Article/details/gjfhcuaaf.sHtML

[U102] JS：本地存储
来源：http://baike.hesvh.cn/Article/details/gkzytsnff.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.hesvh.cn/Article/details/gnngucxov.sHtML

[U103] JS：定时器
来源：http://wap.fehbvm.com/Article/details/gpktcfpgy.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.zdbjq.cn/Article/details/gupfessmo.sHtML

[U104] JS：防抖
来源：http://www.share.zdbjq.cn/Article/details/geoktravz.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gvmhpsdoi.sHtML

[U105] JS：节流
来源：http://baike.hesvh.cn/Article/details/ghnezuawk.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.fehbvm.com/Article/details/gifazrkri.sHtML

[U106] JS：日期格式化
来源：http://m.share.fehbvm.com/Article/details/gnclmxpvb.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.hesvh.cn/Article/details/genxbvhur.sHtML

[U107] JS：数字千分位
来源：http://3g.hesvh.cn/Article/details/gudbrlgab.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.fehbvm.com/Article/details/gstavxkwl.sHtML

[U108] JS：随机整数
来源：http://blog.zdbjq.cn/Article/details/gaxpumwrs.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.hesvh.cn/Article/details/gllhmhvou.sHtML

[U109] JS：数组分组
来源：http://blog.fehbvm.com/Article/details/gxhpxzlyw.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.zdbjq.cn/Article/details/gcmfoqcef.sHtML

[U110] JS：数组分块
来源：http://baike.zdbjq.cn/Article/details/gjkjbhqji.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.zdbjq.cn/Article/details/gikqrqysp.sHtML

[U111] JS：对象转 Map
来源：http://m.share.hesvh.cn/Article/details/gvessfvpv.sHtML

new Map(Object.entries(obj))
来源：http://blog.fehbvm.com/Article/details/gztnkenkh.sHtML

[U112] JS：字符串补位
来源：http://baike.hesvh.cn/Article/details/glfpvypco.sHtML

"7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gddjthnhp.sHtML

[U113] JS：正则替换全部
来源：http://read.share.hesvh.cn/Article/details/gifajtxhs.sHtML

s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gymokvlzw.sHtML

[U114] JS：JSON 深比较
来源：http://blog.zdbjq.cn/Article/details/gwjlguqzk.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fehbvm.com/Article/details/gtculoxwg.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.fehbvm.com/Article/details/gjlktwiin.sHtML

crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gaghszlzu.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.fehbvm.com/Article/details/gisaaxufp.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.fehbvm.com/Article/details/gqsppquei.sHtML

[U117] JS：单元测试
来源：http://www.m.share.fehbvm.com/Article/details/gkulffxyz.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.fehbvm.com/Article/details/gnyndikre.sHtML

[U118] JS：开发服务器
来源：http://www.share.hesvh.cn/Article/details/gajtowicn.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.fehbvm.com/Article/details/gnisrpubx.sHtML

[U119] JS：生产构建
来源：http://wap.zdbjq.cn/Article/details/gikrvcdqo.sHtML

npx vite build
来源：http://www.m.share.fehbvm.com/Article/details/gvowcrahx.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.fehbvm.com/Article/details/godltuamv.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.hesvh.cn/Article/details/gbvzqokrz.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gvxfebstl.sHtML

统计汇总
来源：http://www.blog.zdbjq.cn/Article/details/gblprrcyl.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gzsxdmolz.sHtML

按语言统计（条）：
来源：http://m.share.hesvh.cn/Article/details/gpkzhxqaw.sHtML

Python ......... 252
来源：http://www.share.zdbjq.cn/Article/details/gqimmkzvf.sHtML

PHP ............ 252
来源：http://www.share.zdbjq.cn/Article/details/gtkotkhoq.sHtML

JavaScript ..... 252
来源：http://mobile.fehbvm.com/Article/details/ggkxjnzzg.sHtML

TypeScript ..... 212
来源：http://blog.zdbjq.cn/Article/details/grodreeqr.sHtML

Java ........... 212
来源：http://3g.fehbvm.com/Article/details/gyapmsedp.sHtML

Go ............. 212
来源：http://read.share.zdbjq.cn/Article/details/gqlykdinn.sHtML

Ruby ........... 212
来源：http://www.blog.zdbjq.cn/Article/details/gyvwyvtyh.sHtML

C# ............. 212
来源：http://wap.zdbjq.cn/Article/details/gqfhltnue.sHtML

C .............. 30
来源：http://blog.hesvh.cn/Article/details/gzxrzrgiq.sHtML

C++ ............ 30
来源：http://wap.fehbvm.com/Article/details/ghqrriwid.sHtML

SQL ............ 90
来源：http://3g.hesvh.cn/Article/details/ghiywydlj.sHtML

Bash ........... 80
来源：http://mobile.hesvh.cn/Article/details/gvcdbqcpi.sHtML

Kotlin ......... 15
来源：http://www.share.hesvh.cn/Article/details/gnozsgxmp.sHtML

Swift .......... 15
来源：http://baike.zdbjq.cn/Article/details/gszerleay.sHtML

Lua ............ 10
来源：http://m.share.hesvh.cn/Article/details/gfseedlbz.sHtML

Perl ........... 10
来源：http://m.share.zdbjq.cn/Article/details/girevrdzs.sHtML

Scala .......... 10
来源：http://www.blog.hesvh.cn/Article/details/gfrxmrmjs.sHtML

------------------------------------
来源：http://baike.hesvh.cn/Article/details/gldkrualc.sHtML

合计 ........... 2106 条
来源：http://wap.hesvh.cn/Article/details/gsguflmet.sHtML

按章节统计：
来源：http://mobile.hesvh.cn/Article/details/glsfvdklr.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.zdbjq.cn/Article/details/grzhupidn.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/gcqrrdmwk.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.zdbjq.cn/Article/details/gemkjvizf.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.fehbvm.com/Article/details/ggbqqcluz.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.fehbvm.com/Article/details/gpdmekocy.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.fehbvm.com/Article/details/guoiicglu.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/gthgypjgk.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.fehbvm.com/Article/details/gqdhrufxn.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gakzagfpf.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.fehbvm.com/Article/details/guokjlmif.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/ggjnphroj.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gqvrslypx.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/grhsqbzvz.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.zdbjq.cn/Article/details/glsnnhzqy.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.hesvh.cn/Article/details/gergfwozh.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gszpvkpgc.sHtML

Q SQL 专题                              90
来源：http://blog.fehbvm.com/Article/details/gxagyaeaf.sHtML

R Bash 专题                             80
来源：http://wap.fehbvm.com/Article/details/geeplkuhw.sHtML

S C / C++ 专题                          60
来源：http://www.blog.hesvh.cn/Article/details/gmlczuhdc.sHtML

T 其他语言补充                          60
来源：http://www.m.share.hesvh.cn/Article/details/gxwsrbsqj.sHtML

U 高频实用片段                         120
来源：http://baike.hesvh.cn/Article/details/gnzhcdglv.sHtML

------------------------------------
来源：http://baike.fehbvm.com/Article/details/ggrosysam.sHtML

合计                                  2106 条
来源：http://blog.fehbvm.com/Article/details/gdxbnyrcf.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gbhxcvero.sHtML

使用提醒
来源：http://wap.hesvh.cn/Article/details/gehewtbdd.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gganhlmrg.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.zdbjq.cn/Article/details/gnvngjifr.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.zdbjq.cn/Article/details/gvvuiigyj.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.zdbjq.cn/Article/details/gfrwtmroj.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.hesvh.cn/Article/details/gfnxkpdae.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.zdbjq.cn/Article/details/giwiwupye.sHtML

—— 文件结束 ——
来源：http://3g.fehbvm.com/Article/details/gtuigsstm.sHtML


<!-- 参考信息 -->