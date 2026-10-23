代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3xvkvddbz.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3fnhumjcr.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3fdbqdzxf.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3yygahwfl.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3rfkqogyr.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3aghugpww.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3ycixoqym.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3ttkbxlun.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3sdatjsct.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3pdkffssl.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3zdltwmvg.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3jbciboso.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3ciykztip.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fuoelxpd.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3aksuqyhg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lmcfucfd.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3gdmiivni.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3gxlszjhq.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3qynwgnkl.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xemvvalj.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3igxfeitp.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3mceigkgj.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3eddgiyrk.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3tyditfik.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3rpcbrbhu.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3qlzwfysw.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3nvcnelrv.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3fvozumtt.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3gywvuygc.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3qmeberba.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3yowkcwjh.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3abvfnkwa.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3jtdwpphq.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3ydcvglfp.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3jpdlfyrl.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3vzjppkao.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3tjipjxwn.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3otpzedcu.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3haqifzgw.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ipvlmckv.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3nuufazpn.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3qfvnqlgm.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3anwmhvwr.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3ueqazfve.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3ofpyubhb.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3yqrutucu.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3mksqcizy.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3raprqnwj.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3gjephrpr.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3airnyvte.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3sqpqbmyb.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3fdwjasvy.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3keuwkplo.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3zlerosrv.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3qarselhi.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3lqmygujj.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3cluypfjo.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3nucxzfov.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3qhvgonzn.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3zjxlfwtv.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3cvpmbotc.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3huofnwnw.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3axhllezk.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3bhnclakv.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3tooszxjv.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3edewpkku.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3emybwkbo.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3bwipephm.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3ckgovvmm.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3selyqufo.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3sfggykld.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3otptqleu.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3yltyeclm.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3gtwnehfx.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3pfdceppm.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3ydjnieqg.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3iljvplkc.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3mcaldggp.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3eknefvpv.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3nwbahckj.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3ajbmqdws.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3oldsefjx.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3ghktxkeb.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3rbrikkxg.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3lzcrilyp.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3ubjmvtgx.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3erzekpsb.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3omwghznj.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3qatrliyc.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3dwwwzyns.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3ythynshw.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3dueylpji.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3tgpvxtue.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3sgeirlvn.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3tixzeqeh.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3ndzasikq.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3wusemzvs.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3sqhjjzkq.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3brutzcwx.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3pgvvrkgi.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3sgcoxzpo.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3pawrtqxb.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3hzlzwuoi.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3iuenvxsb.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3ywageoyz.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3zecszpnl.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3qxmknwhy.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3vjqyauhc.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3hsqvwutt.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3jotwopnj.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3swrzlrxw.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ndiclwba.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3sounybkl.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3thxtlqdg.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3cfgwpyav.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lnsukdjw.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3oyoejhxf.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3mdjtlnst.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3wboupuoq.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3eymfezoo.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3qnpkkkei.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3efxdkofl.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3hfxqonzy.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3ditgccjj.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3qieuobhm.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3egllydnj.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3bjivawfk.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hfdsgsya.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3tyuhlzse.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3xfaxmwfv.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3smxcawuo.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3yhtqewpt.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3vzqkrhys.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3jmimltio.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3txdrakjz.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3poatqzvj.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3paukydcx.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3zbowbgck.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3wgefrxmf.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3fopyaxdf.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3rfrwfxvx.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3ivrgkalb.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3dgdxgysd.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3ohiofhrr.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3mysedbsb.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3agisxnke.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3xrkfeomd.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3jzxylevc.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3nomeepnn.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3nbwfqxqq.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3ajmrqnue.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3ycbpxrbu.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3prvsukcn.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3ocsmovdo.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3rypfmmni.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3nsuciakd.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3yczynkdc.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3dnkpwisu.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3jztpjcpj.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3aivmsopb.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3wfwaldjt.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3mmokilkn.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3wynpomio.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3bmpijfbk.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3tfukkhmy.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3mqmmmdtj.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3bmhxohhk.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3lumhcgau.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3fzcrszct.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3wauoytex.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3qrnjvcjs.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3ppnfrzxo.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3dsonnhqx.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3ykkdnrul.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3rmbqejvy.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3tmvohjpy.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3jfhgxvos.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3jmcwlmzb.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3pshprtmx.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3qabnnzgx.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3ljofhozd.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3limzpiop.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3hqruurfp.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3mwmisvtp.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3azrgairf.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3rarukksc.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3pcbqumll.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3fxdibmls.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3njebxobw.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3abeqlzpx.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3iquxfwvi.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3isnvsvbf.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3uguoykeg.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3taebjywe.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3ttflrkuc.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3znykxlro.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xdailuww.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3rdxejjsq.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ttiqcxhg.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3fofdiixp.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rxvapmpw.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3pdhqigcf.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3njhhkvse.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3kbezjcoy.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3kuvjtuzn.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3ifgtiuvm.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3zjqkolav.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ijyhlqnu.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3shtevrtk.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3gybqxvja.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3offcpnwd.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3gddqbbom.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3rvamkvok.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3pzjvuuup.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3tsahksfp.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3reycmqyq.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3klibmccu.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3isqkwvsg.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3iivznzjv.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3qbletski.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3guepayvj.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3nyzvewkv.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3zdrujotu.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3xjhccmsj.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3smhwpuqh.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3sstqlwtj.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3dbdkaeks.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3biuzqlrh.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3kbkonejk.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3wkvlgevv.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3jhwsfbvc.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3ddmsbvio.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3ojvqyjud.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3kdsnhjce.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3tdgqnzyb.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3rgowmkju.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3uwiyaeac.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3lleqbike.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3tgujtwvt.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3nbmppvxo.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3kxspimjb.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ietsbtvs.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3mekqhaew.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3kpcfogfc.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3pvjuxfuf.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3arfpkmgs.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3irdmzkjj.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3jbcrxefa.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3bewkxxpb.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3vkablynm.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3azecxyah.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3zoztrhmv.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3dzyyjdmt.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3rpytwree.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3ktndmjlj.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3yubsyprm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3znqjfjxo.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3yvquglvu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mdsyfocl.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3nybyvjmk.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3zqkolgpa.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3zdhcllsl.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3ghxbhkuc.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3wblomwdj.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3ohoythiz.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3frijaubx.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3xqqlafbs.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3bhdhbaba.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3neazponw.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3mtjczjdv.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3kabbfgoq.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3ddyuntgm.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3gyavtryi.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3klvrpmbb.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3dfxgoihf.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3dqwgqbxz.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3xsnmjouq.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3lilmqjwb.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3lfmqgcfm.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3nzqpjfwb.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3vhlhbeyp.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3ucbyjpfc.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3uufpiuwj.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3jaftgruc.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3kqvglroj.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3wyshwlsz.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3ifgbuyjq.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3esoxkfdj.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3aqkinnrx.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3tneytbfa.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3dthagfje.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3zcvcqfvh.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3nqaclrgm.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3snnwycsm.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3ixtadehy.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3xjiynkvs.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3ojtjuuem.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3lpexpfps.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3tthznasa.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3eivfyhyh.html


<!-- 参考信息 -->