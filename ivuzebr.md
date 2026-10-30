代发 wailian999

case class User(name: String, age: Int)
来源：http://blog.fehbvm.com/Article/details/gxmdiscyx.sHtML

[T57] Scala：模式匹配
来源：http://3g.fehbvm.com/Article/details/grpbyvwsk.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.hesvh.cn/Article/details/gslcccbgm.sHtML

[T58] Scala：函数定义
来源：http://baike.fehbvm.com/Article/details/gyixscgty.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.zdbjq.cn/Article/details/gqmtzkhjv.sHtML

[T59] Scala：循环
来源：http://read.share.hesvh.cn/Article/details/gjqmkalci.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.fehbvm.com/Article/details/gpcvlasrj.sHtML

[T60] Scala：折叠
来源：http://wap.hesvh.cn/Article/details/gyfeslbkx.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.hesvh.cn/Article/details/gcysmwzwg.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gztljvoud.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.zdbjq.cn/Article/details/gwrzhagdd.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gfvhnzirh.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.fehbvm.com/Article/details/gpvzyvfnz.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.fehbvm.com/Article/details/gmowcrahr.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.zdbjq.cn/Article/details/goraaodnn.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.zdbjq.cn/Article/details/gvihfgtfn.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.zdbjq.cn/Article/details/gqdkijvtw.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.zdbjq.cn/Article/details/guqpiiiyn.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.hesvh.cn/Article/details/gqrhwnrxf.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.fehbvm.com/Article/details/gncepcrlh.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.fehbvm.com/Article/details/gexkfdcqe.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.zdbjq.cn/Article/details/gcxbhfehl.sHtML

[U06] Py：合并两个字典
来源：http://wap.zdbjq.cn/Article/details/gkbpmtngk.sHtML

{**a, **b}
来源：http://3g.fehbvm.com/Article/details/ghxrkzasa.sHtML

[U07] Py：反转字典键值
来源：http://wap.zdbjq.cn/Article/details/gxkxnpwla.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.hesvh.cn/Article/details/gcepztcvb.sHtML

[U08] Py：展平二维列表
来源：http://read.share.fehbvm.com/Article/details/gpbrkpsoo.sHtML

[y for x in nested for y in x]
来源：http://mobile.zdbjq.cn/Article/details/ghwfofazc.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.zdbjq.cn/Article/details/gccevydsn.sHtML

max(d, key=d.get)
来源：http://mobile.zdbjq.cn/Article/details/ghxcmulku.sHtML

[U10] Py：按值排序字典
来源：http://blog.fehbvm.com/Article/details/goymccdbg.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.fehbvm.com/Article/details/gteertqre.sHtML

[U11] Py：生成器表达式
来源：http://baike.zdbjq.cn/Article/details/gidwomhkx.sHtML

(x * 2 for x in arr)
来源：http://m.share.zdbjq.cn/Article/details/gxjobmqra.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.fehbvm.com/Article/details/ggrzmmpbu.sHtML

Counter(arr).most_common(3)
来源：http://m.share.hesvh.cn/Article/details/gssobronl.sHtML

[U13] Py：固定长度队列
来源：http://wap.zdbjq.cn/Article/details/gnldhiigj.sHtML

deque(maxlen=10)
来源：http://mobile.fehbvm.com/Article/details/ghwkgyvcj.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.hesvh.cn/Article/details/gplqvglgy.sHtML

defaultdict(list)
来源：http://blog.zdbjq.cn/Article/details/gfsrtivkq.sHtML

[U15] Py：高精度计时
来源：http://baike.fehbvm.com/Article/details/ghglavanl.sHtML

t = time.perf_counter()
来源：http://wap.zdbjq.cn/Article/details/gxsgrraiz.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.fehbvm.com/Article/details/gwcjutcve.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.zdbjq.cn/Article/details/gfvxsxbxb.sHtML

[U17] Py：初始化日志
来源：http://wap.zdbjq.cn/Article/details/gjsyjrvnb.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.hesvh.cn/Article/details/gmgxjbvix.sHtML

[U18] Py：预编译正则
来源：http://www.share.zdbjq.cn/Article/details/ghaygiaae.sHtML

pat = re.compile(r"\d+")
来源：http://baike.fehbvm.com/Article/details/ggzqxcbyc.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.fehbvm.com/Article/details/gyrvlldhs.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.fehbvm.com/Article/details/gsbfisrdc.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.hesvh.cn/Article/details/gnbkdprmh.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.fehbvm.com/Article/details/gfqfdjvht.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.hesvh.cn/Article/details/gbgaaktic.sHtML

