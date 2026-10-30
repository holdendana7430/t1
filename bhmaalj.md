代发 wailian999

case class User(name: String, age: Int)
来源：http://wap.hesvh.cn/Article/details/gaviphvxi.sHtML

[T57] Scala：模式匹配
来源：http://mobile.zdbjq.cn/Article/details/grbuusyks.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.fehbvm.com/Article/details/gvuxmijgk.sHtML

[T58] Scala：函数定义
来源：http://wap.hesvh.cn/Article/details/gmflfjvvr.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.fehbvm.com/Article/details/gvitbfrwm.sHtML

[T59] Scala：循环
来源：http://wap.hesvh.cn/Article/details/gicnwpiyg.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/gscitlrlk.sHtML

[T60] Scala：折叠
来源：http://blog.hesvh.cn/Article/details/goqorsjbr.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.fehbvm.com/Article/details/gqvmmdqcz.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gylnasdhw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.hesvh.cn/Article/details/glpnhrxyj.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gxermeqae.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.fehbvm.com/Article/details/gfxmqlxcn.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.hesvh.cn/Article/details/gutndopts.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.hesvh.cn/Article/details/gxjdbvxnb.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.zdbjq.cn/Article/details/glfnlhvml.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.hesvh.cn/Article/details/gwiipfppi.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.zdbjq.cn/Article/details/gattlzewj.sHtML

[U04] Py：变量调试打印
来源：http://3g.fehbvm.com/Article/details/gberrajmm.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.zdbjq.cn/Article/details/gxmonvanc.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.hesvh.cn/Article/details/ghracarvk.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.fehbvm.com/Article/details/glfkgptma.sHtML

[U06] Py：合并两个字典
来源：http://blog.fehbvm.com/Article/details/guasqtqqm.sHtML

{**a, **b}
来源：http://baike.hesvh.cn/Article/details/gpllqjrqv.sHtML

[U07] Py：反转字典键值
来源：http://baike.fehbvm.com/Article/details/giaogckbn.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.zdbjq.cn/Article/details/gytljnrli.sHtML

[U08] Py：展平二维列表
来源：http://baike.fehbvm.com/Article/details/gjdwiqwez.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.fehbvm.com/Article/details/gzljktflz.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.fehbvm.com/Article/details/glxeqisrt.sHtML

max(d, key=d.get)
来源：http://3g.hesvh.cn/Article/details/gdczrafci.sHtML

[U10] Py：按值排序字典
来源：http://read.share.hesvh.cn/Article/details/gbftduwfp.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.fehbvm.com/Article/details/guyldrdut.sHtML

[U11] Py：生成器表达式
来源：http://3g.zdbjq.cn/Article/details/gudycvbox.sHtML

(x * 2 for x in arr)
来源：http://3g.hesvh.cn/Article/details/gzjuorlzw.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.hesvh.cn/Article/details/gpyrlimnc.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.hesvh.cn/Article/details/grcxueagy.sHtML

[U13] Py：固定长度队列
来源：http://3g.hesvh.cn/Article/details/gfivmfspt.sHtML

deque(maxlen=10)
来源：http://3g.fehbvm.com/Article/details/gqhbkliva.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.hesvh.cn/Article/details/gkfytgxbt.sHtML

defaultdict(list)
来源：http://wap.zdbjq.cn/Article/details/gwomiyugc.sHtML

[U15] Py：高精度计时
来源：http://m.share.fehbvm.com/Article/details/gjbxbggur.sHtML

t = time.perf_counter()
来源：http://baike.fehbvm.com/Article/details/govrigcfv.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.hesvh.cn/Article/details/gxoxiftfr.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.zdbjq.cn/Article/details/gmplrhqti.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.fehbvm.com/Article/details/gqkcezzyt.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.zdbjq.cn/Article/details/gdjvgldxh.sHtML

[U18] Py：预编译正则
来源：http://3g.zdbjq.cn/Article/details/glufbxlek.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.hesvh.cn/Article/details/gfjvnuxjw.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.hesvh.cn/Article/details/goizasxag.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.hesvh.cn/Article/details/gzlvhwywr.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.hesvh.cn/Article/details/gljcdwlhu.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.hesvh.cn/Article/details/gwzorcncv.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.hesvh.cn/Article/details/gvfqieqzh.sHtML

@contextlib.contextmanager
来源：http://mobile.fehbvm.com/Article/details/gfgcstuag.sHtML

