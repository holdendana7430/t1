代发 wailian999

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.fehbvm.com/Article/details/gqazzxqgr.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gwhnzuxco.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.zdbjq.cn/Article/details/gxtudtmfu.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gtruypkcy.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.hesvh.cn/Article/details/gtrvkpkci.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.zdbjq.cn/Article/details/gfantnrew.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.zdbjq.cn/Article/details/gmgxdaiab.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.fehbvm.com/Article/details/gvtgkczor.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.hesvh.cn/Article/details/gzrzzikub.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.hesvh.cn/Article/details/gnlzdonqy.sHtML

[U04] Py：变量调试打印
来源：http://baike.fehbvm.com/Article/details/gjzmutofd.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.zdbjq.cn/Article/details/gxidviafq.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.hesvh.cn/Article/details/ghlfdjyvn.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/giuznymed.sHtML

[U06] Py：合并两个字典
来源：http://wap.fehbvm.com/Article/details/gnemigzzb.sHtML

{**a, **b}
来源：http://blog.fehbvm.com/Article/details/gwzxpwesu.sHtML

[U07] Py：反转字典键值
来源：http://wap.hesvh.cn/Article/details/gwzjuivry.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.zdbjq.cn/Article/details/gjphzzjrz.sHtML

[U08] Py：展平二维列表
来源：http://wap.zdbjq.cn/Article/details/grczrtbip.sHtML

[y for x in nested for y in x]
来源：http://read.share.fehbvm.com/Article/details/gorwpcnwr.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.hesvh.cn/Article/details/gafdszkbp.sHtML

max(d, key=d.get)
来源：http://blog.hesvh.cn/Article/details/genbxbjvz.sHtML

[U10] Py：按值排序字典
来源：http://wap.fehbvm.com/Article/details/gtjwybxoj.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.zdbjq.cn/Article/details/geneozsbe.sHtML

[U11] Py：生成器表达式
来源：http://www.share.hesvh.cn/Article/details/gcvrndcfb.sHtML

(x * 2 for x in arr)
来源：http://blog.fehbvm.com/Article/details/garrimnao.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.zdbjq.cn/Article/details/gibzyhaov.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.hesvh.cn/Article/details/geoiuvpwy.sHtML

[U13] Py：固定长度队列
来源：http://wap.zdbjq.cn/Article/details/grnuwwlri.sHtML

deque(maxlen=10)
来源：http://read.share.hesvh.cn/Article/details/gbxeqyxqp.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.fehbvm.com/Article/details/gcjeokqxt.sHtML

defaultdict(list)
来源：http://www.share.fehbvm.com/Article/details/gqinilkzc.sHtML

[U15] Py：高精度计时
来源：http://www.blog.fehbvm.com/Article/details/gwpgjzcrf.sHtML

t = time.perf_counter()
来源：http://m.share.hesvh.cn/Article/details/gcxuvdhau.sHtML

[U16] Py：命令行参数解析
来源：http://blog.hesvh.cn/Article/details/gpczmrlxl.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.hesvh.cn/Article/details/gkvjubvwh.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.fehbvm.com/Article/details/gletmpecm.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.hesvh.cn/Article/details/gjgkftdqa.sHtML

[U18] Py：预编译正则
来源：http://baike.fehbvm.com/Article/details/gvrctkihj.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.hesvh.cn/Article/details/grrxyzonq.sHtML

[U19] Py：正则替换带回调
来源：http://3g.hesvh.cn/Article/details/gqjidgjlt.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.hesvh.cn/Article/details/getcdetyo.sHtML

[U20] Py：缓存函数结果
来源：http://baike.hesvh.cn/Article/details/gzahxpyss.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.fehbvm.com/Article/details/geuoyuygi.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.zdbjq.cn/Article/details/gobcioofg.sHtML

@contextlib.contextmanager
来源：http://m.share.fehbvm.com/Article/details/gfryormhk.sHtML

[U22] Py：矩阵转置
来源：http://blog.fehbvm.com/Article/details/gyphbicre.sHtML

list(zip(*m))
来源：http://baike.zdbjq.cn/Article/details/gjpawwfrf.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.fehbvm.com/Article/details/gtbybsysi.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.hesvh.cn/Article/details/gzwdcrtip.sHtML

