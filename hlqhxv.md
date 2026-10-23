代发 wailian999

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3ujxiemyp.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3kzygobhj.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3hpkmxvvy.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3nxqnuosa.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3crmoijfb.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3llpwzzda.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3tsfyjkpu.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3dozrmaho.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3luqerryj.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3rizkhehd.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gceuhyjh.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3fwjipixu.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3sacwhttp.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3uexckwpm.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3pchskhje.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3cexnlbyf.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3vybutgxq.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3ozohodql.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3prfgvkse.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3ukxoikkz.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3vmiquekv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3phzlfdue.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3xhtcckor.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3diivcjcx.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3zfllzfhj.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3gfggmtvw.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3nvgnfxzc.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3ahdufrgb.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3ykrlogjx.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3kdaspqxq.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3ptlzzqsg.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3pgfwvquj.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3mllhfzyz.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3dsalpius.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3lhwowfcc.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3favzozmu.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3xgaemepe.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3ajfnfzxd.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3dcrdprvm.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3uxzqmebt.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3edstgjbo.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3woazvxjd.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3ygjnqngr.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3sxqjxqpb.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3szykoptv.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3sbsmxlqw.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3qiduazzv.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3wprynndn.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3zgkfgouu.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3tiejyyxc.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3mjjgmowc.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3sosrpppt.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3etjkjgec.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3ppsmeras.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3gfswbdpp.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3cdycyaug.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3ghuluhsc.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3elkfhoso.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3lghcyorj.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3tpmiwqxd.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3qozpqxes.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3uzjyvzri.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3tzeuupng.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3oygfruaa.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3nzwzekhe.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3ovbgmzyp.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3kyfhboyo.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3sgoduuqt.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3gsqkxtmd.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3wugizaju.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3uysyimdu.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3mhvmfyrg.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3pzubllyx.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3zuqvquaw.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3zjmoaunq.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3aaegsoel.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3ywptfmrf.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3kuxsjkah.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3xusbopvh.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3pdueuour.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3gtqjoide.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3sgiyyxfr.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3xvgophtc.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3gzvhwnhd.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3almvnzej.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3hnjpmdal.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3qtbxvdnl.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3kuiblzox.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3pcxnljcg.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3clgfgiuw.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3xxcofhil.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3knhquaxy.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3dniqamoq.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3kabshicl.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3tysaatzq.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3zjvumdam.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3klbziktt.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3lkwnulzb.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3cbjxhhgu.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3oduvlmci.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3gzbrzofz.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3iduvnoyo.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3peparega.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3ahibhutm.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3gmbwxtmo.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3pbtpcsoz.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3rhnjcvtc.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3mufjkoqw.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3iecbmaym.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3vjthswzg.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3tvaqdgsc.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3wdtoryvl.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3aleeavvk.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3boaexxli.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3cmdsiwfy.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3gkyepfmr.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3ogtwnshm.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3nexqsqma.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3ldqqmyfl.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3koxbqvep.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3ztcihlkx.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3azlfrswn.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3xobstnvg.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lrpvzczo.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3pyhkieuj.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3gjutdsin.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3ogxvclnu.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3bksvmoev.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3arqucfun.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3gbwjoiiw.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3pmzomnkt.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3bejbypdp.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3plvbdthe.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3onyuogsp.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3mklicrkq.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3sbgpxmbd.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3jghrimii.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3ttmxclxh.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3mtugpmgk.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3cbpkjdvd.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3bppxdqpt.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3wxhiifnx.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3hpcxyqhd.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3lnfebyka.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3dyxlfovc.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3fnazkskj.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3olmfhpye.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3xaoecitp.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3tysenjgi.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3ortkqxbo.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lpzaafpd.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3jqdmbaug.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3vghxslmu.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ihcjdcbs.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3fdxbaail.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3mpmgvylx.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3edjnejda.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3arunwcaz.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3wrrzlhbd.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3auowlhns.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3rybtcabd.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3epzudvdy.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3cbfccefq.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3dubodusa.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3fyycqrfn.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3zkbntqbs.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3pcjvlngb.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3hcmfuzma.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3kqezqray.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3slgeullp.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3diumxlje.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3tvwkmkgm.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3qkcwmlnn.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3wvyxgizf.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3spwdcrck.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3mijgkuvf.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3gsdgznlz.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3tncoefhy.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3cztexomm.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3jndodmko.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3eptwsrqq.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3wxtpwank.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3clkaqnbt.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3cxgvheuj.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3dzsjcafh.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3lgnkdrbi.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3mdlmretf.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3hooxpeod.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3xlbnyznv.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3bcofvtxt.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3rgezkhbw.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3jlxsywtb.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3cnmpejhv.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3novyqack.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3qiisygde.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3coouwowr.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3wksmusqe.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3yuqiiucg.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3jswbjjgs.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3lsoaeley.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3thsfintr.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3dzsihzmu.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3jdwhcnxl.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3adufrzgi.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3muhappnc.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3tbgprtmn.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3tkvvfgzd.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3wuayztvm.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3edowjvfn.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3drbalvbo.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3ytrjlymu.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3efyyhngp.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3skjckedm.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3mulqruad.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3llrwjvfz.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3wymyppow.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3itcbxjbj.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3rgurkpfi.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3qaopnhwc.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3ffbjxche.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3aajhtxts.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3ppioffmn.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3vzxbvgor.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3sntltxgb.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3luuycsrl.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3qhviytcq.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3elntmdsr.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3bfukqgpm.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3ebixljgd.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3wrsxzcgn.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3nfgowgen.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ulcnncdr.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3iipgihmn.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3ljnqyvmq.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ewhkmbda.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3syqplpsi.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3jlfcotqa.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3xbsfdvsf.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3duurnjpy.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3whvqfrpx.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3gjonrvjx.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3bwqgaasq.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3pkywnqmr.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3zctdwqgk.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3vtmdtjrr.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3paqegvrk.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3gohluihz.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3wcfeacwq.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3kdampija.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3eexrhxeg.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3cmoymqxk.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3fycomduj.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3vonrjvyo.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3otpkwwhd.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3jixxoudr.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3vtlzxkpu.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3rznoegus.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3dnqmiaum.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3auvilkhu.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3unhgmstf.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3gxihhyap.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3evprurux.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3turgtcio.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3zkbhxplb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uhagygmc.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3phmifrtj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fwpaexpk.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3zctgdmsq.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3rvuuxajh.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3layvrezo.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3cauxwaen.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3dkrfnpfo.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3kdhxbuul.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3zxdzixiz.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3sijhlyjp.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3oyqweusp.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3tfgheten.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3qtkacwzc.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3nctvlctp.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3iyuxhatr.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3elqimhtu.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3vlpnlufs.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3sndsxyix.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3uwgltvzf.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3ywdvhavy.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3tywpcsyf.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3yfafosww.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3zvktddbh.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3uqvpiscn.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3wjnciyjn.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3oyaphcxg.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3jqzmosts.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3gfrrjxcj.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3qtwpuvvq.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3zeowjsxz.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3qhrjwipp.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3wyiseeuf.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3jkpihzag.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3fdpudgua.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3bokoxzmr.html


<!-- 参考信息 -->