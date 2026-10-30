代发 wailian999

[U01] Py：创建虚拟环境
来源：http://mobile.zdbjq.cn/Article/details/guuteauae.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.zdbjq.cn/Article/details/gaddclkja.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.fehbvm.com/Article/details/gdqhviwem.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.zdbjq.cn/Article/details/ghtqxitcr.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.zdbjq.cn/Article/details/gtstgjhao.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.zdbjq.cn/Article/details/gntsqmhuv.sHtML

[U04] Py：变量调试打印
来源：http://www.share.fehbvm.com/Article/details/gftbowrxr.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.zdbjq.cn/Article/details/gxylwqtpb.sHtML

[U05] Py：列表去重且保序
来源：http://3g.fehbvm.com/Article/details/gxhxzsqin.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.zdbjq.cn/Article/details/gydcsxfoy.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.fehbvm.com/Article/details/gitgjqyru.sHtML

{**a, **b}
来源：http://www.m.share.hesvh.cn/Article/details/gvtvhoyuu.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.hesvh.cn/Article/details/ggxexatpe.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.hesvh.cn/Article/details/gapodirge.sHtML

[U08] Py：展平二维列表
来源：http://wap.fehbvm.com/Article/details/gztwfiiss.sHtML

[y for x in nested for y in x]
来源：http://www.share.hesvh.cn/Article/details/gyauywhtd.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.hesvh.cn/Article/details/gjneaipoi.sHtML

max(d, key=d.get)
来源：http://baike.hesvh.cn/Article/details/gvibqtpel.sHtML

[U10] Py：按值排序字典
来源：http://blog.fehbvm.com/Article/details/gkvzfzyrp.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.hesvh.cn/Article/details/gibnahdkn.sHtML

[U11] Py：生成器表达式
来源：http://blog.zdbjq.cn/Article/details/gmdlfolfx.sHtML

(x * 2 for x in arr)
来源：http://www.blog.fehbvm.com/Article/details/gegqbgfdm.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.fehbvm.com/Article/details/gssglngpn.sHtML

Counter(arr).most_common(3)
来源：http://blog.zdbjq.cn/Article/details/gffbaithe.sHtML

[U13] Py：固定长度队列
来源：http://3g.zdbjq.cn/Article/details/gsjeqdyvv.sHtML

deque(maxlen=10)
来源：http://www.blog.hesvh.cn/Article/details/gyxarkhaj.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.hesvh.cn/Article/details/gdfrmqhxr.sHtML

defaultdict(list)
来源：http://3g.zdbjq.cn/Article/details/gdlcypjiu.sHtML

[U15] Py：高精度计时
来源：http://m.share.hesvh.cn/Article/details/gdsasafwf.sHtML

t = time.perf_counter()
来源：http://www.m.share.zdbjq.cn/Article/details/gktesfnny.sHtML

[U16] Py：命令行参数解析
来源：http://baike.fehbvm.com/Article/details/gxhdbiclq.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.hesvh.cn/Article/details/gtpdypafb.sHtML

[U17] Py：初始化日志
来源：http://wap.fehbvm.com/Article/details/gbxnkxzhl.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.hesvh.cn/Article/details/glzujsjhl.sHtML

[U18] Py：预编译正则
来源：http://mobile.hesvh.cn/Article/details/gznwioajj.sHtML

pat = re.compile(r"\d+")
来源：http://wap.fehbvm.com/Article/details/gaovwamvc.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.hesvh.cn/Article/details/grujbhesj.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fehbvm.com/Article/details/gyyhjnrvd.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.hesvh.cn/Article/details/grsmcynze.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.zdbjq.cn/Article/details/gehpkybdo.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.hesvh.cn/Article/details/gwdyjuawb.sHtML

@contextlib.contextmanager
来源：http://mobile.zdbjq.cn/Article/details/gouhlhdmd.sHtML

[U22] Py：矩阵转置
来源：http://www.share.zdbjq.cn/Article/details/gprncktza.sHtML

list(zip(*m))
来源：http://3g.fehbvm.com/Article/details/gpmgfrsxp.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.hesvh.cn/Article/details/gsahyoede.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.hesvh.cn/Article/details/gprtqcnjd.sHtML

[U24] Py：路径操作
来源：http://www.m.share.zdbjq.cn/Article/details/gfguzamkh.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.fehbvm.com/Article/details/gxujstxoo.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.hesvh.cn/Article/details/gjsmszxqs.sHtML

