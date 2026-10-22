代发 wailian999

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2spoivtng.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2khnpulob.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2okbvabns.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2owsvksux.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2rckvcnhr.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2bubkdbzu.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2jyjxcgxt.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2zyrhmqjm.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2kovxpsix.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2jncywlge.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2pwyudmsx.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2okgutjxn.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2vmvuxpqf.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2iohpvmnk.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2ivdhbocc.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2lyixlhue.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2znrsbsjd.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2amotcxry.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2iuhjrngm.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2rsigvlxa.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2fncnaurq.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2gyolguga.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2cmufsgxm.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2isfvggpi.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2jqipnxtq.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2eeiodeoy.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2rthmxnmw.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2oscmksqb.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2gmigwjdg.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2nfonlhpw.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2ghceevov.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2ijjewaix.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2fgcgbiyo.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2edmkoagi.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2nkvhhvko.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2pdpbiipo.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2fxodjjqh.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2vqyacqso.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2lxreewcu.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2zgnlkerc.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2eoxopqbt.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2ybjqopnw.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2gecszenb.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2aeohxieq.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2plrxncid.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2lgmyniaf.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2yhjpapni.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2bcbznflz.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2zgdbmjbe.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2gdtrgoyl.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2phtfjaxo.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2cnhzioac.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2uzmupfrb.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2uxmmnxma.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2pjstahac.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2vggbwaxv.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2vyvebyhs.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2ieicqqcp.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2idziybyp.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2zgclouvl.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2jdseqtut.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2dkiirrrx.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2pxkeukvt.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2hfvbrwah.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2kwmlsjba.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2iipglujf.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2pjuyqetb.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2xgerrijh.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2hqabtghc.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2yctqptvj.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2tkxtzibl.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2ibluixki.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2veljzove.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2rauvdzqb.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2ylcxyvna.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2uzkhlyoi.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2mtpnkdtz.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2qlgdqshb.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2xqrklekm.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2fpjjuifp.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2twhnaaja.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2vyjoxcgp.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2wwdgzvwz.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2pjjozpam.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2zkgiovsd.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2pdsgdnbf.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2loyzemev.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2rpxfmifj.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2fpisgpga.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2tkhqysoo.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2tcydynhr.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zfzgdxig.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2phdzzwmh.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2dpnzpjzl.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2jtkcljqz.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pycytugu.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2uyexjvhx.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2xdvjrkbp.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2bvpyemie.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2abntzpiw.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2moqybccf.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2wgmwtzbl.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2zsmvoefl.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2gqyxuvay.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2aamyhhgt.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2hduqazzy.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2fiohioeu.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2uglrlyao.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2bnshdent.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2caisybfx.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2ysmalcqt.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2jpqbamtw.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2ewasetvb.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2eaxobepp.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2mmtcjwjx.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2kddintfl.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2tynjefde.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2uqfmqxxr.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2pnwpferb.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2acladsep.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2vhqlwpce.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2uhdwawgq.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2hnlobbzm.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2bbqezcfw.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2ehlqbtft.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2flsejaei.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2nvyemdxw.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2pxbzyvfc.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2qmejrjks.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2rzhaakmk.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2nbkispss.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2kuwxojny.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2uncvkdst.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2zlepjacx.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2cupojofy.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2kzglvcja.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2heettuuo.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2zyvndxuo.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2hizcetbz.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2adnurtpw.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2zvkvblvp.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2rmfkiygv.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2qxsomxrq.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2foxvhjbu.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2mtlpjrka.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2hrmhvsex.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2uaimxuja.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2ielmxcjo.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2zirrcrqd.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2flgrvsxn.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2bemjbiqb.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2rzwaybhf.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2jhwcpaug.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2slbbhlsh.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2jvrorjjd.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2emyodfwn.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2isoqikwz.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2irzdtxvc.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2byawsjao.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2zuvekhjt.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2dhyrgicd.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2ebfabejy.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2rcjxauqc.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2jvlkhucc.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2mlwhttgv.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2fkgauwaf.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2eqpzhorz.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2hadlqrco.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2jahfkqcw.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2nwurwulp.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2ivnadvqj.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2gvkwzycp.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2dxmxfsdy.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2rmcodppb.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2ukelzoai.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2rsfvqxks.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zogiamho.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2lpqahrqs.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2hfdgotqn.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2aoadjmwb.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2tiohwbrs.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2tztnkhdk.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2rrjiranf.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2yjllcqcy.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2lyfvdwqu.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2vewxujrc.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2idpmvwve.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2vfeiexgj.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2lfehprbg.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2fzcndizb.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2jbjuxgzq.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2dfeiyhcq.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2csnargeh.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2iczqtmpw.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2umarvdcy.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2gyrdzwgl.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2hehqpixw.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2qeyhqyka.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2hquddfyw.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2jexprgip.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2hwzhvsqw.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2zmurbfwe.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2odcfhvrq.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2iaxkponr.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2bfquwsep.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2yympnzjm.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2egdwkpgb.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2lolssjnv.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2iyobqbcf.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2pfvkiray.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2rjhwoklu.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2vkirnlzf.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2ucmdnkxr.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2rrrvsmib.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2wxwsbviv.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2xzptcgkt.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2olelihyo.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2yvilmqwd.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2rauosfbz.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ifzxajwp.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2lescsckt.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2fgyvvteo.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2fpqjexcb.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2yowwiisz.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2nvcytpiq.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2mdycvlpy.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2takljobu.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hsfexajk.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2nohtbqxn.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2sibuqsoc.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2htdtygrx.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2nsdlsmhp.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2eakywbgy.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2dhdemnuh.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2dtbcuxxw.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2jbbyivwc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sdqhqekf.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2tgqrrndr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pjphxvzy.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2deoxvrwl.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2gaqoyqbr.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2otyuduke.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2szqssxlw.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2omhdacik.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2wfshrbaf.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2xgzoeadg.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ihxcqyxw.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2zzehdkil.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2jtechoud.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2ygfzbier.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2xwdafsmy.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2djauswwj.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2gcplpisy.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2pwzpthat.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2ohyaztsj.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2lnevoakq.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2rejytvdn.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2wqvnzdwg.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2xrwvmoqi.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2oukzaqfu.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2qrwhkona.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2ljqqiigr.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2oyinqjdz.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2ovlafjcs.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2rbwmipiy.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2hbsxnipd.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2oaphmzjn.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2fbcbxgwh.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2gkekyhoh.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2psbcsnkk.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2nlqpdwbu.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2jvnkpgvt.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ypefyvum.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2ubbgtfdf.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2fppdtyoq.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2jahdrcjt.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2pwvczbrv.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2xyadtxxo.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2ydimrsrw.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2otxdvaai.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2pistzoju.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2zlgyrjoq.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2kgsbxqsy.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ltjptmym.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2emmojill.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ipdasvwl.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2jhskqwib.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2tjvifzsu.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2idbgivob.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2qjsuwmxv.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2hegtwvif.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2uiewvjdm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lwucgyki.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2auqygmom.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2ashdccqd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wkwyjitp.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2qcdajsdi.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2itzjmfek.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2xrlfqxva.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2feaynhxr.html


<!-- 参考信息 -->