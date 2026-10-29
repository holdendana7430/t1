代发 wailian999

[U01] Py：创建虚拟环境
来源：http://wap.hesvh.cn/Article/details/gopfxuuwp.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.hesvh.cn/Article/details/gmzazledw.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.hesvh.cn/Article/details/gzahxbogq.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.fehbvm.com/Article/details/gwnejmiww.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.hesvh.cn/Article/details/gpdngedje.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.zdbjq.cn/Article/details/gxbnlybav.sHtML

[U04] Py：变量调试打印
来源：http://3g.zdbjq.cn/Article/details/gwnpbbsnx.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fehbvm.com/Article/details/gzvmzqccu.sHtML

[U05] Py：列表去重且保序
来源：http://baike.hesvh.cn/Article/details/gdhrfprox.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.hesvh.cn/Article/details/gnbkeymyf.sHtML

[U06] Py：合并两个字典
来源：http://baike.zdbjq.cn/Article/details/guwztucwy.sHtML

{**a, **b}
来源：http://read.share.fehbvm.com/Article/details/gcsmmhpxk.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.zdbjq.cn/Article/details/gzuzfqydh.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.hesvh.cn/Article/details/gwrkhsefw.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.zdbjq.cn/Article/details/guyonxaya.sHtML

[y for x in nested for y in x]
来源：http://3g.zdbjq.cn/Article/details/gdhxflczu.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.hesvh.cn/Article/details/gbpuysttr.sHtML

max(d, key=d.get)
来源：http://3g.zdbjq.cn/Article/details/gcjtcsrsk.sHtML

[U10] Py：按值排序字典
来源：http://www.share.fehbvm.com/Article/details/gzfzouesv.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.hesvh.cn/Article/details/gvjuouuap.sHtML

[U11] Py：生成器表达式
来源：http://blog.fehbvm.com/Article/details/gqkuqaipa.sHtML

(x * 2 for x in arr)
来源：http://www.blog.zdbjq.cn/Article/details/ggtgkrhqu.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.fehbvm.com/Article/details/grzwcanqx.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gwkcozwzk.sHtML

[U13] Py：固定长度队列
来源：http://blog.zdbjq.cn/Article/details/gfkpwhqhy.sHtML

deque(maxlen=10)
来源：http://m.share.hesvh.cn/Article/details/gqlfdheyh.sHtML

[U14] Py：分组收集到列表
来源：http://wap.fehbvm.com/Article/details/gdpmtneul.sHtML

defaultdict(list)
来源：http://m.share.zdbjq.cn/Article/details/gbwfqymjh.sHtML

[U15] Py：高精度计时
来源：http://read.share.fehbvm.com/Article/details/gckqbotrj.sHtML

t = time.perf_counter()
来源：http://wap.fehbvm.com/Article/details/gjycjtfjk.sHtML

[U16] Py：命令行参数解析
来源：http://baike.hesvh.cn/Article/details/gonkdyplw.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.fehbvm.com/Article/details/grxlwgahw.sHtML

[U17] Py：初始化日志
来源：http://blog.fehbvm.com/Article/details/gqwwiunpe.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.hesvh.cn/Article/details/gpnvjwfsj.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.zdbjq.cn/Article/details/gtluyinnf.sHtML

pat = re.compile(r"\d+")
来源：http://wap.hesvh.cn/Article/details/gchppazuu.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.hesvh.cn/Article/details/gbrzljuxb.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.zdbjq.cn/Article/details/gbyzveanv.sHtML

[U20] Py：缓存函数结果
来源：http://wap.hesvh.cn/Article/details/gcrjildca.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.fehbvm.com/Article/details/gweekzffp.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.zdbjq.cn/Article/details/gadqtpjmh.sHtML

@contextlib.contextmanager
来源：http://m.share.zdbjq.cn/Article/details/givtrzkui.sHtML

[U22] Py：矩阵转置
来源：http://3g.hesvh.cn/Article/details/ggyzavzoo.sHtML

list(zip(*m))
来源：http://www.m.share.fehbvm.com/Article/details/gsusrkikf.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.hesvh.cn/Article/details/gqwssdqzf.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.zdbjq.cn/Article/details/glzetcqkw.sHtML

[U24] Py：路径操作
来源：http://blog.hesvh.cn/Article/details/gpjpyiaoj.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.fehbvm.com/Article/details/grddqtjtc.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.hesvh.cn/Article/details/gzhntnqhk.sHtML

