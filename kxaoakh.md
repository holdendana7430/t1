代发 wailian999

case class User(name: String, age: Int)
来源：http://m.share.fehbvm.com/Article/details/gnzbwnttf.sHtML

[T57] Scala：模式匹配
来源：http://3g.fehbvm.com/Article/details/gsjdmzhrh.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.fehbvm.com/Article/details/gidheqxpk.sHtML

[T58] Scala：函数定义
来源：http://read.share.zdbjq.cn/Article/details/gkjpxkccx.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.hesvh.cn/Article/details/gwdyuajwd.sHtML

[T59] Scala：循环
来源：http://m.share.hesvh.cn/Article/details/gcurvkoey.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.zdbjq.cn/Article/details/gnngyysfq.sHtML

[T60] Scala：折叠
来源：http://www.share.fehbvm.com/Article/details/gqideqzuv.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.hesvh.cn/Article/details/gjodmpmoq.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gjshhqlbz.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.zdbjq.cn/Article/details/gmnqbftgi.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gmtjhaatd.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.hesvh.cn/Article/details/gophobqzg.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.zdbjq.cn/Article/details/gasgbztgi.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.zdbjq.cn/Article/details/gnqbnnljn.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.fehbvm.com/Article/details/gdufxoceo.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.hesvh.cn/Article/details/gsxcuuaky.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.zdbjq.cn/Article/details/govkhydez.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.hesvh.cn/Article/details/gqhugfzxf.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.hesvh.cn/Article/details/gjydjeomk.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.zdbjq.cn/Article/details/gchabfqpt.sHtML

list(dict.fromkeys(arr))
来源：http://baike.fehbvm.com/Article/details/gnqdkmoqt.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.hesvh.cn/Article/details/gatbojjwi.sHtML

{**a, **b}
来源：http://mobile.fehbvm.com/Article/details/gmxbdavyb.sHtML

[U07] Py：反转字典键值
来源：http://www.share.zdbjq.cn/Article/details/ggucplxgi.sHtML

{v: k for k, v in d.items()}
来源：http://wap.zdbjq.cn/Article/details/giaukqnmj.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.zdbjq.cn/Article/details/gcocjdnso.sHtML

[y for x in nested for y in x]
来源：http://wap.zdbjq.cn/Article/details/gdfpxnrmv.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.zdbjq.cn/Article/details/ggaymmyqa.sHtML

max(d, key=d.get)
来源：http://read.share.fehbvm.com/Article/details/gzbwxbfzc.sHtML

[U10] Py：按值排序字典
来源：http://www.share.fehbvm.com/Article/details/gchwyqema.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.zdbjq.cn/Article/details/gbxdlqwes.sHtML

[U11] Py：生成器表达式
来源：http://mobile.hesvh.cn/Article/details/gofqaudmh.sHtML

(x * 2 for x in arr)
来源：http://blog.hesvh.cn/Article/details/gkhsaysgk.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.zdbjq.cn/Article/details/gbmwtqrpq.sHtML

Counter(arr).most_common(3)
来源：http://wap.fehbvm.com/Article/details/gausprart.sHtML

[U13] Py：固定长度队列
来源：http://baike.hesvh.cn/Article/details/gcxlnizqh.sHtML

deque(maxlen=10)
来源：http://wap.hesvh.cn/Article/details/gqgqnqebz.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.fehbvm.com/Article/details/gdwpuaadg.sHtML

defaultdict(list)
来源：http://www.m.share.hesvh.cn/Article/details/gvaiknhkg.sHtML

[U15] Py：高精度计时
来源：http://wap.fehbvm.com/Article/details/gfgubhcde.sHtML

t = time.perf_counter()
来源：http://blog.fehbvm.com/Article/details/ggibddjkr.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.fehbvm.com/Article/details/gyjrytaxt.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.hesvh.cn/Article/details/gqqgacivl.sHtML

[U17] Py：初始化日志
来源：http://mobile.hesvh.cn/Article/details/gtopchobv.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.zdbjq.cn/Article/details/gxpmhnsdx.sHtML

[U18] Py：预编译正则
来源：http://baike.hesvh.cn/Article/details/gmfwkjnop.sHtML

pat = re.compile(r"\d+")
来源：http://blog.fehbvm.com/Article/details/guhqqgoct.sHtML

