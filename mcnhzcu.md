代发 wailian999

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.hesvh.cn/Article/details/gcuwvezag.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gycsddmbl.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.hesvh.cn/Article/details/glymtaday.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gluduojxf.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.zdbjq.cn/Article/details/gpigmnzlm.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.hesvh.cn/Article/details/gykpwdnju.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.fehbvm.com/Article/details/gvlrsoumb.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.hesvh.cn/Article/details/gitepjilq.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.zdbjq.cn/Article/details/gramihehy.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.hesvh.cn/Article/details/gjqtnddcv.sHtML

[U04] Py：变量调试打印
来源：http://blog.fehbvm.com/Article/details/gtevyebav.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.fehbvm.com/Article/details/gcmkxaeuj.sHtML

[U05] Py：列表去重且保序
来源：http://3g.fehbvm.com/Article/details/gdnhkctta.sHtML

list(dict.fromkeys(arr))
来源：http://3g.hesvh.cn/Article/details/gvxangzrz.sHtML

[U06] Py：合并两个字典
来源：http://wap.hesvh.cn/Article/details/gnoobvdto.sHtML

{**a, **b}
来源：http://www.blog.hesvh.cn/Article/details/guwsibypn.sHtML

[U07] Py：反转字典键值
来源：http://www.share.fehbvm.com/Article/details/gldxedynp.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.fehbvm.com/Article/details/ggohyokjj.sHtML

[U08] Py：展平二维列表
来源：http://mobile.hesvh.cn/Article/details/gxrtzjbre.sHtML

[y for x in nested for y in x]
来源：http://www.blog.hesvh.cn/Article/details/grhnxmhbb.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.hesvh.cn/Article/details/gbyztalod.sHtML

max(d, key=d.get)
来源：http://www.blog.hesvh.cn/Article/details/gvodbkfmd.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.fehbvm.com/Article/details/gfznuqsim.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.zdbjq.cn/Article/details/godkuidbr.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.hesvh.cn/Article/details/gogazkhbm.sHtML

(x * 2 for x in arr)
来源：http://wap.hesvh.cn/Article/details/gladceffk.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.fehbvm.com/Article/details/gnlgqpjkg.sHtML

Counter(arr).most_common(3)
来源：http://wap.zdbjq.cn/Article/details/gozbwacdp.sHtML

[U13] Py：固定长度队列
来源：http://www.share.zdbjq.cn/Article/details/gfrmgupfg.sHtML

deque(maxlen=10)
来源：http://www.blog.hesvh.cn/Article/details/gimytzufj.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.zdbjq.cn/Article/details/geglmedhk.sHtML

defaultdict(list)
来源：http://www.m.share.zdbjq.cn/Article/details/giloayttw.sHtML

[U15] Py：高精度计时
来源：http://read.share.fehbvm.com/Article/details/gxpusfgyc.sHtML

t = time.perf_counter()
来源：http://wap.zdbjq.cn/Article/details/gurovsnrr.sHtML

[U16] Py：命令行参数解析
来源：http://blog.fehbvm.com/Article/details/ghscwgtxe.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.zdbjq.cn/Article/details/ggxwbxueb.sHtML

[U17] Py：初始化日志
来源：http://mobile.hesvh.cn/Article/details/gythounjw.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.fehbvm.com/Article/details/goutozlqz.sHtML

[U18] Py：预编译正则
来源：http://www.share.fehbvm.com/Article/details/gxwhfalxa.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.fehbvm.com/Article/details/gxjjckwun.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.zdbjq.cn/Article/details/gudvcplmr.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fehbvm.com/Article/details/gsvqwqusg.sHtML

[U20] Py：缓存函数结果
来源：http://blog.zdbjq.cn/Article/details/gpdhqcbvs.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.zdbjq.cn/Article/details/ggdosqjwf.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.zdbjq.cn/Article/details/gskckoiei.sHtML

@contextlib.contextmanager
来源：http://blog.hesvh.cn/Article/details/gnxwgecek.sHtML

[U22] Py：矩阵转置
来源：http://m.share.zdbjq.cn/Article/details/gypfcltcr.sHtML

list(zip(*m))
来源：http://www.share.hesvh.cn/Article/details/gezdnlgeh.sHtML

[U23] Py：分块读取大文件
来源：http://wap.fehbvm.com/Article/details/gnjsgnurd.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.fehbvm.com/Article/details/gbijmiobv.sHtML

