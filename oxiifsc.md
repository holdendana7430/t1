代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://3g.hesvh.cn/Article/details/goklpvmsi.sHtML

[T59] Scala：循环
来源：http://www.share.zdbjq.cn/Article/details/gdljupsqn.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.zdbjq.cn/Article/details/gwygkadgt.sHtML

[T60] Scala：折叠
来源：http://www.share.hesvh.cn/Article/details/gfsmrpoev.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.hesvh.cn/Article/details/gpmhneiir.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gligbvfyd.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.zdbjq.cn/Article/details/gllqqexhe.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ggflkqjkp.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.fehbvm.com/Article/details/gjueiinjr.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.hesvh.cn/Article/details/gfhlxlgyw.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.hesvh.cn/Article/details/grwygtgbz.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.hesvh.cn/Article/details/gsjrlslba.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.fehbvm.com/Article/details/geroznwby.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.fehbvm.com/Article/details/gmmzombud.sHtML

[U04] Py：变量调试打印
来源：http://wap.hesvh.cn/Article/details/grcmcinfo.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fehbvm.com/Article/details/gbgngotkc.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.fehbvm.com/Article/details/gpchyzxra.sHtML

list(dict.fromkeys(arr))
来源：http://blog.zdbjq.cn/Article/details/gyogdfbmj.sHtML

[U06] Py：合并两个字典
来源：http://3g.hesvh.cn/Article/details/gbtvgzvtt.sHtML

{**a, **b}
来源：http://baike.fehbvm.com/Article/details/gccxnewjf.sHtML

[U07] Py：反转字典键值
来源：http://www.share.hesvh.cn/Article/details/gcjhovakd.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.hesvh.cn/Article/details/gzxinbijv.sHtML

[U08] Py：展平二维列表
来源：http://3g.fehbvm.com/Article/details/gsprxghis.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.zdbjq.cn/Article/details/gqphtfvwz.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.hesvh.cn/Article/details/gyzhmrnob.sHtML

max(d, key=d.get)
来源：http://blog.hesvh.cn/Article/details/gowpqsunh.sHtML

[U10] Py：按值排序字典
来源：http://baike.zdbjq.cn/Article/details/gkohicuog.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.zdbjq.cn/Article/details/gtcfcxwcs.sHtML

[U11] Py：生成器表达式
来源：http://m.share.fehbvm.com/Article/details/ghaweqbvt.sHtML

(x * 2 for x in arr)
来源：http://wap.hesvh.cn/Article/details/gxzmtzokx.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.fehbvm.com/Article/details/grshovonc.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.hesvh.cn/Article/details/ghzijsvff.sHtML

[U13] Py：固定长度队列
来源：http://wap.zdbjq.cn/Article/details/gwczecztj.sHtML

deque(maxlen=10)
来源：http://baike.zdbjq.cn/Article/details/gsknksotl.sHtML

[U14] Py：分组收集到列表
来源：http://3g.zdbjq.cn/Article/details/gycqkfbcj.sHtML

defaultdict(list)
来源：http://read.share.zdbjq.cn/Article/details/gguivlwvr.sHtML

[U15] Py：高精度计时
来源：http://blog.hesvh.cn/Article/details/ggilfsiqd.sHtML

t = time.perf_counter()
来源：http://baike.fehbvm.com/Article/details/gwdqirypy.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.zdbjq.cn/Article/details/grnmaumip.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.fehbvm.com/Article/details/gdxgsepeb.sHtML

[U17] Py：初始化日志
来源：http://baike.hesvh.cn/Article/details/gvpsnkptd.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.fehbvm.com/Article/details/gmokstqcu.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.hesvh.cn/Article/details/gzpnoezyk.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.fehbvm.com/Article/details/gmbwbuqci.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.fehbvm.com/Article/details/gycuhysnq.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.fehbvm.com/Article/details/gjcaiapmm.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.zdbjq.cn/Article/details/gobkhrnyt.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.zdbjq.cn/Article/details/gejmkzsjg.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.fehbvm.com/Article/details/grkhrijww.sHtML

@contextlib.contextmanager
来源：http://blog.zdbjq.cn/Article/details/gwbftjplr.sHtML

[U22] Py：矩阵转置
来源：http://3g.fehbvm.com/Article/details/gvxokjiqp.sHtML

