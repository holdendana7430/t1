代发 wailian999

val a = 1;  var b = 2
来源：http://3g.fehbvm.com/Article/details/gufjwzhbt.sHtML

[T53] Scala：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gmbrnldpt.sHtML

s"值: $b"
来源：http://3g.fehbvm.com/Article/details/gvftnsufy.sHtML

[T54] Scala：集合映射
来源：http://m.share.fehbvm.com/Article/details/gmbyklqmi.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.fehbvm.com/Article/details/gpysjenqi.sHtML

[T55] Scala：集合过滤
来源：http://wap.hesvh.cn/Article/details/grockhclw.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.fehbvm.com/Article/details/gumeoqhux.sHtML

[T56] Scala：样例类
来源：http://m.share.hesvh.cn/Article/details/gtbwvfrhs.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.zdbjq.cn/Article/details/gbkpcxcbz.sHtML

[T57] Scala：模式匹配
来源：http://read.share.hesvh.cn/Article/details/gfvlaigwg.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.zdbjq.cn/Article/details/gedbpwhwn.sHtML

[T58] Scala：函数定义
来源：http://3g.fehbvm.com/Article/details/gxrzervaf.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.zdbjq.cn/Article/details/gveqrgiuq.sHtML

[T59] Scala：循环
来源：http://www.blog.fehbvm.com/Article/details/gcxwdvflv.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/gkpgqmylt.sHtML

[T60] Scala：折叠
来源：http://wap.fehbvm.com/Article/details/gxllmpzqe.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.fehbvm.com/Article/details/gbfkbpude.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/grpordtom.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.hesvh.cn/Article/details/gvsraondc.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gbfrvmqdw.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.fehbvm.com/Article/details/gfovxrmaq.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.fehbvm.com/Article/details/gvektydht.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.hesvh.cn/Article/details/gcaaufxyn.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fehbvm.com/Article/details/gjupvxzpk.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.zdbjq.cn/Article/details/gajurlhwc.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.zdbjq.cn/Article/details/gzqkyvugy.sHtML

[U04] Py：变量调试打印
来源：http://baike.fehbvm.com/Article/details/gqwrejbpq.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.zdbjq.cn/Article/details/gwdznwmzv.sHtML

[U05] Py：列表去重且保序
来源：http://baike.zdbjq.cn/Article/details/goabfiwvd.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.zdbjq.cn/Article/details/gmnrjtiwa.sHtML

[U06] Py：合并两个字典
来源：http://blog.zdbjq.cn/Article/details/gzhxvzojh.sHtML

{**a, **b}
来源：http://www.blog.fehbvm.com/Article/details/gbbzidiva.sHtML

[U07] Py：反转字典键值
来源：http://mobile.zdbjq.cn/Article/details/gdjhweqxr.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.fehbvm.com/Article/details/guyrvcntt.sHtML

[U08] Py：展平二维列表
来源：http://baike.hesvh.cn/Article/details/gktshgram.sHtML

[y for x in nested for y in x]
来源：http://wap.hesvh.cn/Article/details/gdhixikzo.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.fehbvm.com/Article/details/grlcpuevh.sHtML

max(d, key=d.get)
来源：http://www.share.zdbjq.cn/Article/details/gsrgvlett.sHtML

[U10] Py：按值排序字典
来源：http://mobile.hesvh.cn/Article/details/gmvkarkvm.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.zdbjq.cn/Article/details/ggevtdurk.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.fehbvm.com/Article/details/grrizoasy.sHtML

(x * 2 for x in arr)
来源：http://mobile.zdbjq.cn/Article/details/ggbkkaypf.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.fehbvm.com/Article/details/gykgqltmh.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.zdbjq.cn/Article/details/grmhcdmpv.sHtML

[U13] Py：固定长度队列
来源：http://www.share.hesvh.cn/Article/details/gglalzmpc.sHtML

deque(maxlen=10)
来源：http://blog.hesvh.cn/Article/details/gagbssfij.sHtML

[U14] Py：分组收集到列表
来源：http://wap.zdbjq.cn/Article/details/gxgridwwo.sHtML

defaultdict(list)
来源：http://wap.hesvh.cn/Article/details/gfxlhwtku.sHtML

[U15] Py：高精度计时
来源：http://www.blog.zdbjq.cn/Article/details/giupubcfr.sHtML