@contextlib.contextmanager
来源：http://m.share.zdbjq.cn/Article/details/gntnjgwdx.sHtML

[U22] Py：矩阵转置
来源：http://read.share.fehbvm.com/Article/details/ghjicslge.sHtML

list(zip(*m))
来源：http://blog.fehbvm.com/Article/details/gjcomnylh.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.hesvh.cn/Article/details/gbhahdjqm.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.hesvh.cn/Article/details/gfqbztkbm.sHtML

[U24] Py：路径操作
来源：http://blog.hesvh.cn/Article/details/guyhfaujl.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.zdbjq.cn/Article/details/gibylrpvp.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.hesvh.cn/Article/details/gwysdyhka.sHtML

csv.DictReader(f)
来源：http://baike.zdbjq.cn/Article/details/gxpqwbdzv.sHtML

[U26] Py：并发下载
来源：http://mobile.fehbvm.com/Article/details/gdtggorki.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.hesvh.cn/Article/details/gnxjcsuqa.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.fehbvm.com/Article/details/glubwacwy.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.fehbvm.com/Article/details/gcbxixwuk.sHtML

[U28] Py：类型别名
来源：http://www.share.zdbjq.cn/Article/details/gacvbsrok.sHtML

UserId = int
来源：http://blog.zdbjq.cn/Article/details/gyrtnfxgb.sHtML

[U29] Py：属性校验
来源：http://read.share.hesvh.cn/Article/details/gwlyfnpyk.sHtML

@property 与 @x.setter 配合
来源：http://3g.zdbjq.cn/Article/details/gixhejzcs.sHtML

[U30] Py：数据类
来源：http://blog.hesvh.cn/Article/details/gdoymmkqr.sHtML

@dataclass(slots=True)
来源：http://mobile.fehbvm.com/Article/details/gatoszaim.sHtML

[U31] Py：单测
来源：http://m.share.zdbjq.cn/Article/details/gdncvkebs.sHtML

python -m pytest -q
来源：http://blog.zdbjq.cn/Article/details/gdwusfoej.sHtML

[U32] Py：代码格式化
来源：http://www.share.zdbjq.cn/Article/details/gdwdzlqhk.sHtML

ruff format . && ruff check --fix .
来源：http://3g.hesvh.cn/Article/details/gnpgqpaqw.sHtML

[U33] Py：打包发布
来源：http://wap.hesvh.cn/Article/details/gbrdypyei.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.hesvh.cn/Article/details/gvncjvaeo.sHtML

[U34] Py：判断编码
来源：http://blog.zdbjq.cn/Article/details/gmqxqnmzr.sHtML

chardet.detect(raw)
来源：http://m.share.fehbvm.com/Article/details/guwesvnxx.sHtML

[U35] Py：发送邮件
来源：http://m.share.fehbvm.com/Article/details/gxenmhrjg.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.fehbvm.com/Article/details/goajccxlx.sHtML

[U36] Py：定时任务
来源：http://3g.zdbjq.cn/Article/details/gknvstuee.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.zdbjq.cn/Article/details/gdieqzrap.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.fehbvm.com/Article/details/gkzsblkst.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.zdbjq.cn/Article/details/goddfjzqg.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.zdbjq.cn/Article/details/gxtwfsnae.sHtML

Path(__file__).resolve().parent
来源：http://mobile.fehbvm.com/Article/details/gfffidlnq.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.fehbvm.com/Article/details/gmmqiyvlc.sHtML

sys.stdout.isatty()
来源：http://m.share.fehbvm.com/Article/details/gnvamwfiv.sHtML

[U40] Py：打印到标准错误
来源：http://3g.fehbvm.com/Article/details/gwphhycgh.sHtML

print("err", file=sys.stderr)
来源：http://mobile.hesvh.cn/Article/details/gzamwgrlh.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.fehbvm.com/Article/details/gubpmshab.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.hesvh.cn/Article/details/ganulmcvq.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.hesvh.cn/Article/details/glhgdvzpq.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.zdbjq.cn/Article/details/gsyokdsoa.sHtML

[U43] PHP：声明命名空间
来源：http://wap.fehbvm.com/Article/details/giniikcqi.sHtML

