代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fanxiaobao.xyz/Article/details/gwtdbrqsc.sHtML

[T59] Scala：循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzdnafybw.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.fanxiaobao.xyz/Article/details/geakgcwml.sHtML

[T60] Scala：折叠
来源：http://baike.fanxiaobao.xyz/Article/details/gvysvaggx.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.fanxiaobao.xyz/Article/details/gfjsrhuqc.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghvhycijk.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gfdkjptsb.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gwqmgjhqe.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.fanxiaobao.xyz/Article/details/gxvvddspa.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.fanxiaobao.xyz/Article/details/gueurlfaf.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gifvazbou.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gyscerhzg.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.fanxiaobao.xyz/Article/details/gkoexizkv.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.fanxiaobao.xyz/Article/details/gdjimezih.sHtML

[U04] Py：变量调试打印
来源：http://www.share.fanxiaobao.xyz/Article/details/gdbrqhguy.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fanxiaobao.xyz/Article/details/gsfkgdsbq.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.fanxiaobao.xyz/Article/details/gxbkehwzv.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gubsjgrzk.sHtML

[U06] Py：合并两个字典
来源：http://3g.fanxiaobao.xyz/Article/details/ghilexmcy.sHtML

{**a, **b}
来源：http://read.share.fanxiaobao.xyz/Article/details/guegbnwto.sHtML

[U07] Py：反转字典键值
来源：http://www.share.fanxiaobao.xyz/Article/details/gzxqiqiuh.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.fanxiaobao.xyz/Article/details/grpsgwhzv.sHtML

[U08] Py：展平二维列表
来源：http://baike.fanxiaobao.xyz/Article/details/giwdajogf.sHtML

[y for x in nested for y in x]
来源：http://wap.fanxiaobao.xyz/Article/details/gugknbquw.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.fanxiaobao.xyz/Article/details/ghxwnybpm.sHtML

max(d, key=d.get)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggjebechl.sHtML

[U10] Py：按值排序字典
来源：http://baike.fanxiaobao.xyz/Article/details/gaczwaxfx.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gggyrioki.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gevrbrpcz.sHtML