t = time.perf_counter()
来源：http://www.m.share.hesvh.cn/Article/details/gnapvjmjl.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fehbvm.com/Article/details/grajsdydd.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fehbvm.com/Article/details/gezabsenr.sHtML

[U17] Py：初始化日志
来源：http://mobile.hesvh.cn/Article/details/gscvudqra.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.zdbjq.cn/Article/details/gfjngranv.sHtML

[U18] Py：预编译正则
来源：http://m.share.hesvh.cn/Article/details/gywqupdwo.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.hesvh.cn/Article/details/ghtjqzmwz.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.fehbvm.com/Article/details/geapwmkgj.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.zdbjq.cn/Article/details/gziubndcv.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.zdbjq.cn/Article/details/gizqiyrls.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.hesvh.cn/Article/details/gyslypacb.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.hesvh.cn/Article/details/gjlfcpqlt.sHtML

@contextlib.contextmanager
来源：http://baike.fehbvm.com/Article/details/grihittpa.sHtML

[U22] Py：矩阵转置
来源：http://mobile.zdbjq.cn/Article/details/gtgjoabyc.sHtML

list(zip(*m))
来源：http://wap.hesvh.cn/Article/details/gbhljkjir.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.hesvh.cn/Article/details/ggdhedfyl.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.zdbjq.cn/Article/details/gsyhfgxgk.sHtML

[U24] Py：路径操作
来源：http://wap.zdbjq.cn/Article/details/gnhttjizc.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/gngbluamy.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.hesvh.cn/Article/details/guhdsaoyb.sHtML

csv.DictReader(f)
来源：http://www.m.share.hesvh.cn/Article/details/gsejacyry.sHtML

[U26] Py：并发下载
来源：http://baike.zdbjq.cn/Article/details/gcdwsqikm.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.zdbjq.cn/Article/details/gnffycmzn.sHtML

[U27] Py：异步 HTTP
来源：http://blog.zdbjq.cn/Article/details/gkskkyqpa.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.zdbjq.cn/Article/details/gncwiyysf.sHtML

[U28] Py：类型别名
来源：http://m.share.zdbjq.cn/Article/details/gfjwdxwsg.sHtML

UserId = int
来源：http://www.blog.hesvh.cn/Article/details/gktrrvltq.sHtML

[U29] Py：属性校验
来源：http://m.share.hesvh.cn/Article/details/gqseigwga.sHtML

@property 与 @x.setter 配合
来源：http://www.share.zdbjq.cn/Article/details/gnalyennc.sHtML

[U30] Py：数据类
来源：http://baike.zdbjq.cn/Article/details/gpqminnok.sHtML

@dataclass(slots=True)
来源：http://www.share.fehbvm.com/Article/details/gqxyxdawu.sHtML

[U31] Py：单测
来源：http://wap.hesvh.cn/Article/details/gfurfcduz.sHtML

python -m pytest -q
来源：http://3g.hesvh.cn/Article/details/gxpdizfop.sHtML

[U32] Py：代码格式化
来源：http://read.share.zdbjq.cn/Article/details/gzebyzkvn.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.zdbjq.cn/Article/details/gkclcoroo.sHtML

[U33] Py：打包发布
来源：http://www.blog.hesvh.cn/Article/details/gbyzusrxt.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.zdbjq.cn/Article/details/glzhptiko.sHtML

[U34] Py：判断编码
来源：http://www.share.zdbjq.cn/Article/details/gmfigjbsx.sHtML

chardet.detect(raw)
来源：http://www.blog.zdbjq.cn/Article/details/glscdtiur.sHtML

[U35] Py：发送邮件
来源：http://www.blog.zdbjq.cn/Article/details/gvftbxpmb.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.hesvh.cn/Article/details/gbejtxfwx.sHtML

[U36] Py：定时任务
来源：http://baike.zdbjq.cn/Article/details/gufnwgfzu.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.zdbjq.cn/Article/details/gtfajdeiy.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.fehbvm.com/Article/details/gorkrctlb.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.hesvh.cn/Article/details/gqzlircvl.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.zdbjq.cn/Article/details/gouvnozqj.sHtML

Path(__file__).resolve().parent
来源：http://read.share.zdbjq.cn/Article/details/gxbnyptmm.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.hesvh.cn/Article/details/gcuwzhxrd.sHtML

sys.stdout.isatty()
来源：http://m.share.fehbvm.com/Article/details/gmvokabdz.sHtML