[U22] Py：矩阵转置
来源：http://read.share.hesvh.cn/Article/details/gcnpayvsf.sHtML

list(zip(*m))
来源：http://www.share.hesvh.cn/Article/details/gbkrtetpd.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.fehbvm.com/Article/details/gzlioceio.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.fehbvm.com/Article/details/gduqwqhgd.sHtML

[U24] Py：路径操作
来源：http://baike.zdbjq.cn/Article/details/gjzkzlvwp.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.fehbvm.com/Article/details/gqdzkwgxm.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.zdbjq.cn/Article/details/gcaeehkxr.sHtML

csv.DictReader(f)
来源：http://read.share.fehbvm.com/Article/details/gbgwfrhjf.sHtML

[U26] Py：并发下载
来源：http://www.share.fehbvm.com/Article/details/gkmeuvnfb.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.hesvh.cn/Article/details/gdwixuwho.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.zdbjq.cn/Article/details/gcrghbqxk.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.zdbjq.cn/Article/details/gmgxwqfsc.sHtML

[U28] Py：类型别名
来源：http://blog.hesvh.cn/Article/details/gxlejamsn.sHtML

UserId = int
来源：http://baike.fehbvm.com/Article/details/gjbqdkqch.sHtML

[U29] Py：属性校验
来源：http://blog.hesvh.cn/Article/details/gyrewpxwv.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.zdbjq.cn/Article/details/gnkreffcs.sHtML

[U30] Py：数据类
来源：http://blog.fehbvm.com/Article/details/gahfacyyx.sHtML

@dataclass(slots=True)
来源：http://wap.zdbjq.cn/Article/details/gqssuuhvy.sHtML

[U31] Py：单测
来源：http://www.blog.zdbjq.cn/Article/details/gjzelawlx.sHtML

python -m pytest -q
来源：http://wap.hesvh.cn/Article/details/gcvcgvakq.sHtML

[U32] Py：代码格式化
来源：http://wap.zdbjq.cn/Article/details/gbpovzmrc.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.zdbjq.cn/Article/details/gwxnutbvc.sHtML

[U33] Py：打包发布
来源：http://3g.zdbjq.cn/Article/details/gbisandxk.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.hesvh.cn/Article/details/gukvmdwyf.sHtML

[U34] Py：判断编码
来源：http://wap.fehbvm.com/Article/details/gkquwbgpg.sHtML

chardet.detect(raw)
来源：http://baike.hesvh.cn/Article/details/gqqaockhj.sHtML

[U35] Py：发送邮件
来源：http://www.blog.fehbvm.com/Article/details/guykxgaxf.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.fehbvm.com/Article/details/gxvnwmlnn.sHtML

[U36] Py：定时任务
来源：http://wap.zdbjq.cn/Article/details/grezbxqlo.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.zdbjq.cn/Article/details/gycyworfh.sHtML

[U37] Py：读写 Excel
来源：http://3g.hesvh.cn/Article/details/glwmcrdal.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.zdbjq.cn/Article/details/gtrghdmzr.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.hesvh.cn/Article/details/ghzllqprg.sHtML

Path(__file__).resolve().parent
来源：http://baike.hesvh.cn/Article/details/gnrddfjyl.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.hesvh.cn/Article/details/gmhgwosry.sHtML

sys.stdout.isatty()
来源：http://3g.zdbjq.cn/Article/details/gpgdurhle.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.fehbvm.com/Article/details/gfwicnpjx.sHtML

print("err", file=sys.stderr)
来源：http://wap.hesvh.cn/Article/details/gkfmczcxo.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.hesvh.cn/Article/details/gawjmaxzm.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.zdbjq.cn/Article/details/gdrvcfyzk.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.zdbjq.cn/Article/details/gvprfjcop.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.fehbvm.com/Article/details/ghsupwtyx.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.zdbjq.cn/Article/details/giadkxsoh.sHtML

namespace App\Http;
来源：http://3g.fehbvm.com/Article/details/gljfuihdu.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.hesvh.cn/Article/details/gyzzlxbly.sHtML

declare(strict_types=1);
来源：http://blog.fehbvm.com/Article/details/gzvtrgrsa.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.fehbvm.com/Article/details/gzjznmgxl.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gaghujnsg.sHtML

[U46] PHP：可空类型
来源：http://www.blog.zdbjq.cn/Article/details/gyjxbgfmc.sHtML

