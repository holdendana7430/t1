代发 wailian999

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.fehbvm.com/Article/details/gnkcrvnac.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ghebueaqe.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fehbvm.com/Article/details/gqewdwwik.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gwnnndgkh.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.fehbvm.com/Article/details/gwzdypwnl.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.fehbvm.com/Article/details/gncunluqc.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.fehbvm.com/Article/details/grcrjgexf.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.fehbvm.com/Article/details/gzubcftce.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.hesvh.cn/Article/details/gxyilqhbq.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.zdbjq.cn/Article/details/gxfmgjvkd.sHtML

[U04] Py：变量调试打印
来源：http://wap.fehbvm.com/Article/details/gtqdydgsz.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.zdbjq.cn/Article/details/gkctxfauq.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.fehbvm.com/Article/details/gpvutjaxc.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.zdbjq.cn/Article/details/gjkssxudo.sHtML

[U06] Py：合并两个字典
来源：http://m.share.fehbvm.com/Article/details/gzmfjnzzf.sHtML

{**a, **b}
来源：http://www.blog.zdbjq.cn/Article/details/gxnnydtrg.sHtML

[U07] Py：反转字典键值
来源：http://baike.zdbjq.cn/Article/details/gfzouqrrs.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.hesvh.cn/Article/details/gyszuwblb.sHtML

[U08] Py：展平二维列表
来源：http://mobile.fehbvm.com/Article/details/gvcfscuwt.sHtML

[y for x in nested for y in x]
来源：http://www.share.fehbvm.com/Article/details/gollsexrh.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.zdbjq.cn/Article/details/gnlideszv.sHtML

max(d, key=d.get)
来源：http://m.share.fehbvm.com/Article/details/gvkkdlewf.sHtML

[U10] Py：按值排序字典
来源：http://3g.fehbvm.com/Article/details/gydnkiqdx.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.zdbjq.cn/Article/details/gtvqruxtj.sHtML

[U11] Py：生成器表达式
来源：http://mobile.fehbvm.com/Article/details/gcmsiqzks.sHtML

(x * 2 for x in arr)
来源：http://wap.hesvh.cn/Article/details/gvshgutju.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.fehbvm.com/Article/details/gpqysypxf.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.zdbjq.cn/Article/details/gclfhwosc.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.hesvh.cn/Article/details/gjdspjdvm.sHtML

deque(maxlen=10)
来源：http://www.m.share.fehbvm.com/Article/details/gyvzjxxid.sHtML

[U14] Py：分组收集到列表
来源：http://blog.hesvh.cn/Article/details/gifmjgejk.sHtML

defaultdict(list)
来源：http://www.m.share.hesvh.cn/Article/details/gesbzixuz.sHtML

[U15] Py：高精度计时
来源：http://www.blog.hesvh.cn/Article/details/grhnmundk.sHtML

t = time.perf_counter()
来源：http://3g.fehbvm.com/Article/details/gaecmxmvj.sHtML

[U16] Py：命令行参数解析
来源：http://3g.zdbjq.cn/Article/details/geohbxauf.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.zdbjq.cn/Article/details/gwzlwplhz.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.hesvh.cn/Article/details/gpjdibwvm.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.zdbjq.cn/Article/details/gsolrgcii.sHtML

[U18] Py：预编译正则
来源：http://www.blog.fehbvm.com/Article/details/gnuyiyxgb.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fehbvm.com/Article/details/gmlymbszc.sHtML

[U19] Py：正则替换带回调
来源：http://baike.zdbjq.cn/Article/details/grolwjlka.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.zdbjq.cn/Article/details/ggrgxnrst.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.fehbvm.com/Article/details/gsvlkywiz.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.zdbjq.cn/Article/details/gjhoymrkf.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.zdbjq.cn/Article/details/gohcsjxgy.sHtML

@contextlib.contextmanager
来源：http://wap.fehbvm.com/Article/details/gyrkbngfy.sHtML

[U22] Py：矩阵转置
来源：http://read.share.zdbjq.cn/Article/details/gbrczbgip.sHtML

list(zip(*m))
来源：http://3g.hesvh.cn/Article/details/gmcilrzbl.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.hesvh.cn/Article/details/gklfchvur.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.fehbvm.com/Article/details/gftywiqsv.sHtML

