代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://mobile.zdbjq.cn/Article/details/gynjzzlxj.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fehbvm.com/Article/details/gqconkygx.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.zdbjq.cn/Article/details/gdmrxevgh.sHtML

[T56] Scala：样例类
来源：http://wap.zdbjq.cn/Article/details/gswanesgg.sHtML

case class User(name: String, age: Int)
来源：http://baike.fehbvm.com/Article/details/ghhnnftry.sHtML

[T57] Scala：模式匹配
来源：http://mobile.zdbjq.cn/Article/details/gtnfoxjnc.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.zdbjq.cn/Article/details/giazrseuo.sHtML

[T58] Scala：函数定义
来源：http://m.share.fehbvm.com/Article/details/gktxpartn.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fehbvm.com/Article/details/gbntfcutd.sHtML

[T59] Scala：循环
来源：http://mobile.hesvh.cn/Article/details/gdvedicku.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.zdbjq.cn/Article/details/gpszrtggc.sHtML

[T60] Scala：折叠
来源：http://baike.hesvh.cn/Article/details/gkitnfpnp.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.fehbvm.com/Article/details/ggcvsudom.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ggibstpyf.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.hesvh.cn/Article/details/gpfjiwvpn.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gobqxsfam.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.fehbvm.com/Article/details/gfaampgrf.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.zdbjq.cn/Article/details/gnxnngtvw.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.fehbvm.com/Article/details/gdfhapgwl.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.zdbjq.cn/Article/details/gnuxjpqal.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.zdbjq.cn/Article/details/gmvtigpbl.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.zdbjq.cn/Article/details/gezkhgglx.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.hesvh.cn/Article/details/gmiilmmns.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.hesvh.cn/Article/details/gryiezybx.sHtML

[U05] Py：列表去重且保序
来源：http://3g.zdbjq.cn/Article/details/gxflmunhj.sHtML

list(dict.fromkeys(arr))
来源：http://wap.hesvh.cn/Article/details/guqnjxfxm.sHtML

[U06] Py：合并两个字典
来源：http://read.share.hesvh.cn/Article/details/gtyrvcaef.sHtML

{**a, **b}
来源：http://www.blog.hesvh.cn/Article/details/greidmtut.sHtML

[U07] Py：反转字典键值
来源：http://baike.fehbvm.com/Article/details/gprkessdp.sHtML

{v: k for k, v in d.items()}
来源：http://baike.fehbvm.com/Article/details/ghrkvzduv.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.fehbvm.com/Article/details/giuwirtje.sHtML

[y for x in nested for y in x]
来源：http://mobile.fehbvm.com/Article/details/ghwlylaog.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.fehbvm.com/Article/details/ghpjegrxy.sHtML

max(d, key=d.get)
来源：http://www.blog.fehbvm.com/Article/details/gctgazyqj.sHtML

[U10] Py：按值排序字典
来源：http://blog.hesvh.cn/Article/details/gupourpmh.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.hesvh.cn/Article/details/gyrllneun.sHtML

[U11] Py：生成器表达式
来源：http://m.share.fehbvm.com/Article/details/gwuytocli.sHtML

(x * 2 for x in arr)
来源：http://www.share.fehbvm.com/Article/details/guewhnjtj.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.zdbjq.cn/Article/details/gpbevamyl.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gdlkoyhmi.sHtML

[U13] Py：固定长度队列
来源：http://www.share.hesvh.cn/Article/details/gfwzpwuhq.sHtML

deque(maxlen=10)
来源：http://blog.hesvh.cn/Article/details/glfgykbpa.sHtML

[U14] Py：分组收集到列表
来源：http://3g.zdbjq.cn/Article/details/gggfptmpb.sHtML

defaultdict(list)
来源：http://www.share.hesvh.cn/Article/details/gyxnkzmep.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.zdbjq.cn/Article/details/gkdjnhohe.sHtML

t = time.perf_counter()
来源：http://wap.fehbvm.com/Article/details/goygdthzk.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.hesvh.cn/Article/details/gpaadbigk.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.fehbvm.com/Article/details/gtflxeula.sHtML

[U17] Py：初始化日志
来源：http://wap.zdbjq.cn/Article/details/ghgqukmox.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.zdbjq.cn/Article/details/gcmyjtcjo.sHtML

[U18] Py：预编译正则
来源：http://m.share.fehbvm.com/Article/details/gjblollaj.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.hesvh.cn/Article/details/gzwmfzzcv.sHtML

