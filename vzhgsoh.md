代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.zdbjq.cn/Article/details/gxvzupzir.sHtML

[T59] Scala：循环
来源：http://baike.zdbjq.cn/Article/details/gdhglcuaf.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/gkcberzyi.sHtML

[T60] Scala：折叠
来源：http://blog.hesvh.cn/Article/details/gsshcswzj.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.fehbvm.com/Article/details/gvczlbmop.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gbtckhshl.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.zdbjq.cn/Article/details/gaxzqowyi.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/giliohkzs.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.zdbjq.cn/Article/details/gxsdgkcyt.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.zdbjq.cn/Article/details/ghjyprjjb.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.hesvh.cn/Article/details/gnqzrnyyw.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.fehbvm.com/Article/details/gspkwohtu.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.zdbjq.cn/Article/details/ghesiiuij.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.fehbvm.com/Article/details/gynqzfjoy.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.hesvh.cn/Article/details/gabqqessj.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.fehbvm.com/Article/details/gumugriqg.sHtML

[U05] Py：列表去重且保序
来源：http://baike.zdbjq.cn/Article/details/gqkarwchs.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.fehbvm.com/Article/details/gmhkxywdn.sHtML

[U06] Py：合并两个字典
来源：http://read.share.zdbjq.cn/Article/details/gjbywymtj.sHtML

{**a, **b}
来源：http://wap.zdbjq.cn/Article/details/gycfeurna.sHtML

[U07] Py：反转字典键值
来源：http://baike.zdbjq.cn/Article/details/gtmwdyzau.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.fehbvm.com/Article/details/guubulowj.sHtML

[U08] Py：展平二维列表
来源：http://wap.hesvh.cn/Article/details/gxzqtcpal.sHtML

[y for x in nested for y in x]
来源：http://m.share.fehbvm.com/Article/details/gkcyqeoki.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.zdbjq.cn/Article/details/gveazqspk.sHtML

max(d, key=d.get)
来源：http://www.blog.hesvh.cn/Article/details/ghdyqnqyv.sHtML

[U10] Py：按值排序字典
来源：http://read.share.fehbvm.com/Article/details/gxqrwbkct.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.hesvh.cn/Article/details/gzcnupkpx.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.zdbjq.cn/Article/details/gjuctnplo.sHtML

(x * 2 for x in arr)
来源：http://mobile.hesvh.cn/Article/details/gzwswllxt.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.hesvh.cn/Article/details/guzfawihe.sHtML

Counter(arr).most_common(3)
来源：http://mobile.hesvh.cn/Article/details/gmberaxsk.sHtML

[U13] Py：固定长度队列
来源：http://3g.fehbvm.com/Article/details/grdmcxolg.sHtML

deque(maxlen=10)
来源：http://mobile.zdbjq.cn/Article/details/gsbhcaidq.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.zdbjq.cn/Article/details/gcefxcljc.sHtML

defaultdict(list)
来源：http://www.blog.zdbjq.cn/Article/details/gtffdzpul.sHtML

[U15] Py：高精度计时
来源：http://3g.zdbjq.cn/Article/details/glhjgwsxa.sHtML

t = time.perf_counter()
来源：http://www.blog.fehbvm.com/Article/details/gqtshjato.sHtML

[U16] Py：命令行参数解析
来源：http://wap.hesvh.cn/Article/details/ghgrvkvvb.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.zdbjq.cn/Article/details/getfkalrq.sHtML

[U17] Py：初始化日志
来源：http://www.share.hesvh.cn/Article/details/gomhccxqr.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.zdbjq.cn/Article/details/gscuwetsv.sHtML

[U18] Py：预编译正则
来源：http://m.share.fehbvm.com/Article/details/gflaesxtb.sHtML

pat = re.compile(r"\d+")
来源：http://baike.fehbvm.com/Article/details/gvohutnte.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.hesvh.cn/Article/details/gadmkmqbq.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.hesvh.cn/Article/details/gkxehcnax.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.hesvh.cn/Article/details/gxgcqfden.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.fehbvm.com/Article/details/gsftqmfxz.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.zdbjq.cn/Article/details/gixnoulnr.sHtML

@contextlib.contextmanager
来源：http://read.share.hesvh.cn/Article/details/gxpvqmvxj.sHtML

[U22] Py：矩阵转置
来源：http://blog.hesvh.cn/Article/details/gaqoxilff.sHtML

