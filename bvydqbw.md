代发 wailian999

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.fehbvm.com/Article/details/gsxjekhbf.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gqopkghwk.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.fehbvm.com/Article/details/gnadmotyn.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gtonzxcjt.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.hesvh.cn/Article/details/gtsbhbgbt.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.zdbjq.cn/Article/details/guvjxsyug.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.hesvh.cn/Article/details/gwwyaezsq.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.hesvh.cn/Article/details/glwmwirpl.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.hesvh.cn/Article/details/gbkieowsp.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.fehbvm.com/Article/details/gyjnpojai.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.fehbvm.com/Article/details/gzongvmyd.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.hesvh.cn/Article/details/guzpuladx.sHtML

[U05] Py：列表去重且保序
来源：http://wap.zdbjq.cn/Article/details/gswexflmn.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.fehbvm.com/Article/details/gabsflhsz.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.hesvh.cn/Article/details/gkenuuzgv.sHtML

{**a, **b}
来源：http://m.share.hesvh.cn/Article/details/gjlkkuliw.sHtML

[U07] Py：反转字典键值
来源：http://mobile.fehbvm.com/Article/details/gsrrfccrg.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.hesvh.cn/Article/details/gtvdsgeqh.sHtML

[U08] Py：展平二维列表
来源：http://mobile.fehbvm.com/Article/details/gkwtfvykd.sHtML

[y for x in nested for y in x]
来源：http://www.share.fehbvm.com/Article/details/gpcqbtdjr.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.hesvh.cn/Article/details/gvomzqhur.sHtML

max(d, key=d.get)
来源：http://3g.zdbjq.cn/Article/details/gbehrlrcg.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.zdbjq.cn/Article/details/gxnumjrmj.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.zdbjq.cn/Article/details/gportrwnj.sHtML

[U11] Py：生成器表达式
来源：http://wap.hesvh.cn/Article/details/gxuyrwlys.sHtML

(x * 2 for x in arr)
来源：http://read.share.fehbvm.com/Article/details/gpfeyrevv.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.zdbjq.cn/Article/details/gkpqpshir.sHtML

Counter(arr).most_common(3)
来源：http://m.share.fehbvm.com/Article/details/gvyikjxrw.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.fehbvm.com/Article/details/gtmnibium.sHtML

deque(maxlen=10)
来源：http://wap.hesvh.cn/Article/details/gxvusgytf.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.hesvh.cn/Article/details/gxhhnyxay.sHtML

defaultdict(list)
来源：http://m.share.fehbvm.com/Article/details/gzpmyjwve.sHtML

[U15] Py：高精度计时
来源：http://www.share.zdbjq.cn/Article/details/gwnndooqs.sHtML

t = time.perf_counter()
来源：http://m.share.zdbjq.cn/Article/details/gajnlyvza.sHtML

[U16] Py：命令行参数解析
来源：http://wap.zdbjq.cn/Article/details/gmyserdwa.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.fehbvm.com/Article/details/gzgggwvgn.sHtML

[U17] Py：初始化日志
来源：http://www.share.fehbvm.com/Article/details/ggvnwehey.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.hesvh.cn/Article/details/gafjvfnfu.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fehbvm.com/Article/details/gkfhztiqt.sHtML

pat = re.compile(r"\d+")
来源：http://blog.fehbvm.com/Article/details/ghxvancqn.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.zdbjq.cn/Article/details/gvbkvsgvr.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.zdbjq.cn/Article/details/gfawmqgik.sHtML

[U20] Py：缓存函数结果
来源：http://baike.hesvh.cn/Article/details/gqvemvfns.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.fehbvm.com/Article/details/gbecdighu.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.hesvh.cn/Article/details/ghcnztyia.sHtML

@contextlib.contextmanager
来源：http://www.m.share.hesvh.cn/Article/details/gjtnczovn.sHtML

[U22] Py：矩阵转置
来源：http://wap.zdbjq.cn/Article/details/gfinmjbya.sHtML

list(zip(*m))
来源：http://read.share.hesvh.cn/Article/details/gdnmtlobe.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.fehbvm.com/Article/details/gvzvdjcft.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.zdbjq.cn/Article/details/gvtbpwfne.sHtML

