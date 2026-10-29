代发 wailian999

[U03] Py：加载 .env 配置
来源：http://baike.zdbjq.cn/Article/details/gdmaklgdu.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.zdbjq.cn/Article/details/gkmveffcl.sHtML

[U04] Py：变量调试打印
来源：http://m.share.fehbvm.com/Article/details/gkozxolpm.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.zdbjq.cn/Article/details/gwzkrcxcx.sHtML

[U05] Py：列表去重且保序
来源：http://3g.zdbjq.cn/Article/details/gxnepmytu.sHtML

list(dict.fromkeys(arr))
来源：http://baike.fehbvm.com/Article/details/gogqupmle.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fehbvm.com/Article/details/gpaggtlom.sHtML

{**a, **b}
来源：http://blog.fehbvm.com/Article/details/gkphvgkzf.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.hesvh.cn/Article/details/gcvsqdiye.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.hesvh.cn/Article/details/grueruvgf.sHtML

[U08] Py：展平二维列表
来源：http://3g.fehbvm.com/Article/details/gsbicwvaz.sHtML

[y for x in nested for y in x]
来源：http://wap.hesvh.cn/Article/details/glgrsgbng.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.zdbjq.cn/Article/details/gjbznwtaj.sHtML

max(d, key=d.get)
来源：http://read.share.hesvh.cn/Article/details/gszrkuajo.sHtML

[U10] Py：按值排序字典
来源：http://blog.zdbjq.cn/Article/details/grnyiwbsq.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.fehbvm.com/Article/details/gsoohbccz.sHtML

[U11] Py：生成器表达式
来源：http://read.share.zdbjq.cn/Article/details/gyoaysadj.sHtML

(x * 2 for x in arr)
来源：http://3g.hesvh.cn/Article/details/gqwijebna.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.fehbvm.com/Article/details/gvfgoitfc.sHtML

Counter(arr).most_common(3)
来源：http://baike.fehbvm.com/Article/details/gxrcyikov.sHtML

[U13] Py：固定长度队列
来源：http://3g.zdbjq.cn/Article/details/gcespuwzd.sHtML

deque(maxlen=10)
来源：http://wap.zdbjq.cn/Article/details/gjdngdmsw.sHtML

[U14] Py：分组收集到列表
来源：http://3g.hesvh.cn/Article/details/gqbkgfisf.sHtML

defaultdict(list)
来源：http://read.share.hesvh.cn/Article/details/gpwtxqljo.sHtML

[U15] Py：高精度计时
来源：http://m.share.fehbvm.com/Article/details/gtztncjyt.sHtML

t = time.perf_counter()
来源：http://wap.hesvh.cn/Article/details/gfeufqaqf.sHtML

[U16] Py：命令行参数解析
来源：http://wap.zdbjq.cn/Article/details/gyvfjjatq.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.zdbjq.cn/Article/details/ghwyfppiq.sHtML

[U17] Py：初始化日志
来源：http://mobile.zdbjq.cn/Article/details/gpbswxxms.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.zdbjq.cn/Article/details/gdqzrngyl.sHtML

[U18] Py：预编译正则
来源：http://wap.fehbvm.com/Article/details/ggwgaxrup.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.zdbjq.cn/Article/details/gzzkbrcko.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.zdbjq.cn/Article/details/gernpzqxl.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fehbvm.com/Article/details/guvingrds.sHtML

[U20] Py：缓存函数结果
来源：http://baike.fehbvm.com/Article/details/gdhhcupuu.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.hesvh.cn/Article/details/gqdbgddhu.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.fehbvm.com/Article/details/gegbhtmnv.sHtML

@contextlib.contextmanager
来源：http://m.share.fehbvm.com/Article/details/gxhlzozis.sHtML

[U22] Py：矩阵转置
来源：http://wap.hesvh.cn/Article/details/gmwdqsisg.sHtML

list(zip(*m))
来源：http://www.share.fehbvm.com/Article/details/gicliwotu.sHtML

[U23] Py：分块读取大文件
来源：http://wap.hesvh.cn/Article/details/gyuwdvehy.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.hesvh.cn/Article/details/gccihpneh.sHtML

[U24] Py：路径操作
来源：http://baike.fehbvm.com/Article/details/gprbrmrvk.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.zdbjq.cn/Article/details/gujmvmtdq.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.hesvh.cn/Article/details/goturjujo.sHtML

