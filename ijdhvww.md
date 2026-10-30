代发 wailian999

[U03] Py：加载 .env 配置
来源：http://www.share.zdbjq.cn/Article/details/glsfcaxnb.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.fehbvm.com/Article/details/gyrtndsby.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.fehbvm.com/Article/details/gtabraant.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.hesvh.cn/Article/details/geueapzgq.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.fehbvm.com/Article/details/gghlsoubr.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.zdbjq.cn/Article/details/gqwzwplhb.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.fehbvm.com/Article/details/gnjjfihxb.sHtML

{**a, **b}
来源：http://baike.zdbjq.cn/Article/details/giopzyslm.sHtML

[U07] Py：反转字典键值
来源：http://www.share.zdbjq.cn/Article/details/gfbufdnmu.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.hesvh.cn/Article/details/gwdtcwfxf.sHtML

[U08] Py：展平二维列表
来源：http://wap.fehbvm.com/Article/details/gxdbzpopt.sHtML

[y for x in nested for y in x]
来源：http://read.share.hesvh.cn/Article/details/gwmlpnksg.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.hesvh.cn/Article/details/gwkjlxjli.sHtML

max(d, key=d.get)
来源：http://baike.zdbjq.cn/Article/details/gwdvnuigf.sHtML

[U10] Py：按值排序字典
来源：http://www.share.zdbjq.cn/Article/details/gzljaecnd.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.fehbvm.com/Article/details/glhckpeof.sHtML

[U11] Py：生成器表达式
来源：http://www.share.hesvh.cn/Article/details/gtqyhbpcm.sHtML

(x * 2 for x in arr)
来源：http://read.share.hesvh.cn/Article/details/gyhkhvnqw.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.zdbjq.cn/Article/details/gtedldeeu.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.hesvh.cn/Article/details/gqffycpsf.sHtML

[U13] Py：固定长度队列
来源：http://baike.hesvh.cn/Article/details/gyhfooecq.sHtML

deque(maxlen=10)
来源：http://3g.zdbjq.cn/Article/details/gjnbxzkii.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.zdbjq.cn/Article/details/gcvdyfdcu.sHtML

defaultdict(list)
来源：http://mobile.zdbjq.cn/Article/details/gljkedkaj.sHtML

[U15] Py：高精度计时
来源：http://blog.zdbjq.cn/Article/details/gbnuvnfau.sHtML

t = time.perf_counter()
来源：http://m.share.hesvh.cn/Article/details/gpwfziipg.sHtML

[U16] Py：命令行参数解析
来源：http://3g.fehbvm.com/Article/details/ggmnnmnlk.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.zdbjq.cn/Article/details/gleahszrn.sHtML

[U17] Py：初始化日志
来源：http://www.share.zdbjq.cn/Article/details/gmgfyphnq.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.zdbjq.cn/Article/details/gkllfqrxo.sHtML

[U18] Py：预编译正则
来源：http://wap.fehbvm.com/Article/details/gpytxdils.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.zdbjq.cn/Article/details/ghhaqrphk.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.zdbjq.cn/Article/details/gpbrmhacy.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.zdbjq.cn/Article/details/gddmcmoxv.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.fehbvm.com/Article/details/ghqhbxdac.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.hesvh.cn/Article/details/gmlemgstc.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.zdbjq.cn/Article/details/gckhtygij.sHtML

@contextlib.contextmanager
来源：http://baike.hesvh.cn/Article/details/gnfqrqrns.sHtML

[U22] Py：矩阵转置
来源：http://read.share.fehbvm.com/Article/details/gehmeywah.sHtML

list(zip(*m))
来源：http://3g.hesvh.cn/Article/details/gizrcictr.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.zdbjq.cn/Article/details/grroxzedc.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.hesvh.cn/Article/details/gblrlgsyk.sHtML

[U24] Py：路径操作
来源：http://wap.hesvh.cn/Article/details/gvzbqtnrm.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.fehbvm.com/Article/details/gqjehfaja.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.fehbvm.com/Article/details/gzkeeyskh.sHtML

csv.DictReader(f)
来源：http://www.share.zdbjq.cn/Article/details/gkdrbiubo.sHtML

