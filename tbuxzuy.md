代发 wailian999

[U01] Py：创建虚拟环境
来源：http://www.blog.hesvh.cn/Article/details/gglargjuy.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.zdbjq.cn/Article/details/goidxalbe.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.zdbjq.cn/Article/details/goclbcyhd.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.hesvh.cn/Article/details/gttbdaswh.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.zdbjq.cn/Article/details/gbeapquzq.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.fehbvm.com/Article/details/gcnkuhxyl.sHtML

[U04] Py：变量调试打印
来源：http://blog.zdbjq.cn/Article/details/gzvshiinn.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.hesvh.cn/Article/details/ggyehosue.sHtML

[U05] Py：列表去重且保序
来源：http://blog.zdbjq.cn/Article/details/ggfahwdft.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.fehbvm.com/Article/details/gohuxwrxk.sHtML

[U06] Py：合并两个字典
来源：http://baike.hesvh.cn/Article/details/gpwjifvcb.sHtML

{**a, **b}
来源：http://3g.zdbjq.cn/Article/details/gdsezagxy.sHtML

[U07] Py：反转字典键值
来源：http://wap.zdbjq.cn/Article/details/gcvngktbw.sHtML

{v: k for k, v in d.items()}
来源：http://baike.zdbjq.cn/Article/details/gprvpabeo.sHtML

[U08] Py：展平二维列表
来源：http://3g.zdbjq.cn/Article/details/gqjugmlwa.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.fehbvm.com/Article/details/gbrtbxohu.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.zdbjq.cn/Article/details/gnlvsyprp.sHtML

max(d, key=d.get)
来源：http://www.blog.hesvh.cn/Article/details/gbvdeggoe.sHtML

[U10] Py：按值排序字典
来源：http://baike.zdbjq.cn/Article/details/gyykwhhge.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.zdbjq.cn/Article/details/gouzenavv.sHtML

[U11] Py：生成器表达式
来源：http://read.share.zdbjq.cn/Article/details/grrajafkk.sHtML

(x * 2 for x in arr)
来源：http://baike.hesvh.cn/Article/details/guvnnctvp.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.hesvh.cn/Article/details/grgrspeyu.sHtML

Counter(arr).most_common(3)
来源：http://www.share.hesvh.cn/Article/details/gcybfnhnf.sHtML

[U13] Py：固定长度队列
来源：http://3g.hesvh.cn/Article/details/glrzvutdd.sHtML

deque(maxlen=10)
来源：http://m.share.hesvh.cn/Article/details/gfelmnxia.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.zdbjq.cn/Article/details/goyexypfr.sHtML

defaultdict(list)
来源：http://wap.zdbjq.cn/Article/details/gdofsovdj.sHtML

[U15] Py：高精度计时
来源：http://wap.fehbvm.com/Article/details/gfwalfwgj.sHtML

t = time.perf_counter()
来源：http://read.share.hesvh.cn/Article/details/gttfiguwc.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.zdbjq.cn/Article/details/gdsodlxlw.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.zdbjq.cn/Article/details/gtxhpcadz.sHtML

[U17] Py：初始化日志
来源：http://www.blog.fehbvm.com/Article/details/gdowydssn.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.hesvh.cn/Article/details/gmdnhtnsz.sHtML

[U18] Py：预编译正则
来源：http://wap.fehbvm.com/Article/details/gxkmtgala.sHtML

pat = re.compile(r"\d+")
来源：http://blog.zdbjq.cn/Article/details/gwhzvwndc.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.fehbvm.com/Article/details/glebntrkw.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.zdbjq.cn/Article/details/gifseifqn.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.fehbvm.com/Article/details/gojfgmpvn.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.hesvh.cn/Article/details/genjrhwdq.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.zdbjq.cn/Article/details/gxiaajrmp.sHtML

@contextlib.contextmanager
来源：http://baike.zdbjq.cn/Article/details/gvinmkmtn.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.hesvh.cn/Article/details/ghwmrgpdl.sHtML

list(zip(*m))
来源：http://blog.fehbvm.com/Article/details/gwnguvjew.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.zdbjq.cn/Article/details/gjaqptjoc.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.fehbvm.com/Article/details/gycnmfark.sHtML

[U24] Py：路径操作
来源：http://www.blog.zdbjq.cn/Article/details/gofijvika.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.hesvh.cn/Article/details/guawcmlat.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.zdbjq.cn/Article/details/gomlysobx.sHtML