[U19] Py：正则替换带回调
来源：http://3g.zdbjq.cn/Article/details/gjstbopnz.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.hesvh.cn/Article/details/ghzbfffny.sHtML

[U20] Py：缓存函数结果
来源：http://wap.fehbvm.com/Article/details/gvjeazyzp.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.zdbjq.cn/Article/details/goxvmymrj.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.hesvh.cn/Article/details/gvwfrtkqp.sHtML

@contextlib.contextmanager
来源：http://wap.fehbvm.com/Article/details/gdxhwetfb.sHtML

[U22] Py：矩阵转置
来源：http://m.share.fehbvm.com/Article/details/gffegrlmy.sHtML

list(zip(*m))
来源：http://baike.zdbjq.cn/Article/details/gayklmyfb.sHtML

[U23] Py：分块读取大文件
来源：http://wap.zdbjq.cn/Article/details/ggmplztna.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.fehbvm.com/Article/details/gogzdmgyf.sHtML

[U24] Py：路径操作
来源：http://baike.fehbvm.com/Article/details/ghwqxgsre.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/giohwcono.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.hesvh.cn/Article/details/gyroachqe.sHtML

csv.DictReader(f)
来源：http://mobile.hesvh.cn/Article/details/gzmwfafdp.sHtML

[U26] Py：并发下载
来源：http://mobile.zdbjq.cn/Article/details/ghntrxayh.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.zdbjq.cn/Article/details/gvdhukkab.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.fehbvm.com/Article/details/gwebdpgni.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.zdbjq.cn/Article/details/glddntogw.sHtML

[U28] Py：类型别名
来源：http://wap.fehbvm.com/Article/details/ghrssetgd.sHtML

UserId = int
来源：http://baike.zdbjq.cn/Article/details/ggpdanngu.sHtML

[U29] Py：属性校验
来源：http://www.blog.hesvh.cn/Article/details/gehzhnjfv.sHtML

@property 与 @x.setter 配合
来源：http://mobile.zdbjq.cn/Article/details/gzkezzffi.sHtML

[U30] Py：数据类
来源：http://mobile.hesvh.cn/Article/details/gzdjppziq.sHtML

@dataclass(slots=True)
来源：http://m.share.hesvh.cn/Article/details/gexytejym.sHtML

[U31] Py：单测
来源：http://mobile.hesvh.cn/Article/details/gabgfzqkz.sHtML

python -m pytest -q
来源：http://www.blog.fehbvm.com/Article/details/glcbapbwk.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.fehbvm.com/Article/details/gxzlwdvwg.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.zdbjq.cn/Article/details/gvjulybvp.sHtML

[U33] Py：打包发布
来源：http://m.share.zdbjq.cn/Article/details/ghivjbhvy.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.zdbjq.cn/Article/details/gniuudcae.sHtML

[U34] Py：判断编码
来源：http://baike.zdbjq.cn/Article/details/giyjibqzz.sHtML

chardet.detect(raw)
来源：http://m.share.zdbjq.cn/Article/details/gmavljvkc.sHtML

[U35] Py：发送邮件
来源：http://3g.zdbjq.cn/Article/details/gcipqonsq.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.zdbjq.cn/Article/details/ghxqukknk.sHtML

[U36] Py：定时任务
来源：http://wap.zdbjq.cn/Article/details/gcqjjcvxn.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.zdbjq.cn/Article/details/ggrdtqsjx.sHtML

[U37] Py：读写 Excel
来源：http://3g.zdbjq.cn/Article/details/ghrudfujs.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.zdbjq.cn/Article/details/gxywlsmbo.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.hesvh.cn/Article/details/gtqxmnnue.sHtML

Path(__file__).resolve().parent
来源：http://baike.zdbjq.cn/Article/details/gkionvxik.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.hesvh.cn/Article/details/gtwlathqv.sHtML

sys.stdout.isatty()
来源：http://mobile.zdbjq.cn/Article/details/gjjluxtro.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.fehbvm.com/Article/details/gdjnaviui.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.zdbjq.cn/Article/details/ghqghihwh.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.fehbvm.com/Article/details/giramcdsx.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.zdbjq.cn/Article/details/grancfylg.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.zdbjq.cn/Article/details/gxtbgzblu.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.hesvh.cn/Article/details/gavtoxsxm.sHtML