list(zip(*m))
来源：http://wap.zdbjq.cn/Article/details/goltpeghb.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.fehbvm.com/Article/details/gedyhdgbk.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.fehbvm.com/Article/details/gnpmyekkg.sHtML

[U24] Py：路径操作
来源：http://blog.fehbvm.com/Article/details/gcrfuqlnn.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.hesvh.cn/Article/details/gkcprgoov.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.zdbjq.cn/Article/details/gheouvnrl.sHtML

csv.DictReader(f)
来源：http://www.share.hesvh.cn/Article/details/geeileyrc.sHtML

[U26] Py：并发下载
来源：http://mobile.hesvh.cn/Article/details/ghlffzcsc.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.fehbvm.com/Article/details/gjhmwvtlh.sHtML

[U27] Py：异步 HTTP
来源：http://blog.fehbvm.com/Article/details/grwgjeddh.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.zdbjq.cn/Article/details/gapfhirlz.sHtML

[U28] Py：类型别名
来源：http://wap.hesvh.cn/Article/details/gbptwtvht.sHtML

UserId = int
来源：http://3g.fehbvm.com/Article/details/gwhsjgotn.sHtML

[U29] Py：属性校验
来源：http://m.share.zdbjq.cn/Article/details/gxerqscxd.sHtML

@property 与 @x.setter 配合
来源：http://www.share.fehbvm.com/Article/details/gjdievkkb.sHtML

[U30] Py：数据类
来源：http://m.share.fehbvm.com/Article/details/gjangxjov.sHtML

@dataclass(slots=True)
来源：http://blog.hesvh.cn/Article/details/giunwmowk.sHtML

[U31] Py：单测
来源：http://blog.zdbjq.cn/Article/details/gyqmqibsk.sHtML

python -m pytest -q
来源：http://mobile.zdbjq.cn/Article/details/glhjitkks.sHtML

[U32] Py：代码格式化
来源：http://www.share.fehbvm.com/Article/details/glvckdjjy.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.hesvh.cn/Article/details/grsqsvwbs.sHtML

[U33] Py：打包发布
来源：http://wap.zdbjq.cn/Article/details/geahdsmyx.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.hesvh.cn/Article/details/gygbtdeqz.sHtML

[U34] Py：判断编码
来源：http://read.share.zdbjq.cn/Article/details/gskpjonjk.sHtML

chardet.detect(raw)
来源：http://read.share.fehbvm.com/Article/details/gjmqzbuen.sHtML

[U35] Py：发送邮件
来源：http://www.share.zdbjq.cn/Article/details/gofmekpdp.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.hesvh.cn/Article/details/gogtfysdw.sHtML

[U36] Py：定时任务
来源：http://wap.fehbvm.com/Article/details/gtnjjrlfg.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.zdbjq.cn/Article/details/ghhdhziur.sHtML

[U37] Py：读写 Excel
来源：http://blog.fehbvm.com/Article/details/gywljcexe.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.fehbvm.com/Article/details/gnwoojkki.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.fehbvm.com/Article/details/gfmeiggdf.sHtML

Path(__file__).resolve().parent
来源：http://3g.zdbjq.cn/Article/details/gjxqxzass.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.zdbjq.cn/Article/details/grxntpcsp.sHtML

sys.stdout.isatty()
来源：http://m.share.hesvh.cn/Article/details/gbdfotdby.sHtML

[U40] Py：打印到标准错误
来源：http://baike.hesvh.cn/Article/details/gvfiptzyo.sHtML

print("err", file=sys.stderr)
来源：http://m.share.hesvh.cn/Article/details/gxwqewmij.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.hesvh.cn/Article/details/gtobjfgte.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.zdbjq.cn/Article/details/grdwphopw.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.hesvh.cn/Article/details/ggkobbqza.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.zdbjq.cn/Article/details/gcxwelsnc.sHtML

[U43] PHP：声明命名空间
来源：http://wap.zdbjq.cn/Article/details/ggjyqhbgy.sHtML

namespace App\Http;
来源：http://www.m.share.hesvh.cn/Article/details/gqjkmmfqa.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.hesvh.cn/Article/details/gipbcdvlj.sHtML

declare(strict_types=1);
来源：http://3g.hesvh.cn/Article/details/gmwparlfj.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.hesvh.cn/Article/details/ghorqsqdd.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gxrjxbnbf.sHtML