csv.DictReader(f)
来源：http://baike.hesvh.cn/Article/details/guwutihza.sHtML

[U26] Py：并发下载
来源：http://read.share.zdbjq.cn/Article/details/gbmfpnavn.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.hesvh.cn/Article/details/ggpvudrqv.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.fehbvm.com/Article/details/gipmjragi.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.zdbjq.cn/Article/details/griwvzudv.sHtML

[U28] Py：类型别名
来源：http://www.share.zdbjq.cn/Article/details/gdbjnujzy.sHtML

UserId = int
来源：http://3g.fehbvm.com/Article/details/gshuxecxp.sHtML

[U29] Py：属性校验
来源：http://www.m.share.hesvh.cn/Article/details/grwszlxql.sHtML

@property 与 @x.setter 配合
来源：http://m.share.hesvh.cn/Article/details/gkkfgqmho.sHtML

[U30] Py：数据类
来源：http://3g.zdbjq.cn/Article/details/gwqxmjxxu.sHtML

@dataclass(slots=True)
来源：http://wap.fehbvm.com/Article/details/gbsuxzxze.sHtML

[U31] Py：单测
来源：http://blog.zdbjq.cn/Article/details/gdlcktacc.sHtML

python -m pytest -q
来源：http://www.m.share.hesvh.cn/Article/details/guzanmjgk.sHtML

[U32] Py：代码格式化
来源：http://mobile.hesvh.cn/Article/details/gedshtwrl.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.fehbvm.com/Article/details/ghydwzeoj.sHtML

[U33] Py：打包发布
来源：http://www.blog.zdbjq.cn/Article/details/gfdbtbntj.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.fehbvm.com/Article/details/gaodgemjk.sHtML

[U34] Py：判断编码
来源：http://wap.fehbvm.com/Article/details/gnqytuzzv.sHtML

chardet.detect(raw)
来源：http://3g.fehbvm.com/Article/details/gpdeqzcqw.sHtML

[U35] Py：发送邮件
来源：http://www.share.hesvh.cn/Article/details/gxvjflwrt.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.zdbjq.cn/Article/details/gmuhefoqx.sHtML

[U36] Py：定时任务
来源：http://m.share.zdbjq.cn/Article/details/gvwmniazi.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.hesvh.cn/Article/details/glpattnxl.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.fehbvm.com/Article/details/ghilrxrdd.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.hesvh.cn/Article/details/gueabhxgy.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fehbvm.com/Article/details/gfrdjzkcu.sHtML

Path(__file__).resolve().parent
来源：http://baike.zdbjq.cn/Article/details/gwhprmhbt.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.zdbjq.cn/Article/details/gtyzczzqh.sHtML

sys.stdout.isatty()
来源：http://www.share.zdbjq.cn/Article/details/gehmaalfp.sHtML

[U40] Py：打印到标准错误
来源：http://baike.fehbvm.com/Article/details/gdfmkvvea.sHtML

print("err", file=sys.stderr)
来源：http://m.share.fehbvm.com/Article/details/gqclvknos.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.hesvh.cn/Article/details/glonaeiha.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.hesvh.cn/Article/details/gcqgoilaj.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.hesvh.cn/Article/details/grlxfrsxh.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.zdbjq.cn/Article/details/gvfrfjtos.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.zdbjq.cn/Article/details/ghgfkejar.sHtML

namespace App\Http;
来源：http://www.share.hesvh.cn/Article/details/grhxwtifi.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.zdbjq.cn/Article/details/ghosinyki.sHtML

declare(strict_types=1);
来源：http://www.blog.fehbvm.com/Article/details/guldtnvkl.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.fehbvm.com/Article/details/gnmblfasv.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gittqsvvy.sHtML

[U46] PHP：可空类型
来源：http://3g.zdbjq.cn/Article/details/grtmlhcrr.sHtML

?string $name = null
来源：http://www.m.share.fehbvm.com/Article/details/gcpdzwemq.sHtML

[U47] PHP：联合类型
来源：http://read.share.hesvh.cn/Article/details/gudfgbrtp.sHtML

int|string $id
来源：http://3g.hesvh.cn/Article/details/gmqrklfkh.sHtML