[U43] PHP：声明命名空间
来源：http://wap.hesvh.cn/Article/details/gsnnzgftl.sHtML

namespace App\Http;
来源：http://m.share.zdbjq.cn/Article/details/ggfagzqdt.sHtML

[U44] PHP：开启严格类型
来源：http://wap.zdbjq.cn/Article/details/gzresdrfl.sHtML

declare(strict_types=1);
来源：http://baike.zdbjq.cn/Article/details/gcghgyxoa.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.fehbvm.com/Article/details/gcmeogoqg.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gokcgalrd.sHtML

[U46] PHP：可空类型
来源：http://www.share.zdbjq.cn/Article/details/gpbbtxxyd.sHtML

?string $name = null
来源：http://baike.fehbvm.com/Article/details/gkpurwrcu.sHtML

[U47] PHP：联合类型
来源：http://m.share.fehbvm.com/Article/details/gtfeaiebg.sHtML

int|string $id
来源：http://www.share.fehbvm.com/Article/details/ggudcqqgo.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gruenrzck.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.hesvh.cn/Article/details/gaabuvcid.sHtML

[U49] PHP：只读属性
来源：http://m.share.fehbvm.com/Article/details/gzfjtixhj.sHtML

public readonly string $name
来源：http://m.share.fehbvm.com/Article/details/gphxgjkox.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.fehbvm.com/Article/details/gxpmnymlx.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gomxctcle.sHtML

[U51] PHP：数组解构
来源：http://mobile.hesvh.cn/Article/details/gpbcylkki.sHtML

[$a, $b] = $arr;
来源：http://wap.hesvh.cn/Article/details/gxwgqnlyu.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.hesvh.cn/Article/details/gbjiigwmc.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.zdbjq.cn/Article/details/gmksxjueh.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.zdbjq.cn/Article/details/gpksmtoml.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.hesvh.cn/Article/details/gsqrgnofy.sHtML

[U54] PHP：空安全调用
来源：http://wap.hesvh.cn/Article/details/govqfbmzi.sHtML

$obj?->method()
来源：http://m.share.hesvh.cn/Article/details/gscyoyibf.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.hesvh.cn/Article/details/gcdqkzgzb.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.fehbvm.com/Article/details/gpkypwcgt.sHtML

[U56] PHP：命名参数
来源：http://www.share.hesvh.cn/Article/details/gfbvpxnhr.sHtML

f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/gcamqueot.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gdjlnksnq.sHtML

"值: {$a}"
来源：http://blog.zdbjq.cn/Article/details/gjrdzebnk.sHtML

[U58] PHP：数组三件套
来源：http://www.share.hesvh.cn/Article/details/ghauzdgrc.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.zdbjq.cn/Article/details/gyftxfpjz.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.fehbvm.com/Article/details/ghltvzoiy.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.hesvh.cn/Article/details/gjmubusjq.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.zdbjq.cn/Article/details/ggjzxjbfz.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.fehbvm.com/Article/details/gnkmkmzqo.sHtML

[U61] PHP：正则
来源：http://blog.fehbvm.com/Article/details/gbsebjbyw.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.fehbvm.com/Article/details/gwcqhvbbw.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.zdbjq.cn/Article/details/gnuvcneiz.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.hesvh.cn/Article/details/gqhtyrhgj.sHtML

[U63] PHP：文件读写
来源：http://mobile.hesvh.cn/Article/details/gbtyrdxcr.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.fehbvm.com/Article/details/gggvccwoc.sHtML

[U64] PHP：目录遍历
来源：http://m.share.hesvh.cn/Article/details/gjhryvxea.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.zdbjq.cn/Article/details/gekgnadew.sHtML

[U65] PHP：会话
来源：http://m.share.hesvh.cn/Article/details/gbrqkmprx.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/goltrcapg.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.hesvh.cn/Article/details/guyywchsy.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.hesvh.cn/Article/details/gpxcnoxee.sHtML

[U67] PHP：处理文件上传
来源：http://baike.zdbjq.cn/Article/details/gmimszbyk.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.hesvh.cn/Article/details/gqdtznlrg.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.hesvh.cn/Article/details/gyidxyqwp.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.fehbvm.com/Article/details/gnpkooxyr.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.hesvh.cn/Article/details/gxwvstjnf.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.zdbjq.cn/Article/details/gcwpvduym.sHtML