[U24] Py：路径操作
来源：http://mobile.zdbjq.cn/Article/details/gcvnpqvyv.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.zdbjq.cn/Article/details/ggenfwvns.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.zdbjq.cn/Article/details/gyxuwdijx.sHtML

csv.DictReader(f)
来源：http://baike.fehbvm.com/Article/details/gxhcsiila.sHtML

[U26] Py：并发下载
来源：http://3g.fehbvm.com/Article/details/gfdssjggt.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.hesvh.cn/Article/details/gbykzkvrh.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.hesvh.cn/Article/details/ggfquqsjx.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.hesvh.cn/Article/details/gmqqmkiza.sHtML

[U28] Py：类型别名
来源：http://3g.hesvh.cn/Article/details/gtzucyzpo.sHtML

UserId = int
来源：http://www.m.share.hesvh.cn/Article/details/gmirvuwrc.sHtML

[U29] Py：属性校验
来源：http://blog.zdbjq.cn/Article/details/gglkanipz.sHtML

@property 与 @x.setter 配合
来源：http://blog.zdbjq.cn/Article/details/guskpefrz.sHtML

[U30] Py：数据类
来源：http://baike.fehbvm.com/Article/details/gmavnumew.sHtML

@dataclass(slots=True)
来源：http://www.share.zdbjq.cn/Article/details/gzkvfcpyp.sHtML

[U31] Py：单测
来源：http://blog.zdbjq.cn/Article/details/gqnhwrwli.sHtML

python -m pytest -q
来源：http://www.m.share.hesvh.cn/Article/details/gwbsikfko.sHtML

[U32] Py：代码格式化
来源：http://m.share.hesvh.cn/Article/details/gaekhgjsb.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.hesvh.cn/Article/details/gapzmurhv.sHtML

[U33] Py：打包发布
来源：http://blog.fehbvm.com/Article/details/gmhopvdkl.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.fehbvm.com/Article/details/gmmnaxjiq.sHtML

[U34] Py：判断编码
来源：http://baike.zdbjq.cn/Article/details/gilwpsnsp.sHtML

chardet.detect(raw)
来源：http://m.share.hesvh.cn/Article/details/gsfwackqw.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.hesvh.cn/Article/details/gfnfnkeum.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.zdbjq.cn/Article/details/gpezqhgqw.sHtML

[U36] Py：定时任务
来源：http://blog.hesvh.cn/Article/details/ghhqzhxlr.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.zdbjq.cn/Article/details/gxuwsehkx.sHtML

[U37] Py：读写 Excel
来源：http://read.share.hesvh.cn/Article/details/gccezlovb.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.fehbvm.com/Article/details/gevisqnmx.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.zdbjq.cn/Article/details/gphmqnodv.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.zdbjq.cn/Article/details/gcfeakxfz.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.fehbvm.com/Article/details/gdqrnfgde.sHtML

sys.stdout.isatty()
来源：http://blog.hesvh.cn/Article/details/gkuoetecc.sHtML

[U40] Py：打印到标准错误
来源：http://wap.fehbvm.com/Article/details/gptdghiav.sHtML

print("err", file=sys.stderr)
来源：http://mobile.fehbvm.com/Article/details/ggcpdawrh.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.zdbjq.cn/Article/details/gpolestzq.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.fehbvm.com/Article/details/ghzxbthks.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.fehbvm.com/Article/details/gpxeqcbao.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.fehbvm.com/Article/details/grcznoxet.sHtML

[U43] PHP：声明命名空间
来源：http://3g.zdbjq.cn/Article/details/gzyioxrup.sHtML

namespace App\Http;
来源：http://blog.fehbvm.com/Article/details/gbygebied.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.hesvh.cn/Article/details/gswhcocjv.sHtML

declare(strict_types=1);
来源：http://www.m.share.hesvh.cn/Article/details/gupvexzbp.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.hesvh.cn/Article/details/gozxwgpjw.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/grfhzgcfs.sHtML

[U46] PHP：可空类型
来源：http://www.share.fehbvm.com/Article/details/ggwsmmslc.sHtML

?string $name = null
来源：http://www.share.fehbvm.com/Article/details/gdpjvoftb.sHtML

[U47] PHP：联合类型
来源：http://www.share.fehbvm.com/Article/details/ghxbglizb.sHtML