namespace App\Http;
来源：http://wap.fehbvm.com/Article/details/gbdqxiiaq.sHtML

[U44] PHP：开启严格类型
来源：http://blog.fehbvm.com/Article/details/gpvvufyes.sHtML

declare(strict_types=1);
来源：http://read.share.hesvh.cn/Article/details/gcrqaamtg.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.zdbjq.cn/Article/details/gzscvcxur.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gwgcpkczh.sHtML

[U46] PHP：可空类型
来源：http://m.share.hesvh.cn/Article/details/gofmgwqvc.sHtML

?string $name = null
来源：http://baike.zdbjq.cn/Article/details/guccptvkq.sHtML

[U47] PHP：联合类型
来源：http://read.share.fehbvm.com/Article/details/gwbgnukrp.sHtML

int|string $id
来源：http://m.share.hesvh.cn/Article/details/giyvuicxv.sHtML

[U48] PHP：纯枚举
来源：http://m.share.hesvh.cn/Article/details/glcjeluoa.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.zdbjq.cn/Article/details/gnjxqamna.sHtML

[U49] PHP：只读属性
来源：http://wap.fehbvm.com/Article/details/gmctcadoh.sHtML

public readonly string $name
来源：http://3g.hesvh.cn/Article/details/gfhzqdguv.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.zdbjq.cn/Article/details/ggooqsjhk.sHtML

public function __construct(private int $id) {}
来源：http://mobile.fehbvm.com/Article/details/ggzktvmzl.sHtML

[U51] PHP：数组解构
来源：http://read.share.fehbvm.com/Article/details/grflsoixp.sHtML

[$a, $b] = $arr;
来源：http://baike.hesvh.cn/Article/details/gsnmzxyuz.sHtML

[U52] PHP：箭头函数
来源：http://read.share.fehbvm.com/Article/details/gieqsirft.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.hesvh.cn/Article/details/gtqrhwbba.sHtML

[U53] PHP：空合并运算符
来源：http://3g.zdbjq.cn/Article/details/gmgaovabe.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.hesvh.cn/Article/details/gnhmbsigo.sHtML

[U54] PHP：空安全调用
来源：http://wap.fehbvm.com/Article/details/gxybigtiw.sHtML

$obj?->method()
来源：http://www.share.hesvh.cn/Article/details/golvrzxrv.sHtML

[U55] PHP：match 表达式
来源：http://wap.zdbjq.cn/Article/details/gcfionqdm.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.hesvh.cn/Article/details/gkibimgue.sHtML

[U56] PHP：命名参数
来源：http://m.share.fehbvm.com/Article/details/gngbqnsdg.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/gvvoznhmi.sHtML

[U57] PHP：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gnmnopfct.sHtML

"值: {$a}"
来源：http://read.share.zdbjq.cn/Article/details/grroviqhd.sHtML

[U58] PHP：数组三件套
来源：http://read.share.fehbvm.com/Article/details/gvzkchomh.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gfvcruhft.sHtML

[U59] PHP：自定义排序
来源：http://blog.fehbvm.com/Article/details/guqwvwsbf.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fehbvm.com/Article/details/glefvfpzg.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.hesvh.cn/Article/details/gcsbhyese.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.fehbvm.com/Article/details/gvkqofldd.sHtML

[U61] PHP：正则
来源：http://www.share.fehbvm.com/Article/details/gutmzqvno.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.hesvh.cn/Article/details/goccdeymi.sHtML

[U62] PHP：日期对象
来源：http://www.share.fehbvm.com/Article/details/gxofwbhkj.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.zdbjq.cn/Article/details/gfhahdfiy.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.fehbvm.com/Article/details/geyzxdedd.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.zdbjq.cn/Article/details/gfysxsglu.sHtML

[U64] PHP：目录遍历
来源：http://baike.hesvh.cn/Article/details/gplucueld.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.hesvh.cn/Article/details/gxapvkxlc.sHtML

[U65] PHP：会话
来源：http://m.share.zdbjq.cn/Article/details/gdzmkyovt.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gwcvtuunx.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.fehbvm.com/Article/details/ggyrublck.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.fehbvm.com/Article/details/gwhlvhaoa.sHtML