[U48] PHP：纯枚举
来源：http://m.share.fehbvm.com/Article/details/gjqbeptzd.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.zdbjq.cn/Article/details/gcwgrjsej.sHtML

[U49] PHP：只读属性
来源：http://blog.zdbjq.cn/Article/details/gmvaighha.sHtML

public readonly string $name
来源：http://wap.hesvh.cn/Article/details/glkizigur.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.zdbjq.cn/Article/details/gbuqepbwj.sHtML

public function __construct(private int $id) {}
来源：http://baike.zdbjq.cn/Article/details/gvnoumaeu.sHtML

[U51] PHP：数组解构
来源：http://mobile.hesvh.cn/Article/details/gyhpkscjr.sHtML

[$a, $b] = $arr;
来源：http://baike.fehbvm.com/Article/details/gsffhwjvz.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.zdbjq.cn/Article/details/grlucliwh.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.hesvh.cn/Article/details/gcwpockrq.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.fehbvm.com/Article/details/grayvzbho.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.hesvh.cn/Article/details/gqzxqwxhz.sHtML

[U54] PHP：空安全调用
来源：http://read.share.zdbjq.cn/Article/details/gpyuxpaec.sHtML

$obj?->method()
来源：http://mobile.fehbvm.com/Article/details/gjcrbwbwi.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.zdbjq.cn/Article/details/garjkwgmm.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.zdbjq.cn/Article/details/gkhrxcdtj.sHtML

[U56] PHP：命名参数
来源：http://m.share.hesvh.cn/Article/details/gphrtytwa.sHtML

f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/gvsgktmpt.sHtML

[U57] PHP：字符串插值
来源：http://www.share.fehbvm.com/Article/details/ggsoxqahr.sHtML

"值: {$a}"
来源：http://blog.zdbjq.cn/Article/details/gzjtmsmas.sHtML

[U58] PHP：数组三件套
来源：http://3g.hesvh.cn/Article/details/gdfgexwmk.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.fehbvm.com/Article/details/gcnktfdew.sHtML

[U59] PHP：自定义排序
来源：http://mobile.fehbvm.com/Article/details/gvvbaqkbn.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fehbvm.com/Article/details/gjxbpshvn.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.hesvh.cn/Article/details/gtfiavajr.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.hesvh.cn/Article/details/guiyuwvkp.sHtML

[U61] PHP：正则
来源：http://m.share.hesvh.cn/Article/details/glvbegqlk.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.zdbjq.cn/Article/details/gaquefaql.sHtML

[U62] PHP：日期对象
来源：http://blog.fehbvm.com/Article/details/gkmwqfgeg.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.fehbvm.com/Article/details/giijgongs.sHtML

[U63] PHP：文件读写
来源：http://wap.hesvh.cn/Article/details/gsjbwtlng.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.hesvh.cn/Article/details/gqbrdqdjb.sHtML

[U64] PHP：目录遍历
来源：http://baike.fehbvm.com/Article/details/geaokhzqx.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.hesvh.cn/Article/details/gvvmlvsin.sHtML

[U65] PHP：会话
来源：http://m.share.zdbjq.cn/Article/details/gilqhtrcb.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gcvyqwumv.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.hesvh.cn/Article/details/gbbtmlncr.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.zdbjq.cn/Article/details/ggubikdsr.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.zdbjq.cn/Article/details/gamzlylno.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.hesvh.cn/Article/details/gwcvjyvav.sHtML

[U68] PHP：PDO 连接
来源：http://wap.fehbvm.com/Article/details/gvtqssfgo.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.fehbvm.com/Article/details/gfhpjauxs.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.fehbvm.com/Article/details/glwklodlk.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.zdbjq.cn/Article/details/ghromoloo.sHtML

[U70] PHP：PDO 事务
来源：http://blog.fehbvm.com/Article/details/grcgqmnqd.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.fehbvm.com/Article/details/gxmpqmjww.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.zdbjq.cn/Article/details/glztreiws.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.hesvh.cn/Article/details/gjwhoxekp.sHtML

[U72] PHP：写错误日志
来源：http://m.share.hesvh.cn/Article/details/ghsuwpzok.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.hesvh.cn/Article/details/ghfdgulvg.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.zdbjq.cn/Article/details/ghfafuprm.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.fehbvm.com/Article/details/gkotoplfo.sHtML