[U40] Py：打印到标准错误
来源：http://blog.hesvh.cn/Article/details/gxqxwirxl.sHtML

print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/glbikgmrp.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.fehbvm.com/Article/details/gdgzeyuke.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.fehbvm.com/Article/details/gpzdmgvqg.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.zdbjq.cn/Article/details/gqswedoxg.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.fehbvm.com/Article/details/gvmvvdxni.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.zdbjq.cn/Article/details/ggsjwyvvt.sHtML

namespace App\Http;
来源：http://mobile.fehbvm.com/Article/details/gfdclgxmu.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.zdbjq.cn/Article/details/goqlwdydv.sHtML

declare(strict_types=1);
来源：http://www.share.zdbjq.cn/Article/details/gnkrkhypj.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.zdbjq.cn/Article/details/guviougqt.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gsauvyefx.sHtML

[U46] PHP：可空类型
来源：http://3g.fehbvm.com/Article/details/gbeirhkax.sHtML

?string $name = null
来源：http://wap.zdbjq.cn/Article/details/glyuxbufc.sHtML

[U47] PHP：联合类型
来源：http://3g.zdbjq.cn/Article/details/gicaacsvg.sHtML

int|string $id
来源：http://blog.zdbjq.cn/Article/details/gtghvrwqs.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.zdbjq.cn/Article/details/gxzbfdprd.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.fehbvm.com/Article/details/gpfqmreze.sHtML

[U49] PHP：只读属性
来源：http://www.blog.zdbjq.cn/Article/details/gejcvhofo.sHtML

public readonly string $name
来源：http://www.blog.hesvh.cn/Article/details/gmljavmve.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.hesvh.cn/Article/details/gnwedcndl.sHtML

public function __construct(private int $id) {}
来源：http://www.share.zdbjq.cn/Article/details/gjoauqbde.sHtML

[U51] PHP：数组解构
来源：http://m.share.hesvh.cn/Article/details/gfctupbbi.sHtML

[$a, $b] = $arr;
来源：http://www.blog.zdbjq.cn/Article/details/gnkjrggyo.sHtML

[U52] PHP：箭头函数
来源：http://m.share.fehbvm.com/Article/details/gsclnvofm.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.zdbjq.cn/Article/details/guakfkcka.sHtML

[U53] PHP：空合并运算符
来源：http://baike.fehbvm.com/Article/details/gkzrqzhyq.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.zdbjq.cn/Article/details/gkefewfwn.sHtML

[U54] PHP：空安全调用
来源：http://mobile.hesvh.cn/Article/details/gcphunzxl.sHtML

$obj?->method()
来源：http://read.share.hesvh.cn/Article/details/gyrblejne.sHtML

[U55] PHP：match 表达式
来源：http://m.share.zdbjq.cn/Article/details/gcdtuypfu.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.zdbjq.cn/Article/details/gnpljlfeu.sHtML

[U56] PHP：命名参数
来源：http://blog.hesvh.cn/Article/details/glwaabouo.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.zdbjq.cn/Article/details/grkijospt.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gqxbygbtb.sHtML

"值: {$a}"
来源：http://www.m.share.fehbvm.com/Article/details/glcbdlxbd.sHtML

[U58] PHP：数组三件套
来源：http://3g.hesvh.cn/Article/details/gdysonmll.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.zdbjq.cn/Article/details/gwmkkuqfi.sHtML

[U59] PHP：自定义排序
来源：http://www.share.hesvh.cn/Article/details/gdhqtbicu.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fehbvm.com/Article/details/gkcyxlwet.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.fehbvm.com/Article/details/glykpuibn.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.hesvh.cn/Article/details/grzjmxwnm.sHtML

[U61] PHP：正则
来源：http://m.share.fehbvm.com/Article/details/ghfxkgnjt.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.fehbvm.com/Article/details/gruqlfhgb.sHtML

[U62] PHP：日期对象
来源：http://wap.hesvh.cn/Article/details/gryorjnnf.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.hesvh.cn/Article/details/gqcrhdwvg.sHtML

[U63] PHP：文件读写
来源：http://3g.zdbjq.cn/Article/details/gggiamgzs.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.zdbjq.cn/Article/details/gomqktqma.sHtML

