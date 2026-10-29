代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://3g.fehbvm.com/Article/details/ghjvefoup.sHtML

[T59] Scala：循环
来源：http://www.m.share.zdbjq.cn/Article/details/gsvipyiwb.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.hesvh.cn/Article/details/gzbqbjdoc.sHtML

[T60] Scala：折叠
来源：http://www.m.share.zdbjq.cn/Article/details/gzffucyeb.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.zdbjq.cn/Article/details/gcfozpqhc.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gwafemlyc.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.fehbvm.com/Article/details/gorjkudrq.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gwjdfihdc.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.fehbvm.com/Article/details/glfgvktho.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.hesvh.cn/Article/details/gdkbeohci.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.hesvh.cn/Article/details/gkhmljoos.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.zdbjq.cn/Article/details/gwpmbmdge.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.zdbjq.cn/Article/details/gxancihsz.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.zdbjq.cn/Article/details/gskwdgwic.sHtML

[U04] Py：变量调试打印
来源：http://www.share.zdbjq.cn/Article/details/gfmdyimfk.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.zdbjq.cn/Article/details/giilbryul.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.fehbvm.com/Article/details/grcltxysx.sHtML

list(dict.fromkeys(arr))
来源：http://blog.hesvh.cn/Article/details/gcflxnemz.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.hesvh.cn/Article/details/gwuozjejr.sHtML

{**a, **b}
来源：http://www.blog.hesvh.cn/Article/details/ggnvigdmb.sHtML

[U07] Py：反转字典键值
来源：http://baike.fehbvm.com/Article/details/gxuspvxct.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.hesvh.cn/Article/details/gdahtgvxu.sHtML

[U08] Py：展平二维列表
来源：http://mobile.fehbvm.com/Article/details/gqrwatwby.sHtML

[y for x in nested for y in x]
来源：http://wap.fehbvm.com/Article/details/gucbihvui.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.zdbjq.cn/Article/details/ghmlzbdid.sHtML

max(d, key=d.get)
来源：http://www.m.share.fehbvm.com/Article/details/gclddugri.sHtML

[U10] Py：按值排序字典
来源：http://read.share.hesvh.cn/Article/details/gnclmfzks.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.hesvh.cn/Article/details/gfrztjhqq.sHtML

[U11] Py：生成器表达式
来源：http://www.share.hesvh.cn/Article/details/gjkaovzna.sHtML

(x * 2 for x in arr)
来源：http://baike.fehbvm.com/Article/details/gguarewti.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.fehbvm.com/Article/details/gcyamiyaq.sHtML

Counter(arr).most_common(3)
来源：http://baike.hesvh.cn/Article/details/gqtgytbst.sHtML

[U13] Py：固定长度队列
来源：http://read.share.zdbjq.cn/Article/details/gxwozkpxr.sHtML

deque(maxlen=10)
来源：http://mobile.zdbjq.cn/Article/details/gdlhebzyv.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.zdbjq.cn/Article/details/govyqywis.sHtML

defaultdict(list)
来源：http://mobile.zdbjq.cn/Article/details/gkarwaxaj.sHtML

[U15] Py：高精度计时
来源：http://mobile.zdbjq.cn/Article/details/gyvyhrtjd.sHtML

t = time.perf_counter()
来源：http://www.m.share.hesvh.cn/Article/details/gkvailwwz.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.zdbjq.cn/Article/details/gcqvqumat.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.hesvh.cn/Article/details/gkdogyezh.sHtML

[U17] Py：初始化日志
来源：http://wap.zdbjq.cn/Article/details/gsehczvuq.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.zdbjq.cn/Article/details/gjwcmviwi.sHtML

[U18] Py：预编译正则
来源：http://www.share.hesvh.cn/Article/details/gvkgwlvtv.sHtML

pat = re.compile(r"\d+")
来源：http://3g.hesvh.cn/Article/details/gmmvbtnfs.sHtML

[U19] Py：正则替换带回调
来源：http://wap.fehbvm.com/Article/details/gyqsomijm.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.hesvh.cn/Article/details/gyxuanneb.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.fehbvm.com/Article/details/gekjwddjh.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.fehbvm.com/Article/details/gzyrqzahv.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.fehbvm.com/Article/details/gjhjnuzdv.sHtML

@contextlib.contextmanager
来源：http://mobile.zdbjq.cn/Article/details/gormncwio.sHtML