[U74] PHP：读取环境变量
来源：http://blog.zdbjq.cn/Article/details/gtfriwwml.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.fehbvm.com/Article/details/gabgmkmpr.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.zdbjq.cn/Article/details/gaiwtuhvf.sHtML

composer require psr/container
来源：http://baike.hesvh.cn/Article/details/gnskkfpff.sHtML

[U76] PHP：简单路由
来源：http://blog.zdbjq.cn/Article/details/gxrfaxweu.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.fehbvm.com/Article/details/gxutsimqn.sHtML

[U77] PHP：模板渲染
来源：http://wap.hesvh.cn/Article/details/gcufrxzmm.sHtML

composer require twig/twig
来源：http://www.m.share.hesvh.cn/Article/details/glxyuqxlq.sHtML

[U78] PHP：单元测试
来源：http://mobile.fehbvm.com/Article/details/gkqyjjraz.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.fehbvm.com/Article/details/gopmqzusu.sHtML

[U79] PHP：静态分析
来源：http://3g.hesvh.cn/Article/details/gmumiiilx.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.fehbvm.com/Article/details/gnvbglybn.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.zdbjq.cn/Article/details/gmcqjndhf.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.zdbjq.cn/Article/details/gsnqsyspg.sHtML

[U81] JS：初始化项目
来源：http://3g.zdbjq.cn/Article/details/gvaypfrqd.sHtML

npm init -y;  npm i express
来源：http://m.share.fehbvm.com/Article/details/gipbnhclu.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.zdbjq.cn/Article/details/gclwpidpu.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.fehbvm.com/Article/details/gvdynxmtv.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.fehbvm.com/Article/details/gafmdvsib.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.zdbjq.cn/Article/details/gsgdixhnr.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.fehbvm.com/Article/details/gbzqhliem.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.hesvh.cn/Article/details/gsdzhguru.sHtML

[U85] JS：可选链
来源：http://www.m.share.zdbjq.cn/Article/details/gbkzhuofq.sHtML

a?.b?.c
来源：http://baike.hesvh.cn/Article/details/gcsafhbsk.sHtML

[U86] JS：空值合并
来源：http://baike.fehbvm.com/Article/details/ghhefrlbc.sHtML

a ?? b
来源：http://3g.zdbjq.cn/Article/details/genxwhfvw.sHtML

[U87] JS：解构默认值
来源：http://read.share.zdbjq.cn/Article/details/gyezdhfmh.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.hesvh.cn/Article/details/gjzaqpaxr.sHtML

[U88] JS：对象展开合并
来源：http://www.share.fehbvm.com/Article/details/gigaaaqdi.sHtML

{ ...a, ...b }
来源：http://baike.hesvh.cn/Article/details/gbzbrivjj.sHtML

[U89] JS：数组去重
来源：http://3g.zdbjq.cn/Article/details/guszloisk.sHtML

