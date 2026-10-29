代发 wailian999

case class User(name: String, age: Int)
来源：http://www.share.zdbjq.cn/Article/details/gzdconenf.sHtML

[T57] Scala：模式匹配
来源：http://m.share.fehbvm.com/Article/details/gmymdgveo.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.fehbvm.com/Article/details/ggxojftge.sHtML

[T58] Scala：函数定义
来源：http://blog.fehbvm.com/Article/details/gcvpzxark.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.fehbvm.com/Article/details/gbycdqzlg.sHtML

[T59] Scala：循环
来源：http://read.share.fehbvm.com/Article/details/gmmamjflr.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.zdbjq.cn/Article/details/gdrggyguy.sHtML

[T60] Scala：折叠
来源：http://www.blog.fehbvm.com/Article/details/goyjqkajr.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.hesvh.cn/Article/details/gzwcnqsfg.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gmnmvtqqr.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.hesvh.cn/Article/details/ghqkkijzi.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gijommtgs.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.zdbjq.cn/Article/details/gkwiawfdi.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.fehbvm.com/Article/details/gjytgnzne.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.zdbjq.cn/Article/details/gxdvjimiw.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.zdbjq.cn/Article/details/gdwpcvcqf.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.hesvh.cn/Article/details/gsdslsywi.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.fehbvm.com/Article/details/goookqmsm.sHtML

[U04] Py：变量调试打印
来源：http://www.share.fehbvm.com/Article/details/gxtmlqntx.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.fehbvm.com/Article/details/gdavndnjl.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.hesvh.cn/Article/details/ggugdtzld.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gjgmqvetq.sHtML

[U06] Py：合并两个字典
来源：http://baike.fehbvm.com/Article/details/ghcyvjxdh.sHtML

{**a, **b}
来源：http://m.share.fehbvm.com/Article/details/gmnysggto.sHtML

[U07] Py：反转字典键值
来源：http://mobile.fehbvm.com/Article/details/gqouypbdb.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.hesvh.cn/Article/details/gypjojgin.sHtML

[U08] Py：展平二维列表
来源：http://mobile.zdbjq.cn/Article/details/gfafdfeur.sHtML

[y for x in nested for y in x]
来源：http://baike.fehbvm.com/Article/details/gjzagumvo.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.fehbvm.com/Article/details/gyenvndaq.sHtML

max(d, key=d.get)
来源：http://m.share.zdbjq.cn/Article/details/gqdvjrscq.sHtML

[U10] Py：按值排序字典
来源：http://read.share.hesvh.cn/Article/details/gmibpwlxr.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.fehbvm.com/Article/details/grkwuvxgt.sHtML

[U11] Py：生成器表达式
来源：http://mobile.fehbvm.com/Article/details/gievoddvg.sHtML

(x * 2 for x in arr)
来源：http://www.blog.fehbvm.com/Article/details/gkzmzxovc.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.hesvh.cn/Article/details/grcseqayt.sHtML

Counter(arr).most_common(3)
来源：http://www.share.fehbvm.com/Article/details/gnbhnxifl.sHtML

[U13] Py：固定长度队列
来源：http://blog.zdbjq.cn/Article/details/gxqyvpunx.sHtML

deque(maxlen=10)
来源：http://m.share.fehbvm.com/Article/details/gvreanrqp.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.hesvh.cn/Article/details/gavmxkxck.sHtML

defaultdict(list)
来源：http://3g.hesvh.cn/Article/details/grqiosuhg.sHtML

[U15] Py：高精度计时
来源：http://www.share.hesvh.cn/Article/details/gptgarzqy.sHtML

t = time.perf_counter()
来源：http://baike.hesvh.cn/Article/details/gjvszusug.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.hesvh.cn/Article/details/gyuymdbvx.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.hesvh.cn/Article/details/gdfoquogw.sHtML

[U17] Py：初始化日志
来源：http://blog.hesvh.cn/Article/details/gbuvovqah.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.hesvh.cn/Article/details/gstditnzx.sHtML

[U18] Py：预编译正则
来源：http://baike.hesvh.cn/Article/details/gyozoqdhh.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.zdbjq.cn/Article/details/gbxfpkzpt.sHtML

[U19] Py：正则替换带回调
来源：http://3g.fehbvm.com/Article/details/gndqwtcia.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.zdbjq.cn/Article/details/gnkxrizsk.sHtML