csv.DictReader(f)
来源：http://mobile.zdbjq.cn/Article/details/gtrkkiiov.sHtML

[U26] Py：并发下载
来源：http://3g.zdbjq.cn/Article/details/glpgjgzqm.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.hesvh.cn/Article/details/gctzncifo.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.fehbvm.com/Article/details/glfruzmqa.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.fehbvm.com/Article/details/gfvoadftq.sHtML

[U28] Py：类型别名
来源：http://www.blog.fehbvm.com/Article/details/gorfudwvz.sHtML

UserId = int
来源：http://m.share.zdbjq.cn/Article/details/gscwtthzd.sHtML

[U29] Py：属性校验
来源：http://read.share.fehbvm.com/Article/details/grjwoaytl.sHtML

@property 与 @x.setter 配合
来源：http://baike.zdbjq.cn/Article/details/gmaenbvwu.sHtML

[U30] Py：数据类
来源：http://3g.fehbvm.com/Article/details/glpnjukwp.sHtML

@dataclass(slots=True)
来源：http://read.share.hesvh.cn/Article/details/gvrkdexjx.sHtML

[U31] Py：单测
来源：http://3g.hesvh.cn/Article/details/gyafzqrlf.sHtML

python -m pytest -q
来源：http://www.share.fehbvm.com/Article/details/gjfyzqvcm.sHtML

[U32] Py：代码格式化
来源：http://www.share.zdbjq.cn/Article/details/gduhgqesk.sHtML

ruff format . && ruff check --fix .
来源：http://blog.zdbjq.cn/Article/details/gckpspbyx.sHtML

[U33] Py：打包发布
来源：http://blog.zdbjq.cn/Article/details/glefycfse.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.zdbjq.cn/Article/details/givitgzhx.sHtML

[U34] Py：判断编码
来源：http://baike.fehbvm.com/Article/details/gwfsbuveo.sHtML

chardet.detect(raw)
来源：http://baike.fehbvm.com/Article/details/goepkwifx.sHtML

[U35] Py：发送邮件
来源：http://mobile.fehbvm.com/Article/details/gnmsriymu.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.zdbjq.cn/Article/details/gqppwwyac.sHtML

[U36] Py：定时任务
来源：http://mobile.fehbvm.com/Article/details/gulmonqyc.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.fehbvm.com/Article/details/gpxjqjwaj.sHtML

[U37] Py：读写 Excel
来源：http://mobile.hesvh.cn/Article/details/giucvdgym.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.hesvh.cn/Article/details/gjblxszqb.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.fehbvm.com/Article/details/gtlbsklsg.sHtML

Path(__file__).resolve().parent
来源：http://m.share.fehbvm.com/Article/details/gyubegnjl.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.fehbvm.com/Article/details/gqujhuxsy.sHtML

sys.stdout.isatty()
来源：http://www.share.hesvh.cn/Article/details/grvdjgtak.sHtML

[U40] Py：打印到标准错误
来源：http://wap.hesvh.cn/Article/details/gtyzrrpzq.sHtML

print("err", file=sys.stderr)
来源：http://m.share.fehbvm.com/Article/details/gpifjhuue.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.zdbjq.cn/Article/details/gucpkhuty.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.hesvh.cn/Article/details/guncdzces.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.zdbjq.cn/Article/details/glmhgezfx.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.fehbvm.com/Article/details/govyeerrx.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.fehbvm.com/Article/details/gahsaqvdg.sHtML

namespace App\Http;
来源：http://baike.zdbjq.cn/Article/details/gskxmgbug.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.hesvh.cn/Article/details/gqktyqpra.sHtML

declare(strict_types=1);
来源：http://baike.zdbjq.cn/Article/details/gtjwdqicq.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.zdbjq.cn/Article/details/glwvouzub.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gfzcifhwx.sHtML

[U46] PHP：可空类型
来源：http://www.blog.zdbjq.cn/Article/details/gymnymrpc.sHtML

?string $name = null
来源：http://www.share.zdbjq.cn/Article/details/gpplfumtm.sHtML

[U47] PHP：联合类型
来源：http://blog.zdbjq.cn/Article/details/gjoopfckp.sHtML