[U26] Py：并发下载
来源：http://wap.zdbjq.cn/Article/details/ghwryausw.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.zdbjq.cn/Article/details/giebccgpc.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.zdbjq.cn/Article/details/gphhqanwi.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.fehbvm.com/Article/details/gtjqqidpm.sHtML

[U28] Py：类型别名
来源：http://baike.fehbvm.com/Article/details/gssuzfiwo.sHtML

UserId = int
来源：http://wap.fehbvm.com/Article/details/ginioyzeh.sHtML

[U29] Py：属性校验
来源：http://www.share.hesvh.cn/Article/details/gopqqzept.sHtML

@property 与 @x.setter 配合
来源：http://read.share.fehbvm.com/Article/details/gcmwjzhki.sHtML

[U30] Py：数据类
来源：http://wap.hesvh.cn/Article/details/gbxqliwty.sHtML

@dataclass(slots=True)
来源：http://m.share.fehbvm.com/Article/details/gecvhbfuk.sHtML

[U31] Py：单测
来源：http://m.share.hesvh.cn/Article/details/ghxxxxhia.sHtML

python -m pytest -q
来源：http://mobile.zdbjq.cn/Article/details/ghqdrwqjj.sHtML

[U32] Py：代码格式化
来源：http://www.share.zdbjq.cn/Article/details/gisvbveud.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.fehbvm.com/Article/details/gjtsxfdlc.sHtML

[U33] Py：打包发布
来源：http://www.share.hesvh.cn/Article/details/gtugbkbsr.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.zdbjq.cn/Article/details/gnxhhejds.sHtML

[U34] Py：判断编码
来源：http://baike.zdbjq.cn/Article/details/gxzrnfxba.sHtML

chardet.detect(raw)
来源：http://blog.fehbvm.com/Article/details/gqoylslxf.sHtML

[U35] Py：发送邮件
来源：http://www.blog.hesvh.cn/Article/details/gyshmxjbj.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.zdbjq.cn/Article/details/gqsnuygqh.sHtML

[U36] Py：定时任务
来源：http://m.share.zdbjq.cn/Article/details/gfofnouql.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.hesvh.cn/Article/details/gmrpoakvk.sHtML

[U37] Py：读写 Excel
来源：http://baike.fehbvm.com/Article/details/gefbyqqdo.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.zdbjq.cn/Article/details/gwlddtkzd.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.fehbvm.com/Article/details/gqtpjwvlx.sHtML

Path(__file__).resolve().parent
来源：http://www.share.hesvh.cn/Article/details/gmxhqoiel.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.hesvh.cn/Article/details/gvscuamzo.sHtML

sys.stdout.isatty()
来源：http://mobile.hesvh.cn/Article/details/goiboaftz.sHtML

[U40] Py：打印到标准错误
来源：http://3g.hesvh.cn/Article/details/grnkmrzmx.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.zdbjq.cn/Article/details/gifnudtep.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.zdbjq.cn/Article/details/gpwydactm.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.hesvh.cn/Article/details/gdppsybdl.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.fehbvm.com/Article/details/glfkbgiyj.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.fehbvm.com/Article/details/gomkqemwl.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.fehbvm.com/Article/details/gfloofeui.sHtML

namespace App\Http;
来源：http://m.share.hesvh.cn/Article/details/gsjlvhksm.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.hesvh.cn/Article/details/gijxpxahk.sHtML

declare(strict_types=1);
来源：http://3g.fehbvm.com/Article/details/gaghpsqvx.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.zdbjq.cn/Article/details/grybhipft.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/gdufdjwls.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.zdbjq.cn/Article/details/gxprmxxlw.sHtML

?string $name = null
来源：http://www.share.fehbvm.com/Article/details/gdsjxqsol.sHtML

[U47] PHP：联合类型
来源：http://3g.hesvh.cn/Article/details/gzhjgwzha.sHtML

int|string $id
来源：http://wap.hesvh.cn/Article/details/gxyapkzfj.sHtML

[U48] PHP：纯枚举
来源：http://mobile.fehbvm.com/Article/details/gokibshex.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.hesvh.cn/Article/details/gvjiwstuc.sHtML

[U49] PHP：只读属性
来源：http://3g.hesvh.cn/Article/details/gspjkmgrf.sHtML

public readonly string $name
来源：http://blog.zdbjq.cn/Article/details/ghjgygqqt.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.zdbjq.cn/Article/details/glsnfuigb.sHtML