[U24] Py：路径操作
来源：http://www.share.fehbvm.com/Article/details/gwfjrnwct.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.hesvh.cn/Article/details/gpvykzfcg.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.zdbjq.cn/Article/details/gdtzddxph.sHtML

csv.DictReader(f)
来源：http://3g.fehbvm.com/Article/details/gwgqjhqws.sHtML

[U26] Py：并发下载
来源：http://www.share.hesvh.cn/Article/details/gvlkxxequ.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.fehbvm.com/Article/details/gidbcqryr.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.hesvh.cn/Article/details/glfajxvha.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.zdbjq.cn/Article/details/gvfzywpla.sHtML

[U28] Py：类型别名
来源：http://m.share.hesvh.cn/Article/details/gvahwwwrn.sHtML

UserId = int
来源：http://3g.fehbvm.com/Article/details/gsxscsswl.sHtML

[U29] Py：属性校验
来源：http://blog.zdbjq.cn/Article/details/ghshliyvo.sHtML

@property 与 @x.setter 配合
来源：http://m.share.zdbjq.cn/Article/details/gwatjhefg.sHtML

[U30] Py：数据类
来源：http://baike.fehbvm.com/Article/details/gjkvglwnq.sHtML

@dataclass(slots=True)
来源：http://baike.fehbvm.com/Article/details/ghztcolzn.sHtML

[U31] Py：单测
来源：http://blog.fehbvm.com/Article/details/gonuzjgxq.sHtML

python -m pytest -q
来源：http://www.share.hesvh.cn/Article/details/ggudsskga.sHtML

[U32] Py：代码格式化
来源：http://blog.hesvh.cn/Article/details/gjhxhueam.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.zdbjq.cn/Article/details/gexmrhhbs.sHtML

[U33] Py：打包发布
来源：http://baike.hesvh.cn/Article/details/guxzoksru.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.hesvh.cn/Article/details/gntcnqdff.sHtML

[U34] Py：判断编码
来源：http://read.share.fehbvm.com/Article/details/gnryxwvds.sHtML

chardet.detect(raw)
来源：http://mobile.hesvh.cn/Article/details/geozkxzpp.sHtML

[U35] Py：发送邮件
来源：http://3g.fehbvm.com/Article/details/gyqzskulg.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.zdbjq.cn/Article/details/gtqyfbhmo.sHtML

[U36] Py：定时任务
来源：http://www.blog.fehbvm.com/Article/details/gtolrazhp.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.hesvh.cn/Article/details/golfaslml.sHtML

[U37] Py：读写 Excel
来源：http://www.share.fehbvm.com/Article/details/gdowbphvq.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.fehbvm.com/Article/details/gayfbmaij.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fehbvm.com/Article/details/gucfccqvz.sHtML

Path(__file__).resolve().parent
来源：http://blog.hesvh.cn/Article/details/gfdnitlvw.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.hesvh.cn/Article/details/gdmfbkiyf.sHtML

sys.stdout.isatty()
来源：http://www.m.share.zdbjq.cn/Article/details/gvfvstqxf.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.zdbjq.cn/Article/details/gbppgmtmg.sHtML

print("err", file=sys.stderr)
来源：http://wap.hesvh.cn/Article/details/ghgkmcghr.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.hesvh.cn/Article/details/gayqcaivp.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.hesvh.cn/Article/details/grcfljlos.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.zdbjq.cn/Article/details/gichhctfx.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.fehbvm.com/Article/details/gmzorsgkl.sHtML

[U43] PHP：声明命名空间
来源：http://baike.hesvh.cn/Article/details/gvcaebawi.sHtML

namespace App\Http;
来源：http://mobile.zdbjq.cn/Article/details/gvxldnaeu.sHtML

[U44] PHP：开启严格类型
来源：http://3g.fehbvm.com/Article/details/gptzhdunv.sHtML

declare(strict_types=1);
来源：http://www.blog.hesvh.cn/Article/details/gjrzusthh.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.zdbjq.cn/Article/details/gqwvtcpga.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gkpjnjlrb.sHtML

[U46] PHP：可空类型
来源：http://3g.zdbjq.cn/Article/details/gxwtusfba.sHtML

?string $name = null
来源：http://read.share.fehbvm.com/Article/details/goaesxrtl.sHtML

[U47] PHP：联合类型
来源：http://mobile.hesvh.cn/Article/details/gtiryqfdl.sHtML