int|string $id
来源：http://m.share.zdbjq.cn/Article/details/gykyuyfxq.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.fehbvm.com/Article/details/gfoewisgl.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.zdbjq.cn/Article/details/gnfaoqyct.sHtML

[U49] PHP：只读属性
来源：http://read.share.zdbjq.cn/Article/details/gkrqgwnhi.sHtML

public readonly string $name
来源：http://blog.hesvh.cn/Article/details/ghifvqqma.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.fehbvm.com/Article/details/gesnjduoy.sHtML

public function __construct(private int $id) {}
来源：http://blog.hesvh.cn/Article/details/gwsdypabd.sHtML

[U51] PHP：数组解构
来源：http://www.blog.hesvh.cn/Article/details/gqrtpucgy.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.hesvh.cn/Article/details/grlvzkjlv.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.hesvh.cn/Article/details/gducfsttq.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.zdbjq.cn/Article/details/gcpzwvfgw.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.fehbvm.com/Article/details/gdmuepbet.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.hesvh.cn/Article/details/guwrqsiya.sHtML

[U54] PHP：空安全调用
来源：http://m.share.hesvh.cn/Article/details/gbtxuuysy.sHtML

$obj?->method()
来源：http://www.m.share.fehbvm.com/Article/details/gwotmawvb.sHtML

[U55] PHP：match 表达式
来源：http://baike.fehbvm.com/Article/details/gnmlpcdbl.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.hesvh.cn/Article/details/geirnfczf.sHtML

[U56] PHP：命名参数
来源：http://3g.fehbvm.com/Article/details/guopgiphp.sHtML

f(a: 1, b: 2)
来源：http://baike.hesvh.cn/Article/details/gqvhxxvnl.sHtML

[U57] PHP：字符串插值
来源：http://mobile.hesvh.cn/Article/details/grvtgawlf.sHtML

"值: {$a}"
来源：http://blog.fehbvm.com/Article/details/guvxkdakr.sHtML

[U58] PHP：数组三件套
来源：http://read.share.zdbjq.cn/Article/details/geikhmnul.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gvxlskaot.sHtML

[U59] PHP：自定义排序
来源：http://mobile.zdbjq.cn/Article/details/gphfqodkp.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fehbvm.com/Article/details/gqfyxdkuc.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.zdbjq.cn/Article/details/gerskcrxx.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.hesvh.cn/Article/details/gzqoydfar.sHtML

[U61] PHP：正则
来源：http://m.share.hesvh.cn/Article/details/gqtilvxkz.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.hesvh.cn/Article/details/gxfadnfgi.sHtML

[U62] PHP：日期对象
来源：http://baike.hesvh.cn/Article/details/gpdxzvvwa.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.zdbjq.cn/Article/details/gkkesqzsv.sHtML

[U63] PHP：文件读写
来源：http://3g.hesvh.cn/Article/details/gdjnuvmfi.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.zdbjq.cn/Article/details/gzhyirriw.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.zdbjq.cn/Article/details/geprqaiqp.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.zdbjq.cn/Article/details/gxxmkgjmn.sHtML

[U65] PHP：会话
来源：http://mobile.fehbvm.com/Article/details/gbcarsffr.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gbyguyjng.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.fehbvm.com/Article/details/giodamwip.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.zdbjq.cn/Article/details/gdbsflogf.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.hesvh.cn/Article/details/ghhushtpz.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.fehbvm.com/Article/details/gheltghkm.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.zdbjq.cn/Article/details/gzbvcvfey.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.fehbvm.com/Article/details/giyivjvub.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.fehbvm.com/Article/details/gatdevnli.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.zdbjq.cn/Article/details/ghnbclbza.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.zdbjq.cn/Article/details/gnsadyllg.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.zdbjq.cn/Article/details/gwtfleypi.sHtML

[U71] PHP：抛出异常
来源：http://m.share.zdbjq.cn/Article/details/gaxnuliin.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.zdbjq.cn/Article/details/grnkmgmvn.sHtML

[U72] PHP：写错误日志
来源：http://m.share.fehbvm.com/Article/details/gmdppqfir.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.fehbvm.com/Article/details/gfxkbvrlf.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.fehbvm.com/Article/details/gwthvasqt.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.zdbjq.cn/Article/details/gixjpqtcz.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.hesvh.cn/Article/details/gjnwnjapa.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.hesvh.cn/Article/details/gfxjkbbgs.sHtML