list(zip(*m))
来源：http://3g.zdbjq.cn/Article/details/gyprndrqx.sHtML

[U23] Py：分块读取大文件
来源：http://blog.fehbvm.com/Article/details/gacosmhps.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.zdbjq.cn/Article/details/glaqgfhdj.sHtML

[U24] Py：路径操作
来源：http://blog.zdbjq.cn/Article/details/gdohjbmnj.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.fehbvm.com/Article/details/gaxqedife.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.hesvh.cn/Article/details/gwsvrnevl.sHtML

csv.DictReader(f)
来源：http://mobile.zdbjq.cn/Article/details/gwwjjqifh.sHtML

[U26] Py：并发下载
来源：http://wap.zdbjq.cn/Article/details/gtpvyrsra.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.zdbjq.cn/Article/details/glgwxvoly.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fehbvm.com/Article/details/gxegximec.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.hesvh.cn/Article/details/gfreuzxzg.sHtML

[U28] Py：类型别名
来源：http://www.m.share.fehbvm.com/Article/details/gqgzimned.sHtML

UserId = int
来源：http://blog.zdbjq.cn/Article/details/gxkkzbiou.sHtML

[U29] Py：属性校验
来源：http://mobile.zdbjq.cn/Article/details/goswcwbty.sHtML

@property 与 @x.setter 配合
来源：http://m.share.zdbjq.cn/Article/details/goruulljm.sHtML

[U30] Py：数据类
来源：http://mobile.zdbjq.cn/Article/details/gkvqnvgak.sHtML

@dataclass(slots=True)
来源：http://3g.zdbjq.cn/Article/details/gebeuqrsi.sHtML

[U31] Py：单测
来源：http://m.share.zdbjq.cn/Article/details/gxxqcmppj.sHtML

python -m pytest -q
来源：http://read.share.fehbvm.com/Article/details/gswzdcvtz.sHtML

[U32] Py：代码格式化
来源：http://mobile.fehbvm.com/Article/details/gmzcxbaim.sHtML

ruff format . && ruff check --fix .
来源：http://3g.zdbjq.cn/Article/details/gsczfyzrs.sHtML

[U33] Py：打包发布
来源：http://blog.hesvh.cn/Article/details/gsfxotkuv.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.zdbjq.cn/Article/details/gajolttvx.sHtML

[U34] Py：判断编码
来源：http://www.blog.fehbvm.com/Article/details/gualkrojp.sHtML

chardet.detect(raw)
来源：http://www.share.fehbvm.com/Article/details/gqwwzdzvf.sHtML

[U35] Py：发送邮件
来源：http://wap.fehbvm.com/Article/details/gwluvzbcn.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.zdbjq.cn/Article/details/grexjjbny.sHtML

[U36] Py：定时任务
来源：http://read.share.fehbvm.com/Article/details/gnqhklhce.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.zdbjq.cn/Article/details/gzdpgggtv.sHtML

[U37] Py：读写 Excel
来源：http://3g.hesvh.cn/Article/details/gzyudlwem.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.fehbvm.com/Article/details/goflwqbto.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.zdbjq.cn/Article/details/gitaucuxa.sHtML

Path(__file__).resolve().parent
来源：http://blog.fehbvm.com/Article/details/gutgcgrjw.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.fehbvm.com/Article/details/gqkhvlojb.sHtML

sys.stdout.isatty()
来源：http://blog.hesvh.cn/Article/details/gizuolgrz.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.fehbvm.com/Article/details/gfhxbpmyr.sHtML

print("err", file=sys.stderr)
来源：http://m.share.fehbvm.com/Article/details/guaggtcvc.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.hesvh.cn/Article/details/gjkowmvph.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.hesvh.cn/Article/details/gtzjndvpc.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.zdbjq.cn/Article/details/grrcbecmd.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.hesvh.cn/Article/details/gifsafpjn.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.zdbjq.cn/Article/details/glqqdvjly.sHtML

namespace App\Http;
来源：http://www.blog.zdbjq.cn/Article/details/gcxtkqiir.sHtML

[U44] PHP：开启严格类型
来源：http://blog.fehbvm.com/Article/details/gzyfdqwoz.sHtML

declare(strict_types=1);
来源：http://www.share.zdbjq.cn/Article/details/gbghtvwtp.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.zdbjq.cn/Article/details/gswupolon.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gznbeozfp.sHtML