[U24] Py：路径操作
来源：http://3g.hesvh.cn/Article/details/gdxbbyagq.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.zdbjq.cn/Article/details/gosgtuogq.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.hesvh.cn/Article/details/ggwftmxpe.sHtML

csv.DictReader(f)
来源：http://3g.zdbjq.cn/Article/details/goykyepqn.sHtML

[U26] Py：并发下载
来源：http://www.share.hesvh.cn/Article/details/gtbclkoli.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.zdbjq.cn/Article/details/gbuvlbbjp.sHtML

[U27] Py：异步 HTTP
来源：http://wap.hesvh.cn/Article/details/gbmszizub.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.hesvh.cn/Article/details/gmcjzsojl.sHtML

[U28] Py：类型别名
来源：http://wap.fehbvm.com/Article/details/gjxwacolb.sHtML

UserId = int
来源：http://baike.fehbvm.com/Article/details/gxenhhsah.sHtML

[U29] Py：属性校验
来源：http://wap.hesvh.cn/Article/details/gmxuegnsn.sHtML

@property 与 @x.setter 配合
来源：http://mobile.hesvh.cn/Article/details/gairmtrjc.sHtML

[U30] Py：数据类
来源：http://blog.hesvh.cn/Article/details/gojaomjbx.sHtML

@dataclass(slots=True)
来源：http://mobile.zdbjq.cn/Article/details/gqnbwalpd.sHtML

[U31] Py：单测
来源：http://baike.fehbvm.com/Article/details/gzhauebcu.sHtML

python -m pytest -q
来源：http://wap.zdbjq.cn/Article/details/gcvsolkyo.sHtML

[U32] Py：代码格式化
来源：http://m.share.hesvh.cn/Article/details/gqlsnvwbn.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.zdbjq.cn/Article/details/gatyqpttp.sHtML

[U33] Py：打包发布
来源：http://blog.fehbvm.com/Article/details/gyigtxuuq.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.fehbvm.com/Article/details/gbxsvtxqv.sHtML

[U34] Py：判断编码
来源：http://wap.hesvh.cn/Article/details/gkpadodwc.sHtML

chardet.detect(raw)
来源：http://www.blog.hesvh.cn/Article/details/gmxewpcmk.sHtML

[U35] Py：发送邮件
来源：http://www.blog.hesvh.cn/Article/details/grlpnuuxw.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.zdbjq.cn/Article/details/gflzjhsvv.sHtML

[U36] Py：定时任务
来源：http://3g.fehbvm.com/Article/details/gddmbyqnt.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.hesvh.cn/Article/details/gjjpxauwr.sHtML

[U37] Py：读写 Excel
来源：http://wap.hesvh.cn/Article/details/gustjetph.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.zdbjq.cn/Article/details/gfcoyppqb.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.hesvh.cn/Article/details/gxrjbfdub.sHtML

Path(__file__).resolve().parent
来源：http://www.share.zdbjq.cn/Article/details/gqlscjoia.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.hesvh.cn/Article/details/georwdmve.sHtML

sys.stdout.isatty()
来源：http://wap.fehbvm.com/Article/details/gafvpzxbc.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.fehbvm.com/Article/details/gwtbfbdgq.sHtML

print("err", file=sys.stderr)
来源：http://read.share.zdbjq.cn/Article/details/ggwmucmrq.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.hesvh.cn/Article/details/gulgfpjtf.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.fehbvm.com/Article/details/gvlnaotvi.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.fehbvm.com/Article/details/gifrjvfee.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.hesvh.cn/Article/details/giyuxtlga.sHtML

[U43] PHP：声明命名空间
来源：http://blog.fehbvm.com/Article/details/gmxwfuaqx.sHtML

namespace App\Http;
来源：http://baike.zdbjq.cn/Article/details/gddbzybgd.sHtML

[U44] PHP：开启严格类型
来源：http://wap.zdbjq.cn/Article/details/ggcnumlgs.sHtML

declare(strict_types=1);
来源：http://m.share.fehbvm.com/Article/details/gslalvinp.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.zdbjq.cn/Article/details/gvvgczfgo.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gpjzamlmk.sHtML

[U46] PHP：可空类型
来源：http://3g.hesvh.cn/Article/details/gtggjfxmz.sHtML

?string $name = null
来源：http://baike.hesvh.cn/Article/details/gfwzifegz.sHtML

