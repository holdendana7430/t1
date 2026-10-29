代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://3g.hesvh.cn/Article/details/gmfqvnknq.sHtML

[T55] Scala：集合过滤
来源：http://www.share.hesvh.cn/Article/details/gsdspnotp.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.zdbjq.cn/Article/details/gqllhrwey.sHtML

[T56] Scala：样例类
来源：http://blog.hesvh.cn/Article/details/gxqyvhzxd.sHtML

case class User(name: String, age: Int)
来源：http://www.share.hesvh.cn/Article/details/gnbbcxvsm.sHtML

[T57] Scala：模式匹配
来源：http://blog.hesvh.cn/Article/details/gxroxelzg.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.zdbjq.cn/Article/details/gaayikbou.sHtML

[T58] Scala：函数定义
来源：http://mobile.fehbvm.com/Article/details/gkkfqsqpm.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.hesvh.cn/Article/details/ghdnciamt.sHtML

[T59] Scala：循环
来源：http://wap.fehbvm.com/Article/details/gborviwko.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.hesvh.cn/Article/details/gjoxccfvq.sHtML

[T60] Scala：折叠
来源：http://mobile.zdbjq.cn/Article/details/gqoycffbr.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.hesvh.cn/Article/details/gyscjjgpp.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gcgkufflh.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fehbvm.com/Article/details/gkukgulkf.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gjwdedscy.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.fehbvm.com/Article/details/gfwhbnmqz.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.fehbvm.com/Article/details/gnpextrcd.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.hesvh.cn/Article/details/geitqfahy.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.zdbjq.cn/Article/details/gfptprmps.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.zdbjq.cn/Article/details/gbyftnlzy.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.hesvh.cn/Article/details/gpzotcxvo.sHtML

[U04] Py：变量调试打印
来源：http://baike.hesvh.cn/Article/details/gburvtfya.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.zdbjq.cn/Article/details/guomjjdkv.sHtML

[U05] Py：列表去重且保序
来源：http://blog.fehbvm.com/Article/details/goirlrnwx.sHtML

list(dict.fromkeys(arr))
来源：http://baike.zdbjq.cn/Article/details/ghzmfooqp.sHtML

[U06] Py：合并两个字典
来源：http://wap.fehbvm.com/Article/details/gnnyhzgif.sHtML

{**a, **b}
来源：http://wap.fehbvm.com/Article/details/ghaiuvgmo.sHtML

[U07] Py：反转字典键值
来源：http://3g.zdbjq.cn/Article/details/godrcbkue.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.zdbjq.cn/Article/details/gcfrkkkin.sHtML

[U08] Py：展平二维列表
来源：http://m.share.zdbjq.cn/Article/details/glqletyor.sHtML

[y for x in nested for y in x]
来源：http://3g.hesvh.cn/Article/details/gkhcfzpur.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.hesvh.cn/Article/details/gsnsgwmpq.sHtML

max(d, key=d.get)
来源：http://www.blog.fehbvm.com/Article/details/guishbdwq.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.hesvh.cn/Article/details/gmtavqnai.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.zdbjq.cn/Article/details/gjgokkneg.sHtML

[U11] Py：生成器表达式
来源：http://3g.fehbvm.com/Article/details/gtzyzuzss.sHtML

(x * 2 for x in arr)
来源：http://m.share.fehbvm.com/Article/details/gmlfvcvqo.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.fehbvm.com/Article/details/gxgvmqixs.sHtML

Counter(arr).most_common(3)
来源：http://wap.hesvh.cn/Article/details/ghhfunxff.sHtML

[U13] Py：固定长度队列
来源：http://baike.hesvh.cn/Article/details/gtggzourg.sHtML

deque(maxlen=10)
来源：http://3g.fehbvm.com/Article/details/guakbdiqy.sHtML

[U14] Py：分组收集到列表
来源：http://baike.fehbvm.com/Article/details/gqmchwxow.sHtML

defaultdict(list)
来源：http://wap.hesvh.cn/Article/details/gjfgvtjfz.sHtML

[U15] Py：高精度计时
来源：http://3g.zdbjq.cn/Article/details/gmmjblcql.sHtML

t = time.perf_counter()
来源：http://blog.zdbjq.cn/Article/details/gnqhzcmfj.sHtML