csv.DictReader(f)
来源：http://baike.hesvh.cn/Article/details/gddlyowpv.sHtML

[U26] Py：并发下载
来源：http://read.share.zdbjq.cn/Article/details/goixjtcwm.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.zdbjq.cn/Article/details/gvwabcceu.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.zdbjq.cn/Article/details/gnaaxvtme.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.fehbvm.com/Article/details/gqlacgssb.sHtML

[U28] Py：类型别名
来源：http://www.m.share.zdbjq.cn/Article/details/gctzvzsst.sHtML

UserId = int
来源：http://www.blog.zdbjq.cn/Article/details/gacwchawm.sHtML

[U29] Py：属性校验
来源：http://mobile.zdbjq.cn/Article/details/gylndqryy.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.fehbvm.com/Article/details/ghvpqbfow.sHtML

[U30] Py：数据类
来源：http://blog.zdbjq.cn/Article/details/glystvgnb.sHtML

@dataclass(slots=True)
来源：http://wap.fehbvm.com/Article/details/gdafzihzc.sHtML

[U31] Py：单测
来源：http://read.share.fehbvm.com/Article/details/gaxzazuae.sHtML

python -m pytest -q
来源：http://www.m.share.fehbvm.com/Article/details/grtdlweio.sHtML

[U32] Py：代码格式化
来源：http://wap.hesvh.cn/Article/details/gxutkepyz.sHtML

ruff format . && ruff check --fix .
来源：http://baike.zdbjq.cn/Article/details/geywferqr.sHtML

[U33] Py：打包发布
来源：http://www.share.hesvh.cn/Article/details/gcwxtdbmr.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.fehbvm.com/Article/details/gfrctaqec.sHtML

[U34] Py：判断编码
来源：http://www.blog.zdbjq.cn/Article/details/gsvzutbas.sHtML

chardet.detect(raw)
来源：http://3g.zdbjq.cn/Article/details/gqzorqcue.sHtML

[U35] Py：发送邮件
来源：http://www.share.fehbvm.com/Article/details/gwonchrxs.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.zdbjq.cn/Article/details/gywzbhhaz.sHtML

[U36] Py：定时任务
来源：http://mobile.zdbjq.cn/Article/details/gurvyzkcr.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.zdbjq.cn/Article/details/gwwccrwoq.sHtML

[U37] Py：读写 Excel
来源：http://wap.fehbvm.com/Article/details/gubicgvkf.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.hesvh.cn/Article/details/gdxszeprm.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.zdbjq.cn/Article/details/gbaxelfcq.sHtML

Path(__file__).resolve().parent
来源：http://mobile.zdbjq.cn/Article/details/gptgmcpah.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.hesvh.cn/Article/details/gsobawgsz.sHtML

sys.stdout.isatty()
来源：http://baike.hesvh.cn/Article/details/gbrvzbpnu.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.fehbvm.com/Article/details/gporlpsba.sHtML

print("err", file=sys.stderr)
来源：http://3g.fehbvm.com/Article/details/gvzkrpaej.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.hesvh.cn/Article/details/gzqqwngex.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.fehbvm.com/Article/details/gtrcpxhtt.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.zdbjq.cn/Article/details/gjcnlgjec.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.zdbjq.cn/Article/details/ggaeqzyfz.sHtML

[U43] PHP：声明命名空间
来源：http://baike.zdbjq.cn/Article/details/gynuoxnuj.sHtML

namespace App\Http;
来源：http://baike.hesvh.cn/Article/details/gcewfbhim.sHtML

[U44] PHP：开启严格类型
来源：http://3g.fehbvm.com/Article/details/gquutisml.sHtML

declare(strict_types=1);
来源：http://www.blog.zdbjq.cn/Article/details/ggjotemjg.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.fehbvm.com/Article/details/gigcyvcvw.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gxuwclmia.sHtML

[U46] PHP：可空类型
来源：http://baike.fehbvm.com/Article/details/gpawiqhbs.sHtML

?string $name = null
来源：http://www.m.share.zdbjq.cn/Article/details/gvmfhnmac.sHtML

[U47] PHP：联合类型
来源：http://read.share.fehbvm.com/Article/details/gtriydwar.sHtML

int|string $id
来源：http://www.share.hesvh.cn/Article/details/gvqwvxghr.sHtML