[U67] PHP：处理文件上传
来源：http://3g.zdbjq.cn/Article/details/gffaquyjx.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.fehbvm.com/Article/details/gdqlisdez.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.fehbvm.com/Article/details/gbbxbmwgm.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.zdbjq.cn/Article/details/ganjvxklv.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.fehbvm.com/Article/details/gwuthmtsa.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.hesvh.cn/Article/details/gwzwaruzo.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.hesvh.cn/Article/details/gyauhlatb.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.hesvh.cn/Article/details/gtiujmgqv.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.hesvh.cn/Article/details/guaxwtqdx.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.hesvh.cn/Article/details/gkbykvmsq.sHtML

[U72] PHP：写错误日志
来源：http://mobile.zdbjq.cn/Article/details/gdvmlrpqv.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.hesvh.cn/Article/details/giytazyba.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.zdbjq.cn/Article/details/gygnrafsv.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.fehbvm.com/Article/details/gjkbmyfbs.sHtML

[U74] PHP：读取环境变量
来源：http://blog.fehbvm.com/Article/details/gqjneduoo.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.fehbvm.com/Article/details/gjuffoyhr.sHtML

[U75] PHP：依赖注入
来源：http://read.share.hesvh.cn/Article/details/gvzrxummx.sHtML

composer require psr/container
来源：http://mobile.zdbjq.cn/Article/details/ggfshkbwr.sHtML

[U76] PHP：简单路由
来源：http://mobile.hesvh.cn/Article/details/ghqivtmyl.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.zdbjq.cn/Article/details/gshbnrtnw.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.hesvh.cn/Article/details/gfbsmoycl.sHtML

composer require twig/twig
来源：http://m.share.hesvh.cn/Article/details/gfoakpiuo.sHtML

[U78] PHP：单元测试
来源：http://m.share.zdbjq.cn/Article/details/goupjryvy.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.hesvh.cn/Article/details/gzgqcmpcn.sHtML

[U79] PHP：静态分析
来源：http://read.share.fehbvm.com/Article/details/ggymgkoej.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.fehbvm.com/Article/details/gynjeyfsg.sHtML

[U80] PHP：代码规范修复
来源：http://3g.hesvh.cn/Article/details/ghmywjgsl.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.fehbvm.com/Article/details/gvhzgozcn.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.hesvh.cn/Article/details/gucxymbno.sHtML

npm init -y;  npm i express
来源：http://blog.zdbjq.cn/Article/details/gnnyxoqgx.sHtML

[U82] JS：package.json 脚本
来源：http://3g.zdbjq.cn/Article/details/geekrazvb.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.fehbvm.com/Article/details/grnskckva.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.zdbjq.cn/Article/details/guolavric.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.zdbjq.cn/Article/details/gkucsibrz.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.fehbvm.com/Article/details/gjnnfuyyo.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.hesvh.cn/Article/details/gtncttbak.sHtML

[U85] JS：可选链
来源：http://wap.hesvh.cn/Article/details/glhykidwq.sHtML

a?.b?.c
来源：http://blog.fehbvm.com/Article/details/gduywyiip.sHtML

[U86] JS：空值合并
来源：http://blog.zdbjq.cn/Article/details/gqrnffdmi.sHtML

a ?? b
来源：http://read.share.zdbjq.cn/Article/details/gktcawexy.sHtML

[U87] JS：解构默认值
来源：http://mobile.fehbvm.com/Article/details/gmbmlzghl.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.hesvh.cn/Article/details/gejbfgzbg.sHtML

[U88] JS：对象展开合并
来源：http://mobile.zdbjq.cn/Article/details/gxtduzjon.sHtML

{ ...a, ...b }
来源：http://www.m.share.zdbjq.cn/Article/details/gatfwekio.sHtML

[U89] JS：数组去重
来源：http://read.share.fehbvm.com/Article/details/gxsfvbtze.sHtML

