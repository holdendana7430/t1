代发 wailian999

[U05] Py：列表去重且保序
来源：http://blog.fanxiaobao.xyz/Article/details/gtwaguhmm.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.fanxiaobao.xyz/Article/details/gifmophwc.sHtML

[U06] Py：合并两个字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gnvicbtsa.sHtML

{**a, **b}
来源：http://mobile.fanxiaobao.xyz/Article/details/gpnemriyo.sHtML

[U07] Py：反转字典键值
来源：http://www.share.fanxiaobao.xyz/Article/details/gmtmlrrrn.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gemacbakn.sHtML

[U08] Py：展平二维列表
来源：http://mobile.fanxiaobao.xyz/Article/details/gxvqxxsmk.sHtML

[y for x in nested for y in x]
来源：http://mobile.fanxiaobao.xyz/Article/details/gredjyrxr.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.fanxiaobao.xyz/Article/details/gixkyerjn.sHtML

max(d, key=d.get)
来源：http://mobile.fanxiaobao.xyz/Article/details/giwvekogz.sHtML

[U10] Py：按值排序字典
来源：http://3g.fanxiaobao.xyz/Article/details/gcmedvnhk.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.fanxiaobao.xyz/Article/details/ggylcgecn.sHtML

[U11] Py：生成器表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gwehovfxy.sHtML