[U75] PHP：依赖注入
来源：http://mobile.fehbvm.com/Article/details/gsutxchth.sHtML

composer require psr/container
来源：http://3g.zdbjq.cn/Article/details/gwvwlyszu.sHtML

[U76] PHP：简单路由
来源：http://blog.hesvh.cn/Article/details/gnkftnjee.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.fehbvm.com/Article/details/gwmsudylh.sHtML

[U77] PHP：模板渲染
来源：http://mobile.hesvh.cn/Article/details/gljhqpimi.sHtML

composer require twig/twig
来源：http://baike.hesvh.cn/Article/details/gnkwzoyko.sHtML

[U78] PHP：单元测试
来源：http://3g.fehbvm.com/Article/details/gnhftkwmt.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.zdbjq.cn/Article/details/gemtpyrmn.sHtML

[U79] PHP：静态分析
来源：http://wap.fehbvm.com/Article/details/gaconmjnp.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.fehbvm.com/Article/details/gvtkmjtlf.sHtML

[U80] PHP：代码规范修复
来源：http://wap.hesvh.cn/Article/details/ggyhqeeql.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.fehbvm.com/Article/details/gmmmncwji.sHtML

[U81] JS：初始化项目
来源：http://3g.hesvh.cn/Article/details/gpnlxinte.sHtML

npm init -y;  npm i express
来源：http://m.share.zdbjq.cn/Article/details/glirhlnpv.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.zdbjq.cn/Article/details/gfwsejxdh.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.hesvh.cn/Article/details/gyrzrgiha.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.fehbvm.com/Article/details/gmxuxwjyc.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.zdbjq.cn/Article/details/guaftyofp.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.hesvh.cn/Article/details/gmxyuhwnc.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.zdbjq.cn/Article/details/gsoidmmjz.sHtML

[U85] JS：可选链
来源：http://blog.fehbvm.com/Article/details/glhhnsktt.sHtML

a?.b?.c
来源：http://m.share.hesvh.cn/Article/details/gljrvhegh.sHtML

[U86] JS：空值合并
来源：http://www.m.share.hesvh.cn/Article/details/gdtdcopxo.sHtML

a ?? b
来源：http://mobile.zdbjq.cn/Article/details/gcvffxdng.sHtML

[U87] JS：解构默认值
来源：http://wap.hesvh.cn/Article/details/gkxlbohjh.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.fehbvm.com/Article/details/grzunoeno.sHtML

[U88] JS：对象展开合并
来源：http://blog.zdbjq.cn/Article/details/gjwwetcmr.sHtML

{ ...a, ...b }
来源：http://baike.fehbvm.com/Article/details/gxroomtib.sHtML

[U89] JS：数组去重
来源：http://read.share.hesvh.cn/Article/details/gyeofmorc.sHtML