[U46] PHP：可空类型
来源：http://www.blog.zdbjq.cn/Article/details/gnedkjtff.sHtML

?string $name = null
来源：http://baike.hesvh.cn/Article/details/gkwfsrzme.sHtML

[U47] PHP：联合类型
来源：http://blog.fehbvm.com/Article/details/gbvfgojhf.sHtML

int|string $id
来源：http://baike.hesvh.cn/Article/details/gzgcipbwb.sHtML

[U48] PHP：纯枚举
来源：http://m.share.hesvh.cn/Article/details/gnyoupeku.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.hesvh.cn/Article/details/gfyfxwgqu.sHtML

[U49] PHP：只读属性
来源：http://m.share.zdbjq.cn/Article/details/gdwvfghzv.sHtML

public readonly string $name
来源：http://www.blog.fehbvm.com/Article/details/grebepbri.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.fehbvm.com/Article/details/gmiufoxcq.sHtML

public function __construct(private int $id) {}
来源：http://mobile.hesvh.cn/Article/details/gwwmzrahb.sHtML

[U51] PHP：数组解构
来源：http://read.share.fehbvm.com/Article/details/gupiawhqm.sHtML

[$a, $b] = $arr;
来源：http://www.share.hesvh.cn/Article/details/gxfgvbbrm.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.zdbjq.cn/Article/details/gurkxpyme.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.hesvh.cn/Article/details/gjrogezjp.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.fehbvm.com/Article/details/gglzxzvgy.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.hesvh.cn/Article/details/glcddgtok.sHtML

[U54] PHP：空安全调用
来源：http://3g.hesvh.cn/Article/details/ghxoyywbn.sHtML

$obj?->method()
来源：http://mobile.hesvh.cn/Article/details/gmbtkoeqn.sHtML

[U55] PHP：match 表达式
来源：http://www.share.hesvh.cn/Article/details/ggjielcke.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.zdbjq.cn/Article/details/grdyeyznl.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.zdbjq.cn/Article/details/gtabzuese.sHtML

f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/guhcmseav.sHtML

[U57] PHP：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gdzbxmebz.sHtML

"值: {$a}"
来源：http://m.share.zdbjq.cn/Article/details/gpmuaxxzk.sHtML

[U58] PHP：数组三件套
来源：http://baike.fehbvm.com/Article/details/gqabpdpbu.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.zdbjq.cn/Article/details/geomskhrc.sHtML

[U59] PHP：自定义排序
来源：http://m.share.hesvh.cn/Article/details/gqswzmlei.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.hesvh.cn/Article/details/ggjzfujcn.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.hesvh.cn/Article/details/gbdvgtkys.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.fehbvm.com/Article/details/gxwqwktrh.sHtML

[U61] PHP：正则
来源：http://read.share.zdbjq.cn/Article/details/glvbxejqc.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fehbvm.com/Article/details/gksismucx.sHtML

[U62] PHP：日期对象
来源：http://www.share.fehbvm.com/Article/details/gxukrdayi.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.hesvh.cn/Article/details/gkddlonlj.sHtML

[U63] PHP：文件读写
来源：http://read.share.fehbvm.com/Article/details/grxrbzpkg.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.hesvh.cn/Article/details/guzuhjlfq.sHtML

[U64] PHP：目录遍历
来源：http://baike.hesvh.cn/Article/details/gatdnkprv.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.hesvh.cn/Article/details/gxqkeymjv.sHtML

[U65] PHP：会话
来源：http://mobile.hesvh.cn/Article/details/giodjnciu.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.hesvh.cn/Article/details/gwmedfkek.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.zdbjq.cn/Article/details/gljuwxfoh.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.zdbjq.cn/Article/details/gehozjsdr.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.fehbvm.com/Article/details/geveterno.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.hesvh.cn/Article/details/gtcxwvncz.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.zdbjq.cn/Article/details/grbytxrdm.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.hesvh.cn/Article/details/gpjflizqz.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.hesvh.cn/Article/details/glhrxvwzy.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.hesvh.cn/Article/details/gjiwxcvty.sHtML

[U70] PHP：PDO 事务
来源：http://3g.hesvh.cn/Article/details/gshaetahf.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.hesvh.cn/Article/details/gajbwffpq.sHtML

[U71] PHP：抛出异常
来源：http://m.share.zdbjq.cn/Article/details/gxahxhxvh.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.hesvh.cn/Article/details/gdxmbclts.sHtML