csv.DictReader(f)
来源：http://www.m.share.hesvh.cn/Article/details/gwnfllamk.sHtML

[U26] Py：并发下载
来源：http://www.share.hesvh.cn/Article/details/gttifvoiz.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.hesvh.cn/Article/details/gxglstayo.sHtML

[U27] Py：异步 HTTP
来源：http://3g.fehbvm.com/Article/details/gvafooqcv.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.hesvh.cn/Article/details/gzoqncaki.sHtML

[U28] Py：类型别名
来源：http://wap.fehbvm.com/Article/details/ggcjorglq.sHtML

UserId = int
来源：http://mobile.zdbjq.cn/Article/details/gpywxkywm.sHtML

[U29] Py：属性校验
来源：http://baike.fehbvm.com/Article/details/gjexyakqn.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.fehbvm.com/Article/details/gkrbzbmgj.sHtML

[U30] Py：数据类
来源：http://3g.fehbvm.com/Article/details/gtjxkyljk.sHtML

@dataclass(slots=True)
来源：http://read.share.zdbjq.cn/Article/details/gfqkmgqkj.sHtML

[U31] Py：单测
来源：http://wap.zdbjq.cn/Article/details/gejppsrpw.sHtML

python -m pytest -q
来源：http://read.share.fehbvm.com/Article/details/gyqworpir.sHtML

[U32] Py：代码格式化
来源：http://blog.fehbvm.com/Article/details/gyqeybpqw.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.zdbjq.cn/Article/details/gzjmapndo.sHtML

[U33] Py：打包发布
来源：http://mobile.zdbjq.cn/Article/details/gwrzbgnew.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.hesvh.cn/Article/details/gasbnipbf.sHtML

[U34] Py：判断编码
来源：http://www.share.hesvh.cn/Article/details/gxarelmfg.sHtML

chardet.detect(raw)
来源：http://read.share.hesvh.cn/Article/details/gsbzbbflb.sHtML

[U35] Py：发送邮件
来源：http://wap.hesvh.cn/Article/details/gtgiqhbbz.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.hesvh.cn/Article/details/grvwuugkw.sHtML

[U36] Py：定时任务
来源：http://www.blog.hesvh.cn/Article/details/gamatgyfe.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.hesvh.cn/Article/details/gdzffxiuu.sHtML

[U37] Py：读写 Excel
来源：http://read.share.zdbjq.cn/Article/details/gcwgfqvim.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.hesvh.cn/Article/details/gxvedyriq.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.zdbjq.cn/Article/details/gmfhovplz.sHtML

Path(__file__).resolve().parent
来源：http://read.share.hesvh.cn/Article/details/ggklgbhqw.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.fehbvm.com/Article/details/gjhimmkka.sHtML

sys.stdout.isatty()
来源：http://www.m.share.fehbvm.com/Article/details/gohgkffoc.sHtML

[U40] Py：打印到标准错误
来源：http://baike.fehbvm.com/Article/details/gquxsfski.sHtML

print("err", file=sys.stderr)
来源：http://wap.hesvh.cn/Article/details/gaslawjas.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.fehbvm.com/Article/details/gozrhcwta.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.zdbjq.cn/Article/details/gknhpselo.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.hesvh.cn/Article/details/gwniprqmo.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.fehbvm.com/Article/details/gotbcrgyx.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.zdbjq.cn/Article/details/gessvlhmt.sHtML

namespace App\Http;
来源：http://3g.fehbvm.com/Article/details/ghddciild.sHtML

[U44] PHP：开启严格类型
来源：http://blog.fehbvm.com/Article/details/gyxjorlil.sHtML

declare(strict_types=1);
来源：http://mobile.fehbvm.com/Article/details/gtcalaaka.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.fehbvm.com/Article/details/guhshwogn.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/grmvfprvo.sHtML

[U46] PHP：可空类型
来源：http://mobile.zdbjq.cn/Article/details/guxzhvmre.sHtML

?string $name = null
来源：http://mobile.hesvh.cn/Article/details/gxsqpsvgv.sHtML

[U47] PHP：联合类型
来源：http://wap.zdbjq.cn/Article/details/gyxfseqoi.sHtML

int|string $id
来源：http://m.share.hesvh.cn/Article/details/gcboxuuak.sHtML