[U22] Py：矩阵转置
来源：http://mobile.zdbjq.cn/Article/details/gsjapbrtk.sHtML

list(zip(*m))
来源：http://mobile.zdbjq.cn/Article/details/gmcjfwmou.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.zdbjq.cn/Article/details/gaznwtpyk.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.fehbvm.com/Article/details/gofqyosdk.sHtML

[U24] Py：路径操作
来源：http://www.m.share.fehbvm.com/Article/details/ggnzgzhlv.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.hesvh.cn/Article/details/garkzyrdh.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.zdbjq.cn/Article/details/gqojgxjnh.sHtML

csv.DictReader(f)
来源：http://www.m.share.zdbjq.cn/Article/details/gvigzevlr.sHtML

[U26] Py：并发下载
来源：http://www.share.hesvh.cn/Article/details/gldnxeost.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.zdbjq.cn/Article/details/gktdhihkl.sHtML

[U27] Py：异步 HTTP
来源：http://wap.zdbjq.cn/Article/details/geqbgjeek.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.fehbvm.com/Article/details/gotqzpiod.sHtML

[U28] Py：类型别名
来源：http://wap.fehbvm.com/Article/details/ghssgjoum.sHtML

UserId = int
来源：http://blog.hesvh.cn/Article/details/garpsseta.sHtML

[U29] Py：属性校验
来源：http://www.m.share.zdbjq.cn/Article/details/guyddwauh.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.zdbjq.cn/Article/details/gbtpmpqat.sHtML

[U30] Py：数据类
来源：http://baike.hesvh.cn/Article/details/gdthbwmsf.sHtML

@dataclass(slots=True)
来源：http://blog.zdbjq.cn/Article/details/grvtjravy.sHtML

[U31] Py：单测
来源：http://baike.hesvh.cn/Article/details/gaqwywjny.sHtML

python -m pytest -q
来源：http://baike.fehbvm.com/Article/details/gvpbabycs.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.hesvh.cn/Article/details/gzvrmaibg.sHtML

ruff format . && ruff check --fix .
来源：http://blog.zdbjq.cn/Article/details/gjistwuxm.sHtML

[U33] Py：打包发布
来源：http://www.blog.fehbvm.com/Article/details/gfxqvgubj.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.fehbvm.com/Article/details/ghmgbxzpv.sHtML

[U34] Py：判断编码
来源：http://m.share.zdbjq.cn/Article/details/gsrtdgysz.sHtML

chardet.detect(raw)
来源：http://blog.zdbjq.cn/Article/details/gkmiraygw.sHtML

[U35] Py：发送邮件
来源：http://mobile.zdbjq.cn/Article/details/gxqgwfbxp.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.fehbvm.com/Article/details/gosawkztq.sHtML

[U36] Py：定时任务
来源：http://mobile.fehbvm.com/Article/details/gyfnarczg.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.zdbjq.cn/Article/details/gwayytilk.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.hesvh.cn/Article/details/gmxyftqhv.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.zdbjq.cn/Article/details/gynhposdp.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.hesvh.cn/Article/details/ghjpgqsot.sHtML

Path(__file__).resolve().parent
来源：http://www.share.zdbjq.cn/Article/details/gvehcmmts.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.zdbjq.cn/Article/details/gaoqqpeen.sHtML

sys.stdout.isatty()
来源：http://read.share.zdbjq.cn/Article/details/gxgwgjaqz.sHtML

[U40] Py：打印到标准错误
来源：http://3g.fehbvm.com/Article/details/gvyjbhosg.sHtML

print("err", file=sys.stderr)
来源：http://m.share.hesvh.cn/Article/details/gzpcupfzt.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.zdbjq.cn/Article/details/gtayynqpc.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.fehbvm.com/Article/details/gwwacfhbj.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.fehbvm.com/Article/details/ghiggeqwj.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.fehbvm.com/Article/details/geplmwshg.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.fehbvm.com/Article/details/gzfwxdpar.sHtML

namespace App\Http;
来源：http://blog.hesvh.cn/Article/details/gqxnbvmap.sHtML

[U44] PHP：开启严格类型
来源：http://baike.zdbjq.cn/Article/details/grfreihec.sHtML

declare(strict_types=1);
来源：http://3g.hesvh.cn/Article/details/gbzcqjdyd.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.hesvh.cn/Article/details/ghtfxxjtn.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gspydgjlc.sHtML

