代发 wailian999

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2dcymjbzv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2datzddgl.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2fsvagjfj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hrogxdlk.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2gkkmsggu.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2laxagpzi.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2ykohetry.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2kcqlqjeh.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2jmkqzoao.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2fxusntol.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2qdtvbvme.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2pvlxzrkb.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2flhauhpi.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2qcjmnkck.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2jfnukkrj.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2tpigsodj.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2mriowfyq.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2ytnztlkj.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2jwxhqmwj.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2iksaacyy.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2dwaghsvf.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2lueysssz.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2zueqfjsb.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2tboqvcfj.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2awqnlasd.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gtbwvpwb.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2gwlhvevz.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2bljldouz.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2hudumpyd.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2pezagtzb.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2bhdkdbdm.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2uqtzolnx.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2msvjhrse.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2kbqywhrr.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2gripbxwi.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2ffjxltaa.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2qbsnopux.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2xiezqeya.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2fyigryie.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2ijzlfalu.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2ftuvkhsm.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2tltvxbhk.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2ypztjgvf.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2qbbzdjkx.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2gwvzuyqb.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2kbctikvo.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2gptmrspv.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2zjevjljc.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2tvmarrib.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2vygrnjcw.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2psbyhnth.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2vqfnrydv.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2zplirpxu.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2rshxnzuy.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2vzptesmf.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2qocodfws.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2wmmggzzy.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2ufsivwuk.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2tapaikkj.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2pgdauwrw.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2ldpwpksa.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2arbgrinb.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2oybbowqk.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2ezbzjwgd.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2vflgwnnj.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2cxqxyqtu.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2cdiodssp.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2ydgtuqrn.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2wlfzmdvv.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2aoeiqihv.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2bundpdwo.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2kdognagp.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2yxbafzxf.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2vgasyqgn.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2hyefdqog.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2dufydmmq.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2roagkjxn.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2vkiwzxhc.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2ktsjsbom.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2jphrdzaw.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2keukgncl.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2jvsulcfy.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2cofbncwa.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2vaktbsfw.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2reypefaa.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2gypnzwpc.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2wdxocltv.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2nsgjjoju.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2vwileedb.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2rbtvmjgt.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2nwixoacw.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2huzxqkuu.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2kjuxggtk.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2vrfzxpkw.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2blwqkwdo.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2ysediabx.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2ydvldivd.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2svcnlvil.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2ediafxca.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2stuidrpc.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2satucbks.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2dwwikuzc.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2bgxosyjh.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ckhdqflf.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2dhtezcvq.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2nttjysqf.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2xjtqhodx.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2qufcycnn.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2xfrysmzf.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2cmlrsuoh.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2myqaxefc.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2saypywqr.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2alkvvwmi.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2ftmgfgzn.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2gkfkgzir.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2cbodhzrl.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2oklujnbd.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2ogpvsdaf.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2glaczcss.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2dctigyfr.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2sciowhgk.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2qcsdgawj.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2gzjrvlwf.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2gcvpneqf.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2unxgyyln.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2piwxqnbb.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2kmbeahhw.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2fjafoorz.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2jejyzflz.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2qwpqciom.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zrlfovrb.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2tartvtdj.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2nskqsqod.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2cfbauxio.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2elkqtxib.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2tdtpkphf.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2tbvaulgh.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2tkzsbfql.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2nlnaaqtt.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2iiripste.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2soqwfkel.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2xbvpfzca.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2ffhtibwh.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2cgsghnys.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2dwlywlrx.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2tjwrnvyt.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2drekwmzl.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2pwimesmn.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2yqvqythi.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2ydjkmgjg.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2tleajzfw.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2kgzanyfk.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2ujtrixxj.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2fbyayqng.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2jpwbyizk.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2rinjfpch.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2prnobwni.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2btrounhf.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2hxahlwhj.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2ryevmvwz.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2knuprvdy.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2joqvhisf.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2fcactefd.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2wznhcyio.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2zrvijjyk.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2dlbozvyq.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2xqrinklh.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2nxwozmok.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2vbvddlim.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2nuudyddx.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2fdrqgcrw.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2ddxgqsuj.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2ganhdbdj.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2ojaezvsz.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2bbpbebsu.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2isagcuvt.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2rrjbvekm.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2zdcfazjo.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2mxvkqapq.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2mtjecixb.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2ghogreet.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2pkptvbms.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2rxrvubjh.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2zlmlhpdh.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vxyjhkhq.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2ckjqaomg.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2sgdeggyp.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2kllbjwci.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2owuiregj.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2votcqtrd.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2fgunjydy.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2vfphlkzm.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2pyrjgnvs.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2gluoydji.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2boksesql.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2goqifwxj.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2lnrfommk.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2msudhwew.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2rxvbwzmx.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2mtndjwca.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2hrqcwfvp.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2bpacfrhd.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2sqnudddh.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2teaymwdy.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2aiolgzqr.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2qhvmvciz.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2ndtovlcs.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2rgogvhkv.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2mpqooyrj.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2qdxuejwq.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2mwmfxrrt.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2soamlifr.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2znewusmw.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2taqhtcdp.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2vaaruhoi.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2ouymfzfe.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2liwfuzsk.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2xdudvfba.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2prnsbqbd.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2kqxpfmur.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2ukekbeyy.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2vykqatpd.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2zuxayvlu.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2mmlkuzwl.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2ttuwrgyj.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2hccttpmp.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2yokjdxwt.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2yflwelcn.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2dxpsbokb.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2bkjvcwml.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2jzxogewa.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2goyfprvj.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2bbhuhaqw.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2njdpthgc.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2hiisnqxj.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2qhcyvjti.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2rgupahqf.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2oulqobxl.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2oyvmdwks.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2sgbtpumf.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2emjsnfjw.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2ekwjewts.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2moksdvgh.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2ixlvzzkv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aubjysku.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2hqnzfmhc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lwiibkaf.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2zqokxiyq.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2qieduprm.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2epjovmcf.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2jpwazvqs.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2quscnray.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2oenyggzk.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2sgxtlpoz.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2zyrziabe.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2uheowyrs.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2bbtsxtmv.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2vblwpfwh.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2zgxinmrf.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2ivzpgmch.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2uirnqldy.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2kshvpqwi.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2dnazkklh.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2ckzyiotf.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2nsgovdod.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2nwydthgw.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2voxxvuki.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2twuhpzdx.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2tiiiqeuc.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2sbnpbwxq.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2nzziahuq.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2klewityr.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2amtovbfv.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2vvytilqn.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2yyudioia.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2aljlyfjb.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2xvgxxuaa.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2obuevrzy.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2wgdrvkpe.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2etoyijne.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2kueanoiq.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2idsynsgs.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2axpmdcqn.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2oifzxvft.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2nyxvxagi.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2mzibvsry.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2payhywfb.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2kjaebevs.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2dccvmhbx.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2rwtsxnow.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2nujhlgmq.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2gtrcevuq.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2iidcngea.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2cacldrrx.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2piajyxuv.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2dkfigshd.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2zhkttrts.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2srkcvyqo.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2nfpqeetw.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2rbsnlpvc.html


<!-- 参考信息 -->