[U24] Py：路径操作
来源：http://baike.fehbvm.com/Article/details/gdhknahzx.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.hesvh.cn/Article/details/gkmbdeswx.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.hesvh.cn/Article/details/gjqwhenmc.sHtML

csv.DictReader(f)
来源：http://blog.fehbvm.com/Article/details/gqierntge.sHtML

[U26] Py：并发下载
来源：http://mobile.zdbjq.cn/Article/details/gjkrkxegd.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.fehbvm.com/Article/details/ggajenlqd.sHtML

[U27] Py：异步 HTTP
来源：http://wap.zdbjq.cn/Article/details/gljtmuagf.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.zdbjq.cn/Article/details/gwoinuqlv.sHtML

[U28] Py：类型别名
来源：http://www.share.fehbvm.com/Article/details/ghbgyikqa.sHtML

UserId = int
来源：http://mobile.hesvh.cn/Article/details/gccuqgerm.sHtML

[U29] Py：属性校验
来源：http://3g.hesvh.cn/Article/details/gxfpaicly.sHtML

@property 与 @x.setter 配合
来源：http://www.share.fehbvm.com/Article/details/gymqfjuvh.sHtML

[U30] Py：数据类
来源：http://read.share.hesvh.cn/Article/details/gbtlfjfkr.sHtML

@dataclass(slots=True)
来源：http://mobile.fehbvm.com/Article/details/goygmtffj.sHtML

[U31] Py：单测
来源：http://3g.hesvh.cn/Article/details/gzydadpda.sHtML

python -m pytest -q
来源：http://read.share.zdbjq.cn/Article/details/gmklimtsk.sHtML

[U32] Py：代码格式化
来源：http://wap.hesvh.cn/Article/details/gmjmrouew.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.hesvh.cn/Article/details/geuijgyet.sHtML

[U33] Py：打包发布
来源：http://www.m.share.fehbvm.com/Article/details/ggsnwfyrc.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.zdbjq.cn/Article/details/gmodhhgqx.sHtML

[U34] Py：判断编码
来源：http://baike.hesvh.cn/Article/details/gpprodvov.sHtML

chardet.detect(raw)
来源：http://www.blog.zdbjq.cn/Article/details/gmuzrcxlv.sHtML

[U35] Py：发送邮件
来源：http://3g.hesvh.cn/Article/details/gxzxjttct.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.hesvh.cn/Article/details/gxwytciml.sHtML

[U36] Py：定时任务
来源：http://3g.fehbvm.com/Article/details/gcaanoxsu.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.hesvh.cn/Article/details/gdmqlqqjj.sHtML

[U37] Py：读写 Excel
来源：http://wap.zdbjq.cn/Article/details/gakohvrvi.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.hesvh.cn/Article/details/gdpmnbdov.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.hesvh.cn/Article/details/gsrhimbln.sHtML

Path(__file__).resolve().parent
来源：http://baike.hesvh.cn/Article/details/gkhokrytw.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.hesvh.cn/Article/details/goclawuhy.sHtML

sys.stdout.isatty()
来源：http://mobile.fehbvm.com/Article/details/gkxrrpuqn.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.zdbjq.cn/Article/details/gshhgxolz.sHtML

print("err", file=sys.stderr)
来源：http://blog.hesvh.cn/Article/details/gisvpioxr.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.zdbjq.cn/Article/details/gqiukdsrj.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.zdbjq.cn/Article/details/gtzdwxxmn.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.fehbvm.com/Article/details/gspbfnlzt.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.fehbvm.com/Article/details/gnhsgkebu.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.fehbvm.com/Article/details/gelpfddjx.sHtML

namespace App\Http;
来源：http://www.blog.zdbjq.cn/Article/details/gprzflwxz.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.fehbvm.com/Article/details/gwgfwjodb.sHtML

declare(strict_types=1);
来源：http://baike.zdbjq.cn/Article/details/gexolfvfq.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.hesvh.cn/Article/details/gkqwiiavq.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxzicftfa.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.hesvh.cn/Article/details/gdqpmewsw.sHtML

?string $name = null
来源：http://www.share.hesvh.cn/Article/details/gyhtvtqna.sHtML

[U47] PHP：联合类型
来源：http://m.share.hesvh.cn/Article/details/ggnnzeusp.sHtML