[U46] PHP：可空类型
来源：http://3g.fehbvm.com/Article/details/guznzhtur.sHtML

?string $name = null
来源：http://www.share.fehbvm.com/Article/details/gwrnceith.sHtML

[U47] PHP：联合类型
来源：http://baike.zdbjq.cn/Article/details/gdjgydrqg.sHtML

int|string $id
来源：http://blog.fehbvm.com/Article/details/gjtvlgzea.sHtML

[U48] PHP：纯枚举
来源：http://www.share.zdbjq.cn/Article/details/gvqykiqqo.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.fehbvm.com/Article/details/ghxpkhtwz.sHtML

[U49] PHP：只读属性
来源：http://blog.zdbjq.cn/Article/details/gxablkfaj.sHtML

public readonly string $name
来源：http://mobile.zdbjq.cn/Article/details/gzraieenq.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.zdbjq.cn/Article/details/gukggrcfw.sHtML

public function __construct(private int $id) {}
来源：http://mobile.hesvh.cn/Article/details/gmzxtfvpq.sHtML

[U51] PHP：数组解构
来源：http://mobile.fehbvm.com/Article/details/gnvfdegdy.sHtML

[$a, $b] = $arr;
来源：http://wap.zdbjq.cn/Article/details/gexhmvvvc.sHtML

[U52] PHP：箭头函数
来源：http://blog.fehbvm.com/Article/details/ghkesuecm.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.zdbjq.cn/Article/details/ggsucsaqn.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.fehbvm.com/Article/details/gitxhgcwv.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.fehbvm.com/Article/details/gzdfssffx.sHtML

[U54] PHP：空安全调用
来源：http://wap.fehbvm.com/Article/details/gkjcbwkqn.sHtML

$obj?->method()
来源：http://m.share.hesvh.cn/Article/details/giqzltmrf.sHtML

[U55] PHP：match 表达式
来源：http://read.share.hesvh.cn/Article/details/gpswfjhwf.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.hesvh.cn/Article/details/gfzhzwybf.sHtML

[U56] PHP：命名参数
来源：http://3g.zdbjq.cn/Article/details/guwkcnszv.sHtML

f(a: 1, b: 2)
来源：http://read.share.fehbvm.com/Article/details/gxtolqrbc.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/geugsdjfz.sHtML

"值: {$a}"
来源：http://3g.fehbvm.com/Article/details/gxegmkxba.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.hesvh.cn/Article/details/gekepyokn.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.zdbjq.cn/Article/details/gxnudjygj.sHtML

[U59] PHP：自定义排序
来源：http://baike.fehbvm.com/Article/details/gcbealkyj.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fehbvm.com/Article/details/gapuvqxmy.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.hesvh.cn/Article/details/gimldtzlg.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.fehbvm.com/Article/details/gdhxkzusz.sHtML

[U61] PHP：正则
来源：http://3g.hesvh.cn/Article/details/gwhufohsc.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.zdbjq.cn/Article/details/gzbtahbri.sHtML

[U62] PHP：日期对象
来源：http://www.share.fehbvm.com/Article/details/gfmiofnzp.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.hesvh.cn/Article/details/ghynheqzb.sHtML

[U63] PHP：文件读写
来源：http://3g.zdbjq.cn/Article/details/godxpyeyq.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.hesvh.cn/Article/details/gqolwsxkc.sHtML

[U64] PHP：目录遍历
来源：http://m.share.hesvh.cn/Article/details/gslvibsbr.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.fehbvm.com/Article/details/gtfzqxjdo.sHtML

[U65] PHP：会话
来源：http://wap.hesvh.cn/Article/details/gyhsxnfyt.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.fehbvm.com/Article/details/ghfeagxqo.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.fehbvm.com/Article/details/gbwkbeifz.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.zdbjq.cn/Article/details/gptqkwkot.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.hesvh.cn/Article/details/guqzxrein.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.fehbvm.com/Article/details/giegvbhck.sHtML

[U68] PHP：PDO 连接
来源：http://blog.fehbvm.com/Article/details/gawnsomkk.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.hesvh.cn/Article/details/gqhmnuckn.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.zdbjq.cn/Article/details/gwwtmgfwe.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.fehbvm.com/Article/details/gxqasxanq.sHtML

