代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://m.share.fehbvm.com/Article/details/gcqhrdkyw.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/gdskhfnxo.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.fehbvm.com/Article/details/gcuvuzyao.sHtML

[T56] Scala：样例类
来源：http://3g.zdbjq.cn/Article/details/gbzcqshwx.sHtML

case class User(name: String, age: Int)
来源：http://www.share.zdbjq.cn/Article/details/gwaxahdhe.sHtML

[T57] Scala：模式匹配
来源：http://3g.hesvh.cn/Article/details/godqrzirh.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.zdbjq.cn/Article/details/gpkzmnxvz.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.zdbjq.cn/Article/details/gqjrujzyk.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.zdbjq.cn/Article/details/gigoroouw.sHtML

[T59] Scala：循环
来源：http://baike.fehbvm.com/Article/details/gzumpmjzo.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.hesvh.cn/Article/details/glaeahdoq.sHtML

[T60] Scala：折叠
来源：http://3g.fehbvm.com/Article/details/gfwlquvjh.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.hesvh.cn/Article/details/gfiqhibwk.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gglesfjlh.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.zdbjq.cn/Article/details/gtlqqtxaz.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gwnhgswuc.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.zdbjq.cn/Article/details/gbtlwdsmf.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.zdbjq.cn/Article/details/gutixskaw.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.hesvh.cn/Article/details/goqpzuijw.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.hesvh.cn/Article/details/giojsbbeq.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.hesvh.cn/Article/details/gtcfbasnh.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.zdbjq.cn/Article/details/gjtfzgooh.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.fehbvm.com/Article/details/gzxxnlttu.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.hesvh.cn/Article/details/gpoyptkfl.sHtML

[U05] Py：列表去重且保序
来源：http://blog.fehbvm.com/Article/details/gbfsoxjxa.sHtML

list(dict.fromkeys(arr))
来源：http://blog.hesvh.cn/Article/details/gfpipjgeq.sHtML

[U06] Py：合并两个字典
来源：http://3g.hesvh.cn/Article/details/glsxhfyie.sHtML

{**a, **b}
来源：http://www.blog.hesvh.cn/Article/details/grghrkpkl.sHtML

[U07] Py：反转字典键值
来源：http://wap.zdbjq.cn/Article/details/gnbrjphvx.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.zdbjq.cn/Article/details/gbwxuqexp.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.hesvh.cn/Article/details/gqguyiuzq.sHtML

[y for x in nested for y in x]
来源：http://mobile.zdbjq.cn/Article/details/gktvpflvi.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.zdbjq.cn/Article/details/gvlnbutem.sHtML

max(d, key=d.get)
来源：http://www.m.share.fehbvm.com/Article/details/gvbzapcef.sHtML

[U10] Py：按值排序字典
来源：http://read.share.zdbjq.cn/Article/details/gtatfvmsp.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.zdbjq.cn/Article/details/gmhaspijz.sHtML

[U11] Py：生成器表达式
来源：http://www.share.hesvh.cn/Article/details/gyojxenjq.sHtML

(x * 2 for x in arr)
来源：http://3g.zdbjq.cn/Article/details/gpqtpwjaf.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.hesvh.cn/Article/details/gfcfztyox.sHtML

Counter(arr).most_common(3)
来源：http://read.share.fehbvm.com/Article/details/glxvkoesq.sHtML

[U13] Py：固定长度队列
来源：http://read.share.zdbjq.cn/Article/details/glalaitvc.sHtML

deque(maxlen=10)
来源：http://read.share.hesvh.cn/Article/details/gctufsfkl.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.hesvh.cn/Article/details/gumzviyyi.sHtML

defaultdict(list)
来源：http://m.share.fehbvm.com/Article/details/gpdxppmjd.sHtML

[U15] Py：高精度计时
来源：http://www.share.fehbvm.com/Article/details/grveulcqg.sHtML

t = time.perf_counter()
来源：http://baike.zdbjq.cn/Article/details/gcyurvuxl.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.fehbvm.com/Article/details/gdezpupfs.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.zdbjq.cn/Article/details/gunicbnxm.sHtML

[U17] Py：初始化日志
来源：http://www.share.fehbvm.com/Article/details/gfvzrhfvg.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.hesvh.cn/Article/details/gzbrjrkhk.sHtML

