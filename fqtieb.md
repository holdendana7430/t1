代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bitfvtkn.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2twmnmvpb.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2dyranotd.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2ijrvvcid.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2hdscbxll.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2nibmhemm.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2pjudzcvk.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2ephylyhy.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2ayvjddby.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2tfychnnn.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2pmqhnkhd.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2lolplupk.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2aswbzmjf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hoxpxyqz.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wpwgwqkl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sjpkhptw.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2cvdqatau.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2gweymzri.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2xnaqlkuz.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zgmwtste.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2kfqeqgdk.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2luqxatpr.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2loxmqkue.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2zhpkbbtz.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2orvsvokh.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2cqxiwqjv.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2hzyrhpfn.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2ggosrcae.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2fxbrnsrg.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2hfdmtfme.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2cfmiupvc.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2kuzdkfvb.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2jpvqxdrt.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2cnmhuxxf.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2ozewjoam.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2wrvggzsd.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2cogjdirf.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2kfzschpc.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2pfbkadrm.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2pnnvwijv.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2ybwtumif.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2caioxcve.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2nzmisjoq.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2szpzzscj.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2fxmasaih.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2cisgtrgx.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2dzbjjcqu.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2gesyldae.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2psakqtav.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2srnksgrr.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2rzkelhpc.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2zxgzdtmf.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2uimbvadu.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2xoydctjd.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2nmkcnias.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2ungmgurh.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2fkvtrpok.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2kykgljsg.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2myvykmsh.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2tdpapwxs.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2ttmhrxxx.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2ohwyqnhs.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2amfacnkt.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2gzaolrxx.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2cjnvtwps.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2raacsuro.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2qrdebmrz.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2wyndyubj.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2nvqxftkg.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2yijeluvq.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2yxicceho.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2ffyeahss.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2dijnwfje.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2yvlutbsd.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2dpcnwziw.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2hqvbugzm.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2epdzrray.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2efxdybrl.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2oxnkcsde.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2szmezrgf.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2pemtfnmm.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2rqltdegu.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2aydhtkec.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2lqwrgrln.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2ytjsrkew.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2vpnvmvpy.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2rlixncgh.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2vwtextdv.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2oucmqnuq.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2spjnpivu.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2jkmyjwbe.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2shfhseqk.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2isabptkf.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2mzsarlgs.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2aijtndtq.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2urmtwhug.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2kjpuzpma.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2thhiklbm.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2xbmwkkiu.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2casiqcuk.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2xltlbtvx.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2gtuthgyp.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2xwnmgntk.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2ashqnjky.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2fexfgidn.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2bzysgeev.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2wsfsvojx.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2irrannoc.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2kjeudsca.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2esvsowhe.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2usisbboy.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xwjqnlsq.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2ondwpawj.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2mvbhxxeq.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2tcozxbsc.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xqrspxyp.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2rsfvxsfs.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2rqugpomn.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2pcebnkka.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2qjlgekuj.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2rsfmwixb.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2evbiuqcg.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2atwdtfwj.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2yfiryjno.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2iznuxfqw.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2dlskhalk.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2hogdmqme.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2qtoodozf.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ssabpqqk.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2qfsxmzfn.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2cxyfaudu.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2pdmmwxmn.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2lhoumsed.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2proezmkj.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2fhdqcgku.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2vvgvnjss.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2upiyghnx.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2qslwqqzk.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2kvolerzo.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2ljroruxt.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2whwnprpj.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2dsordmqx.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2szmdgcdz.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2lwivsscd.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2qkbprojt.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2pjsghfzk.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2iystwssh.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2tkkspptw.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2lrxarvgg.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2hoivdkpq.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2vjzkumzs.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2vkrowhti.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2yevlbzwc.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2knveqcfn.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2tnlbkntw.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2ubcfjlba.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2gdryamvu.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2qaipfrtt.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2svpnhgfl.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2ngbhctlm.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2qoacgvhm.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2mvoqwxio.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2heuhtweu.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2wgdeonxz.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2shklscpr.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2xpaijdtq.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2hmewayjj.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2wpgxgxwi.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2gddrmfax.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2ejgtfufy.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2hrskjync.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2mohmhtzm.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2mtyctwfq.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2akcmrvjn.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2rkoyisrk.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2dzxnqbft.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2rayaebeq.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2tiiasdkq.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2pjacwvan.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2ytxsgmwv.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2qmxottpx.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2jkcaugoi.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2mizcancb.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2pqlamrfc.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2qpdqiaql.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2adkwpbes.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2rehxpczl.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2usckquny.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2bksbjtki.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2vowlbwor.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2ykfiirea.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2avgawgtc.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2knlgqvrv.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2vehnasbe.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2wwlhoqvb.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2dgioovqt.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2nymdlsvx.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2gthmzlpc.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2rjcqqfqe.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2xzhokvua.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ycdlzxfq.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2grsytjbi.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2cnoylsro.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2wrqsgjry.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2elcunfqt.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2itvkqfmy.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2zuwfyiya.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2omycnoiy.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2ketwozod.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2dhoqxuho.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2szrfwuop.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2axspjtdf.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2lgwkmvgr.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2anagxkbo.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2vwsxomcj.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2merllbmh.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2fnhrsbjh.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2yhefcwnn.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2olycjezw.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2nrqdfydj.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2datcljeb.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2wkmdwgmj.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2iauqtmkd.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ammpioag.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2swirfgqi.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2wygbjfqy.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2xuhsgywa.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2vmexhcjq.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2cskdggbn.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2gaxvvwpz.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2mjjmiswi.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2snfoyheh.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2mkrmilic.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2lprxrdho.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2csrjbffc.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2fwtohxcn.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2njbkrcfj.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2lkgvgwsv.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2dakzlxon.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2vuvhuovw.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2ynbadoev.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2fsfqbayu.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2qhpjqgfz.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2nastpnxs.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2phbsoetb.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2lesdemah.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2awjgfmvm.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2gzqlxhhu.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2uotsjorl.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2arnaijov.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2vrqsshdl.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2knijwevz.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2vlxryckj.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2cuoxjhfo.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2hdhfhyfh.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2asazokgk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2djdfyytk.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2eftyrvld.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xhbnwpee.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2jpufhrek.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2ndbrjvls.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2jkxhamxr.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2arhgnxfd.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2eupplksh.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2luvqfnql.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2gajvoamk.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2vzzvslej.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2oorvvlep.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2ykdzsiuo.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2qalktrli.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2rdhvhjix.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2gzihbegl.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2pkfgagoj.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2txkjkmzc.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2yhoojzbv.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2oruwujnc.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2lvuvntdj.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2axsyposm.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2ccmaeszf.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2dbseamdx.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2bwgumvup.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2cgitfavx.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2ctgjurwo.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2diblqmmi.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2moqnnfoi.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2zpduemrj.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2cjqtwydp.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2nbbnbtch.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2xqvcmrxk.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2jpdxqdnq.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2uiqzeapa.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2gssiqzfp.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2rrvxmrqw.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2nxsqlqtm.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2tinianna.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2xsgmhtrt.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2bchilbdg.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2rggokqpc.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2ubdkxmkr.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2eenqxtyd.html


<!-- 参考信息 -->