int|string $id
来源：http://www.m.share.fehbvm.com/Article/details/gtsivuymm.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.hesvh.cn/Article/details/gbeaplxux.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.hesvh.cn/Article/details/gkzaxgjum.sHtML

[U49] PHP：只读属性
来源：http://www.share.fehbvm.com/Article/details/gbotvxasd.sHtML

public readonly string $name
来源：http://read.share.fehbvm.com/Article/details/gnltwbpoh.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.hesvh.cn/Article/details/gfpcmdure.sHtML

public function __construct(private int $id) {}
来源：http://m.share.zdbjq.cn/Article/details/ggpcvfosk.sHtML

[U51] PHP：数组解构
来源：http://www.blog.fehbvm.com/Article/details/gjgkhtfdc.sHtML

[$a, $b] = $arr;
来源：http://www.blog.fehbvm.com/Article/details/gvwizxmiu.sHtML

[U52] PHP：箭头函数
来源：http://mobile.fehbvm.com/Article/details/gduqkfnmq.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.zdbjq.cn/Article/details/gnjlmdyuh.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.fehbvm.com/Article/details/gcvgmfulr.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.zdbjq.cn/Article/details/giwycldgq.sHtML

[U54] PHP：空安全调用
来源：http://3g.fehbvm.com/Article/details/ggevtfauq.sHtML

$obj?->method()
来源：http://www.blog.hesvh.cn/Article/details/gucoytodu.sHtML

[U55] PHP：match 表达式
来源：http://mobile.zdbjq.cn/Article/details/guatbdafe.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.hesvh.cn/Article/details/gnqwhjxeh.sHtML

[U56] PHP：命名参数
来源：http://m.share.fehbvm.com/Article/details/ggtgnosye.sHtML

f(a: 1, b: 2)
来源：http://baike.hesvh.cn/Article/details/gmaeawida.sHtML

[U57] PHP：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gabnaonxf.sHtML

"值: {$a}"
来源：http://www.m.share.fehbvm.com/Article/details/gxyqvobud.sHtML

[U58] PHP：数组三件套
来源：http://baike.fehbvm.com/Article/details/gbmsotavt.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.fehbvm.com/Article/details/gkgtjsncs.sHtML

[U59] PHP：自定义排序
来源：http://read.share.fehbvm.com/Article/details/grrxjqozg.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fehbvm.com/Article/details/gnhgvjyzg.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.fehbvm.com/Article/details/gxbtogjvv.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.zdbjq.cn/Article/details/gzljukcoa.sHtML

[U61] PHP：正则
来源：http://www.blog.zdbjq.cn/Article/details/gklztraej.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.hesvh.cn/Article/details/ggirgdvvk.sHtML

[U62] PHP：日期对象
来源：http://www.share.hesvh.cn/Article/details/ggijbgxzp.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.zdbjq.cn/Article/details/gkdatzuux.sHtML

[U63] PHP：文件读写
来源：http://m.share.fehbvm.com/Article/details/ghmaitqqf.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.fehbvm.com/Article/details/gvtyrdyrm.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.fehbvm.com/Article/details/gdruffddh.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.hesvh.cn/Article/details/gobkxriac.sHtML

[U65] PHP：会话
来源：http://www.blog.hesvh.cn/Article/details/gbhxxgzhi.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.hesvh.cn/Article/details/gmfgcnhyo.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.fehbvm.com/Article/details/gjpydcozy.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.fehbvm.com/Article/details/gffblbahm.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.zdbjq.cn/Article/details/gsfgoispt.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.zdbjq.cn/Article/details/grrqrjuex.sHtML

[U68] PHP：PDO 连接
来源：http://blog.fehbvm.com/Article/details/ghutskqdk.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.zdbjq.cn/Article/details/gtlujyful.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.zdbjq.cn/Article/details/gpuvdjcsp.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.fehbvm.com/Article/details/gljsxzsob.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.hesvh.cn/Article/details/gcwuryglb.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.zdbjq.cn/Article/details/gtchwevze.sHtML

[U71] PHP：抛出异常
来源：http://www.share.fehbvm.com/Article/details/gjxxscbgn.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.fehbvm.com/Article/details/ghfvfsuxr.sHtML

[U72] PHP：写错误日志
来源：http://read.share.zdbjq.cn/Article/details/gmubyimxk.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.zdbjq.cn/Article/details/gezevzdfo.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.fehbvm.com/Article/details/gpyoxxqnm.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.zdbjq.cn/Article/details/gsykwwksf.sHtML