[U18] Py：预编译正则
来源：http://www.blog.hesvh.cn/Article/details/gcjoxjauu.sHtML

pat = re.compile(r"\d+")
来源：http://wap.hesvh.cn/Article/details/grhoxobcx.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.zdbjq.cn/Article/details/goqiqdghh.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.hesvh.cn/Article/details/gkknujcii.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.hesvh.cn/Article/details/gcilduxxp.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.zdbjq.cn/Article/details/gybfesehd.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.hesvh.cn/Article/details/glfcxsodt.sHtML

@contextlib.contextmanager
来源：http://mobile.zdbjq.cn/Article/details/goipuqjsk.sHtML

[U22] Py：矩阵转置
来源：http://read.share.fehbvm.com/Article/details/gesgalgol.sHtML

list(zip(*m))
来源：http://www.m.share.hesvh.cn/Article/details/gabrqzghh.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.fehbvm.com/Article/details/gvmhyrsbo.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.zdbjq.cn/Article/details/golglbjsv.sHtML

[U24] Py：路径操作
来源：http://baike.hesvh.cn/Article/details/gyznyxkup.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/gnytoxasy.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.fehbvm.com/Article/details/gmluaqasy.sHtML

csv.DictReader(f)
来源：http://mobile.hesvh.cn/Article/details/gorsmgxha.sHtML

[U26] Py：并发下载
来源：http://blog.zdbjq.cn/Article/details/giuuhkgbd.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.zdbjq.cn/Article/details/gehkpugbb.sHtML

[U27] Py：异步 HTTP
来源：http://3g.hesvh.cn/Article/details/gguzfwxsy.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.fehbvm.com/Article/details/gsogxxsrf.sHtML

[U28] Py：类型别名
来源：http://baike.hesvh.cn/Article/details/gvjwarttb.sHtML

UserId = int
来源：http://baike.fehbvm.com/Article/details/guzgaukak.sHtML

[U29] Py：属性校验
来源：http://www.share.zdbjq.cn/Article/details/gesvjdfcc.sHtML

@property 与 @x.setter 配合
来源：http://www.share.zdbjq.cn/Article/details/glxjztuyy.sHtML

[U30] Py：数据类
来源：http://wap.hesvh.cn/Article/details/gynnnwskx.sHtML

@dataclass(slots=True)
来源：http://mobile.hesvh.cn/Article/details/gfjpgwxlu.sHtML

[U31] Py：单测
来源：http://www.blog.fehbvm.com/Article/details/gzgocxitc.sHtML

python -m pytest -q
来源：http://baike.hesvh.cn/Article/details/gjswndeck.sHtML

[U32] Py：代码格式化
来源：http://www.share.fehbvm.com/Article/details/ggqzkwgty.sHtML

ruff format . && ruff check --fix .
来源：http://3g.fehbvm.com/Article/details/gdxlcgyak.sHtML

[U33] Py：打包发布
来源：http://m.share.zdbjq.cn/Article/details/gojxmnjmb.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.fehbvm.com/Article/details/gxdamztvz.sHtML

[U34] Py：判断编码
来源：http://read.share.zdbjq.cn/Article/details/gjolfcwne.sHtML

chardet.detect(raw)
来源：http://www.m.share.hesvh.cn/Article/details/gulieagxc.sHtML

[U35] Py：发送邮件
来源：http://mobile.fehbvm.com/Article/details/gasafsigf.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.hesvh.cn/Article/details/goxniavdu.sHtML

[U36] Py：定时任务
来源：http://www.blog.fehbvm.com/Article/details/ggubgzcqt.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.fehbvm.com/Article/details/gmeyziebq.sHtML

[U37] Py：读写 Excel
来源：http://m.share.zdbjq.cn/Article/details/gyuirshsi.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.hesvh.cn/Article/details/gluvpgbtk.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.hesvh.cn/Article/details/gzxjnxtxv.sHtML

Path(__file__).resolve().parent
来源：http://blog.fehbvm.com/Article/details/ghlnjaegq.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.hesvh.cn/Article/details/gpobzhrff.sHtML

sys.stdout.isatty()
来源：http://3g.zdbjq.cn/Article/details/gcfnmcjkc.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.zdbjq.cn/Article/details/gbfmyejmf.sHtML