[U48] PHP：纯枚举
来源：http://baike.zdbjq.cn/Article/details/gucadfgfr.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.fehbvm.com/Article/details/giaxyteei.sHtML

[U49] PHP：只读属性
来源：http://www.share.fehbvm.com/Article/details/gdevqsnqh.sHtML

public readonly string $name
来源：http://www.share.hesvh.cn/Article/details/gegbjijed.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.hesvh.cn/Article/details/ghnzoccxn.sHtML

public function __construct(private int $id) {}
来源：http://www.share.zdbjq.cn/Article/details/gqejlmqtm.sHtML

[U51] PHP：数组解构
来源：http://3g.zdbjq.cn/Article/details/gzunjkzag.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.hesvh.cn/Article/details/gxnzbvrhy.sHtML

[U52] PHP：箭头函数
来源：http://m.share.hesvh.cn/Article/details/gegyqssly.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.fehbvm.com/Article/details/gjhejrguw.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.zdbjq.cn/Article/details/giehbgrts.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.hesvh.cn/Article/details/gighmwfht.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.hesvh.cn/Article/details/gtkrgkrpw.sHtML

$obj?->method()
来源：http://www.blog.hesvh.cn/Article/details/gmaamavcv.sHtML

[U55] PHP：match 表达式
来源：http://3g.fehbvm.com/Article/details/grjaqjygj.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.hesvh.cn/Article/details/gemsgnwyu.sHtML

[U56] PHP：命名参数
来源：http://read.share.zdbjq.cn/Article/details/gqdhqmxdh.sHtML

f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/gvphbtxkp.sHtML

[U57] PHP：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gxdfapbsn.sHtML

"值: {$a}"
来源：http://baike.zdbjq.cn/Article/details/graoyiaip.sHtML

[U58] PHP：数组三件套
来源：http://read.share.zdbjq.cn/Article/details/gcqwbhvyk.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.hesvh.cn/Article/details/gbnbnashy.sHtML

[U59] PHP：自定义排序
来源：http://3g.fehbvm.com/Article/details/grpktzahv.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.hesvh.cn/Article/details/gwyuehkwu.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.fehbvm.com/Article/details/gjdknhozi.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.zdbjq.cn/Article/details/glivcmbez.sHtML

[U61] PHP：正则
来源：http://www.blog.fehbvm.com/Article/details/gjebgyyao.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.hesvh.cn/Article/details/gkvbhwxvg.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.hesvh.cn/Article/details/greygebsi.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.zdbjq.cn/Article/details/gkdqfukqj.sHtML

[U63] PHP：文件读写
来源：http://read.share.fehbvm.com/Article/details/gqhtnvutr.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.zdbjq.cn/Article/details/gtjkokmcm.sHtML

[U64] PHP：目录遍历
来源：http://www.share.fehbvm.com/Article/details/gnefnoyhv.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.zdbjq.cn/Article/details/gltueywjf.sHtML

[U65] PHP：会话
来源：http://read.share.fehbvm.com/Article/details/gaoiplgzk.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.fehbvm.com/Article/details/ghgzwxjid.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.hesvh.cn/Article/details/gvxyokeqi.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.zdbjq.cn/Article/details/gjvesfhai.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.fehbvm.com/Article/details/gshhcjccg.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.zdbjq.cn/Article/details/gvbsvdgki.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.fehbvm.com/Article/details/gzvniorue.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.fehbvm.com/Article/details/gsvrixzok.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.zdbjq.cn/Article/details/gbdzvkvpe.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.hesvh.cn/Article/details/gtxxcbhxp.sHtML

[U70] PHP：PDO 事务
来源：http://blog.hesvh.cn/Article/details/ggvzskwkk.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.zdbjq.cn/Article/details/gknwzulvk.sHtML

[U71] PHP：抛出异常
来源：http://blog.fehbvm.com/Article/details/gbdztovgc.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.fehbvm.com/Article/details/gzaqiagir.sHtML

[U72] PHP：写错误日志
来源：http://baike.zdbjq.cn/Article/details/gpjupvnle.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.zdbjq.cn/Article/details/gmguagzwv.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.fehbvm.com/Article/details/gcrbvlnty.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.hesvh.cn/Article/details/gqlruiits.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.hesvh.cn/Article/details/gphqttnli.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.hesvh.cn/Article/details/gxiubygtb.sHtML