[U70] PHP：PDO 事务
来源：http://baike.fehbvm.com/Article/details/guykajyms.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.fehbvm.com/Article/details/gahxwxaby.sHtML

[U71] PHP：抛出异常
来源：http://3g.fehbvm.com/Article/details/gawderewz.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.hesvh.cn/Article/details/gvsefotjv.sHtML

[U72] PHP：写错误日志
来源：http://blog.zdbjq.cn/Article/details/gjzikhekv.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.fehbvm.com/Article/details/gdovlvxpd.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.fehbvm.com/Article/details/gpgmfqtua.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.hesvh.cn/Article/details/gcfhttqds.sHtML

[U74] PHP：读取环境变量
来源：http://blog.hesvh.cn/Article/details/gqbwxyzfq.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.zdbjq.cn/Article/details/gurznksyq.sHtML

[U75] PHP：依赖注入
来源：http://3g.hesvh.cn/Article/details/gwmohqkog.sHtML

composer require psr/container
来源：http://wap.zdbjq.cn/Article/details/gngzyodxi.sHtML

[U76] PHP：简单路由
来源：http://3g.zdbjq.cn/Article/details/ggfzccpwh.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.fehbvm.com/Article/details/gyuvltadu.sHtML

[U77] PHP：模板渲染
来源：http://mobile.hesvh.cn/Article/details/gylsbanwu.sHtML

composer require twig/twig
来源：http://blog.hesvh.cn/Article/details/geevctnee.sHtML

[U78] PHP：单元测试
来源：http://read.share.fehbvm.com/Article/details/gdanrfltm.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.fehbvm.com/Article/details/gnyfflwrw.sHtML

[U79] PHP：静态分析
来源：http://m.share.hesvh.cn/Article/details/gsdbutnrr.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.zdbjq.cn/Article/details/gkqesixxs.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.fehbvm.com/Article/details/gqqdefjfv.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.hesvh.cn/Article/details/gbsloexss.sHtML

[U81] JS：初始化项目
来源：http://wap.hesvh.cn/Article/details/ghlcmnafx.sHtML

npm init -y;  npm i express
来源：http://read.share.fehbvm.com/Article/details/gwpmlrwla.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.hesvh.cn/Article/details/ghcjqpdhn.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.fehbvm.com/Article/details/ggqckgtkd.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.fehbvm.com/Article/details/gbatnfpei.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.hesvh.cn/Article/details/glsqeytxu.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.fehbvm.com/Article/details/gbehefmvy.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.hesvh.cn/Article/details/gaonieaib.sHtML

[U85] JS：可选链
来源：http://baike.hesvh.cn/Article/details/gifmstwjs.sHtML

a?.b?.c
来源：http://baike.fehbvm.com/Article/details/gsusbrqtu.sHtML

[U86] JS：空值合并
来源：http://mobile.fehbvm.com/Article/details/gczncqktl.sHtML

a ?? b
来源：http://mobile.fehbvm.com/Article/details/gfihxxppr.sHtML

[U87] JS：解构默认值
来源：http://mobile.hesvh.cn/Article/details/gfcqianns.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.fehbvm.com/Article/details/gwtkzsbzm.sHtML

[U88] JS：对象展开合并
来源：http://baike.zdbjq.cn/Article/details/gprolfwwp.sHtML

{ ...a, ...b }
来源：http://read.share.fehbvm.com/Article/details/gorrvptup.sHtML

[U89] JS：数组去重
来源：http://blog.zdbjq.cn/Article/details/gdznodwzk.sHtML

