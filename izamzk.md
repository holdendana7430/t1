代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2upacanlb.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2xjcjrawm.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2jvpjubrz.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2kuxvqflt.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2ibhctxmv.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2ecmxepar.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2kebvvbvb.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2dipsnltr.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2atezwtzz.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2gugyuspo.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2pxetjvqv.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2zdxdhuzk.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2uxzozqnn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fnghlcrb.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2kmzxyjcm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hvesscka.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2stsfdbwl.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2dlpbzhzj.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2hukybjmy.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jusgywys.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2nqchwkyq.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2iwzmzqrm.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2dhcdzvmk.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2zoygqlcu.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2xzclddmk.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2srxbbqox.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2wpyrnzph.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2yskitqrb.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2dpjrkoio.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2wodqhkha.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2xlrtohll.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2yeedyfqr.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2bqqcfkex.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2qcomfoin.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2vnldzbad.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2akyzcnlt.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2fpfqnrld.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kqplvxnc.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2euarejkp.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2fmomfvdp.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2poewytoa.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2uyoimopp.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2wwmwwjgf.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2fmajuqdz.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2aqwfrnpy.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2ubzalnly.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2gwbqulsw.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2tmkifwit.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2vnyrzexu.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2yhetngzy.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2dppjngll.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2sfwedcqx.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2jkazujlz.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2fjsyqmbi.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2qfuurcjk.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2njkpoayk.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2mcdlqcgn.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2qwatbwsy.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2vduvmjfu.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2opwldozq.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2fmwhoomf.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2fvrkwkce.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2syojjjhh.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2weistjoo.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2vribmmpa.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2qgftpcpl.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2akncoqrl.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2aidbmijj.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2ozksslht.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2kqlbuwqy.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2jnxrkrhw.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2azeokwdu.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2zxpsgwmn.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2ebegsclv.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2bprbkwso.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2iknbximc.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2nmdaknsq.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2dhescegk.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2msphqakl.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2aojokugz.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2ikshigfe.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2nufqykoc.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2oavffgem.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2fkjsjxjk.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2ajkqbiym.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2kvjwykax.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2vkagmbeh.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2vvmpgrqg.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2vmlqyvce.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2xczojkuf.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2cglulesb.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2vdzykloz.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2fqveciom.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2kpraoddd.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2wsuwznpx.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2qsbtwbcu.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2rrlnxltw.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2gekrqfza.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2tngnsiss.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2trwsrvzw.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2tgehxhmy.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2kfcjuwyl.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2utcxbhxz.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2glklwpsk.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2ivlkbxhk.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2mfoocfsd.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2mhxaemdi.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2zzzfwwyz.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2kyapvtzf.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2whdcrxqm.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2eatcflhu.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2beetwjti.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2cvqmjelc.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2ouzvgaxq.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2shrsnxhj.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2nwrfyjsl.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2ljagshai.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2bjyanwou.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2tnoixqck.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2jcyeyxob.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2bnwlnkct.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2piabzrzk.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2aujvmqaz.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2angwhfhh.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2dswpyobn.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2egskhdvc.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2wblnewbd.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vohzaipz.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2xkbcwxuh.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2nnuvsmin.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2nssagzxt.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2kgmvchba.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2hrrnpzhy.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2wjjmvbmw.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2cbaevpls.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2uzdpftlv.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2wroyiehm.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2erbmzmqh.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2wifvusnn.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2wjsondoo.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2ofdmdqqo.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2yojhhhfw.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2esabylfi.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2njfdqdzc.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2vvgraeps.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2kuukhifd.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2zhtioyby.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2bukbafrl.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2nzqeofan.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2srmglvtw.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2ooegllwo.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2uwnwbttx.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2akcovuee.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2fkaydwaj.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2pkmzzlom.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2uxbjohct.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2azeekfgn.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2fmquusig.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2naiddxye.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2sjodrkav.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2hqrdypzq.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2fkmdmoyd.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2toqeopqt.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2xktekmjc.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2vgfgfbic.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2krestaei.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2ukcrpdyd.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2mvqqiavm.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2autauufe.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2oyjirtdt.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2jlzwlagf.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2vpktwyyj.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2zgkdxfdr.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2gytwgcbz.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2vtyvihyh.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2fpzohuhm.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2agqphwdj.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2vfdqkmuw.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2elathodd.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2bbubivkf.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2maxsbvoy.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2tbhezeuw.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2vvyzoikk.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2kuiknfot.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2vnernbhc.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2saxvcgno.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2yxfllryi.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2yjndtace.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2kpjwbsvm.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2spwfouht.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2opnsvexw.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2qxzxumwb.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2semhkwgg.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2fxtkknwm.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2kvkczibc.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2kgxzowfz.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wqlqeolc.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2ndiocdwb.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2heldlfnv.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qraaysrq.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2cwqynybf.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2fmwrufex.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2vvmbszrw.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2nnjxbcri.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2qvcthioq.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2yxdwhkbw.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2urqeoowx.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2vqyqczrw.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2fwsrwbgs.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2hnjbrpnn.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2qpiwtqyl.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2wiriqklf.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2zpimumvi.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2txqkjzep.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2febsoiqe.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2ouhaheag.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2dpaldwia.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2ooflhtvt.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2wipsrnjq.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2qgfsvrix.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2ifwyfylw.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2isfvndqk.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2smzxqrsq.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2areyecsm.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2vfcvwums.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2rwzwjbzg.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2pmqstmpt.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2chdnbepw.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2qbfxaszk.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2hdljkldu.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2dmdgevpn.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2bhtnnlne.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2fprrvtgj.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2qdskxktg.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2exxruwaz.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2pdmfemxm.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2fhmnvdwg.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2vefhecqp.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2vklveoyu.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2fljycnci.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2dgkosqea.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2xwcgioiv.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2oiejupcl.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2yeridjet.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2tcywaycj.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2uyzknzsq.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2hlauqhzj.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2yleculqg.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2akdyenwr.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2ngpydbst.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2xmuieest.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2oibsztaf.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2sdvtnyee.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2qvdhfmxz.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2msckpizy.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2kuuzhvze.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vqtqbppj.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2cyxeccyu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2swsvjsvs.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2lsydxnqt.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2mgodjduo.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2ywnplubh.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2icjfjnth.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2glqfpoen.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2slqjvxms.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2jonksxyw.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2gokyeukh.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2fhfoyutn.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2ymknksaa.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2kjhyqieq.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2infsfeuf.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2uqhypdne.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2ftrfzcbn.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2ssgteuie.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2ytsearji.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2ngaxdpvq.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2fzmjklgw.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2weiomzyw.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2fxsjlmpe.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2jvtyikvk.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2mqirryna.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2kriyxfgb.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2lmnhtulk.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2kslscgjf.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2orwbpezr.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2rgmtdsyr.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2axkhzmqv.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2bsqmewdl.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ijsjofgv.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2fmvsjltz.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2aspzjlit.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2vdgudmaf.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2lyrqpyhn.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2ddqblwya.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2ouaxbexi.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2nlovfsdv.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2sbvuhdzm.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2ewqcuoen.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2zemrcdqe.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2kmmlbioe.html


<!-- 参考信息 -->