[U16] Py：命令行参数解析
来源：http://baike.zdbjq.cn/Article/details/gxppmhesh.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.hesvh.cn/Article/details/geuzuhcbo.sHtML

[U17] Py：初始化日志
来源：http://baike.zdbjq.cn/Article/details/ggeyncznb.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.hesvh.cn/Article/details/gqhkumzck.sHtML

[U18] Py：预编译正则
来源：http://blog.hesvh.cn/Article/details/gmitrtkap.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.hesvh.cn/Article/details/gvwgkpzkg.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.fehbvm.com/Article/details/gtchjculu.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.hesvh.cn/Article/details/ghmmpkoxx.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.fehbvm.com/Article/details/gcflhlmgh.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.zdbjq.cn/Article/details/gkodqutne.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.zdbjq.cn/Article/details/glwbevgsz.sHtML

@contextlib.contextmanager
来源：http://3g.hesvh.cn/Article/details/gbhaoaemy.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.zdbjq.cn/Article/details/gpldlnlft.sHtML

list(zip(*m))
来源：http://www.share.hesvh.cn/Article/details/gbotpeopv.sHtML

[U23] Py：分块读取大文件
来源：http://baike.hesvh.cn/Article/details/gtyapgyjf.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.zdbjq.cn/Article/details/gyqumfmoo.sHtML

[U24] Py：路径操作
来源：http://3g.zdbjq.cn/Article/details/guhyhwzuj.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.hesvh.cn/Article/details/gyqamytqw.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.hesvh.cn/Article/details/gaxmeavzm.sHtML

csv.DictReader(f)
来源：http://www.blog.zdbjq.cn/Article/details/gwxybhkem.sHtML

[U26] Py：并发下载
来源：http://blog.fehbvm.com/Article/details/gedpoxvwt.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.hesvh.cn/Article/details/gtgvrxpeo.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.fehbvm.com/Article/details/gzozdujmi.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.fehbvm.com/Article/details/gmzkljvfa.sHtML

[U28] Py：类型别名
来源：http://www.share.hesvh.cn/Article/details/gvkuavosq.sHtML

UserId = int
来源：http://baike.fehbvm.com/Article/details/gczisfiwn.sHtML

[U29] Py：属性校验
来源：http://m.share.fehbvm.com/Article/details/gjblsdmmc.sHtML

@property 与 @x.setter 配合
来源：http://wap.zdbjq.cn/Article/details/gkuapuxei.sHtML

[U30] Py：数据类
来源：http://www.share.hesvh.cn/Article/details/gwaveoxel.sHtML

@dataclass(slots=True)
来源：http://www.blog.hesvh.cn/Article/details/gsnvswkyo.sHtML

[U31] Py：单测
来源：http://blog.zdbjq.cn/Article/details/gnxvwrgdm.sHtML

python -m pytest -q
来源：http://mobile.hesvh.cn/Article/details/gdxuerbkp.sHtML

[U32] Py：代码格式化
来源：http://baike.hesvh.cn/Article/details/gejubmrzw.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.zdbjq.cn/Article/details/gdbgwkbuq.sHtML

[U33] Py：打包发布
来源：http://read.share.fehbvm.com/Article/details/gfrhuyedz.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.hesvh.cn/Article/details/gfiskwuln.sHtML

[U34] Py：判断编码
来源：http://read.share.hesvh.cn/Article/details/gqtnfwkuq.sHtML

chardet.detect(raw)
来源：http://wap.fehbvm.com/Article/details/gtgsbbdkd.sHtML

[U35] Py：发送邮件
来源：http://read.share.fehbvm.com/Article/details/govxztnbr.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.fehbvm.com/Article/details/gvgrkxwmz.sHtML

[U36] Py：定时任务
来源：http://www.share.zdbjq.cn/Article/details/gpveqnhxx.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.fehbvm.com/Article/details/gryucozwi.sHtML

[U37] Py：读写 Excel
来源：http://blog.fehbvm.com/Article/details/ggivnyrah.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.fehbvm.com/Article/details/glnvqidnw.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.zdbjq.cn/Article/details/gfpxouojm.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.zdbjq.cn/Article/details/gysjbznqd.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.fehbvm.com/Article/details/goowkrbpi.sHtML