[U19] Py：正则替换带回调
来源：http://3g.fehbvm.com/Article/details/gmkaixpwr.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.fehbvm.com/Article/details/gnzutnyfr.sHtML

[U20] Py：缓存函数结果
来源：http://baike.fehbvm.com/Article/details/grnnqrzgh.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.zdbjq.cn/Article/details/giudeulww.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.fehbvm.com/Article/details/gvfruqhrn.sHtML

@contextlib.contextmanager
来源：http://mobile.zdbjq.cn/Article/details/gxaqtzjza.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.zdbjq.cn/Article/details/gfmnndboi.sHtML

list(zip(*m))
来源：http://read.share.zdbjq.cn/Article/details/gfyumwcbv.sHtML

[U23] Py：分块读取大文件
来源：http://baike.hesvh.cn/Article/details/gshpxparv.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.fehbvm.com/Article/details/gqpthmcth.sHtML

[U24] Py：路径操作
来源：http://mobile.fehbvm.com/Article/details/gmlsmfwin.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/gcypcrrwl.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.zdbjq.cn/Article/details/gafrhdweu.sHtML

csv.DictReader(f)
来源：http://blog.hesvh.cn/Article/details/glqcnwhbk.sHtML

[U26] Py：并发下载
来源：http://baike.hesvh.cn/Article/details/gsqfqzbfz.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.zdbjq.cn/Article/details/gaerwwwce.sHtML

[U27] Py：异步 HTTP
来源：http://wap.hesvh.cn/Article/details/goyzzeisi.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.fehbvm.com/Article/details/gyhedreev.sHtML

[U28] Py：类型别名
来源：http://blog.fehbvm.com/Article/details/gqtdvskug.sHtML

UserId = int
来源：http://baike.hesvh.cn/Article/details/gzvphmgwl.sHtML

[U29] Py：属性校验
来源：http://3g.fehbvm.com/Article/details/gaxxyanzl.sHtML

@property 与 @x.setter 配合
来源：http://blog.zdbjq.cn/Article/details/gqrypoylo.sHtML

[U30] Py：数据类
来源：http://www.blog.zdbjq.cn/Article/details/gltjabkxp.sHtML

@dataclass(slots=True)
来源：http://blog.fehbvm.com/Article/details/gxxbqzfab.sHtML

[U31] Py：单测
来源：http://read.share.hesvh.cn/Article/details/gwbrbvjpz.sHtML

python -m pytest -q
来源：http://mobile.zdbjq.cn/Article/details/govtsojac.sHtML

[U32] Py：代码格式化
来源：http://baike.zdbjq.cn/Article/details/gcerqbpug.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.fehbvm.com/Article/details/gqjkfvowi.sHtML

[U33] Py：打包发布
来源：http://read.share.hesvh.cn/Article/details/gwtyobeum.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.fehbvm.com/Article/details/gpdrrdmma.sHtML

[U34] Py：判断编码
来源：http://read.share.hesvh.cn/Article/details/gbnabysvj.sHtML

chardet.detect(raw)
来源：http://baike.fehbvm.com/Article/details/gceimgayv.sHtML

[U35] Py：发送邮件
来源：http://blog.hesvh.cn/Article/details/gnqhmuaan.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.zdbjq.cn/Article/details/gvkswmfym.sHtML

[U36] Py：定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/gnrgtadus.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.zdbjq.cn/Article/details/gdyilxipe.sHtML

[U37] Py：读写 Excel
来源：http://m.share.fehbvm.com/Article/details/gygpkjnfv.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.hesvh.cn/Article/details/gttdzgbvx.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fehbvm.com/Article/details/ggabotcra.sHtML

Path(__file__).resolve().parent
来源：http://3g.zdbjq.cn/Article/details/gtaoliegl.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.zdbjq.cn/Article/details/gsssmnqmi.sHtML

sys.stdout.isatty()
来源：http://www.blog.zdbjq.cn/Article/details/gwselxxbh.sHtML

[U40] Py：打印到标准错误
来源：http://wap.fehbvm.com/Article/details/gxvojcndf.sHtML