(x * 2 for x in arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtopgpvyj.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gpncpegoj.sHtML

Counter(arr).most_common(3)
来源：http://baike.fanxiaobao.xyz/Article/details/gyfvxhdwy.sHtML

[U13] Py：固定长度队列
来源：http://m.share.fanxiaobao.xyz/Article/details/ghflycwtn.sHtML

deque(maxlen=10)
来源：http://wap.fanxiaobao.xyz/Article/details/goihjsooi.sHtML

[U14] Py：分组收集到列表
来源：http://baike.fanxiaobao.xyz/Article/details/gjaxjesmm.sHtML

defaultdict(list)
来源：http://baike.fanxiaobao.xyz/Article/details/grkqcnwqu.sHtML

[U15] Py：高精度计时
来源：http://baike.fanxiaobao.xyz/Article/details/gcrvqqoun.sHtML

t = time.perf_counter()
来源：http://blog.fanxiaobao.xyz/Article/details/gktktcdrt.sHtML

[U16] Py：命令行参数解析
来源：http://3g.fanxiaobao.xyz/Article/details/gdbjwjanw.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fanxiaobao.xyz/Article/details/gltzgnfgt.sHtML

[U17] Py：初始化日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gqlxiettm.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.fanxiaobao.xyz/Article/details/gvrikdslo.sHtML

[U18] Py：预编译正则
来源：http://www.share.fanxiaobao.xyz/Article/details/gnfqhdraj.sHtML

pat = re.compile(r"\d+")
来源：http://wap.fanxiaobao.xyz/Article/details/gfdzhrpgz.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.fanxiaobao.xyz/Article/details/gddlqnptj.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gklahuocm.sHtML

[U20] Py：缓存函数结果
来源：http://blog.fanxiaobao.xyz/Article/details/gnxlphkoj.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnwkllxlu.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyjloqhtl.sHtML

@contextlib.contextmanager
来源：http://wap.fanxiaobao.xyz/Article/details/gpqruicro.sHtML

[U22] Py：矩阵转置
来源：http://3g.fanxiaobao.xyz/Article/details/gfyljyaiz.sHtML

list(zip(*m))
来源：http://wap.fanxiaobao.xyz/Article/details/gioemsypr.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gbkuvbnot.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.fanxiaobao.xyz/Article/details/gctfowvae.sHtML

[U24] Py：路径操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gttispvdo.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxfrkhinc.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.fanxiaobao.xyz/Article/details/guloyeckv.sHtML

csv.DictReader(f)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmnplijiw.sHtML

[U26] Py：并发下载
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvryaxmqk.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaeujibnx.sHtML

[U27] Py：异步 HTTP
来源：http://blog.fanxiaobao.xyz/Article/details/gedjnsgbu.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghjboqikh.sHtML

[U28] Py：类型别名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glylhswvf.sHtML

UserId = int
来源：http://blog.fanxiaobao.xyz/Article/details/gkqbdqjmw.sHtML

[U29] Py：属性校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsgqdadhk.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.fanxiaobao.xyz/Article/details/gayagqiqp.sHtML

[U30] Py：数据类
来源：http://m.share.fanxiaobao.xyz/Article/details/gmrirdvyh.sHtML

@dataclass(slots=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxdwlpswr.sHtML

[U31] Py：单测
来源：http://wap.fanxiaobao.xyz/Article/details/ghtnjbqnc.sHtML

python -m pytest -q
来源：http://www.share.fanxiaobao.xyz/Article/details/gasgrayxv.sHtML

[U32] Py：代码格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gkjxqqrbm.sHtML

ruff format . && ruff check --fix .
来源：http://baike.fanxiaobao.xyz/Article/details/gclwlubsd.sHtML

[U33] Py：打包发布
来源：http://www.share.fanxiaobao.xyz/Article/details/gcbbkwmyc.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.fanxiaobao.xyz/Article/details/gbamhyyac.sHtML

[U34] Py：判断编码
来源：http://read.share.fanxiaobao.xyz/Article/details/gevqjupkf.sHtML

chardet.detect(raw)
来源：http://3g.fanxiaobao.xyz/Article/details/gqgrjeiqc.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbxdjduhx.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.fanxiaobao.xyz/Article/details/gimaurlgj.sHtML

[U36] Py：定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/ghzdqytbn.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghediqunp.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdevdivjp.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.fanxiaobao.xyz/Article/details/gxvzmvnob.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.fanxiaobao.xyz/Article/details/griaortgb.sHtML

Path(__file__).resolve().parent
来源：http://3g.fanxiaobao.xyz/Article/details/gsxzuwgar.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.fanxiaobao.xyz/Article/details/gokonktas.sHtML

sys.stdout.isatty()
来源：http://wap.fanxiaobao.xyz/Article/details/gxwkgjani.sHtML

[U40] Py：打印到标准错误
来源：http://3g.fanxiaobao.xyz/Article/details/gdrujuafv.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqklddwvw.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnsprttox.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpfjdfaam.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcupvsdgp.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.fanxiaobao.xyz/Article/details/gevrgvghi.sHtML

[U43] PHP：声明命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/gkjdkojoe.sHtML

namespace App\Http;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpykqhoaq.sHtML

[U44] PHP：开启严格类型
来源：http://3g.fanxiaobao.xyz/Article/details/gnvbhhfzo.sHtML

declare(strict_types=1);
来源：http://3g.fanxiaobao.xyz/Article/details/gkdooeazg.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.fanxiaobao.xyz/Article/details/ghlimlpit.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gjoeuwxrb.sHtML

[U46] PHP：可空类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gkspojrll.sHtML

?string $name = null
来源：http://baike.fanxiaobao.xyz/Article/details/gddaidaen.sHtML

[U47] PHP：联合类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gnayujage.sHtML

int|string $id
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpxthplxv.sHtML

[U48] PHP：纯枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/guowcuiwz.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gpnlzzgmr.sHtML

[U49] PHP：只读属性
来源：http://wap.fanxiaobao.xyz/Article/details/gzmkaylce.sHtML

public readonly string $name
来源：http://read.share.fanxiaobao.xyz/Article/details/gnkedebrk.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.fanxiaobao.xyz/Article/details/gzyutqdvi.sHtML

public function __construct(private int $id) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/guaoqwcaq.sHtML

[U51] PHP：数组解构
来源：http://mobile.fanxiaobao.xyz/Article/details/gejgzzcig.sHtML

[$a, $b] = $arr;
来源：http://m.share.fanxiaobao.xyz/Article/details/gamfswroy.sHtML

[U52] PHP：箭头函数
来源：http://blog.fanxiaobao.xyz/Article/details/gtmvtijfd.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfufewtcs.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.fanxiaobao.xyz/Article/details/gqxshlxeu.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcmqtyyqa.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmluwokpr.sHtML

$obj?->method()
来源：http://m.share.fanxiaobao.xyz/Article/details/gltpzchsm.sHtML

[U55] PHP：match 表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gdgchdpop.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.fanxiaobao.xyz/Article/details/gqdmyqftu.sHtML

[U56] PHP：命名参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjtqifbqi.sHtML

f(a: 1, b: 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gtkdvxfch.sHtML

[U57] PHP：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/guehalgin.sHtML

"值: {$a}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gwqvsajwd.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwxrxsdrm.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.fanxiaobao.xyz/Article/details/gteakslpr.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geebttntg.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyjzjmvoj.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.fanxiaobao.xyz/Article/details/gmppckulw.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.fanxiaobao.xyz/Article/details/gsyddshgu.sHtML

[U61] PHP：正则
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gclurdiuj.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gigmzhntx.sHtML

[U62] PHP：日期对象
来源：http://3g.fanxiaobao.xyz/Article/details/goqcaifvw.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.fanxiaobao.xyz/Article/details/gcyssbedx.sHtML

[U63] PHP：文件读写
来源：http://baike.fanxiaobao.xyz/Article/details/glqwgsnka.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.fanxiaobao.xyz/Article/details/glbhntpzj.sHtML

[U64] PHP：目录遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gwxefhlfo.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.fanxiaobao.xyz/Article/details/gawkvabgd.sHtML

[U65] PHP：会话
来源：http://baike.fanxiaobao.xyz/Article/details/gnsidwcpg.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkkuusvdr.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.fanxiaobao.xyz/Article/details/gykcmhrcu.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwnlbrxcw.sHtML

[U67] PHP：处理文件上传
来源：http://baike.fanxiaobao.xyz/Article/details/gbkovoxum.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmekzivwu.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gtprablfk.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.fanxiaobao.xyz/Article/details/gcimnucvv.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gzjkeulfo.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjfvmighd.sHtML

[U70] PHP：PDO 事务
来源：http://blog.fanxiaobao.xyz/Article/details/geyhenftg.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gurlutich.sHtML

[U71] PHP：抛出异常
来源：http://read.share.fanxiaobao.xyz/Article/details/gnallgrqi.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.fanxiaobao.xyz/Article/details/gvtlhdnsc.sHtML

[U72] PHP：写错误日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gekpxkatu.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.fanxiaobao.xyz/Article/details/glhldqfjb.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.fanxiaobao.xyz/Article/details/gecmttemx.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.fanxiaobao.xyz/Article/details/gqzertvnf.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gplqmztdu.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.fanxiaobao.xyz/Article/details/gdavsmgwt.sHtML

[U75] PHP：依赖注入
来源：http://3g.fanxiaobao.xyz/Article/details/gpmbdbfov.sHtML

composer require psr/container
来源：http://baike.fanxiaobao.xyz/Article/details/grqkqotls.sHtML

[U76] PHP：简单路由
来源：http://www.share.fanxiaobao.xyz/Article/details/ggwzsivoa.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.fanxiaobao.xyz/Article/details/gwoiocrpb.sHtML

[U77] PHP：模板渲染
来源：http://mobile.fanxiaobao.xyz/Article/details/gukkfrbnr.sHtML

composer require twig/twig
来源：http://baike.fanxiaobao.xyz/Article/details/glpmtjovi.sHtML

[U78] PHP：单元测试
来源：http://mobile.fanxiaobao.xyz/Article/details/gcjdphebm.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.fanxiaobao.xyz/Article/details/gpnrbogok.sHtML

[U79] PHP：静态分析
来源：http://m.share.fanxiaobao.xyz/Article/details/gevlvwxhm.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.fanxiaobao.xyz/Article/details/gxyhetwus.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.fanxiaobao.xyz/Article/details/gndtddgtm.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.fanxiaobao.xyz/Article/details/gbnmtbjks.sHtML

[U81] JS：初始化项目
来源：http://read.share.fanxiaobao.xyz/Article/details/gfhyjfanl.sHtML

npm init -y;  npm i express
来源：http://m.share.fanxiaobao.xyz/Article/details/gakwyhvnd.sHtML

[U82] JS：package.json 脚本
来源：http://baike.fanxiaobao.xyz/Article/details/ghjonfbwx.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzobmvcql.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.fanxiaobao.xyz/Article/details/gjssornyw.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.fanxiaobao.xyz/Article/details/gwpbphvao.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.fanxiaobao.xyz/Article/details/glpbcwkit.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.fanxiaobao.xyz/Article/details/geyctjvun.sHtML

[U85] JS：可选链
来源：http://read.share.fanxiaobao.xyz/Article/details/gmgvljbgr.sHtML

a?.b?.c
来源：http://read.share.fanxiaobao.xyz/Article/details/gosewaqve.sHtML

[U86] JS：空值合并
来源：http://read.share.fanxiaobao.xyz/Article/details/gehnltyly.sHtML

a ?? b
来源：http://www.share.fanxiaobao.xyz/Article/details/guptdvzam.sHtML

[U87] JS：解构默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/gnybfhrck.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.fanxiaobao.xyz/Article/details/guuxzysyh.sHtML

[U88] JS：对象展开合并
来源：http://baike.fanxiaobao.xyz/Article/details/gxoltvpdj.sHtML

{ ...a, ...b }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmbxlgred.sHtML

[U89] JS：数组去重
来源：http://blog.fanxiaobao.xyz/Article/details/gzszjerop.sHtML

[...new Set(arr)]
来源：http://mobile.fanxiaobao.xyz/Article/details/gyengogus.sHtML

[U90] JS：数字数组排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gclokrqtx.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gweiynget.sHtML

[U91] JS：对象键值遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gdnbswrfb.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.fanxiaobao.xyz/Article/details/gdvbzeoqs.sHtML

[U92] JS：深拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gomshcdqx.sHtML

structuredClone(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/gtvxahjhz.sHtML

[U93] JS：模板字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/giwjkqvbd.sHtML

`共 ${n} 条`
来源：http://wap.fanxiaobao.xyz/Article/details/gzdufsorg.sHtML

[U94] JS：箭头函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjcttxufz.sHtML

const double = x => x * 2;
来源：http://mobile.fanxiaobao.xyz/Article/details/gatydcbhn.sHtML

[U95] JS：Promise 包装
来源：http://www.share.fanxiaobao.xyz/Article/details/gehllzwzy.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.fanxiaobao.xyz/Article/details/gmjqnaeow.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.fanxiaobao.xyz/Article/details/gcbzzybdl.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.fanxiaobao.xyz/Article/details/gjqwupstn.sHtML

[U97] JS：并发请求
来源：http://3g.fanxiaobao.xyz/Article/details/glavjsyed.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fanxiaobao.xyz/Article/details/gyhhmpfhq.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/gsxbabwqs.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.fanxiaobao.xyz/Article/details/gwsrpnycr.sHtML

[U99] JS：事件监听
来源：http://m.share.fanxiaobao.xyz/Article/details/glsauusws.sHtML

el.addEventListener("click", e => {})
来源：http://wap.fanxiaobao.xyz/Article/details/ggdipfrce.sHtML

[U100] JS：DOM 查询
来源：http://www.share.fanxiaobao.xyz/Article/details/guoflotjg.sHtML

document.querySelector(".item")
来源：http://m.share.fanxiaobao.xyz/Article/details/gikbrgfhn.sHtML

[U101] JS：classList 操作
来源：http://3g.fanxiaobao.xyz/Article/details/gujhxzqco.sHtML

el.classList.toggle("active")
来源：http://mobile.fanxiaobao.xyz/Article/details/gdvnzeemd.sHtML

[U102] JS：本地存储
来源：http://www.share.fanxiaobao.xyz/Article/details/gfhckovwm.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.fanxiaobao.xyz/Article/details/gjfevfacf.sHtML

[U103] JS：定时器
来源：http://mobile.fanxiaobao.xyz/Article/details/geqsacdut.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.fanxiaobao.xyz/Article/details/gaeabzhjg.sHtML

[U104] JS：防抖
来源：http://mobile.fanxiaobao.xyz/Article/details/gyjzwfiuh.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gdtuendmk.sHtML

[U105] JS：节流
来源：http://read.share.fanxiaobao.xyz/Article/details/ghrlfrpeq.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmedgpefd.sHtML

[U106] JS：日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/ganqvrpsz.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gthulioex.sHtML

[U107] JS：数字千分位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbpbegdmv.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gidihzpyn.sHtML

[U108] JS：随机整数
来源：http://read.share.fanxiaobao.xyz/Article/details/gjmyhvsuf.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.fanxiaobao.xyz/Article/details/gxaoazdxv.sHtML

[U109] JS：数组分组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwrlcvgok.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfdixywrd.sHtML

[U110] JS：数组分块
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpahflznf.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.fanxiaobao.xyz/Article/details/gkcxkthvp.sHtML

[U111] JS：对象转 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/gkhrualzp.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.fanxiaobao.xyz/Article/details/grdgzsoiy.sHtML

[U112] JS：字符串补位
来源：http://blog.fanxiaobao.xyz/Article/details/gsynulbwt.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gljikutei.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtvoutsjl.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcjvswtsy.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.fanxiaobao.xyz/Article/details/ggvlootct.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gregjkzhc.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmdjhquhc.sHtML

crypto.randomUUID()
来源：http://read.share.fanxiaobao.xyz/Article/details/gcfbyeohv.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.fanxiaobao.xyz/Article/details/gseojzsid.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gbyssnoww.sHtML

[U117] JS：单元测试
来源：http://3g.fanxiaobao.xyz/Article/details/ghonxvmjb.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghzctjiik.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmdpjowma.sHtML

npm i -D vite;  npx vite
来源：http://blog.fanxiaobao.xyz/Article/details/gpxswflyb.sHtML

[U119] JS：生产构建
来源：http://3g.fanxiaobao.xyz/Article/details/gthefbdlz.sHtML

npx vite build
来源：http://blog.fanxiaobao.xyz/Article/details/gxradquvc.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gajrzmgna.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.fanxiaobao.xyz/Article/details/geccekwzm.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/grxlhtqsz.sHtML

统计汇总
来源：http://blog.fanxiaobao.xyz/Article/details/gidflytha.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gbypglwal.sHtML

按语言统计（条）：
来源：http://3g.fanxiaobao.xyz/Article/details/gnluofcmr.sHtML

Python ......... 252
来源：http://baike.fanxiaobao.xyz/Article/details/gfwdmidzw.sHtML

PHP ............ 252
来源：http://blog.fanxiaobao.xyz/Article/details/gthsyviup.sHtML

JavaScript ..... 252
来源：http://blog.fanxiaobao.xyz/Article/details/gwokopjpo.sHtML

TypeScript ..... 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/girddozfy.sHtML

Java ........... 212
来源：http://baike.fanxiaobao.xyz/Article/details/gxqoguwwj.sHtML

Go ............. 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gqmnvriag.sHtML

Ruby ........... 212
来源：http://read.share.fanxiaobao.xyz/Article/details/grixcoogi.sHtML

C# ............. 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gthbphtgu.sHtML

C .............. 30
来源：http://baike.fanxiaobao.xyz/Article/details/gcqsbliqa.sHtML

C++ ............ 30
来源：http://read.share.fanxiaobao.xyz/Article/details/gtbgujjzv.sHtML

SQL ............ 90
来源：http://www.blog.fanxiaobao.xyz/Article/details/grsadajci.sHtML

Bash ........... 80
来源：http://read.share.fanxiaobao.xyz/Article/details/gjwommygi.sHtML

Kotlin ......... 15
来源：http://wap.fanxiaobao.xyz/Article/details/gbmgncwit.sHtML

Swift .......... 15
来源：http://baike.fanxiaobao.xyz/Article/details/gdfkrwdgh.sHtML

Lua ............ 10
来源：http://read.share.fanxiaobao.xyz/Article/details/glglhctal.sHtML

Perl ........... 10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaxcrmvdd.sHtML

Scala .......... 10
来源：http://baike.fanxiaobao.xyz/Article/details/gjcvyxydq.sHtML

------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfagfkcdh.sHtML

合计 ........... 2106 条
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geozsekpi.sHtML

按章节统计：
来源：http://baike.fanxiaobao.xyz/Article/details/gpszkuaeq.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.fanxiaobao.xyz/Article/details/gmrybechy.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.fanxiaobao.xyz/Article/details/gymvsgygb.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.fanxiaobao.xyz/Article/details/gutolxdbo.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gifgdlnbn.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.fanxiaobao.xyz/Article/details/guazfewnc.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.fanxiaobao.xyz/Article/details/gnyhkjhat.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.fanxiaobao.xyz/Article/details/gakgjisdb.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.fanxiaobao.xyz/Article/details/gtbfyywaq.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/goxgcrhre.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.fanxiaobao.xyz/Article/details/gylwltkkp.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/grxjbqojp.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/geqyifhtn.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gednueftp.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqefzxnag.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.fanxiaobao.xyz/Article/details/gbpraxmdt.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gutsuazmh.sHtML

Q SQL 专题                              90
来源：http://3g.fanxiaobao.xyz/Article/details/gvbttbbhm.sHtML

R Bash 专题                             80
来源：http://read.share.fanxiaobao.xyz/Article/details/gasllwkdf.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcwfgeuoy.sHtML

T 其他语言补充                          60
来源：http://m.share.fanxiaobao.xyz/Article/details/gdkpptcrg.sHtML

U 高频实用片段                         120
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkbaznfka.sHtML

------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/gutlghbhv.sHtML

合计                                  2106 条
来源：http://wap.fanxiaobao.xyz/Article/details/gnrgfqhyt.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzuhidcvq.sHtML

使用提醒
来源：http://m.share.fanxiaobao.xyz/Article/details/gwlotliod.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/gmsbsltzu.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.fanxiaobao.xyz/Article/details/gdzgfeuln.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfcchtrxe.sHtML


<!-- 参考信息 -->