[U46] PHP：可空类型
来源：http://blog.zdbjq.cn/Article/details/gogxkwlpj.sHtML

?string $name = null
来源：http://www.share.hesvh.cn/Article/details/gxbeoblnn.sHtML

[U47] PHP：联合类型
来源：http://www.blog.fehbvm.com/Article/details/genliyaeb.sHtML

int|string $id
来源：http://m.share.zdbjq.cn/Article/details/gucqvbatx.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.hesvh.cn/Article/details/gyturfobq.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.zdbjq.cn/Article/details/gizzjxysr.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.zdbjq.cn/Article/details/gysituvbm.sHtML

public readonly string $name
来源：http://m.share.hesvh.cn/Article/details/gprtppabs.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.zdbjq.cn/Article/details/gndaqvund.sHtML

public function __construct(private int $id) {}
来源：http://baike.fehbvm.com/Article/details/gzaiobgyq.sHtML

[U51] PHP：数组解构
来源：http://wap.hesvh.cn/Article/details/gsslbvndv.sHtML

[$a, $b] = $arr;
来源：http://baike.fehbvm.com/Article/details/givvqmdfu.sHtML

[U52] PHP：箭头函数
来源：http://wap.hesvh.cn/Article/details/gcsyywlbt.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.fehbvm.com/Article/details/glnebnoar.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.zdbjq.cn/Article/details/gmufqcsou.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.fehbvm.com/Article/details/gotmovkdb.sHtML

[U54] PHP：空安全调用
来源：http://baike.fehbvm.com/Article/details/gdpbjtbim.sHtML

$obj?->method()
来源：http://blog.hesvh.cn/Article/details/gmombpxxx.sHtML

[U55] PHP：match 表达式
来源：http://blog.hesvh.cn/Article/details/gaxgzrtjw.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.hesvh.cn/Article/details/gninfdzgl.sHtML

[U56] PHP：命名参数
来源：http://baike.hesvh.cn/Article/details/gepdeepjo.sHtML

f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/gfverehja.sHtML

[U57] PHP：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gtkzptycf.sHtML

"值: {$a}"
来源：http://baike.zdbjq.cn/Article/details/gxzcbzbfh.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.hesvh.cn/Article/details/gbqphrytj.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.fehbvm.com/Article/details/gnippkmde.sHtML

[U59] PHP：自定义排序
来源：http://m.share.hesvh.cn/Article/details/gpmjuxhjt.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fehbvm.com/Article/details/grieaayft.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.fehbvm.com/Article/details/ghhupiqoi.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.zdbjq.cn/Article/details/gsqlezqka.sHtML

[U61] PHP：正则
来源：http://www.m.share.fehbvm.com/Article/details/gtpbjffsq.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.zdbjq.cn/Article/details/gkzugzlyl.sHtML

[U62] PHP：日期对象
来源：http://read.share.fehbvm.com/Article/details/gvnvpijxg.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.hesvh.cn/Article/details/gxehwbxlj.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.zdbjq.cn/Article/details/gtdscsevr.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.fehbvm.com/Article/details/gliwcfqbr.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.hesvh.cn/Article/details/gnbdwukio.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.hesvh.cn/Article/details/gdxijbvgb.sHtML

[U65] PHP：会话
来源：http://mobile.fehbvm.com/Article/details/ggwckiffd.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gjbtbhlml.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.hesvh.cn/Article/details/gduuilqkx.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.fehbvm.com/Article/details/ggtmdqrai.sHtML

[U67] PHP：处理文件上传
来源：http://blog.hesvh.cn/Article/details/gngwwghfc.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.zdbjq.cn/Article/details/gjyzowryl.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.fehbvm.com/Article/details/gepoigtld.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.zdbjq.cn/Article/details/gykutnkpi.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.fehbvm.com/Article/details/gvhjatery.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.hesvh.cn/Article/details/grfomxrod.sHtML

[U70] PHP：PDO 事务
来源：http://baike.fehbvm.com/Article/details/gemskgmnb.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.fehbvm.com/Article/details/geasgvxxe.sHtML

[U71] PHP：抛出异常
来源：http://www.share.zdbjq.cn/Article/details/gjczulill.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.hesvh.cn/Article/details/goqwyjwig.sHtML