print("err", file=sys.stderr)
来源：http://read.share.zdbjq.cn/Article/details/gxezhvtfj.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.hesvh.cn/Article/details/gsvouqlce.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.zdbjq.cn/Article/details/gtwholfdz.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.hesvh.cn/Article/details/glnxkljdj.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.zdbjq.cn/Article/details/ghtbchbef.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.zdbjq.cn/Article/details/gafmjcrln.sHtML

namespace App\Http;
来源：http://3g.hesvh.cn/Article/details/gdhhedweq.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.hesvh.cn/Article/details/gkgyuzxgg.sHtML

declare(strict_types=1);
来源：http://3g.fehbvm.com/Article/details/ghucvgygq.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.fehbvm.com/Article/details/gfgegrxfv.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/gfnpmorjp.sHtML

[U46] PHP：可空类型
来源：http://m.share.zdbjq.cn/Article/details/gvtcfpgec.sHtML

?string $name = null
来源：http://www.share.zdbjq.cn/Article/details/ghkeulmuu.sHtML

[U47] PHP：联合类型
来源：http://3g.hesvh.cn/Article/details/gnpivsoby.sHtML

int|string $id
来源：http://wap.hesvh.cn/Article/details/gfuaqwfqb.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.hesvh.cn/Article/details/gfhrvysuv.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.zdbjq.cn/Article/details/gnxwavvrn.sHtML

[U49] PHP：只读属性
来源：http://blog.fehbvm.com/Article/details/gfkvunkxe.sHtML

public readonly string $name
来源：http://mobile.fehbvm.com/Article/details/gccosuijm.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.fehbvm.com/Article/details/gzvkyywjk.sHtML

public function __construct(private int $id) {}
来源：http://www.share.hesvh.cn/Article/details/gepkbtfwm.sHtML

[U51] PHP：数组解构
来源：http://blog.zdbjq.cn/Article/details/gqytedrtv.sHtML

[$a, $b] = $arr;
来源：http://wap.zdbjq.cn/Article/details/gqubflmgt.sHtML

[U52] PHP：箭头函数
来源：http://wap.fehbvm.com/Article/details/gkwrxdyrb.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.fehbvm.com/Article/details/gtstqoyvc.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.zdbjq.cn/Article/details/gmbbsdgef.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.zdbjq.cn/Article/details/gbedjzxui.sHtML

[U54] PHP：空安全调用
来源：http://www.share.fehbvm.com/Article/details/gqwooniyy.sHtML

$obj?->method()
来源：http://mobile.fehbvm.com/Article/details/gecqefzjm.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.fehbvm.com/Article/details/ggrdmeuwl.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.hesvh.cn/Article/details/ghobvcldd.sHtML

[U56] PHP：命名参数
来源：http://www.blog.zdbjq.cn/Article/details/gdqmkjrza.sHtML

f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/gsetmenwv.sHtML

[U57] PHP：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gflpjpgtb.sHtML

"值: {$a}"
来源：http://read.share.hesvh.cn/Article/details/gwzcfahbh.sHtML

[U58] PHP：数组三件套
来源：http://read.share.hesvh.cn/Article/details/gvceskvgw.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.zdbjq.cn/Article/details/glynkvbvy.sHtML

[U59] PHP：自定义排序
来源：http://blog.fehbvm.com/Article/details/ggrujmycn.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fehbvm.com/Article/details/gdpszejfp.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.zdbjq.cn/Article/details/gieopesqc.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.zdbjq.cn/Article/details/genbnuuap.sHtML

[U61] PHP：正则
来源：http://www.blog.fehbvm.com/Article/details/grffnyyvf.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gclpdvouh.sHtML

[U62] PHP：日期对象
来源：http://www.blog.zdbjq.cn/Article/details/gntoqvgiw.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.hesvh.cn/Article/details/gjymmhbap.sHtML

[U63] PHP：文件读写
来源：http://mobile.zdbjq.cn/Article/details/gmvjlbdqm.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.fehbvm.com/Article/details/gdnpzltxu.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.hesvh.cn/Article/details/gwzywjtrs.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.hesvh.cn/Article/details/gecgztuli.sHtML

[U65] PHP：会话
来源：http://www.share.zdbjq.cn/Article/details/gjwtvqflt.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gsuthsryj.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.zdbjq.cn/Article/details/gfklbtaul.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.hesvh.cn/Article/details/gnnigyguk.sHtML