(x * 2 for x in arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gmzqgsnlo.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxsjzbqju.sHtML

Counter(arr).most_common(3)
来源：http://baike.fanxiaobao.xyz/Article/details/glbkxjxfu.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcvuxbkef.sHtML

deque(maxlen=10)
来源：http://wap.fanxiaobao.xyz/Article/details/gjbcuhyrc.sHtML

[U14] Py：分组收集到列表
来源：http://wap.fanxiaobao.xyz/Article/details/gngfexvpi.sHtML

defaultdict(list)
来源：http://wap.fanxiaobao.xyz/Article/details/gnrhgfqts.sHtML

[U15] Py：高精度计时
来源：http://m.share.fanxiaobao.xyz/Article/details/gceqjjdaq.sHtML

t = time.perf_counter()
来源：http://3g.fanxiaobao.xyz/Article/details/gsmjaernc.sHtML

[U16] Py：命令行参数解析
来源：http://3g.fanxiaobao.xyz/Article/details/gcwhuqntw.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gleplthhd.sHtML

[U17] Py：初始化日志
来源：http://baike.fanxiaobao.xyz/Article/details/gyciwfbyn.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.fanxiaobao.xyz/Article/details/gkjirvgaj.sHtML

[U18] Py：预编译正则
来源：http://wap.fanxiaobao.xyz/Article/details/gpdsonnoz.sHtML

pat = re.compile(r"\d+")
来源：http://baike.fanxiaobao.xyz/Article/details/glwphytmh.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.fanxiaobao.xyz/Article/details/gycoqpjpf.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfdrgnrfc.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.fanxiaobao.xyz/Article/details/gbprmohxq.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyhslvcly.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.fanxiaobao.xyz/Article/details/gcuaznlsa.sHtML

@contextlib.contextmanager
来源：http://mobile.fanxiaobao.xyz/Article/details/gafjxmbtq.sHtML

[U22] Py：矩阵转置
来源：http://m.share.fanxiaobao.xyz/Article/details/gytfadept.sHtML

list(zip(*m))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdwktpzja.sHtML

[U23] Py：分块读取大文件
来源：http://3g.fanxiaobao.xyz/Article/details/gziaybmou.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.fanxiaobao.xyz/Article/details/gygrrrmly.sHtML

[U24] Py：路径操作
来源：http://blog.fanxiaobao.xyz/Article/details/gnnfxiqxy.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjxcrwyka.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.fanxiaobao.xyz/Article/details/grdmiutpg.sHtML

csv.DictReader(f)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvusizhqg.sHtML

[U26] Py：并发下载
来源：http://m.share.fanxiaobao.xyz/Article/details/ggqkgpreg.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyafvutvu.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gexzrjnfw.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.fanxiaobao.xyz/Article/details/ggnsxorzw.sHtML

[U28] Py：类型别名
来源：http://read.share.fanxiaobao.xyz/Article/details/gpncezhaz.sHtML

UserId = int
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjitqfvny.sHtML

[U29] Py：属性校验
来源：http://wap.fanxiaobao.xyz/Article/details/gyusnhsnu.sHtML

@property 与 @x.setter 配合
来源：http://mobile.fanxiaobao.xyz/Article/details/gsigkrvfk.sHtML

[U30] Py：数据类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/getrxrvmu.sHtML

@dataclass(slots=True)
来源：http://baike.fanxiaobao.xyz/Article/details/gocrevkvj.sHtML

[U31] Py：单测
来源：http://blog.fanxiaobao.xyz/Article/details/ghwxpznfn.sHtML

python -m pytest -q
来源：http://www.blog.fanxiaobao.xyz/Article/details/guddvyeng.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjpmnvvsf.sHtML

ruff format . && ruff check --fix .
来源：http://wap.fanxiaobao.xyz/Article/details/gpieowsuy.sHtML

[U33] Py：打包发布
来源：http://baike.fanxiaobao.xyz/Article/details/geuogdnkr.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.fanxiaobao.xyz/Article/details/gezzuazmo.sHtML

[U34] Py：判断编码
来源：http://blog.fanxiaobao.xyz/Article/details/gbxlvwjbt.sHtML

chardet.detect(raw)
来源：http://3g.fanxiaobao.xyz/Article/details/ggbhmunyo.sHtML

[U35] Py：发送邮件
来源：http://www.share.fanxiaobao.xyz/Article/details/gkmjobavb.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.fanxiaobao.xyz/Article/details/gghexlqnp.sHtML

[U36] Py：定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/guodyuvpx.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvvekxihf.sHtML

[U37] Py：读写 Excel
来源：http://mobile.fanxiaobao.xyz/Article/details/gfthwojyp.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.fanxiaobao.xyz/Article/details/gikcvggly.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.fanxiaobao.xyz/Article/details/gdsdrxexa.sHtML

Path(__file__).resolve().parent
来源：http://mobile.fanxiaobao.xyz/Article/details/gwkcjmplq.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.fanxiaobao.xyz/Article/details/gafefxapp.sHtML

sys.stdout.isatty()
来源：http://read.share.fanxiaobao.xyz/Article/details/gzwjawekj.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gorknkyox.sHtML

print("err", file=sys.stderr)
来源：http://3g.fanxiaobao.xyz/Article/details/ggabefywr.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.fanxiaobao.xyz/Article/details/grxswhqfl.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.fanxiaobao.xyz/Article/details/gupvacvaa.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.fanxiaobao.xyz/Article/details/gcwzlcgsz.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gewsbcxjx.sHtML

[U43] PHP：声明命名空间
来源：http://wap.fanxiaobao.xyz/Article/details/ggmvrqvcr.sHtML

namespace App\Http;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvqecsgsk.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gredjawen.sHtML

declare(strict_types=1);
来源：http://wap.fanxiaobao.xyz/Article/details/gigpnfcea.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gkzsxnfyg.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gxmvzgsvn.sHtML

[U46] PHP：可空类型
来源：http://blog.fanxiaobao.xyz/Article/details/gtfhtqrug.sHtML

?string $name = null
来源：http://3g.fanxiaobao.xyz/Article/details/gdzpayjcd.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjouambmw.sHtML

int|string $id
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjdathjur.sHtML

[U48] PHP：纯枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/ghaquczwm.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grpdpttvv.sHtML

[U49] PHP：只读属性
来源：http://blog.fanxiaobao.xyz/Article/details/gtrainpts.sHtML

public readonly string $name
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfuidbcrc.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.fanxiaobao.xyz/Article/details/glukycyfs.sHtML

public function __construct(private int $id) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gedknehil.sHtML

[U51] PHP：数组解构
来源：http://m.share.fanxiaobao.xyz/Article/details/gcscrraky.sHtML

[$a, $b] = $arr;
来源：http://blog.fanxiaobao.xyz/Article/details/gxjbharad.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxenrcwgc.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmegkxxtw.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.fanxiaobao.xyz/Article/details/gjocujygo.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.fanxiaobao.xyz/Article/details/gdnzrxqwq.sHtML

[U54] PHP：空安全调用
来源：http://3g.fanxiaobao.xyz/Article/details/gyeosaeqo.sHtML

$obj?->method()
来源：http://baike.fanxiaobao.xyz/Article/details/gcishpihh.sHtML

[U55] PHP：match 表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gxdwgdfqa.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.fanxiaobao.xyz/Article/details/gsprqsjhy.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giqfjcxxo.sHtML

f(a: 1, b: 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gycbulccf.sHtML

[U57] PHP：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gvyhglusb.sHtML

"值: {$a}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkneqbrji.sHtML

[U58] PHP：数组三件套
来源：http://read.share.fanxiaobao.xyz/Article/details/gafyqjzef.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqllqoyqy.sHtML

[U59] PHP：自定义排序
来源：http://wap.fanxiaobao.xyz/Article/details/gugjvluha.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fanxiaobao.xyz/Article/details/glxgueepe.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.fanxiaobao.xyz/Article/details/gsnpybokf.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.fanxiaobao.xyz/Article/details/ghpcyhugb.sHtML

[U61] PHP：正则
来源：http://blog.fanxiaobao.xyz/Article/details/gwqowftjk.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fanxiaobao.xyz/Article/details/gfesuoyrp.sHtML

[U62] PHP：日期对象
来源：http://www.blog.fanxiaobao.xyz/Article/details/grheqhigx.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.fanxiaobao.xyz/Article/details/gurpqbnmj.sHtML

[U63] PHP：文件读写
来源：http://blog.fanxiaobao.xyz/Article/details/gnidozydb.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtkcyzxiv.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaeravdkw.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbfofbhzt.sHtML

[U65] PHP：会话
来源：http://mobile.fanxiaobao.xyz/Article/details/gdcnjibun.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmibmpfwd.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.fanxiaobao.xyz/Article/details/gbqfqwiqm.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjrrkuipz.sHtML

[U67] PHP：处理文件上传
来源：http://baike.fanxiaobao.xyz/Article/details/gdjeerffi.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.fanxiaobao.xyz/Article/details/gkbztfvwr.sHtML

[U68] PHP：PDO 连接
来源：http://3g.fanxiaobao.xyz/Article/details/ghmwfkkwq.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqpdkjrui.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gnutahmyi.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.fanxiaobao.xyz/Article/details/gmxanmoeq.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gienuvbse.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.fanxiaobao.xyz/Article/details/grsbxdkke.sHtML

[U71] PHP：抛出异常
来源：http://mobile.fanxiaobao.xyz/Article/details/gpkwnwqtw.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.fanxiaobao.xyz/Article/details/glmxxaxgn.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsimezxzx.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.fanxiaobao.xyz/Article/details/glcclpayc.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.fanxiaobao.xyz/Article/details/gcgjirnss.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.fanxiaobao.xyz/Article/details/geofdbetc.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gbdaxlorf.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.fanxiaobao.xyz/Article/details/gtyeiitir.sHtML

[U75] PHP：依赖注入
来源：http://www.share.fanxiaobao.xyz/Article/details/gqhrmjxhf.sHtML

composer require psr/container
来源：http://read.share.fanxiaobao.xyz/Article/details/gbtdfzykr.sHtML

[U76] PHP：简单路由
来源：http://mobile.fanxiaobao.xyz/Article/details/gofjfxiur.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.fanxiaobao.xyz/Article/details/gvvbkjnxk.sHtML

[U77] PHP：模板渲染
来源：http://read.share.fanxiaobao.xyz/Article/details/gmuovauqc.sHtML

composer require twig/twig
来源：http://read.share.fanxiaobao.xyz/Article/details/gbfocvhbo.sHtML

[U78] PHP：单元测试
来源：http://read.share.fanxiaobao.xyz/Article/details/gtptvkxpk.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghncywuzq.sHtML

[U79] PHP：静态分析
来源：http://read.share.fanxiaobao.xyz/Article/details/goxmbtbhf.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.fanxiaobao.xyz/Article/details/gejzlyjjt.sHtML

[U80] PHP：代码规范修复
来源：http://baike.fanxiaobao.xyz/Article/details/gsynckujj.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxxxnjtgr.sHtML

[U81] JS：初始化项目
来源：http://www.share.fanxiaobao.xyz/Article/details/guydxmehw.sHtML

npm init -y;  npm i express
来源：http://3g.fanxiaobao.xyz/Article/details/gjrlyvcjw.sHtML

[U82] JS：package.json 脚本
来源：http://blog.fanxiaobao.xyz/Article/details/gwuqkwwce.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwtgflfgi.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.fanxiaobao.xyz/Article/details/gfxgkkcga.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.fanxiaobao.xyz/Article/details/gmuyhfjqe.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.fanxiaobao.xyz/Article/details/gwdhbypob.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.fanxiaobao.xyz/Article/details/gcqsnzrbf.sHtML

[U85] JS：可选链
来源：http://m.share.fanxiaobao.xyz/Article/details/gnpykftou.sHtML

a?.b?.c
来源：http://www.share.fanxiaobao.xyz/Article/details/gwuwyqlsp.sHtML

[U86] JS：空值合并
来源：http://read.share.fanxiaobao.xyz/Article/details/gsvtmiylj.sHtML

a ?? b
来源：http://baike.fanxiaobao.xyz/Article/details/ggusehukm.sHtML

[U87] JS：解构默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/gfrxwkihx.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.fanxiaobao.xyz/Article/details/gupdlegop.sHtML

[U88] JS：对象展开合并
来源：http://mobile.fanxiaobao.xyz/Article/details/gzlmkhojo.sHtML

{ ...a, ...b }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gegyfaipc.sHtML

[U89] JS：数组去重
来源：http://m.share.fanxiaobao.xyz/Article/details/grvefrnkq.sHtML

[...new Set(arr)]
来源：http://3g.fanxiaobao.xyz/Article/details/gvpnzqzhb.sHtML

[U90] JS：数字数组排序
来源：http://3g.fanxiaobao.xyz/Article/details/gasrclgrz.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmbnxdwgj.sHtML

[U91] JS：对象键值遍历
来源：http://3g.fanxiaobao.xyz/Article/details/ghienamwk.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.fanxiaobao.xyz/Article/details/galhrzicq.sHtML

[U92] JS：深拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gjrjcptfm.sHtML

structuredClone(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/gnvfsxdnl.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkmisbzfa.sHtML

`共 ${n} 条`
来源：http://wap.fanxiaobao.xyz/Article/details/goqyyjniz.sHtML

[U94] JS：箭头函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gvagmphyn.sHtML

const double = x => x * 2;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gosmkkwet.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvartvgte.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.fanxiaobao.xyz/Article/details/gtwzztkyp.sHtML

[U96] JS：async/await 与异常
来源：http://wap.fanxiaobao.xyz/Article/details/gublyxpqf.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.fanxiaobao.xyz/Article/details/gjvzfusza.sHtML

[U97] JS：并发请求
来源：http://m.share.fanxiaobao.xyz/Article/details/grsnliyhz.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fanxiaobao.xyz/Article/details/gbvjbkkps.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/ghyslgufo.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcgztejbc.sHtML

[U99] JS：事件监听
来源：http://blog.fanxiaobao.xyz/Article/details/gvibdfobm.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.fanxiaobao.xyz/Article/details/gpxisdvho.sHtML

[U100] JS：DOM 查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gfxdjbdvj.sHtML

document.querySelector(".item")
来源：http://3g.fanxiaobao.xyz/Article/details/gbebzpgno.sHtML

[U101] JS：classList 操作
来源：http://wap.fanxiaobao.xyz/Article/details/gimnqjgsb.sHtML

el.classList.toggle("active")
来源：http://m.share.fanxiaobao.xyz/Article/details/gxlrpxrxa.sHtML

[U102] JS：本地存储
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpawaeflt.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.fanxiaobao.xyz/Article/details/gwxhxfxrs.sHtML

[U103] JS：定时器
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyuldhped.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.fanxiaobao.xyz/Article/details/gwxzrwkmx.sHtML

[U104] JS：防抖
来源：http://baike.fanxiaobao.xyz/Article/details/glhhwvfgb.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fanxiaobao.xyz/Article/details/gadqyipvo.sHtML

[U105] JS：节流
来源：http://blog.fanxiaobao.xyz/Article/details/gxevuocpt.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.fanxiaobao.xyz/Article/details/glyicxmdg.sHtML

[U106] JS：日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gjqftcedy.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfzevxdke.sHtML

[U107] JS：数字千分位
来源：http://m.share.fanxiaobao.xyz/Article/details/genzqkuir.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvnvoidpw.sHtML

[U108] JS：随机整数
来源：http://3g.fanxiaobao.xyz/Article/details/gmycalmec.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.fanxiaobao.xyz/Article/details/giexvcimw.sHtML

[U109] JS：数组分组
来源：http://wap.fanxiaobao.xyz/Article/details/gfshaxcve.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.fanxiaobao.xyz/Article/details/gunywbxve.sHtML

[U110] JS：数组分块
来源：http://m.share.fanxiaobao.xyz/Article/details/gvngsbszk.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.fanxiaobao.xyz/Article/details/gclzdchqg.sHtML

[U111] JS：对象转 Map
来源：http://3g.fanxiaobao.xyz/Article/details/grldsplbg.sHtML

new Map(Object.entries(obj))
来源：http://m.share.fanxiaobao.xyz/Article/details/gwejpinpc.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gggyaconm.sHtML

"7".padStart(3, "0")
来源：http://read.share.fanxiaobao.xyz/Article/details/gyvdzwokj.sHtML

[U113] JS：正则替换全部
来源：http://blog.fanxiaobao.xyz/Article/details/gcetdnoog.sHtML

s.replaceAll("a", "b")
来源：http://mobile.fanxiaobao.xyz/Article/details/gewefvgmn.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkeezkufy.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fanxiaobao.xyz/Article/details/gfqvwmbqr.sHtML

[U115] JS：生成 UUID
来源：http://www.share.fanxiaobao.xyz/Article/details/gzmuxlhmb.sHtML

crypto.randomUUID()
来源：http://blog.fanxiaobao.xyz/Article/details/gsvpqhewq.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.fanxiaobao.xyz/Article/details/gzrrhelzr.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gxgzymwtz.sHtML

[U117] JS：单元测试
来源：http://baike.fanxiaobao.xyz/Article/details/gxkptgrks.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glxbijrow.sHtML

[U118] JS：开发服务器
来源：http://mobile.fanxiaobao.xyz/Article/details/gaocgqjva.sHtML

npm i -D vite;  npx vite
来源：http://read.share.fanxiaobao.xyz/Article/details/gsiabpqyx.sHtML

[U119] JS：生产构建
来源：http://3g.fanxiaobao.xyz/Article/details/gbumvqxyq.sHtML

npx vite build
来源：http://mobile.fanxiaobao.xyz/Article/details/gyyixkmfp.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfctafpse.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.fanxiaobao.xyz/Article/details/gwcqgqlus.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gwkvowewr.sHtML

统计汇总
来源：http://read.share.fanxiaobao.xyz/Article/details/gjblhhrpw.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmjhwfzgk.sHtML

按语言统计（条）：
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmhqalzdt.sHtML

Python ......... 252
来源：http://wap.fanxiaobao.xyz/Article/details/gvwfsiply.sHtML

PHP ............ 252
来源：http://www.share.fanxiaobao.xyz/Article/details/giyoookwq.sHtML

JavaScript ..... 252
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnhoebhlq.sHtML

TypeScript ..... 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbexrvjro.sHtML

Java ........... 212
来源：http://baike.fanxiaobao.xyz/Article/details/goqzyouhh.sHtML

Go ............. 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gcuqyiyeo.sHtML

Ruby ........... 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gkoyuzcfj.sHtML

C# ............. 212
来源：http://3g.fanxiaobao.xyz/Article/details/grhrscuda.sHtML

C .............. 30
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glvlhzyny.sHtML

C++ ............ 30
来源：http://mobile.fanxiaobao.xyz/Article/details/gjhcdaukk.sHtML

SQL ............ 90
来源：http://3g.fanxiaobao.xyz/Article/details/geybalxvc.sHtML

Bash ........... 80
来源：http://m.share.fanxiaobao.xyz/Article/details/gcpznwtyb.sHtML

Kotlin ......... 15
来源：http://3g.fanxiaobao.xyz/Article/details/gynbymbdd.sHtML

Swift .......... 15
来源：http://read.share.fanxiaobao.xyz/Article/details/gdnvjrztx.sHtML

Lua ............ 10
来源：http://mobile.fanxiaobao.xyz/Article/details/gcqrtsgsj.sHtML

Perl ........... 10
来源：http://3g.fanxiaobao.xyz/Article/details/gdbalnyjh.sHtML

Scala .......... 10
来源：http://m.share.fanxiaobao.xyz/Article/details/gwuaudmer.sHtML

------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/gbwcvohkv.sHtML

合计 ........... 2106 条
来源：http://m.share.fanxiaobao.xyz/Article/details/gnuqqetcx.sHtML

按章节统计：
来源：http://baike.fanxiaobao.xyz/Article/details/gfnqdmhuh.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.fanxiaobao.xyz/Article/details/gpkvtmuzf.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsfnnvyex.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpsgxqbtg.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.fanxiaobao.xyz/Article/details/gzicflncf.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvzcgzfra.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.fanxiaobao.xyz/Article/details/gjttnckji.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.fanxiaobao.xyz/Article/details/gzegxjfrr.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.fanxiaobao.xyz/Article/details/gwyeopmyg.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpqyhjpiz.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.fanxiaobao.xyz/Article/details/gfjybaxjg.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/gqjhqzwlj.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggyveghon.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/goepulkle.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmorktwzq.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.fanxiaobao.xyz/Article/details/ggqgrycka.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmtvqxslg.sHtML

Q SQL 专题                              90
来源：http://www.share.fanxiaobao.xyz/Article/details/grvzuvkil.sHtML

R Bash 专题                             80
来源：http://www.share.fanxiaobao.xyz/Article/details/grvjgfarz.sHtML

S C / C++ 专题                          60
来源：http://blog.fanxiaobao.xyz/Article/details/ggrnznmcq.sHtML

T 其他语言补充                          60
来源：http://blog.fanxiaobao.xyz/Article/details/gcmiyxghs.sHtML

U 高频实用片段                         120
来源：http://mobile.fanxiaobao.xyz/Article/details/gwlpcfjky.sHtML

------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/ggvjbxlcz.sHtML

合计                                  2106 条
来源：http://mobile.fanxiaobao.xyz/Article/details/gpnfmtnpb.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/gkozmqpvx.sHtML

使用提醒
来源：http://3g.fanxiaobao.xyz/Article/details/gbxrlxdgw.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/gbxdhgoed.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.fanxiaobao.xyz/Article/details/gyznklvgx.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.fanxiaobao.xyz/Article/details/giihlbfmu.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.fanxiaobao.xyz/Article/details/grdqdqsxe.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.fanxiaobao.xyz/Article/details/gdnwcorut.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.fanxiaobao.xyz/Article/details/goxfbqbnb.sHtML

—— 文件结束 ——
来源：http://3g.fanxiaobao.xyz/Article/details/glwuuiokl.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gfdqiwlmx.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtzjumcud.sHtML

Common Programming Examples Cheat Book
来源：http://wap.fanxiaobao.xyz/Article/details/gkveikrhk.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gxdvwggcs.sHtML

【收录内容】
来源：http://blog.fanxiaobao.xyz/Article/details/gtwnzvmsd.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjshphytz.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqzdqohrt.sHtML

SQL · Bash · C · C++
来源：http://blog.fanxiaobao.xyz/Article/details/gthwugxta.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.fanxiaobao.xyz/Article/details/glcdptalx.sHtML

【使用说明】
来源：http://3g.fanxiaobao.xyz/Article/details/glbijvvbx.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.fanxiaobao.xyz/Article/details/gpclumrwy.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.fanxiaobao.xyz/Article/details/glegernyr.sHtML


<!-- 参考信息 -->