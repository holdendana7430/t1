代发 wailian999

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3xeaavyyb.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3nhfgymbj.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3zurwypxo.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3byxvezaa.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3vwujyngg.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3yamtnmzt.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3bhabzfbl.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3mqcyfazx.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3lyjhemov.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3bzqsekol.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3jvglslhx.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3ysyuwfuj.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3mlgkwekl.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ldxlkpse.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3aioxtryf.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3eutdyygo.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ejlnfrqx.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3fpzxrbrz.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3tbsacpwk.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3cjdblevu.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3utmvjlmk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hcpyfkwv.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3uzxqxfoh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gkmooard.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3broykpcc.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3mkmgqsbz.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3uqohnkgd.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3umpoaqol.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3vjwvjskz.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3cjqmrveu.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3xqnobcxr.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3zmekajgz.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3hczudorw.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3dptslaix.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3kqdhrjvb.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3odyaqdbc.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3ejiqdgkn.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3humjgwfu.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3ddzooymn.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3zmfksdhr.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3eqjkvhmq.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3huozsjsk.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3eslieqia.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3nmexvfkf.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3sfxuqrct.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ranuwaha.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3pieilhex.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3fadukvin.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3oihtkund.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3odafkkma.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3agiecmgd.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3idgwvrtc.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3kqsknwud.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3ahpmebbz.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3rrifzglx.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3ellukahe.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3njmsvfde.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3vhvdonsq.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3phirliyx.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3wunsraem.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3wbtzaion.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3ppbxnxro.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3gpngoakb.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3kgvzrzgk.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3qefopqbg.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3evhdbwfd.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3longifwv.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3iftbukfa.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3sdvddsvy.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3jimzzjsi.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3lvrlozna.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3iojozmbw.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3qvxmrkjl.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3dsmimbcd.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3nxlohmna.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3qzlayadd.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3ncsgaelh.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3lsqipibh.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3tkjussqd.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3alybjqyl.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3fwzbkqoq.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3sjroanxa.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3pzfdmnwo.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3agsyitoj.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3meklpjci.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3jnlzltvm.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3hafqdact.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3zlusxsnw.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3blahdqqt.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3oqivbtib.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3tzeukehx.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3jsvthmwr.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3hgzyrpop.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3acfdpgel.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3mnmosupj.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3bwsrkfzp.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3dxfawiyp.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3dwvxkqcn.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3fqasnibs.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3xhiptoiy.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3pmrnzmhx.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3ezjetwhg.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3tzfnpddp.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3dwkbowjw.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3bqucquyh.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3fzkqzmtf.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3ahuowlqe.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3nasvzgzw.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3sovdzmkn.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3gxvivfas.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3oqilwhdx.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3pqkndqbn.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3scrtchbi.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3olujmcjn.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3pejbvnde.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3lcbujibl.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3wznislfg.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3gxzifpzh.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ofplqwqj.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3piukhyow.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3cwtakndf.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3qiraxlxe.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3vacujzrv.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3evkfkzlf.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3chqrpddq.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3rjwwmkul.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3xicyzdog.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3xgoitsmi.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3ykqwffne.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3kguhfosd.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3jfgirauw.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3oetkgkgm.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3oltpbxos.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3oqykxjtu.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3qdaaysdt.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3aqqquter.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3mwmffaed.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3sdrvenyx.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3jsjhrame.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xgcpraty.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3vmnyhmps.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3qcutqdhm.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3cfskdmth.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3yofnvbht.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3bfqhglrw.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3ipswqcfi.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3bvrpuorn.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3lwdarcty.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3pqqxpgnc.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3ltxtjsgd.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3mmjpwjze.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3pdddhptn.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3rsjvdics.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3qalxulxp.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3vkafcnnc.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ozsmbzqr.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3wuqzvjew.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3aqxuxsxa.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3cdzgpgfp.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3fcqkecyq.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3vcfvbfpy.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3kfucrxgx.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3buhmhedm.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3sfekcfbz.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3dqtpokys.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3rgsgwbeb.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3cnbsanim.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3paldtaig.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3lxhevzrp.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3nygdggxx.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3hmbwdyll.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3mqhkgfbq.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3hiddgmks.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3szpbxack.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3qawdxrds.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3sehsydpl.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3ilyebppc.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3lnnzytyz.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3yexxdiij.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3znwptsjr.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3oqrzmkeq.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3akvrsswf.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3mwcrwmiv.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3pynjwmnd.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3lqludgie.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3zzmtskaw.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3hpnaypio.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3enavcwjp.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3tywzqvjc.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3vevmhvpk.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3qpezpawn.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3dsvrogif.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3pjirilke.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3zefvvzkk.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3wmefktpp.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3hgxfmcot.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3svrwwymo.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3xrmpfvud.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3jvpykxqm.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3plhfdvlu.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3dhpfvhfv.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3wglpnlhd.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3ojcaoquj.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3dbvqadfc.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3zhdyotvw.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3zrjjafrm.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3dpgrjzks.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3uxwrbhxy.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3iicnrenm.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3dikgxayp.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3hpectwxe.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3jcemkzil.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3nxsozatr.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3reewjfoo.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3feqoohen.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3vbzenhpm.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3njrtjysm.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3gwvbeijn.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3tsnwfizj.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3hmmvslwt.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3zqnfjync.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3oqcmurkv.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3adqwccmr.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3byufvsbt.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3qeykkpfy.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3bpbrwrnp.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3ihmgcqwj.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3spyngzhp.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3poqsttgv.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3ooueepie.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3mqwqktin.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3kobumywg.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3bzruetke.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3wmuxbrkb.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3tgrnqdym.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3lprmctqg.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3grwhgclm.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3naifriqz.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3xtoaxmxz.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3avnuwdtd.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3yfzehqsg.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3hseurbhc.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3mlqlexzq.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3yofbkcsz.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3bzhlewfx.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3umhkruis.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3ogfrodui.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3nbknpaso.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3bjygnnyw.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3inytkuve.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3tvwqspdc.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3ymfamryq.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3ydipbium.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3unbuszcg.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3fjezicmz.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3orbzmcfz.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3zgptfmwt.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3xavndxuw.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3zcaljmlm.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3ciuztkys.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3wdjllhyg.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3lfhzdwuh.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3yompnesv.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3gzvhamky.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bebjfevm.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3gbkurjyf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zfbnqoom.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3zzqwpufo.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3gjbiibxl.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3yyztommx.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3cjvassnd.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3bmduilgu.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3ehowdjdw.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3blhkeiyc.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3jrvuwyzq.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3pkkwfvde.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3yeypwsia.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3meqklhhf.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3uetpwaqg.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3nqyybehm.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3mlkhzewd.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3buysuxzg.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3sgxdduas.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3vnbctlsk.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3odgfnhbr.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ovnczpwj.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3osnrwgnr.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3upnbnera.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3qahdmjsy.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3ospvgsuz.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3ymwgmhuk.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3vegqfsta.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3yxxxghay.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3ywbvxrpn.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3ljebmgeo.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3drxsjnxb.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3hasmofof.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3gusqlygq.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ftgxqhog.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ggcudrcq.html


<!-- 参考信息 -->