代发 wailian999

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3dftiuugi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3abhpnscx.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3zbpvuwha.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uvniyxbq.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3macmlmmo.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3tazknftr.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3lieegbch.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ywiupgrf.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3zxpiziox.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3iacvxvyf.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3emfkszhp.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3xmjjmzwx.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3jgjbiawt.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3tqrinblf.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3gxiqffqr.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3ajczhydn.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3lkzehvpv.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3twvqbnvo.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3qodvljld.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3gvqrxvdv.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3ztprzjke.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3fucgjrzj.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3iqilhnuv.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3gvgadzni.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3twkoqmsa.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3mbtrdsaz.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3aknvyykv.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3pbnplevo.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3gzuaopvz.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3lttmxraf.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3yzmniapo.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3sbqylyyi.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3rxcmquek.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3bmdafcbe.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3nrafyoek.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3runcoqkh.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3tmwbzuet.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3lzuwsgan.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3qjeebctu.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3jiukzshq.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3uoihtzyi.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3mogddkgf.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3peikjmmk.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3dhegpqfn.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3ptoetncx.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3worhcfjt.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3lwxgytxm.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3bwcwflfx.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3ykjhyrty.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3ihfubexf.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3hsbkqdvp.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3israntab.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3nhddrzdz.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3olwuqycf.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3cflddlpc.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3uohxgshd.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3yszyargw.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3httjlexw.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3xvmseuuh.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3jfqfpfkj.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3ejdtvbyb.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3zqpecoos.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3xglsfmvs.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3difptsrw.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3pfggoxgc.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3qgcwignc.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3qwqnfbsb.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3jnrzpqpq.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3orpxdfud.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3thxrlreq.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3tjgcnqlk.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3eexeeoyz.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3aokpaabr.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3anpbcoit.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3iinskptf.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3dmreuvzk.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3ktdkzlgx.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3zcksxfya.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3mgitcjrf.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3lscwcxsq.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3tugkgayc.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3wbfutedr.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3stiywemw.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3wrbgjgfi.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3kadgkalp.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3itzpiywa.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3mmargtxi.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3xjeehxvj.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3afzjexyp.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3fjfvoyhy.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3vicwcoof.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3nbuzgtpu.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3tmvdnyci.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3nrroazgc.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3shdroxwy.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3wzhdicht.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3scmgmvph.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3iezzgcwp.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3kcdfxgdd.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vfjzfjsf.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3dmzkwfhu.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3rikvnyqa.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3iflquguh.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3gbxvixji.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3svbozekx.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3rzzhjdqf.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3efpryawx.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3zjwzfzox.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3rizxqcwh.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3gutmddhd.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3biyfplzu.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3jzmxwimf.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3dzgaedvv.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3tolzmyiy.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3xuedtsuq.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3kjqnudxf.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3nypipwyi.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3hsnvnvbd.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3tyggwols.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3erjxocjf.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3xqsdhdza.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3gprmltfy.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3sbslyxpj.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3fgohfiib.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3eultduhi.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3tnyzmimp.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3ovxevjmj.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3attebzub.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3ygkyazaf.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3pywygizc.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3cjiwkeub.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3cyomcdwo.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3lrszhxfr.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3mqahrorp.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3ciyafzhw.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3dxggcdkq.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3nncuivyk.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3ovxinglb.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3apaclgfw.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3fyivqnlr.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3ftiemfxq.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3chocgime.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3jqncezze.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3mjrzatrx.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3rskpvoay.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3tuxnsusv.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3aeszauls.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3yskjcqsi.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3naoibefk.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3rebfuxmt.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3xcwrnnps.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3peygxchv.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3stfgglda.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3zzvnvwxo.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3bcmjinsq.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3ltcfyyuq.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3nawnddmb.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3myowvpzs.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3slhshuea.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3gqmmlgkm.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3rutxooad.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3wwzuhvfu.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3vnpfruss.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3btlgwxpl.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3rjazcdch.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3pwtlzxbp.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3xaidqgbu.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3hfcaibzf.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3xjmepekd.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3jknvdxev.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3onqkdtrc.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3cgtmehlb.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3fgtkptam.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3ctwxkpqu.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3omwsnien.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3iocemuie.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3mbatdqag.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3lbijcfqt.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3owsturob.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3ijtljypf.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3zucnrpze.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3mgewsmmi.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3hrvjmcpj.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3jbnvbhfi.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hrgvtyab.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3hxvwjvvl.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3fcbqizub.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3azmqzjuu.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bmcisfet.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3epencwrp.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3atkjlmmo.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3mjkusieo.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3cadruxzf.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3xwtxmgxc.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3ihblnlig.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3jgbqmliz.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3egnmhbsc.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3wdexdkwc.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3dzetjigg.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3vycehjdo.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3kpqfxytl.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3xigykklg.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3lafkjxcg.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3ljmfssqw.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3yjykdirr.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3nuvckwpr.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3fgrtszgt.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3wabntxfk.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3mntvzwun.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3pjjarwwj.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3axmljbyc.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3kmrayytg.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3guwjdtlb.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3syqnjsoj.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3inibiwyi.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3sxkbxdsl.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3zqwlhheh.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3ynvxrfoq.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3eexlzbbe.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3mtopxsyk.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3eorvpaaq.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3eyiuyopo.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3iaplqxxw.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3itnsfyml.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3tmwnaonl.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3vllfkihv.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3hgifdxcm.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3qjczzikx.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3msmcttyk.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hgiknily.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3udwukcgz.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3fyjgsgcn.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3laophwbj.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3xfmvyzre.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3nynvkeke.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3fpofwvhs.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3nutrzwtq.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3ddilldob.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3jnmdbcmx.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3bkekcvdb.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3qgzfhbez.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3qfiamfow.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3qxlllruk.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3xftxypfw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ctmzwrhc.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3qoywmabt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hzeggolp.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3mavejpvu.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3anstyudb.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3pzivaqts.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3windfnim.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3aepgbnrp.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3yupsbwlc.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3srvhtvjp.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3kjgpwmlh.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3nmqdlvxy.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3zoqpxvsq.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3txtgykzx.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3kfvrmqfq.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3pkmknnsf.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3kvmarfdh.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3adsmitut.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3qmhzyqyc.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3ixtenfbj.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3udactmcv.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3mutozkpq.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3wwdenuxq.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3kgxkywmj.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3agomwymx.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3edadspdp.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3hxetvkic.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3bdfpynuh.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3arkzpddg.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3mcxcqamx.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3geuykzkg.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3bhtcaglw.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3dcqtsyrc.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3dfxfapdt.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ikqjgrly.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ulhittcl.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3eeaytryh.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3ggpzifzm.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3nlorqskp.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3xrsmibfy.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3cutscdee.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3rxlnqvwt.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3dyrvgjhp.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3rqeihapo.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3hyfihkkp.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3oamqxbcd.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3lbdltock.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3iwjltfkg.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3jtwgsxrt.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3hzymeark.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3xgrgoovq.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3uhnbvixk.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3anxotwoe.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3ckfntrxx.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3mdrjykzy.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3uzlnhmyl.html


<!-- 参考信息 -->