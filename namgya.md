代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2wlmwudud.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2epfilloi.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2siqwteky.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2shqghpns.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2igdeoxep.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lpfxodjy.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2udeotlxr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2noedrxqr.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2saedafpy.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2uvhukveu.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2ulfxphns.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jsksfcyz.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2ekyolrfo.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2afkifzsg.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2hszelvmn.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2llfwuocb.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2ohxzzvrw.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2woxyjxmg.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2whhodicm.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2hlocfirh.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2frqfypid.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2haoywbjw.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2ssecnipm.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2fdfuvoeb.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2baosnebx.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2aoimenyt.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2qywcwtfg.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2krpbewjd.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2whryltic.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2xscyctdt.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2moekhnua.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2rlfyolbq.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2izoypeph.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2vxvtbbfk.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2hnthbrkv.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2xzwjgjou.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2etpgfgng.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2qhkjjbjy.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2xydjarfp.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2kpveqwjg.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2stwmfrbz.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2sypzebqp.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2nodgzwnj.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2egkqmela.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2swesnvtg.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2nmsmzhgd.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2pmlybbdq.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2znwqowsd.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2kzhgtjpd.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2yvogaeup.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2sbkqleda.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2lnilbgod.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2suwcnomy.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2pwjyncvt.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2xpomkkca.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2oilbtnut.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2jkjqwutt.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2jeuitlgo.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2ehoxtnmy.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2ebjnxvyl.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2qvelcbzl.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2fsffaiof.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2mnfccjaq.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2bskzxpvd.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2zdfluixu.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2dezgidud.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2lhvbewcr.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ttygjbst.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2clzttfwx.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2zgsjwqnu.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2zcxtppfu.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2eszicrkt.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2xaapmbiu.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2siwestod.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2jkqechvy.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2tfqbsimn.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2uflwazqb.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2skwbbpif.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2zfhldrrq.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2uehrjzvz.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2nudgnmgr.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2htnzswyf.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2xruscunk.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2rigkdxcn.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2urwwgpbg.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2afdwnhvj.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2lfxsnfqn.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2bidibtxt.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2qmwpscgu.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2ajnqhxvn.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2nlpvrgcu.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2vlqbbmtq.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2bmrlqmak.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2kvnhgudm.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2uwzikwvq.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2koxaafdr.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2fbtsieym.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jrvbplsz.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2jevsgmwy.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2ajftxzeg.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2xgyhvmpw.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2fazqjauy.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2llcmrbog.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hwahchhz.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2asjsxjcb.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2lnmqqmrh.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2mdcwoddh.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qmmrdmah.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2jxleiidk.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2qtpttopd.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2byqqrhqi.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2hicnbeng.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2gxnmwqfa.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2xipueijy.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2nibqkjfv.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2tjzbxbuw.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2unoufkgj.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2pbelagoa.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2lpfkeura.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lttzjwum.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2cujqeble.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2fnajaurw.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2mhgwugfv.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2nsapolwq.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2emagbnto.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2ziglgvih.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2dogbcdik.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2iirfhoiz.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2haagzvyh.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2csuygspg.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2obzsquwk.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2zgspbmyx.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2vfakqnwr.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2lxltpcsj.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2onenifyw.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2dtjrutmc.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2nbftladp.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2wblrsbwj.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2pqqprbzi.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2jbxbaaey.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2elbawnfj.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2idzgilmp.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2uiripboq.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2zxncxzor.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2kjkfuwzl.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2zoudpjcs.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2qyxnfldy.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2wqzfaheb.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2mggbmdyg.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2cihfheqm.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2lazphaks.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2jvlegyyn.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2iuaunmhl.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2kmzqqumm.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2bwudozce.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2jayvtjqg.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2nxssvndc.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2bnxhuyho.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2exusrqgy.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2kyzlxtpg.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2yeezkzgu.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2clumride.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2lzopfazh.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2headkeio.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2mvsbcwtd.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2kryuppud.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2tdnkkhqs.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2vaxfngje.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2tmeqzaql.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2pgkimuuf.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2bacwfkew.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2rkwnxvzn.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2tpvnxtqv.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2omlodwkz.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2nqnuhace.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2ebhyqjdj.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2iwbwuauz.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2burxumsn.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2sffrdbcz.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2zhmymauo.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2kpabvxuk.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2exugialw.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2objojjjg.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2gnsvvnir.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2mfjdnovt.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2jwgdzsik.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2mbmltqei.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2jnoaeysv.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2aekzkskv.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2znmyqqjl.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2fykcvwkj.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2aivmsocx.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tldbtgsl.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2mwocxmom.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2qtauzncv.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2cnfusyfb.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2kxpfrxui.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2qhrhbneo.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2wnwbthsv.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2rwgwmtqv.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2yojzardu.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ubboubod.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2gltfoyzh.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2ymagjscp.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2zjuuvthu.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2vmuhqolv.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2xxnqikjc.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2shzxwicc.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2iqlukzrc.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2tbqjrsyi.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2gqnbbmlg.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2ipssfeze.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2murfubzl.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2myrwrppy.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2vgfsmqzy.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2osqgvhgt.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2fnxzpswr.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2lsrsxiuw.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ohyulaye.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2gsebcaxw.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2rpfiojop.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2yxesceir.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2ygnrvppj.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2dwlntqww.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2vjcarfyw.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2sopuqjqm.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2ofrekhtv.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2dicbokal.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2ghmthfkv.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2xjogysnt.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2bircsezp.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2dxethyda.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2lwsykkrq.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2lttiuvsx.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2kiobolmm.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2oxvuxobp.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2pgwpjkfo.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2crcmrqbi.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2ymnavvun.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mfhfqqzt.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2tevrnpir.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2servwxnf.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2zeqiptuu.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2bkqxuzhh.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2hmuzuscx.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2xvajxxxh.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2suicgmss.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2jlomubtr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kpiearzb.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2cpyacflk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xzyaeuxs.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2gxfxmlqm.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2hfgyoypi.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2uwfulcyo.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2bvjbxzvs.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2btduzqun.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2hlabbsql.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2sgkxgprb.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2kguymnre.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2xhqrtglk.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2cxwuqypm.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2hehdpcsb.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2ubhvzgzb.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2hxkfoxat.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2einlgros.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2kljqrmhq.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2xxhwbvek.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2xmarekew.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2gblcidiv.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2hrtghanv.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2ktumnhvo.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2yfhifppn.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2cdvvhkma.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2zakzwreu.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2ekzcfqha.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2kjpqwwbs.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2ixykzswg.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2zgsmxoph.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2xqgjvado.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2twhmfotn.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2lycinrqz.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2inxublxh.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2uxnwutgr.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2szbcuvlf.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2kfpndysm.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2ncfeqyjf.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2nidvdgub.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2hubxnbxj.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2miivlyat.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2wslyroqe.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2dbqdodee.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2yhacauwg.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2mgoekfnb.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2avmfhmha.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2rmystwfp.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ewzqahiv.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2qmfnnakb.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2opomzknh.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2eowvslvw.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2lvrcmbzh.html


<!-- 参考信息 -->