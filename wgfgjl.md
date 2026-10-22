代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fwmsiptp.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2hkthjxvl.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2trabxksq.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2tilkgwst.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2jptqfelm.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ychbjmmt.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2mdplbuxh.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2afvyfabi.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2hobvwsdo.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2bxzcqhdy.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2nlondrae.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2rgucvhqe.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2ntdyprlz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rgufcaaw.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mylktyxs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gjdkcolw.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2jsilugbg.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2hktpbrdu.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2urjfjafk.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2sixmsgpz.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2taakkfzw.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2nhomprxp.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2eiczmypr.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2bbecuolf.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2jbcxbwtv.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2mvkczncd.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2qbpgywhr.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2edygftxh.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2tohkpsiw.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2nlbesycz.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2psaatwwe.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2ankdgnic.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2yszvkelu.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2cqbjcvbi.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2mjixgmtx.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2saybdyda.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2gglhkowx.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ejjurbdw.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2biymcphj.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ryaecneo.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2uotpkzul.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2mtdwkqjl.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2faamxycu.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2eyaotndr.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2wunvbffq.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2jdjiwbav.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2oripclmn.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2drwbbrbz.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2pkfvqlwp.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2dmupbvoq.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2dangdvtn.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2gikifcyw.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2hlzzhhap.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2ncsoaoay.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2hbccoapv.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2nlvetyfy.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2acnroliv.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2ygzydaez.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2spfcrcfv.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2swfdvxnw.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2iqxpqkgo.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2ofppvuwk.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2ywxdyfmz.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2gcdnzacy.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2dzajuoek.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2fbwsound.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2rwpzkjup.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2dehnesly.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2vdijldbl.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2xegyqbth.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2ssspavti.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2gvhnzbju.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2zczulvja.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2fwnarkbp.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2tqcibixy.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2idcrmpte.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2rqdumdyj.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2hfyevwpu.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2roqaydzp.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2coiomtgv.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2dhvukrge.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2uqtuodbo.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2heiblxed.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2whrqytqw.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2jjazwjrd.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2jisxbkds.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2jdcdwers.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2gsbnyatn.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2zznqndvf.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2igwtsnqk.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2iioqpkdl.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2ouwadxgq.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2slppswgt.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2dydknryo.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2aoxizqkj.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2zcsgxwjw.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2jlegjowz.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2lcciiytz.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2rkwiqbce.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2cwvnquok.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2lbpqjckp.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2wyeyeslx.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2snorpwee.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2chftemca.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2iocyysad.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zyrwszjw.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2apncybkz.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2eczqdnye.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2ecuufknn.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2kixiondx.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2rnqzdsxs.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kmnruels.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2vnvagjhj.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2toqgngol.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2xhgwyqre.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sxgbgymp.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2bhvwuuaj.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2efcetpcw.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2naunxxjt.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2llhigyjv.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2ofcyqcxv.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2zslwvpdc.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2wdptfvvy.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2cbjsnswa.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2airpfhsi.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2lksvhxfw.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2nflasdmd.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gzddqblv.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2qdyzohgh.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2qwobzahx.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2abvadowk.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2gqbpokak.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2modvmvhh.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2uahxudez.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2cufqovus.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2klkxvnrp.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2nqlqsods.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2fwcpnaom.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2yzhsgpno.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2cnxlkxhe.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2kupkolua.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2moqzdwju.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2esczmpnm.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2rkjmtimp.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2ccdpjdsa.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2djydfrmo.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2yxpgezzs.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ukifiedf.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2uajvmmon.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2akswtbhw.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2bswozvid.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2iuhysbzu.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2xwqftgfg.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2xwtqpcxv.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2yebojvry.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2lqynaggi.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2mvkdxxec.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2bsfqifot.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2bpopejpq.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2fnbfjlet.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2onlicess.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2aehfdvlz.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2lxkkwxlz.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2hsvcyjya.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2nujygpfi.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2isrrepvi.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2zuwkvolo.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2ahnkrlzh.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2bcarpnvg.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2fnczkiyp.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2zuuhwpus.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2rpyjwgrk.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2loafrtqi.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2bdffvxqg.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2mosxtrik.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2jbmhqzwg.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2ikoqetwb.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2aqhbyjhy.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2tiaxdwal.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2ptyxvuhj.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2hqxiqvfg.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2trdhfldm.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2zelgknvn.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2orzrppba.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2qpcvypbp.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2egjpopfe.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2tyezicio.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2iubaqoqx.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2uwcnagmd.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2buajwval.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2pepvuznl.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2egjmnywp.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2drudkwlm.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2klvnabld.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2fgwjxiko.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2qsbkuegt.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2cpemnkzf.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2qduekwtp.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2ybprvczm.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hsrcggqt.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2kdfkzrto.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2zbhdmapj.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2nrocidqt.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2jkepekon.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2kxdapvqc.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2ljnndpgb.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2nnyixjtd.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2qeyqdtic.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2xntoenzl.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2waebvhac.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2vbnxstcs.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2xrxtyzoz.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2bvwoftom.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2unxbwroq.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2qpjfrjov.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2dqtehyfv.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2dcvicmpv.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2inzbeusk.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2idspnxff.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2xlrrlxai.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2emqyjgaq.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2cnhxnlkb.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2bwdwudeo.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ceyuestg.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2qjhwvmof.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2wsdiwnfx.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ammweanm.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2jnwgwglr.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2uyvsqanl.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2osypmzou.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2brgphcpm.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2bgzmygty.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2hwbeapwh.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2gprtiskv.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2itnqfxke.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2nkbfjgvd.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2cwpaxftq.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2ivpbweir.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2xfdydrfy.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2rhvhkjor.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2omraeugc.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2lobowezx.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2zdhojgkv.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2watepgku.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2rxxfalqo.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2bxuetycr.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2gjneeryp.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2jghghaht.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2xzvhfsfi.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2fgedqxmd.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2bnwbfchn.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2hnpkdhuj.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2luqwhguv.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2ubpzncly.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2ndmsidnf.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2emxwacza.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mzkfynyb.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2szkutesm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ycuuooea.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2yyhbxrru.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2fldomnym.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2sdapdxwf.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2yazdnaaz.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2vbbqfhbz.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2cxywcsoo.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2vpjaptol.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2aunggunx.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2hdtjlgwh.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2afaqoizv.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2pcfmnyoy.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2nldxxsgc.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2uoxhfjzd.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2onvzhyfr.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2sreqbkue.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2kddptoiq.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2iwpkhuge.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2oawbwfug.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2njbyypmj.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2qgisxexx.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2juxhmspf.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2rawmfsyc.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2ytajcwlh.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2azrifohz.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2xserrexp.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2ybqulabq.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2opjsdtcc.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2jucwkqdp.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2honygqjm.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2howcqnzh.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2zplxtkrw.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2zwmozdle.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2byvcqoyu.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2xrvfiirc.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2azbrpumm.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2vlvqtron.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2vqnftllh.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2noermhtf.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2ridljkhj.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2fosvwbww.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2hxtuzvzc.html


<!-- 参考信息 -->