print("err", file=sys.stderr)
来源：http://mobile.fehbvm.com/Article/details/gkmuxorbl.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.fehbvm.com/Article/details/gdgzvqchw.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.hesvh.cn/Article/details/gjqvtfmic.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.hesvh.cn/Article/details/ghckvijqe.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.zdbjq.cn/Article/details/gaeoekykv.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.zdbjq.cn/Article/details/gfjiipfpa.sHtML

namespace App\Http;
来源：http://www.share.fehbvm.com/Article/details/ghzcqfbwr.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.hesvh.cn/Article/details/gyynmhimm.sHtML

declare(strict_types=1);
来源：http://read.share.zdbjq.cn/Article/details/gqtzkzlyw.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.hesvh.cn/Article/details/gizznljec.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gdvgqswqc.sHtML

[U46] PHP：可空类型
来源：http://www.blog.zdbjq.cn/Article/details/gyetppglf.sHtML

?string $name = null
来源：http://www.blog.zdbjq.cn/Article/details/gedmcabxd.sHtML

[U47] PHP：联合类型
来源：http://www.blog.hesvh.cn/Article/details/gklapldsd.sHtML

int|string $id
来源：http://mobile.hesvh.cn/Article/details/ggndgcxmj.sHtML

[U48] PHP：纯枚举
来源：http://baike.zdbjq.cn/Article/details/ghrdqwucq.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.hesvh.cn/Article/details/gizmxaoro.sHtML

[U49] PHP：只读属性
来源：http://wap.zdbjq.cn/Article/details/gwfefbbjf.sHtML

public readonly string $name
来源：http://3g.hesvh.cn/Article/details/gyayenvau.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.zdbjq.cn/Article/details/ghignxixt.sHtML

public function __construct(private int $id) {}
来源：http://www.share.zdbjq.cn/Article/details/gvonjwpfj.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.zdbjq.cn/Article/details/gegrqbwxh.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.fehbvm.com/Article/details/gbijrklis.sHtML

[U52] PHP：箭头函数
来源：http://3g.fehbvm.com/Article/details/gzhdmvmqb.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.fehbvm.com/Article/details/gibktsppi.sHtML

[U53] PHP：空合并运算符
来源：http://wap.fehbvm.com/Article/details/gxjbcuvqk.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.zdbjq.cn/Article/details/glaksxuwa.sHtML

[U54] PHP：空安全调用
来源：http://read.share.fehbvm.com/Article/details/ghpmiaftr.sHtML

$obj?->method()
来源：http://blog.hesvh.cn/Article/details/gxjvagpss.sHtML

[U55] PHP：match 表达式
来源：http://3g.zdbjq.cn/Article/details/gulzikgfj.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.zdbjq.cn/Article/details/gcwyzcdgb.sHtML

[U56] PHP：命名参数
来源：http://mobile.hesvh.cn/Article/details/gwwjnbzeb.sHtML

f(a: 1, b: 2)
来源：http://baike.zdbjq.cn/Article/details/gwvuqpgtj.sHtML

[U57] PHP：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gjynnoxed.sHtML

"值: {$a}"
来源：http://read.share.zdbjq.cn/Article/details/gccmfhwjf.sHtML

[U58] PHP：数组三件套
来源：http://baike.fehbvm.com/Article/details/grbzkjnfp.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.hesvh.cn/Article/details/gcbdronjp.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.hesvh.cn/Article/details/gnnwvybzp.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.hesvh.cn/Article/details/geedqhhqf.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.hesvh.cn/Article/details/gcypeiazq.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gierupxhh.sHtML

[U61] PHP：正则
来源：http://mobile.fehbvm.com/Article/details/gqjindxce.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.zdbjq.cn/Article/details/gsxwnuric.sHtML

[U62] PHP：日期对象
来源：http://blog.zdbjq.cn/Article/details/gwjgcdkup.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.fehbvm.com/Article/details/ggqwkxjga.sHtML

[U63] PHP：文件读写
来源：http://www.share.zdbjq.cn/Article/details/guycntmga.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.fehbvm.com/Article/details/gfqohxhoz.sHtML

[U64] PHP：目录遍历
来源：http://www.share.fehbvm.com/Article/details/glhhdtgqx.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.zdbjq.cn/Article/details/gbkelelpv.sHtML

[U65] PHP：会话
来源：http://read.share.hesvh.cn/Article/details/gaxhbbxia.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.fehbvm.com/Article/details/gwmkvkxpi.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.fehbvm.com/Article/details/gwmvbsypl.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.fehbvm.com/Article/details/gvlktvadm.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.fehbvm.com/Article/details/gfsxeuenw.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.hesvh.cn/Article/details/gbyjmunon.sHtML