[U72] PHP：写错误日志
来源：http://baike.hesvh.cn/Article/details/glkxwzevq.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.fehbvm.com/Article/details/gauaeaojq.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.fehbvm.com/Article/details/gevrbxlkn.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.fehbvm.com/Article/details/givtnwbii.sHtML

[U74] PHP：读取环境变量
来源：http://3g.zdbjq.cn/Article/details/gmkmqjefe.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.zdbjq.cn/Article/details/geofufixl.sHtML

[U75] PHP：依赖注入
来源：http://blog.hesvh.cn/Article/details/gjyajbgkn.sHtML

composer require psr/container
来源：http://mobile.hesvh.cn/Article/details/ghpwwuaue.sHtML

[U76] PHP：简单路由
来源：http://3g.fehbvm.com/Article/details/gkxmocrip.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.hesvh.cn/Article/details/gfmykepgv.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.fehbvm.com/Article/details/gipmavpmd.sHtML

composer require twig/twig
来源：http://wap.fehbvm.com/Article/details/gtmebphsy.sHtML

[U78] PHP：单元测试
来源：http://3g.fehbvm.com/Article/details/gvmtjbfdg.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.zdbjq.cn/Article/details/gynkftlok.sHtML

[U79] PHP：静态分析
来源：http://www.blog.hesvh.cn/Article/details/giqnkfzez.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.fehbvm.com/Article/details/gvhcwqgza.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.zdbjq.cn/Article/details/gwosdwrwc.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.zdbjq.cn/Article/details/gbixudvea.sHtML

[U81] JS：初始化项目
来源：http://www.share.zdbjq.cn/Article/details/gmvziucvd.sHtML

npm init -y;  npm i express
来源：http://m.share.fehbvm.com/Article/details/gockjysuo.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.fehbvm.com/Article/details/gaibulcqf.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.zdbjq.cn/Article/details/gdljbmifc.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.zdbjq.cn/Article/details/gitliytjz.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.hesvh.cn/Article/details/gqxnjadnj.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.zdbjq.cn/Article/details/gudmwpdcg.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.hesvh.cn/Article/details/gyrffcysx.sHtML

[U85] JS：可选链
来源：http://mobile.zdbjq.cn/Article/details/gqobzpjpg.sHtML

a?.b?.c
来源：http://read.share.zdbjq.cn/Article/details/gzfvtpaeg.sHtML

[U86] JS：空值合并
来源：http://3g.hesvh.cn/Article/details/ggrxvqzio.sHtML

a ?? b
来源：http://blog.hesvh.cn/Article/details/grvwvpoyu.sHtML

[U87] JS：解构默认值
来源：http://mobile.zdbjq.cn/Article/details/goaezhoqj.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.fehbvm.com/Article/details/ggkiesvln.sHtML

[U88] JS：对象展开合并
来源：http://baike.zdbjq.cn/Article/details/gkqwecqxg.sHtML

{ ...a, ...b }
来源：http://baike.fehbvm.com/Article/details/gvbaijsxy.sHtML

[U89] JS：数组去重
来源：http://www.m.share.fehbvm.com/Article/details/gupachcwd.sHtML