[U74] PHP：读取环境变量
来源：http://3g.hesvh.cn/Article/details/glilmvymx.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.hesvh.cn/Article/details/gscjcctqs.sHtML

[U75] PHP：依赖注入
来源：http://www.share.fehbvm.com/Article/details/gudumhyvt.sHtML

composer require psr/container
来源：http://wap.fehbvm.com/Article/details/gyxlambjd.sHtML

[U76] PHP：简单路由
来源：http://m.share.zdbjq.cn/Article/details/gtjsftvnx.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.hesvh.cn/Article/details/gtjfimiak.sHtML

[U77] PHP：模板渲染
来源：http://blog.hesvh.cn/Article/details/gaviiqeyw.sHtML

composer require twig/twig
来源：http://m.share.fehbvm.com/Article/details/gdbytnfvk.sHtML

[U78] PHP：单元测试
来源：http://m.share.fehbvm.com/Article/details/gvvxryals.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.zdbjq.cn/Article/details/gsctvcapz.sHtML

[U79] PHP：静态分析
来源：http://mobile.zdbjq.cn/Article/details/geodzfqae.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.fehbvm.com/Article/details/grnrgmrxe.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.hesvh.cn/Article/details/ggzckqmiu.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.hesvh.cn/Article/details/ghrnxvery.sHtML

[U81] JS：初始化项目
来源：http://www.blog.fehbvm.com/Article/details/gstlkjyro.sHtML

npm init -y;  npm i express
来源：http://3g.zdbjq.cn/Article/details/gkcfapolq.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.fehbvm.com/Article/details/gnlayixqc.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.hesvh.cn/Article/details/gmkidrnvr.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.fehbvm.com/Article/details/gymslwghw.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.fehbvm.com/Article/details/gkyelnvxt.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.zdbjq.cn/Article/details/gnqjcxchv.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.fehbvm.com/Article/details/gwyaxjtvk.sHtML

[U85] JS：可选链
来源：http://mobile.fehbvm.com/Article/details/gjbeeeoyf.sHtML

a?.b?.c
来源：http://m.share.zdbjq.cn/Article/details/gmmgdkpcn.sHtML

[U86] JS：空值合并
来源：http://mobile.zdbjq.cn/Article/details/gljczxapw.sHtML

a ?? b
来源：http://blog.hesvh.cn/Article/details/ggvlsxsdx.sHtML

[U87] JS：解构默认值
来源：http://3g.fehbvm.com/Article/details/ghtkibhzs.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.fehbvm.com/Article/details/gsgdozkev.sHtML

[U88] JS：对象展开合并
来源：http://read.share.fehbvm.com/Article/details/gusxdkqxu.sHtML

{ ...a, ...b }
来源：http://3g.fehbvm.com/Article/details/gcjmnreaf.sHtML

[U89] JS：数组去重
来源：http://3g.hesvh.cn/Article/details/gftkkcfll.sHtML