[U47] PHP：联合类型
来源：http://mobile.hesvh.cn/Article/details/gtqzkpsnm.sHtML

int|string $id
来源：http://www.blog.hesvh.cn/Article/details/gacsnygpx.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.hesvh.cn/Article/details/gkqinmdjj.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.fehbvm.com/Article/details/gjheroxsq.sHtML

[U49] PHP：只读属性
来源：http://wap.zdbjq.cn/Article/details/guqjudpxy.sHtML

public readonly string $name
来源：http://3g.fehbvm.com/Article/details/ggsslumec.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.hesvh.cn/Article/details/gprsggcse.sHtML

public function __construct(private int $id) {}
来源：http://www.share.zdbjq.cn/Article/details/gygwtwuqn.sHtML

[U51] PHP：数组解构
来源：http://blog.zdbjq.cn/Article/details/gdjilolam.sHtML

[$a, $b] = $arr;
来源：http://m.share.zdbjq.cn/Article/details/glmskuqtw.sHtML

[U52] PHP：箭头函数
来源：http://baike.zdbjq.cn/Article/details/gqsnrfyxx.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.fehbvm.com/Article/details/gcuivtbzh.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.hesvh.cn/Article/details/gwysjfvbf.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.zdbjq.cn/Article/details/gveewqgvi.sHtML

[U54] PHP：空安全调用
来源：http://read.share.zdbjq.cn/Article/details/gkivkfioz.sHtML

$obj?->method()
来源：http://mobile.fehbvm.com/Article/details/gmtgeptps.sHtML

[U55] PHP：match 表达式
来源：http://mobile.fehbvm.com/Article/details/gncontauj.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.zdbjq.cn/Article/details/gloigfbdb.sHtML

[U56] PHP：命名参数
来源：http://www.blog.zdbjq.cn/Article/details/giugmptpy.sHtML

f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/gtrqerklj.sHtML

[U57] PHP：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gyxjpmapv.sHtML

"值: {$a}"
来源：http://baike.hesvh.cn/Article/details/gohjqjwbf.sHtML

[U58] PHP：数组三件套
来源：http://3g.fehbvm.com/Article/details/gtbxvusij.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.zdbjq.cn/Article/details/gvsbtcgli.sHtML

[U59] PHP：自定义排序
来源：http://3g.zdbjq.cn/Article/details/gcmsrtfiv.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.hesvh.cn/Article/details/gvlbjtuko.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.hesvh.cn/Article/details/gzxyjoogh.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.fehbvm.com/Article/details/gxmadzeez.sHtML

[U61] PHP：正则
来源：http://3g.hesvh.cn/Article/details/gcfosolsr.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.hesvh.cn/Article/details/gbifivcvh.sHtML

[U62] PHP：日期对象
来源：http://baike.fehbvm.com/Article/details/gygbudyxx.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.fehbvm.com/Article/details/guzpupopz.sHtML

[U63] PHP：文件读写
来源：http://www.share.hesvh.cn/Article/details/gtxqzhukk.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.fehbvm.com/Article/details/grgjjglbg.sHtML

[U64] PHP：目录遍历
来源：http://mobile.hesvh.cn/Article/details/gnetkcrdn.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.zdbjq.cn/Article/details/gqandqtzl.sHtML

[U65] PHP：会话
来源：http://baike.fehbvm.com/Article/details/gexmvadsl.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gtalgnnvx.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.fehbvm.com/Article/details/gosqxnwuf.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.hesvh.cn/Article/details/gdpjbgnka.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.zdbjq.cn/Article/details/gxhilcinw.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.zdbjq.cn/Article/details/gioxvtfoa.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.hesvh.cn/Article/details/gyzifhfsa.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.fehbvm.com/Article/details/ghthqjiff.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.fehbvm.com/Article/details/giersogkl.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.fehbvm.com/Article/details/gcgdjbfed.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.hesvh.cn/Article/details/gtgnlfslm.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.zdbjq.cn/Article/details/gerpacbbf.sHtML

[U71] PHP：抛出异常
来源：http://mobile.fehbvm.com/Article/details/gomlaxokp.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.hesvh.cn/Article/details/gdjjeqjjx.sHtML

