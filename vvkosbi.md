代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fanxiaobao.xyz/Article/details/gifywgzlr.sHtML

[T59] Scala：循环
来源：http://3g.fanxiaobao.xyz/Article/details/gcrygweoo.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.fanxiaobao.xyz/Article/details/gstjozibm.sHtML

[T60] Scala：折叠
来源：http://read.share.fanxiaobao.xyz/Article/details/ghlqjchtq.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpxqxvcgm.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gqqpjpczq.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gmykimpjn.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gachrtcby.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.fanxiaobao.xyz/Article/details/gcumkqcjk.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.fanxiaobao.xyz/Article/details/gxiloxkqo.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.fanxiaobao.xyz/Article/details/gnhkkcvwr.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwyotkqho.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.fanxiaobao.xyz/Article/details/glrgfidhw.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpdsgvhkd.sHtML

[U04] Py：变量调试打印
来源：http://blog.fanxiaobao.xyz/Article/details/geyymfnmo.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.fanxiaobao.xyz/Article/details/gasjpttbr.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.fanxiaobao.xyz/Article/details/gtfhrsrhr.sHtML

list(dict.fromkeys(arr))
来源：http://blog.fanxiaobao.xyz/Article/details/gaybygvsg.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gggzvxxul.sHtML

{**a, **b}
来源：http://blog.fanxiaobao.xyz/Article/details/gigvvrbjt.sHtML

[U07] Py：反转字典键值
来源：http://m.share.fanxiaobao.xyz/Article/details/gegemmqjn.sHtML

{v: k for k, v in d.items()}
来源：http://3g.fanxiaobao.xyz/Article/details/grqcpwaft.sHtML

[U08] Py：展平二维列表
来源：http://wap.fanxiaobao.xyz/Article/details/gvdjuzpzf.sHtML

[y for x in nested for y in x]
来源：http://mobile.fanxiaobao.xyz/Article/details/gmyxwddyq.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.fanxiaobao.xyz/Article/details/goercqwxb.sHtML

max(d, key=d.get)
来源：http://baike.fanxiaobao.xyz/Article/details/giipmpzut.sHtML

[U10] Py：按值排序字典
来源：http://baike.fanxiaobao.xyz/Article/details/gesdfyzuk.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.fanxiaobao.xyz/Article/details/gkvgbifvi.sHtML

[U11] Py：生成器表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gvgfgicyr.sHtML

