代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2frgcvftn.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2gffjqlft.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ttxxkmbh.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2dicurloz.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2kdhkwsll.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2gedngcma.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2emviqper.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2ljgnlfah.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2znezbubs.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2cmcunffo.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2euvsbtbk.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2pendjuos.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2wnereyuh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dmjqwlfm.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ofkvnkud.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vdaibkfy.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2jiqaqvbq.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2ceozqrad.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2ozzebrgf.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wufucmaf.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2kkdaywlc.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2fuzaqgyr.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2zowdzvvf.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2wascngcu.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2hxnnfvjy.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2htenrggl.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2kyyshxzf.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2wrtlidns.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2uigzorie.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2ppgqjtvl.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2eknfhvpp.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2uonfeoyi.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2eryrnaif.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2fwxdnxsz.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2gledzowc.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2idvqgqxe.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2zsolbcfd.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pqcbnhbf.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2huchzimh.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2ledxknmi.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2mmglqpih.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2kdvstkpp.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2hhhtiahw.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2htsjbors.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2hslztywe.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2wqaxzsqd.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2jmkaugoq.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2abbqekid.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2qksyygly.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2tnyxqijl.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2isoudeil.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2jjhnmqic.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2bwdcjxls.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2xbbangfo.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2oujuddgq.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2dsfvdzgi.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2xwvpsqoi.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2plbnryni.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2dszrczfl.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2rlkzijbi.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2ldtdntfk.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2ayfvgaoy.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2chlvrtrk.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2mgeyylnk.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2fngujbpz.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2kfsvvogm.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2cbnpvkps.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2hmsyfdpq.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2pjvygosz.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2vzlswgjd.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2jbkchslv.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2xotlbzjk.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2fwbnarzl.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2eqezpvhc.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2wjrblzcp.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2wzkyqhtp.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2jnftqhmm.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2jmyrnroj.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2eiznovbd.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2cplznbrb.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2ozuyxssq.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2fdgkrtwe.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2pjkziron.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2llxjofwd.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2yvwantsi.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2hyuutfsa.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2irsajdtl.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2xbyywflv.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2gmzvkado.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2yxuumowi.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2elvsejpf.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2oqywetvw.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2kmvbmtce.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2efxumodq.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2kinuaymy.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2vxbcnabl.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2cvzfmwvk.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2jybpzflq.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2jqbcesmq.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2xmcrtgmz.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2jthwduto.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2mwkbqzmb.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2ykxprwdr.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2mqitibmj.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2ibhmxjts.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2qxixdmng.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2poaswyod.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2cbaruhki.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2ujgyaxgf.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2nqqirsqm.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2bumloolv.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2twvxelpq.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2ojvydtcm.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2cblcoxfk.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2fdogelqf.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fdhadmty.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2guwpdjox.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2zjsdhhkf.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2tlxypwai.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2ajezrqqj.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2gcmlovrj.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2fujfyvvp.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2nuvfvlnv.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2ywqnmgnl.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2drfhvxyr.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2lsiugxdq.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2vzcmzhju.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2qwyltvvk.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2baqfjkfb.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2cawideaz.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2yyfdbtly.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2cruxuucy.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2rhrufweg.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2tilmuanr.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2ylywvlau.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2cglarwom.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2otaoecat.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2fbsqzxpm.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2qnfygfnp.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2vzjovbvr.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2cgaoancd.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2nrdfffbk.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2cdixzxom.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2awxsekbs.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2uuesubny.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2mqpjmdgv.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2uxydamjo.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2eowperju.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2ugdrlzig.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2xdwnnlwq.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2zazngrfn.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2kwhpkygu.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2zrikfmnl.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2mgstvzuh.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2kjflhnof.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2gqmluiqj.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2zdambhfq.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2udbtyfub.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2ssobttno.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2yszeswjr.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2kpwigqub.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2xucawkww.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2zohaiqpx.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2zehfpzvd.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2ptbtyhez.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2lrwnpiym.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2tkwrtcwf.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2mtazagsf.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2oijdmrox.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2kobwpjha.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2ljhqfryf.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2ndlgowpk.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2ufngebtj.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2ndflgoca.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2ktmilpuh.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2hwaadkyi.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2niqjrgih.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2uwdkruxx.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2igdwrfwm.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2htjlhazt.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2igckwugp.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2yxavooxa.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2eanrxopq.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2uxmiadrc.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2zqircbbe.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2ysbffera.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2wexxzooe.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2fyvbjvxn.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2cylzmsvo.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2acjqaocg.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2pdolaxtc.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2goywqvwu.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2aklajbxr.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2memfkjcr.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2pxhxdgrz.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2bmsekqyo.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2jijhxydw.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2qelebsuo.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2pqnjdzad.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2vsxtpeln.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nrxmvmmc.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2iwiuvanz.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2amsxndoh.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2asdaqeew.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2ytbjlmsk.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2vtbcswks.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2vunpiqvb.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2hpxjkeot.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2aatunyfh.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2xgqqydzy.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2mxrhjalw.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2odukysik.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2yoypwnfq.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2jrfecgpf.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2uckgyskp.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2wngaofwj.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2kidejbac.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2fwqhclxe.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2eczgsahq.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2mypzchnf.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2fcnumcnj.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2lfnbyevp.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2cewxlxeh.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2nrxwdshs.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2tbmrcsfe.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2jddhhowg.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ptyxohmw.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2safulkal.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2fdwxswuu.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2wmnvobps.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2itxellkq.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2zscflxmy.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2blmcgkqx.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2sybifpnx.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2bylaisaq.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2zouyntoy.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2bnjyczfz.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2ovypvmxj.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2mrvfqzkl.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2yptkobda.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2stcwzzsu.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qdzretel.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2esckhmne.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2xyufeunx.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2colmfzvb.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2njsfaynf.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2isavwujf.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mfbawhzq.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2iqbtpowt.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2lzwgntob.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2rqzxzwpz.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2hfenlomi.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2qkwpftuj.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2bxhhpkhl.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2vsqygsng.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2qwkkxmzf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eczipnnr.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2wiqquctf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bhumuenz.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2yhejenwm.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2firpmdha.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2qlqaxyyw.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2xuogrbit.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2gnychzum.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2kkmpuwuk.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2zjtgujvu.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2htwhzwsq.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2soeqtavh.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2dlarfbzj.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2cnjcwcsy.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2yypmcsdi.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2yylmtmng.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2gadwguxo.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2ffiiizup.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2lngaoxct.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2odabmrqs.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2qvnwjspf.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2alyadfdk.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2bpmoxtra.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2btbtytqu.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2vrwklpda.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2xgnykjkd.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2ttjvxaoo.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2arxpsjek.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2lzfciclx.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2rssnqohw.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2sqodxego.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2apvdmaui.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2hvxdrcrx.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2pegucrjc.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2qsilqhqh.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2kdlloroc.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2fpjraind.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2oaohnfte.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2oqszbsiz.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2pcebxnem.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2yrxyabhb.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2raeffrkr.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2qohijvtu.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2uoypgccq.html


<!-- 参考信息 -->