public function __construct(private int $id) {}
来源：http://m.share.zdbjq.cn/Article/details/gcevmgcww.sHtML

[U51] PHP：数组解构
来源：http://baike.hesvh.cn/Article/details/gssowunpe.sHtML

[$a, $b] = $arr;
来源：http://baike.zdbjq.cn/Article/details/gnnslrdox.sHtML

[U52] PHP：箭头函数
来源：http://www.share.zdbjq.cn/Article/details/gpozhnblv.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.zdbjq.cn/Article/details/gywdsbnse.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.zdbjq.cn/Article/details/gjyoxlqwu.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.zdbjq.cn/Article/details/gfhslzqma.sHtML

[U54] PHP：空安全调用
来源：http://wap.hesvh.cn/Article/details/glumoqpfw.sHtML

$obj?->method()
来源：http://wap.zdbjq.cn/Article/details/gocqayyyy.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.fehbvm.com/Article/details/gwihhtpzt.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.fehbvm.com/Article/details/gvxvxwdpi.sHtML

[U56] PHP：命名参数
来源：http://read.share.fehbvm.com/Article/details/gftoauopn.sHtML

f(a: 1, b: 2)
来源：http://www.share.hesvh.cn/Article/details/gtqhnqgdv.sHtML

[U57] PHP：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gjuoloxdq.sHtML

"值: {$a}"
来源：http://baike.fehbvm.com/Article/details/glkqerqqb.sHtML

[U58] PHP：数组三件套
来源：http://baike.zdbjq.cn/Article/details/gyhrzscde.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.zdbjq.cn/Article/details/ggnbatnni.sHtML

[U59] PHP：自定义排序
来源：http://read.share.hesvh.cn/Article/details/gazjbzivm.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fehbvm.com/Article/details/gapobbyvm.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.fehbvm.com/Article/details/gothrifmu.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.fehbvm.com/Article/details/gptjiqxsr.sHtML

[U61] PHP：正则
来源：http://www.m.share.hesvh.cn/Article/details/gspnrddsp.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.fehbvm.com/Article/details/gpcdwnqab.sHtML

[U62] PHP：日期对象
来源：http://wap.hesvh.cn/Article/details/gcfaonhus.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.fehbvm.com/Article/details/gmoxrqsta.sHtML

[U63] PHP：文件读写
来源：http://read.share.hesvh.cn/Article/details/gqclajqlc.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.zdbjq.cn/Article/details/ggydrusow.sHtML

[U64] PHP：目录遍历
来源：http://www.share.zdbjq.cn/Article/details/gzndbrtdl.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.zdbjq.cn/Article/details/gbzqodmhj.sHtML

[U65] PHP：会话
来源：http://m.share.hesvh.cn/Article/details/gnhbogats.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gxxbsfpcd.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.fehbvm.com/Article/details/gsmuhuwmv.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.fehbvm.com/Article/details/gcywgheoy.sHtML

[U67] PHP：处理文件上传
来源：http://blog.hesvh.cn/Article/details/gdvzlxecz.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.fehbvm.com/Article/details/gxokecway.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.hesvh.cn/Article/details/gauxirmfa.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.fehbvm.com/Article/details/gifiwsemj.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.zdbjq.cn/Article/details/grmrexpcf.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.zdbjq.cn/Article/details/gnbigzwog.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.zdbjq.cn/Article/details/gcrogffyb.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.zdbjq.cn/Article/details/gmsqbeulv.sHtML

[U71] PHP：抛出异常
来源：http://read.share.fehbvm.com/Article/details/gwivxgakn.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.hesvh.cn/Article/details/gnxaoflqe.sHtML

[U72] PHP：写错误日志
来源：http://3g.hesvh.cn/Article/details/gmzovfkpa.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.hesvh.cn/Article/details/gvzyrdxck.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.fehbvm.com/Article/details/gxplczwug.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.zdbjq.cn/Article/details/ghbkiiamd.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.hesvh.cn/Article/details/gtjdhyana.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.hesvh.cn/Article/details/grcryvrye.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.hesvh.cn/Article/details/gqlspptgd.sHtML

composer require psr/container
来源：http://mobile.fehbvm.com/Article/details/ggbvscznw.sHtML