[U20] Py：缓存函数结果
来源：http://wap.fehbvm.com/Article/details/gifyyhgko.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.zdbjq.cn/Article/details/gmwoaqqab.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.hesvh.cn/Article/details/ggynhmsiq.sHtML

@contextlib.contextmanager
来源：http://www.m.share.zdbjq.cn/Article/details/gdeixuujt.sHtML

[U22] Py：矩阵转置
来源：http://m.share.fehbvm.com/Article/details/guusmaoiu.sHtML

list(zip(*m))
来源：http://www.blog.hesvh.cn/Article/details/glilodvmc.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.fehbvm.com/Article/details/gipsxrrfy.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.zdbjq.cn/Article/details/gqoalgamz.sHtML

[U24] Py：路径操作
来源：http://www.share.fehbvm.com/Article/details/gabzbzoyh.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/gshirnccb.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.hesvh.cn/Article/details/gagafobyu.sHtML

csv.DictReader(f)
来源：http://wap.hesvh.cn/Article/details/gsdvpcyjz.sHtML

[U26] Py：并发下载
来源：http://read.share.hesvh.cn/Article/details/gedlisvxt.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.zdbjq.cn/Article/details/gkpricogc.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fehbvm.com/Article/details/gwdlhqqfz.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.hesvh.cn/Article/details/ghnfglqmt.sHtML

[U28] Py：类型别名
来源：http://www.share.zdbjq.cn/Article/details/gkaxwqfaq.sHtML

UserId = int
来源：http://www.share.hesvh.cn/Article/details/gbqjkwpon.sHtML

[U29] Py：属性校验
来源：http://www.share.zdbjq.cn/Article/details/gqpfclxkk.sHtML

@property 与 @x.setter 配合
来源：http://3g.fehbvm.com/Article/details/gjrwpprgv.sHtML

[U30] Py：数据类
来源：http://www.share.zdbjq.cn/Article/details/gqauaquvw.sHtML

@dataclass(slots=True)
来源：http://wap.zdbjq.cn/Article/details/gbtbjxdey.sHtML

[U31] Py：单测
来源：http://m.share.hesvh.cn/Article/details/gpaoasagj.sHtML

python -m pytest -q
来源：http://mobile.hesvh.cn/Article/details/gvdimpwwy.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.hesvh.cn/Article/details/galbguwyd.sHtML

ruff format . && ruff check --fix .
来源：http://wap.zdbjq.cn/Article/details/govewcfnr.sHtML

[U33] Py：打包发布
来源：http://www.m.share.hesvh.cn/Article/details/gxusvqpan.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.zdbjq.cn/Article/details/glgllemua.sHtML

[U34] Py：判断编码
来源：http://wap.fehbvm.com/Article/details/gpgsoabbv.sHtML

chardet.detect(raw)
来源：http://3g.zdbjq.cn/Article/details/gnxcighva.sHtML

[U35] Py：发送邮件
来源：http://3g.zdbjq.cn/Article/details/gjxljvvzz.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.fehbvm.com/Article/details/gvdpbhavf.sHtML

[U36] Py：定时任务
来源：http://3g.zdbjq.cn/Article/details/gbycwpcer.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.fehbvm.com/Article/details/gvpxovxek.sHtML

[U37] Py：读写 Excel
来源：http://www.share.zdbjq.cn/Article/details/gheueniee.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.hesvh.cn/Article/details/gcaoxpzdb.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.fehbvm.com/Article/details/gviwkedjm.sHtML

Path(__file__).resolve().parent
来源：http://m.share.zdbjq.cn/Article/details/gbqhznopg.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.hesvh.cn/Article/details/gsgzisnsa.sHtML

sys.stdout.isatty()
来源：http://wap.zdbjq.cn/Article/details/grocezhtd.sHtML

[U40] Py：打印到标准错误
来源：http://3g.zdbjq.cn/Article/details/ggakbdxgc.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.zdbjq.cn/Article/details/gkxaovrrt.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.zdbjq.cn/Article/details/gzjufchiz.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.hesvh.cn/Article/details/gearnaupm.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.hesvh.cn/Article/details/gjycfgdom.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.fehbvm.com/Article/details/gutwniipk.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.zdbjq.cn/Article/details/goqthivha.sHtML