sys.stdout.isatty()
来源：http://blog.fehbvm.com/Article/details/gfjyhdmek.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.fehbvm.com/Article/details/gbpdyovyc.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.zdbjq.cn/Article/details/gduwrewzd.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.hesvh.cn/Article/details/gxugoaltu.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.zdbjq.cn/Article/details/gtcqojxmr.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.zdbjq.cn/Article/details/gaatztguk.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.zdbjq.cn/Article/details/ghwegftpl.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.fehbvm.com/Article/details/gskwajnrc.sHtML

namespace App\Http;
来源：http://wap.hesvh.cn/Article/details/grxpzteqh.sHtML

[U44] PHP：开启严格类型
来源：http://baike.fehbvm.com/Article/details/gfeokdhut.sHtML

declare(strict_types=1);
来源：http://www.m.share.zdbjq.cn/Article/details/gvhnohoil.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.hesvh.cn/Article/details/gbgagkyqv.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/geokokycw.sHtML

[U46] PHP：可空类型
来源：http://3g.zdbjq.cn/Article/details/gyhngohfz.sHtML

?string $name = null
来源：http://read.share.fehbvm.com/Article/details/grrtwsfiq.sHtML

[U47] PHP：联合类型
来源：http://3g.zdbjq.cn/Article/details/gvqgcoshz.sHtML

int|string $id
来源：http://www.m.share.zdbjq.cn/Article/details/gfinrsfdl.sHtML

[U48] PHP：纯枚举
来源：http://3g.zdbjq.cn/Article/details/gtgsvkpep.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.zdbjq.cn/Article/details/gnwpelvek.sHtML

[U49] PHP：只读属性
来源：http://read.share.zdbjq.cn/Article/details/gcvuqftob.sHtML

public readonly string $name
来源：http://wap.hesvh.cn/Article/details/ghpskmlbo.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.fehbvm.com/Article/details/gnqldjhzh.sHtML

public function __construct(private int $id) {}
来源：http://blog.hesvh.cn/Article/details/gfpcwhvlq.sHtML

[U51] PHP：数组解构
来源：http://read.share.zdbjq.cn/Article/details/gwjmmnoeg.sHtML

[$a, $b] = $arr;
来源：http://mobile.hesvh.cn/Article/details/gkzrrzvfp.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.hesvh.cn/Article/details/geiulovwt.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.zdbjq.cn/Article/details/gjdsrmxjg.sHtML

[U53] PHP：空合并运算符
来源：http://3g.hesvh.cn/Article/details/gtbkqgrzh.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.hesvh.cn/Article/details/ggmsiepta.sHtML

[U54] PHP：空安全调用
来源：http://mobile.fehbvm.com/Article/details/gxuwljoal.sHtML

$obj?->method()
来源：http://m.share.hesvh.cn/Article/details/gfutpnikf.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gzcskpdkm.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.zdbjq.cn/Article/details/gpfynajkc.sHtML

[U56] PHP：命名参数
来源：http://mobile.hesvh.cn/Article/details/gayyubsts.sHtML

f(a: 1, b: 2)
来源：http://wap.zdbjq.cn/Article/details/gxebyvovk.sHtML

[U57] PHP：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gqdskqirs.sHtML

"值: {$a}"
来源：http://read.share.zdbjq.cn/Article/details/glvvetykd.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.zdbjq.cn/Article/details/gadfcmpdc.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.zdbjq.cn/Article/details/gsnpixjhf.sHtML

[U59] PHP：自定义排序
来源：http://3g.zdbjq.cn/Article/details/glokayoxp.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.hesvh.cn/Article/details/grhdsofjp.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.fehbvm.com/Article/details/giyeprwlj.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.hesvh.cn/Article/details/gjkatigll.sHtML

[U61] PHP：正则
来源：http://wap.fehbvm.com/Article/details/gdopmqbcl.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.fehbvm.com/Article/details/gysqvabas.sHtML

[U62] PHP：日期对象
来源：http://wap.fehbvm.com/Article/details/gdipkwrmi.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.hesvh.cn/Article/details/gtbtaclkp.sHtML

[U63] PHP：文件读写
来源：http://m.share.hesvh.cn/Article/details/grsqrwdby.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.hesvh.cn/Article/details/gqdassgus.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gzomyypfz.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.fehbvm.com/Article/details/ghrctlhqn.sHtML