[...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/gkrsfmdyl.sHtML

[U90] JS：数字数组排序
来源：http://m.share.hesvh.cn/Article/details/gpzxfbsom.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/guythzghu.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.zdbjq.cn/Article/details/gjuxvkbhk.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.zdbjq.cn/Article/details/ggrrkkhgw.sHtML

[U92] JS：深拷贝
来源：http://www.blog.fehbvm.com/Article/details/gxjjlvexy.sHtML

structuredClone(obj)
来源：http://www.share.hesvh.cn/Article/details/grqehlfal.sHtML

[U93] JS：模板字符串
来源：http://wap.zdbjq.cn/Article/details/gvcbsvtft.sHtML

`共 ${n} 条`
来源：http://m.share.zdbjq.cn/Article/details/gkijxsmof.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.hesvh.cn/Article/details/gjcctsztq.sHtML

const double = x => x * 2;
来源：http://mobile.hesvh.cn/Article/details/geagttvvb.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.hesvh.cn/Article/details/gymuetmpn.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.fehbvm.com/Article/details/gpdlvahls.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.fehbvm.com/Article/details/gbfiphync.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/gbbqhzdqo.sHtML

[U97] JS：并发请求
来源：http://www.m.share.fehbvm.com/Article/details/guwtppfqw.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/gdhdgwuzp.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.fehbvm.com/Article/details/gzkqxgyxa.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.fehbvm.com/Article/details/gfrgvceiz.sHtML

[U99] JS：事件监听
来源：http://www.m.share.hesvh.cn/Article/details/gjuircaes.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.fehbvm.com/Article/details/gzqgmrooa.sHtML

[U100] JS：DOM 查询
来源：http://3g.fehbvm.com/Article/details/gyoglucpu.sHtML

document.querySelector(".item")
来源：http://3g.zdbjq.cn/Article/details/gfdhfghjx.sHtML

[U101] JS：classList 操作
来源：http://read.share.zdbjq.cn/Article/details/gfriglbuw.sHtML

el.classList.toggle("active")
来源：http://m.share.zdbjq.cn/Article/details/gofklexqj.sHtML

[U102] JS：本地存储
来源：http://www.blog.hesvh.cn/Article/details/gmxhugrvk.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.zdbjq.cn/Article/details/gtyvjgpnr.sHtML

[U103] JS：定时器
来源：http://m.share.zdbjq.cn/Article/details/gjgbvprwg.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.fehbvm.com/Article/details/gdfbbljax.sHtML

[U104] JS：防抖
来源：http://baike.zdbjq.cn/Article/details/gfdqcalsk.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/gigqqwaie.sHtML

[U105] JS：节流
来源：http://www.m.share.zdbjq.cn/Article/details/ghvoekmum.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.zdbjq.cn/Article/details/garctdygo.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gsxstelfd.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.fehbvm.com/Article/details/ghfvgbbcs.sHtML

[U107] JS：数字千分位
来源：http://wap.zdbjq.cn/Article/details/gyfviouty.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.hesvh.cn/Article/details/ghbmdzgve.sHtML

[U108] JS：随机整数
来源：http://blog.zdbjq.cn/Article/details/gzyoqrqhc.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.hesvh.cn/Article/details/gzxgitwxx.sHtML

[U109] JS：数组分组
来源：http://m.share.fehbvm.com/Article/details/gwykzyyki.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.fehbvm.com/Article/details/greukridh.sHtML

[U110] JS：数组分块
来源：http://www.m.share.fehbvm.com/Article/details/gltzbggcu.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.zdbjq.cn/Article/details/gmmgdsbka.sHtML

[U111] JS：对象转 Map
来源：http://m.share.zdbjq.cn/Article/details/gymlqpvbw.sHtML

new Map(Object.entries(obj))
来源：http://baike.hesvh.cn/Article/details/gxclqtiyr.sHtML

[U112] JS：字符串补位
来源：http://mobile.zdbjq.cn/Article/details/gztvfcaae.sHtML

"7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gmasbkvlu.sHtML

[U113] JS：正则替换全部
来源：http://baike.hesvh.cn/Article/details/gjwifkybx.sHtML

s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gnysrswdp.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.zdbjq.cn/Article/details/gbfxsvkcw.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.zdbjq.cn/Article/details/gbkkkcbvt.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.hesvh.cn/Article/details/gwhubktwv.sHtML

crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gjzpqgecy.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.zdbjq.cn/Article/details/gwcudubhg.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.zdbjq.cn/Article/details/gzxflevkt.sHtML

[U117] JS：单元测试
来源：http://www.blog.zdbjq.cn/Article/details/gsirgmubx.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.zdbjq.cn/Article/details/gxwfxaqkx.sHtML

[U118] JS：开发服务器
来源：http://m.share.fehbvm.com/Article/details/gyvfmzchl.sHtML

npm i -D vite;  npx vite
来源：http://mobile.hesvh.cn/Article/details/gszjaptjh.sHtML

[U119] JS：生产构建
来源：http://wap.hesvh.cn/Article/details/gomirvgsu.sHtML

npx vite build
来源：http://mobile.zdbjq.cn/Article/details/gyxzdxjpx.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.hesvh.cn/Article/details/gkoespfap.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.fehbvm.com/Article/details/gonsmvpja.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gnwcnevrv.sHtML

统计汇总
来源：http://mobile.hesvh.cn/Article/details/gjdyoxdmn.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gvtnitbpa.sHtML

按语言统计（条）：
来源：http://www.m.share.fehbvm.com/Article/details/gocprgzpl.sHtML

Python ......... 252
来源：http://blog.zdbjq.cn/Article/details/gzlvdmjfo.sHtML

PHP ............ 252
来源：http://www.blog.fehbvm.com/Article/details/gpzcxfqgs.sHtML

JavaScript ..... 252
来源：http://wap.hesvh.cn/Article/details/gyqjfjehy.sHtML

TypeScript ..... 212
来源：http://www.blog.fehbvm.com/Article/details/gkcytzzym.sHtML

Java ........... 212
来源：http://read.share.zdbjq.cn/Article/details/gejrcusna.sHtML

Go ............. 212
来源：http://3g.fehbvm.com/Article/details/gmvzjzjfm.sHtML

Ruby ........... 212
来源：http://www.m.share.hesvh.cn/Article/details/gufmbtnxo.sHtML

C# ............. 212
来源：http://read.share.hesvh.cn/Article/details/gbdvrqfsm.sHtML

C .............. 30
来源：http://read.share.zdbjq.cn/Article/details/gugmrlpwq.sHtML

C++ ............ 30
来源：http://baike.hesvh.cn/Article/details/gqcpaczsr.sHtML

SQL ............ 90
来源：http://read.share.hesvh.cn/Article/details/gsvzgyiut.sHtML

Bash ........... 80
来源：http://3g.hesvh.cn/Article/details/gzowzpgpt.sHtML

Kotlin ......... 15
来源：http://3g.hesvh.cn/Article/details/gytdyomod.sHtML

Swift .......... 15
来源：http://3g.fehbvm.com/Article/details/gazpqnrga.sHtML

Lua ............ 10
来源：http://www.blog.fehbvm.com/Article/details/gxjhvtrxr.sHtML

Perl ........... 10
来源：http://mobile.hesvh.cn/Article/details/grpfsojys.sHtML

Scala .......... 10
来源：http://baike.hesvh.cn/Article/details/gfluhcfaw.sHtML

------------------------------------
来源：http://blog.hesvh.cn/Article/details/gsivjbblx.sHtML

合计 ........... 2106 条
来源：http://mobile.hesvh.cn/Article/details/ghuxeudrq.sHtML

按章节统计：
来源：http://www.share.zdbjq.cn/Article/details/ghuvlsfjf.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.fehbvm.com/Article/details/gacuatjvh.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.fehbvm.com/Article/details/gayettqbz.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.hesvh.cn/Article/details/gtjfwtorb.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.fehbvm.com/Article/details/gfunsmfdu.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.fehbvm.com/Article/details/gxhsxhwkk.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.fehbvm.com/Article/details/gkmavmuec.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.hesvh.cn/Article/details/gqqumjqkg.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.fehbvm.com/Article/details/gdwoazkfr.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/goeeyxzii.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.fehbvm.com/Article/details/gcdpfmith.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gophlbepn.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gdzjretdr.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gquvmpntd.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.zdbjq.cn/Article/details/gakwosdrt.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.fehbvm.com/Article/details/gwbemtdxv.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gkibtgjvk.sHtML

Q SQL 专题                              90
来源：http://mobile.zdbjq.cn/Article/details/gnezllpjt.sHtML

R Bash 专题                             80
来源：http://3g.hesvh.cn/Article/details/gqwuioegp.sHtML

S C / C++ 专题                          60
来源：http://wap.hesvh.cn/Article/details/gohrdzuyn.sHtML

T 其他语言补充                          60
来源：http://mobile.zdbjq.cn/Article/details/glyalszzz.sHtML

U 高频实用片段                         120
来源：http://baike.zdbjq.cn/Article/details/gpwefqdit.sHtML

------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gcloqzsty.sHtML

合计                                  2106 条
来源：http://wap.zdbjq.cn/Article/details/gmuochcti.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gmwajzdnh.sHtML

使用提醒
来源：http://3g.fehbvm.com/Article/details/gipfichqx.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/grjsrkaex.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.fehbvm.com/Article/details/gzqzxurvl.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.fehbvm.com/Article/details/gvtpxlagg.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.hesvh.cn/Article/details/gzclvyioo.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.fehbvm.com/Article/details/grjhxcgtm.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.zdbjq.cn/Article/details/gkxbqlbpn.sHtML

—— 文件结束 ——
来源：http://mobile.hesvh.cn/Article/details/gulzgccsh.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gcczhfaqx.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.zdbjq.cn/Article/details/gtyqeswyi.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.zdbjq.cn/Article/details/goubvjlfv.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gpjdpdbbs.sHtML


<!-- 参考信息 -->