namespace App\Http;
来源：http://mobile.zdbjq.cn/Article/details/gantdjwky.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.hesvh.cn/Article/details/gxtvgdwzi.sHtML

declare(strict_types=1);
来源：http://baike.zdbjq.cn/Article/details/gxkeluspr.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.fehbvm.com/Article/details/gmdghnqqr.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gymltkygi.sHtML

[U46] PHP：可空类型
来源：http://mobile.hesvh.cn/Article/details/golpbvdee.sHtML

?string $name = null
来源：http://read.share.zdbjq.cn/Article/details/gahmtsxmu.sHtML

[U47] PHP：联合类型
来源：http://wap.hesvh.cn/Article/details/gpnkmseno.sHtML

int|string $id
来源：http://read.share.hesvh.cn/Article/details/gfiprzsgh.sHtML

[U48] PHP：纯枚举
来源：http://m.share.zdbjq.cn/Article/details/gwnxvttnf.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.fehbvm.com/Article/details/giagligum.sHtML

[U49] PHP：只读属性
来源：http://3g.fehbvm.com/Article/details/gfzoergvb.sHtML

public readonly string $name
来源：http://baike.hesvh.cn/Article/details/gtszlsoht.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.hesvh.cn/Article/details/gkaiiwmnn.sHtML

public function __construct(private int $id) {}
来源：http://3g.hesvh.cn/Article/details/givyldndc.sHtML

[U51] PHP：数组解构
来源：http://m.share.fehbvm.com/Article/details/gicexxkik.sHtML

[$a, $b] = $arr;
来源：http://3g.zdbjq.cn/Article/details/gcfmwsljx.sHtML

[U52] PHP：箭头函数
来源：http://mobile.fehbvm.com/Article/details/gfslspgmi.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.hesvh.cn/Article/details/gebtjcysc.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.hesvh.cn/Article/details/gvlcybwfs.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.hesvh.cn/Article/details/ghykrvbrl.sHtML

[U54] PHP：空安全调用
来源：http://mobile.hesvh.cn/Article/details/grjuxefxz.sHtML

$obj?->method()
来源：http://www.m.share.fehbvm.com/Article/details/gggmhphfa.sHtML

[U55] PHP：match 表达式
来源：http://3g.fehbvm.com/Article/details/gxbuptiqc.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.fehbvm.com/Article/details/gdqsjzcox.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.fehbvm.com/Article/details/gdkaelkdr.sHtML

f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/gripgauek.sHtML

[U57] PHP：字符串插值
来源：http://blog.fehbvm.com/Article/details/gjsblxnjh.sHtML

"值: {$a}"
来源：http://m.share.fehbvm.com/Article/details/giugautli.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.zdbjq.cn/Article/details/graevyfot.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.hesvh.cn/Article/details/gunerlfvv.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.fehbvm.com/Article/details/gftchdfzq.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fehbvm.com/Article/details/glodcazgq.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.hesvh.cn/Article/details/gxjzjzjsw.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.zdbjq.cn/Article/details/gqgxztyat.sHtML

[U61] PHP：正则
来源：http://3g.hesvh.cn/Article/details/gsljkgvoq.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.hesvh.cn/Article/details/gihujgkco.sHtML

[U62] PHP：日期对象
来源：http://wap.hesvh.cn/Article/details/gixqyrncn.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.zdbjq.cn/Article/details/giegtplyo.sHtML

[U63] PHP：文件读写
来源：http://www.share.zdbjq.cn/Article/details/gzauwpqpy.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.fehbvm.com/Article/details/glgoarjce.sHtML

[U64] PHP：目录遍历
来源：http://mobile.hesvh.cn/Article/details/gfpusgaeq.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.fehbvm.com/Article/details/gjwicznpn.sHtML

[U65] PHP：会话
来源：http://www.blog.hesvh.cn/Article/details/gldyvxtwx.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gweyevefz.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.fehbvm.com/Article/details/gwkofkshk.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.zdbjq.cn/Article/details/gnqzgrmdz.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.zdbjq.cn/Article/details/gpezlkend.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.fehbvm.com/Article/details/giwpdodks.sHtML