[U65] PHP：会话
来源：http://www.share.fehbvm.com/Article/details/gborhadvi.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/glppxfbxe.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.hesvh.cn/Article/details/gtajoaivp.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.fehbvm.com/Article/details/gjelzrxmo.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.zdbjq.cn/Article/details/gxnlzxrvg.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.fehbvm.com/Article/details/gkesccsyi.sHtML

[U68] PHP：PDO 连接
来源：http://wap.zdbjq.cn/Article/details/gdzzdpzij.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.zdbjq.cn/Article/details/ghybydfaz.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.hesvh.cn/Article/details/gjfxtifow.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.fehbvm.com/Article/details/ghlyqbxyb.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.fehbvm.com/Article/details/giykutflp.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.fehbvm.com/Article/details/geozmhvfs.sHtML

[U71] PHP：抛出异常
来源：http://read.share.fehbvm.com/Article/details/gtepctezx.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.fehbvm.com/Article/details/gdtawiqss.sHtML

[U72] PHP：写错误日志
来源：http://blog.zdbjq.cn/Article/details/gwwesbrej.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.hesvh.cn/Article/details/gaxxxogzd.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.zdbjq.cn/Article/details/gekebgndy.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.zdbjq.cn/Article/details/greusvcqz.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.fehbvm.com/Article/details/gopdazuxp.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.hesvh.cn/Article/details/gtzqnwhme.sHtML

[U75] PHP：依赖注入
来源：http://www.share.fehbvm.com/Article/details/gjmgruowd.sHtML

composer require psr/container
来源：http://blog.fehbvm.com/Article/details/ggqrmlweo.sHtML

[U76] PHP：简单路由
来源：http://blog.hesvh.cn/Article/details/gitgwxfsq.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.fehbvm.com/Article/details/ggzqkslkm.sHtML

[U77] PHP：模板渲染
来源：http://3g.zdbjq.cn/Article/details/gxegochhu.sHtML

composer require twig/twig
来源：http://www.m.share.zdbjq.cn/Article/details/grohuyfoe.sHtML

[U78] PHP：单元测试
来源：http://mobile.hesvh.cn/Article/details/gjebcktrn.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.fehbvm.com/Article/details/gwfmcujsd.sHtML

[U79] PHP：静态分析
来源：http://baike.hesvh.cn/Article/details/gjkuwpync.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.zdbjq.cn/Article/details/gsbxyndjk.sHtML

[U80] PHP：代码规范修复
来源：http://baike.zdbjq.cn/Article/details/gpygqiptm.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.hesvh.cn/Article/details/gjvghzclb.sHtML

[U81] JS：初始化项目
来源：http://read.share.hesvh.cn/Article/details/grdqzjsnl.sHtML

npm init -y;  npm i express
来源：http://3g.fehbvm.com/Article/details/gwjbuukjv.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.hesvh.cn/Article/details/gzroevbqe.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.fehbvm.com/Article/details/gdyqnerkp.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.zdbjq.cn/Article/details/gkwbzdsmf.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.zdbjq.cn/Article/details/guuhmjggr.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.hesvh.cn/Article/details/ggarhfjnq.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.hesvh.cn/Article/details/giorbivio.sHtML

[U85] JS：可选链
来源：http://mobile.hesvh.cn/Article/details/gomfomeop.sHtML

a?.b?.c
来源：http://read.share.fehbvm.com/Article/details/gjbytxpeg.sHtML

[U86] JS：空值合并
来源：http://blog.zdbjq.cn/Article/details/gyuneuzvq.sHtML

a ?? b
来源：http://baike.hesvh.cn/Article/details/gabgituta.sHtML

[U87] JS：解构默认值
来源：http://read.share.zdbjq.cn/Article/details/galvkrxwx.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.hesvh.cn/Article/details/gmwqvhgcf.sHtML

[U88] JS：对象展开合并
来源：http://m.share.zdbjq.cn/Article/details/gfgfvkchu.sHtML

{ ...a, ...b }
来源：http://blog.zdbjq.cn/Article/details/gciyalpds.sHtML

[U89] JS：数组去重
来源：http://3g.zdbjq.cn/Article/details/grwzpscpt.sHtML