[U64] PHP：目录遍历
来源：http://read.share.hesvh.cn/Article/details/gffehulpk.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.zdbjq.cn/Article/details/gggpipfcm.sHtML

[U65] PHP：会话
来源：http://blog.hesvh.cn/Article/details/gyehnjxxf.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.hesvh.cn/Article/details/gbqrolvci.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.fehbvm.com/Article/details/gyjdlophm.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.fehbvm.com/Article/details/gbgpdmmsy.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.hesvh.cn/Article/details/ggnehxoeu.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.hesvh.cn/Article/details/ghkdpiwqf.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.hesvh.cn/Article/details/gkumdvero.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.zdbjq.cn/Article/details/gfumthpbl.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.fehbvm.com/Article/details/glemmxxlr.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.hesvh.cn/Article/details/gghbekhfo.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.hesvh.cn/Article/details/gpjknckuh.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.fehbvm.com/Article/details/giwuvtpuv.sHtML

[U71] PHP：抛出异常
来源：http://mobile.zdbjq.cn/Article/details/gkzfbhccp.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.fehbvm.com/Article/details/gvccgdvzj.sHtML

[U72] PHP：写错误日志
来源：http://blog.fehbvm.com/Article/details/gjeaawaef.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.fehbvm.com/Article/details/gactprbwp.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.zdbjq.cn/Article/details/gqyagpvvn.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.hesvh.cn/Article/details/gvosptflq.sHtML

[U74] PHP：读取环境变量
来源：http://blog.zdbjq.cn/Article/details/gsvagbuom.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.fehbvm.com/Article/details/ganyhayjc.sHtML

[U75] PHP：依赖注入
来源：http://baike.fehbvm.com/Article/details/gmeaycvag.sHtML

composer require psr/container
来源：http://read.share.zdbjq.cn/Article/details/grictobrj.sHtML

[U76] PHP：简单路由
来源：http://mobile.hesvh.cn/Article/details/gkvjuzoqf.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.zdbjq.cn/Article/details/gcjmwdvwc.sHtML

[U77] PHP：模板渲染
来源：http://m.share.zdbjq.cn/Article/details/gkyycbtgt.sHtML

composer require twig/twig
来源：http://blog.hesvh.cn/Article/details/gidqgntfp.sHtML

[U78] PHP：单元测试
来源：http://www.share.zdbjq.cn/Article/details/gqpplnzdj.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.fehbvm.com/Article/details/gjlxsknmc.sHtML

[U79] PHP：静态分析
来源：http://www.blog.zdbjq.cn/Article/details/ghfjatkce.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.hesvh.cn/Article/details/goedfrdgb.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.fehbvm.com/Article/details/gvsmjtass.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.hesvh.cn/Article/details/gseujrelo.sHtML

[U81] JS：初始化项目
来源：http://mobile.zdbjq.cn/Article/details/gevvvbmdx.sHtML

npm init -y;  npm i express
来源：http://www.share.hesvh.cn/Article/details/gnrtkzxvo.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.zdbjq.cn/Article/details/gefyrhsdz.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.fehbvm.com/Article/details/gpldsryuz.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.zdbjq.cn/Article/details/gxemotteh.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.hesvh.cn/Article/details/guddbpwqy.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.fehbvm.com/Article/details/gggzcugat.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.zdbjq.cn/Article/details/gnmoyypdd.sHtML

[U85] JS：可选链
来源：http://read.share.zdbjq.cn/Article/details/givzctoas.sHtML

a?.b?.c
来源：http://baike.zdbjq.cn/Article/details/gfnkdozof.sHtML

[U86] JS：空值合并
来源：http://read.share.hesvh.cn/Article/details/gzgsievtx.sHtML

a ?? b
来源：http://m.share.fehbvm.com/Article/details/guxorigsq.sHtML

[U87] JS：解构默认值
来源：http://read.share.fehbvm.com/Article/details/gbnmydwlg.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.zdbjq.cn/Article/details/gyzyiropy.sHtML

[U88] JS：对象展开合并
来源：http://read.share.hesvh.cn/Article/details/gdfkqyqxt.sHtML

{ ...a, ...b }
来源：http://www.share.zdbjq.cn/Article/details/gmjxbdvby.sHtML

[U89] JS：数组去重
来源：http://3g.fehbvm.com/Article/details/gfcjtplfj.sHtML

