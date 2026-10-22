代发 wailian999

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2ybjtndcs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rzfgmjbc.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ujglqqbj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2srkomyaj.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2uynxqlus.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2ymuxeeyt.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2rroxhnie.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2hfaqllzl.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2ffakhafp.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2mtdhlmrm.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2qciajdcv.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2okkzooyi.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2laxhrrzc.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2cxvubqqa.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2tdwrylaw.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2gcwsrxov.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2oerjowag.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2sbyhxeru.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2ajnjnfhq.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2skazpmyg.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2pyffvpmv.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2uyloyrvu.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2jzxputxc.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2szxsoffe.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2yepwnrmb.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2qlfoaqvi.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2fufttceq.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ojewhipt.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2ctvwoahe.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2hccusjzo.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2sczgoevu.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2tcdiopoc.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2mnjamsoy.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2urivigyk.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2chfdjssm.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2xkjcmsxb.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2bvfkqraq.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2hrvnwfor.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2nwyplwho.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2gfujksas.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2wtoscfol.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2rwbcikly.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2xubjssuv.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2ikhqanpk.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2fugdnisw.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2dbpkvqiw.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2mgnkevcf.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2qqrgomxf.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2pitmlzma.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2gfkvrbgs.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2dlnovpmc.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2pkklpeqr.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2bcacgasn.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2xcremfdr.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2lqlypiie.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2ytzqtidl.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2pvzqxmcg.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2cfrxwxbg.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2fongelzy.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2vkafserx.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2snvmacpk.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2gphyhdbh.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2bfyccpec.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2ukloturx.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2qcrzsyiw.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2dbkvyifc.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2rrdxmlrn.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2xwnjjata.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2gwxuvzsk.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2qlajcnbo.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2rmyqxomb.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2mqrkiipk.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2mxayhfec.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2hqmtbcsr.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2xtrxjfao.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2rlocsahi.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2klvbpqkw.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2mijptjsc.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2lxnlvbwi.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2afsprjit.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2gebhhhpz.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2arqvlbpk.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2hncjxkff.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2fpfnyekz.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2vycearkv.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2prvrrbzq.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2yumzquxm.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2ejmuognd.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2akpqawpl.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2fzwnbyba.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2rcxlglxr.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2qsserybq.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2gsrledwy.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2yuiybdkn.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2nvyblkcw.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2bfghzyfz.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2eiiydblc.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2lxxmgtts.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2uvjwtpas.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sqlscsbs.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2kamihakx.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2kaanypag.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2uzcxncjn.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2kmletsoj.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2jwkmsdbx.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2yoytssyo.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2lthyvluc.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2wkexqutc.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2dvodqccs.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2dvyoiomm.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2zexrscge.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2tiyldrvx.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2nxmrobhs.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2jhuirhix.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2wgqlxyxj.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2xcjdnlgl.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ltbbtfzu.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2epodtcva.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2ouonekxg.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2lkgqkopl.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2aklcjbrs.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2repuoycy.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2mahtkyqw.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ynaejgsv.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2efxmfzmh.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2otovlhan.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2fwfdwskx.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2yeyinbfg.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2wggupqvw.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2uivwdxwo.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2pnlrequx.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2vgrxhkvi.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2kbcpbdjb.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2pwkbltda.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2trazfkij.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2tvxlloti.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2cjwapiwy.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2xfvausyy.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2rctzpthx.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2qegidbou.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2hpxngdsw.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2vepkfety.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2dzqyipki.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2zbbiozmk.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2fhpmcsmo.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2vwjsuuwc.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2ioeskbdi.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2ihdanhpc.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2cjfkmksj.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2zdqblnsx.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2yycahvfz.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2ddrzqyhe.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2nzvveord.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2xpgxaqgh.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2pcjpmzyy.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2hmbconvp.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2hgdxjuxl.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2wlevqwiw.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2zwjyupav.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2nxvkcknl.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2jvudmrtp.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2sopviizx.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2tzmlotod.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2ijmrezwq.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2ecvwawft.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2bsdvmvvo.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2zydmlfst.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2kpakuukx.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2xygyjhke.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2yqdafltz.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2wgatlaoi.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2rymivciu.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2ucqmqant.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2ebkpoqxi.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2nsubtpqt.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2fibnwenq.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2iqimzimo.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2gtzdetfy.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2sauiedrx.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2pigltnng.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2zuvvpiqe.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2vcfjvkyv.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2jtkoyopk.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2qfnzoqbr.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2bgsnewmv.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2dxeglqqq.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2xcyllyaq.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2novrztmw.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2lrcnjdfj.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2qhbuigkg.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2ggqbxlut.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2wttcgwwt.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2zsshpzug.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2uftryofa.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2fcvpmdyj.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2drzhcrim.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2hxcirwne.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ltnscmiw.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2lycoging.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2efjlbumy.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2gwmvbnhr.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2btlmleuv.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2nhffazzv.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2lakcxzvq.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2polwpexb.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2alqulxjm.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2osvczwsu.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2wpjhzmnl.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2biafffbz.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2cjhokexq.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2fmfcgevp.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2meepkbyc.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2hrlhjnqf.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2hsvqmaoq.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ewjeqqnj.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2kiakprbu.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2lpbirufo.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2hsqyexml.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2wknaekza.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2bgxsxfbb.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2zwlktkry.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2ecgmsxnc.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2rzdtjdxz.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2zssylrxy.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2axecqbpv.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2macgyset.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2qvhvzckm.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2aywzakul.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2avsbdavc.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2hjaacxsr.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2najcsawk.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2gwouacmf.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2wejxyvot.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2fdfdtaoy.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2zydvvpgr.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2wlpolaes.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2awwrprcw.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2kmtwcjmx.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2mrvartpa.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2ntghlkam.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2anacosbo.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2sdupohpt.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2qpbruxev.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2ibhxereo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2snmvyoyv.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2uclqdqre.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uybbguij.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2tfrqgmye.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2lszupmpz.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2xuvfuvfs.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2tvivaloi.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2kpubnkar.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2oasewfcb.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2vajqyqpq.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2tpquidoq.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2qfnfcqll.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2mawplhhn.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2zpeohbto.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2qhpsgjbh.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2unlmzdhd.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2xfhklgfr.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2wnhofoxf.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2ucoetxie.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2awgmhdav.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2ffvjmube.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2oetqfxko.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2jbdtqsuc.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2rwoyhpmj.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2fmurhkym.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2mjtfmtjj.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2htxtneda.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2fiyafumc.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2vcqokciy.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2lpxdonpf.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2dlrzelfs.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2evtlzbza.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2pczbmcie.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2shyrhxcp.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2stxrzcgn.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2xxldjxqd.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ibrdnluc.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2kcpqkfls.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2lhztieaf.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2nrmdybmf.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2ojeikzgq.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2ylsbowcf.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2hxotmpcp.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2byhkycgz.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2ppbynpla.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2bdrtdnuu.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2mdzeychv.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2wutlfxwu.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2hyckboci.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2whcohqap.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2rrhyoofw.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2wdsslhme.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2sngmuwki.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2jrwxasov.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2cybdnddd.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2qxuytjyi.html


<!-- 参考信息 -->