[...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/gvlhksyis.sHtML

[U90] JS：数字数组排序
来源：http://www.share.hesvh.cn/Article/details/giwmflvoj.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gujdfppfk.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.zdbjq.cn/Article/details/grxufqchc.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.fehbvm.com/Article/details/gqngqmzgt.sHtML

[U92] JS：深拷贝
来源：http://baike.zdbjq.cn/Article/details/gtphunure.sHtML

structuredClone(obj)
来源：http://www.blog.hesvh.cn/Article/details/gmpdlldlp.sHtML

[U93] JS：模板字符串
来源：http://baike.hesvh.cn/Article/details/gvltqfmqj.sHtML

`共 ${n} 条`
来源：http://baike.zdbjq.cn/Article/details/ghraizbvu.sHtML

[U94] JS：箭头函数
来源：http://mobile.zdbjq.cn/Article/details/gobuhtzrv.sHtML

const double = x => x * 2;
来源：http://baike.fehbvm.com/Article/details/gkyorfbun.sHtML

[U95] JS：Promise 包装
来源：http://blog.fehbvm.com/Article/details/gjeinezbf.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.fehbvm.com/Article/details/geriwesel.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.fehbvm.com/Article/details/gmhuwfcsl.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/gmpfectdg.sHtML

[U97] JS：并发请求
来源：http://read.share.fehbvm.com/Article/details/gkrydpwbl.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/gyjpmvucf.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.zdbjq.cn/Article/details/goputuluz.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.zdbjq.cn/Article/details/gchmktxcn.sHtML

[U99] JS：事件监听
来源：http://read.share.fehbvm.com/Article/details/gdduzpkus.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.zdbjq.cn/Article/details/gmawqrnab.sHtML

[U100] JS：DOM 查询
来源：http://read.share.fehbvm.com/Article/details/gnyeaoyzy.sHtML

document.querySelector(".item")
来源：http://3g.zdbjq.cn/Article/details/gazdumowp.sHtML

[U101] JS：classList 操作
来源：http://3g.fehbvm.com/Article/details/gsymvjcjs.sHtML

el.classList.toggle("active")
来源：http://mobile.fehbvm.com/Article/details/gwnwlubly.sHtML

[U102] JS：本地存储
来源：http://read.share.hesvh.cn/Article/details/gtyrpkywz.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.hesvh.cn/Article/details/giotryeir.sHtML

[U103] JS：定时器
来源：http://3g.zdbjq.cn/Article/details/gqoafjsma.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.hesvh.cn/Article/details/gytkrnqqg.sHtML

[U104] JS：防抖
来源：http://3g.fehbvm.com/Article/details/gfqkledog.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/ggfjscliz.sHtML

[U105] JS：节流
来源：http://read.share.fehbvm.com/Article/details/gtfqamopz.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.hesvh.cn/Article/details/gpfzprkxo.sHtML

[U106] JS：日期格式化
来源：http://m.share.zdbjq.cn/Article/details/goziouogf.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.zdbjq.cn/Article/details/gdyojltna.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.zdbjq.cn/Article/details/gziptvmsf.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.hesvh.cn/Article/details/gutjrqarf.sHtML

[U108] JS：随机整数
来源：http://read.share.fehbvm.com/Article/details/gpetcqpsw.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.hesvh.cn/Article/details/gtluhtycx.sHtML

[U109] JS：数组分组
来源：http://mobile.fehbvm.com/Article/details/gpntwbcqy.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.fehbvm.com/Article/details/gdxwavbzh.sHtML

[U110] JS：数组分块
来源：http://blog.zdbjq.cn/Article/details/gjhxkqnkn.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.hesvh.cn/Article/details/gkqnwajja.sHtML

[U111] JS：对象转 Map
来源：http://www.share.fehbvm.com/Article/details/goplepxut.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.fehbvm.com/Article/details/gsmsvywom.sHtML

[U112] JS：字符串补位
来源：http://baike.zdbjq.cn/Article/details/gpuohgzyv.sHtML

"7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/gcalptrye.sHtML

[U113] JS：正则替换全部
来源：http://m.share.fehbvm.com/Article/details/gqirjwupn.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gzwvwtvdu.sHtML

[U114] JS：JSON 深比较
来源：http://blog.fehbvm.com/Article/details/gzpxdrhma.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fehbvm.com/Article/details/gppzzkwhd.sHtML

[U115] JS：生成 UUID
来源：http://blog.zdbjq.cn/Article/details/gkvtlrbyt.sHtML

crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gwofgpjas.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.hesvh.cn/Article/details/gkmjlulbm.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.hesvh.cn/Article/details/gvhbdodgj.sHtML

[U117] JS：单元测试
来源：http://mobile.fehbvm.com/Article/details/glcqruylj.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.fehbvm.com/Article/details/gouxlajpb.sHtML

[U118] JS：开发服务器
来源：http://baike.hesvh.cn/Article/details/gncwaufll.sHtML

npm i -D vite;  npx vite
来源：http://baike.fehbvm.com/Article/details/grldpmtgo.sHtML

[U119] JS：生产构建
来源：http://m.share.hesvh.cn/Article/details/gmydqiamr.sHtML

npx vite build
来源：http://read.share.hesvh.cn/Article/details/gmtvznnoq.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.hesvh.cn/Article/details/getncswud.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.zdbjq.cn/Article/details/giqxvvycy.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gxyhozpfp.sHtML

统计汇总
来源：http://read.share.hesvh.cn/Article/details/gqyceusos.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gjorrifuu.sHtML

按语言统计（条）：
来源：http://wap.zdbjq.cn/Article/details/gquvjwuoc.sHtML

Python ......... 252
来源：http://3g.hesvh.cn/Article/details/goylfljxs.sHtML

PHP ............ 252
来源：http://blog.zdbjq.cn/Article/details/gyqorgccj.sHtML

JavaScript ..... 252
来源：http://3g.fehbvm.com/Article/details/gtqnicwdj.sHtML

TypeScript ..... 212
来源：http://baike.fehbvm.com/Article/details/glsfgpjie.sHtML

Java ........... 212
来源：http://www.m.share.fehbvm.com/Article/details/gdqsiixtq.sHtML

Go ............. 212
来源：http://m.share.fehbvm.com/Article/details/gezeuikmt.sHtML

Ruby ........... 212
来源：http://mobile.zdbjq.cn/Article/details/glbljtxyz.sHtML

C# ............. 212
来源：http://m.share.fehbvm.com/Article/details/gbdhokrmc.sHtML

C .............. 30
来源：http://3g.hesvh.cn/Article/details/gwwiayqey.sHtML

C++ ............ 30
来源：http://3g.hesvh.cn/Article/details/gzllrezdm.sHtML

SQL ............ 90
来源：http://www.m.share.hesvh.cn/Article/details/gylnvwpth.sHtML

Bash ........... 80
来源：http://www.share.fehbvm.com/Article/details/glibvbrds.sHtML

Kotlin ......... 15
来源：http://baike.zdbjq.cn/Article/details/giarjvnzj.sHtML

Swift .......... 15
来源：http://wap.hesvh.cn/Article/details/gmzkdxkqp.sHtML

Lua ............ 10
来源：http://blog.zdbjq.cn/Article/details/gexsvilnt.sHtML

Perl ........... 10
来源：http://wap.zdbjq.cn/Article/details/grkeccxkx.sHtML

Scala .......... 10
来源：http://baike.zdbjq.cn/Article/details/gnwnzeqjc.sHtML

------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gnkjnjbkz.sHtML

合计 ........... 2106 条
来源：http://m.share.fehbvm.com/Article/details/gxhcwctud.sHtML

按章节统计：
来源：http://read.share.fehbvm.com/Article/details/gqnlputcv.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.hesvh.cn/Article/details/gvnwfqkwj.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/gdclqvvjg.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/gnkjjxshw.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.fehbvm.com/Article/details/gxapyoskf.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.fehbvm.com/Article/details/grqedrhig.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.hesvh.cn/Article/details/grptfiuqf.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.zdbjq.cn/Article/details/gzsngitgs.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.zdbjq.cn/Article/details/guogchzso.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gmczpsmoa.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.zdbjq.cn/Article/details/gmlhntowa.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gogwpsyza.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gzfgralat.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gceocbsfa.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.zdbjq.cn/Article/details/gfhoddxvo.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.fehbvm.com/Article/details/ghubzgaws.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gcxkysrwt.sHtML

Q SQL 专题                              90
来源：http://baike.fehbvm.com/Article/details/guhuxpzug.sHtML

R Bash 专题                             80
来源：http://www.blog.fehbvm.com/Article/details/gnplgpjel.sHtML

S C / C++ 专题                          60
来源：http://www.blog.zdbjq.cn/Article/details/gzxcihymc.sHtML

T 其他语言补充                          60
来源：http://www.share.hesvh.cn/Article/details/gfvqiviys.sHtML


<!-- 参考信息 -->