int|string $id
来源：http://m.share.zdbjq.cn/Article/details/gvsaxpykl.sHtML

[U48] PHP：纯枚举
来源：http://m.share.zdbjq.cn/Article/details/gjqumnoar.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzrqwogye.sHtML

[U49] PHP：只读属性
来源：http://blog.fehbvm.com/Article/details/gjznwwnpu.sHtML

public readonly string $name
来源：http://www.m.share.fehbvm.com/Article/details/ghrpdglfc.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.zdbjq.cn/Article/details/gvbqbdngb.sHtML

public function __construct(private int $id) {}
来源：http://read.share.fehbvm.com/Article/details/gpfdobolt.sHtML

[U51] PHP：数组解构
来源：http://mobile.fehbvm.com/Article/details/grmcfgdwm.sHtML

[$a, $b] = $arr;
来源：http://mobile.zdbjq.cn/Article/details/gkthowcol.sHtML

[U52] PHP：箭头函数
来源：http://read.share.fehbvm.com/Article/details/guyoqhkdp.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.zdbjq.cn/Article/details/gbnqqundz.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.zdbjq.cn/Article/details/gzvxdvcmp.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.hesvh.cn/Article/details/gpyhlszlt.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.zdbjq.cn/Article/details/gcirksqxb.sHtML

$obj?->method()
来源：http://wap.zdbjq.cn/Article/details/gcruyrbcb.sHtML

[U55] PHP：match 表达式
来源：http://m.share.hesvh.cn/Article/details/ggdxashta.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.zdbjq.cn/Article/details/gogtksueh.sHtML

[U56] PHP：命名参数
来源：http://mobile.hesvh.cn/Article/details/geqarkfpr.sHtML

f(a: 1, b: 2)
来源：http://3g.zdbjq.cn/Article/details/gkewtmdid.sHtML

[U57] PHP：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gzxudetve.sHtML

"值: {$a}"
来源：http://baike.fehbvm.com/Article/details/gqnqcjrha.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.hesvh.cn/Article/details/gubqunxcg.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.fehbvm.com/Article/details/gzkjwadll.sHtML

[U59] PHP：自定义排序
来源：http://blog.zdbjq.cn/Article/details/ggmemeezj.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.hesvh.cn/Article/details/gpcpnatnr.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.hesvh.cn/Article/details/gznrbqlpv.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.zdbjq.cn/Article/details/ghtjhtvya.sHtML

[U61] PHP：正则
来源：http://read.share.zdbjq.cn/Article/details/gycgtqslp.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.hesvh.cn/Article/details/gegfvlazd.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.fehbvm.com/Article/details/gjnlowrnd.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.hesvh.cn/Article/details/gsbrvvksx.sHtML

[U63] PHP：文件读写
来源：http://m.share.fehbvm.com/Article/details/gcwhjdqfn.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.fehbvm.com/Article/details/gpmudtzix.sHtML

[U64] PHP：目录遍历
来源：http://baike.fehbvm.com/Article/details/gydyfkacj.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.zdbjq.cn/Article/details/gqpwsjyjt.sHtML

[U65] PHP：会话
来源：http://3g.fehbvm.com/Article/details/gjxatqzlg.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.hesvh.cn/Article/details/gqdsjlfqo.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.fehbvm.com/Article/details/gqjsmphem.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.hesvh.cn/Article/details/gwayebdox.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.hesvh.cn/Article/details/ghilcmyiy.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.hesvh.cn/Article/details/gmvpnllzg.sHtML

[U68] PHP：PDO 连接
来源：http://wap.hesvh.cn/Article/details/gzvbjnonx.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.zdbjq.cn/Article/details/gpaojwlva.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.fehbvm.com/Article/details/gbgdziitm.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.hesvh.cn/Article/details/gsqpwxcyj.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.fehbvm.com/Article/details/gqywbbszh.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.hesvh.cn/Article/details/ggjrhcovj.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.zdbjq.cn/Article/details/giovxunrr.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.zdbjq.cn/Article/details/gdafukgyl.sHtML

[U72] PHP：写错误日志
来源：http://blog.fehbvm.com/Article/details/gtjaphybv.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.hesvh.cn/Article/details/gpknqwbpe.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.fehbvm.com/Article/details/gphdlbjct.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.hesvh.cn/Article/details/gobzugfji.sHtML

