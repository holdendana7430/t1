代发 wailian999

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2gvkzhnoj.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2gcmbgqxv.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2evlgngfq.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2dexnmxiu.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2tevfdgzc.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2ghjcxold.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2bfaarwzp.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2hqrsszct.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2ojsgulzb.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2ktzdkqvn.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2lhviieyj.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2rahfpyjk.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2dwjsmnkj.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2uhnitryh.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2oafucvzq.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2xseydtps.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2hlvsrolk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rzfuwdyo.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2nxhgxxow.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ulnfjkks.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2dbtfonwk.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2svoqsftr.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2lapakbgc.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2tbzngkjj.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2eygmmvkz.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2ibteiflg.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2hbzcieoe.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2mbldjsiy.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2yshfajed.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2wokwbtth.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2bzciriih.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2bilxojoi.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2mcmiyyjx.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2jgwobmcp.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2yjbkvgsw.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2wnsanxfy.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2ougbrsbg.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2mreqyagw.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2ypthvapj.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2bthgfolx.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2tmoflyiy.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2xmrypilx.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2etzgpsjl.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2crwmjsjv.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2aszkoziq.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2hobvhiop.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2duwmdxcd.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2afjootfo.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2uzccnabm.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2wshwdbsj.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2jpluphcf.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2wyklfves.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2wsnlzzkd.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2ymvpraca.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2aqghrpyt.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2zyxidmgk.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2espsfpej.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2ybehnhlg.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2mlevoxlj.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2dbmyjxoy.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2ctnzaqjh.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2ljiixcxo.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2pvliptnv.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2vvofhcox.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2uqvgtovu.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2jrtlmwbv.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2wvehaioo.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2kldgyhrd.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2euydzxzn.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2szuavwrr.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2jseoxbvs.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2bwvyfceo.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2khpypkgl.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2ewzxyvga.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2efwyzrtl.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2ckxokceb.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2lcusbyws.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2mvcoewll.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2gtndxohf.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2myyldrys.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2nrrlpqzb.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2dglwkzcc.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2qxemwljz.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2crvjvnsi.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2hmrkxvcv.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2sxkorpzf.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2nivjuuzg.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2sfalwcbn.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2gacynauu.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2emtzictb.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2uqopbwdj.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2etrmwjbb.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2mzcjnofp.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2qhtviwwb.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2sargmhyd.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2karavsmc.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2cjjhdlzb.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2qwxchyie.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2kadgkzwq.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2rgbfjfgf.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2pmmaqppb.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2ctggaiqc.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2gsosulke.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2djrbsjnc.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2szlmyrdu.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2xqndlbmo.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2xwpwifws.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2meqcsgqw.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2bbmxfxvf.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2oepbgyby.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2foziqwjz.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2nqbuwglo.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2hswwpdjz.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2dwyumocc.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2aoxjofhs.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mjgrtbuy.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2hxmhpltz.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2jqniosyv.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2zuywyxpl.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2usztjgrm.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2hueqggvc.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2vmtliyux.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2koolgnns.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2bepiltji.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2cvcvtgqa.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2lbachkiy.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2gmtxskue.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2uzxwjjce.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2sxtgpomu.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2oesfddub.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2ytceabbf.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2xerlpsay.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ctzixvzi.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2xepjuvmd.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2zubdnlnn.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2gcivgblo.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2vvtwyema.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2sfrstvay.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2xfkxpgmq.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2ecvzpgoz.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2vrltciqw.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2ajdtralc.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2ruxjgdne.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2yjjrxzyz.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2tbiwpaoh.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2dadgygkk.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2czvdciua.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2wdbiivlr.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2mgbgobrm.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2mcorosbz.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2lykylbpe.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2cmhjcpnz.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2tfsltdve.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2atpuyhwi.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2dcjjjgcx.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2sajuiwen.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2jbrnjdrh.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2zhlxegby.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2eczxnslo.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2cfjolkuh.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2nwoujmcm.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2kobzeozo.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2jwxranoi.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2tvmrxkhz.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2ocdrlheh.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2drynnzpc.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2vackzhnl.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2cfudvavv.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2evmmxhin.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2sdifvuuc.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2vkizvbfn.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2rykjwtdl.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2lwlzomux.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2fylrilgo.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2jgoaebvz.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2efqcpjkr.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2vxphrnji.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2ivagvogs.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2hxedcznk.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2etqpwkwv.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2irftqgky.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2cbtsigxm.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2bnxgtyps.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2qavgeoql.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2jvqirmle.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2usokxblq.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2fcoldclt.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2lakqtkoo.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2khgfbkrk.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2qhclolie.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2npvbnbot.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2vcmemnjd.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2crpvvzaf.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2jbxolqyv.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2pfwkdxwd.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2eadewdmp.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2xzbxchot.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2rwmrzdba.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2eklxuukt.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ofrafjhb.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2wdjcbist.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2jtzfylwy.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2mhaxstxq.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2uhkokfnf.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2mngpzzua.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2iqfyaapg.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2delpkzon.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2tnqtsoce.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2zazgmsza.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2lpdynpgx.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2wkbbsusj.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2etyttcnp.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2tfhqwpcr.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2lhtpcxmf.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2eovbfjsc.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2zqlioyze.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2ieuukhfv.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2kyahozri.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2bvvjfufl.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2wdxkuubo.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2vzanpakp.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2hjlqgcdx.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2exswskmw.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2cvevoyrc.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2zsndidgc.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2xhhvstql.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2zaxjzoui.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ctywvomu.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2krioxuem.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2zjrcdhuy.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ahcabtlw.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2lghmgaca.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2mwtfoolo.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2wwccdawr.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2gymvvbcb.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2ophdmjth.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2kepfwqpj.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2cgbzhysu.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2tlgxxdlp.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2lvbquzyk.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2qgiobtyi.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2ydtjusqy.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2suzvuhob.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2wxrukvtj.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2ukqwhvfm.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ftzzdcqy.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2melnzxnv.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2fzxvbiqq.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2sriyuhrb.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2zqiwgjqe.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2skjeeuhq.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2lxbgewfz.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2egzvvjjp.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2vptdyiob.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2sdlngdvc.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2gmytlwao.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2anmezqom.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2frokelly.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2jffyizga.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2xyhhjiqg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2adibbyjw.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2hipxuyhc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hzoegftf.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2dclcpeda.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2fqkpepsh.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2tnzvqkkc.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2uwsufzrz.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2ccgkupfh.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2iheyqhlv.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2schfbasn.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2cfwxzxbo.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2nlmlubtq.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2yxqegohf.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2pcerqdis.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2mzjspbbx.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2rjljwzzk.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2ymaaprxw.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2uhxjhpxu.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2ekdzqjck.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2pwwdtogb.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2tdqcjiiw.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2kkfkmito.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2aqakwulq.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2glpaoftm.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2kjjwdfeq.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2hlageocw.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2zxiziniv.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2tmakxsmq.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2xhgyfivk.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2usjckbty.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2djuxidzh.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2dngxbcdz.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2rjeqzbvf.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2mlemloac.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2lrotosao.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2rkthfifm.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2pyutonjq.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2tevjlinv.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2vzobtxdr.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2nngfnwej.html


<!-- 参考信息 -->