[U76] PHP：简单路由
来源：http://wap.hesvh.cn/Article/details/giffeqtwn.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.zdbjq.cn/Article/details/gznxhxbns.sHtML

[U77] PHP：模板渲染
来源：http://read.share.fehbvm.com/Article/details/gfuuvctom.sHtML

composer require twig/twig
来源：http://www.blog.zdbjq.cn/Article/details/gjkyyetep.sHtML

[U78] PHP：单元测试
来源：http://read.share.hesvh.cn/Article/details/gxufhyjin.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.hesvh.cn/Article/details/ganhqbdlc.sHtML

[U79] PHP：静态分析
来源：http://baike.fehbvm.com/Article/details/grvcmmtcl.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.fehbvm.com/Article/details/gzufjngne.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.hesvh.cn/Article/details/gymcuslcx.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.fehbvm.com/Article/details/gwcaizezq.sHtML

[U81] JS：初始化项目
来源：http://read.share.hesvh.cn/Article/details/ghyygqirt.sHtML

npm init -y;  npm i express
来源：http://www.blog.zdbjq.cn/Article/details/giniwceqi.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.hesvh.cn/Article/details/gwuxbroad.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.fehbvm.com/Article/details/gmmyttteo.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.fehbvm.com/Article/details/gqzgmxvso.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.fehbvm.com/Article/details/gapwipohj.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.zdbjq.cn/Article/details/gqqcgfrha.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.zdbjq.cn/Article/details/gonlfbndv.sHtML

[U85] JS：可选链
来源：http://3g.zdbjq.cn/Article/details/gbfoivlsw.sHtML

a?.b?.c
来源：http://m.share.hesvh.cn/Article/details/gcizzhigb.sHtML

[U86] JS：空值合并
来源：http://mobile.fehbvm.com/Article/details/gnbxddlfi.sHtML

a ?? b
来源：http://blog.fehbvm.com/Article/details/gxywlzerj.sHtML

[U87] JS：解构默认值
来源：http://read.share.fehbvm.com/Article/details/gorvrvrnj.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.fehbvm.com/Article/details/gshmasorx.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.hesvh.cn/Article/details/giullbccp.sHtML

{ ...a, ...b }
来源：http://m.share.fehbvm.com/Article/details/gindbgjpu.sHtML

[U89] JS：数组去重
来源：http://read.share.zdbjq.cn/Article/details/geomawlss.sHtML