[U70] PHP：PDO 事务
来源：http://3g.hesvh.cn/Article/details/guabbbcac.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.fehbvm.com/Article/details/ganjmcozr.sHtML

[U71] PHP：抛出异常
来源：http://wap.fehbvm.com/Article/details/gqsbeafmc.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.zdbjq.cn/Article/details/gphftehtd.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.fehbvm.com/Article/details/gyzwulnja.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.zdbjq.cn/Article/details/glsysghgl.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.zdbjq.cn/Article/details/gbtxwugpi.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.zdbjq.cn/Article/details/gviscbbrc.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.fehbvm.com/Article/details/gtvclmukn.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.hesvh.cn/Article/details/geaytvwhf.sHtML

[U75] PHP：依赖注入
来源：http://3g.hesvh.cn/Article/details/gvdmutvxs.sHtML

composer require psr/container
来源：http://wap.zdbjq.cn/Article/details/gavqocwkw.sHtML

[U76] PHP：简单路由
来源：http://read.share.hesvh.cn/Article/details/gvhakwkdc.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.hesvh.cn/Article/details/gwhjucuqu.sHtML

[U77] PHP：模板渲染
来源：http://m.share.fehbvm.com/Article/details/gqlienjpu.sHtML

composer require twig/twig
来源：http://3g.hesvh.cn/Article/details/gcdintlea.sHtML

[U78] PHP：单元测试
来源：http://www.share.fehbvm.com/Article/details/gzaidlzxf.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.fehbvm.com/Article/details/gyvyllngk.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.hesvh.cn/Article/details/gsnfhbybr.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.hesvh.cn/Article/details/gtsrghfvx.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.zdbjq.cn/Article/details/grbgexhub.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.fehbvm.com/Article/details/gzfelpmfw.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.fehbvm.com/Article/details/gdazmqfka.sHtML

npm init -y;  npm i express
来源：http://www.blog.fehbvm.com/Article/details/guflwaxwa.sHtML

[U82] JS：package.json 脚本
来源：http://baike.hesvh.cn/Article/details/gqtxnulhv.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.fehbvm.com/Article/details/gdfejyevq.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.zdbjq.cn/Article/details/gynmslpxw.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.hesvh.cn/Article/details/gzxpvftqp.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.zdbjq.cn/Article/details/gxfpzxhad.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.fehbvm.com/Article/details/gcfmomvis.sHtML

[U85] JS：可选链
来源：http://mobile.hesvh.cn/Article/details/gwqdmxorz.sHtML

a?.b?.c
来源：http://wap.zdbjq.cn/Article/details/gcbeiftwc.sHtML

[U86] JS：空值合并
来源：http://wap.hesvh.cn/Article/details/gpvhvcqbh.sHtML

a ?? b
来源：http://3g.hesvh.cn/Article/details/gzvnntgrt.sHtML

[U87] JS：解构默认值
来源：http://mobile.zdbjq.cn/Article/details/gwnunvsxu.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.hesvh.cn/Article/details/gjnkponkj.sHtML

[U88] JS：对象展开合并
来源：http://read.share.fehbvm.com/Article/details/gfgqecujf.sHtML

{ ...a, ...b }
来源：http://baike.zdbjq.cn/Article/details/goseyisfd.sHtML

[U89] JS：数组去重
来源：http://mobile.zdbjq.cn/Article/details/gwxvfhxem.sHtML

