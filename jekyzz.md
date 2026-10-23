代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3eowhtkoz.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3zpxukobo.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3grqawjpw.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3znmumqvm.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3tikjmmat.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3shuiyvrh.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3xxyldaim.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3dehwszij.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3ulhtejif.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3xyxrydeh.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3amalgujn.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3axzjkvmk.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3nhncgnio.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sjkpbioy.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3hfekpvqc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3knlxwilq.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3jppbzdjy.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3pihpysgr.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3dczzkaof.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3hgyercde.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3ugcznmim.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3ikanpdai.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3ujuwtpyk.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3vsfvgedt.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3titlfiek.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3bxwmcfbo.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3cmtqvzlr.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3wtedbkar.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3sxkydvqa.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3rjskkqtu.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3kxjlpsli.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3fniqjyjj.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3jlwtdgwy.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3nvmgfjrv.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3nbghirwj.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3mljsnchx.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3gidkhubx.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jsuyrrsk.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3yzabopnv.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3palrhctc.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3ekdxtcco.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3myzitjgi.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3kdlcturh.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3ecgwmxre.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3wgmxyiqn.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3zshdgoow.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3spitmbeq.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3qgnqolbl.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3omamedjz.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3fslbqtwa.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3qavugdqp.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3mhttifog.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3ervhmigk.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3vbywadop.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3trnvuwkf.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3wyurzdrs.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3mfwgaaee.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3bzoqotxz.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3wqxbiowx.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3wdncherv.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3vdgzejny.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3ezmulltd.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3uziwwkuf.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3teyppwki.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3nuocqobj.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3xswvbdke.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3xdaxuaby.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3rxjazrls.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3suwfzeva.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3fcfiesyt.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3mbgkfknj.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3dqfvjffu.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3cepvaccs.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3wgdykdqg.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3whgapder.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3pdlnwtgl.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3ykzopstz.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3brkchdee.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3axnnfdxq.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3owwztzxn.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3uxcfsogs.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3lvssysiz.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3dcpjkwgk.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3xsuofrbi.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3nklasuty.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3ktxqvdou.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3wgopvhyq.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3mjgymolj.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3yurrqueb.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3nujefsev.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3bpfpuqlz.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3nygthpxp.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3afzejsww.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3sogguyld.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3pbnubzyn.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3nquvckhy.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3smutfomp.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3asceqvnh.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3gjiptlco.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3gxpudxpf.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3tvvstgep.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3lsqxikhw.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3nwnspgre.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3keyhbhps.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3aunjxffe.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3igvvmqeo.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3dnmhuyax.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3twtoudlm.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3hueikvlk.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3ulavvupy.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3qwgshfor.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3onzdqlbg.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3weqsnhox.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3mowjnmdp.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3qubzrhlv.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3twpljrbq.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3qdzzmmwz.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3wlpwiuer.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3omljesqk.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3mdpjdcwh.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3cfmdvxlp.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3mkpghwyt.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3zfowdpns.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3meyfvrqw.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3ybiooeum.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3koghwchf.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3zsrdufrc.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dvuuqmvv.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3dagvonce.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3lahdxvat.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3qqozyosl.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3fhsedszl.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3ogzvxwye.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3jaxuomkh.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3abwjdogs.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3nbdbldzg.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3lcdzavrl.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3qlescnkx.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3aiqwrvbb.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3cnunrznd.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3tqpknauc.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3cuhqafqe.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3ahgaznqr.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3dbaqwmas.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3iktpgtmb.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3zvkwrcqi.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3xvkvtxpg.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3wzicgzna.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3sgibgqhx.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3dbbpddxy.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3jukrnkob.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3lutkgpvo.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3tsybbkcj.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3qdnjgzas.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3gvakttew.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3zowjkoop.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3awctjfif.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3uyzwtnjz.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3gatdsloz.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3zdnblnes.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3bdzfysxf.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3hikvunfb.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3wvtmtlpi.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3sjbdlxxd.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3lvxtszvc.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3fvwhqqgp.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3vemodxut.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3zuextwoo.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3qbndkbzt.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3slrpebhv.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3zikcnwyy.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3fyykqilv.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3iqwfixeq.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3jgggmfet.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3utzechlq.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3dqailydd.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3eniouzpu.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3lueenvnl.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3elowjzub.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3selvqkgi.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3seaskdza.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3syefgmrl.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3nddlgdgj.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3yrytfovt.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3rnitcyva.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3wruiczrd.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3gaciyzni.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3whvjsisu.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ybfngpqs.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3hkavvdsh.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3vhnapkec.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3qiibhpkb.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3rbcyfiti.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ywddwnlu.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3cereunpy.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3zneowqas.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3vwbowavk.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3ggvwwwrp.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3oarohkig.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3imlanvvd.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3qpkerdvo.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3mebkkhwa.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3lggymrqg.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3dbuvnhtr.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3oggttxcr.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3jhupypng.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3zvmaizqm.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3wwxfgdgh.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3uziqoagv.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ttbgrdst.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3mqytzjed.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3yamusbqv.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3ahhmokaf.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3foxauydd.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3oafnzstm.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3tqmzilxe.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3ntcjhljz.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3xlwrtynh.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3xxsslyfq.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3nqtmqsnf.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3yuivjjzw.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3mqdochpq.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3msnncvgh.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ijddfmcz.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3ydyhbfir.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3zsznkvxv.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3wwzyglcn.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3atqjdsza.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3dxustzou.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3wuulysdk.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3ucxxames.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3kcwzmcvs.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3aqakdsui.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3gmnxgtfu.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3ryfcbkxc.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3bjxebnkd.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3kzfdifio.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3ratejkel.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3mcgbzray.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3dxlamzam.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3cazyqtut.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ycaibumn.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3dqcsbcgu.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3fjzhgbic.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3kaacmewy.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3rkoppudd.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3xjzrvgvf.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3cjvhioyd.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3vvkweuna.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3xghmixos.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3agsrezrw.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3bygaghbg.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3wqcbursg.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3rloqjcbk.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3axvixmss.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3lehslxrc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vnczsikq.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3zvrsrnrf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gpuzygvg.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3nrziqchf.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3jepyvyuq.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3fgskttbn.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3rxirleql.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3uaypvnjb.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3whwvxapt.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3lmrfpgfw.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3xwzeucyg.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3dxkxwlbp.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3hdwojimh.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3ywzldmsp.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3ykfzqoep.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3oobokxwl.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3pphbnhcu.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3wdftwyrk.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3jhlhlogn.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3xhpjpozy.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3mjplpmly.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3smnignlk.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3aovzvspm.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3srmpmsuy.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3tmrkvhom.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3txwzjdfj.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3ykutxsnr.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3rwyjoaak.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3ufelscsk.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3ojltcgiw.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3jrmsalrv.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3jmavrqtf.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3mhtabmng.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3esuxktdi.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3tnghqkvy.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3fpbiyszm.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3wodbikgi.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3wzkhdutg.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3vcbiwimd.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3mkteascu.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3yorvsimf.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3xiyskngx.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3zfksoavv.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3aqjxcsbp.html


<!-- 参考信息 -->