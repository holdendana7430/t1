代发 wailian999

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2amrytovp.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2otthwqqc.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2tblicffi.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2bwgfwmhq.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2uwmxzgci.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2orajxewq.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2mkmjajvx.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2vmbtcvay.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2fsyzkijm.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2jujzwywj.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2kuzfbnys.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2zhqkerlb.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2pigcvzgv.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2xyxrbsvz.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2jrilxjtl.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2uvgwxmax.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2sfsbeape.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2spjdwucv.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mwedcvhx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lesikkon.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2dolhqedp.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2mkehimwz.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2zmafgihq.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2xfihhgxq.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2sockewhw.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2nyxkxnfp.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2cnzykrqx.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2bybbegfc.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2amunpese.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2iaqjgkdm.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2uafjxdll.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2irrytpuk.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2kaqamgbh.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2ydzwzzyv.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2jsbhfyak.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2jpevipgf.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2lalzcmdu.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2ltmebmmd.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2evbdaben.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2obmkdwdk.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2kgoxongd.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fdsosccy.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2awzlhtpl.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2znnpmvrz.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2gzzfmqqb.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2cskwfmhl.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2semstdxf.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2pieqmwsa.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2rxjkibmf.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2aliaxuiv.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2bajtddbv.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2ykkclczg.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2khcloaat.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2cpyiahir.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2nrotjtol.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2tkdhqkii.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2xdnkoqib.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2roivtftz.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2xcmxgsre.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2lnyjtgnf.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2ujyerucf.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2kltlqbur.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2zhwedgia.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2klfwgdkg.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2qhsodpvh.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2uxxcmumb.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2kkdvdxzk.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2whvrcely.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2ymczhmhu.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2brqhtbvd.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2begxmxal.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2vuoqskai.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2gkwzpuno.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2fuxivmaa.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2obnzwrmx.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2hjpyuhok.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2ocwbjtof.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2ggyazpgk.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2cataacsv.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2vhtealhc.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2yrszkalo.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2rgjiyflk.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2vmgdismm.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2rakornsk.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2fnaswmud.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2inpekjij.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2qxargdsz.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2drafmwfe.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2tehwhozt.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2rtqobhbp.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2tkuofbrn.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2ouczwzxi.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2ocmypqcr.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2wyadtvgo.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2qnyiccgu.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2ystgjmje.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2toyzybdk.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2zsjzbpxd.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2yrmzhjjt.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2nrgusqbh.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2guuimxfk.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2furijvpk.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2ojpyqesc.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2dhzbompd.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2qwpyctje.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2uptncynw.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2hylmwznq.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2nzsmiawq.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2omeymkqr.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mfbxjsrh.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2ldmdytrp.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2aimnlqmo.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2zklunewp.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2ixxnsyrv.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2pnsqsdzx.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gdmfewsf.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2gjpewnaa.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2obiryxnc.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2qzvsedqj.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2ifcdrogu.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2ylpqymaw.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2miigkslw.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2knbqupdx.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2pjffyddb.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2vmjtcslt.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2vqrswsaq.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2vmdbzfbi.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2atnurgjl.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2ppcxymje.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2jvmquxpn.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2fgdskbiq.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lgtnscmq.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2efukcpgz.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2raemmcmd.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2mrmmjnwe.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rpvszhbp.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2gxxcjvwl.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2vifdnztb.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2sczmdetp.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2ocjltpmj.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2lpqkcdfp.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2hkzwcvtm.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2lrkspiib.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2rkcatnow.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2aawchmda.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2lrprvkky.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ycitlpfx.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2bwgoylcf.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2ipcangwg.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ehqkbeaz.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2uqnewvkz.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2wfehgccg.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2dueqroqp.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2cbxzrymr.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2ciqzvfdw.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2jpbdrici.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2szvkhxbs.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2wonpuicm.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2yzhrfbjc.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2olosbeuu.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2rkbkdycs.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2adhbacse.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2vkfvyern.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2uuqsyhvs.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2gvlhvtoh.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2stnjmdlg.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2gtzkqoyg.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2gxwdbhag.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2yrzzokch.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2jyucxvxt.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2bwcrmlay.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2awecksoy.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2eopsvwes.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2jfirzdqu.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2ezpgbakl.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2qxshclfs.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2yestygby.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2jhbtlgnl.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2iydsqsas.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2unkbwxzk.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2nhengqdl.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2fffgbquw.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2kxhrzqnn.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2lygaarue.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2sdajazaw.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2ptsuaell.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2nndqlvhw.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2ulbmnsvl.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2uteofxus.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2ldmqhdwy.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2kgnwukpy.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2facdilgz.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2ovkbxzjh.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2fmafjafx.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2xlacwprc.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2qieispfl.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2sfblzdto.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2mgchtojv.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2bndmircv.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2vwleqdoc.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2utsggezs.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2budgqpkg.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2ldrtbxyy.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2wytfahhu.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2aqhxidyd.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2oqtjulha.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2pyepysix.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2vsnejlwo.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2mxeoebys.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2vdpocbix.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2xsbmqjss.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2hyjycmzd.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2kebvbefy.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2rxwjuors.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2nygyyzyr.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2ihhklbek.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2kuhdlwth.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2wwleugch.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2rrldimry.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2npznjkpd.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2fdytdpgo.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2axafcpvb.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2pkwwsdci.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2nqavkhbu.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2oqoucqax.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2vsjaafqm.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2vrkfjtki.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2bvabwsrc.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2cqlchgxq.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2epskesjd.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ykdcubmi.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2ipszqzuu.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2boklipin.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2towlfbrb.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2muabqery.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2efdyatga.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2fukqfpeu.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2cciptdtp.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2gnxlmjym.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2kdvvbkrp.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2ehrekcnz.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2amogbmvo.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2gyikvjgn.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2exmwrtht.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2rgzxctcn.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2wrhiqkns.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2wpaclxir.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2aqqabrni.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2ixlrahpm.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2vauqgrqi.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2dkcjyfgn.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rowffzwq.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2gdyuhwjv.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2jmvduhzq.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2izehfqbw.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2gqhwxnzx.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2ngwgnkpi.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2znfbydob.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2jvgnjuik.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2fewgbelw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dkmkxysk.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2bstyvcxt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2abfyojwg.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2zbseadch.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2lnipmffb.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2oytstqiw.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2jswhunti.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2fbpfebio.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2xdpztuxx.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2godxczag.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2uoctzmfn.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2hkjjkmyc.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2tlxzttsg.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2mjujfsek.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2ootpxcef.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2xjizjwtq.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2lhaytwyy.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2wlflhixp.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2rnueeflx.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2lqbcmgnh.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2clzfwird.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2dxjaskvb.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2dczyrruh.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2ksngrgha.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2qmdeixzd.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2yfrkiyhn.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2sjyuaiqn.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2riubcdol.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2mmzvyrcj.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2cclsyrpl.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2yyhaeupi.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2dsokqucs.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ycnwkohx.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2qlutwmou.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2vjhcdmpr.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2rivojvfs.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2qjnekfnd.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2dryhxazf.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2wbwnxxhf.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2kyrdjgkj.html


<!-- 参考信息 -->