[U68] PHP：PDO 连接
来源：http://3g.hesvh.cn/Article/details/gdlvxlwtc.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.hesvh.cn/Article/details/ghnustkpt.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.zdbjq.cn/Article/details/gxevousph.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.zdbjq.cn/Article/details/gvhdniozo.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.hesvh.cn/Article/details/gfidnuobq.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.hesvh.cn/Article/details/gaaqdhbth.sHtML

[U71] PHP：抛出异常
来源：http://mobile.hesvh.cn/Article/details/ggrtyvsvy.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.zdbjq.cn/Article/details/gpezqnfls.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.hesvh.cn/Article/details/gruidfidh.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.zdbjq.cn/Article/details/gfazgodev.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.hesvh.cn/Article/details/gxkucgqjm.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.hesvh.cn/Article/details/gdhoqgjud.sHtML

[U74] PHP：读取环境变量
来源：http://wap.hesvh.cn/Article/details/glqvjcaeq.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.zdbjq.cn/Article/details/gamdfyroo.sHtML

[U75] PHP：依赖注入
来源：http://baike.zdbjq.cn/Article/details/guoahljhh.sHtML

composer require psr/container
来源：http://m.share.zdbjq.cn/Article/details/gdiczxnvy.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.zdbjq.cn/Article/details/gfgngzruw.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.hesvh.cn/Article/details/gcawhzsqt.sHtML

[U77] PHP：模板渲染
来源：http://m.share.fehbvm.com/Article/details/gexcyfhhw.sHtML

composer require twig/twig
来源：http://baike.zdbjq.cn/Article/details/gcbfiysiv.sHtML

[U78] PHP：单元测试
来源：http://mobile.fehbvm.com/Article/details/glofujnbp.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.zdbjq.cn/Article/details/gwmajrzte.sHtML

[U79] PHP：静态分析
来源：http://mobile.zdbjq.cn/Article/details/ggiduwwjx.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.zdbjq.cn/Article/details/gjtmfhrrf.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.zdbjq.cn/Article/details/gqtmifbro.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.fehbvm.com/Article/details/gaoysqqem.sHtML

[U81] JS：初始化项目
来源：http://m.share.zdbjq.cn/Article/details/gouornrsy.sHtML

npm init -y;  npm i express
来源：http://3g.fehbvm.com/Article/details/gbjdivwrh.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.hesvh.cn/Article/details/gfkkzzefx.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.fehbvm.com/Article/details/gsahrgycf.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.hesvh.cn/Article/details/gfruplsai.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.hesvh.cn/Article/details/gnwrdchsh.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.hesvh.cn/Article/details/gejakynis.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.zdbjq.cn/Article/details/gxbhkheii.sHtML

[U85] JS：可选链
来源：http://www.share.fehbvm.com/Article/details/gtgapojqf.sHtML

a?.b?.c
来源：http://3g.hesvh.cn/Article/details/gisagdxzx.sHtML

[U86] JS：空值合并
来源：http://3g.zdbjq.cn/Article/details/ggadayowo.sHtML

a ?? b
来源：http://wap.zdbjq.cn/Article/details/gffsbdcdw.sHtML

[U87] JS：解构默认值
来源：http://www.share.fehbvm.com/Article/details/gtldwervh.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.zdbjq.cn/Article/details/gxlffirev.sHtML

[U88] JS：对象展开合并
来源：http://www.share.hesvh.cn/Article/details/gvztcgqxe.sHtML

{ ...a, ...b }
来源：http://wap.zdbjq.cn/Article/details/glmqdstls.sHtML

[U89] JS：数组去重
来源：http://mobile.fehbvm.com/Article/details/gevmcsuht.sHtML