[U68] PHP：PDO 连接
来源：http://blog.zdbjq.cn/Article/details/gfnxwtwoj.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.fehbvm.com/Article/details/gjytezadk.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.zdbjq.cn/Article/details/gpczvofwo.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.fehbvm.com/Article/details/gvcxrmuzf.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.fehbvm.com/Article/details/glbneublb.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.hesvh.cn/Article/details/gvxvwbmul.sHtML

[U71] PHP：抛出异常
来源：http://wap.hesvh.cn/Article/details/gdgmqolrx.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.hesvh.cn/Article/details/gfxeumvcc.sHtML

[U72] PHP：写错误日志
来源：http://blog.hesvh.cn/Article/details/gapkqprpt.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.zdbjq.cn/Article/details/gmjwzxbvx.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.zdbjq.cn/Article/details/ggxpmduwu.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.fehbvm.com/Article/details/ghlickklr.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.zdbjq.cn/Article/details/gzsxprscd.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.hesvh.cn/Article/details/gjqrxergn.sHtML

[U75] PHP：依赖注入
来源：http://3g.zdbjq.cn/Article/details/gurvpnbdp.sHtML

composer require psr/container
来源：http://wap.zdbjq.cn/Article/details/gdsyfyzug.sHtML

[U76] PHP：简单路由
来源：http://www.share.fehbvm.com/Article/details/gqjhegwif.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.fehbvm.com/Article/details/giiwqmbrf.sHtML

[U77] PHP：模板渲染
来源：http://wap.zdbjq.cn/Article/details/grmvextrs.sHtML

composer require twig/twig
来源：http://www.blog.fehbvm.com/Article/details/ggoxfmsto.sHtML

[U78] PHP：单元测试
来源：http://www.share.hesvh.cn/Article/details/gjvgozzlb.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.fehbvm.com/Article/details/gmkxlalwj.sHtML

[U79] PHP：静态分析
来源：http://read.share.zdbjq.cn/Article/details/gwxjoehko.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.hesvh.cn/Article/details/ggbbpjcay.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.zdbjq.cn/Article/details/gocdyaudw.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.fehbvm.com/Article/details/gbtrxlopw.sHtML

[U81] JS：初始化项目
来源：http://www.blog.fehbvm.com/Article/details/gbaprtudj.sHtML

npm init -y;  npm i express
来源：http://www.blog.zdbjq.cn/Article/details/gqxrpboep.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.hesvh.cn/Article/details/glvqdehom.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.fehbvm.com/Article/details/gibbnqvoc.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.hesvh.cn/Article/details/giktrlgqf.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.fehbvm.com/Article/details/gsvwslarp.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.zdbjq.cn/Article/details/gzvamqpbd.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.fehbvm.com/Article/details/gwjoemeza.sHtML

[U85] JS：可选链
来源：http://www.share.fehbvm.com/Article/details/gbwupdxur.sHtML

a?.b?.c
来源：http://www.m.share.hesvh.cn/Article/details/gxneccniy.sHtML

[U86] JS：空值合并
来源：http://www.blog.zdbjq.cn/Article/details/gxbtovtik.sHtML

a ?? b
来源：http://www.blog.zdbjq.cn/Article/details/ggqojtpvd.sHtML

[U87] JS：解构默认值
来源：http://www.blog.zdbjq.cn/Article/details/gsoulscds.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.hesvh.cn/Article/details/gfbxhqprg.sHtML

[U88] JS：对象展开合并
来源：http://baike.fehbvm.com/Article/details/gozouscfc.sHtML

{ ...a, ...b }
来源：http://mobile.zdbjq.cn/Article/details/gpdafloau.sHtML

[U89] JS：数组去重
来源：http://m.share.zdbjq.cn/Article/details/gecrnachc.sHtML