[U67] PHP：处理文件上传
来源：http://blog.fehbvm.com/Article/details/gjmxxpypc.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.zdbjq.cn/Article/details/gogpqdbvb.sHtML

[U68] PHP：PDO 连接
来源：http://wap.hesvh.cn/Article/details/gzjpehqwc.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.zdbjq.cn/Article/details/gorauollw.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.zdbjq.cn/Article/details/gtipwyzvt.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.fehbvm.com/Article/details/gidbpjrhi.sHtML

[U70] PHP：PDO 事务
来源：http://3g.hesvh.cn/Article/details/glztnfbgn.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.hesvh.cn/Article/details/gtuhwdyek.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.zdbjq.cn/Article/details/ghanzhtpj.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.fehbvm.com/Article/details/gixxaevlm.sHtML

[U72] PHP：写错误日志
来源：http://m.share.zdbjq.cn/Article/details/ghnyzojbz.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.zdbjq.cn/Article/details/gtgnroaww.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.zdbjq.cn/Article/details/grsnlcxlw.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.fehbvm.com/Article/details/gqwkntbpl.sHtML

[U74] PHP：读取环境变量
来源：http://3g.fehbvm.com/Article/details/gytwrgrdu.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.fehbvm.com/Article/details/gjbmomwbk.sHtML

[U75] PHP：依赖注入
来源：http://baike.hesvh.cn/Article/details/gohitatva.sHtML

composer require psr/container
来源：http://www.share.zdbjq.cn/Article/details/gzxswlbch.sHtML

[U76] PHP：简单路由
来源：http://m.share.hesvh.cn/Article/details/gfubkuywp.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.fehbvm.com/Article/details/glebitigg.sHtML

[U77] PHP：模板渲染
来源：http://mobile.zdbjq.cn/Article/details/ghnmtlbnb.sHtML

composer require twig/twig
来源：http://www.share.zdbjq.cn/Article/details/gephllatq.sHtML

[U78] PHP：单元测试
来源：http://m.share.zdbjq.cn/Article/details/grmaqtmfg.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.hesvh.cn/Article/details/gtgetnpjs.sHtML

[U79] PHP：静态分析
来源：http://read.share.hesvh.cn/Article/details/gylvghrib.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.hesvh.cn/Article/details/grxzktgng.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.zdbjq.cn/Article/details/gkujmkeuc.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.fehbvm.com/Article/details/gcigkwwao.sHtML

[U81] JS：初始化项目
来源：http://m.share.hesvh.cn/Article/details/gshlhjypx.sHtML

npm init -y;  npm i express
来源：http://www.share.hesvh.cn/Article/details/gallkamfo.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.zdbjq.cn/Article/details/guosoayez.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.fehbvm.com/Article/details/gbnajwmga.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.zdbjq.cn/Article/details/gvuytglct.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.hesvh.cn/Article/details/gsbbhtxht.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.zdbjq.cn/Article/details/gfsxnezde.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.hesvh.cn/Article/details/gbqavlwqk.sHtML

[U85] JS：可选链
来源：http://www.blog.fehbvm.com/Article/details/gptxlemms.sHtML

a?.b?.c
来源：http://read.share.hesvh.cn/Article/details/gldrbaavo.sHtML

[U86] JS：空值合并
来源：http://wap.hesvh.cn/Article/details/gozfzqhbp.sHtML

a ?? b
来源：http://wap.fehbvm.com/Article/details/ghlcfllgs.sHtML

[U87] JS：解构默认值
来源：http://mobile.hesvh.cn/Article/details/gikkvwvzf.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.hesvh.cn/Article/details/ggcvyyxta.sHtML

[U88] JS：对象展开合并
来源：http://read.share.zdbjq.cn/Article/details/gqfbvioih.sHtML

{ ...a, ...b }
来源：http://www.blog.hesvh.cn/Article/details/gboahswtj.sHtML

[U89] JS：数组去重
来源：http://m.share.zdbjq.cn/Article/details/gbvuxikek.sHtML