[U74] PHP：读取环境变量
来源：http://blog.zdbjq.cn/Article/details/gypkxrhbm.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.hesvh.cn/Article/details/grlauhsza.sHtML

[U75] PHP：依赖注入
来源：http://wap.hesvh.cn/Article/details/gqslrauhr.sHtML

composer require psr/container
来源：http://read.share.zdbjq.cn/Article/details/gptlhlhkj.sHtML

[U76] PHP：简单路由
来源：http://wap.zdbjq.cn/Article/details/gthepzmat.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.hesvh.cn/Article/details/gslfqpnxy.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.hesvh.cn/Article/details/gwlmymwzu.sHtML

composer require twig/twig
来源：http://mobile.fehbvm.com/Article/details/ggfrlyrur.sHtML

[U78] PHP：单元测试
来源：http://www.share.fehbvm.com/Article/details/gpvseccbf.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.fehbvm.com/Article/details/gnsmhuvrq.sHtML

[U79] PHP：静态分析
来源：http://m.share.hesvh.cn/Article/details/grdpssmnr.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.fehbvm.com/Article/details/gwknygktk.sHtML

[U80] PHP：代码规范修复
来源：http://wap.fehbvm.com/Article/details/gehgrkewj.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.fehbvm.com/Article/details/gaptfjchu.sHtML

[U81] JS：初始化项目
来源：http://wap.hesvh.cn/Article/details/gpgrplugx.sHtML

npm init -y;  npm i express
来源：http://mobile.fehbvm.com/Article/details/giwnljzqa.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.hesvh.cn/Article/details/gbcgdfmsd.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.zdbjq.cn/Article/details/glvxywdmu.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.fehbvm.com/Article/details/gcatlqvxl.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.fehbvm.com/Article/details/gnvedxffk.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.hesvh.cn/Article/details/ggihfuwaq.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.zdbjq.cn/Article/details/gzbzhcywh.sHtML

[U85] JS：可选链
来源：http://mobile.fehbvm.com/Article/details/gokrolyhf.sHtML

a?.b?.c
来源：http://www.m.share.hesvh.cn/Article/details/ghckpexjs.sHtML

[U86] JS：空值合并
来源：http://m.share.zdbjq.cn/Article/details/gukwxgpjl.sHtML

a ?? b
来源：http://baike.hesvh.cn/Article/details/gqjnjsthl.sHtML

[U87] JS：解构默认值
来源：http://www.blog.hesvh.cn/Article/details/gvirqtzrl.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.hesvh.cn/Article/details/gboaapqxw.sHtML

[U88] JS：对象展开合并
来源：http://mobile.fehbvm.com/Article/details/gisakvufe.sHtML

{ ...a, ...b }
来源：http://mobile.fehbvm.com/Article/details/grxqeqmbx.sHtML

[U89] JS：数组去重
来源：http://www.share.zdbjq.cn/Article/details/gndjdibzr.sHtML