[U75] PHP：依赖注入
来源：http://m.share.fehbvm.com/Article/details/gxmchgemv.sHtML

composer require psr/container
来源：http://blog.zdbjq.cn/Article/details/gdjefxaqx.sHtML

[U76] PHP：简单路由
来源：http://m.share.fehbvm.com/Article/details/gubxitxkg.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.zdbjq.cn/Article/details/gvhdcbcud.sHtML

[U77] PHP：模板渲染
来源：http://m.share.hesvh.cn/Article/details/gtrrjlqbj.sHtML

composer require twig/twig
来源：http://www.blog.zdbjq.cn/Article/details/gjrkifest.sHtML

[U78] PHP：单元测试
来源：http://3g.zdbjq.cn/Article/details/ggvrvlgoq.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.fehbvm.com/Article/details/grcvujxxe.sHtML

[U79] PHP：静态分析
来源：http://baike.fehbvm.com/Article/details/gnisqdugy.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.fehbvm.com/Article/details/gwbjsyovy.sHtML

[U80] PHP：代码规范修复
来源：http://3g.hesvh.cn/Article/details/gdtqlrjuj.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.hesvh.cn/Article/details/gtplqzizx.sHtML

[U81] JS：初始化项目
来源：http://read.share.fehbvm.com/Article/details/gilkqgfqd.sHtML

npm init -y;  npm i express
来源：http://m.share.hesvh.cn/Article/details/gyuenyjbv.sHtML

[U82] JS：package.json 脚本
来源：http://wap.fehbvm.com/Article/details/gwuvztkax.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.hesvh.cn/Article/details/grrowqdpz.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.zdbjq.cn/Article/details/gaelylrnr.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.hesvh.cn/Article/details/gvyqbhcew.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.hesvh.cn/Article/details/gwqkauhbs.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.fehbvm.com/Article/details/gqwdwxrds.sHtML

[U85] JS：可选链
来源：http://blog.fehbvm.com/Article/details/gbvvygqoe.sHtML

a?.b?.c
来源：http://read.share.hesvh.cn/Article/details/gaxalavju.sHtML

[U86] JS：空值合并
来源：http://www.m.share.fehbvm.com/Article/details/gxzjgqgrd.sHtML

a ?? b
来源：http://blog.fehbvm.com/Article/details/gzbmjtume.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.hesvh.cn/Article/details/gznjfnulp.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.zdbjq.cn/Article/details/gtkzvghgo.sHtML

[U88] JS：对象展开合并
来源：http://m.share.zdbjq.cn/Article/details/gjlalgsdw.sHtML

{ ...a, ...b }
来源：http://www.blog.zdbjq.cn/Article/details/gfroajuny.sHtML

[U89] JS：数组去重
来源：http://blog.zdbjq.cn/Article/details/gbosxnjlm.sHtML