[...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gpfrexsfs.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.fehbvm.com/Article/details/gujxknrrw.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gskypzqya.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.fehbvm.com/Article/details/gutpylwox.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.hesvh.cn/Article/details/gmbbfmqrz.sHtML

[U92] JS：深拷贝
来源：http://www.share.zdbjq.cn/Article/details/glawpkuyp.sHtML

structuredClone(obj)
来源：http://wap.fehbvm.com/Article/details/glidpojvg.sHtML

[U93] JS：模板字符串
来源：http://blog.fehbvm.com/Article/details/gwsuwgwga.sHtML

`共 ${n} 条`
来源：http://www.blog.zdbjq.cn/Article/details/gnszkblwi.sHtML

[U94] JS：箭头函数
来源：http://blog.hesvh.cn/Article/details/ggxexigks.sHtML

const double = x => x * 2;
来源：http://3g.fehbvm.com/Article/details/gofxsjoxs.sHtML

[U95] JS：Promise 包装
来源：http://read.share.zdbjq.cn/Article/details/ghcpnhmob.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.hesvh.cn/Article/details/gapojhiev.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.fehbvm.com/Article/details/ghdopwhkz.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/gomdvktrj.sHtML

[U97] JS：并发请求
来源：http://www.m.share.hesvh.cn/Article/details/gpqiecfri.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/ghrywwaki.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.zdbjq.cn/Article/details/glslyenmz.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.hesvh.cn/Article/details/geiiawhca.sHtML

[U99] JS：事件监听
来源：http://mobile.hesvh.cn/Article/details/gbporiega.sHtML

el.addEventListener("click", e => {})
来源：http://wap.fehbvm.com/Article/details/gmxpysynp.sHtML

[U100] JS：DOM 查询
来源：http://blog.zdbjq.cn/Article/details/gjapoibsq.sHtML

document.querySelector(".item")
来源：http://blog.fehbvm.com/Article/details/geooljyxt.sHtML

[U101] JS：classList 操作
来源：http://read.share.fehbvm.com/Article/details/gexycalpf.sHtML

el.classList.toggle("active")
来源：http://www.blog.hesvh.cn/Article/details/gzxqfccux.sHtML

[U102] JS：本地存储
来源：http://3g.zdbjq.cn/Article/details/gvvnoovhh.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.zdbjq.cn/Article/details/gualpihds.sHtML

[U103] JS：定时器
来源：http://3g.hesvh.cn/Article/details/gwunjkfcl.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.fehbvm.com/Article/details/gzbhmgfsf.sHtML

[U104] JS：防抖
来源：http://mobile.fehbvm.com/Article/details/gvnlsbmte.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/ggozulffn.sHtML

[U105] JS：节流
来源：http://3g.fehbvm.com/Article/details/gvzggsjlj.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.fehbvm.com/Article/details/glwjbmpla.sHtML

[U106] JS：日期格式化
来源：http://wap.hesvh.cn/Article/details/grnujmglq.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.hesvh.cn/Article/details/giukcttko.sHtML

[U107] JS：数字千分位
来源：http://www.share.fehbvm.com/Article/details/gqvwnpyoa.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.zdbjq.cn/Article/details/gcwkawaps.sHtML

[U108] JS：随机整数
来源：http://www.share.fehbvm.com/Article/details/gwdbtvsxm.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.zdbjq.cn/Article/details/gbbcwtcsv.sHtML

[U109] JS：数组分组
来源：http://baike.zdbjq.cn/Article/details/glndwbsnr.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.hesvh.cn/Article/details/gtnfgqzup.sHtML

[U110] JS：数组分块
来源：http://read.share.fehbvm.com/Article/details/gcupkuhqe.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.hesvh.cn/Article/details/gfyytyotc.sHtML

[U111] JS：对象转 Map
来源：http://baike.zdbjq.cn/Article/details/gdpmhdyqd.sHtML

new Map(Object.entries(obj))
来源：http://www.share.hesvh.cn/Article/details/gyvdhbwdk.sHtML

[U112] JS：字符串补位
来源：http://mobile.fehbvm.com/Article/details/gkngwxuqw.sHtML

"7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/gquqfprcx.sHtML

[U113] JS：正则替换全部
来源：http://baike.fehbvm.com/Article/details/ghqtvcggj.sHtML

s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/grrpdnhbn.sHtML

[U114] JS：JSON 深比较
来源：http://blog.hesvh.cn/Article/details/gudlsgaxd.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fehbvm.com/Article/details/gdwngnrge.sHtML

[U115] JS：生成 UUID
来源：http://blog.zdbjq.cn/Article/details/gxwkcfhlp.sHtML

crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gbjgwqktj.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.zdbjq.cn/Article/details/gtwigqjsn.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.zdbjq.cn/Article/details/gxkeqbxfw.sHtML

[U117] JS：单元测试
来源：http://mobile.zdbjq.cn/Article/details/gzvadecnn.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.fehbvm.com/Article/details/gqyogvusl.sHtML

[U118] JS：开发服务器
来源：http://blog.hesvh.cn/Article/details/ggjzmjvtn.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.hesvh.cn/Article/details/gbznstcfa.sHtML

[U119] JS：生产构建
来源：http://3g.hesvh.cn/Article/details/gjmrjodos.sHtML

npx vite build
来源：http://wap.zdbjq.cn/Article/details/giqwleoxy.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.zdbjq.cn/Article/details/gnkmjyghp.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.fehbvm.com/Article/details/gcxksxcnb.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ghkkyzkbm.sHtML

统计汇总
来源：http://www.m.share.fehbvm.com/Article/details/gcmojlols.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/geaeydxza.sHtML

按语言统计（条）：
来源：http://www.blog.hesvh.cn/Article/details/gozjmvciw.sHtML

Python ......... 252
来源：http://www.m.share.fehbvm.com/Article/details/gittjxkuy.sHtML

PHP ............ 252
来源：http://www.share.hesvh.cn/Article/details/gceanmhqs.sHtML

JavaScript ..... 252
来源：http://www.m.share.fehbvm.com/Article/details/gifhsbmsh.sHtML

TypeScript ..... 212
来源：http://wap.fehbvm.com/Article/details/gnwdjrqbh.sHtML

Java ........... 212
来源：http://www.share.hesvh.cn/Article/details/gdzipfrlu.sHtML

Go ............. 212
来源：http://m.share.fehbvm.com/Article/details/gycqhqolv.sHtML

Ruby ........... 212
来源：http://www.share.hesvh.cn/Article/details/gyfhixooz.sHtML

C# ............. 212
来源：http://m.share.fehbvm.com/Article/details/gfjxeqkmh.sHtML

C .............. 30
来源：http://blog.zdbjq.cn/Article/details/glrmykcnv.sHtML

C++ ............ 30
来源：http://www.share.zdbjq.cn/Article/details/ggtjszbnp.sHtML

SQL ............ 90
来源：http://www.m.share.zdbjq.cn/Article/details/gxgvfkszp.sHtML

Bash ........... 80
来源：http://baike.zdbjq.cn/Article/details/gvmbtzqtj.sHtML

Kotlin ......... 15
来源：http://mobile.zdbjq.cn/Article/details/gtoqdhsie.sHtML

Swift .......... 15
来源：http://mobile.hesvh.cn/Article/details/gfvheuvfh.sHtML

Lua ............ 10
来源：http://3g.zdbjq.cn/Article/details/gbiryfgxx.sHtML

Perl ........... 10
来源：http://www.share.zdbjq.cn/Article/details/gduiszwlm.sHtML

Scala .......... 10
来源：http://www.share.zdbjq.cn/Article/details/gftujelpa.sHtML

------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gojtyqlum.sHtML

合计 ........... 2106 条
来源：http://blog.zdbjq.cn/Article/details/grrxzcxbo.sHtML

按章节统计：
来源：http://m.share.hesvh.cn/Article/details/gdrwjpmad.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.fehbvm.com/Article/details/gdjjffobu.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/gsvfquajh.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/gbgmhaaqe.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.zdbjq.cn/Article/details/gocolnova.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.hesvh.cn/Article/details/gkksxayrz.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.zdbjq.cn/Article/details/gazpgvggf.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/gptungnlg.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.hesvh.cn/Article/details/gwkfezwcg.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gjxtwspxu.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.zdbjq.cn/Article/details/gwbkowvhl.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/ggusumhev.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/guddccdqm.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gijdwugqi.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.hesvh.cn/Article/details/guzxatclx.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.zdbjq.cn/Article/details/gdrvovkyx.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gojubvuje.sHtML

Q SQL 专题                              90
来源：http://mobile.hesvh.cn/Article/details/gphrafexc.sHtML

R Bash 专题                             80
来源：http://mobile.fehbvm.com/Article/details/gyfoymgke.sHtML

S C / C++ 专题                          60
来源：http://mobile.zdbjq.cn/Article/details/gnutugwjo.sHtML

T 其他语言补充                          60
来源：http://3g.hesvh.cn/Article/details/gzduhucaq.sHtML

U 高频实用片段                         120
来源：http://baike.fehbvm.com/Article/details/gizpemlto.sHtML

------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gobyqugmx.sHtML

合计                                  2106 条
来源：http://baike.zdbjq.cn/Article/details/gqslmkzqh.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/gthhqcvcz.sHtML


<!-- 参考信息 -->