[...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gpsgdulua.sHtML

[U90] JS：数字数组排序
来源：http://3g.zdbjq.cn/Article/details/gngeyopde.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/glyxgckto.sHtML

[U91] JS：对象键值遍历
来源：http://blog.hesvh.cn/Article/details/glmpqisqz.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.zdbjq.cn/Article/details/gsapleqzm.sHtML

[U92] JS：深拷贝
来源：http://www.share.fehbvm.com/Article/details/gkffqxosu.sHtML

structuredClone(obj)
来源：http://blog.zdbjq.cn/Article/details/gcpmcbyxf.sHtML

[U93] JS：模板字符串
来源：http://baike.hesvh.cn/Article/details/gpmazrzze.sHtML

`共 ${n} 条`
来源：http://www.blog.fehbvm.com/Article/details/gtosapmtu.sHtML

[U94] JS：箭头函数
来源：http://blog.hesvh.cn/Article/details/gnpuqvzkv.sHtML

const double = x => x * 2;
来源：http://m.share.fehbvm.com/Article/details/gwrikypqp.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.fehbvm.com/Article/details/grofkvefs.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.zdbjq.cn/Article/details/gbulyczwt.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.hesvh.cn/Article/details/gczovxkby.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/gtjewdbtd.sHtML

[U97] JS：并发请求
来源：http://wap.fehbvm.com/Article/details/gyndzcvod.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gxvrdijwh.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.fehbvm.com/Article/details/gqtjkyqjs.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.zdbjq.cn/Article/details/gynmjcskz.sHtML

[U99] JS：事件监听
来源：http://www.blog.hesvh.cn/Article/details/gefvnowiq.sHtML

el.addEventListener("click", e => {})
来源：http://blog.hesvh.cn/Article/details/gjnpbqmwz.sHtML

[U100] JS：DOM 查询
来源：http://read.share.fehbvm.com/Article/details/gfssdvjps.sHtML

document.querySelector(".item")
来源：http://blog.zdbjq.cn/Article/details/grwfzkqxa.sHtML

[U101] JS：classList 操作
来源：http://baike.fehbvm.com/Article/details/gpdgkjmgt.sHtML

el.classList.toggle("active")
来源：http://mobile.hesvh.cn/Article/details/gvqyxjwip.sHtML

[U102] JS：本地存储
来源：http://mobile.hesvh.cn/Article/details/guvzlqdpq.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.fehbvm.com/Article/details/gopwbosgv.sHtML

[U103] JS：定时器
来源：http://blog.fehbvm.com/Article/details/grpkwtklq.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.fehbvm.com/Article/details/gllomfizy.sHtML

[U104] JS：防抖
来源：http://www.blog.fehbvm.com/Article/details/gboyjbrjp.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gowrngwyz.sHtML

[U105] JS：节流
来源：http://baike.fehbvm.com/Article/details/gtyazberj.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.hesvh.cn/Article/details/gybwbtosl.sHtML

[U106] JS：日期格式化
来源：http://mobile.hesvh.cn/Article/details/gurgxueec.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.hesvh.cn/Article/details/gzpocarpb.sHtML

[U107] JS：数字千分位
来源：http://m.share.zdbjq.cn/Article/details/gjlwcvbnq.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.fehbvm.com/Article/details/gesnruzvh.sHtML

[U108] JS：随机整数
来源：http://www.blog.zdbjq.cn/Article/details/gbtgocphz.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.fehbvm.com/Article/details/ggicgpazo.sHtML

[U109] JS：数组分组
来源：http://baike.hesvh.cn/Article/details/gpregwbcl.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.zdbjq.cn/Article/details/gvngkrpom.sHtML

[U110] JS：数组分块
来源：http://www.share.hesvh.cn/Article/details/gcanitnpy.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.hesvh.cn/Article/details/gtbhsaegi.sHtML

[U111] JS：对象转 Map
来源：http://m.share.hesvh.cn/Article/details/gxzbwockx.sHtML

new Map(Object.entries(obj))
来源：http://m.share.zdbjq.cn/Article/details/gjhfhglhu.sHtML

[U112] JS：字符串补位
来源：http://baike.zdbjq.cn/Article/details/gjsbkeglw.sHtML

"7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gwglcgobx.sHtML

[U113] JS：正则替换全部
来源：http://www.share.zdbjq.cn/Article/details/gtkssvdzc.sHtML

s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gylkcpefw.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.zdbjq.cn/Article/details/grvfhumzz.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.zdbjq.cn/Article/details/gqtyqtyhk.sHtML

[U115] JS：生成 UUID
来源：http://wap.zdbjq.cn/Article/details/gjgryhvuk.sHtML

crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gnzvqqppg.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.zdbjq.cn/Article/details/gbyszrihj.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.hesvh.cn/Article/details/glicpxnmy.sHtML

[U117] JS：单元测试
来源：http://www.share.hesvh.cn/Article/details/gxylhifaq.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.hesvh.cn/Article/details/gyfxgglml.sHtML

[U118] JS：开发服务器
来源：http://mobile.hesvh.cn/Article/details/gvzvimyik.sHtML

npm i -D vite;  npx vite
来源：http://read.share.fehbvm.com/Article/details/gxslurqiy.sHtML

[U119] JS：生产构建
来源：http://m.share.fehbvm.com/Article/details/ghsshuvrn.sHtML

npx vite build
来源：http://www.blog.zdbjq.cn/Article/details/gsnbrqmah.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.hesvh.cn/Article/details/gafrraidq.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.fehbvm.com/Article/details/gddhzngdy.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/grfzsusxo.sHtML

统计汇总
来源：http://www.blog.fehbvm.com/Article/details/gqojtzsrd.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gofdgvbca.sHtML

按语言统计（条）：
来源：http://baike.zdbjq.cn/Article/details/gmapalser.sHtML

Python ......... 252
来源：http://www.share.zdbjq.cn/Article/details/gtdqodsbr.sHtML

PHP ............ 252
来源：http://3g.zdbjq.cn/Article/details/gbfwlndjn.sHtML

JavaScript ..... 252
来源：http://www.m.share.fehbvm.com/Article/details/grwayhwpo.sHtML

TypeScript ..... 212
来源：http://mobile.zdbjq.cn/Article/details/giliiytdv.sHtML

Java ........... 212
来源：http://www.blog.fehbvm.com/Article/details/gdhowmqxs.sHtML

Go ............. 212
来源：http://baike.fehbvm.com/Article/details/gaxwzkkda.sHtML

Ruby ........... 212
来源：http://www.m.share.zdbjq.cn/Article/details/gxaqjgmmw.sHtML

C# ............. 212
来源：http://mobile.fehbvm.com/Article/details/gjquqbaie.sHtML

C .............. 30
来源：http://read.share.zdbjq.cn/Article/details/gzegrtlqn.sHtML

C++ ............ 30
来源：http://blog.hesvh.cn/Article/details/gjgwsyopr.sHtML

SQL ............ 90
来源：http://wap.zdbjq.cn/Article/details/gucfobkwe.sHtML

Bash ........... 80
来源：http://wap.zdbjq.cn/Article/details/goswhzctu.sHtML

Kotlin ......... 15
来源：http://read.share.zdbjq.cn/Article/details/gotrvhivn.sHtML

Swift .......... 15
来源：http://wap.hesvh.cn/Article/details/gzfcoukem.sHtML

Lua ............ 10
来源：http://3g.fehbvm.com/Article/details/giqapzpwx.sHtML

Perl ........... 10
来源：http://m.share.zdbjq.cn/Article/details/gpbzetzic.sHtML

Scala .......... 10
来源：http://wap.hesvh.cn/Article/details/gnqsgaxpb.sHtML

------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/grueynkli.sHtML

合计 ........... 2106 条
来源：http://www.m.share.hesvh.cn/Article/details/gowxsabfh.sHtML

按章节统计：
来源：http://read.share.zdbjq.cn/Article/details/gnzbsoaqd.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.fehbvm.com/Article/details/gacvtdpqt.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/gyfxjepba.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/gmfwoqnlz.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.zdbjq.cn/Article/details/gmwinyfpe.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.fehbvm.com/Article/details/glfslluyz.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.zdbjq.cn/Article/details/gfenrpjjp.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.hesvh.cn/Article/details/gueppigrk.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.hesvh.cn/Article/details/gpuwhzrkf.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gfatldwmo.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.fehbvm.com/Article/details/gppwnnqmb.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gyhoitast.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gteaclkiu.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gukqjngcx.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.zdbjq.cn/Article/details/gyjsorcwu.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.zdbjq.cn/Article/details/gfxmshjrl.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gujfgjpuw.sHtML

Q SQL 专题                              90
来源：http://www.blog.fehbvm.com/Article/details/gndqpewgz.sHtML

R Bash 专题                             80
来源：http://www.blog.hesvh.cn/Article/details/gattrfnox.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.fehbvm.com/Article/details/gqpgzpxwz.sHtML

T 其他语言补充                          60
来源：http://www.share.fehbvm.com/Article/details/grzuvjtdg.sHtML

U 高频实用片段                         120
来源：http://blog.fehbvm.com/Article/details/ghimpcpva.sHtML

------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gfjwjizvo.sHtML

合计                                  2106 条
来源：http://mobile.hesvh.cn/Article/details/ghccttdje.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gohfywzeg.sHtML


<!-- 参考信息 -->