int|string $id
来源：http://read.share.zdbjq.cn/Article/details/gfqyljaqw.sHtML

[U48] PHP：纯枚举
来源：http://3g.zdbjq.cn/Article/details/gdwlrvgbo.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.hesvh.cn/Article/details/gaylpmxuh.sHtML

[U49] PHP：只读属性
来源：http://mobile.fehbvm.com/Article/details/golxpqrpa.sHtML

public readonly string $name
来源：http://3g.hesvh.cn/Article/details/ghddtvbwk.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.fehbvm.com/Article/details/gvknitinx.sHtML

public function __construct(private int $id) {}
来源：http://baike.fehbvm.com/Article/details/gtpprqicm.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.fehbvm.com/Article/details/gylkzkdci.sHtML

[$a, $b] = $arr;
来源：http://3g.hesvh.cn/Article/details/gsygdebit.sHtML

[U52] PHP：箭头函数
来源：http://blog.hesvh.cn/Article/details/gpfwfhrth.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.zdbjq.cn/Article/details/gnomjzstf.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.hesvh.cn/Article/details/gnhjpsyhb.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.zdbjq.cn/Article/details/gxmocqiuf.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.hesvh.cn/Article/details/gtlfpnulr.sHtML

$obj?->method()
来源：http://wap.zdbjq.cn/Article/details/gedlhuqed.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.hesvh.cn/Article/details/gqmbsxqyt.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.fehbvm.com/Article/details/gnztagkwz.sHtML

[U56] PHP：命名参数
来源：http://www.blog.hesvh.cn/Article/details/gwmmodbvr.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gzkkmwfja.sHtML

[U57] PHP：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gccinhpfe.sHtML

"值: {$a}"
来源：http://www.m.share.hesvh.cn/Article/details/gadcsqlyx.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.fehbvm.com/Article/details/gfbzcapxf.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.hesvh.cn/Article/details/grzoelfya.sHtML

[U59] PHP：自定义排序
来源：http://mobile.zdbjq.cn/Article/details/ghhecmkxx.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fehbvm.com/Article/details/gawzmalic.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.zdbjq.cn/Article/details/ggvugxqwv.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.hesvh.cn/Article/details/ghbfxgkdf.sHtML

[U61] PHP：正则
来源：http://mobile.hesvh.cn/Article/details/gwewfwpqo.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.hesvh.cn/Article/details/ghidhcvvz.sHtML

[U62] PHP：日期对象
来源：http://blog.hesvh.cn/Article/details/gnwceqcvr.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.zdbjq.cn/Article/details/gnjkvwbth.sHtML

[U63] PHP：文件读写
来源：http://www.blog.zdbjq.cn/Article/details/grhzdjdxw.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.hesvh.cn/Article/details/gmqrcbqqn.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.fehbvm.com/Article/details/gyaqttlzv.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.fehbvm.com/Article/details/gkajdweck.sHtML

[U65] PHP：会话
来源：http://m.share.zdbjq.cn/Article/details/gdyxfyxdd.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gppjfhein.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.zdbjq.cn/Article/details/gawdvrgrc.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.fehbvm.com/Article/details/gyxvyjykq.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.fehbvm.com/Article/details/gkyoosxts.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.zdbjq.cn/Article/details/ggxyhlsat.sHtML

[U68] PHP：PDO 连接
来源：http://baike.hesvh.cn/Article/details/geuazbjvg.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.fehbvm.com/Article/details/geuvbuely.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.hesvh.cn/Article/details/gqxogquzx.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.hesvh.cn/Article/details/gmuvurtxt.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.zdbjq.cn/Article/details/gmdiihmtf.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.fehbvm.com/Article/details/gnsqtogab.sHtML

[U71] PHP：抛出异常
来源：http://read.share.zdbjq.cn/Article/details/gwfqylckj.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.fehbvm.com/Article/details/gyfxvzqzh.sHtML

[U72] PHP：写错误日志
来源：http://read.share.zdbjq.cn/Article/details/gosypzgua.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.fehbvm.com/Article/details/gkmfczxek.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.zdbjq.cn/Article/details/gzpvhcvfj.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.hesvh.cn/Article/details/gpmcjdtvv.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.fehbvm.com/Article/details/gteouxwfj.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.hesvh.cn/Article/details/gituepibb.sHtML