[U48] PHP：纯枚举
来源：http://mobile.fehbvm.com/Article/details/gohxyzqhv.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.fehbvm.com/Article/details/gjsmihpam.sHtML

[U49] PHP：只读属性
来源：http://mobile.zdbjq.cn/Article/details/gwapyfwtf.sHtML

public readonly string $name
来源：http://read.share.fehbvm.com/Article/details/gtnqhrkkh.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.fehbvm.com/Article/details/gnpqpyjvx.sHtML

public function __construct(private int $id) {}
来源：http://blog.hesvh.cn/Article/details/gfvpuglnu.sHtML

[U51] PHP：数组解构
来源：http://baike.zdbjq.cn/Article/details/ghodrchrr.sHtML

[$a, $b] = $arr;
来源：http://m.share.fehbvm.com/Article/details/gsfwxdmxo.sHtML

[U52] PHP：箭头函数
来源：http://read.share.zdbjq.cn/Article/details/gqpjxcwhm.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.hesvh.cn/Article/details/gdzffggvv.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.zdbjq.cn/Article/details/gmwfzimel.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.hesvh.cn/Article/details/glneyxsnh.sHtML

[U54] PHP：空安全调用
来源：http://blog.fehbvm.com/Article/details/glapijcow.sHtML

$obj?->method()
来源：http://wap.hesvh.cn/Article/details/gszhkwwfy.sHtML

[U55] PHP：match 表达式
来源：http://www.share.hesvh.cn/Article/details/glpqghyri.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.zdbjq.cn/Article/details/gltoowsyl.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.hesvh.cn/Article/details/gndcgvwlj.sHtML

f(a: 1, b: 2)
来源：http://www.blog.fehbvm.com/Article/details/gztorwyvn.sHtML

[U57] PHP：字符串插值
来源：http://read.share.hesvh.cn/Article/details/guymxsskg.sHtML

"值: {$a}"
来源：http://www.blog.fehbvm.com/Article/details/grjyjuzbv.sHtML

[U58] PHP：数组三件套
来源：http://blog.hesvh.cn/Article/details/gtxreavdg.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.zdbjq.cn/Article/details/gtsswpege.sHtML

[U59] PHP：自定义排序
来源：http://blog.zdbjq.cn/Article/details/gnschqrom.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.hesvh.cn/Article/details/ggkzkyitv.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.zdbjq.cn/Article/details/gvrgwnrgk.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.fehbvm.com/Article/details/grhhwaogv.sHtML

[U61] PHP：正则
来源：http://m.share.hesvh.cn/Article/details/gvlggbtrp.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.hesvh.cn/Article/details/gzrzgsvil.sHtML

[U62] PHP：日期对象
来源：http://www.share.zdbjq.cn/Article/details/gnjxcuamd.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.fehbvm.com/Article/details/gjmvxopsf.sHtML

[U63] PHP：文件读写
来源：http://www.share.zdbjq.cn/Article/details/gabvlirlh.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.zdbjq.cn/Article/details/gawkrrdew.sHtML

[U64] PHP：目录遍历
来源：http://m.share.hesvh.cn/Article/details/gsihhmjqs.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.zdbjq.cn/Article/details/gazixpabg.sHtML

[U65] PHP：会话
来源：http://3g.hesvh.cn/Article/details/gvkacxdea.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gczypmrhs.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.zdbjq.cn/Article/details/gqaqarogo.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.fehbvm.com/Article/details/gjaqlfzdm.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.hesvh.cn/Article/details/gftdibyzq.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.fehbvm.com/Article/details/gpsedunng.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.fehbvm.com/Article/details/gzbhontfr.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.hesvh.cn/Article/details/gqsriimqs.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.hesvh.cn/Article/details/gltzwskyk.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.zdbjq.cn/Article/details/gvufhrsgg.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.fehbvm.com/Article/details/gpmagglid.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.hesvh.cn/Article/details/gkaizvlut.sHtML

[U71] PHP：抛出异常
来源：http://www.share.fehbvm.com/Article/details/gnfvwfwaj.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.zdbjq.cn/Article/details/gijdjbhaa.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.hesvh.cn/Article/details/gxeftaadl.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.fehbvm.com/Article/details/gubnfaztm.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.hesvh.cn/Article/details/gczxnxohm.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.fehbvm.com/Article/details/gfoisgvpk.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.fehbvm.com/Article/details/gpcmzhnpo.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.hesvh.cn/Article/details/gehuaqaar.sHtML