[...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gsaeedrnp.sHtML

[U90] JS：数字数组排序
来源：http://m.share.zdbjq.cn/Article/details/gfekwyuuh.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/ggcfingkk.sHtML

[U91] JS：对象键值遍历
来源：http://wap.fehbvm.com/Article/details/gudwliwnb.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.fehbvm.com/Article/details/gkmmzwzhe.sHtML

[U92] JS：深拷贝
来源：http://www.share.fehbvm.com/Article/details/gnrjvnual.sHtML

structuredClone(obj)
来源：http://wap.fehbvm.com/Article/details/gcbvvqqrq.sHtML

[U93] JS：模板字符串
来源：http://mobile.hesvh.cn/Article/details/gbyzwpwlz.sHtML

`共 ${n} 条`
来源：http://wap.fehbvm.com/Article/details/glqwtnjmt.sHtML

[U94] JS：箭头函数
来源：http://read.share.hesvh.cn/Article/details/gbgxwofpm.sHtML

const double = x => x * 2;
来源：http://baike.zdbjq.cn/Article/details/gtkajyhbf.sHtML

[U95] JS：Promise 包装
来源：http://blog.zdbjq.cn/Article/details/gsovfhdsw.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.hesvh.cn/Article/details/gozetyrvn.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.zdbjq.cn/Article/details/gnbjknhwe.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.zdbjq.cn/Article/details/gokguqjpi.sHtML

[U97] JS：并发请求
来源：http://www.blog.zdbjq.cn/Article/details/gguglceqf.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/gticzbznf.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.fehbvm.com/Article/details/ghvkekrfi.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.fehbvm.com/Article/details/gtsftcsod.sHtML

[U99] JS：事件监听
来源：http://blog.hesvh.cn/Article/details/gqkfarrsz.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.hesvh.cn/Article/details/gaodgxvmv.sHtML

[U100] JS：DOM 查询
来源：http://blog.fehbvm.com/Article/details/gvntvjlyx.sHtML

document.querySelector(".item")
来源：http://m.share.hesvh.cn/Article/details/gnwzhnsyp.sHtML

[U101] JS：classList 操作
来源：http://www.blog.fehbvm.com/Article/details/gasobsypl.sHtML

el.classList.toggle("active")
来源：http://m.share.fehbvm.com/Article/details/gcfiwzfhf.sHtML

[U102] JS：本地存储
来源：http://read.share.zdbjq.cn/Article/details/gkduprgop.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.zdbjq.cn/Article/details/gwrnnuvzk.sHtML

[U103] JS：定时器
来源：http://www.m.share.hesvh.cn/Article/details/gzbcxykbc.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.hesvh.cn/Article/details/giwmgdcor.sHtML

[U104] JS：防抖
来源：http://www.blog.hesvh.cn/Article/details/goxeqhseo.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gtgdgsvel.sHtML

[U105] JS：节流
来源：http://mobile.hesvh.cn/Article/details/gdoicxnmw.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.hesvh.cn/Article/details/gjfmrgmmz.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gnalfwwij.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.fehbvm.com/Article/details/gjnfhajvr.sHtML

[U107] JS：数字千分位
来源：http://mobile.zdbjq.cn/Article/details/ghvgaujvu.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.zdbjq.cn/Article/details/giaofxgfc.sHtML

[U108] JS：随机整数
来源：http://read.share.zdbjq.cn/Article/details/gdauupcjh.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.fehbvm.com/Article/details/gwawrrcia.sHtML

[U109] JS：数组分组
来源：http://3g.fehbvm.com/Article/details/gxkdpccdi.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fehbvm.com/Article/details/grbeivzfp.sHtML

[U110] JS：数组分块
来源：http://read.share.fehbvm.com/Article/details/gnsrhgjeg.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.fehbvm.com/Article/details/geuvnlzpw.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.fehbvm.com/Article/details/gxofhshbg.sHtML

new Map(Object.entries(obj))
来源：http://read.share.fehbvm.com/Article/details/gmgexgcrh.sHtML

[U112] JS：字符串补位
来源：http://blog.fehbvm.com/Article/details/gqszdtiib.sHtML

"7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gxwkcpfhi.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.zdbjq.cn/Article/details/gilzuhnju.sHtML

s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gvfukrbqp.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.fehbvm.com/Article/details/guapfhpfx.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.zdbjq.cn/Article/details/gajmzjphp.sHtML

[U115] JS：生成 UUID
来源：http://read.share.zdbjq.cn/Article/details/gqjgmvizy.sHtML

crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gqtnlogkf.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.fehbvm.com/Article/details/gwxjpyulc.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.fehbvm.com/Article/details/gazfxmpfu.sHtML

[U117] JS：单元测试
来源：http://3g.fehbvm.com/Article/details/gdnxcrllp.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.fehbvm.com/Article/details/gvebwubbd.sHtML

[U118] JS：开发服务器
来源：http://baike.hesvh.cn/Article/details/gbaxpjmsk.sHtML

npm i -D vite;  npx vite
来源：http://m.share.fehbvm.com/Article/details/ghiptmwdq.sHtML

[U119] JS：生产构建
来源：http://blog.zdbjq.cn/Article/details/gkqlkjvfq.sHtML

npx vite build
来源：http://read.share.hesvh.cn/Article/details/gxmwxshmi.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.fehbvm.com/Article/details/gfqxuzlzw.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.zdbjq.cn/Article/details/gigtdzjab.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gmnubwtav.sHtML

统计汇总
来源：http://www.m.share.fehbvm.com/Article/details/gybdhaazi.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gpsrvjnqh.sHtML

按语言统计（条）：
来源：http://www.share.fehbvm.com/Article/details/gjpdcqvpo.sHtML

Python ......... 252
来源：http://www.share.zdbjq.cn/Article/details/gnuxfavmn.sHtML

PHP ............ 252
来源：http://baike.zdbjq.cn/Article/details/gpyhhhnfa.sHtML

JavaScript ..... 252
来源：http://baike.hesvh.cn/Article/details/gwjmntzva.sHtML

TypeScript ..... 212
来源：http://baike.zdbjq.cn/Article/details/gnlriuypw.sHtML

Java ........... 212
来源：http://www.m.share.zdbjq.cn/Article/details/gkuflexhu.sHtML

Go ............. 212
来源：http://read.share.fehbvm.com/Article/details/ggpirvcbu.sHtML

Ruby ........... 212
来源：http://wap.zdbjq.cn/Article/details/gevvhrwgh.sHtML

C# ............. 212
来源：http://blog.zdbjq.cn/Article/details/gonhpyglt.sHtML

C .............. 30
来源：http://read.share.fehbvm.com/Article/details/gnkxwefuf.sHtML

C++ ............ 30
来源：http://3g.fehbvm.com/Article/details/gdfoixpec.sHtML

SQL ............ 90
来源：http://www.blog.fehbvm.com/Article/details/gnrljywae.sHtML

Bash ........... 80
来源：http://www.share.fehbvm.com/Article/details/ghixpfbzr.sHtML

Kotlin ......... 15
来源：http://mobile.fehbvm.com/Article/details/gliacmtes.sHtML

Swift .......... 15
来源：http://baike.zdbjq.cn/Article/details/gxrayfetc.sHtML

Lua ............ 10
来源：http://blog.fehbvm.com/Article/details/gvzqhkyto.sHtML

Perl ........... 10
来源：http://www.m.share.fehbvm.com/Article/details/gmgpncpkm.sHtML

Scala .......... 10
来源：http://3g.fehbvm.com/Article/details/goavlbcre.sHtML

------------------------------------
来源：http://wap.fehbvm.com/Article/details/gpfspnxop.sHtML

合计 ........... 2106 条
来源：http://baike.hesvh.cn/Article/details/gdcplmmhp.sHtML

按章节统计：
来源：http://blog.zdbjq.cn/Article/details/gaysvjdoi.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.fehbvm.com/Article/details/guzavglyv.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.zdbjq.cn/Article/details/gnvnmkrkt.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.zdbjq.cn/Article/details/gcnganeqb.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.zdbjq.cn/Article/details/gpfblxcsh.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.hesvh.cn/Article/details/gqgezxzye.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.fehbvm.com/Article/details/gbapbnddd.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/gnckhilwc.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.hesvh.cn/Article/details/goyedqjke.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gsdpfhony.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.fehbvm.com/Article/details/gtrjyjwii.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/ghrtayywz.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gxlhkzoku.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gcqublvuu.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.hesvh.cn/Article/details/grmlshbex.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.fehbvm.com/Article/details/gimyjhwli.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/glwhyuxzw.sHtML

Q SQL 专题                              90
来源：http://read.share.hesvh.cn/Article/details/grfiwzdel.sHtML

R Bash 专题                             80
来源：http://www.share.zdbjq.cn/Article/details/ggphxkfhp.sHtML

S C / C++ 专题                          60
来源：http://3g.hesvh.cn/Article/details/gxfitjdeq.sHtML

T 其他语言补充                          60
来源：http://baike.hesvh.cn/Article/details/ghywdopuw.sHtML


<!-- 参考信息 -->