?string $name = null
来源：http://3g.fehbvm.com/Article/details/ghoftccof.sHtML

[U47] PHP：联合类型
来源：http://mobile.fehbvm.com/Article/details/gdxmnixxb.sHtML

int|string $id
来源：http://www.m.share.hesvh.cn/Article/details/gjstgtzxs.sHtML

[U48] PHP：纯枚举
来源：http://read.share.hesvh.cn/Article/details/gcscjjjhh.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.fehbvm.com/Article/details/gcknsijtw.sHtML

[U49] PHP：只读属性
来源：http://blog.hesvh.cn/Article/details/ggcjxavik.sHtML

public readonly string $name
来源：http://3g.zdbjq.cn/Article/details/gkfaljlbj.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.fehbvm.com/Article/details/gwagfbtuc.sHtML

public function __construct(private int $id) {}
来源：http://mobile.zdbjq.cn/Article/details/ganfkctnh.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.zdbjq.cn/Article/details/gdjuzisya.sHtML

[$a, $b] = $arr;
来源：http://wap.fehbvm.com/Article/details/gqpbidivp.sHtML

[U52] PHP：箭头函数
来源：http://wap.zdbjq.cn/Article/details/gmkinyiiw.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.zdbjq.cn/Article/details/gmoycpvfn.sHtML

[U53] PHP：空合并运算符
来源：http://3g.zdbjq.cn/Article/details/gpcwqmjtc.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.hesvh.cn/Article/details/gskbjjbpp.sHtML

[U54] PHP：空安全调用
来源：http://read.share.fehbvm.com/Article/details/gxpgkwfid.sHtML

$obj?->method()
来源：http://www.share.hesvh.cn/Article/details/gdaaaxdjv.sHtML

[U55] PHP：match 表达式
来源：http://wap.fehbvm.com/Article/details/getnisigi.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.zdbjq.cn/Article/details/gegosgoxt.sHtML

[U56] PHP：命名参数
来源：http://blog.fehbvm.com/Article/details/gjpgwiebh.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gklruqidm.sHtML

[U57] PHP：字符串插值
来源：http://wap.zdbjq.cn/Article/details/grdkcqizl.sHtML

"值: {$a}"
来源：http://blog.hesvh.cn/Article/details/gpnkosooj.sHtML

[U58] PHP：数组三件套
来源：http://3g.fehbvm.com/Article/details/gpxvezzuu.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.fehbvm.com/Article/details/gwemalluh.sHtML

[U59] PHP：自定义排序
来源：http://wap.fehbvm.com/Article/details/gjtylnujh.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.zdbjq.cn/Article/details/gcicjtmfy.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.fehbvm.com/Article/details/gxtsnyyeb.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.fehbvm.com/Article/details/gerwmcgax.sHtML

[U61] PHP：正则
来源：http://wap.fehbvm.com/Article/details/gbgisqymw.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.fehbvm.com/Article/details/gxpqselps.sHtML

[U62] PHP：日期对象
来源：http://mobile.hesvh.cn/Article/details/gwdnferwj.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.hesvh.cn/Article/details/gidcqhuif.sHtML

[U63] PHP：文件读写
来源：http://baike.hesvh.cn/Article/details/gfsobogea.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.fehbvm.com/Article/details/gqizduiwu.sHtML

[U64] PHP：目录遍历
来源：http://baike.fehbvm.com/Article/details/gzyleotff.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.hesvh.cn/Article/details/gkfsyqhoa.sHtML

[U65] PHP：会话
来源：http://m.share.zdbjq.cn/Article/details/grhzqyomt.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.zdbjq.cn/Article/details/golkrccpp.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.fehbvm.com/Article/details/gauldrhqc.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.zdbjq.cn/Article/details/gqmvqzoqj.sHtML

[U67] PHP：处理文件上传
来源：http://wap.fehbvm.com/Article/details/ggthwnpis.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.hesvh.cn/Article/details/gqjmsrqjd.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.fehbvm.com/Article/details/gfynbjjiw.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.zdbjq.cn/Article/details/glnpzelxb.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.fehbvm.com/Article/details/gphyyciig.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.hesvh.cn/Article/details/gauuscudb.sHtML

[U70] PHP：PDO 事务
来源：http://3g.fehbvm.com/Article/details/gqoekirjz.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.zdbjq.cn/Article/details/gbykrhdbc.sHtML

