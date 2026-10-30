代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.fanxiaobao.xyz/Article/details/glcqrkyhz.sHtML

[T59] Scala：循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gfjizelzz.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvxvieemi.sHtML

[T60] Scala：折叠
来源：http://wap.fanxiaobao.xyz/Article/details/gbcoztdyp.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtytutguu.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gpqgaffrj.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.fanxiaobao.xyz/Article/details/ghqdldlcv.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gdbsroolk.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.fanxiaobao.xyz/Article/details/gveapoywa.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.fanxiaobao.xyz/Article/details/gajysjszz.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fanxiaobao.xyz/Article/details/gkogfwklw.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/grufmfgys.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.fanxiaobao.xyz/Article/details/glijzfqhj.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.fanxiaobao.xyz/Article/details/gprsfjrix.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpymwxmdo.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.fanxiaobao.xyz/Article/details/glhupqkxv.sHtML

[U05] Py：列表去重且保序
来源：http://3g.fanxiaobao.xyz/Article/details/ghhehmrdd.sHtML

list(dict.fromkeys(arr))
来源：http://blog.fanxiaobao.xyz/Article/details/gvvbjemph.sHtML

[U06] Py：合并两个字典
来源：http://3g.fanxiaobao.xyz/Article/details/gqgjtmkiz.sHtML

{**a, **b}
来源：http://read.share.fanxiaobao.xyz/Article/details/gttrhpkmz.sHtML

[U07] Py：反转字典键值
来源：http://read.share.fanxiaobao.xyz/Article/details/gsthubvqq.sHtML

{v: k for k, v in d.items()}
来源：http://wap.fanxiaobao.xyz/Article/details/gzgmxpyhm.sHtML

[U08] Py：展平二维列表
来源：http://read.share.fanxiaobao.xyz/Article/details/gcyogvnlb.sHtML

[y for x in nested for y in x]
来源：http://blog.fanxiaobao.xyz/Article/details/ghggbtjcg.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.fanxiaobao.xyz/Article/details/guhjqqzqf.sHtML

max(d, key=d.get)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsgiyskhl.sHtML

[U10] Py：按值排序字典
来源：http://wap.fanxiaobao.xyz/Article/details/gfswrrnnd.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.fanxiaobao.xyz/Article/details/gxknlkuhi.sHtML

[U11] Py：生成器表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gwsktkweq.sHtML