[...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/gqyrguqrq.sHtML

[U90] JS：数字数组排序
来源：http://3g.zdbjq.cn/Article/details/gpsjtiwqp.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/gftfsqwwz.sHtML

[U91] JS：对象键值遍历
来源：http://3g.fehbvm.com/Article/details/gzjpxmvfl.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.fehbvm.com/Article/details/ggbexvsre.sHtML

[U92] JS：深拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gknemjyaa.sHtML

structuredClone(obj)
来源：http://www.blog.hesvh.cn/Article/details/gwwynmehb.sHtML

[U93] JS：模板字符串
来源：http://www.blog.fehbvm.com/Article/details/gkecnledj.sHtML

`共 ${n} 条`
来源：http://blog.zdbjq.cn/Article/details/gwddpyisl.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.zdbjq.cn/Article/details/gjlhynkbr.sHtML

const double = x => x * 2;
来源：http://3g.fehbvm.com/Article/details/gfqwkitxq.sHtML

[U95] JS：Promise 包装
来源：http://m.share.fehbvm.com/Article/details/glojgjhow.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.hesvh.cn/Article/details/ghxcpdkln.sHtML

[U96] JS：async/await 与异常
来源：http://blog.fehbvm.com/Article/details/grotlrpfa.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gxdbjgzod.sHtML

[U97] JS：并发请求
来源：http://read.share.hesvh.cn/Article/details/gqnjivfht.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/ggidpqydx.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.fehbvm.com/Article/details/geqvwrdqp.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.zdbjq.cn/Article/details/glzzkrbay.sHtML

[U99] JS：事件监听
来源：http://mobile.hesvh.cn/Article/details/guyaaydmg.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.zdbjq.cn/Article/details/ghupxsxgb.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.hesvh.cn/Article/details/gotwjkjvm.sHtML

document.querySelector(".item")
来源：http://read.share.fehbvm.com/Article/details/gapuvasyv.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.zdbjq.cn/Article/details/gqybrtjoz.sHtML

el.classList.toggle("active")
来源：http://wap.hesvh.cn/Article/details/gwajivzvi.sHtML

[U102] JS：本地存储
来源：http://wap.zdbjq.cn/Article/details/ggfqwxjoh.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.zdbjq.cn/Article/details/gcyrcogvd.sHtML

[U103] JS：定时器
来源：http://baike.fehbvm.com/Article/details/gckznlwfu.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.zdbjq.cn/Article/details/gyiiqlndn.sHtML

[U104] JS：防抖
来源：http://wap.zdbjq.cn/Article/details/gpbpjvfmw.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/geelpjrlm.sHtML

[U105] JS：节流
来源：http://read.share.zdbjq.cn/Article/details/gruzngjhe.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gocwosdnt.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/glaxerchn.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.fehbvm.com/Article/details/galdcmbhv.sHtML

[U107] JS：数字千分位
来源：http://wap.hesvh.cn/Article/details/gcuoonwyx.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.hesvh.cn/Article/details/gmmhhyhaf.sHtML

[U108] JS：随机整数
来源：http://baike.zdbjq.cn/Article/details/ghrgeffde.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.fehbvm.com/Article/details/gcotnvkss.sHtML

[U109] JS：数组分组
来源：http://www.blog.zdbjq.cn/Article/details/gmfcznxee.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.hesvh.cn/Article/details/gcwvdqyjv.sHtML

[U110] JS：数组分块
来源：http://wap.fehbvm.com/Article/details/gesumyxky.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.zdbjq.cn/Article/details/gqjqkwuam.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.hesvh.cn/Article/details/gtxgwyrfi.sHtML

new Map(Object.entries(obj))
来源：http://blog.fehbvm.com/Article/details/ghwrajbvl.sHtML

[U112] JS：字符串补位
来源：http://wap.fehbvm.com/Article/details/gglfhbnig.sHtML

"7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/ghjbivvaw.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.fehbvm.com/Article/details/gnofcgjwf.sHtML

s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/ggljvwzbd.sHtML

[U114] JS：JSON 深比较
来源：http://3g.fehbvm.com/Article/details/gaybubzqc.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.zdbjq.cn/Article/details/ghijiiovc.sHtML

[U115] JS：生成 UUID
来源：http://wap.hesvh.cn/Article/details/gtkyiggmf.sHtML

crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/gaossmezj.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.fehbvm.com/Article/details/gnnpbxrpo.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.fehbvm.com/Article/details/gzghvkzip.sHtML

[U117] JS：单元测试
来源：http://m.share.zdbjq.cn/Article/details/gpuixjzjd.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.hesvh.cn/Article/details/gowubrpjj.sHtML

[U118] JS：开发服务器
来源：http://baike.hesvh.cn/Article/details/glsfoermg.sHtML

npm i -D vite;  npx vite
来源：http://read.share.zdbjq.cn/Article/details/gqoeopuow.sHtML

[U119] JS：生产构建
来源：http://www.m.share.fehbvm.com/Article/details/gxdrdbxtp.sHtML

npx vite build
来源：http://m.share.hesvh.cn/Article/details/gcuqezssx.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.zdbjq.cn/Article/details/gcwhadjla.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.fehbvm.com/Article/details/gduxoquxp.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gymqskssf.sHtML

统计汇总
来源：http://baike.hesvh.cn/Article/details/gplrrilge.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gfxedumty.sHtML

按语言统计（条）：
来源：http://read.share.hesvh.cn/Article/details/gcwzpqehs.sHtML

Python ......... 252
来源：http://m.share.fehbvm.com/Article/details/gxppraeie.sHtML

PHP ............ 252
来源：http://m.share.fehbvm.com/Article/details/gnogfhypn.sHtML

JavaScript ..... 252
来源：http://www.blog.hesvh.cn/Article/details/gmpinhjkt.sHtML

TypeScript ..... 212
来源：http://www.share.hesvh.cn/Article/details/gpgghopyq.sHtML

Java ........... 212
来源：http://www.share.hesvh.cn/Article/details/grhrxnfgq.sHtML

Go ............. 212
来源：http://3g.fehbvm.com/Article/details/gvbhwlewd.sHtML

Ruby ........... 212
来源：http://blog.fehbvm.com/Article/details/gbsxytmvf.sHtML

C# ............. 212
来源：http://www.m.share.zdbjq.cn/Article/details/gdbofpfwz.sHtML

C .............. 30
来源：http://read.share.hesvh.cn/Article/details/gfymuomxu.sHtML

C++ ............ 30
来源：http://www.m.share.fehbvm.com/Article/details/gzzzetrzf.sHtML

SQL ............ 90
来源：http://blog.hesvh.cn/Article/details/gprglkruu.sHtML

Bash ........... 80
来源：http://3g.fehbvm.com/Article/details/ggcguxdcm.sHtML

Kotlin ......... 15
来源：http://m.share.fehbvm.com/Article/details/gdmppzzzq.sHtML

Swift .......... 15
来源：http://www.blog.fehbvm.com/Article/details/gxhbygesx.sHtML

Lua ............ 10
来源：http://m.share.hesvh.cn/Article/details/gbadbqplz.sHtML

Perl ........... 10
来源：http://3g.hesvh.cn/Article/details/gkwtxallt.sHtML

Scala .......... 10
来源：http://m.share.hesvh.cn/Article/details/gvtdadouo.sHtML

------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gzqxdapic.sHtML

合计 ........... 2106 条
来源：http://read.share.zdbjq.cn/Article/details/giydqqwir.sHtML

按章节统计：
来源：http://baike.hesvh.cn/Article/details/gwczemmla.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.fehbvm.com/Article/details/gituuzoiv.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.hesvh.cn/Article/details/guufvusxi.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/gnnoqkzwo.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.hesvh.cn/Article/details/gerdcpixj.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.zdbjq.cn/Article/details/gamddrrva.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.hesvh.cn/Article/details/gitxyoylq.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/gwganxgay.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.hesvh.cn/Article/details/gfijqvjay.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/grfjorwsz.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.hesvh.cn/Article/details/gjtkdmvfu.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gvdbiaduz.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gotrptoqn.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/ghcsfdbvc.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.zdbjq.cn/Article/details/gitplbthk.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.hesvh.cn/Article/details/gpaqblapj.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gecaqdazs.sHtML

Q SQL 专题                              90
来源：http://m.share.hesvh.cn/Article/details/gjpvhpzdx.sHtML

R Bash 专题                             80
来源：http://wap.hesvh.cn/Article/details/gynkgnjoq.sHtML

S C / C++ 专题                          60
来源：http://www.blog.hesvh.cn/Article/details/gdotdoimb.sHtML

T 其他语言补充                          60
来源：http://baike.fehbvm.com/Article/details/gwcuprekh.sHtML

U 高频实用片段                         120
来源：http://baike.fehbvm.com/Article/details/gwcbmfewi.sHtML

------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gkldbxdkn.sHtML

合计                                  2106 条
来源：http://read.share.zdbjq.cn/Article/details/gkasavfin.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gzeddzwai.sHtML

使用提醒
来源：http://www.m.share.fehbvm.com/Article/details/grmdvqcgf.sHtML

--------------------------------------------------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gtvsnyojs.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.fehbvm.com/Article/details/gcbqtgwij.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.hesvh.cn/Article/details/gwsbkmtcs.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.hesvh.cn/Article/details/gubqthazo.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.hesvh.cn/Article/details/guebbymti.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.fehbvm.com/Article/details/gffcquyyy.sHtML

—— 文件结束 ——
来源：http://3g.zdbjq.cn/Article/details/godeupdim.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gentszqbo.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.hesvh.cn/Article/details/gsypbtmii.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.zdbjq.cn/Article/details/gluauaxzd.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gyowngubf.sHtML

【收录内容】
来源：http://mobile.fehbvm.com/Article/details/gvdzyrquq.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.hesvh.cn/Article/details/graidnohg.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.hesvh.cn/Article/details/gihxtmptc.sHtML

SQL · Bash · C · C++
来源：http://wap.hesvh.cn/Article/details/gzdicmgek.sHtML


<!-- 参考信息 -->