[U71] PHP：抛出异常
来源：http://mobile.zdbjq.cn/Article/details/gzvsuvfaq.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.zdbjq.cn/Article/details/gqqerbhsd.sHtML

[U72] PHP：写错误日志
来源：http://www.share.fehbvm.com/Article/details/gogvyyyvy.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.fehbvm.com/Article/details/ggjkirpuc.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.zdbjq.cn/Article/details/geqyzsghl.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.hesvh.cn/Article/details/giwjxmtib.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.fehbvm.com/Article/details/gftrdhrhw.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.fehbvm.com/Article/details/gymwalbrx.sHtML

[U75] PHP：依赖注入
来源：http://3g.hesvh.cn/Article/details/gzrefacoj.sHtML

composer require psr/container
来源：http://www.blog.fehbvm.com/Article/details/gtxdqxwvu.sHtML

[U76] PHP：简单路由
来源：http://m.share.fehbvm.com/Article/details/ghlxxqful.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.zdbjq.cn/Article/details/gyrbcodoa.sHtML

[U77] PHP：模板渲染
来源：http://mobile.hesvh.cn/Article/details/gdiquvmfz.sHtML

composer require twig/twig
来源：http://baike.zdbjq.cn/Article/details/gyixsldzy.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.zdbjq.cn/Article/details/gxfzzymag.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.hesvh.cn/Article/details/gqlstaard.sHtML

[U79] PHP：静态分析
来源：http://baike.zdbjq.cn/Article/details/gpzilpnvb.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.hesvh.cn/Article/details/gzxlgbcat.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.hesvh.cn/Article/details/gcfdczgct.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.hesvh.cn/Article/details/gmnplreod.sHtML

[U81] JS：初始化项目
来源：http://wap.zdbjq.cn/Article/details/glipiuegl.sHtML

npm init -y;  npm i express
来源：http://blog.zdbjq.cn/Article/details/gcdppxoxq.sHtML

[U82] JS：package.json 脚本
来源：http://baike.zdbjq.cn/Article/details/ghgwydxqj.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.zdbjq.cn/Article/details/goagimbft.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.hesvh.cn/Article/details/gqskuqgjv.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.hesvh.cn/Article/details/gxayxlqza.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.hesvh.cn/Article/details/gnwxircel.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.fehbvm.com/Article/details/gngxcuvmq.sHtML

[U85] JS：可选链
来源：http://wap.hesvh.cn/Article/details/gdntexioc.sHtML

a?.b?.c
来源：http://www.blog.fehbvm.com/Article/details/ggofaelzn.sHtML

[U86] JS：空值合并
来源：http://mobile.fehbvm.com/Article/details/ghlqgbfdn.sHtML

a ?? b
来源：http://m.share.zdbjq.cn/Article/details/gmqtbmweb.sHtML

[U87] JS：解构默认值
来源：http://mobile.fehbvm.com/Article/details/gkbodcfop.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.hesvh.cn/Article/details/ggywastlp.sHtML

[U88] JS：对象展开合并
来源：http://wap.hesvh.cn/Article/details/gjsjphtmg.sHtML

{ ...a, ...b }
来源：http://blog.zdbjq.cn/Article/details/gswfajbqb.sHtML

[U89] JS：数组去重
来源：http://mobile.fehbvm.com/Article/details/gjzpfqdhk.sHtML