(x * 2 for x in arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmbnbaced.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.fanxiaobao.xyz/Article/details/gefipzjhm.sHtML

Counter(arr).most_common(3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqtbyztst.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmaatjycn.sHtML

deque(maxlen=10)
来源：http://www.share.fanxiaobao.xyz/Article/details/gngtrdyan.sHtML

[U14] Py：分组收集到列表
来源：http://baike.fanxiaobao.xyz/Article/details/gmdptwslz.sHtML

defaultdict(list)
来源：http://wap.fanxiaobao.xyz/Article/details/glebmjqhl.sHtML

[U15] Py：高精度计时
来源：http://baike.fanxiaobao.xyz/Article/details/ggbgnvylm.sHtML

t = time.perf_counter()
来源：http://wap.fanxiaobao.xyz/Article/details/gggrokonc.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.fanxiaobao.xyz/Article/details/gxjlzxjbq.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fanxiaobao.xyz/Article/details/glkimaari.sHtML

[U17] Py：初始化日志
来源：http://baike.fanxiaobao.xyz/Article/details/gjefeuzqk.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.fanxiaobao.xyz/Article/details/gyfrtcmcc.sHtML

[U18] Py：预编译正则
来源：http://www.share.fanxiaobao.xyz/Article/details/gqkmmxxvw.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.fanxiaobao.xyz/Article/details/gzuyosbvv.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.fanxiaobao.xyz/Article/details/gynmnknqo.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdghgugyo.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.fanxiaobao.xyz/Article/details/gzafubaso.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghzeratji.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.fanxiaobao.xyz/Article/details/gomgzbpoo.sHtML

@contextlib.contextmanager
来源：http://3g.fanxiaobao.xyz/Article/details/gjpbmvauj.sHtML

[U22] Py：矩阵转置
来源：http://3g.fanxiaobao.xyz/Article/details/geewqjmac.sHtML

list(zip(*m))
来源：http://3g.fanxiaobao.xyz/Article/details/guucfnomx.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gopkrbpyi.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.fanxiaobao.xyz/Article/details/genbfpyps.sHtML

[U24] Py：路径操作
来源：http://3g.fanxiaobao.xyz/Article/details/gfhsbfalv.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnzjsfybm.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.fanxiaobao.xyz/Article/details/gndovxxpa.sHtML

csv.DictReader(f)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfzlumjgo.sHtML

[U26] Py：并发下载
来源：http://mobile.fanxiaobao.xyz/Article/details/ghadjaoqj.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvxccaqak.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbjnnlcen.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gimxoiltw.sHtML

[U28] Py：类型别名
来源：http://mobile.fanxiaobao.xyz/Article/details/gtdlgleht.sHtML

UserId = int
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmlthrzxn.sHtML

[U29] Py：属性校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnnhahago.sHtML

@property 与 @x.setter 配合
来源：http://blog.fanxiaobao.xyz/Article/details/giityqeyy.sHtML

[U30] Py：数据类
来源：http://baike.fanxiaobao.xyz/Article/details/gxcyqvdxf.sHtML

@dataclass(slots=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grhxuktji.sHtML

[U31] Py：单测
来源：http://3g.fanxiaobao.xyz/Article/details/gctnzmvwd.sHtML

python -m pytest -q
来源：http://3g.fanxiaobao.xyz/Article/details/gsefntgro.sHtML

[U32] Py：代码格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gcqxufmjn.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.fanxiaobao.xyz/Article/details/gwktdodup.sHtML

[U33] Py：打包发布
来源：http://mobile.fanxiaobao.xyz/Article/details/gyydthzzc.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.fanxiaobao.xyz/Article/details/gnqzgsann.sHtML

[U34] Py：判断编码
来源：http://wap.fanxiaobao.xyz/Article/details/gftrntbpr.sHtML

chardet.detect(raw)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggkyylkzo.sHtML

[U35] Py：发送邮件
来源：http://mobile.fanxiaobao.xyz/Article/details/gqytlotup.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpusxqjwq.sHtML

[U36] Py：定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/goanbatwg.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.fanxiaobao.xyz/Article/details/gfvvzhxig.sHtML

[U37] Py：读写 Excel
来源：http://www.share.fanxiaobao.xyz/Article/details/gybjjhlhr.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.fanxiaobao.xyz/Article/details/gozxclyky.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.fanxiaobao.xyz/Article/details/ghoyyhnyb.sHtML

Path(__file__).resolve().parent
来源：http://wap.fanxiaobao.xyz/Article/details/gvecxrqcf.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzpxpalbf.sHtML

sys.stdout.isatty()
来源：http://baike.fanxiaobao.xyz/Article/details/gsgfqhpak.sHtML

[U40] Py：打印到标准错误
来源：http://3g.fanxiaobao.xyz/Article/details/gxpwxqahk.sHtML

print("err", file=sys.stderr)
来源：http://baike.fanxiaobao.xyz/Article/details/gxjxzqhwx.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.fanxiaobao.xyz/Article/details/gwcumjbxe.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.fanxiaobao.xyz/Article/details/gwzsyiaje.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.fanxiaobao.xyz/Article/details/grlzqgjeq.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.fanxiaobao.xyz/Article/details/gkdtgmxkr.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmiykzzph.sHtML

namespace App\Http;
来源：http://read.share.fanxiaobao.xyz/Article/details/gyhvafeho.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gffotbips.sHtML

declare(strict_types=1);
来源：http://blog.fanxiaobao.xyz/Article/details/goxuailwn.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.fanxiaobao.xyz/Article/details/gddyrgold.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gaoiyhqsc.sHtML

[U46] PHP：可空类型
来源：http://blog.fanxiaobao.xyz/Article/details/gynhjtpwm.sHtML

?string $name = null
来源：http://m.share.fanxiaobao.xyz/Article/details/giooimwud.sHtML

[U47] PHP：联合类型
来源：http://3g.fanxiaobao.xyz/Article/details/gjodufodu.sHtML

int|string $id
来源：http://wap.fanxiaobao.xyz/Article/details/gujwwjbxg.sHtML

[U48] PHP：纯枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gbhchbjjo.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtrggbrui.sHtML

[U49] PHP：只读属性
来源：http://wap.fanxiaobao.xyz/Article/details/gneasweiz.sHtML

public readonly string $name
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwsqjbvwq.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.fanxiaobao.xyz/Article/details/gdiebnjwr.sHtML

public function __construct(private int $id) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gjiavttgw.sHtML

[U51] PHP：数组解构
来源：http://m.share.fanxiaobao.xyz/Article/details/gezwqeqzh.sHtML

[$a, $b] = $arr;
来源：http://m.share.fanxiaobao.xyz/Article/details/gplntkiqw.sHtML

[U52] PHP：箭头函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gxarwilpy.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.fanxiaobao.xyz/Article/details/gezpsuklr.sHtML

[U53] PHP：空合并运算符
来源：http://wap.fanxiaobao.xyz/Article/details/gzldvdaou.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.fanxiaobao.xyz/Article/details/gnkqlcxoe.sHtML

[U54] PHP：空安全调用
来源：http://blog.fanxiaobao.xyz/Article/details/gsiegcgzl.sHtML

$obj?->method()
来源：http://3g.fanxiaobao.xyz/Article/details/gononhrhn.sHtML

[U55] PHP：match 表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gwrjwbplo.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.fanxiaobao.xyz/Article/details/gssfkamjv.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtfqjuafj.sHtML

f(a: 1, b: 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gchrmtmea.sHtML

[U57] PHP：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/geqpqabdf.sHtML

"值: {$a}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gvmiihjpa.sHtML

[U58] PHP：数组三件套
来源：http://wap.fanxiaobao.xyz/Article/details/giptmedef.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.fanxiaobao.xyz/Article/details/gribsbqvc.sHtML

[U59] PHP：自定义排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gsikttedp.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gpcqzeakj.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.fanxiaobao.xyz/Article/details/gluzlrdgx.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.fanxiaobao.xyz/Article/details/gyjgvkwru.sHtML

[U61] PHP：正则
来源：http://wap.fanxiaobao.xyz/Article/details/grlfwrpns.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdbzgzyrm.sHtML

[U62] PHP：日期对象
来源：http://baike.fanxiaobao.xyz/Article/details/grueqxjjw.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghfefakqh.sHtML

[U63] PHP：文件读写
来源：http://mobile.fanxiaobao.xyz/Article/details/gdxgvrwac.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.fanxiaobao.xyz/Article/details/gcjlolpal.sHtML

[U64] PHP：目录遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/glpowfssp.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.fanxiaobao.xyz/Article/details/gnftulocl.sHtML

[U65] PHP：会话
来源：http://3g.fanxiaobao.xyz/Article/details/gjiomwbfm.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gqtbyaxjg.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.fanxiaobao.xyz/Article/details/gruiarpdl.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtovdkjux.sHtML

[U67] PHP：处理文件上传
来源：http://baike.fanxiaobao.xyz/Article/details/gzbgdvwqo.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvxzlkndm.sHtML

[U68] PHP：PDO 连接
来源：http://blog.fanxiaobao.xyz/Article/details/glabvcdra.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.fanxiaobao.xyz/Article/details/geryusqaj.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.fanxiaobao.xyz/Article/details/gaxhxdmsb.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghjiouviv.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gesfeqcki.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.fanxiaobao.xyz/Article/details/gebcmvxnu.sHtML

[U71] PHP：抛出异常
来源：http://3g.fanxiaobao.xyz/Article/details/gwenkflah.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmpsscmrl.sHtML

[U72] PHP：写错误日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gryehccut.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.fanxiaobao.xyz/Article/details/gpsmbgzfc.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.fanxiaobao.xyz/Article/details/grvmvtxkq.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.fanxiaobao.xyz/Article/details/gottvafor.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpeghbfak.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.fanxiaobao.xyz/Article/details/gnxdlmfic.sHtML

[U75] PHP：依赖注入
来源：http://wap.fanxiaobao.xyz/Article/details/ggnnnyswu.sHtML

composer require psr/container
来源：http://baike.fanxiaobao.xyz/Article/details/gmqkzqlco.sHtML

[U76] PHP：简单路由
来源：http://3g.fanxiaobao.xyz/Article/details/gviaamlid.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.fanxiaobao.xyz/Article/details/gkfciciau.sHtML

[U77] PHP：模板渲染
来源：http://wap.fanxiaobao.xyz/Article/details/gaqsovuma.sHtML

composer require twig/twig
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gihkesvpz.sHtML

[U78] PHP：单元测试
来源：http://read.share.fanxiaobao.xyz/Article/details/gxkqvunqw.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.fanxiaobao.xyz/Article/details/gzqqxvzod.sHtML

[U79] PHP：静态分析
来源：http://wap.fanxiaobao.xyz/Article/details/gnujmevhf.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.fanxiaobao.xyz/Article/details/gwjnqrsrx.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.fanxiaobao.xyz/Article/details/gselhfmfj.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.fanxiaobao.xyz/Article/details/gzbiglhpg.sHtML

[U81] JS：初始化项目
来源：http://www.blog.fanxiaobao.xyz/Article/details/gviyjscrs.sHtML

npm init -y;  npm i express
来源：http://baike.fanxiaobao.xyz/Article/details/gakcaftqr.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.fanxiaobao.xyz/Article/details/gdzhehguq.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.fanxiaobao.xyz/Article/details/gqrehvqlb.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.fanxiaobao.xyz/Article/details/guhxajxvl.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.fanxiaobao.xyz/Article/details/gsstadnfh.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.fanxiaobao.xyz/Article/details/gekaorclj.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.fanxiaobao.xyz/Article/details/gbokvnebm.sHtML

[U85] JS：可选链
来源：http://wap.fanxiaobao.xyz/Article/details/gvwrgusgt.sHtML

a?.b?.c
来源：http://blog.fanxiaobao.xyz/Article/details/gllhqnhbu.sHtML

[U86] JS：空值合并
来源：http://read.share.fanxiaobao.xyz/Article/details/gojvqvedg.sHtML

a ?? b
来源：http://blog.fanxiaobao.xyz/Article/details/ghmuxandg.sHtML

[U87] JS：解构默认值
来源：http://3g.fanxiaobao.xyz/Article/details/glafdvmqz.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggypnryac.sHtML

[U88] JS：对象展开合并
来源：http://blog.fanxiaobao.xyz/Article/details/glnkthbro.sHtML

{ ...a, ...b }
来源：http://wap.fanxiaobao.xyz/Article/details/gyqdsgozb.sHtML

[U89] JS：数组去重
来源：http://wap.fanxiaobao.xyz/Article/details/geqfbmysw.sHtML

[...new Set(arr)]
来源：http://read.share.fanxiaobao.xyz/Article/details/gglboncjn.sHtML

[U90] JS：数字数组排序
来源：http://read.share.fanxiaobao.xyz/Article/details/grnqacgrb.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.fanxiaobao.xyz/Article/details/ghzudhegn.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwbfmdeka.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.fanxiaobao.xyz/Article/details/gtznzroyy.sHtML

[U92] JS：深拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gjtbngxah.sHtML

structuredClone(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkqjsseem.sHtML

[U93] JS：模板字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gacrerpdm.sHtML

`共 ${n} 条`
来源：http://read.share.fanxiaobao.xyz/Article/details/ghdokcxmo.sHtML

[U94] JS：箭头函数
来源：http://baike.fanxiaobao.xyz/Article/details/gidwwnlqs.sHtML

const double = x => x * 2;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsdjvmuiu.sHtML

[U95] JS：Promise 包装
来源：http://mobile.fanxiaobao.xyz/Article/details/gjbnmqkvj.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.fanxiaobao.xyz/Article/details/gyonuteel.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gudlpatno.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.fanxiaobao.xyz/Article/details/grqsndjve.sHtML

[U97] JS：并发请求
来源：http://www.share.fanxiaobao.xyz/Article/details/gbkdgmlmf.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gidkhpkzr.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsbhltqms.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.fanxiaobao.xyz/Article/details/galzlzqys.sHtML

[U99] JS：事件监听
来源：http://mobile.fanxiaobao.xyz/Article/details/gxvibhpsc.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.fanxiaobao.xyz/Article/details/gnpgmovtq.sHtML

[U100] JS：DOM 查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gydkpmsvi.sHtML

document.querySelector(".item")
来源：http://m.share.fanxiaobao.xyz/Article/details/gyheduuwk.sHtML

[U101] JS：classList 操作
来源：http://read.share.fanxiaobao.xyz/Article/details/glizjcqlp.sHtML

el.classList.toggle("active")
来源：http://baike.fanxiaobao.xyz/Article/details/gyujouwxi.sHtML

[U102] JS：本地存储
来源：http://mobile.fanxiaobao.xyz/Article/details/gpnskyync.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.fanxiaobao.xyz/Article/details/gniuchpei.sHtML

[U103] JS：定时器
来源：http://baike.fanxiaobao.xyz/Article/details/gtgvqqvkw.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvuawrbqz.sHtML

[U104] JS：防抖
来源：http://wap.fanxiaobao.xyz/Article/details/goyiezgpt.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvepnkuhv.sHtML

[U105] JS：节流
来源：http://read.share.fanxiaobao.xyz/Article/details/gajekbpwg.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.fanxiaobao.xyz/Article/details/gxsfyazpa.sHtML

[U106] JS：日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gawruszuy.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.fanxiaobao.xyz/Article/details/gvpoqrucb.sHtML

[U107] JS：数字千分位
来源：http://3g.fanxiaobao.xyz/Article/details/gkhtvduzh.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.fanxiaobao.xyz/Article/details/guprdvaaq.sHtML

[U108] JS：随机整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gjmvtvjvb.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.fanxiaobao.xyz/Article/details/gfrnfxcdy.sHtML

[U109] JS：数组分组
来源：http://3g.fanxiaobao.xyz/Article/details/grplqbxvf.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.fanxiaobao.xyz/Article/details/gmavcqyse.sHtML

[U110] JS：数组分块
来源：http://wap.fanxiaobao.xyz/Article/details/gdrsqyrhh.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.fanxiaobao.xyz/Article/details/gsxkfdhwp.sHtML

[U111] JS：对象转 Map
来源：http://blog.fanxiaobao.xyz/Article/details/gzxvzyrkz.sHtML

new Map(Object.entries(obj))
来源：http://mobile.fanxiaobao.xyz/Article/details/gdymkhyen.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gprqcxcsi.sHtML

"7".padStart(3, "0")
来源：http://m.share.fanxiaobao.xyz/Article/details/gnihvozbj.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gocactizq.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqcrdmphu.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.fanxiaobao.xyz/Article/details/ghocnqndj.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcdssptfp.sHtML

[U115] JS：生成 UUID
来源：http://www.share.fanxiaobao.xyz/Article/details/gmhtfrwne.sHtML

crypto.randomUUID()
来源：http://mobile.fanxiaobao.xyz/Article/details/gycbckyyt.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.fanxiaobao.xyz/Article/details/gdzezjznk.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdvqbbglw.sHtML

[U117] JS：单元测试
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmfabehar.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.fanxiaobao.xyz/Article/details/givcibxgq.sHtML

[U118] JS：开发服务器
来源：http://read.share.fanxiaobao.xyz/Article/details/gnjidyqrc.sHtML

npm i -D vite;  npx vite
来源：http://www.share.fanxiaobao.xyz/Article/details/goaxhqzfm.sHtML

[U119] JS：生产构建
来源：http://www.share.fanxiaobao.xyz/Article/details/glsezhxtq.sHtML

npx vite build
来源：http://baike.fanxiaobao.xyz/Article/details/gdvassaic.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.fanxiaobao.xyz/Article/details/gjrxuxiho.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.fanxiaobao.xyz/Article/details/gcxgujjrw.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gvieimcpv.sHtML

统计汇总
来源：http://www.share.fanxiaobao.xyz/Article/details/gleplerwj.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gibadzsmp.sHtML

按语言统计（条）：
来源：http://m.share.fanxiaobao.xyz/Article/details/goqdhubjv.sHtML

Python ......... 252
来源：http://mobile.fanxiaobao.xyz/Article/details/gqgkwtuon.sHtML

PHP ............ 252
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gddjxlzve.sHtML

JavaScript ..... 252
来源：http://www.share.fanxiaobao.xyz/Article/details/gkfjxrvxw.sHtML

TypeScript ..... 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gkyzitbpq.sHtML

Java ........... 212
来源：http://baike.fanxiaobao.xyz/Article/details/gqabiodgo.sHtML

Go ............. 212
来源：http://m.share.fanxiaobao.xyz/Article/details/ganvinrca.sHtML

Ruby ........... 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gjxkdaxtp.sHtML

C# ............. 212
来源：http://baike.fanxiaobao.xyz/Article/details/gnsauxhcu.sHtML

C .............. 30
来源：http://blog.fanxiaobao.xyz/Article/details/gayvpucky.sHtML

C++ ............ 30
来源：http://mobile.fanxiaobao.xyz/Article/details/gccoqfufk.sHtML

SQL ............ 90
来源：http://www.blog.fanxiaobao.xyz/Article/details/gozsiqnyv.sHtML

Bash ........... 80
来源：http://blog.fanxiaobao.xyz/Article/details/gxybuewip.sHtML

Kotlin ......... 15
来源：http://m.share.fanxiaobao.xyz/Article/details/goncxcozj.sHtML

Swift .......... 15
来源：http://baike.fanxiaobao.xyz/Article/details/gtutsqati.sHtML

Lua ............ 10
来源：http://wap.fanxiaobao.xyz/Article/details/galosajgz.sHtML

Perl ........... 10
来源：http://blog.fanxiaobao.xyz/Article/details/gldjiqbae.sHtML

Scala .......... 10
来源：http://m.share.fanxiaobao.xyz/Article/details/goaqferit.sHtML

------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/gifchvfni.sHtML

合计 ........... 2106 条
来源：http://baike.fanxiaobao.xyz/Article/details/ghxyxbshl.sHtML

按章节统计：
来源：http://baike.fanxiaobao.xyz/Article/details/gyzyzhgnj.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxggsxyif.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.fanxiaobao.xyz/Article/details/gpyasljxj.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.fanxiaobao.xyz/Article/details/gnejuxqsi.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.fanxiaobao.xyz/Article/details/gegudtusx.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.fanxiaobao.xyz/Article/details/gsuzcyqhn.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.fanxiaobao.xyz/Article/details/gzzvtocst.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.fanxiaobao.xyz/Article/details/gpmbzdalc.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.fanxiaobao.xyz/Article/details/gxvgrzggh.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/gbaftblnw.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkgqzrkzt.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gdsgddjgd.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gdgxhscav.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gctorvkuz.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.fanxiaobao.xyz/Article/details/gbujpmvfy.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.fanxiaobao.xyz/Article/details/gdnucrjgq.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/gfrqaimcf.sHtML

Q SQL 专题                              90
来源：http://3g.fanxiaobao.xyz/Article/details/gniqicous.sHtML

R Bash 专题                             80
来源：http://wap.fanxiaobao.xyz/Article/details/gyqoolzih.sHtML

S C / C++ 专题                          60
来源：http://wap.fanxiaobao.xyz/Article/details/grzedslgq.sHtML

T 其他语言补充                          60
来源：http://m.share.fanxiaobao.xyz/Article/details/gocvthkgh.sHtML

U 高频实用片段                         120
来源：http://www.share.fanxiaobao.xyz/Article/details/ggyvjasoa.sHtML

------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/gpyfmetvn.sHtML

合计                                  2106 条
来源：http://www.share.fanxiaobao.xyz/Article/details/gysbqzvun.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/gbupjcqxs.sHtML

使用提醒
来源：http://mobile.fanxiaobao.xyz/Article/details/ghgashqrj.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkseklqcv.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcgbkguyi.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.fanxiaobao.xyz/Article/details/gvxmjseyu.sHtML


<!-- 参考信息 -->