[U72] PHP：写错误日志
来源：http://www.share.zdbjq.cn/Article/details/gdtfbdjch.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.zdbjq.cn/Article/details/gnpkkampd.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.fehbvm.com/Article/details/gslpfzwxf.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.hesvh.cn/Article/details/ggareawrd.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.hesvh.cn/Article/details/glskmfist.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.fehbvm.com/Article/details/glxnvsqgz.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.hesvh.cn/Article/details/giafbwava.sHtML

composer require psr/container
来源：http://www.share.hesvh.cn/Article/details/gefmysuqf.sHtML

[U76] PHP：简单路由
来源：http://baike.fehbvm.com/Article/details/gdiuxjtlf.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.zdbjq.cn/Article/details/gjgemjeng.sHtML

[U77] PHP：模板渲染
来源：http://m.share.zdbjq.cn/Article/details/gjkfbkfpv.sHtML

composer require twig/twig
来源：http://baike.zdbjq.cn/Article/details/gtpjfkbyg.sHtML

[U78] PHP：单元测试
来源：http://m.share.hesvh.cn/Article/details/ghjsnrprd.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.hesvh.cn/Article/details/gkelckwez.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.zdbjq.cn/Article/details/guvyzogid.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.fehbvm.com/Article/details/gpdfldhjn.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.zdbjq.cn/Article/details/gvjgezxsy.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.zdbjq.cn/Article/details/gvhcegqyz.sHtML

[U81] JS：初始化项目
来源：http://mobile.hesvh.cn/Article/details/gllulfcsi.sHtML

npm init -y;  npm i express
来源：http://mobile.hesvh.cn/Article/details/gbrhfksoh.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.zdbjq.cn/Article/details/gxgviwkwt.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.zdbjq.cn/Article/details/gelicxpil.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.fehbvm.com/Article/details/gmolshvpj.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.hesvh.cn/Article/details/gmczhxtxw.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.hesvh.cn/Article/details/gmtllccjk.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.fehbvm.com/Article/details/gnrjynuho.sHtML

[U85] JS：可选链
来源：http://mobile.zdbjq.cn/Article/details/gbxmvuxch.sHtML

a?.b?.c
来源：http://mobile.hesvh.cn/Article/details/gsguwiggo.sHtML

[U86] JS：空值合并
来源：http://baike.hesvh.cn/Article/details/gkowqojor.sHtML

a ?? b
来源：http://baike.fehbvm.com/Article/details/gydjuhyfk.sHtML

[U87] JS：解构默认值
来源：http://blog.hesvh.cn/Article/details/gywtccmsj.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.fehbvm.com/Article/details/gpbktdplo.sHtML

[U88] JS：对象展开合并
来源：http://blog.zdbjq.cn/Article/details/gbtpbgcin.sHtML

{ ...a, ...b }
来源：http://m.share.zdbjq.cn/Article/details/gqpwpivxw.sHtML

[U89] JS：数组去重
来源：http://3g.zdbjq.cn/Article/details/gfoskkwkp.sHtML