(x * 2 for x in arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gskkxfbyk.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.fanxiaobao.xyz/Article/details/gmdegxuky.sHtML

Counter(arr).most_common(3)
来源：http://wap.fanxiaobao.xyz/Article/details/gjwirjrlg.sHtML

[U13] Py：固定长度队列
来源：http://read.share.fanxiaobao.xyz/Article/details/gjeothrjl.sHtML

deque(maxlen=10)
来源：http://3g.fanxiaobao.xyz/Article/details/gebchrpcm.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gthgihllp.sHtML

defaultdict(list)
来源：http://blog.fanxiaobao.xyz/Article/details/gwwnpgmht.sHtML

[U15] Py：高精度计时
来源：http://baike.fanxiaobao.xyz/Article/details/gsupxdigo.sHtML

t = time.perf_counter()
来源：http://www.share.fanxiaobao.xyz/Article/details/gwnfvymgg.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.fanxiaobao.xyz/Article/details/gbcpmnobx.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.fanxiaobao.xyz/Article/details/gzxzanres.sHtML

[U17] Py：初始化日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqgkscll.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.fanxiaobao.xyz/Article/details/gfcdagdff.sHtML

[U18] Py：预编译正则
来源：http://wap.fanxiaobao.xyz/Article/details/gqcmgyqet.sHtML

pat = re.compile(r"\d+")
来源：http://3g.fanxiaobao.xyz/Article/details/gshknygcr.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbgdtkeyd.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.fanxiaobao.xyz/Article/details/grjzobtnz.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.fanxiaobao.xyz/Article/details/gcnxzklxn.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.fanxiaobao.xyz/Article/details/gfdpasudi.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.fanxiaobao.xyz/Article/details/gcjugxkte.sHtML

@contextlib.contextmanager
来源：http://baike.fanxiaobao.xyz/Article/details/gjfmpddkr.sHtML

[U22] Py：矩阵转置
来源：http://www.share.fanxiaobao.xyz/Article/details/gkuqazwlk.sHtML

list(zip(*m))
来源：http://3g.fanxiaobao.xyz/Article/details/grtvaqhpf.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gakdueola.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.fanxiaobao.xyz/Article/details/gsbwbptca.sHtML

[U24] Py：路径操作
来源：http://wap.fanxiaobao.xyz/Article/details/gagildgqb.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggmtoktxb.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.fanxiaobao.xyz/Article/details/ghoahqrpr.sHtML

csv.DictReader(f)
来源：http://mobile.fanxiaobao.xyz/Article/details/gixghcjfw.sHtML

[U26] Py：并发下载
来源：http://www.blog.fanxiaobao.xyz/Article/details/gparkgamn.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.fanxiaobao.xyz/Article/details/gpwglzxoe.sHtML

[U27] Py：异步 HTTP
来源：http://blog.fanxiaobao.xyz/Article/details/gbhcbvdwh.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.fanxiaobao.xyz/Article/details/gdzcoqcrx.sHtML

[U28] Py：类型别名
来源：http://3g.fanxiaobao.xyz/Article/details/gssfcdhud.sHtML

UserId = int
来源：http://www.blog.fanxiaobao.xyz/Article/details/grtevqvgz.sHtML

[U29] Py：属性校验
来源：http://wap.fanxiaobao.xyz/Article/details/gqixdpxxi.sHtML

@property 与 @x.setter 配合
来源：http://mobile.fanxiaobao.xyz/Article/details/gggovopnq.sHtML

[U30] Py：数据类
来源：http://3g.fanxiaobao.xyz/Article/details/gzsxvkmht.sHtML

@dataclass(slots=True)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzdlgxgwk.sHtML

[U31] Py：单测
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwiezwohh.sHtML

python -m pytest -q
来源：http://m.share.fanxiaobao.xyz/Article/details/gxquywyci.sHtML

[U32] Py：代码格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gfrojkylm.sHtML

ruff format . && ruff check --fix .
来源：http://baike.fanxiaobao.xyz/Article/details/gxoxohkuq.sHtML

[U33] Py：打包发布
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkkxslihy.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.fanxiaobao.xyz/Article/details/gzksbcxck.sHtML

[U34] Py：判断编码
来源：http://www.share.fanxiaobao.xyz/Article/details/gmbbnylbh.sHtML

chardet.detect(raw)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gblzttiph.sHtML

[U35] Py：发送邮件
来源：http://www.share.fanxiaobao.xyz/Article/details/gtylijcvl.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjpuslxnu.sHtML

[U36] Py：定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gnyuibrjy.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.fanxiaobao.xyz/Article/details/gobpgfrus.sHtML

[U37] Py：读写 Excel
来源：http://m.share.fanxiaobao.xyz/Article/details/gynfhlcfi.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gufnfbpzj.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.fanxiaobao.xyz/Article/details/gopbzceqt.sHtML

Path(__file__).resolve().parent
来源：http://mobile.fanxiaobao.xyz/Article/details/geeitcrsj.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.fanxiaobao.xyz/Article/details/gqbdydjyu.sHtML

sys.stdout.isatty()
来源：http://baike.fanxiaobao.xyz/Article/details/ggmeoqjmn.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gqxwldczf.sHtML

print("err", file=sys.stderr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gudqhqbjz.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giiynsurz.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqkvpxcal.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.fanxiaobao.xyz/Article/details/ghmdfussj.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.fanxiaobao.xyz/Article/details/giuxkanth.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.fanxiaobao.xyz/Article/details/ghgmvdlbl.sHtML

namespace App\Http;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpjjkcsnq.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gncfzhvsy.sHtML

declare(strict_types=1);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvzhdvirh.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.fanxiaobao.xyz/Article/details/gxuzrahns.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gjnbkieie.sHtML

[U46] PHP：可空类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/giiouuuxr.sHtML

?string $name = null
来源：http://mobile.fanxiaobao.xyz/Article/details/ggasirtew.sHtML

[U47] PHP：联合类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gksiaxjtk.sHtML

int|string $id
来源：http://www.share.fanxiaobao.xyz/Article/details/gynivvacu.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghqdujqsn.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gfbrxxqsr.sHtML

[U49] PHP：只读属性
来源：http://mobile.fanxiaobao.xyz/Article/details/gtxfxlhjf.sHtML

public readonly string $name
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvsekvwih.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.fanxiaobao.xyz/Article/details/gmrltaaji.sHtML

public function __construct(private int $id) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/ghuzmauqs.sHtML

[U51] PHP：数组解构
来源：http://wap.fanxiaobao.xyz/Article/details/gxuvhrdvz.sHtML

[$a, $b] = $arr;
来源：http://3g.fanxiaobao.xyz/Article/details/gadzchywq.sHtML

[U52] PHP：箭头函数
来源：http://baike.fanxiaobao.xyz/Article/details/gbsgbyocb.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmluvgotq.sHtML

[U53] PHP：空合并运算符
来源：http://blog.fanxiaobao.xyz/Article/details/gbmjrxbvu.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.fanxiaobao.xyz/Article/details/gnpgsgojg.sHtML

[U54] PHP：空安全调用
来源：http://baike.fanxiaobao.xyz/Article/details/gtequonhh.sHtML

$obj?->method()
来源：http://blog.fanxiaobao.xyz/Article/details/gqbdmkubv.sHtML

[U55] PHP：match 表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gtphfyedl.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.fanxiaobao.xyz/Article/details/gsptnkltv.sHtML

[U56] PHP：命名参数
来源：http://blog.fanxiaobao.xyz/Article/details/gftmdlaze.sHtML

f(a: 1, b: 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdfipjffy.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gchdqslmf.sHtML

"值: {$a}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gqhpmmcpm.sHtML

[U58] PHP：数组三件套
来源：http://baike.fanxiaobao.xyz/Article/details/gnzhhccys.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqqyvpsot.sHtML

[U59] PHP：自定义排序
来源：http://3g.fanxiaobao.xyz/Article/details/gzxagtojs.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxkzirbkm.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.fanxiaobao.xyz/Article/details/gmnyerwmh.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.fanxiaobao.xyz/Article/details/gcnvxuwmu.sHtML

[U61] PHP：正则
来源：http://blog.fanxiaobao.xyz/Article/details/gxdeebjlq.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxixeysqu.sHtML

[U62] PHP：日期对象
来源：http://blog.fanxiaobao.xyz/Article/details/gdipfwkxm.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.fanxiaobao.xyz/Article/details/gqltuthyn.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqxhpprto.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghvoxhnvt.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/glgcxcbkq.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.fanxiaobao.xyz/Article/details/gynomioml.sHtML

[U65] PHP：会话
来源：http://www.share.fanxiaobao.xyz/Article/details/gfcqwwmns.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvcpgphag.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.fanxiaobao.xyz/Article/details/gpjhqpepc.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.fanxiaobao.xyz/Article/details/gsrisagdv.sHtML

[U67] PHP：处理文件上传
来源：http://baike.fanxiaobao.xyz/Article/details/gxkvhsalu.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.fanxiaobao.xyz/Article/details/girpkcmrl.sHtML

[U68] PHP：PDO 连接
来源：http://blog.fanxiaobao.xyz/Article/details/gkbfiswvf.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.fanxiaobao.xyz/Article/details/gdycwchdg.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gijtqarar.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.fanxiaobao.xyz/Article/details/gquhwkhpn.sHtML

[U70] PHP：PDO 事务
来源：http://3g.fanxiaobao.xyz/Article/details/gcqxsiwpz.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.fanxiaobao.xyz/Article/details/gszzfyrwb.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqbiycevr.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwoygeqit.sHtML

[U72] PHP：写错误日志
来源：http://3g.fanxiaobao.xyz/Article/details/guqxencxo.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.fanxiaobao.xyz/Article/details/ghdpnuifa.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.fanxiaobao.xyz/Article/details/grsiasgwt.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.fanxiaobao.xyz/Article/details/gazwwyonr.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gyqagubbg.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.fanxiaobao.xyz/Article/details/gwejytqoh.sHtML

[U75] PHP：依赖注入
来源：http://wap.fanxiaobao.xyz/Article/details/gbxfdoqgv.sHtML

composer require psr/container
来源：http://mobile.fanxiaobao.xyz/Article/details/gtrkxjbri.sHtML

[U76] PHP：简单路由
来源：http://mobile.fanxiaobao.xyz/Article/details/gzmtegbub.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzylxznob.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpqblnsgr.sHtML

composer require twig/twig
来源：http://baike.fanxiaobao.xyz/Article/details/gnuucxfhp.sHtML

[U78] PHP：单元测试
来源：http://wap.fanxiaobao.xyz/Article/details/glomekfdl.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.fanxiaobao.xyz/Article/details/gpogwsclt.sHtML

[U79] PHP：静态分析
来源：http://wap.fanxiaobao.xyz/Article/details/gwzhtrkit.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.fanxiaobao.xyz/Article/details/gzmzoqson.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.fanxiaobao.xyz/Article/details/gklkcacrx.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.fanxiaobao.xyz/Article/details/guwexllws.sHtML

[U81] JS：初始化项目
来源：http://www.blog.fanxiaobao.xyz/Article/details/gijapuext.sHtML

npm init -y;  npm i express
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdwywlcmp.sHtML

[U82] JS：package.json 脚本
来源：http://3g.fanxiaobao.xyz/Article/details/gxqklliun.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.fanxiaobao.xyz/Article/details/goopqbfnj.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.fanxiaobao.xyz/Article/details/gwlqvzayu.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.fanxiaobao.xyz/Article/details/goqissriw.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.fanxiaobao.xyz/Article/details/gbdhlgbpi.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.fanxiaobao.xyz/Article/details/gjutvblys.sHtML

[U85] JS：可选链
来源：http://3g.fanxiaobao.xyz/Article/details/gjoxjgrsw.sHtML

a?.b?.c
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbcreegzo.sHtML

[U86] JS：空值合并
来源：http://wap.fanxiaobao.xyz/Article/details/ghxntscjl.sHtML

a ?? b
来源：http://read.share.fanxiaobao.xyz/Article/details/gfqhkgnvq.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfyyaywde.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggyiglmvy.sHtML

[U88] JS：对象展开合并
来源：http://blog.fanxiaobao.xyz/Article/details/gsdcovllp.sHtML

{ ...a, ...b }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggfxeigir.sHtML

[U89] JS：数组去重
来源：http://baike.fanxiaobao.xyz/Article/details/gofdcmuqj.sHtML

[...new Set(arr)]
来源：http://read.share.fanxiaobao.xyz/Article/details/ggapbuvwe.sHtML

[U90] JS：数字数组排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gmwuqpexg.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxiyyeokr.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gznpkhlym.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.fanxiaobao.xyz/Article/details/gekarwbpv.sHtML

[U92] JS：深拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gatdwdswj.sHtML

structuredClone(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcllnboza.sHtML

[U93] JS：模板字符串
来源：http://wap.fanxiaobao.xyz/Article/details/giisiqwcy.sHtML

`共 ${n} 条`
来源：http://baike.fanxiaobao.xyz/Article/details/ghlmpgixo.sHtML

[U94] JS：箭头函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmrrhalcj.sHtML

const double = x => x * 2;
来源：http://mobile.fanxiaobao.xyz/Article/details/goipfuwdl.sHtML

[U95] JS：Promise 包装
来源：http://baike.fanxiaobao.xyz/Article/details/gzxazuvxn.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.fanxiaobao.xyz/Article/details/gvibohsgy.sHtML

[U96] JS：async/await 与异常
来源：http://wap.fanxiaobao.xyz/Article/details/gkxrqwikg.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkmbzqsod.sHtML

[U97] JS：并发请求
来源：http://baike.fanxiaobao.xyz/Article/details/ggdzgxwwn.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fanxiaobao.xyz/Article/details/gasfjnule.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gbbulevgp.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.fanxiaobao.xyz/Article/details/gfsxomjek.sHtML

[U99] JS：事件监听
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnyakoumh.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.fanxiaobao.xyz/Article/details/gwwxhmmms.sHtML

[U100] JS：DOM 查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gaxbxtbzl.sHtML

document.querySelector(".item")
来源：http://www.blog.fanxiaobao.xyz/Article/details/glxxpoqps.sHtML

[U101] JS：classList 操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gmevlfhac.sHtML

el.classList.toggle("active")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggcujbdmg.sHtML

[U102] JS：本地存储
来源：http://baike.fanxiaobao.xyz/Article/details/ghgmbvsrf.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.fanxiaobao.xyz/Article/details/guceqwyzp.sHtML

[U103] JS：定时器
来源：http://mobile.fanxiaobao.xyz/Article/details/gvlqnzsci.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.fanxiaobao.xyz/Article/details/goffqottl.sHtML

[U104] JS：防抖
来源：http://3g.fanxiaobao.xyz/Article/details/gcjqsmzlv.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fanxiaobao.xyz/Article/details/gtmsxzhvf.sHtML

[U105] JS：节流
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glncokhve.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gunvgbeuo.sHtML

[U106] JS：日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gmmwpdtia.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.fanxiaobao.xyz/Article/details/gspuellpj.sHtML

[U107] JS：数字千分位
来源：http://mobile.fanxiaobao.xyz/Article/details/gfhlndovy.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.fanxiaobao.xyz/Article/details/gywzyyjkq.sHtML

[U108] JS：随机整数
来源：http://blog.fanxiaobao.xyz/Article/details/gfmsxsxdj.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.fanxiaobao.xyz/Article/details/glqbmuycb.sHtML

[U109] JS：数组分组
来源：http://3g.fanxiaobao.xyz/Article/details/gtbuqcavd.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.fanxiaobao.xyz/Article/details/grdhckztl.sHtML

[U110] JS：数组分块
来源：http://mobile.fanxiaobao.xyz/Article/details/gxuzfisox.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnztkumxw.sHtML

[U111] JS：对象转 Map
来源：http://baike.fanxiaobao.xyz/Article/details/gyhflsews.sHtML

new Map(Object.entries(obj))
来源：http://www.share.fanxiaobao.xyz/Article/details/gkxnwyuob.sHtML

[U112] JS：字符串补位
来源：http://wap.fanxiaobao.xyz/Article/details/gsbplhgnb.sHtML

"7".padStart(3, "0")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsnpprcsm.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfmbarhwt.sHtML

s.replaceAll("a", "b")
来源：http://blog.fanxiaobao.xyz/Article/details/gohbvddgb.sHtML

[U114] JS：JSON 深比较
来源：http://3g.fanxiaobao.xyz/Article/details/gdyynhmby.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gavyhxbxz.sHtML

[U115] JS：生成 UUID
来源：http://m.share.fanxiaobao.xyz/Article/details/gqgubawyq.sHtML

crypto.randomUUID()
来源：http://baike.fanxiaobao.xyz/Article/details/gzyzfaawu.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.fanxiaobao.xyz/Article/details/guonoghtt.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gdmfgsztq.sHtML

[U117] JS：单元测试
来源：http://www.share.fanxiaobao.xyz/Article/details/gxvhkozxw.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.fanxiaobao.xyz/Article/details/goomcuxel.sHtML

[U118] JS：开发服务器
来源：http://baike.fanxiaobao.xyz/Article/details/gqrdlbeix.sHtML

npm i -D vite;  npx vite
来源：http://3g.fanxiaobao.xyz/Article/details/gisnxxmca.sHtML

[U119] JS：生产构建
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxiicrsoe.sHtML

npx vite build
来源：http://baike.fanxiaobao.xyz/Article/details/gasfhflmg.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.fanxiaobao.xyz/Article/details/gpidcjgae.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.fanxiaobao.xyz/Article/details/gggfdbhjk.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gahlyxbit.sHtML

统计汇总
来源：http://wap.fanxiaobao.xyz/Article/details/gkarjfizq.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gujovhgss.sHtML

按语言统计（条）：
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpvlzqmok.sHtML

Python ......... 252
来源：http://mobile.fanxiaobao.xyz/Article/details/gmcfccdcx.sHtML

PHP ............ 252
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdofryarl.sHtML

JavaScript ..... 252
来源：http://mobile.fanxiaobao.xyz/Article/details/gdbwyksut.sHtML

TypeScript ..... 212
来源：http://wap.fanxiaobao.xyz/Article/details/gzjlnaxgx.sHtML

Java ........... 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gvqkkmgcj.sHtML

Go ............. 212
来源：http://wap.fanxiaobao.xyz/Article/details/glclalhhs.sHtML

Ruby ........... 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gfflsvnil.sHtML

C# ............. 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gqenstekh.sHtML

C .............. 30
来源：http://www.blog.fanxiaobao.xyz/Article/details/geaagbdup.sHtML

C++ ............ 30
来源：http://m.share.fanxiaobao.xyz/Article/details/gyuzpoydj.sHtML

SQL ............ 90
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfelsqiho.sHtML

Bash ........... 80
来源：http://www.blog.fanxiaobao.xyz/Article/details/gehkrelze.sHtML

Kotlin ......... 15
来源：http://baike.fanxiaobao.xyz/Article/details/gwzkenzwz.sHtML

Swift .......... 15
来源：http://3g.fanxiaobao.xyz/Article/details/gtiqglutw.sHtML

Lua ............ 10
来源：http://wap.fanxiaobao.xyz/Article/details/gjsvoxbdj.sHtML

Perl ........... 10
来源：http://wap.fanxiaobao.xyz/Article/details/guttlcayy.sHtML

Scala .......... 10
来源：http://m.share.fanxiaobao.xyz/Article/details/gugklrtph.sHtML

------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/gdxtqmkwc.sHtML

合计 ........... 2106 条
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grmhweaon.sHtML

按章节统计：
来源：http://www.blog.fanxiaobao.xyz/Article/details/glbfuiwth.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.fanxiaobao.xyz/Article/details/gokleaxdo.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.fanxiaobao.xyz/Article/details/gcqpxskqh.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.fanxiaobao.xyz/Article/details/glpfrqgfv.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.fanxiaobao.xyz/Article/details/glmcklmwm.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.fanxiaobao.xyz/Article/details/grdvzrhgy.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.fanxiaobao.xyz/Article/details/gptpltsig.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.fanxiaobao.xyz/Article/details/gplonzgjo.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggfyyhszl.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/gbuwjvxiz.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdwlpdhuh.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/gilydnljh.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gydammwnl.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/grfuokpxo.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.fanxiaobao.xyz/Article/details/gefsmvvzu.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.fanxiaobao.xyz/Article/details/grtsnmjgw.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gkkikgwpp.sHtML

Q SQL 专题                              90
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcgmkuiyz.sHtML

R Bash 专题                             80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glclvapsu.sHtML

S C / C++ 专题                          60
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfdtrntft.sHtML

T 其他语言补充                          60
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghwmpvtwj.sHtML

U 高频实用片段                         120
来源：http://3g.fanxiaobao.xyz/Article/details/gracalrqo.sHtML

------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/gnnherxsm.sHtML

合计                                  2106 条
来源：http://read.share.fanxiaobao.xyz/Article/details/gtphdrpzm.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/gqxpglfhy.sHtML

使用提醒
来源：http://mobile.fanxiaobao.xyz/Article/details/guvhigrhr.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/gvhqwsugz.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gutcbtlxk.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpvnwtzjl.sHtML


<!-- 参考信息 -->