[...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/grpgjluzm.sHtML

[U90] JS：数字数组排序
来源：http://www.share.zdbjq.cn/Article/details/giuqespnv.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gsnamsrmx.sHtML

[U91] JS：对象键值遍历
来源：http://blog.zdbjq.cn/Article/details/gqbsqivku.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.fehbvm.com/Article/details/gowbjbsmf.sHtML

[U92] JS：深拷贝
来源：http://baike.hesvh.cn/Article/details/gvqryljee.sHtML

structuredClone(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gejdocqlm.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.fehbvm.com/Article/details/ghnqywlwv.sHtML

`共 ${n} 条`
来源：http://mobile.hesvh.cn/Article/details/ggihzgugy.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.hesvh.cn/Article/details/ggqvtqsdz.sHtML

const double = x => x * 2;
来源：http://www.blog.hesvh.cn/Article/details/gzsoytsxt.sHtML

[U95] JS：Promise 包装
来源：http://read.share.hesvh.cn/Article/details/gijjdvpna.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.fehbvm.com/Article/details/gnrviizhz.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.fehbvm.com/Article/details/gkkxraijz.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/gojaiyjvw.sHtML

[U97] JS：并发请求
来源：http://www.share.zdbjq.cn/Article/details/gpohfjijn.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/gbsjtulrc.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.hesvh.cn/Article/details/gsuexxxcm.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.hesvh.cn/Article/details/grlsudjyp.sHtML

[U99] JS：事件监听
来源：http://www.m.share.zdbjq.cn/Article/details/gitygcdah.sHtML

el.addEventListener("click", e => {})
来源：http://wap.zdbjq.cn/Article/details/ghiaiwnuh.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.hesvh.cn/Article/details/getggdfir.sHtML

document.querySelector(".item")
来源：http://baike.hesvh.cn/Article/details/gzxagqqxs.sHtML

[U101] JS：classList 操作
来源：http://www.share.hesvh.cn/Article/details/gogsdtlcq.sHtML

el.classList.toggle("active")
来源：http://m.share.hesvh.cn/Article/details/gchkozmmc.sHtML

[U102] JS：本地存储
来源：http://mobile.zdbjq.cn/Article/details/gggtqjwio.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.zdbjq.cn/Article/details/goiyiiufz.sHtML

[U103] JS：定时器
来源：http://baike.zdbjq.cn/Article/details/gvfmsjqqp.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.zdbjq.cn/Article/details/gbtspwouj.sHtML

[U104] JS：防抖
来源：http://blog.hesvh.cn/Article/details/gyvuucdfo.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gaxloijno.sHtML

[U105] JS：节流
来源：http://3g.fehbvm.com/Article/details/gdkjkamqi.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.fehbvm.com/Article/details/ggsehlsaz.sHtML

[U106] JS：日期格式化
来源：http://mobile.fehbvm.com/Article/details/gwsdpkqma.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.hesvh.cn/Article/details/glzjbmvvv.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.zdbjq.cn/Article/details/gliwzunug.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.zdbjq.cn/Article/details/gfslxiuyv.sHtML

[U108] JS：随机整数
来源：http://blog.zdbjq.cn/Article/details/gtnfbprwh.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.hesvh.cn/Article/details/gaifjvfca.sHtML

[U109] JS：数组分组
来源：http://wap.zdbjq.cn/Article/details/gxokdllmf.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.zdbjq.cn/Article/details/gqrxxbryz.sHtML

[U110] JS：数组分块
来源：http://baike.hesvh.cn/Article/details/gedbtenuk.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.fehbvm.com/Article/details/gugkfczba.sHtML

[U111] JS：对象转 Map
来源：http://blog.zdbjq.cn/Article/details/gxsdvuode.sHtML

new Map(Object.entries(obj))
来源：http://baike.fehbvm.com/Article/details/gtiysrdje.sHtML

[U112] JS：字符串补位
来源：http://blog.fehbvm.com/Article/details/gmgrpdgif.sHtML

"7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gvplkcmpi.sHtML

[U113] JS：正则替换全部
来源：http://baike.hesvh.cn/Article/details/gdvkvtjzr.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gtgrzfezw.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.zdbjq.cn/Article/details/geqypdhsl.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fehbvm.com/Article/details/goowjchju.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.fehbvm.com/Article/details/grwdarniz.sHtML

crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/gkdunlsap.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.fehbvm.com/Article/details/gqwlpkwcx.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.fehbvm.com/Article/details/gphgbwedz.sHtML

[U117] JS：单元测试
来源：http://blog.hesvh.cn/Article/details/glgghpqyp.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.zdbjq.cn/Article/details/geenbvvvz.sHtML

[U118] JS：开发服务器
来源：http://www.share.fehbvm.com/Article/details/gaowwoagu.sHtML

npm i -D vite;  npx vite
来源：http://blog.zdbjq.cn/Article/details/gzhdtjhxa.sHtML

[U119] JS：生产构建
来源：http://mobile.fehbvm.com/Article/details/gyofnxutz.sHtML

npx vite build
来源：http://baike.hesvh.cn/Article/details/gpagpwcqg.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.zdbjq.cn/Article/details/glsbqxkee.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.zdbjq.cn/Article/details/gwnhnhryh.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gebcjbnih.sHtML

统计汇总
来源：http://www.share.fehbvm.com/Article/details/gmncdtvmp.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gkqntxweg.sHtML

按语言统计（条）：
来源：http://3g.zdbjq.cn/Article/details/gscvvqvwt.sHtML

Python ......... 252
来源：http://m.share.fehbvm.com/Article/details/gthqpqvxc.sHtML

PHP ............ 252
来源：http://read.share.fehbvm.com/Article/details/ghytcmuef.sHtML

JavaScript ..... 252
来源：http://baike.fehbvm.com/Article/details/gesubbyot.sHtML

TypeScript ..... 212
来源：http://read.share.hesvh.cn/Article/details/gkepfxoor.sHtML

Java ........... 212
来源：http://3g.zdbjq.cn/Article/details/gqhyvfmtj.sHtML

Go ............. 212
来源：http://www.m.share.zdbjq.cn/Article/details/gsxgnpxlq.sHtML

Ruby ........... 212
来源：http://baike.fehbvm.com/Article/details/gjgrcswii.sHtML

C# ............. 212
来源：http://www.share.hesvh.cn/Article/details/gfktpjvis.sHtML

C .............. 30
来源：http://baike.hesvh.cn/Article/details/gwhnkwbux.sHtML

C++ ............ 30
来源：http://3g.hesvh.cn/Article/details/gypsnyfof.sHtML

SQL ............ 90
来源：http://baike.zdbjq.cn/Article/details/gfacnljjt.sHtML

Bash ........... 80
来源：http://www.m.share.zdbjq.cn/Article/details/gdwihnsry.sHtML

Kotlin ......... 15
来源：http://www.m.share.zdbjq.cn/Article/details/gmaanbikm.sHtML

Swift .......... 15
来源：http://blog.hesvh.cn/Article/details/gshffzpox.sHtML

Lua ............ 10
来源：http://blog.zdbjq.cn/Article/details/goahzxsxl.sHtML

Perl ........... 10
来源：http://m.share.fehbvm.com/Article/details/gkntxuzht.sHtML

Scala .......... 10
来源：http://baike.fehbvm.com/Article/details/gsdbhrxdp.sHtML

------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gcgyksxbi.sHtML

合计 ........... 2106 条
来源：http://www.blog.hesvh.cn/Article/details/gycgiszre.sHtML

按章节统计：
来源：http://www.m.share.hesvh.cn/Article/details/gwoelrzud.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.fehbvm.com/Article/details/gkeibvupa.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.fehbvm.com/Article/details/gkswxrweg.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.hesvh.cn/Article/details/gmgdfixht.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.fehbvm.com/Article/details/gymprqign.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.zdbjq.cn/Article/details/gemdxwuoz.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.zdbjq.cn/Article/details/gtoezqrbd.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/gdxlvopoj.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.zdbjq.cn/Article/details/grfituiml.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gyyhfjblh.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.fehbvm.com/Article/details/gtghjhcaf.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gjhyhgxyq.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gawvfmzbt.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gqlruiofr.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.zdbjq.cn/Article/details/ghylxetln.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.hesvh.cn/Article/details/gxhxgkhqr.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gysumndcn.sHtML

Q SQL 专题                              90
来源：http://mobile.fehbvm.com/Article/details/gpzwshkhp.sHtML

R Bash 专题                             80
来源：http://blog.zdbjq.cn/Article/details/ggnqguwjm.sHtML

S C / C++ 专题                          60
来源：http://wap.fehbvm.com/Article/details/gbmcxwyzd.sHtML

T 其他语言补充                          60
来源：http://www.share.zdbjq.cn/Article/details/ggdrvnmyl.sHtML

U 高频实用片段                         120
来源：http://3g.hesvh.cn/Article/details/gdlbldivf.sHtML

------------------------------------
来源：http://wap.fehbvm.com/Article/details/gskgcqdgg.sHtML

合计                                  2106 条
来源：http://mobile.fehbvm.com/Article/details/gctxqdsft.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gbqdsveng.sHtML


<!-- 参考信息 -->