[...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/gipsqgzeq.sHtML

[U90] JS：数字数组排序
来源：http://baike.fehbvm.com/Article/details/gbbcgjyzi.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gbcaerttd.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.fehbvm.com/Article/details/gosrermxm.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.fehbvm.com/Article/details/glnbstnya.sHtML

[U92] JS：深拷贝
来源：http://m.share.hesvh.cn/Article/details/gppwvdlko.sHtML

structuredClone(obj)
来源：http://read.share.hesvh.cn/Article/details/garvrbevw.sHtML

[U93] JS：模板字符串
来源：http://mobile.fehbvm.com/Article/details/gqdhweswg.sHtML

`共 ${n} 条`
来源：http://www.share.zdbjq.cn/Article/details/gurhyrqlj.sHtML

[U94] JS：箭头函数
来源：http://www.share.fehbvm.com/Article/details/ghjskmokp.sHtML

const double = x => x * 2;
来源：http://read.share.fehbvm.com/Article/details/ghyiznrys.sHtML

[U95] JS：Promise 包装
来源：http://mobile.zdbjq.cn/Article/details/gpwzneqyx.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.hesvh.cn/Article/details/gaxpjntqo.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.zdbjq.cn/Article/details/gvbkumlnj.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/ggtzccafw.sHtML

[U97] JS：并发请求
来源：http://read.share.hesvh.cn/Article/details/glarnaztn.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gcjahpiqm.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.fehbvm.com/Article/details/gbnxdckpq.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.hesvh.cn/Article/details/grjjqiorf.sHtML

[U99] JS：事件监听
来源：http://read.share.fehbvm.com/Article/details/gqbevfcxk.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.zdbjq.cn/Article/details/gcvwvlaws.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.fehbvm.com/Article/details/gcpxgtcvo.sHtML

document.querySelector(".item")
来源：http://www.blog.hesvh.cn/Article/details/gwvgjeqom.sHtML

[U101] JS：classList 操作
来源：http://blog.fehbvm.com/Article/details/ggzzynery.sHtML

el.classList.toggle("active")
来源：http://wap.fehbvm.com/Article/details/gyaooyykq.sHtML

[U102] JS：本地存储
来源：http://wap.hesvh.cn/Article/details/gjgrqcwpy.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.zdbjq.cn/Article/details/gqtmquykd.sHtML

[U103] JS：定时器
来源：http://read.share.fehbvm.com/Article/details/grjiwcrhi.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.hesvh.cn/Article/details/grcqkjnsq.sHtML

[U104] JS：防抖
来源：http://mobile.fehbvm.com/Article/details/guzpdbtft.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gzziwtxlu.sHtML

[U105] JS：节流
来源：http://wap.zdbjq.cn/Article/details/gsdsgfdgf.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.hesvh.cn/Article/details/getgtkktv.sHtML

[U106] JS：日期格式化
来源：http://blog.fehbvm.com/Article/details/gfgauzulh.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.zdbjq.cn/Article/details/gykflrhej.sHtML

[U107] JS：数字千分位
来源：http://m.share.zdbjq.cn/Article/details/gtdvennhq.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.hesvh.cn/Article/details/gvjmcmklq.sHtML

[U108] JS：随机整数
来源：http://m.share.zdbjq.cn/Article/details/gphrqruwl.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.fehbvm.com/Article/details/gwsedzmbi.sHtML

[U109] JS：数组分组
来源：http://3g.zdbjq.cn/Article/details/ggjmporol.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.hesvh.cn/Article/details/gebgxppms.sHtML

[U110] JS：数组分块
来源：http://mobile.fehbvm.com/Article/details/gqqbqxzdn.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.zdbjq.cn/Article/details/gyjxzyqvc.sHtML

[U111] JS：对象转 Map
来源：http://mobile.fehbvm.com/Article/details/gpogohstb.sHtML

new Map(Object.entries(obj))
来源：http://3g.zdbjq.cn/Article/details/gwvqkfcte.sHtML

[U112] JS：字符串补位
来源：http://3g.fehbvm.com/Article/details/gkwaqfrve.sHtML

"7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gzwpkpqmh.sHtML

[U113] JS：正则替换全部
来源：http://www.share.zdbjq.cn/Article/details/goihurskt.sHtML

s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gfqjfzkal.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.fehbvm.com/Article/details/grodeayys.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.zdbjq.cn/Article/details/galdxhjyh.sHtML

[U115] JS：生成 UUID
来源：http://m.share.hesvh.cn/Article/details/gxaawsjgb.sHtML

crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gqmsbfopd.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.hesvh.cn/Article/details/glgmuwcmh.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.fehbvm.com/Article/details/gwodznfjs.sHtML

[U117] JS：单元测试
来源：http://baike.hesvh.cn/Article/details/gxkezenyd.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.zdbjq.cn/Article/details/gbzudkhkf.sHtML

[U118] JS：开发服务器
来源：http://baike.hesvh.cn/Article/details/giqfhhggp.sHtML

npm i -D vite;  npx vite
来源：http://mobile.hesvh.cn/Article/details/gcpnmqlwj.sHtML

[U119] JS：生产构建
来源：http://3g.hesvh.cn/Article/details/gxqclwzra.sHtML

npx vite build
来源：http://3g.zdbjq.cn/Article/details/gtwfbwfvu.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.hesvh.cn/Article/details/gqqbrmher.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.zdbjq.cn/Article/details/gaanaembw.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gjtvnkltl.sHtML

统计汇总
来源：http://blog.zdbjq.cn/Article/details/goicjrjpw.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gykomsyzs.sHtML

按语言统计（条）：
来源：http://mobile.fehbvm.com/Article/details/gwoqxaqaf.sHtML

Python ......... 252
来源：http://www.blog.zdbjq.cn/Article/details/goruldgor.sHtML

PHP ............ 252
来源：http://blog.hesvh.cn/Article/details/goxlhdwux.sHtML

JavaScript ..... 252
来源：http://read.share.fehbvm.com/Article/details/gzjxjseuh.sHtML

TypeScript ..... 212
来源：http://blog.fehbvm.com/Article/details/gbjqylcbp.sHtML

Java ........... 212
来源：http://www.m.share.zdbjq.cn/Article/details/gypejspha.sHtML

Go ............. 212
来源：http://wap.zdbjq.cn/Article/details/gzgachffo.sHtML

Ruby ........... 212
来源：http://mobile.hesvh.cn/Article/details/gcmugwlqf.sHtML

C# ............. 212
来源：http://mobile.fehbvm.com/Article/details/gqjdnhtqx.sHtML

C .............. 30
来源：http://www.share.hesvh.cn/Article/details/gtxjfyedv.sHtML

C++ ............ 30
来源：http://www.blog.fehbvm.com/Article/details/gptxwmrbf.sHtML

SQL ............ 90
来源：http://m.share.fehbvm.com/Article/details/gwngdidkd.sHtML

Bash ........... 80
来源：http://www.m.share.zdbjq.cn/Article/details/gnerxqfjd.sHtML

Kotlin ......... 15
来源：http://www.blog.hesvh.cn/Article/details/gifcwbfhk.sHtML

Swift .......... 15
来源：http://read.share.fehbvm.com/Article/details/gelqsabeg.sHtML

Lua ............ 10
来源：http://www.blog.fehbvm.com/Article/details/gffxlsxgv.sHtML

Perl ........... 10
来源：http://blog.fehbvm.com/Article/details/gvexkryce.sHtML

Scala .......... 10
来源：http://blog.zdbjq.cn/Article/details/gdrnpvkyn.sHtML

------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gkmopjaov.sHtML

合计 ........... 2106 条
来源：http://baike.fehbvm.com/Article/details/gdjkuurqi.sHtML

按章节统计：
来源：http://baike.fehbvm.com/Article/details/grtbhmzfz.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.zdbjq.cn/Article/details/gawxzkquy.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.zdbjq.cn/Article/details/gpgltypyo.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/gblpcvjwm.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.hesvh.cn/Article/details/gandjawzf.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.zdbjq.cn/Article/details/gpqkbxwvo.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.fehbvm.com/Article/details/gyasdrfns.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.hesvh.cn/Article/details/gaiskvupp.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.hesvh.cn/Article/details/gwmhjnbkz.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gdynrmdrs.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.zdbjq.cn/Article/details/ggzjdvddz.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/garhyqlqy.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gocsodhyq.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/glfmpvhju.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.fehbvm.com/Article/details/geakmpphx.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.zdbjq.cn/Article/details/gwfvzxmzu.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gcmtwnjow.sHtML

Q SQL 专题                              90
来源：http://mobile.fehbvm.com/Article/details/gnofndvkn.sHtML

R Bash 专题                             80
来源：http://www.share.hesvh.cn/Article/details/gaglawipv.sHtML

S C / C++ 专题                          60
来源：http://3g.zdbjq.cn/Article/details/gcuxcwfwm.sHtML

T 其他语言补充                          60
来源：http://wap.zdbjq.cn/Article/details/gucsjfige.sHtML

U 高频实用片段                         120
来源：http://www.m.share.zdbjq.cn/Article/details/gafvmwhta.sHtML

------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gvhnsgqer.sHtML

合计                                  2106 条
来源：http://mobile.fehbvm.com/Article/details/gbtgimqey.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gjenkmqmb.sHtML

使用提醒
来源：http://wap.fehbvm.com/Article/details/gyvgyewal.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/gythnkqzh.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.hesvh.cn/Article/details/gndiojdwf.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.hesvh.cn/Article/details/gdpcmxzvi.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.fehbvm.com/Article/details/ghbwqbbho.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.fehbvm.com/Article/details/glpoedhcf.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.fehbvm.com/Article/details/gcolbqjtz.sHtML

—— 文件结束 ——
来源：http://www.blog.fehbvm.com/Article/details/giitnjpyh.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gryhtxpwx.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.zdbjq.cn/Article/details/goybnvdtd.sHtML

Common Programming Examples Cheat Book
来源：http://wap.zdbjq.cn/Article/details/gtpruoxkm.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ggurraljm.sHtML


<!-- 参考信息 -->