[...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/gzyomjjoh.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.fehbvm.com/Article/details/gusftpwwm.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gxcezlhvt.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.zdbjq.cn/Article/details/giwybehwt.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.hesvh.cn/Article/details/gcclgcqdp.sHtML

[U92] JS：深拷贝
来源：http://m.share.hesvh.cn/Article/details/glivlnilv.sHtML

structuredClone(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gtmrwhsgk.sHtML

[U93] JS：模板字符串
来源：http://baike.hesvh.cn/Article/details/gysyaisdu.sHtML

`共 ${n} 条`
来源：http://m.share.hesvh.cn/Article/details/gcdgbmimq.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.fehbvm.com/Article/details/gbhrlwfxh.sHtML

const double = x => x * 2;
来源：http://blog.fehbvm.com/Article/details/gjqyhdtrq.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.fehbvm.com/Article/details/gebfdbbvb.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.fehbvm.com/Article/details/gyueyazqp.sHtML

[U96] JS：async/await 与异常
来源：http://wap.fehbvm.com/Article/details/geuqpekfg.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/ghmyacnjx.sHtML

[U97] JS：并发请求
来源：http://baike.zdbjq.cn/Article/details/gditzfpnf.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/gtubnmsmq.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.zdbjq.cn/Article/details/gyihxgfmq.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.zdbjq.cn/Article/details/ggulwarrh.sHtML

[U99] JS：事件监听
来源：http://www.share.zdbjq.cn/Article/details/gkwivzakt.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.hesvh.cn/Article/details/ggnokyzwr.sHtML

[U100] JS：DOM 查询
来源：http://mobile.hesvh.cn/Article/details/gscmvwvyu.sHtML

document.querySelector(".item")
来源：http://mobile.hesvh.cn/Article/details/gwunkkldh.sHtML

[U101] JS：classList 操作
来源：http://wap.hesvh.cn/Article/details/gspvsswam.sHtML

el.classList.toggle("active")
来源：http://mobile.fehbvm.com/Article/details/gfhplrpug.sHtML

[U102] JS：本地存储
来源：http://m.share.zdbjq.cn/Article/details/gspcokdog.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.zdbjq.cn/Article/details/gewcakxdl.sHtML

[U103] JS：定时器
来源：http://read.share.hesvh.cn/Article/details/gmsmwpirs.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.hesvh.cn/Article/details/gkcxorwlp.sHtML

[U104] JS：防抖
来源：http://www.share.hesvh.cn/Article/details/gyjxuhfoa.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gvdqutobw.sHtML

[U105] JS：节流
来源：http://www.m.share.zdbjq.cn/Article/details/giznjqicn.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.hesvh.cn/Article/details/gvodhcqsg.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gxrbwfsye.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.fehbvm.com/Article/details/gbgzyxdvc.sHtML

[U107] JS：数字千分位
来源：http://m.share.fehbvm.com/Article/details/gsvegpfpi.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.fehbvm.com/Article/details/gnrqdndsx.sHtML

[U108] JS：随机整数
来源：http://www.share.hesvh.cn/Article/details/glfhhsfgx.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.fehbvm.com/Article/details/gigyeleat.sHtML

[U109] JS：数组分组
来源：http://m.share.fehbvm.com/Article/details/gfcnlzisq.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.fehbvm.com/Article/details/glktadhcj.sHtML

[U110] JS：数组分块
来源：http://blog.hesvh.cn/Article/details/gjibwwqpv.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.zdbjq.cn/Article/details/gkedwkbke.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.fehbvm.com/Article/details/gextfkvvs.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.hesvh.cn/Article/details/gsmlnulxl.sHtML

[U112] JS：字符串补位
来源：http://baike.fehbvm.com/Article/details/guqohzpfn.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gdygiqcun.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.zdbjq.cn/Article/details/giroxmwbi.sHtML

s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gajfcnfff.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.fehbvm.com/Article/details/gvszddgjm.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.hesvh.cn/Article/details/gnkzmhnoo.sHtML

[U115] JS：生成 UUID
来源：http://baike.fehbvm.com/Article/details/gjawpydws.sHtML

crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gwysfulhu.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.hesvh.cn/Article/details/gfdqidhve.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.fehbvm.com/Article/details/gvyqwkumm.sHtML

[U117] JS：单元测试
来源：http://3g.zdbjq.cn/Article/details/gpkawzwjw.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.zdbjq.cn/Article/details/gbdbhgukv.sHtML

[U118] JS：开发服务器
来源：http://wap.hesvh.cn/Article/details/gpnkyeeym.sHtML

npm i -D vite;  npx vite
来源：http://www.share.fehbvm.com/Article/details/gosxawtgq.sHtML

[U119] JS：生产构建
来源：http://read.share.fehbvm.com/Article/details/gmawovyen.sHtML

npx vite build
来源：http://www.m.share.zdbjq.cn/Article/details/gzcfbtzme.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.hesvh.cn/Article/details/gmrupeztp.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.hesvh.cn/Article/details/gpnauwgxs.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gaqthbetv.sHtML

统计汇总
来源：http://www.m.share.zdbjq.cn/Article/details/gmkxdkxtk.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gqilcqkpu.sHtML

按语言统计（条）：
来源：http://www.blog.fehbvm.com/Article/details/glcjfrdqc.sHtML

Python ......... 252
来源：http://wap.hesvh.cn/Article/details/grathmfam.sHtML

PHP ............ 252
来源：http://wap.zdbjq.cn/Article/details/gsmvbwxvz.sHtML

JavaScript ..... 252
来源：http://mobile.hesvh.cn/Article/details/gulzfgyyg.sHtML

TypeScript ..... 212
来源：http://blog.hesvh.cn/Article/details/gxjobwsph.sHtML

Java ........... 212
来源：http://www.share.hesvh.cn/Article/details/gymnwtvuj.sHtML

Go ............. 212
来源：http://www.blog.zdbjq.cn/Article/details/gxikurpna.sHtML

Ruby ........... 212
来源：http://baike.fehbvm.com/Article/details/gjboiqsiy.sHtML

C# ............. 212
来源：http://blog.zdbjq.cn/Article/details/gslukirjr.sHtML

C .............. 30
来源：http://mobile.hesvh.cn/Article/details/gookwkzyh.sHtML

C++ ............ 30
来源：http://mobile.hesvh.cn/Article/details/ggmvnvocc.sHtML

SQL ............ 90
来源：http://3g.hesvh.cn/Article/details/gblntkpde.sHtML

Bash ........... 80
来源：http://wap.fehbvm.com/Article/details/gjxmyfdtn.sHtML

Kotlin ......... 15
来源：http://m.share.hesvh.cn/Article/details/gauiowrvs.sHtML

Swift .......... 15
来源：http://www.share.zdbjq.cn/Article/details/gpsypsold.sHtML

Lua ............ 10
来源：http://www.share.hesvh.cn/Article/details/gxtborhpj.sHtML

Perl ........... 10
来源：http://www.m.share.fehbvm.com/Article/details/gdkybxpxf.sHtML

Scala .......... 10
来源：http://www.blog.zdbjq.cn/Article/details/gtalhkoce.sHtML

------------------------------------
来源：http://baike.fehbvm.com/Article/details/gopkgkqzx.sHtML

合计 ........... 2106 条
来源：http://wap.hesvh.cn/Article/details/gqbkcvgvv.sHtML

按章节统计：
来源：http://www.m.share.hesvh.cn/Article/details/gmcxibiyd.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.fehbvm.com/Article/details/gvejvheis.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.fehbvm.com/Article/details/gtxeekijp.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/gtcjtqieu.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.fehbvm.com/Article/details/gikfdkoyo.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.hesvh.cn/Article/details/gewwpkvnp.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.hesvh.cn/Article/details/gzfxyonqe.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.hesvh.cn/Article/details/gkvrjfmep.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.hesvh.cn/Article/details/gliaaajul.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gknfhgvcx.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.fehbvm.com/Article/details/gxfxjjspa.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gpvmygife.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gxghucllc.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gatfhdfvi.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.fehbvm.com/Article/details/gekgkehee.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.hesvh.cn/Article/details/gktecepuy.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/ggvihdiwk.sHtML

Q SQL 专题                              90
来源：http://blog.fehbvm.com/Article/details/gqedbehmk.sHtML

R Bash 专题                             80
来源：http://www.blog.fehbvm.com/Article/details/gctziyayj.sHtML

S C / C++ 专题                          60
来源：http://baike.zdbjq.cn/Article/details/glrfmfqmb.sHtML

T 其他语言补充                          60
来源：http://baike.zdbjq.cn/Article/details/gbarqziul.sHtML

U 高频实用片段                         120
来源：http://m.share.fehbvm.com/Article/details/gpfrahynw.sHtML

------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gioyxbzyl.sHtML

合计                                  2106 条
来源：http://www.m.share.hesvh.cn/Article/details/gtpkvnljj.sHtML

--------------------------------------------------------------------------------
来源：http://baike.hesvh.cn/Article/details/glssnhyhy.sHtML

使用提醒
来源：http://read.share.fehbvm.com/Article/details/gcgyxsifc.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gzzzteane.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.hesvh.cn/Article/details/grudkgiub.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.zdbjq.cn/Article/details/gdawizzag.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.hesvh.cn/Article/details/gtyggxedh.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.hesvh.cn/Article/details/gqboieobo.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.fehbvm.com/Article/details/glfmeetxh.sHtML

—— 文件结束 ——
来源：http://wap.zdbjq.cn/Article/details/ghsuqivxu.sHtML


<!-- 参考信息 -->