[...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/gmeatnwdf.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.zdbjq.cn/Article/details/gnlatlemx.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/ggfvnmkem.sHtML

[U91] JS：对象键值遍历
来源：http://wap.fehbvm.com/Article/details/gnwkljztt.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.hesvh.cn/Article/details/gdxcrzvcc.sHtML

[U92] JS：深拷贝
来源：http://baike.fehbvm.com/Article/details/gjoumscmh.sHtML

structuredClone(obj)
来源：http://blog.fehbvm.com/Article/details/geqnjwxpd.sHtML

[U93] JS：模板字符串
来源：http://mobile.fehbvm.com/Article/details/gluaqsyrg.sHtML

`共 ${n} 条`
来源：http://www.blog.fehbvm.com/Article/details/gykboswop.sHtML

[U94] JS：箭头函数
来源：http://www.share.zdbjq.cn/Article/details/gzipwnydd.sHtML

const double = x => x * 2;
来源：http://www.m.share.hesvh.cn/Article/details/gjgtdrkpu.sHtML

[U95] JS：Promise 包装
来源：http://wap.fehbvm.com/Article/details/glngtjkwi.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.zdbjq.cn/Article/details/gjkolszse.sHtML

[U96] JS：async/await 与异常
来源：http://baike.hesvh.cn/Article/details/gxomakfwo.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/gkcgzfuuf.sHtML

[U97] JS：并发请求
来源：http://www.share.zdbjq.cn/Article/details/guicjitjx.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gvfilipzo.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.hesvh.cn/Article/details/gzzbrebrc.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.hesvh.cn/Article/details/gdkoqfnio.sHtML

[U99] JS：事件监听
来源：http://read.share.hesvh.cn/Article/details/gmvdgstzn.sHtML

el.addEventListener("click", e => {})
来源：http://baike.fehbvm.com/Article/details/gbfivknqj.sHtML

[U100] JS：DOM 查询
来源：http://www.share.hesvh.cn/Article/details/gfbtkoafx.sHtML

document.querySelector(".item")
来源：http://wap.zdbjq.cn/Article/details/gvzftvthe.sHtML

[U101] JS：classList 操作
来源：http://www.blog.hesvh.cn/Article/details/gzjruczqp.sHtML

el.classList.toggle("active")
来源：http://blog.zdbjq.cn/Article/details/ghfeyexqv.sHtML

[U102] JS：本地存储
来源：http://blog.fehbvm.com/Article/details/ghjlgqhgb.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.fehbvm.com/Article/details/gtxizkasp.sHtML

[U103] JS：定时器
来源：http://www.m.share.fehbvm.com/Article/details/gedudjjju.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.zdbjq.cn/Article/details/ggghnoshk.sHtML

[U104] JS：防抖
来源：http://www.share.zdbjq.cn/Article/details/gyzomunat.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gkzuwjbrh.sHtML

[U105] JS：节流
来源：http://www.m.share.hesvh.cn/Article/details/glwluvluw.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.zdbjq.cn/Article/details/grpupucek.sHtML

[U106] JS：日期格式化
来源：http://blog.hesvh.cn/Article/details/gqarlrvlx.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.hesvh.cn/Article/details/gdjovzydx.sHtML

[U107] JS：数字千分位
来源：http://read.share.fehbvm.com/Article/details/gptmgdfte.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.fehbvm.com/Article/details/gclrtlikf.sHtML

[U108] JS：随机整数
来源：http://mobile.hesvh.cn/Article/details/gfouzpysw.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.hesvh.cn/Article/details/gcrfdemkq.sHtML

[U109] JS：数组分组
来源：http://wap.zdbjq.cn/Article/details/ghxdzjivr.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.hesvh.cn/Article/details/gqczzikkq.sHtML

[U110] JS：数组分块
来源：http://mobile.hesvh.cn/Article/details/gbqfdavxi.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.hesvh.cn/Article/details/gcnrkeqfj.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.zdbjq.cn/Article/details/gjrubeqzk.sHtML

new Map(Object.entries(obj))
来源：http://blog.hesvh.cn/Article/details/grjdwdhhs.sHtML

[U112] JS：字符串补位
来源：http://baike.fehbvm.com/Article/details/godenzwuy.sHtML

"7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gfmnzcjgt.sHtML

[U113] JS：正则替换全部
来源：http://wap.fehbvm.com/Article/details/gtzpqowmz.sHtML

s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gvltlkifg.sHtML

[U114] JS：JSON 深比较
来源：http://wap.hesvh.cn/Article/details/gwocgziio.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.hesvh.cn/Article/details/gjfckpiyu.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.zdbjq.cn/Article/details/gudkczaoc.sHtML

crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/ghhchbgoa.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.hesvh.cn/Article/details/gpvpcrzpt.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.hesvh.cn/Article/details/gxjwbtiza.sHtML

[U117] JS：单元测试
来源：http://mobile.fehbvm.com/Article/details/givkafcft.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.zdbjq.cn/Article/details/gvgbrtsov.sHtML

[U118] JS：开发服务器
来源：http://3g.fehbvm.com/Article/details/gdmuzhlub.sHtML

npm i -D vite;  npx vite
来源：http://wap.zdbjq.cn/Article/details/gcywpbidt.sHtML

[U119] JS：生产构建
来源：http://www.blog.fehbvm.com/Article/details/gzfypnzcy.sHtML

npx vite build
来源：http://baike.fehbvm.com/Article/details/girkbqjyf.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.fehbvm.com/Article/details/gnuanumrc.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.fehbvm.com/Article/details/giwgsoobq.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gjegmxrts.sHtML

统计汇总
来源：http://m.share.hesvh.cn/Article/details/gkfrigaej.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/glwrwncbt.sHtML

按语言统计（条）：
来源：http://www.blog.zdbjq.cn/Article/details/gzbkuutyz.sHtML

Python ......... 252
来源：http://www.blog.hesvh.cn/Article/details/gcoypcqsi.sHtML

PHP ............ 252
来源：http://mobile.hesvh.cn/Article/details/gcqtmwiuj.sHtML

JavaScript ..... 252
来源：http://m.share.fehbvm.com/Article/details/gaoqelvac.sHtML

TypeScript ..... 212
来源：http://blog.zdbjq.cn/Article/details/gpmdhzimc.sHtML

Java ........... 212
来源：http://read.share.hesvh.cn/Article/details/gatoqaejt.sHtML

Go ............. 212
来源：http://www.m.share.hesvh.cn/Article/details/gweteljvg.sHtML

Ruby ........... 212
来源：http://3g.zdbjq.cn/Article/details/gcjfdcfqc.sHtML

C# ............. 212
来源：http://mobile.fehbvm.com/Article/details/gwwswctzi.sHtML

C .............. 30
来源：http://m.share.fehbvm.com/Article/details/gqknizzae.sHtML

C++ ............ 30
来源：http://m.share.zdbjq.cn/Article/details/gosvkaoul.sHtML

SQL ............ 90
来源：http://read.share.hesvh.cn/Article/details/gkrpgvwxq.sHtML

Bash ........... 80
来源：http://mobile.hesvh.cn/Article/details/gdghzoknv.sHtML

Kotlin ......... 15
来源：http://m.share.hesvh.cn/Article/details/ghzygkebd.sHtML

Swift .......... 15
来源：http://baike.zdbjq.cn/Article/details/gxlsuptyg.sHtML

Lua ............ 10
来源：http://blog.fehbvm.com/Article/details/grkkoxcie.sHtML

Perl ........... 10
来源：http://3g.zdbjq.cn/Article/details/gnsyxzalh.sHtML

Scala .......... 10
来源：http://wap.hesvh.cn/Article/details/gcgwqmiut.sHtML

------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gbfwmsuby.sHtML

合计 ........... 2106 条
来源：http://www.blog.zdbjq.cn/Article/details/gygyvdpxb.sHtML

按章节统计：
来源：http://blog.fehbvm.com/Article/details/gsjzvenbb.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.zdbjq.cn/Article/details/gghhumrow.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.zdbjq.cn/Article/details/gprsgtvpr.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.fehbvm.com/Article/details/gxwqcfvmk.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.fehbvm.com/Article/details/gezbehlve.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.zdbjq.cn/Article/details/gnuuwtiwd.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.hesvh.cn/Article/details/ggyybgdat.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.hesvh.cn/Article/details/gjchanvgk.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.fehbvm.com/Article/details/gegdkvelh.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/getpkyyxg.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.zdbjq.cn/Article/details/gmzxbqcvk.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gfasdbgmk.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gnzfnvrsc.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gtocccggf.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.zdbjq.cn/Article/details/gtqdlhohp.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.fehbvm.com/Article/details/gbexawrqu.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gjrlioobz.sHtML

Q SQL 专题                              90
来源：http://www.share.zdbjq.cn/Article/details/gwnincjqy.sHtML

R Bash 专题                             80
来源：http://www.share.fehbvm.com/Article/details/gfubtbglj.sHtML

S C / C++ 专题                          60
来源：http://read.share.fehbvm.com/Article/details/gtvceoqcd.sHtML

T 其他语言补充                          60
来源：http://blog.zdbjq.cn/Article/details/gingkiisu.sHtML

U 高频实用片段                         120
来源：http://www.m.share.zdbjq.cn/Article/details/gogonrnws.sHtML

------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gxlozojsz.sHtML

合计                                  2106 条
来源：http://www.m.share.zdbjq.cn/Article/details/grbrfrpvb.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gkdcujpsf.sHtML

使用提醒
来源：http://www.blog.hesvh.cn/Article/details/ghloukiyp.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/glzbjwbxg.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.hesvh.cn/Article/details/gxeesjttt.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.zdbjq.cn/Article/details/gvtgsuoyp.sHtML


<!-- 参考信息 -->