[U75] PHP：依赖注入
来源：http://baike.hesvh.cn/Article/details/gwepmwsfh.sHtML

composer require psr/container
来源：http://www.m.share.fehbvm.com/Article/details/gbfmolejz.sHtML

[U76] PHP：简单路由
来源：http://3g.zdbjq.cn/Article/details/giqhwnnov.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.hesvh.cn/Article/details/gapsgbrzm.sHtML

[U77] PHP：模板渲染
来源：http://m.share.fehbvm.com/Article/details/gxegnwock.sHtML

composer require twig/twig
来源：http://read.share.zdbjq.cn/Article/details/gbtutrtlf.sHtML

[U78] PHP：单元测试
来源：http://www.blog.hesvh.cn/Article/details/gglcduzdw.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.hesvh.cn/Article/details/gypqjprop.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.fehbvm.com/Article/details/glgpfudjw.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.fehbvm.com/Article/details/gsbuerzgt.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.zdbjq.cn/Article/details/gksagmfyx.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.zdbjq.cn/Article/details/gdrkaqodz.sHtML

[U81] JS：初始化项目
来源：http://3g.zdbjq.cn/Article/details/gpfgslwfk.sHtML

npm init -y;  npm i express
来源：http://blog.hesvh.cn/Article/details/ghdblmszd.sHtML

[U82] JS：package.json 脚本
来源：http://baike.hesvh.cn/Article/details/gqprjfbhz.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.fehbvm.com/Article/details/gbzefnozu.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.fehbvm.com/Article/details/gzzwgduxt.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.hesvh.cn/Article/details/gnolzhxnv.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.fehbvm.com/Article/details/gicsqprbe.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.zdbjq.cn/Article/details/goijcknig.sHtML

[U85] JS：可选链
来源：http://wap.hesvh.cn/Article/details/ggzfwnxnp.sHtML

a?.b?.c
来源：http://m.share.hesvh.cn/Article/details/ghhoatqsb.sHtML

[U86] JS：空值合并
来源：http://wap.hesvh.cn/Article/details/gpmmplugw.sHtML

a ?? b
来源：http://www.share.fehbvm.com/Article/details/gpepaugwm.sHtML

[U87] JS：解构默认值
来源：http://www.blog.hesvh.cn/Article/details/ghjjtopsz.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.hesvh.cn/Article/details/glevholuj.sHtML

[U88] JS：对象展开合并
来源：http://3g.fehbvm.com/Article/details/gegqxikvr.sHtML

{ ...a, ...b }
来源：http://baike.fehbvm.com/Article/details/gioxbmcqi.sHtML

[U89] JS：数组去重
来源：http://wap.hesvh.cn/Article/details/gvlzujtcz.sHtML

