代发 wailian999

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2zqsuytus.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2ipdgmjfw.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2ihofvlqs.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qowvcmwo.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2gbmbyyrq.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2huwpexom.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2ovxszzmg.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2tpoktoeg.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2adqrlwms.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2zrgbsbdw.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2tljzawkd.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2uibcywov.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2ggqoyinb.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2stouzbzq.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2kzngjlts.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2xclayoad.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2mubqxkcy.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2oafezdzo.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2pyrqsvcl.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2oyhegaxf.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2wdkdaquy.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2jzvwxwdj.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2isirmxhw.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2pkmzimdu.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2gvvkioek.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2rgtjcgxp.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2whalvefy.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2mavxicih.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2thabmcls.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2rqliirdi.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2afyfsyln.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2rtrdbmsy.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2fkcwwatd.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2ovubosgx.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2dscabhmu.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2plpmdmeh.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2yzixfjiq.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2dvnjdewp.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2lxnrkrpn.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2gbasdpat.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2hujlzgcd.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2cigucvim.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2pcgddyzx.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2lomhfqfs.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2hetldygm.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2qzlpgrmo.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2lslbovku.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2mllxuvdt.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2padfozqu.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2lceelrxp.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2pumhmzzq.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2pjaweaiy.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2mogbflzm.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2ivvpdncq.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2awypeyyx.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2szidbxxl.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2prrssodb.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2ztbzkdkw.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2cjvycyoa.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2hsvvkxbm.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2jzjnplmn.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2yktmszkc.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2mxrpolbi.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2gwqlwacv.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2gjwnfsbx.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2uvgjikyf.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2yxqnxzxt.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2ipfidzat.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2stcjgvne.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2hgtuofew.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2qpryowep.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2eyakutgd.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2xwfpnidb.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2ftcrohvu.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2yntcbfwf.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2dopbftyx.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2xblqaogj.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2yblzdlhh.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2cxwixzmg.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2bbfnpnlm.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2jxmvvljr.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2ldexrquy.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2iqttnwub.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2vkvhgcrw.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2uthocqnt.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2vurhxuaf.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2okhupdkr.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2kcsattci.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2vcrganxk.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ovmdkimk.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2urnlteae.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2jnuippjp.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2qvxzrzfb.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2oictioqc.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2yipsupph.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2fxnftscp.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2xftfhpiz.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2aoudvbml.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2phhjctpf.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2eesiknty.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2cotdypma.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2momftftl.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2bwugwivu.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2ivqivnsn.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2jsizteym.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2fjyyxdsx.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2ailegpst.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2jignkqvi.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2mesapxmh.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2pynrvulq.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2steakixa.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gfarsnok.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2lqjxqwzl.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2nuhcskis.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2xrficjek.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2exeaebgq.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2pkmjttzl.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2djtcduds.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2wybnlkqs.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2bmuqjgdl.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2efhomdim.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2zuegkhrq.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2sjfjkkei.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2lanluctr.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2dabqytuw.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2licvwkoq.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2pdvmbrkw.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2njzmhtjp.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2nokoegig.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2otzuzoia.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2roehrcby.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2jnkajwgv.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2xscvdjrx.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2wwfidsah.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2lqroosea.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2gcencupi.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2rmiceqqh.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2nqtbkwar.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2sxcpvfij.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2frmhrqop.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2bbhlfkib.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2zhqrfmnz.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2skraslpk.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2suocpnoh.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2ohqbaems.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2fdfkmedo.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2grqtvesc.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2evnayaec.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2aaafgkkn.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2oxvivkdr.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2tvjpiayf.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2mmnwtkpm.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2zxegfskd.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2vbibhevs.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2efljvcuk.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2bodofyyv.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2blobikwx.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2iiozygyx.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2zfuhmiak.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2igiydjwr.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2xnybzzwv.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2xdvnvxek.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2xmvogqwx.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2relijier.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2fqitdjjd.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2iuxxrxjs.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2ldgvnnhu.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2heqmglpu.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2xxsaqdbo.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2brczvcgu.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2zzmcebyi.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2zqwyqyfj.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2rvwohmrs.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2sstioykw.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2ivrsdfvf.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2srtlrgxh.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2ltyleqzf.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2veqhgzyl.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2dwgcydsr.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2eiezbuqs.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jqoavnhw.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2gwgwrtnz.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2xtrdqgyo.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2iqcmltxw.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2lphqzhbt.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2cevoreup.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2dmwyxgue.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2snkewidk.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2tdtguqye.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2blgxykkk.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2exuqavjf.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2pcabgumn.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2oywohbiy.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2psxlhxgc.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2puyukkuk.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2gvibatdr.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2ojflnasq.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2cgegbxnl.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2zofxxckt.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2egsockhh.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2sdpxhufl.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2ulhvhxsb.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2bnnezmpy.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2dmszunjl.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2dknfsiru.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2muoeelno.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2pqwhnirx.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2xwggwxxs.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2emooodlx.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2zshmfqvt.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2cuijzxfg.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2yogjjctx.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2siowqyza.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2aqniznfe.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2orrrugmx.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2cymmjnjg.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2zbvoegcj.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2fzynduqc.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2xzbggebd.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2wiehhjvg.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2cjpaswav.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2xmrvtkvu.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2ojabigfa.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2jmxhrhnl.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2fxovhgnd.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2grbtbwkk.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2nuuazrdy.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2zrthyrmu.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2dgsrqhbe.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2utnitbjb.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2qikuydmb.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2uxhpxgfi.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2lzgjwnfk.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2mdxvtnfg.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2uiqjnljg.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2ccatzbuo.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2tzslcsyl.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2nabhbsms.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2subaayqu.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2xeppefbv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oplfzanr.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2semcldng.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ztlwwnbh.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2ozziddrg.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2mxrjzhsf.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2sxgluafy.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2hdvtcyhp.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2kdoawhzb.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2bohupgii.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2lzoxtcbw.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2tlpaofho.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2trigpuky.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2oxkjmohk.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2jinzvtqs.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2tbzfveny.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2ukiptczq.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2qakahtmm.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2qjuwkigs.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2sssdjsoe.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2cdqwohrx.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2iazdwlxw.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2zmsfizpi.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2cywinfps.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2mbhibwln.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2szvjvogj.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2ajmjrwsy.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2talpjpic.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2wbhblheq.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2fttrzbxa.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2hxgdobbi.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2fihlnlnm.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2uvbmtumv.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2xuruzoqs.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2xqfqseyg.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2kxreoqvm.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2mpbvhrml.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2nqqvpqeq.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2vszkrojd.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2bvcnfgho.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2cjarmqxn.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2gnfyhutx.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2fvzbomeb.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2oincffaa.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2kdcnjqov.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2gmbmjigq.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2admohksf.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2cketxust.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2uloamcwh.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2bshnftiu.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2mxaoacgj.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2oedkcrka.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2uzwqipet.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2omocxvxs.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2wxiglfcl.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2dokkjdkr.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2ybdnxfhv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bceruowy.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2alnlxkbs.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2ticzttdc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jpdpxruo.html


<!-- 参考信息 -->