[...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/gexcwpfjv.sHtML

[U90] JS：数字数组排序
来源：http://3g.hesvh.cn/Article/details/gjuaxulbk.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/gjcitssrx.sHtML

[U91] JS：对象键值遍历
来源：http://baike.zdbjq.cn/Article/details/gaabmpinh.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.zdbjq.cn/Article/details/gvudgibak.sHtML

[U92] JS：深拷贝
来源：http://m.share.fehbvm.com/Article/details/gmfzvqvka.sHtML

structuredClone(obj)
来源：http://read.share.hesvh.cn/Article/details/gapetvyeg.sHtML

[U93] JS：模板字符串
来源：http://m.share.zdbjq.cn/Article/details/gutuzophd.sHtML

`共 ${n} 条`
来源：http://3g.hesvh.cn/Article/details/gzwniinbk.sHtML

[U94] JS：箭头函数
来源：http://read.share.hesvh.cn/Article/details/gffmpclxz.sHtML

const double = x => x * 2;
来源：http://baike.fehbvm.com/Article/details/gjjvdohqi.sHtML

[U95] JS：Promise 包装
来源：http://read.share.fehbvm.com/Article/details/gkwkviwxb.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.fehbvm.com/Article/details/grqngoljf.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.zdbjq.cn/Article/details/gvfswqkna.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/gjeceevst.sHtML

[U97] JS：并发请求
来源：http://mobile.fehbvm.com/Article/details/gbyggrzzg.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/goyjugsbq.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.zdbjq.cn/Article/details/gkdalwclk.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.fehbvm.com/Article/details/gfokrpvdz.sHtML

[U99] JS：事件监听
来源：http://www.share.zdbjq.cn/Article/details/gondognag.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.fehbvm.com/Article/details/glkberyod.sHtML

[U100] JS：DOM 查询
来源：http://www.share.fehbvm.com/Article/details/gefhmpewb.sHtML

document.querySelector(".item")
来源：http://mobile.zdbjq.cn/Article/details/gvbpxscma.sHtML

[U101] JS：classList 操作
来源：http://baike.hesvh.cn/Article/details/gwahtvxop.sHtML

el.classList.toggle("active")
来源：http://mobile.fehbvm.com/Article/details/gthkofvjc.sHtML

[U102] JS：本地存储
来源：http://mobile.zdbjq.cn/Article/details/gxflfswfn.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.zdbjq.cn/Article/details/gwilriluv.sHtML

[U103] JS：定时器
来源：http://wap.fehbvm.com/Article/details/gepoxazfd.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.fehbvm.com/Article/details/gbmlwtcqb.sHtML

[U104] JS：防抖
来源：http://wap.hesvh.cn/Article/details/gispmswqj.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/glzlnnfja.sHtML

[U105] JS：节流
来源：http://baike.zdbjq.cn/Article/details/gupkcxodz.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.hesvh.cn/Article/details/gjiybbwzu.sHtML

[U106] JS：日期格式化
来源：http://read.share.hesvh.cn/Article/details/gbxmgtkqx.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.zdbjq.cn/Article/details/gvorsptdf.sHtML

[U107] JS：数字千分位
来源：http://wap.fehbvm.com/Article/details/gxflqjpgh.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.fehbvm.com/Article/details/gpmvugaww.sHtML

[U108] JS：随机整数
来源：http://blog.hesvh.cn/Article/details/grolwxjcq.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.fehbvm.com/Article/details/gbyriyilu.sHtML

[U109] JS：数组分组
来源：http://m.share.zdbjq.cn/Article/details/gjnaqrind.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.hesvh.cn/Article/details/gtjkmxevk.sHtML

[U110] JS：数组分块
来源：http://baike.fehbvm.com/Article/details/gjihexmld.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.fehbvm.com/Article/details/ghrzokzfz.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.fehbvm.com/Article/details/gdjidlnqm.sHtML

new Map(Object.entries(obj))
来源：http://blog.hesvh.cn/Article/details/gmmhuyflt.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.fehbvm.com/Article/details/guqdbxjfj.sHtML

"7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gaqnscpdy.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.zdbjq.cn/Article/details/gcnuejuax.sHtML

s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gqkqdvrie.sHtML

[U114] JS：JSON 深比较
来源：http://wap.zdbjq.cn/Article/details/gysfnexcx.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.hesvh.cn/Article/details/gbvkydluy.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.hesvh.cn/Article/details/gnnqvgohv.sHtML

crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/gokwkbkqr.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.fehbvm.com/Article/details/gyjbxyova.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.fehbvm.com/Article/details/gbcokwaoh.sHtML

[U117] JS：单元测试
来源：http://www.blog.hesvh.cn/Article/details/gnrkfnlhi.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.hesvh.cn/Article/details/ggxzkzkjg.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.zdbjq.cn/Article/details/ghkeovupc.sHtML

npm i -D vite;  npx vite
来源：http://m.share.fehbvm.com/Article/details/gqphxgdza.sHtML

[U119] JS：生产构建
来源：http://www.share.hesvh.cn/Article/details/gkmjdthla.sHtML

npx vite build
来源：http://www.m.share.zdbjq.cn/Article/details/gcjgahjbj.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.zdbjq.cn/Article/details/godqdkcbe.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.fehbvm.com/Article/details/gcgaaxpim.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gilfanbvb.sHtML

统计汇总
来源：http://m.share.hesvh.cn/Article/details/gnnxaerxf.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gyjsmctxn.sHtML

按语言统计（条）：
来源：http://www.m.share.fehbvm.com/Article/details/gmgrupvvf.sHtML

Python ......... 252
来源：http://www.m.share.fehbvm.com/Article/details/gzgqkmvvc.sHtML

PHP ............ 252
来源：http://m.share.zdbjq.cn/Article/details/gjfjpagwq.sHtML

JavaScript ..... 252
来源：http://read.share.fehbvm.com/Article/details/gvwzjnbdn.sHtML

TypeScript ..... 212
来源：http://www.blog.hesvh.cn/Article/details/gkrcmhsnq.sHtML

Java ........... 212
来源：http://wap.fehbvm.com/Article/details/gaajzbszb.sHtML

Go ............. 212
来源：http://www.share.hesvh.cn/Article/details/ghtblktwk.sHtML

Ruby ........... 212
来源：http://3g.hesvh.cn/Article/details/gwkckrsiw.sHtML

C# ............. 212
来源：http://mobile.hesvh.cn/Article/details/gtfurjnnj.sHtML

C .............. 30
来源：http://baike.hesvh.cn/Article/details/gkansesei.sHtML

C++ ............ 30
来源：http://www.share.fehbvm.com/Article/details/ggxgwzmci.sHtML

SQL ............ 90
来源：http://www.m.share.hesvh.cn/Article/details/giivvdrim.sHtML

Bash ........... 80
来源：http://www.share.hesvh.cn/Article/details/gpjzsqplr.sHtML

Kotlin ......... 15
来源：http://baike.zdbjq.cn/Article/details/gfzqovksc.sHtML

Swift .......... 15
来源：http://read.share.fehbvm.com/Article/details/gcqxmfwfq.sHtML

Lua ............ 10
来源：http://blog.fehbvm.com/Article/details/gkiftgnyf.sHtML

Perl ........... 10
来源：http://baike.fehbvm.com/Article/details/gnrwhivux.sHtML

Scala .......... 10
来源：http://read.share.zdbjq.cn/Article/details/gfzlmeabg.sHtML

------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gmkisbjgy.sHtML

合计 ........... 2106 条
来源：http://www.share.hesvh.cn/Article/details/gqeimlswe.sHtML

按章节统计：
来源：http://www.share.zdbjq.cn/Article/details/gdadfxujz.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.hesvh.cn/Article/details/gaikxhyvy.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/giussfqmu.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.zdbjq.cn/Article/details/gqxfscuqo.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.zdbjq.cn/Article/details/gzadhldoh.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.fehbvm.com/Article/details/gvffxxbgc.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.fehbvm.com/Article/details/gbuxjskva.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.hesvh.cn/Article/details/gwycyzxlw.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.zdbjq.cn/Article/details/giwdvegvt.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gzoxlhbwi.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.zdbjq.cn/Article/details/geniolopt.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gdlwxhrvt.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gfyrfostq.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gkgjyfzvn.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.fehbvm.com/Article/details/gpzxkjwtn.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.hesvh.cn/Article/details/gafqxklbb.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gdvgrmzwo.sHtML

Q SQL 专题                              90
来源：http://m.share.zdbjq.cn/Article/details/gckcmtscv.sHtML

R Bash 专题                             80
来源：http://wap.fehbvm.com/Article/details/gtnmyetxv.sHtML

S C / C++ 专题                          60
来源：http://www.blog.zdbjq.cn/Article/details/gpnjpezsi.sHtML

T 其他语言补充                          60
来源：http://m.share.fehbvm.com/Article/details/gwcymbdgi.sHtML

U 高频实用片段                         120
来源：http://m.share.hesvh.cn/Article/details/guszozjnv.sHtML

------------------------------------
来源：http://baike.fehbvm.com/Article/details/gwgiaoite.sHtML

合计                                  2106 条
来源：http://www.m.share.fehbvm.com/Article/details/gabzrbgdv.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gllphnmug.sHtML

使用提醒
来源：http://3g.zdbjq.cn/Article/details/grnspznzt.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/gtramranx.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.hesvh.cn/Article/details/goyhxumoc.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.hesvh.cn/Article/details/gsapvsplw.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.zdbjq.cn/Article/details/gvdxdfiqo.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.hesvh.cn/Article/details/gqbmkguvd.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.zdbjq.cn/Article/details/gbupfxuha.sHtML

—— 文件结束 ——
来源：http://baike.zdbjq.cn/Article/details/gjmkumwdu.sHtML


<!-- 参考信息 -->