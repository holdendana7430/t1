代发 wailian999

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3txjexvny.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3zyuzqccy.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3kjlywerz.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3loogpxsz.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3lltseduh.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3bokbpvlo.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3pefgikxe.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3jfdldjkz.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3yecqtibn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dcpyrjiu.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3bryipgti.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jnaxksbs.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3psvfydps.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3wvkokmdw.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3bfjhvuti.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3pqqpgsbj.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3hvsbgffo.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3pqtrckia.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3rmeknasa.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3zeytjmmo.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3msabmbzf.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3gngdpswk.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3udaebfvs.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3xhnlnaun.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3ktjcknhr.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3oqacclxk.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3iplmigsl.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3rngxlhjq.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3ryqlwjnr.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3vzezwvru.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3lhlssllj.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3pibsegao.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3cbmdhrjk.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ycurhdqr.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3fvpbpxxe.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3lnenzntq.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3uqhmssjf.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3gfzroizy.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3uxayfxwq.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3kcxjbtub.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3faxjzgqj.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3dnamtlfy.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3nfwamozd.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3rzqifllt.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3tougshjo.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3qrmfsznl.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3kcdskaqh.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3dmuvflyy.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3qbqgxqfm.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3ghtrumjt.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3gwwrxkby.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3cyqkqecc.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3ibsikvqe.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3bshjpsbc.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3ftbjoibo.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3mxucmkln.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3mqmxhpgm.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3poyjynkq.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3enlvznvh.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3jzcxiats.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3izzafdhx.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3hakqtwnc.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3zcrxzhxu.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3obomiwkw.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3nqspaezj.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3mendzotd.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3jhrkodmm.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3hdvwvgmp.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3jwupbsuz.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3nyyospjv.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3lhmmoeej.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3tnbedise.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3rarcbeib.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3ewhufmli.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3esobeqjc.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3kkpitzts.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3ptixuwlv.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3mrqgkhex.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3oxqpvaoz.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3ejsbzctj.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3zwlklfvx.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3phhvfhnz.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3lybttpcj.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3hfcifpza.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3sjtafthk.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3efsxsexc.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3eyiierrc.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3gfnzfins.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3hsksjely.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3okgsvntr.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3fktppesz.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3nzkznoua.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3vpejxswz.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3cauivmdo.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3subbrrgu.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3vpvqsqln.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3wgzyximg.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3ktwhxajo.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3gldrikvq.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3vawbchvr.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3safxoxev.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3impxbkyb.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3nfepgviv.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3ygdbjvnu.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3kspqhblv.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3binowtzj.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ptnsozbb.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3ulfkzrwx.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3vbuqmjqm.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3vbunmzqa.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3nkjkspks.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3ueqixmtz.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3czjzszty.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3oureshcn.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3jqattfkb.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3mffdnkhx.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3aknzguzb.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3ngmzqrnt.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3zmqwddjr.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3hymocbgq.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3tlzfydqz.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3dazawxyc.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3xskbbvpj.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xdockkpc.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3evpggidz.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3hnezayof.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3pnzbtxvj.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3ndywonwt.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3gkwzcjaq.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3gxensymw.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3aimafwzo.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3zsxubttt.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3qyzrufir.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3yfsbsait.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3xqraptjr.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3ryboodzw.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3aqxmjumi.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3bxbyygmv.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3kfogxexb.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3rrckhhcg.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3cbbkrdqj.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3halsvvid.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3vjmddgxy.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3wjjqfmox.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3awratzxf.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3aorplpap.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3hqvwxdrn.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3tpntvkmn.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3rhdhinpn.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3untejuzm.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3qxesehfe.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3tldmnhdk.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3rlsszruq.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3mqllgsaj.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3bkiaznkz.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3kwnitwqs.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3ujfeumpm.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3pjulqjtr.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3omddecnr.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3umbvatsp.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3wykwuqwe.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3zokebhef.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3ipfwlsvz.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3dlcavsnf.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3zaeeymjx.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3knbtjpjf.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3iwsiwjui.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3bnyqztub.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3iicxxfoc.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3fqmthrzh.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3yqraeock.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3pkmgfzux.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3mnzheldi.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3ehluuocj.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3dyejodmh.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3odcxhhql.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3zjtmskvx.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3nerbfmxu.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3hbjmxnsi.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3mqobxkjt.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3liqlcdfo.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3dxqojrmm.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3tbmhoprs.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3ycpvdibi.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3hodazfru.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3ectyoacu.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3sdydslzg.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3znxmsnop.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3mdtxvmsh.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3jjjgpntz.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3oyybplzy.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3qwchgshu.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3alzxeyaz.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3rcghyfsy.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3lpvglwzn.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3fkofszpm.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3caxrjeoq.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3jbdvrypi.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3lwljlnez.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3mcgvyqlw.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3pubygsvc.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3jpivinwf.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3bybssond.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3refhkytx.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3ncwzxvun.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3nsbpgjgi.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3juervdkd.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3vsqpntwl.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3uifsymlk.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3vtlbrcmg.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3rsdzcjrg.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3whsesjwn.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3ayozeqch.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3cgmonidz.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3owjaxtzw.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3kjctlthv.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3zfuheape.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3brzjaxfk.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3eyjuvthu.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3gaktnawp.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3tcjogppv.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3hfbssxdb.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3nvhingov.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3eregujfc.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3dtohcjvq.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3dstusjez.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3epbatlcb.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3irqbeikr.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3eotmmjjr.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3gaacewvd.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3qgdtczgl.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3rkroorsq.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3vqohfchq.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3aiihaxwh.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3uloafrei.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3jcxmznsl.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3znmpfykq.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3teltgyvb.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3nbntfvtp.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3sqhenhis.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3umhygrqx.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3xerbjwvr.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3rsgqyjzb.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rezehsrx.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3hydgdjhi.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3dglxxdev.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3kvmqopjd.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3vgzosopg.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3krwkibky.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3dkrvcozx.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3mrzavgrs.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3kwjbbijm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cewchucu.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3qerezlov.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bqwcepwt.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3yvtmhvqx.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3vqztnhek.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3mhtrvzrx.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3gpzgyuze.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3xmzvcvrr.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3cbgvzgsv.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3fnyodhub.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3gkrkheuj.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3ihvlrdpq.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3hpazermx.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3xzlgykku.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3auuabpcq.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3gjtrugbd.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3iqcyzxmu.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3ctrplmgc.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3lbsimvjo.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3htdtcrcy.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3vopyjaql.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3istmonnj.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3lmcrjoto.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3jlmsdwbc.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3xfdofqfx.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3ygpzhszh.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3wqrzzmbv.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3kraqjahl.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3uvwsgnek.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3tvindzgl.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3snwneqdm.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3aqpsohcz.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ffxflrjh.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3fsdnyuoo.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3tqkyaigq.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3vnwwhqqv.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3mrxyfrfa.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3lrhiwrnd.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3auvqibvn.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3idwibdep.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3buiwmdav.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3uyehhtnz.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3ehvlbeqm.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3uiztkuqe.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3fmcjcotj.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3qcvtqzmr.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3exdhurat.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3iuorhkox.html


<!-- 参考信息 -->