[...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/gyhotaicz.sHtML

[U90] JS：数字数组排序
来源：http://blog.zdbjq.cn/Article/details/gyquanemy.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/ggeftrwzf.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.fehbvm.com/Article/details/gwcluelpz.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.fehbvm.com/Article/details/gimdsrpyi.sHtML

[U92] JS：深拷贝
来源：http://www.share.fehbvm.com/Article/details/gqztphxym.sHtML

structuredClone(obj)
来源：http://mobile.fehbvm.com/Article/details/gqyabguhh.sHtML

[U93] JS：模板字符串
来源：http://blog.zdbjq.cn/Article/details/glnpnvfyl.sHtML

`共 ${n} 条`
来源：http://read.share.hesvh.cn/Article/details/genmleier.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.hesvh.cn/Article/details/gjehfaqzs.sHtML

const double = x => x * 2;
来源：http://read.share.fehbvm.com/Article/details/gldbtfozx.sHtML

[U95] JS：Promise 包装
来源：http://www.share.fehbvm.com/Article/details/gwbccarno.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.hesvh.cn/Article/details/ggzuwphck.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.hesvh.cn/Article/details/ggzggqfnd.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/gwknalgxp.sHtML

[U97] JS：并发请求
来源：http://www.m.share.zdbjq.cn/Article/details/gvrbwoxoe.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gjfgagpuy.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.zdbjq.cn/Article/details/gpewkacxu.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.zdbjq.cn/Article/details/goybnursk.sHtML

[U99] JS：事件监听
来源：http://blog.zdbjq.cn/Article/details/gctsakxth.sHtML

el.addEventListener("click", e => {})
来源：http://baike.fehbvm.com/Article/details/gctfgefce.sHtML

[U100] JS：DOM 查询
来源：http://baike.fehbvm.com/Article/details/gonratbsd.sHtML

document.querySelector(".item")
来源：http://www.share.fehbvm.com/Article/details/gbgklqkfz.sHtML

[U101] JS：classList 操作
来源：http://blog.fehbvm.com/Article/details/gfonkyrxk.sHtML

el.classList.toggle("active")
来源：http://read.share.zdbjq.cn/Article/details/gxijnakxs.sHtML

[U102] JS：本地存储
来源：http://m.share.hesvh.cn/Article/details/gxlakxvgs.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.zdbjq.cn/Article/details/gkznfkmml.sHtML

[U103] JS：定时器
来源：http://baike.fehbvm.com/Article/details/gmujyzmju.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.fehbvm.com/Article/details/gbtffvdla.sHtML

[U104] JS：防抖
来源：http://blog.hesvh.cn/Article/details/gpyecbqhs.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/gqewjyxii.sHtML

[U105] JS：节流
来源：http://baike.fehbvm.com/Article/details/ghahvghzl.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.fehbvm.com/Article/details/gsqovxjit.sHtML

[U106] JS：日期格式化
来源：http://blog.fehbvm.com/Article/details/gwruyrwrg.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.hesvh.cn/Article/details/gurnskvuy.sHtML

[U107] JS：数字千分位
来源：http://3g.zdbjq.cn/Article/details/gehphtnbh.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.zdbjq.cn/Article/details/gyzxowaop.sHtML

[U108] JS：随机整数
来源：http://blog.zdbjq.cn/Article/details/gnctzbauh.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.zdbjq.cn/Article/details/gaguoslas.sHtML

[U109] JS：数组分组
来源：http://read.share.fehbvm.com/Article/details/gewomcvyu.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.hesvh.cn/Article/details/gwiqfnqgi.sHtML

[U110] JS：数组分块
来源：http://wap.hesvh.cn/Article/details/gahgfggjp.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.hesvh.cn/Article/details/gmhselfsf.sHtML

[U111] JS：对象转 Map
来源：http://blog.zdbjq.cn/Article/details/gxhquaiyk.sHtML

new Map(Object.entries(obj))
来源：http://read.share.fehbvm.com/Article/details/gxytddwwy.sHtML

[U112] JS：字符串补位
来源：http://blog.zdbjq.cn/Article/details/gkvfeljbg.sHtML

"7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gpvxwxyiv.sHtML

[U113] JS：正则替换全部
来源：http://3g.fehbvm.com/Article/details/gwaikxkky.sHtML

s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gpnlbkhcu.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.zdbjq.cn/Article/details/gyrniwdvd.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.hesvh.cn/Article/details/ginowjsdl.sHtML

[U115] JS：生成 UUID
来源：http://m.share.fehbvm.com/Article/details/gzmnfqfdy.sHtML

crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/ghrmnvzbk.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.fehbvm.com/Article/details/gtfeekslk.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.fehbvm.com/Article/details/gcipashae.sHtML

[U117] JS：单元测试
来源：http://read.share.hesvh.cn/Article/details/gpqeadvei.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.fehbvm.com/Article/details/gxdctusrr.sHtML

[U118] JS：开发服务器
来源：http://read.share.hesvh.cn/Article/details/gbwfkdedv.sHtML

npm i -D vite;  npx vite
来源：http://m.share.hesvh.cn/Article/details/ggcpdsgcs.sHtML

[U119] JS：生产构建
来源：http://baike.fehbvm.com/Article/details/gvlcwehmv.sHtML

npx vite build
来源：http://www.blog.fehbvm.com/Article/details/gglfhryze.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.fehbvm.com/Article/details/grktgrbvh.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.zdbjq.cn/Article/details/gwofyrrkp.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/grhcbgzfu.sHtML

统计汇总
来源：http://wap.fehbvm.com/Article/details/gdqjcxvvi.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/glbgvpnwx.sHtML

按语言统计（条）：
来源：http://mobile.zdbjq.cn/Article/details/gampacrow.sHtML

Python ......... 252
来源：http://www.share.zdbjq.cn/Article/details/glbjtkhfe.sHtML

PHP ............ 252
来源：http://m.share.zdbjq.cn/Article/details/gdajycmyj.sHtML

JavaScript ..... 252
来源：http://read.share.zdbjq.cn/Article/details/gddrrcipl.sHtML

TypeScript ..... 212
来源：http://baike.zdbjq.cn/Article/details/gtzqbikzm.sHtML

Java ........... 212
来源：http://www.blog.hesvh.cn/Article/details/glcprxzll.sHtML

Go ............. 212
来源：http://read.share.hesvh.cn/Article/details/gzraxkjdk.sHtML

Ruby ........... 212
来源：http://m.share.fehbvm.com/Article/details/gtlzfgzmq.sHtML

C# ............. 212
来源：http://wap.fehbvm.com/Article/details/gteynlzmr.sHtML

C .............. 30
来源：http://mobile.hesvh.cn/Article/details/ghgurqvvy.sHtML

C++ ............ 30
来源：http://mobile.fehbvm.com/Article/details/gkbuszasm.sHtML

SQL ............ 90
来源：http://www.m.share.zdbjq.cn/Article/details/grprjlumi.sHtML

Bash ........... 80
来源：http://blog.zdbjq.cn/Article/details/gujscdspm.sHtML

Kotlin ......... 15
来源：http://baike.hesvh.cn/Article/details/gmqbgehww.sHtML

Swift .......... 15
来源：http://read.share.zdbjq.cn/Article/details/gnzwphobb.sHtML

Lua ............ 10
来源：http://baike.hesvh.cn/Article/details/ghjmikxox.sHtML

Perl ........... 10
来源：http://www.share.fehbvm.com/Article/details/gxkjqcily.sHtML

Scala .......... 10
来源：http://www.blog.hesvh.cn/Article/details/godkvzvto.sHtML

------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gqogfqcyf.sHtML

合计 ........... 2106 条
来源：http://wap.zdbjq.cn/Article/details/gzxpzmtnk.sHtML

按章节统计：
来源：http://m.share.hesvh.cn/Article/details/gcgzbgrls.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.fehbvm.com/Article/details/gbpycjiyk.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.fehbvm.com/Article/details/grnommjga.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.hesvh.cn/Article/details/gpfslujcl.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.zdbjq.cn/Article/details/ggmiphcsz.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.hesvh.cn/Article/details/gqnayobeb.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.zdbjq.cn/Article/details/gyebutjtl.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.hesvh.cn/Article/details/gtuwwsuis.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.hesvh.cn/Article/details/ggrxvslum.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gbnauyjkx.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.fehbvm.com/Article/details/gwoyfbgdn.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gfntuzybt.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gudazrbkv.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gvylnxzeh.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.hesvh.cn/Article/details/gwchivfeq.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.hesvh.cn/Article/details/gximchuft.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/genlxnaik.sHtML

Q SQL 专题                              90
来源：http://mobile.fehbvm.com/Article/details/gbteyybrg.sHtML

R Bash 专题                             80
来源：http://m.share.hesvh.cn/Article/details/garjzrnch.sHtML

S C / C++ 专题                          60
来源：http://blog.hesvh.cn/Article/details/gqaxdlcvr.sHtML

T 其他语言补充                          60
来源：http://www.share.hesvh.cn/Article/details/gasyrgoic.sHtML

U 高频实用片段                         120
来源：http://blog.fehbvm.com/Article/details/gyovikewt.sHtML

------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gpvqtycet.sHtML

合计                                  2106 条
来源：http://mobile.zdbjq.cn/Article/details/gedipknjw.sHtML

--------------------------------------------------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gtgxeirhv.sHtML

使用提醒
来源：http://mobile.fehbvm.com/Article/details/gwaolzcga.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/glhkjlkut.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.hesvh.cn/Article/details/gzlauiudx.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.fehbvm.com/Article/details/gidoconia.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.hesvh.cn/Article/details/gvfcgqqfj.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.zdbjq.cn/Article/details/ggkjpvgfv.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.zdbjq.cn/Article/details/gtfksxqvi.sHtML

—— 文件结束 ——
来源：http://wap.zdbjq.cn/Article/details/geteizypq.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ghengesnj.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.fehbvm.com/Article/details/gevfxlgpu.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.hesvh.cn/Article/details/gqazkwzqf.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ggtdfgdit.sHtML


<!-- 参考信息 -->