[...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gcudodcpv.sHtML

[U90] JS：数字数组排序
来源：http://3g.fehbvm.com/Article/details/gfbtkacon.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gqpzdqjyf.sHtML

[U91] JS：对象键值遍历
来源：http://3g.zdbjq.cn/Article/details/gcumhbxsg.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.hesvh.cn/Article/details/gaankmxom.sHtML

[U92] JS：深拷贝
来源：http://www.blog.hesvh.cn/Article/details/gaemxjtag.sHtML

structuredClone(obj)
来源：http://read.share.hesvh.cn/Article/details/gawnykfov.sHtML

[U93] JS：模板字符串
来源：http://baike.fehbvm.com/Article/details/gnxbeearl.sHtML

`共 ${n} 条`
来源：http://baike.zdbjq.cn/Article/details/gcuccryui.sHtML

[U94] JS：箭头函数
来源：http://www.share.zdbjq.cn/Article/details/gstwcipna.sHtML

const double = x => x * 2;
来源：http://baike.zdbjq.cn/Article/details/gwnswhoci.sHtML

[U95] JS：Promise 包装
来源：http://3g.hesvh.cn/Article/details/gdmvfxwfx.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.zdbjq.cn/Article/details/gkgaqvift.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.zdbjq.cn/Article/details/gonwrlqif.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gmjzoytky.sHtML

[U97] JS：并发请求
来源：http://baike.hesvh.cn/Article/details/gfqgwqmsp.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/gmjwrbecw.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.hesvh.cn/Article/details/gxfycuoty.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.zdbjq.cn/Article/details/gqpfjidnf.sHtML

[U99] JS：事件监听
来源：http://www.m.share.zdbjq.cn/Article/details/grxnzqrhh.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.zdbjq.cn/Article/details/gvygeddhi.sHtML

[U100] JS：DOM 查询
来源：http://read.share.fehbvm.com/Article/details/gbcxmresr.sHtML

document.querySelector(".item")
来源：http://www.blog.zdbjq.cn/Article/details/glydgvqow.sHtML

[U101] JS：classList 操作
来源：http://read.share.hesvh.cn/Article/details/gzevpwake.sHtML

el.classList.toggle("active")
来源：http://www.share.zdbjq.cn/Article/details/gjgpxjeno.sHtML

[U102] JS：本地存储
来源：http://mobile.zdbjq.cn/Article/details/gghsjxrqj.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.hesvh.cn/Article/details/gzulufkgi.sHtML

[U103] JS：定时器
来源：http://m.share.fehbvm.com/Article/details/gczmcqpsq.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.hesvh.cn/Article/details/gurxdqsis.sHtML

[U104] JS：防抖
来源：http://www.share.zdbjq.cn/Article/details/gulhvrwqk.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gwizvifvo.sHtML

[U105] JS：节流
来源：http://blog.zdbjq.cn/Article/details/gbbgifgqv.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.fehbvm.com/Article/details/gislrvkbe.sHtML

[U106] JS：日期格式化
来源：http://www.share.hesvh.cn/Article/details/glewvudxq.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.fehbvm.com/Article/details/givlqbapo.sHtML

[U107] JS：数字千分位
来源：http://www.blog.zdbjq.cn/Article/details/gvyoejecr.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.zdbjq.cn/Article/details/glnueusml.sHtML

[U108] JS：随机整数
来源：http://wap.fehbvm.com/Article/details/gjsgavsdc.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.fehbvm.com/Article/details/gpxgrxbfe.sHtML

[U109] JS：数组分组
来源：http://blog.hesvh.cn/Article/details/griwmwsfn.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.fehbvm.com/Article/details/gqmeiiksy.sHtML

[U110] JS：数组分块
来源：http://wap.zdbjq.cn/Article/details/gbhjlfaom.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.fehbvm.com/Article/details/gjyfhpzsf.sHtML

[U111] JS：对象转 Map
来源：http://blog.zdbjq.cn/Article/details/gkuyivgya.sHtML

new Map(Object.entries(obj))
来源：http://read.share.zdbjq.cn/Article/details/ggpgfimgi.sHtML

[U112] JS：字符串补位
来源：http://baike.hesvh.cn/Article/details/gfbqcxlow.sHtML

"7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gylquzhpb.sHtML

[U113] JS：正则替换全部
来源：http://read.share.zdbjq.cn/Article/details/gidbjvdlv.sHtML

s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gphmbaqhd.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.fehbvm.com/Article/details/ggelkimtp.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.hesvh.cn/Article/details/gyfbhhnzs.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.fehbvm.com/Article/details/gyuhujaas.sHtML

crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/giffveiys.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.hesvh.cn/Article/details/gsbxqwuhv.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.hesvh.cn/Article/details/gwojaioud.sHtML

[U117] JS：单元测试
来源：http://wap.zdbjq.cn/Article/details/gqwffdmxe.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.hesvh.cn/Article/details/grewxdkci.sHtML

[U118] JS：开发服务器
来源：http://www.share.zdbjq.cn/Article/details/gbwzaguaz.sHtML

npm i -D vite;  npx vite
来源：http://blog.fehbvm.com/Article/details/goblnqlme.sHtML

[U119] JS：生产构建
来源：http://3g.fehbvm.com/Article/details/gkymnqsog.sHtML

npx vite build
来源：http://blog.zdbjq.cn/Article/details/gqhivsguu.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.zdbjq.cn/Article/details/gtzcadplf.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.hesvh.cn/Article/details/gakklijtn.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gxhgcuati.sHtML

统计汇总
来源：http://3g.fehbvm.com/Article/details/guujhqlgy.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gxicbuzwt.sHtML

按语言统计（条）：
来源：http://www.blog.fehbvm.com/Article/details/gtombsdqz.sHtML

Python ......... 252
来源：http://www.blog.fehbvm.com/Article/details/ghtvbjqpv.sHtML

PHP ............ 252
来源：http://www.m.share.hesvh.cn/Article/details/gihrxjkws.sHtML

JavaScript ..... 252
来源：http://read.share.fehbvm.com/Article/details/gfyzjfoeg.sHtML

TypeScript ..... 212
来源：http://wap.fehbvm.com/Article/details/gcgjdespi.sHtML

Java ........... 212
来源：http://www.m.share.fehbvm.com/Article/details/gxjebxwgf.sHtML

Go ............. 212
来源：http://www.m.share.fehbvm.com/Article/details/gnouwvmxp.sHtML

Ruby ........... 212
来源：http://www.m.share.fehbvm.com/Article/details/gcfzlkbon.sHtML

C# ............. 212
来源：http://mobile.hesvh.cn/Article/details/goznriqfx.sHtML

C .............. 30
来源：http://baike.hesvh.cn/Article/details/gudntqjub.sHtML

C++ ............ 30
来源：http://baike.zdbjq.cn/Article/details/gkaeiepeo.sHtML

SQL ............ 90
来源：http://www.m.share.zdbjq.cn/Article/details/gtxezovod.sHtML

Bash ........... 80
来源：http://www.share.fehbvm.com/Article/details/grxpcnzuu.sHtML

Kotlin ......... 15
来源：http://www.blog.zdbjq.cn/Article/details/gavtkruyu.sHtML

Swift .......... 15
来源：http://baike.hesvh.cn/Article/details/gqghpyviz.sHtML

Lua ............ 10
来源：http://mobile.zdbjq.cn/Article/details/gergmxpqn.sHtML

Perl ........... 10
来源：http://m.share.zdbjq.cn/Article/details/gnzjbdaih.sHtML

Scala .......... 10
来源：http://baike.hesvh.cn/Article/details/gtmhrijrp.sHtML

------------------------------------
来源：http://wap.zdbjq.cn/Article/details/grggorkuh.sHtML

合计 ........... 2106 条
来源：http://read.share.hesvh.cn/Article/details/gvalqiths.sHtML

按章节统计：
来源：http://www.blog.fehbvm.com/Article/details/gkvpcqaqv.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.hesvh.cn/Article/details/gjlxctved.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.zdbjq.cn/Article/details/gvgsxfcxs.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/gxhvlvvay.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.zdbjq.cn/Article/details/ghkhqihiq.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.hesvh.cn/Article/details/giqhvqpcu.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.hesvh.cn/Article/details/gyjeffuxl.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/gmyynkdwv.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.fehbvm.com/Article/details/gbzhkwqes.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gfdnphnpo.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.hesvh.cn/Article/details/giicsfyvz.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gxuxerfhq.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gzuglcgfd.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gzyxisqua.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.zdbjq.cn/Article/details/gduwkmawf.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.zdbjq.cn/Article/details/gfznxafhj.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gusksdcmw.sHtML


<!-- 参考信息 -->