[U72] PHP：写错误日志
来源：http://wap.hesvh.cn/Article/details/grqphjdew.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.zdbjq.cn/Article/details/gcnfizuhc.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.hesvh.cn/Article/details/gmbbyomye.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.zdbjq.cn/Article/details/grneqvekt.sHtML

[U74] PHP：读取环境变量
来源：http://blog.hesvh.cn/Article/details/gdyjldexa.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.fehbvm.com/Article/details/guvthdbuc.sHtML

[U75] PHP：依赖注入
来源：http://3g.zdbjq.cn/Article/details/gmokomkfq.sHtML

composer require psr/container
来源：http://m.share.hesvh.cn/Article/details/grkrtbbmg.sHtML

[U76] PHP：简单路由
来源：http://3g.zdbjq.cn/Article/details/gkswadfev.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.fehbvm.com/Article/details/gmgnmfqqt.sHtML

[U77] PHP：模板渲染
来源：http://read.share.fehbvm.com/Article/details/gkiuxcktt.sHtML

composer require twig/twig
来源：http://blog.fehbvm.com/Article/details/glxznidps.sHtML

[U78] PHP：单元测试
来源：http://www.share.hesvh.cn/Article/details/gtfeqiwyc.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.hesvh.cn/Article/details/gzhklgkip.sHtML

[U79] PHP：静态分析
来源：http://baike.zdbjq.cn/Article/details/ghwmoznoe.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.hesvh.cn/Article/details/grlkbcplu.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.hesvh.cn/Article/details/gpfkaplco.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.hesvh.cn/Article/details/gqwoznmew.sHtML

[U81] JS：初始化项目
来源：http://wap.hesvh.cn/Article/details/ggefewrgg.sHtML

npm init -y;  npm i express
来源：http://www.blog.hesvh.cn/Article/details/gngdlkqhp.sHtML

[U82] JS：package.json 脚本
来源：http://wap.zdbjq.cn/Article/details/gsyjkayto.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.zdbjq.cn/Article/details/gytfuczsm.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.hesvh.cn/Article/details/geyhitgqe.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.hesvh.cn/Article/details/gpgxlwylv.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.hesvh.cn/Article/details/gapyvgvbd.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.zdbjq.cn/Article/details/ghjjmived.sHtML

[U85] JS：可选链
来源：http://3g.hesvh.cn/Article/details/gkysrnjot.sHtML

a?.b?.c
来源：http://3g.zdbjq.cn/Article/details/gcqvtrmmt.sHtML

[U86] JS：空值合并
来源：http://baike.fehbvm.com/Article/details/gdowqauem.sHtML

a ?? b
来源：http://www.share.fehbvm.com/Article/details/gqcsulmon.sHtML

[U87] JS：解构默认值
来源：http://baike.zdbjq.cn/Article/details/gmvxjwcml.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.hesvh.cn/Article/details/geuaqsczb.sHtML

[U88] JS：对象展开合并
来源：http://www.share.hesvh.cn/Article/details/gfcwagtun.sHtML

{ ...a, ...b }
来源：http://m.share.zdbjq.cn/Article/details/gdssasrty.sHtML

[U89] JS：数组去重
来源：http://www.m.share.hesvh.cn/Article/details/gxaprjrib.sHtML