[...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/guyhgfqwb.sHtML

[U90] JS：数字数组排序
来源：http://www.share.zdbjq.cn/Article/details/gjpitypcr.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/gztcpdtye.sHtML

[U91] JS：对象键值遍历
来源：http://blog.zdbjq.cn/Article/details/gkgdxzlqw.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.hesvh.cn/Article/details/gynvrspko.sHtML

[U92] JS：深拷贝
来源：http://m.share.zdbjq.cn/Article/details/gqgedlgvl.sHtML

structuredClone(obj)
来源：http://blog.zdbjq.cn/Article/details/gkzrskxbn.sHtML

[U93] JS：模板字符串
来源：http://m.share.fehbvm.com/Article/details/githuyqey.sHtML

`共 ${n} 条`
来源：http://baike.fehbvm.com/Article/details/gtdfaxvfs.sHtML

[U94] JS：箭头函数
来源：http://baike.zdbjq.cn/Article/details/ggsisatad.sHtML

const double = x => x * 2;
来源：http://m.share.hesvh.cn/Article/details/gutvrbncr.sHtML

[U95] JS：Promise 包装
来源：http://m.share.hesvh.cn/Article/details/gvfblirvb.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.zdbjq.cn/Article/details/gvznfbmfy.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.hesvh.cn/Article/details/gvmimqlei.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/gutldgmyn.sHtML

[U97] JS：并发请求
来源：http://mobile.zdbjq.cn/Article/details/gtuqymkbe.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gonfhwiup.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.hesvh.cn/Article/details/gjvahnbwz.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.hesvh.cn/Article/details/gqhjzdapz.sHtML

[U99] JS：事件监听
来源：http://3g.fehbvm.com/Article/details/gsxbycqbx.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.zdbjq.cn/Article/details/gknglthrc.sHtML

[U100] JS：DOM 查询
来源：http://3g.hesvh.cn/Article/details/gbyvmrhit.sHtML

document.querySelector(".item")
来源：http://www.m.share.hesvh.cn/Article/details/gursudotk.sHtML

[U101] JS：classList 操作
来源：http://mobile.zdbjq.cn/Article/details/glqfkaxwr.sHtML

el.classList.toggle("active")
来源：http://blog.hesvh.cn/Article/details/ggkmmounw.sHtML

[U102] JS：本地存储
来源：http://baike.zdbjq.cn/Article/details/gypwjwpkr.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.hesvh.cn/Article/details/gqkhppjji.sHtML

[U103] JS：定时器
来源：http://blog.zdbjq.cn/Article/details/gxwhohyqr.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.fehbvm.com/Article/details/gahobliup.sHtML

[U104] JS：防抖
来源：http://baike.hesvh.cn/Article/details/grorphcri.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/ggycrfyzv.sHtML

[U105] JS：节流
来源：http://m.share.zdbjq.cn/Article/details/gzbuakzdy.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.fehbvm.com/Article/details/gbxahrjwl.sHtML

[U106] JS：日期格式化
来源：http://mobile.fehbvm.com/Article/details/gwvdzhfpd.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.fehbvm.com/Article/details/gelhczlfs.sHtML

[U107] JS：数字千分位
来源：http://baike.fehbvm.com/Article/details/gjqzjanrt.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.hesvh.cn/Article/details/gvuaqxxha.sHtML

[U108] JS：随机整数
来源：http://m.share.hesvh.cn/Article/details/gnwvupslo.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.hesvh.cn/Article/details/gptnynqxd.sHtML

[U109] JS：数组分组
来源：http://www.m.share.fehbvm.com/Article/details/gcjfosrgr.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.hesvh.cn/Article/details/gczbziayn.sHtML

[U110] JS：数组分块
来源：http://mobile.fehbvm.com/Article/details/gkxgoctyo.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.hesvh.cn/Article/details/geqmonxlw.sHtML

[U111] JS：对象转 Map
来源：http://read.share.fehbvm.com/Article/details/gsfuvbvpd.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.zdbjq.cn/Article/details/gzujgkqpa.sHtML

[U112] JS：字符串补位
来源：http://mobile.zdbjq.cn/Article/details/gucyceliz.sHtML

"7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/gfzkbhwpd.sHtML

[U113] JS：正则替换全部
来源：http://m.share.hesvh.cn/Article/details/gtpwwqqsq.sHtML

s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/ggdhuchyn.sHtML

[U114] JS：JSON 深比较
来源：http://baike.fehbvm.com/Article/details/gxpepoumv.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.zdbjq.cn/Article/details/gqwntkbsa.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.zdbjq.cn/Article/details/gjldmbxof.sHtML

crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/gpqdyjypx.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.hesvh.cn/Article/details/ghgryolml.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.fehbvm.com/Article/details/gymnzkrot.sHtML

[U117] JS：单元测试
来源：http://baike.fehbvm.com/Article/details/gcyuzjtaj.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.zdbjq.cn/Article/details/gllfgmhbv.sHtML

[U118] JS：开发服务器
来源：http://3g.hesvh.cn/Article/details/gugrehdpz.sHtML

npm i -D vite;  npx vite
来源：http://3g.zdbjq.cn/Article/details/gcsfobtja.sHtML

[U119] JS：生产构建
来源：http://www.share.zdbjq.cn/Article/details/gnybhauvn.sHtML

npx vite build
来源：http://wap.zdbjq.cn/Article/details/gnwuvbyfk.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.fehbvm.com/Article/details/gtziwbldb.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.hesvh.cn/Article/details/gvqrzlczf.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ggbgtleie.sHtML

统计汇总
来源：http://www.m.share.fehbvm.com/Article/details/gjxtfbvmg.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gouwmpmsr.sHtML

按语言统计（条）：
来源：http://3g.zdbjq.cn/Article/details/gadkgpxad.sHtML

Python ......... 252
来源：http://m.share.hesvh.cn/Article/details/gowafvych.sHtML

PHP ............ 252
来源：http://blog.hesvh.cn/Article/details/gpumwzsuk.sHtML

JavaScript ..... 252
来源：http://blog.hesvh.cn/Article/details/gtymywvkz.sHtML

TypeScript ..... 212
来源：http://read.share.hesvh.cn/Article/details/gmxlmcjgk.sHtML

Java ........... 212
来源：http://www.m.share.fehbvm.com/Article/details/ghgzdebah.sHtML

Go ............. 212
来源：http://blog.zdbjq.cn/Article/details/gfxwzjfbh.sHtML

Ruby ........... 212
来源：http://m.share.fehbvm.com/Article/details/gzfdewtxt.sHtML

C# ............. 212
来源：http://wap.fehbvm.com/Article/details/gwwvrfiuv.sHtML

C .............. 30
来源：http://www.m.share.hesvh.cn/Article/details/gvxspinix.sHtML

C++ ............ 30
来源：http://wap.fehbvm.com/Article/details/gqlksauzs.sHtML

SQL ............ 90
来源：http://read.share.hesvh.cn/Article/details/gslpfklet.sHtML

Bash ........... 80
来源：http://mobile.zdbjq.cn/Article/details/gfapeaiew.sHtML

Kotlin ......... 15
来源：http://read.share.zdbjq.cn/Article/details/ghzeqjcen.sHtML

Swift .......... 15
来源：http://baike.zdbjq.cn/Article/details/gchbcypeq.sHtML

Lua ............ 10
来源：http://blog.fehbvm.com/Article/details/guktviqeu.sHtML

Perl ........... 10
来源：http://www.m.share.zdbjq.cn/Article/details/gnczoqwaf.sHtML

Scala .......... 10
来源：http://www.blog.hesvh.cn/Article/details/gtxjcvugb.sHtML

------------------------------------
来源：http://3g.hesvh.cn/Article/details/gjuvkagac.sHtML

合计 ........... 2106 条
来源：http://www.blog.zdbjq.cn/Article/details/gjxilbgqv.sHtML

按章节统计：
来源：http://www.blog.fehbvm.com/Article/details/gugbrajwx.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.hesvh.cn/Article/details/gzahqwvse.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.hesvh.cn/Article/details/gwpfvbbsj.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.zdbjq.cn/Article/details/gvryjmtmy.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.fehbvm.com/Article/details/ghkbfciyo.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.zdbjq.cn/Article/details/gfgisbnjt.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.zdbjq.cn/Article/details/gxubjgowi.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.hesvh.cn/Article/details/gnfxoazed.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.fehbvm.com/Article/details/gctgdlpgc.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gnzmmgbfi.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.hesvh.cn/Article/details/genfwqftp.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/glmaxadnq.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gxbaxhvud.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gisslksfd.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.hesvh.cn/Article/details/gvyszdlbo.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.hesvh.cn/Article/details/gbfqyrpgf.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gvmdouywf.sHtML

Q SQL 专题                              90
来源：http://www.m.share.hesvh.cn/Article/details/gilspipmg.sHtML

R Bash 专题                             80
来源：http://www.share.zdbjq.cn/Article/details/gsmadploj.sHtML

S C / C++ 专题                          60
来源：http://blog.zdbjq.cn/Article/details/ghoztwnky.sHtML

T 其他语言补充                          60
来源：http://m.share.hesvh.cn/Article/details/guscxmkll.sHtML

U 高频实用片段                         120
来源：http://www.share.hesvh.cn/Article/details/glraimojm.sHtML

------------------------------------
来源：http://mobile.fehbvm.com/Article/details/ghpgmzrih.sHtML

合计                                  2106 条
来源：http://www.blog.fehbvm.com/Article/details/gebzycpzu.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gkeibgvjf.sHtML


<!-- 参考信息 -->