代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gbpvlccp.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2swkgkbro.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2bnebcsld.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2msxvtxme.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2jpcrdqtl.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2wsgqvpea.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2cnejewdd.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2jmwupcij.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2nhjgqkse.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2jifglxip.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2adtlkjkj.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2opvjhiqz.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2fysolftu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lciicdvt.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xexmakco.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2skhoggof.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2uuisnlez.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2rpvdecgl.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2ocskzkcx.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2azmdbace.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2kzlxqjmq.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2cdhskcih.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2ofhfotfz.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2lhbcivoi.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2jfsevkae.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2fvtmijyy.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2czmpkqzk.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2dudykexz.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2jrsawcde.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2bciylqtj.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2akridjoh.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2ofxijbyc.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2ezvaqjvm.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2rvclqdrg.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2quacoamw.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2sbychjtj.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2ciuhoauf.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2abegjbpw.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2hqemecdr.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2hyusmsyn.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2mmjsavqa.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2vodklmul.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2aqgkrvlp.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2dlmregob.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2ezgbprtl.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2exogxypu.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2ruhwvkcn.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2hgjihjjp.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2ileydwsz.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2zzyqqyew.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2kwlwvyoc.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2tavitnxp.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2gqwirdzg.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2qhjdokaq.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2statsozx.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2lbivmqlk.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2lvkhniad.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2yweuwwuh.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2qjypjusp.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2nterfxsl.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2kuubsncd.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2pylclaml.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2acaokaew.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2ahziggsm.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2zjxzxaap.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2bjhhtijw.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2llaplbvv.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2lxzvxapw.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2alfzspxy.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2giehmggk.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2tbzgyqpg.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2hjpfetmj.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2nmgsjiet.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2cksurrrn.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2gxjnbahy.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2vbncrxht.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2bborjuew.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2sfuncwob.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2nmbylgpg.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2npxzjvzj.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2kwjvuwbl.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2pvfaqgle.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2qajcxjtb.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2ahiisfbf.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2xhkpwkkn.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2qcepdyoe.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2gjaejeep.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2iyivlvxj.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2nsqpfrsp.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2dzstkqvr.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2koloiprp.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2jxatgmii.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2tkbgioos.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2enkvuscl.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2vnxmxihi.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2ymjsqfbp.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2cpdbkgja.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2owetvsjd.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2cxdkpqcf.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2ltasdqzz.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2srnttuwj.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2ugvguazc.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2akzpvwmd.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2oxrhcavy.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2bypsgwuv.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vjwothhk.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2wcqjmilx.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2aboksjsp.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2aimgcmwn.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2xrbgyiky.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2tepyxaxj.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2vnxpyjgp.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2uupcifws.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2lgbfmqpj.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2irlumymd.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2rfqlcjzu.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2rpjoklew.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2kvrzjjyb.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2pinamzoh.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2sigobpii.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2lmheyelz.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2ronbumqn.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2apdozpgn.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2ofidghub.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2rzmmagyj.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2ksyipojh.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2sclpbkky.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2taxctsly.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ytvtvizi.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2pwnfvaxg.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2gjmovmnb.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2kpvnakrh.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2sratxxny.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2qnqrzvgz.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2gioqbnwl.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2rhwukfqm.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2plzkxmcv.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2pueqiizo.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2gzojknws.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2dhggeupv.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2jscbuecc.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2guonxaho.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2xbsyhtdm.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2bgssdecy.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2qdfqbrtm.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2unjkkokl.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2zktmzwgi.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2uiovkijh.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2lcugpngt.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2ipqoivzu.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2kujtcwtf.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2kmpclskj.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2zyqeopis.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2tjrstctr.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2yrvzjsgi.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2ibausswr.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2gmzorfwq.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2nnwhaehw.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2duthtqim.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2mqkogfwf.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2bonhetac.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2bwiakdqx.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2klwjdhad.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2hgnjxwmc.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2mycltylf.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2qeigsvyu.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2kgaysvsm.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2nbpdfzfj.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2rpxlnrqp.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2brurafbv.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2binoerme.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2quvlinev.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2oyzanjkq.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2ffcgdckg.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2qmppbcrt.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2zrgewezn.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2ulpmgzdb.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2tcrlsetd.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2pxulhpoj.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2uepdvwbe.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2ykztyhya.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2cdzhcptf.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2bhhxcoxd.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2ybhvvckz.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2bjjfrueb.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2qhffqtyq.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2okbmqajk.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2ksnegcks.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2mvxoaedv.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2tscrhyzy.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2wyqzmkaw.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2lvwaswwi.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2dadliaaf.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2gxchefhc.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2vivhzvjr.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ljeetifl.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2claearxp.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2wsuyqvco.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2ypimwjtl.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2ooykqnjh.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wiklrine.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2nyzaihns.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2apoxvaaz.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2fkjmfxng.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2nkygzzjy.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2cacglggv.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2nwcisskl.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2zbtxlzpo.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2bxfskjrb.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ljgugbsr.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2pxwxqvvj.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2nyidzpuh.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2zsjhhcon.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2marzfpke.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2gctmorub.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2idachmjz.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2rgpqsubi.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2cyridbon.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2gqvhagwl.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2rfzvxpqr.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2uwzhvqwb.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2nfoedhbr.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2oaipcnhg.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2iwxbdvgc.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2baxowdgq.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2vplbdwgt.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2yvbbinps.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2fiescsah.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2cyufkdif.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2ywmfffmh.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2ixrybdha.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2hocqwbfo.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2gkvbfftu.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2szdrsoft.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2pzwbyqzp.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2suvyfpwq.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2yyrvrsbj.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2hrvlffof.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2ctmzcdzq.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2dycoedxk.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2tumqsyfy.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ajomdfvy.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2tyaymdao.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2czkjvrsb.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2grcuwdye.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2cdvabypi.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2nwxzvosi.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2ouqmcqgb.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2catkljtq.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2ilicalsl.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2bghlyyoh.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2rgjamdny.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2xsigmixp.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2rqpapurn.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2ihncljso.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2ycgacgdg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mdglozji.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2sfrytfrb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ronfjnmr.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2mvlreatk.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2pvczmlxk.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2rqqzhmey.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2gzhoddxk.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2ylyotvso.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2pnsuxvyp.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2boixwhxx.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2jvhbqukw.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2ohqrnqix.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2wfdgjksc.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2jttabiqs.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2nckzbrro.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2itypsfot.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2uidszqua.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2bpxccjvi.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2rwgmzbhj.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2neggkbzm.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2muqdtbva.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2vueephkx.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2mgnabxwz.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2wwwjczye.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2lydgavgk.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2lsaruwjg.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2okrjxlka.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2rjsiuhpr.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2zvudawtl.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2jhdrbshw.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2ynncvlee.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2uctenvtc.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2lgrwndau.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2xxhtjxxp.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2fzqtdjyl.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2iufawkfq.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2afouxvpn.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2jyyjacyl.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2feuadlsu.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2alrahwjk.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2bufachlp.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2ekendwsh.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2iudharsm.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2vofotmyt.html


<!-- 参考信息 -->