[...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/gxuvhqenw.sHtML

[U90] JS：数字数组排序
来源：http://m.share.hesvh.cn/Article/details/gkldlyktx.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gehsrposa.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.hesvh.cn/Article/details/grifltzjw.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.zdbjq.cn/Article/details/gkvnhqnok.sHtML

[U92] JS：深拷贝
来源：http://baike.zdbjq.cn/Article/details/grxgbzvik.sHtML

structuredClone(obj)
来源：http://blog.hesvh.cn/Article/details/gisbpslqq.sHtML

[U93] JS：模板字符串
来源：http://wap.zdbjq.cn/Article/details/gcjebncrw.sHtML

`共 ${n} 条`
来源：http://www.m.share.hesvh.cn/Article/details/geqqucnuu.sHtML

[U94] JS：箭头函数
来源：http://m.share.zdbjq.cn/Article/details/gdpxpmhun.sHtML

const double = x => x * 2;
来源：http://baike.fehbvm.com/Article/details/gutlugedd.sHtML

[U95] JS：Promise 包装
来源：http://read.share.zdbjq.cn/Article/details/gnbokygyc.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.zdbjq.cn/Article/details/gvmsfmnza.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.fehbvm.com/Article/details/gpbtfgkwa.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/glfwbaysb.sHtML

[U97] JS：并发请求
来源：http://www.m.share.zdbjq.cn/Article/details/gerdbdqih.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/goyrxnbjr.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.zdbjq.cn/Article/details/gwhvjyjff.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.fehbvm.com/Article/details/goscccprb.sHtML

[U99] JS：事件监听
来源：http://mobile.fehbvm.com/Article/details/gtuepxigh.sHtML

el.addEventListener("click", e => {})
来源：http://baike.zdbjq.cn/Article/details/gqmvxoshj.sHtML

[U100] JS：DOM 查询
来源：http://baike.zdbjq.cn/Article/details/ghmgvkpjj.sHtML

document.querySelector(".item")
来源：http://www.blog.hesvh.cn/Article/details/gmozszmpd.sHtML

[U101] JS：classList 操作
来源：http://m.share.fehbvm.com/Article/details/goizklwkp.sHtML

el.classList.toggle("active")
来源：http://m.share.fehbvm.com/Article/details/ghxgmraoq.sHtML

[U102] JS：本地存储
来源：http://www.m.share.fehbvm.com/Article/details/guftiosqq.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.hesvh.cn/Article/details/ggxujojox.sHtML

[U103] JS：定时器
来源：http://baike.fehbvm.com/Article/details/gxabmmtuu.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.fehbvm.com/Article/details/gqkooibax.sHtML

[U104] JS：防抖
来源：http://wap.zdbjq.cn/Article/details/gjdxwuqxo.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/glyymxbzb.sHtML

[U105] JS：节流
来源：http://3g.hesvh.cn/Article/details/gnpiiiblk.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.zdbjq.cn/Article/details/gikjxssal.sHtML

[U106] JS：日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gbutyouyg.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.zdbjq.cn/Article/details/gsydjrrly.sHtML

[U107] JS：数字千分位
来源：http://m.share.fehbvm.com/Article/details/grqriifum.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.fehbvm.com/Article/details/guwotsbcv.sHtML

[U108] JS：随机整数
来源：http://www.share.hesvh.cn/Article/details/gfpqoruef.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.fehbvm.com/Article/details/gjnlivdfr.sHtML

[U109] JS：数组分组
来源：http://blog.fehbvm.com/Article/details/gngibksel.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.zdbjq.cn/Article/details/gibfacfpq.sHtML

[U110] JS：数组分块
来源：http://wap.hesvh.cn/Article/details/gipgqzcpd.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.fehbvm.com/Article/details/gxtonlsyf.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.fehbvm.com/Article/details/gzwqijtkd.sHtML

new Map(Object.entries(obj))
来源：http://baike.fehbvm.com/Article/details/gywvzhavo.sHtML

[U112] JS：字符串补位
来源：http://baike.hesvh.cn/Article/details/gfoilbdas.sHtML

"7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/gemrvymxj.sHtML

[U113] JS：正则替换全部
来源：http://mobile.hesvh.cn/Article/details/ghzruwvva.sHtML

s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gomkxprzq.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.fehbvm.com/Article/details/gbcpaachk.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fehbvm.com/Article/details/grioqsito.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.zdbjq.cn/Article/details/guhdaimxk.sHtML

crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gldlojafl.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.zdbjq.cn/Article/details/gmtdmpjhu.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.zdbjq.cn/Article/details/gvwbzmzxr.sHtML

[U117] JS：单元测试
来源：http://mobile.fehbvm.com/Article/details/gypkscofy.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.hesvh.cn/Article/details/goofkrnnp.sHtML

[U118] JS：开发服务器
来源：http://www.blog.hesvh.cn/Article/details/gmwwuwlic.sHtML

npm i -D vite;  npx vite
来源：http://read.share.hesvh.cn/Article/details/gyyouflof.sHtML

[U119] JS：生产构建
来源：http://www.blog.fehbvm.com/Article/details/gejkybngp.sHtML

npx vite build
来源：http://www.blog.zdbjq.cn/Article/details/gimrdljjx.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.zdbjq.cn/Article/details/gwjyouccm.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.fehbvm.com/Article/details/gdqfoibuh.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gjsjnxtwj.sHtML

统计汇总
来源：http://m.share.hesvh.cn/Article/details/gmvpwkdye.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/glpxbjubp.sHtML

按语言统计（条）：
来源：http://wap.zdbjq.cn/Article/details/ggbnfgsfp.sHtML

Python ......... 252
来源：http://wap.zdbjq.cn/Article/details/gfvbqfbif.sHtML

PHP ............ 252
来源：http://www.blog.hesvh.cn/Article/details/gmqdfimyw.sHtML

JavaScript ..... 252
来源：http://m.share.hesvh.cn/Article/details/gkarxopnb.sHtML

TypeScript ..... 212
来源：http://blog.zdbjq.cn/Article/details/gofcksfew.sHtML

Java ........... 212
来源：http://wap.hesvh.cn/Article/details/gtvihuazx.sHtML

Go ............. 212
来源：http://www.blog.zdbjq.cn/Article/details/gxraqbkhf.sHtML

Ruby ........... 212
来源：http://blog.fehbvm.com/Article/details/gtaykiyyh.sHtML

C# ............. 212
来源：http://m.share.zdbjq.cn/Article/details/gbzhmgubh.sHtML

C .............. 30
来源：http://read.share.zdbjq.cn/Article/details/gcpcstwbl.sHtML

C++ ............ 30
来源：http://baike.hesvh.cn/Article/details/gxjaopvsw.sHtML

SQL ............ 90
来源：http://read.share.zdbjq.cn/Article/details/gigcwukbu.sHtML

Bash ........... 80
来源：http://blog.zdbjq.cn/Article/details/grkuyjrbu.sHtML

Kotlin ......... 15
来源：http://m.share.zdbjq.cn/Article/details/gvomdgacl.sHtML

Swift .......... 15
来源：http://www.m.share.hesvh.cn/Article/details/ggeqqlwds.sHtML

Lua ............ 10
来源：http://www.m.share.fehbvm.com/Article/details/gkrhesker.sHtML

Perl ........... 10
来源：http://www.m.share.zdbjq.cn/Article/details/gghmzgqcc.sHtML

Scala .......... 10
来源：http://www.blog.fehbvm.com/Article/details/gdapgtwyc.sHtML

------------------------------------
来源：http://3g.fehbvm.com/Article/details/ghwncrplp.sHtML

合计 ........... 2106 条
来源：http://baike.hesvh.cn/Article/details/gxvlkmoxi.sHtML

按章节统计：
来源：http://www.blog.hesvh.cn/Article/details/gwpruwimn.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.fehbvm.com/Article/details/ghkaxgqlh.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.zdbjq.cn/Article/details/gcsugzlwn.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/gedgxferl.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.hesvh.cn/Article/details/ggllytuow.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.zdbjq.cn/Article/details/grgcioyge.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.hesvh.cn/Article/details/glgxjtnyd.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/gorsckdfj.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.hesvh.cn/Article/details/gvsmtpomo.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gxhsrvttm.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.fehbvm.com/Article/details/gqcpfxvxk.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gsbvgqxus.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gkonyrdma.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gsxvtxcdz.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.hesvh.cn/Article/details/gvvnfompq.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.fehbvm.com/Article/details/guvgkgnhy.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gznpzuxbr.sHtML

Q SQL 专题                              90
来源：http://mobile.zdbjq.cn/Article/details/gsltlebwj.sHtML

R Bash 专题                             80
来源：http://blog.fehbvm.com/Article/details/gyumztyzi.sHtML

S C / C++ 专题                          60
来源：http://3g.hesvh.cn/Article/details/goiyyppzq.sHtML

T 其他语言补充                          60
来源：http://www.blog.fehbvm.com/Article/details/gckaytbxl.sHtML

U 高频实用片段                         120
来源：http://3g.zdbjq.cn/Article/details/gfcczxswc.sHtML

------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gjhakvdxy.sHtML

合计                                  2106 条
来源：http://www.m.share.fehbvm.com/Article/details/grlayvnvc.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/guepdxnla.sHtML

使用提醒
来源：http://read.share.hesvh.cn/Article/details/gvunfhfox.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/gcfxekyhf.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.fehbvm.com/Article/details/gofzdrvaa.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.hesvh.cn/Article/details/ggqsrnuka.sHtML


<!-- 参考信息 -->