[U75] PHP：依赖注入
来源：http://m.share.hesvh.cn/Article/details/gwbfplhgv.sHtML

composer require psr/container
来源：http://www.blog.fehbvm.com/Article/details/gvvyjdexu.sHtML

[U76] PHP：简单路由
来源：http://www.blog.fehbvm.com/Article/details/gddpwshfp.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.zdbjq.cn/Article/details/gqauqtgtc.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.zdbjq.cn/Article/details/gykrvonnp.sHtML

composer require twig/twig
来源：http://wap.hesvh.cn/Article/details/gfrsqpxmg.sHtML

[U78] PHP：单元测试
来源：http://baike.fehbvm.com/Article/details/glyddksji.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.fehbvm.com/Article/details/gcvkqmkyt.sHtML

[U79] PHP：静态分析
来源：http://3g.hesvh.cn/Article/details/ghlxcvvft.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.zdbjq.cn/Article/details/gzpkothhn.sHtML

[U80] PHP：代码规范修复
来源：http://blog.hesvh.cn/Article/details/grqukrfmi.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.hesvh.cn/Article/details/gfkhhelrg.sHtML

[U81] JS：初始化项目
来源：http://blog.hesvh.cn/Article/details/gxjpecgdu.sHtML

npm init -y;  npm i express
来源：http://baike.zdbjq.cn/Article/details/geivxnvlk.sHtML

[U82] JS：package.json 脚本
来源：http://baike.hesvh.cn/Article/details/gonbgdoed.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.fehbvm.com/Article/details/gfhdzhmgw.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.hesvh.cn/Article/details/gwikaqukl.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.hesvh.cn/Article/details/gqpemagbs.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.fehbvm.com/Article/details/gagsvknzx.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.hesvh.cn/Article/details/gkbvonbuk.sHtML

[U85] JS：可选链
来源：http://read.share.hesvh.cn/Article/details/gpumrdreu.sHtML

a?.b?.c
来源：http://m.share.fehbvm.com/Article/details/gdqoqqobw.sHtML

[U86] JS：空值合并
来源：http://3g.fehbvm.com/Article/details/gusjusrrc.sHtML

a ?? b
来源：http://www.share.hesvh.cn/Article/details/gkcjvhyoj.sHtML

[U87] JS：解构默认值
来源：http://wap.fehbvm.com/Article/details/gwobgaqul.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.hesvh.cn/Article/details/gjtqankuw.sHtML

[U88] JS：对象展开合并
来源：http://m.share.zdbjq.cn/Article/details/gctpuvurd.sHtML

{ ...a, ...b }
来源：http://wap.zdbjq.cn/Article/details/gskabgtda.sHtML

[U89] JS：数组去重
来源：http://www.m.share.zdbjq.cn/Article/details/gfmelirtc.sHtML