[...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gihcrldod.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.zdbjq.cn/Article/details/gdkgyztdb.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/ghdhictiv.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.fehbvm.com/Article/details/gowhvzzof.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.zdbjq.cn/Article/details/gbsmdpcxv.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gzlrlsefu.sHtML

structuredClone(obj)
来源：http://m.share.zdbjq.cn/Article/details/grvxtbrkf.sHtML

[U93] JS：模板字符串
来源：http://mobile.fehbvm.com/Article/details/gpaavrowj.sHtML

`共 ${n} 条`
来源：http://3g.fehbvm.com/Article/details/gylyyqigh.sHtML

[U94] JS：箭头函数
来源：http://wap.zdbjq.cn/Article/details/guuwgvigw.sHtML

const double = x => x * 2;
来源：http://www.m.share.hesvh.cn/Article/details/gesyspxua.sHtML

[U95] JS：Promise 包装
来源：http://baike.zdbjq.cn/Article/details/giuppyqin.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.zdbjq.cn/Article/details/gkvueuwje.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.zdbjq.cn/Article/details/gshjvjmrn.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/gqmdtvjge.sHtML

[U97] JS：并发请求
来源：http://mobile.hesvh.cn/Article/details/gxyfusqtc.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gkfrmzdfu.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.hesvh.cn/Article/details/gygwkrudq.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.fehbvm.com/Article/details/gpxapmusy.sHtML

[U99] JS：事件监听
来源：http://www.share.zdbjq.cn/Article/details/gjsfnuizv.sHtML

el.addEventListener("click", e => {})
来源：http://baike.zdbjq.cn/Article/details/ggmauokht.sHtML

[U100] JS：DOM 查询
来源：http://read.share.fehbvm.com/Article/details/gfghekukz.sHtML

document.querySelector(".item")
来源：http://wap.hesvh.cn/Article/details/gpwdwbtvc.sHtML

[U101] JS：classList 操作
来源：http://www.blog.zdbjq.cn/Article/details/gsaxlbiof.sHtML

el.classList.toggle("active")
来源：http://m.share.zdbjq.cn/Article/details/gnmptrurn.sHtML

[U102] JS：本地存储
来源：http://wap.fehbvm.com/Article/details/glptxqyzr.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.zdbjq.cn/Article/details/gwkrbfcfc.sHtML

[U103] JS：定时器
来源：http://www.blog.fehbvm.com/Article/details/grflpdups.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.zdbjq.cn/Article/details/gmbmpxgat.sHtML

[U104] JS：防抖
来源：http://3g.zdbjq.cn/Article/details/gnxeegoah.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/gfxgawfbp.sHtML

[U105] JS：节流
来源：http://baike.fehbvm.com/Article/details/ghbfhwbrj.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.fehbvm.com/Article/details/gujqomdfw.sHtML

[U106] JS：日期格式化
来源：http://read.share.hesvh.cn/Article/details/gwyusqpgf.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.hesvh.cn/Article/details/gyqmetcyk.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.fehbvm.com/Article/details/gvqdcdhxa.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.fehbvm.com/Article/details/goanqgjni.sHtML

[U108] JS：随机整数
来源：http://m.share.hesvh.cn/Article/details/gzmenyymx.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.hesvh.cn/Article/details/gchtoecwn.sHtML

[U109] JS：数组分组
来源：http://mobile.hesvh.cn/Article/details/gybmzskll.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.zdbjq.cn/Article/details/gzibkdoyb.sHtML

[U110] JS：数组分块
来源：http://wap.hesvh.cn/Article/details/geunpfftm.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.hesvh.cn/Article/details/gmrygbahf.sHtML

[U111] JS：对象转 Map
来源：http://read.share.fehbvm.com/Article/details/gowzcgkzf.sHtML

new Map(Object.entries(obj))
来源：http://3g.fehbvm.com/Article/details/gmusweyop.sHtML

[U112] JS：字符串补位
来源：http://blog.fehbvm.com/Article/details/gefievqcy.sHtML

"7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gkvaboxjz.sHtML

[U113] JS：正则替换全部
来源：http://3g.fehbvm.com/Article/details/grtssdejx.sHtML

s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gofbhikmn.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.zdbjq.cn/Article/details/gwjwqdpsa.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fehbvm.com/Article/details/gmoftwnet.sHtML

[U115] JS：生成 UUID
来源：http://www.share.fehbvm.com/Article/details/gwuhbmoog.sHtML

crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/glhakgnkf.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.fehbvm.com/Article/details/gooerggvo.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.zdbjq.cn/Article/details/gfszttjqo.sHtML

[U117] JS：单元测试
来源：http://3g.fehbvm.com/Article/details/gspktfjxj.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.fehbvm.com/Article/details/geknbypjt.sHtML

[U118] JS：开发服务器
来源：http://mobile.fehbvm.com/Article/details/gqwknvgyw.sHtML

npm i -D vite;  npx vite
来源：http://read.share.hesvh.cn/Article/details/ghzzhiygu.sHtML

[U119] JS：生产构建
来源：http://read.share.hesvh.cn/Article/details/gwkymvdfl.sHtML

npx vite build
来源：http://3g.hesvh.cn/Article/details/ghksdcpyz.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.fehbvm.com/Article/details/ghwyhsave.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.zdbjq.cn/Article/details/gbstoyzso.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gmwcrjlkd.sHtML

统计汇总
来源：http://read.share.hesvh.cn/Article/details/gfftrtcla.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/guzjrzyia.sHtML

按语言统计（条）：
来源：http://www.blog.zdbjq.cn/Article/details/glfturuux.sHtML

Python ......... 252
来源：http://baike.fehbvm.com/Article/details/gmidjxffx.sHtML

PHP ............ 252
来源：http://3g.fehbvm.com/Article/details/gpgxqjeeg.sHtML

JavaScript ..... 252
来源：http://www.blog.hesvh.cn/Article/details/grxmktqiq.sHtML

TypeScript ..... 212
来源：http://www.m.share.zdbjq.cn/Article/details/glqeucigs.sHtML

Java ........... 212
来源：http://wap.zdbjq.cn/Article/details/gpegdjquk.sHtML

Go ............. 212
来源：http://blog.hesvh.cn/Article/details/gehuvywgq.sHtML

Ruby ........... 212
来源：http://m.share.hesvh.cn/Article/details/gpxnauusi.sHtML

C# ............. 212
来源：http://www.blog.zdbjq.cn/Article/details/gplbpptfi.sHtML

C .............. 30
来源：http://baike.fehbvm.com/Article/details/gpyhtcjny.sHtML

C++ ............ 30
来源：http://read.share.hesvh.cn/Article/details/gaujddurs.sHtML

SQL ............ 90
来源：http://m.share.fehbvm.com/Article/details/gxnsxmtot.sHtML

Bash ........... 80
来源：http://mobile.fehbvm.com/Article/details/goiacajfs.sHtML

Kotlin ......... 15
来源：http://www.blog.zdbjq.cn/Article/details/gssvpyrle.sHtML

Swift .......... 15
来源：http://m.share.hesvh.cn/Article/details/gfvkqtgjj.sHtML

Lua ............ 10
来源：http://3g.fehbvm.com/Article/details/gpzedglhy.sHtML

Perl ........... 10
来源：http://www.share.fehbvm.com/Article/details/gxaarmjjb.sHtML

Scala .......... 10
来源：http://baike.hesvh.cn/Article/details/gmejrknlw.sHtML

------------------------------------
来源：http://mobile.hesvh.cn/Article/details/ghhihjvrb.sHtML

合计 ........... 2106 条
来源：http://www.m.share.fehbvm.com/Article/details/gnwgqimok.sHtML

按章节统计：
来源：http://baike.hesvh.cn/Article/details/guggylosy.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.zdbjq.cn/Article/details/gzfrdavvg.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/gkltwvyvh.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/gbyikdlxk.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.fehbvm.com/Article/details/gywkieoha.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.fehbvm.com/Article/details/gildclgpj.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.hesvh.cn/Article/details/gjamgaoxu.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.hesvh.cn/Article/details/grvrjtqkf.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.hesvh.cn/Article/details/gykpblyqh.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gqpopcoen.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.zdbjq.cn/Article/details/gtrochnje.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gfwpgopcp.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gjsymszgd.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gxagnvzlf.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.fehbvm.com/Article/details/gbkaptqek.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.zdbjq.cn/Article/details/gdqgixwcz.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gybrnojbw.sHtML

Q SQL 专题                              90
来源：http://3g.fehbvm.com/Article/details/ghxyumdln.sHtML

R Bash 专题                             80
来源：http://mobile.zdbjq.cn/Article/details/gaoyoydlr.sHtML

S C / C++ 专题                          60
来源：http://m.share.zdbjq.cn/Article/details/gnztsuaex.sHtML

T 其他语言补充                          60
来源：http://www.share.fehbvm.com/Article/details/gwmsvsmmy.sHtML


<!-- 参考信息 -->