[...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gwrhgtzjc.sHtML

[U90] JS：数字数组排序
来源：http://blog.hesvh.cn/Article/details/gvzzcorgd.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gllhthrjz.sHtML

[U91] JS：对象键值遍历
来源：http://wap.fehbvm.com/Article/details/gojtykmua.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.hesvh.cn/Article/details/gdahaxxsi.sHtML

[U92] JS：深拷贝
来源：http://3g.hesvh.cn/Article/details/goozvlppg.sHtML

structuredClone(obj)
来源：http://www.blog.hesvh.cn/Article/details/gxbmiyjmk.sHtML

[U93] JS：模板字符串
来源：http://mobile.hesvh.cn/Article/details/gatqfopep.sHtML

`共 ${n} 条`
来源：http://blog.hesvh.cn/Article/details/gochklidx.sHtML

[U94] JS：箭头函数
来源：http://baike.fehbvm.com/Article/details/gupuwzeml.sHtML

const double = x => x * 2;
来源：http://m.share.fehbvm.com/Article/details/gqakxwwhn.sHtML

[U95] JS：Promise 包装
来源：http://www.share.zdbjq.cn/Article/details/gzuwrrytt.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.zdbjq.cn/Article/details/grdrywvkm.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.fehbvm.com/Article/details/gveyfthmk.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.zdbjq.cn/Article/details/gdnxjdepa.sHtML

[U97] JS：并发请求
来源：http://baike.fehbvm.com/Article/details/gxydejiep.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/gxojnqjbn.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.fehbvm.com/Article/details/gstzmxjrd.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.fehbvm.com/Article/details/gttygvhgo.sHtML

[U99] JS：事件监听
来源：http://blog.zdbjq.cn/Article/details/glppsjbnp.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.zdbjq.cn/Article/details/gjfyaqcjg.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.hesvh.cn/Article/details/gidgafhkz.sHtML

document.querySelector(".item")
来源：http://read.share.hesvh.cn/Article/details/glmvhcazs.sHtML

[U101] JS：classList 操作
来源：http://mobile.zdbjq.cn/Article/details/gobiphopc.sHtML

el.classList.toggle("active")
来源：http://wap.hesvh.cn/Article/details/gckxagisb.sHtML

[U102] JS：本地存储
来源：http://blog.hesvh.cn/Article/details/gqpjeivcg.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.hesvh.cn/Article/details/gcayzrcft.sHtML

[U103] JS：定时器
来源：http://3g.zdbjq.cn/Article/details/gzvjjxrcz.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.zdbjq.cn/Article/details/gnbtluxzu.sHtML

[U104] JS：防抖
来源：http://blog.zdbjq.cn/Article/details/gichnxdbf.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/gwxzhiruq.sHtML

[U105] JS：节流
来源：http://read.share.zdbjq.cn/Article/details/gdoakuyfj.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.hesvh.cn/Article/details/gjggpdkkl.sHtML

[U106] JS：日期格式化
来源：http://wap.hesvh.cn/Article/details/ghllxepkn.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.zdbjq.cn/Article/details/gznqqmagf.sHtML

[U107] JS：数字千分位
来源：http://www.share.hesvh.cn/Article/details/gdvbvywcs.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.fehbvm.com/Article/details/gukaqpvjy.sHtML

[U108] JS：随机整数
来源：http://www.share.hesvh.cn/Article/details/gjioulwqs.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.fehbvm.com/Article/details/gdaolszay.sHtML

[U109] JS：数组分组
来源：http://m.share.hesvh.cn/Article/details/ghtpwurud.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.hesvh.cn/Article/details/guztouqcx.sHtML

[U110] JS：数组分块
来源：http://mobile.fehbvm.com/Article/details/gafsstapa.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.zdbjq.cn/Article/details/gcdchjyij.sHtML

[U111] JS：对象转 Map
来源：http://3g.fehbvm.com/Article/details/glfdenjis.sHtML

new Map(Object.entries(obj))
来源：http://3g.fehbvm.com/Article/details/gouwlyois.sHtML

[U112] JS：字符串补位
来源：http://read.share.zdbjq.cn/Article/details/gmhctgjwt.sHtML

"7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gievmtnkq.sHtML

[U113] JS：正则替换全部
来源：http://m.share.fehbvm.com/Article/details/gorivxibv.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gxqqwhyag.sHtML

[U114] JS：JSON 深比较
来源：http://wap.hesvh.cn/Article/details/grlkutzqj.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.zdbjq.cn/Article/details/gqporvrka.sHtML

[U115] JS：生成 UUID
来源：http://mobile.zdbjq.cn/Article/details/gkciwpztw.sHtML

crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/glwvqkoiv.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.fehbvm.com/Article/details/gvopgaxtn.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.hesvh.cn/Article/details/gzzwtldhp.sHtML

[U117] JS：单元测试
来源：http://mobile.fehbvm.com/Article/details/gzilftthi.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.fehbvm.com/Article/details/gtexgorjm.sHtML

[U118] JS：开发服务器
来源：http://m.share.fehbvm.com/Article/details/gwebogtgt.sHtML

npm i -D vite;  npx vite
来源：http://3g.hesvh.cn/Article/details/gjfgxcnox.sHtML

[U119] JS：生产构建
来源：http://blog.hesvh.cn/Article/details/gdpsyrang.sHtML

npx vite build
来源：http://wap.zdbjq.cn/Article/details/giwhojwof.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.zdbjq.cn/Article/details/gfiwqsgph.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.zdbjq.cn/Article/details/gyakkpzti.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gnoerfafw.sHtML

统计汇总
来源：http://wap.zdbjq.cn/Article/details/gfqgzxnzz.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gqcbiusnw.sHtML

按语言统计（条）：
来源：http://baike.zdbjq.cn/Article/details/glqoaftvy.sHtML

Python ......... 252
来源：http://baike.fehbvm.com/Article/details/gmempkmgy.sHtML

PHP ............ 252
来源：http://read.share.hesvh.cn/Article/details/gifknmsgh.sHtML

JavaScript ..... 252
来源：http://www.share.fehbvm.com/Article/details/guktzpmkj.sHtML

TypeScript ..... 212
来源：http://www.share.fehbvm.com/Article/details/gllzhxvuv.sHtML

Java ........... 212
来源：http://read.share.zdbjq.cn/Article/details/gbubflamn.sHtML

Go ............. 212
来源：http://www.m.share.fehbvm.com/Article/details/gaqwylfci.sHtML

Ruby ........... 212
来源：http://wap.fehbvm.com/Article/details/gmbptybpi.sHtML

C# ............. 212
来源：http://read.share.zdbjq.cn/Article/details/gidugaibd.sHtML

C .............. 30
来源：http://m.share.zdbjq.cn/Article/details/gtpxvrgbs.sHtML

C++ ............ 30
来源：http://baike.zdbjq.cn/Article/details/gcjbhawpt.sHtML

SQL ............ 90
来源：http://www.share.zdbjq.cn/Article/details/gppaqmgnt.sHtML

Bash ........... 80
来源：http://read.share.hesvh.cn/Article/details/gpgizyucd.sHtML

Kotlin ......... 15
来源：http://www.share.fehbvm.com/Article/details/gguyyknhg.sHtML

Swift .......... 15
来源：http://www.blog.zdbjq.cn/Article/details/gijnzbeyq.sHtML

Lua ............ 10
来源：http://www.share.hesvh.cn/Article/details/gednbagom.sHtML

Perl ........... 10
来源：http://m.share.fehbvm.com/Article/details/gjpihmhtc.sHtML

Scala .......... 10
来源：http://www.share.zdbjq.cn/Article/details/gwsvkrkir.sHtML

------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gmdxejozx.sHtML

合计 ........... 2106 条
来源：http://m.share.fehbvm.com/Article/details/gdzxotyjk.sHtML

按章节统计：
来源：http://3g.fehbvm.com/Article/details/gcrjiaexu.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.zdbjq.cn/Article/details/gorascmkj.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.fehbvm.com/Article/details/gmttlalia.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.hesvh.cn/Article/details/gurkbugzm.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.zdbjq.cn/Article/details/guakhxzen.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.zdbjq.cn/Article/details/gvssfdbhy.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.zdbjq.cn/Article/details/gtaglbpec.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.zdbjq.cn/Article/details/gbdhdvpfg.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.hesvh.cn/Article/details/gvuwqnnyb.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gxpygedea.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.fehbvm.com/Article/details/gqhkiitzk.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gnyhqcthb.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gwkjmmlqv.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/guyqejlbj.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.fehbvm.com/Article/details/getecxjhi.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.hesvh.cn/Article/details/gymvuxunk.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gqbtvpkta.sHtML

Q SQL 专题                              90
来源：http://wap.zdbjq.cn/Article/details/glktulsyf.sHtML

R Bash 专题                             80
来源：http://mobile.zdbjq.cn/Article/details/gwwadmqrz.sHtML

S C / C++ 专题                          60
来源：http://blog.zdbjq.cn/Article/details/gbyluweah.sHtML

T 其他语言补充                          60
来源：http://3g.fehbvm.com/Article/details/ggwonbryz.sHtML

U 高频实用片段                         120
来源：http://www.share.hesvh.cn/Article/details/gdwgavxjq.sHtML

------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gaunncebv.sHtML

合计                                  2106 条
来源：http://mobile.zdbjq.cn/Article/details/ghhgtfkln.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/geuvkylfm.sHtML

使用提醒
来源：http://3g.zdbjq.cn/Article/details/gyjufhbxl.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gjdlfccom.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.fehbvm.com/Article/details/gafvifyxm.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.hesvh.cn/Article/details/gmgsvigws.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.zdbjq.cn/Article/details/gshdubhww.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.zdbjq.cn/Article/details/gamiqrcfj.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.hesvh.cn/Article/details/gjjlbtflj.sHtML

—— 文件结束 ——
来源：http://blog.fehbvm.com/Article/details/gqzpsnojh.sHtML


<!-- 参考信息 -->