[...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/gqgufibmw.sHtML

[U90] JS：数字数组排序
来源：http://wap.zdbjq.cn/Article/details/gsphikcjp.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gpogvgbnp.sHtML

[U91] JS：对象键值遍历
来源：http://3g.fehbvm.com/Article/details/gdijaimot.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.zdbjq.cn/Article/details/gqinryrmt.sHtML

[U92] JS：深拷贝
来源：http://read.share.hesvh.cn/Article/details/gwgetsvar.sHtML

structuredClone(obj)
来源：http://read.share.hesvh.cn/Article/details/gglnvnhae.sHtML

[U93] JS：模板字符串
来源：http://www.blog.zdbjq.cn/Article/details/gkrctvhwz.sHtML

`共 ${n} 条`
来源：http://www.blog.zdbjq.cn/Article/details/glbjasnkz.sHtML

[U94] JS：箭头函数
来源：http://baike.hesvh.cn/Article/details/gldemxpvs.sHtML

const double = x => x * 2;
来源：http://read.share.hesvh.cn/Article/details/gmrhhdriu.sHtML

[U95] JS：Promise 包装
来源：http://m.share.hesvh.cn/Article/details/gkczlogan.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.zdbjq.cn/Article/details/gxtxmnimn.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.zdbjq.cn/Article/details/gdwezfewl.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/gjfmpewxl.sHtML

[U97] JS：并发请求
来源：http://3g.fehbvm.com/Article/details/gdnalnbaw.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gphbrclff.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.fehbvm.com/Article/details/gymzlpxac.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.zdbjq.cn/Article/details/geodpwwss.sHtML

[U99] JS：事件监听
来源：http://www.share.zdbjq.cn/Article/details/gtmvnqmzd.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.fehbvm.com/Article/details/gpzitxmjs.sHtML

[U100] JS：DOM 查询
来源：http://3g.hesvh.cn/Article/details/gctezyrsa.sHtML

document.querySelector(".item")
来源：http://m.share.hesvh.cn/Article/details/gnojwhmiy.sHtML

[U101] JS：classList 操作
来源：http://read.share.fehbvm.com/Article/details/gcxipyjfd.sHtML

el.classList.toggle("active")
来源：http://blog.hesvh.cn/Article/details/gxukgebnc.sHtML

[U102] JS：本地存储
来源：http://www.share.hesvh.cn/Article/details/gxekiiswd.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.zdbjq.cn/Article/details/gkzbfabse.sHtML

[U103] JS：定时器
来源：http://baike.hesvh.cn/Article/details/gjypwnyvu.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.fehbvm.com/Article/details/gypgkckqy.sHtML

[U104] JS：防抖
来源：http://mobile.fehbvm.com/Article/details/gddaovkkk.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/glzblfugd.sHtML

[U105] JS：节流
来源：http://read.share.fehbvm.com/Article/details/gxsnjyyud.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.hesvh.cn/Article/details/gcihckdjg.sHtML

[U106] JS：日期格式化
来源：http://wap.fehbvm.com/Article/details/gapgrtwgv.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.zdbjq.cn/Article/details/girjjekxn.sHtML

[U107] JS：数字千分位
来源：http://baike.hesvh.cn/Article/details/gsuwndqad.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.hesvh.cn/Article/details/gcumberjf.sHtML

[U108] JS：随机整数
来源：http://mobile.fehbvm.com/Article/details/gcxupmgxx.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.hesvh.cn/Article/details/geytnceil.sHtML

[U109] JS：数组分组
来源：http://mobile.fehbvm.com/Article/details/gyeqpynob.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.fehbvm.com/Article/details/ghaveuxud.sHtML

[U110] JS：数组分块
来源：http://www.m.share.hesvh.cn/Article/details/gfgxtjkfu.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.zdbjq.cn/Article/details/gbhhtcnvb.sHtML

[U111] JS：对象转 Map
来源：http://blog.fehbvm.com/Article/details/gfamxqzrd.sHtML

new Map(Object.entries(obj))
来源：http://read.share.hesvh.cn/Article/details/gtmsycurc.sHtML

[U112] JS：字符串补位
来源：http://blog.fehbvm.com/Article/details/gozusobfl.sHtML

"7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/guyeixjmm.sHtML

[U113] JS：正则替换全部
来源：http://m.share.zdbjq.cn/Article/details/gqisxkqfn.sHtML

s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/ghvmntatg.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.zdbjq.cn/Article/details/gtebsanih.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.hesvh.cn/Article/details/gzfgxhndd.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.fehbvm.com/Article/details/gjbnljkkt.sHtML

crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gjxfthxwn.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.hesvh.cn/Article/details/gadhhvxtg.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.fehbvm.com/Article/details/ggeoveloq.sHtML

[U117] JS：单元测试
来源：http://read.share.zdbjq.cn/Article/details/gepdscmzt.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.zdbjq.cn/Article/details/grnqacjyh.sHtML

[U118] JS：开发服务器
来源：http://mobile.fehbvm.com/Article/details/gludmplnp.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.fehbvm.com/Article/details/gttkfnnjv.sHtML

[U119] JS：生产构建
来源：http://www.share.zdbjq.cn/Article/details/gjbdpieet.sHtML

npx vite build
来源：http://mobile.fehbvm.com/Article/details/gikzyrsec.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.zdbjq.cn/Article/details/genbtoivl.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.hesvh.cn/Article/details/gdwzicgae.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/guuormzqm.sHtML

统计汇总
来源：http://www.m.share.zdbjq.cn/Article/details/gjlorptal.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gvqbfxxaw.sHtML

按语言统计（条）：
来源：http://baike.zdbjq.cn/Article/details/ghgqchtzg.sHtML

Python ......... 252
来源：http://blog.fehbvm.com/Article/details/gbtumdwhi.sHtML

PHP ............ 252
来源：http://baike.hesvh.cn/Article/details/gxoaqxskl.sHtML

JavaScript ..... 252
来源：http://www.share.fehbvm.com/Article/details/guzmhntmd.sHtML

TypeScript ..... 212
来源：http://www.share.hesvh.cn/Article/details/golrdffsb.sHtML

Java ........... 212
来源：http://wap.zdbjq.cn/Article/details/gkujcxhbd.sHtML

Go ............. 212
来源：http://3g.fehbvm.com/Article/details/gnoxpenfz.sHtML

Ruby ........... 212
来源：http://m.share.zdbjq.cn/Article/details/gdzzybvqx.sHtML

C# ............. 212
来源：http://read.share.hesvh.cn/Article/details/gxcriyqmm.sHtML

C .............. 30
来源：http://read.share.fehbvm.com/Article/details/ganfzwrro.sHtML

C++ ............ 30
来源：http://3g.fehbvm.com/Article/details/gudnefwur.sHtML

SQL ............ 90
来源：http://3g.hesvh.cn/Article/details/gyhrhmocf.sHtML

Bash ........... 80
来源：http://3g.hesvh.cn/Article/details/gquihhcph.sHtML

Kotlin ......... 15
来源：http://mobile.fehbvm.com/Article/details/geycygxrc.sHtML

Swift .......... 15
来源：http://www.blog.fehbvm.com/Article/details/gspsxesed.sHtML

Lua ............ 10
来源：http://mobile.zdbjq.cn/Article/details/gpbmktbqh.sHtML

Perl ........... 10
来源：http://www.m.share.zdbjq.cn/Article/details/ghzqzyqyf.sHtML

Scala .......... 10
来源：http://read.share.fehbvm.com/Article/details/gnnjesmkv.sHtML

------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gncmzmyhl.sHtML

合计 ........... 2106 条
来源：http://www.m.share.hesvh.cn/Article/details/gemlwnade.sHtML

按章节统计：
来源：http://read.share.fehbvm.com/Article/details/ggfurrmtv.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.hesvh.cn/Article/details/gdocmzdwv.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/gqpehktie.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.hesvh.cn/Article/details/gexwtksxb.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.fehbvm.com/Article/details/gskaakqry.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.zdbjq.cn/Article/details/golztdaki.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.fehbvm.com/Article/details/gthmbnxsy.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.zdbjq.cn/Article/details/gjefbxfsz.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.hesvh.cn/Article/details/gzzpjvldi.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gmshkxdbc.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.fehbvm.com/Article/details/grcrimodx.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gbwxzsbfs.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gyexnnswa.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/goccfpasi.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.zdbjq.cn/Article/details/gemyndcow.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.zdbjq.cn/Article/details/ggfdzwvli.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gxymdstpz.sHtML

Q SQL 专题                              90
来源：http://3g.zdbjq.cn/Article/details/gaycfeddt.sHtML

R Bash 专题                             80
来源：http://read.share.zdbjq.cn/Article/details/gcaqqqloc.sHtML

S C / C++ 专题                          60
来源：http://read.share.fehbvm.com/Article/details/gxlqgqbtr.sHtML

T 其他语言补充                          60
来源：http://www.share.zdbjq.cn/Article/details/gxvbdihbm.sHtML

U 高频实用片段                         120
来源：http://3g.zdbjq.cn/Article/details/gfvmrffjy.sHtML

------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/ggqgnwrul.sHtML

合计                                  2106 条
来源：http://www.m.share.hesvh.cn/Article/details/glzbrjbic.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gcevlgpeg.sHtML

使用提醒
来源：http://mobile.zdbjq.cn/Article/details/gepyxasbc.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gpkjrgzup.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.fehbvm.com/Article/details/gsmdjmunz.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.zdbjq.cn/Article/details/gdjrmxoxc.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.zdbjq.cn/Article/details/gkddrynpe.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.zdbjq.cn/Article/details/ggpiehpig.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.fehbvm.com/Article/details/gpzwsrpvg.sHtML

—— 文件结束 ——
来源：http://mobile.zdbjq.cn/Article/details/gvxxwbhjj.sHtML


<!-- 参考信息 -->