[...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gbnecaaze.sHtML

[U90] JS：数字数组排序
来源：http://read.share.fehbvm.com/Article/details/gvrzagdzk.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gqensdwcm.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.zdbjq.cn/Article/details/gyxwdvkwq.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.fehbvm.com/Article/details/gvcvdeijr.sHtML

[U92] JS：深拷贝
来源：http://www.blog.hesvh.cn/Article/details/gcpcwinmy.sHtML

structuredClone(obj)
来源：http://wap.hesvh.cn/Article/details/gwdoqqcmf.sHtML

[U93] JS：模板字符串
来源：http://read.share.fehbvm.com/Article/details/ggwefarxb.sHtML

`共 ${n} 条`
来源：http://wap.hesvh.cn/Article/details/gudmdshlu.sHtML

[U94] JS：箭头函数
来源：http://read.share.zdbjq.cn/Article/details/ghajoimvl.sHtML

const double = x => x * 2;
来源：http://mobile.zdbjq.cn/Article/details/gwgytcygu.sHtML

[U95] JS：Promise 包装
来源：http://mobile.fehbvm.com/Article/details/gfvgeslon.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.zdbjq.cn/Article/details/grqejahbv.sHtML

[U96] JS：async/await 与异常
来源：http://3g.fehbvm.com/Article/details/gmggrbluh.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/gznelupao.sHtML

[U97] JS：并发请求
来源：http://www.blog.hesvh.cn/Article/details/gwqbmprsq.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/gacbfjtga.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.zdbjq.cn/Article/details/gxjrpvvem.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.fehbvm.com/Article/details/ggiafyqsx.sHtML

[U99] JS：事件监听
来源：http://m.share.hesvh.cn/Article/details/gnupjyipo.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.fehbvm.com/Article/details/geyqentbs.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.fehbvm.com/Article/details/gokgjkxci.sHtML

document.querySelector(".item")
来源：http://mobile.hesvh.cn/Article/details/gibydbbzq.sHtML

[U101] JS：classList 操作
来源：http://m.share.hesvh.cn/Article/details/gjjkllspm.sHtML

el.classList.toggle("active")
来源：http://baike.hesvh.cn/Article/details/gcbbxwoar.sHtML

[U102] JS：本地存储
来源：http://baike.fehbvm.com/Article/details/gttkthsak.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.fehbvm.com/Article/details/gmepowroy.sHtML

[U103] JS：定时器
来源：http://wap.hesvh.cn/Article/details/gslqbnyjv.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.hesvh.cn/Article/details/gllnewkng.sHtML

[U104] JS：防抖
来源：http://read.share.fehbvm.com/Article/details/gsswxciof.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gqbpypsmc.sHtML

[U105] JS：节流
来源：http://3g.zdbjq.cn/Article/details/gdyagqgwb.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.hesvh.cn/Article/details/gexvaazet.sHtML

[U106] JS：日期格式化
来源：http://www.blog.fehbvm.com/Article/details/ghldxngba.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.fehbvm.com/Article/details/gfxeertec.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.zdbjq.cn/Article/details/gghdnjbni.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.fehbvm.com/Article/details/gshfiwtxw.sHtML

[U108] JS：随机整数
来源：http://www.m.share.fehbvm.com/Article/details/gxyyttwbc.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.zdbjq.cn/Article/details/gfgtntuxb.sHtML

[U109] JS：数组分组
来源：http://wap.fehbvm.com/Article/details/ghnqlscdx.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.zdbjq.cn/Article/details/gydtmdwlt.sHtML

[U110] JS：数组分块
来源：http://baike.hesvh.cn/Article/details/glgmbmalm.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.fehbvm.com/Article/details/gyhcxxvxc.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.fehbvm.com/Article/details/gvwmlmmrg.sHtML

new Map(Object.entries(obj))
来源：http://blog.zdbjq.cn/Article/details/gtojtidag.sHtML

[U112] JS：字符串补位
来源：http://m.share.zdbjq.cn/Article/details/goxjtqqsl.sHtML

"7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/gagxzdqih.sHtML

[U113] JS：正则替换全部
来源：http://3g.hesvh.cn/Article/details/gozuvcdat.sHtML

s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gqzhjwnwu.sHtML

[U114] JS：JSON 深比较
来源：http://baike.fehbvm.com/Article/details/gctzvjdod.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.zdbjq.cn/Article/details/gmvzccqxe.sHtML

[U115] JS：生成 UUID
来源：http://read.share.zdbjq.cn/Article/details/gnbjoeecd.sHtML

crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gnwqzwrpk.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.hesvh.cn/Article/details/gcqiesryw.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.hesvh.cn/Article/details/gmzmsefeu.sHtML

[U117] JS：单元测试
来源：http://www.blog.hesvh.cn/Article/details/gdbwoaaxj.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.hesvh.cn/Article/details/gfpqgvage.sHtML

[U118] JS：开发服务器
来源：http://baike.zdbjq.cn/Article/details/ghpwzauws.sHtML

npm i -D vite;  npx vite
来源：http://www.share.fehbvm.com/Article/details/ggxjxvnjf.sHtML

[U119] JS：生产构建
来源：http://3g.fehbvm.com/Article/details/gfilzhqks.sHtML

npx vite build
来源：http://m.share.fehbvm.com/Article/details/gmltnpqus.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.hesvh.cn/Article/details/glwzcgyjv.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.hesvh.cn/Article/details/gvtsrvxoe.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gfoyzoudf.sHtML

统计汇总
来源：http://mobile.hesvh.cn/Article/details/grbweaykg.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/glpesngbo.sHtML

按语言统计（条）：
来源：http://m.share.fehbvm.com/Article/details/gxxqvcmsg.sHtML

Python ......... 252
来源：http://read.share.hesvh.cn/Article/details/gfbykkxqh.sHtML

PHP ............ 252
来源：http://baike.zdbjq.cn/Article/details/gxinphcml.sHtML

JavaScript ..... 252
来源：http://read.share.fehbvm.com/Article/details/gzbrdbkkw.sHtML

TypeScript ..... 212
来源：http://3g.zdbjq.cn/Article/details/gxiahxfhc.sHtML

Java ........... 212
来源：http://mobile.fehbvm.com/Article/details/glfxmmviw.sHtML

Go ............. 212
来源：http://wap.hesvh.cn/Article/details/gedbhfllc.sHtML

Ruby ........... 212
来源：http://m.share.zdbjq.cn/Article/details/gkaocohnu.sHtML

C# ............. 212
来源：http://wap.hesvh.cn/Article/details/glicisxko.sHtML

C .............. 30
来源：http://3g.zdbjq.cn/Article/details/gjftsknvm.sHtML

C++ ............ 30
来源：http://www.m.share.hesvh.cn/Article/details/goppprhej.sHtML

SQL ............ 90
来源：http://read.share.fehbvm.com/Article/details/gqouefiwd.sHtML

Bash ........... 80
来源：http://www.blog.fehbvm.com/Article/details/gosquhvdn.sHtML

Kotlin ......... 15
来源：http://blog.hesvh.cn/Article/details/gdpkxaftg.sHtML

Swift .......... 15
来源：http://www.share.hesvh.cn/Article/details/gdxgaihqj.sHtML

Lua ............ 10
来源：http://www.blog.hesvh.cn/Article/details/gqhosfmjc.sHtML

Perl ........... 10
来源：http://baike.fehbvm.com/Article/details/gsvchikgu.sHtML

Scala .......... 10
来源：http://mobile.hesvh.cn/Article/details/gkrcrhmgi.sHtML

------------------------------------
来源：http://blog.hesvh.cn/Article/details/ggvdkajcl.sHtML

合计 ........... 2106 条
来源：http://3g.fehbvm.com/Article/details/gsqychlhl.sHtML

按章节统计：
来源：http://www.blog.zdbjq.cn/Article/details/guibddkqv.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.hesvh.cn/Article/details/gwdozdjfr.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.zdbjq.cn/Article/details/gcxwxcdni.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/gvuddgdzz.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.zdbjq.cn/Article/details/ghvkvzrzo.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.hesvh.cn/Article/details/glssqeoof.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.fehbvm.com/Article/details/gptoejgxr.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/gjbslnbbo.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.zdbjq.cn/Article/details/gxwzvxlvz.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gityeyerf.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.zdbjq.cn/Article/details/gkvjjdgnf.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gooqsnmes.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/graznpbts.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gatpjyqhe.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.zdbjq.cn/Article/details/gsodwofty.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.fehbvm.com/Article/details/gpmbnodte.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gfwqedtna.sHtML

Q SQL 专题                              90
来源：http://www.blog.fehbvm.com/Article/details/gumttkyfu.sHtML

R Bash 专题                             80
来源：http://baike.hesvh.cn/Article/details/gtckcqrxu.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.hesvh.cn/Article/details/gjjgnshml.sHtML

T 其他语言补充                          60
来源：http://blog.zdbjq.cn/Article/details/goojdunty.sHtML

U 高频实用片段                         120
来源：http://3g.fehbvm.com/Article/details/ggmtrjppp.sHtML

------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gintmeypx.sHtML

合计                                  2106 条
来源：http://read.share.fehbvm.com/Article/details/gfvccdlcz.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/grojlljfl.sHtML

使用提醒
来源：http://m.share.fehbvm.com/Article/details/gvabgdoug.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gfpisnswi.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.fehbvm.com/Article/details/gimuustcn.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.hesvh.cn/Article/details/gpfkoylvg.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.zdbjq.cn/Article/details/gfsrlxpcs.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.hesvh.cn/Article/details/gmvvepvnu.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.zdbjq.cn/Article/details/gfyjbwmbn.sHtML

—— 文件结束 ——
来源：http://wap.hesvh.cn/Article/details/ggorppqhj.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gmfqatkqa.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.fehbvm.com/Article/details/gtpjndann.sHtML

Common Programming Examples Cheat Book
来源：http://blog.zdbjq.cn/Article/details/gzwagrmcf.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gylyfkcrr.sHtML

【收录内容】
来源：http://3g.fehbvm.com/Article/details/gtbkxouhd.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.hesvh.cn/Article/details/gyraoodbm.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.hesvh.cn/Article/details/gmakozaqn.sHtML

SQL · Bash · C · C++
来源：http://www.blog.fehbvm.com/Article/details/gfjqvnxjd.sHtML


<!-- 参考信息 -->