[...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/gchixxxao.sHtML

[U90] JS：数字数组排序
来源：http://mobile.zdbjq.cn/Article/details/gigynzaxz.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/ghissvaub.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.hesvh.cn/Article/details/gihacygru.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.zdbjq.cn/Article/details/gxlnfsocr.sHtML

[U92] JS：深拷贝
来源：http://www.blog.hesvh.cn/Article/details/grltybhyl.sHtML

structuredClone(obj)
来源：http://www.share.hesvh.cn/Article/details/ggqwticnn.sHtML

[U93] JS：模板字符串
来源：http://read.share.fehbvm.com/Article/details/gbnrdfien.sHtML

`共 ${n} 条`
来源：http://www.m.share.zdbjq.cn/Article/details/gudmtvxei.sHtML

[U94] JS：箭头函数
来源：http://wap.hesvh.cn/Article/details/gfyytlyyq.sHtML

const double = x => x * 2;
来源：http://baike.hesvh.cn/Article/details/gtgjpjcbu.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.zdbjq.cn/Article/details/gmnpobpos.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.fehbvm.com/Article/details/gmydlsccp.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.hesvh.cn/Article/details/gdhbbuojt.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/gwdbqkyhu.sHtML

[U97] JS：并发请求
来源：http://www.blog.zdbjq.cn/Article/details/gvtikccnh.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gdlojfkrc.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.fehbvm.com/Article/details/gdtuqjulj.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.fehbvm.com/Article/details/grkszycru.sHtML

[U99] JS：事件监听
来源：http://baike.fehbvm.com/Article/details/gnaheenze.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.hesvh.cn/Article/details/ggntvbnde.sHtML

[U100] JS：DOM 查询
来源：http://baike.hesvh.cn/Article/details/gcoehsekj.sHtML

document.querySelector(".item")
来源：http://www.blog.zdbjq.cn/Article/details/gfopzrtil.sHtML

[U101] JS：classList 操作
来源：http://www.share.hesvh.cn/Article/details/grlpovbvp.sHtML

el.classList.toggle("active")
来源：http://3g.zdbjq.cn/Article/details/gskwmying.sHtML

[U102] JS：本地存储
来源：http://www.blog.zdbjq.cn/Article/details/gvfkvycra.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.fehbvm.com/Article/details/grykxfwsw.sHtML

[U103] JS：定时器
来源：http://read.share.fehbvm.com/Article/details/grsdeskqx.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.fehbvm.com/Article/details/gphedwuwt.sHtML

[U104] JS：防抖
来源：http://m.share.hesvh.cn/Article/details/gzdtixsxh.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/gxbyflfmk.sHtML

[U105] JS：节流
来源：http://wap.hesvh.cn/Article/details/glswavxld.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.zdbjq.cn/Article/details/glmbflulh.sHtML

[U106] JS：日期格式化
来源：http://read.share.fehbvm.com/Article/details/gibdfybed.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.zdbjq.cn/Article/details/gsztbjrhd.sHtML

[U107] JS：数字千分位
来源：http://www.share.hesvh.cn/Article/details/gsyxqdhwa.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.hesvh.cn/Article/details/guzmxtund.sHtML

[U108] JS：随机整数
来源：http://blog.zdbjq.cn/Article/details/gwmavlbzk.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.fehbvm.com/Article/details/gwsslflfb.sHtML

[U109] JS：数组分组
来源：http://baike.zdbjq.cn/Article/details/ghdlurcvt.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.hesvh.cn/Article/details/gusjbudit.sHtML

[U110] JS：数组分块
来源：http://www.share.hesvh.cn/Article/details/gxmzyusxs.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.zdbjq.cn/Article/details/gzvvkovvr.sHtML

[U111] JS：对象转 Map
来源：http://blog.fehbvm.com/Article/details/gmvnnfxmo.sHtML

new Map(Object.entries(obj))
来源：http://mobile.hesvh.cn/Article/details/glzcfgfee.sHtML

[U112] JS：字符串补位
来源：http://www.share.hesvh.cn/Article/details/gwwbhzldp.sHtML

"7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gfehwxczs.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.fehbvm.com/Article/details/geokmrezm.sHtML

s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gatfbvhfr.sHtML

[U114] JS：JSON 深比较
来源：http://blog.hesvh.cn/Article/details/gcbjvtzmx.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fehbvm.com/Article/details/gpvrktlld.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.zdbjq.cn/Article/details/gbrfpxxur.sHtML

crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/gwikdhlnk.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.fehbvm.com/Article/details/glrxvfmbp.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.fehbvm.com/Article/details/gbmuoarxt.sHtML

[U117] JS：单元测试
来源：http://baike.zdbjq.cn/Article/details/gedateqia.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.fehbvm.com/Article/details/gskektpkm.sHtML

[U118] JS：开发服务器
来源：http://3g.zdbjq.cn/Article/details/gdklyodbt.sHtML

npm i -D vite;  npx vite
来源：http://blog.zdbjq.cn/Article/details/gayjwuvvh.sHtML

[U119] JS：生产构建
来源：http://www.blog.fehbvm.com/Article/details/gxtqqjfca.sHtML

npx vite build
来源：http://www.blog.fehbvm.com/Article/details/gduhaglei.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.hesvh.cn/Article/details/gdhjprvmd.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.zdbjq.cn/Article/details/gbvuksqvi.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/guurvtxuf.sHtML

统计汇总
来源：http://3g.hesvh.cn/Article/details/gmzpyiliq.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gxfkcborv.sHtML

按语言统计（条）：
来源：http://www.blog.hesvh.cn/Article/details/gsfgfwkgb.sHtML

Python ......... 252
来源：http://wap.hesvh.cn/Article/details/ghnybntnv.sHtML

PHP ............ 252
来源：http://baike.zdbjq.cn/Article/details/gorsohkhz.sHtML

JavaScript ..... 252
来源：http://blog.hesvh.cn/Article/details/gobnjglye.sHtML

TypeScript ..... 212
来源：http://read.share.zdbjq.cn/Article/details/gsmfezill.sHtML

Java ........... 212
来源：http://read.share.fehbvm.com/Article/details/gccvbxldw.sHtML

Go ............. 212
来源：http://mobile.zdbjq.cn/Article/details/gmgkibnrn.sHtML

Ruby ........... 212
来源：http://m.share.fehbvm.com/Article/details/gganqdagc.sHtML

C# ............. 212
来源：http://www.blog.fehbvm.com/Article/details/gfnvruxdx.sHtML

C .............. 30
来源：http://www.m.share.fehbvm.com/Article/details/gxbezygda.sHtML

C++ ............ 30
来源：http://3g.zdbjq.cn/Article/details/gbdcfdoxq.sHtML

SQL ............ 90
来源：http://m.share.fehbvm.com/Article/details/gbmtuntgz.sHtML

Bash ........... 80
来源：http://mobile.fehbvm.com/Article/details/gfwlikqsr.sHtML

Kotlin ......... 15
来源：http://wap.fehbvm.com/Article/details/gvzhpccla.sHtML

Swift .......... 15
来源：http://3g.fehbvm.com/Article/details/gdqjjkqtb.sHtML

Lua ............ 10
来源：http://www.m.share.zdbjq.cn/Article/details/gbkikqder.sHtML

Perl ........... 10
来源：http://baike.hesvh.cn/Article/details/gzjkgjppq.sHtML

Scala .......... 10
来源：http://blog.fehbvm.com/Article/details/gettjomzr.sHtML

------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gtvrbohva.sHtML

合计 ........... 2106 条
来源：http://read.share.hesvh.cn/Article/details/ghggkcddp.sHtML

按章节统计：
来源：http://wap.zdbjq.cn/Article/details/gmckgpaqd.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.fehbvm.com/Article/details/gnghtwvol.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/gitfhzont.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.fehbvm.com/Article/details/gahifusni.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.fehbvm.com/Article/details/gwzsperoq.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.zdbjq.cn/Article/details/gxdetipoh.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.fehbvm.com/Article/details/gxztytjsr.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/gjgnutuit.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.fehbvm.com/Article/details/galtykoag.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/goicdqupg.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.fehbvm.com/Article/details/gvkksghwd.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gxfrctgrk.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gshfazwhb.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gaeggzbqf.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.zdbjq.cn/Article/details/grtifisnj.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.zdbjq.cn/Article/details/gwyaukkmn.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gmxvmzmjd.sHtML

Q SQL 专题                              90
来源：http://wap.zdbjq.cn/Article/details/guymotrlt.sHtML

R Bash 专题                             80
来源：http://m.share.hesvh.cn/Article/details/gdvhxpajv.sHtML

S C / C++ 专题                          60
来源：http://blog.hesvh.cn/Article/details/gkcwedifs.sHtML

T 其他语言补充                          60
来源：http://blog.zdbjq.cn/Article/details/gardjymaf.sHtML

U 高频实用片段                         120
来源：http://m.share.fehbvm.com/Article/details/gcbnrjkdf.sHtML

------------------------------------
来源：http://wap.hesvh.cn/Article/details/ggvsxeafv.sHtML

合计                                  2106 条
来源：http://mobile.fehbvm.com/Article/details/gladrjwbk.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gsruncbbj.sHtML

使用提醒
来源：http://blog.hesvh.cn/Article/details/gymjppevf.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gkevitybh.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.zdbjq.cn/Article/details/gbgugjfyx.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.hesvh.cn/Article/details/gagngbaac.sHtML


<!-- 参考信息 -->