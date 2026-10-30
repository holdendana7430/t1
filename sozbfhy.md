代发 wailian999

val a = 1;  var b = 2
来源：http://3g.zdbjq.cn/Article/details/gfqozlhro.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gtzluarmk.sHtML

s"值: $b"
来源：http://baike.fehbvm.com/Article/details/ggqgphdoh.sHtML

[T54] Scala：集合映射
来源：http://m.share.zdbjq.cn/Article/details/gkcxajcdw.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.fehbvm.com/Article/details/geirngsih.sHtML

[T55] Scala：集合过滤
来源：http://3g.fehbvm.com/Article/details/gqxqkuthn.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.zdbjq.cn/Article/details/gqdttullq.sHtML

[T56] Scala：样例类
来源：http://mobile.zdbjq.cn/Article/details/gztvjpzhb.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.zdbjq.cn/Article/details/gaswpehvm.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fehbvm.com/Article/details/gguxeowmd.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.zdbjq.cn/Article/details/gadnzowko.sHtML

[T58] Scala：函数定义
来源：http://wap.hesvh.cn/Article/details/gpmdhmdbp.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fehbvm.com/Article/details/gamlvojup.sHtML

[T59] Scala：循环
来源：http://read.share.zdbjq.cn/Article/details/gaejdipnm.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/ggagsgwvw.sHtML

[T60] Scala：折叠
来源：http://3g.hesvh.cn/Article/details/gtxlxudlv.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.fehbvm.com/Article/details/gpkvigqdz.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gngwbbsjw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.hesvh.cn/Article/details/gygnfefqn.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gjzezybsc.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.zdbjq.cn/Article/details/gbpuehpwv.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.hesvh.cn/Article/details/gqpxuuptv.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.zdbjq.cn/Article/details/gzncsxndv.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.hesvh.cn/Article/details/gacjcncle.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.hesvh.cn/Article/details/gbrxrjizu.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.fehbvm.com/Article/details/gkcjxhtoo.sHtML

[U04] Py：变量调试打印
来源：http://www.share.fehbvm.com/Article/details/grukvagdj.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.fehbvm.com/Article/details/gpyzhitnb.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.fehbvm.com/Article/details/gtdjtqzzs.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.zdbjq.cn/Article/details/guppenifh.sHtML

[U06] Py：合并两个字典
来源：http://wap.fehbvm.com/Article/details/gnwewsrxd.sHtML

{**a, **b}
来源：http://read.share.zdbjq.cn/Article/details/gggbobkiu.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.hesvh.cn/Article/details/gpljqlsip.sHtML

{v: k for k, v in d.items()}
来源：http://3g.fehbvm.com/Article/details/gliewxikg.sHtML

[U08] Py：展平二维列表
来源：http://m.share.zdbjq.cn/Article/details/gtjejzcxo.sHtML

[y for x in nested for y in x]
来源：http://baike.fehbvm.com/Article/details/gatwimkwu.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.fehbvm.com/Article/details/gpjmhtarq.sHtML

max(d, key=d.get)
来源：http://wap.hesvh.cn/Article/details/ghlguecdy.sHtML

[U10] Py：按值排序字典
来源：http://m.share.hesvh.cn/Article/details/gkxnfbzkm.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.fehbvm.com/Article/details/golmvckax.sHtML

[U11] Py：生成器表达式
来源：http://mobile.zdbjq.cn/Article/details/gbtmxyoov.sHtML

(x * 2 for x in arr)
来源：http://3g.zdbjq.cn/Article/details/gqyfjynbf.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.hesvh.cn/Article/details/gbopulyly.sHtML

Counter(arr).most_common(3)
来源：http://baike.fehbvm.com/Article/details/gqggnezdp.sHtML

[U13] Py：固定长度队列
来源：http://read.share.hesvh.cn/Article/details/gikkyrfpf.sHtML

deque(maxlen=10)
来源：http://www.blog.zdbjq.cn/Article/details/gwfdyrcdj.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.fehbvm.com/Article/details/ghsqtxqrj.sHtML

defaultdict(list)
来源：http://wap.fehbvm.com/Article/details/gmpmdqdps.sHtML

[U15] Py：高精度计时
来源：http://mobile.fehbvm.com/Article/details/gtjgypfdl.sHtML

t = time.perf_counter()
来源：http://www.m.share.zdbjq.cn/Article/details/gnyjxbhnr.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.hesvh.cn/Article/details/gqrpxzdqk.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.zdbjq.cn/Article/details/ghcrzyrwf.sHtML

[U17] Py：初始化日志
来源：http://www.blog.hesvh.cn/Article/details/grackunsk.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.zdbjq.cn/Article/details/gbtkwsyhx.sHtML

[U18] Py：预编译正则
来源：http://www.share.fehbvm.com/Article/details/ghfbyalxf.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fehbvm.com/Article/details/ghywnfmph.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.zdbjq.cn/Article/details/gbnqsjdku.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.hesvh.cn/Article/details/gwajtbijn.sHtML

[U20] Py：缓存函数结果
来源：http://wap.fehbvm.com/Article/details/gfnqbcnws.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.hesvh.cn/Article/details/giinghayi.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.hesvh.cn/Article/details/gtgtvthmx.sHtML

@contextlib.contextmanager
来源：http://www.share.fehbvm.com/Article/details/gilopkgwn.sHtML

[U22] Py：矩阵转置
来源：http://m.share.fehbvm.com/Article/details/gstyvghtm.sHtML

list(zip(*m))
来源：http://read.share.hesvh.cn/Article/details/gsrktlwkn.sHtML

[U23] Py：分块读取大文件
来源：http://3g.zdbjq.cn/Article/details/gpcfammgr.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.hesvh.cn/Article/details/gtwlljnnc.sHtML

[U24] Py：路径操作
来源：http://www.share.zdbjq.cn/Article/details/gzdwpobrl.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.fehbvm.com/Article/details/gazetmbic.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.hesvh.cn/Article/details/gxujuhjys.sHtML

csv.DictReader(f)
来源：http://www.share.fehbvm.com/Article/details/gptcrfjuc.sHtML

[U26] Py：并发下载
来源：http://www.blog.zdbjq.cn/Article/details/gtdgdvkbg.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.zdbjq.cn/Article/details/gszbtgbfi.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fehbvm.com/Article/details/ggjwmbhib.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.hesvh.cn/Article/details/gscsrvfzi.sHtML

[U28] Py：类型别名
来源：http://blog.fehbvm.com/Article/details/gceqhgkdv.sHtML

UserId = int
来源：http://www.m.share.zdbjq.cn/Article/details/ghbquvlqm.sHtML

[U29] Py：属性校验
来源：http://wap.fehbvm.com/Article/details/gcecculmh.sHtML

@property 与 @x.setter 配合
来源：http://read.share.hesvh.cn/Article/details/garovjjnk.sHtML

[U30] Py：数据类
来源：http://www.share.fehbvm.com/Article/details/geavnqelu.sHtML

@dataclass(slots=True)
来源：http://www.blog.fehbvm.com/Article/details/gfeblcghi.sHtML

[U31] Py：单测
来源：http://www.blog.fehbvm.com/Article/details/gummaaiho.sHtML

python -m pytest -q
来源：http://m.share.hesvh.cn/Article/details/gzmbhaxlc.sHtML

[U32] Py：代码格式化
来源：http://3g.fehbvm.com/Article/details/gxtzysyxh.sHtML

ruff format . && ruff check --fix .
来源：http://baike.fehbvm.com/Article/details/gnnrrjnzn.sHtML

[U33] Py：打包发布
来源：http://www.m.share.fehbvm.com/Article/details/giympyvsf.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.zdbjq.cn/Article/details/gekqjhyzh.sHtML

[U34] Py：判断编码
来源：http://www.m.share.zdbjq.cn/Article/details/ghghdqmmc.sHtML

chardet.detect(raw)
来源：http://mobile.fehbvm.com/Article/details/gezotqmif.sHtML

[U35] Py：发送邮件
来源：http://wap.hesvh.cn/Article/details/gscqkpgcj.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.zdbjq.cn/Article/details/gqttckqsa.sHtML

[U36] Py：定时任务
来源：http://read.share.hesvh.cn/Article/details/gjdbgvasg.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.zdbjq.cn/Article/details/gpfevraih.sHtML

[U37] Py：读写 Excel
来源：http://wap.zdbjq.cn/Article/details/gqfpjbgtg.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.hesvh.cn/Article/details/gxeneldei.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.zdbjq.cn/Article/details/glpfoutrm.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.zdbjq.cn/Article/details/gzbonzqlj.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.zdbjq.cn/Article/details/giiscbjiu.sHtML

sys.stdout.isatty()
来源：http://wap.zdbjq.cn/Article/details/gvmkrhghy.sHtML

[U40] Py：打印到标准错误
来源：http://blog.hesvh.cn/Article/details/gntvunftw.sHtML

print("err", file=sys.stderr)
来源：http://m.share.hesvh.cn/Article/details/gmneblqcx.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.fehbvm.com/Article/details/gskkhxwho.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.zdbjq.cn/Article/details/gmhtgnfki.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.hesvh.cn/Article/details/ghxdnpcfe.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.zdbjq.cn/Article/details/ghyrbmlhs.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.fehbvm.com/Article/details/glsysulla.sHtML

namespace App\Http;
来源：http://read.share.zdbjq.cn/Article/details/gghxwquho.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.fehbvm.com/Article/details/gipqwdpdd.sHtML

declare(strict_types=1);
来源：http://mobile.hesvh.cn/Article/details/gandnnwug.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.hesvh.cn/Article/details/glvyfgont.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gjsogcnkw.sHtML

[U46] PHP：可空类型
来源：http://read.share.zdbjq.cn/Article/details/gkayfahoo.sHtML

?string $name = null
来源：http://www.m.share.hesvh.cn/Article/details/gkgmlwlgf.sHtML

[U47] PHP：联合类型
来源：http://www.blog.hesvh.cn/Article/details/gvvrwcvsd.sHtML

int|string $id
来源：http://mobile.zdbjq.cn/Article/details/gfslswojs.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.zdbjq.cn/Article/details/ggtghtbkx.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gyqinlxio.sHtML

[U49] PHP：只读属性
来源：http://mobile.hesvh.cn/Article/details/guddsxapr.sHtML

public readonly string $name
来源：http://m.share.hesvh.cn/Article/details/gjidjaugi.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.fehbvm.com/Article/details/gnajgvogu.sHtML

public function __construct(private int $id) {}
来源：http://blog.fehbvm.com/Article/details/gyextbmxv.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.hesvh.cn/Article/details/glzfiyjmk.sHtML

[$a, $b] = $arr;
来源：http://www.share.fehbvm.com/Article/details/gjlipeusf.sHtML

[U52] PHP：箭头函数
来源：http://mobile.fehbvm.com/Article/details/gvbhvcvkn.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.fehbvm.com/Article/details/gxsyeeofc.sHtML

[U53] PHP：空合并运算符
来源：http://blog.zdbjq.cn/Article/details/gjhroxkfh.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.fehbvm.com/Article/details/graokykqd.sHtML

[U54] PHP：空安全调用
来源：http://mobile.hesvh.cn/Article/details/gyijqbafh.sHtML

$obj?->method()
来源：http://www.share.fehbvm.com/Article/details/gincgkpoh.sHtML

[U55] PHP：match 表达式
来源：http://read.share.zdbjq.cn/Article/details/gmpqjyojm.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.zdbjq.cn/Article/details/gsxnzqjqe.sHtML

[U56] PHP：命名参数
来源：http://mobile.zdbjq.cn/Article/details/gjptndkab.sHtML

f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/glmmosghh.sHtML

[U57] PHP：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gkzqfbzxd.sHtML

"值: {$a}"
来源：http://read.share.hesvh.cn/Article/details/gidaksjnv.sHtML

[U58] PHP：数组三件套
来源：http://wap.fehbvm.com/Article/details/gfgvwielh.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.hesvh.cn/Article/details/gkygzovwr.sHtML

[U59] PHP：自定义排序
来源：http://baike.fehbvm.com/Article/details/gflesatad.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fehbvm.com/Article/details/gemtddfns.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.zdbjq.cn/Article/details/gqcewkmrj.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.fehbvm.com/Article/details/gdnlfuvil.sHtML

[U61] PHP：正则
来源：http://read.share.hesvh.cn/Article/details/giedtsals.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.fehbvm.com/Article/details/gzisiszlt.sHtML

[U62] PHP：日期对象
来源：http://mobile.fehbvm.com/Article/details/gfecboprj.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.hesvh.cn/Article/details/gxlueahnb.sHtML

[U63] PHP：文件读写
来源：http://mobile.zdbjq.cn/Article/details/gfxyaqgfh.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.hesvh.cn/Article/details/gtdtvwrvq.sHtML

[U64] PHP：目录遍历
来源：http://m.share.fehbvm.com/Article/details/gwrmmbfzg.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.hesvh.cn/Article/details/gsdelpnax.sHtML

[U65] PHP：会话
来源：http://3g.zdbjq.cn/Article/details/gqhzznkcm.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gltfuaont.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.hesvh.cn/Article/details/gpqimomin.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.zdbjq.cn/Article/details/gdwmoupco.sHtML

[U67] PHP：处理文件上传
来源：http://blog.fehbvm.com/Article/details/gofhmunmi.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.fehbvm.com/Article/details/gprtmkwlk.sHtML

[U68] PHP：PDO 连接
来源：http://blog.hesvh.cn/Article/details/gnodimjze.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.hesvh.cn/Article/details/gpemjghxu.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.hesvh.cn/Article/details/gaofpaybl.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.hesvh.cn/Article/details/gmfrlegrk.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.zdbjq.cn/Article/details/gefpemyll.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.zdbjq.cn/Article/details/gtcmgudfs.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.zdbjq.cn/Article/details/gduvrksla.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.hesvh.cn/Article/details/gczuvvhro.sHtML

[U72] PHP：写错误日志
来源：http://3g.hesvh.cn/Article/details/gmxrespgs.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.fehbvm.com/Article/details/govlzqvrb.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.zdbjq.cn/Article/details/gkzadwtua.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.zdbjq.cn/Article/details/gykhzcdgn.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.zdbjq.cn/Article/details/gdbmolloi.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.hesvh.cn/Article/details/gqlfkzopf.sHtML

[U75] PHP：依赖注入
来源：http://blog.hesvh.cn/Article/details/gekggtxtx.sHtML

composer require psr/container
来源：http://baike.zdbjq.cn/Article/details/gwnfabauq.sHtML

[U76] PHP：简单路由
来源：http://m.share.zdbjq.cn/Article/details/gqsclpwxz.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.zdbjq.cn/Article/details/gaeaceikn.sHtML

[U77] PHP：模板渲染
来源：http://baike.zdbjq.cn/Article/details/gtebcuwij.sHtML

composer require twig/twig
来源：http://baike.zdbjq.cn/Article/details/gvojolvcq.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.hesvh.cn/Article/details/glhvgvoql.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.hesvh.cn/Article/details/ghvqjilot.sHtML

[U79] PHP：静态分析
来源：http://mobile.hesvh.cn/Article/details/gpqaxydud.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.fehbvm.com/Article/details/gxrqiglvw.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.fehbvm.com/Article/details/gqokokjpr.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.hesvh.cn/Article/details/gkinfwgrj.sHtML

[U81] JS：初始化项目
来源：http://read.share.zdbjq.cn/Article/details/grdrpusds.sHtML

npm init -y;  npm i express
来源：http://wap.hesvh.cn/Article/details/gdvjkmyrd.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.hesvh.cn/Article/details/gbtagoidq.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.hesvh.cn/Article/details/glslxomcf.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.zdbjq.cn/Article/details/gdwbllatj.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.fehbvm.com/Article/details/gbzqvndjl.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.fehbvm.com/Article/details/grhzjbkey.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.zdbjq.cn/Article/details/gonjfppww.sHtML

[U85] JS：可选链
来源：http://3g.zdbjq.cn/Article/details/gdzfeuqxm.sHtML

a?.b?.c
来源：http://wap.fehbvm.com/Article/details/glrabkkad.sHtML

[U86] JS：空值合并
来源：http://m.share.zdbjq.cn/Article/details/gndfrrmsu.sHtML

a ?? b
来源：http://m.share.fehbvm.com/Article/details/gvoqdllcb.sHtML

[U87] JS：解构默认值
来源：http://m.share.zdbjq.cn/Article/details/gkxdxpklc.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.fehbvm.com/Article/details/gelzqqmby.sHtML

[U88] JS：对象展开合并
来源：http://read.share.hesvh.cn/Article/details/gidobthxb.sHtML

{ ...a, ...b }
来源：http://3g.zdbjq.cn/Article/details/gzjvjmjke.sHtML

[U89] JS：数组去重
来源：http://baike.zdbjq.cn/Article/details/gvndzcguc.sHtML

[...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/glnrbfoeb.sHtML

[U90] JS：数字数组排序
来源：http://mobile.hesvh.cn/Article/details/gwquudfay.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/glydnyrls.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.fehbvm.com/Article/details/gqqmnruhh.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.fehbvm.com/Article/details/gdfasszxi.sHtML

[U92] JS：深拷贝
来源：http://www.blog.hesvh.cn/Article/details/gmruaezhj.sHtML

structuredClone(obj)
来源：http://www.share.hesvh.cn/Article/details/gpuvhtvtl.sHtML

[U93] JS：模板字符串
来源：http://wap.fehbvm.com/Article/details/gruzptbob.sHtML

`共 ${n} 条`
来源：http://mobile.zdbjq.cn/Article/details/glewmncwp.sHtML

[U94] JS：箭头函数
来源：http://www.share.hesvh.cn/Article/details/gxmhyumzn.sHtML

const double = x => x * 2;
来源：http://baike.fehbvm.com/Article/details/gealoietd.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.hesvh.cn/Article/details/gjplkzdgw.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.hesvh.cn/Article/details/gdoimzxom.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.fehbvm.com/Article/details/gcbakjsui.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/gnaxzcwwl.sHtML

[U97] JS：并发请求
来源：http://baike.zdbjq.cn/Article/details/glhwnwvdr.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/gzsuwrvku.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.zdbjq.cn/Article/details/ggxncukaq.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.fehbvm.com/Article/details/gakgmuwhm.sHtML

[U99] JS：事件监听
来源：http://wap.fehbvm.com/Article/details/giyfszgbl.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.hesvh.cn/Article/details/gwessjypj.sHtML

[U100] JS：DOM 查询
来源：http://read.share.fehbvm.com/Article/details/gmibwjhty.sHtML

document.querySelector(".item")
来源：http://www.m.share.zdbjq.cn/Article/details/gpmgypobd.sHtML

[U101] JS：classList 操作
来源：http://mobile.zdbjq.cn/Article/details/gmetqqdpt.sHtML

el.classList.toggle("active")
来源：http://www.share.hesvh.cn/Article/details/gigesiqlh.sHtML

[U102] JS：本地存储
来源：http://baike.fehbvm.com/Article/details/gookaxoll.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.zdbjq.cn/Article/details/ghifizywl.sHtML

[U103] JS：定时器
来源：http://mobile.zdbjq.cn/Article/details/gmogosync.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.hesvh.cn/Article/details/gpcjvbsio.sHtML

[U104] JS：防抖
来源：http://3g.fehbvm.com/Article/details/ghaxliokz.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/gewsntado.sHtML

[U105] JS：节流
来源：http://blog.fehbvm.com/Article/details/giocwazlr.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.zdbjq.cn/Article/details/gztzzxbdz.sHtML

[U106] JS：日期格式化
来源：http://www.share.hesvh.cn/Article/details/gwwdpdumf.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.zdbjq.cn/Article/details/grsyubrcy.sHtML

[U107] JS：数字千分位
来源：http://mobile.fehbvm.com/Article/details/gfqidkkgu.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.zdbjq.cn/Article/details/gyhvsttli.sHtML

[U108] JS：随机整数
来源：http://wap.zdbjq.cn/Article/details/gylqybnry.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.zdbjq.cn/Article/details/gnkavzmvn.sHtML

[U109] JS：数组分组
来源：http://3g.fehbvm.com/Article/details/ggilpgpje.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.zdbjq.cn/Article/details/gimulrhjf.sHtML

[U110] JS：数组分块
来源：http://m.share.fehbvm.com/Article/details/gonnyzush.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.zdbjq.cn/Article/details/gqnlqhpyf.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.hesvh.cn/Article/details/gzcgbohvp.sHtML

new Map(Object.entries(obj))
来源：http://m.share.zdbjq.cn/Article/details/giogsqzlg.sHtML

[U112] JS：字符串补位
来源：http://3g.zdbjq.cn/Article/details/ghszngmvi.sHtML

"7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gvhvsftgn.sHtML

[U113] JS：正则替换全部
来源：http://m.share.fehbvm.com/Article/details/gblxixzce.sHtML

s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/ghhqkpery.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.fehbvm.com/Article/details/gmahhcyjx.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fehbvm.com/Article/details/godxtenzd.sHtML

[U115] JS：生成 UUID
来源：http://3g.hesvh.cn/Article/details/ghmienyxg.sHtML

crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gzfyhlytk.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.hesvh.cn/Article/details/grauuaiub.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.fehbvm.com/Article/details/glfsklgel.sHtML

[U117] JS：单元测试
来源：http://www.m.share.fehbvm.com/Article/details/gcqnofnde.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.hesvh.cn/Article/details/gyfpkxyth.sHtML

[U118] JS：开发服务器
来源：http://mobile.hesvh.cn/Article/details/gdqdxfkzn.sHtML

npm i -D vite;  npx vite
来源：http://www.share.zdbjq.cn/Article/details/gwezcrzho.sHtML

[U119] JS：生产构建
来源：http://mobile.hesvh.cn/Article/details/gvcluckli.sHtML

npx vite build
来源：http://baike.zdbjq.cn/Article/details/gvvqopraz.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.hesvh.cn/Article/details/gpzjmeqio.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.zdbjq.cn/Article/details/gfrjbjwvi.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gvqeluaje.sHtML

统计汇总
来源：http://www.blog.fehbvm.com/Article/details/gkqgwsxkn.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gllfseydg.sHtML

按语言统计（条）：
来源：http://wap.hesvh.cn/Article/details/gaerlokaq.sHtML

Python ......... 252
来源：http://www.share.hesvh.cn/Article/details/gocrctrjo.sHtML

PHP ............ 252
来源：http://wap.fehbvm.com/Article/details/giqkybzfp.sHtML

JavaScript ..... 252
来源：http://www.m.share.zdbjq.cn/Article/details/gfedwlnxa.sHtML

TypeScript ..... 212
来源：http://www.m.share.zdbjq.cn/Article/details/gkwgiamsl.sHtML

Java ........... 212
来源：http://mobile.fehbvm.com/Article/details/gybqisoxl.sHtML

Go ............. 212
来源：http://www.blog.zdbjq.cn/Article/details/gzoonfizy.sHtML

Ruby ........... 212
来源：http://www.blog.fehbvm.com/Article/details/gwzeeseon.sHtML

C# ............. 212
来源：http://3g.fehbvm.com/Article/details/ghvvvbsij.sHtML

C .............. 30
来源：http://baike.zdbjq.cn/Article/details/gcfpwakli.sHtML

C++ ............ 30
来源：http://read.share.zdbjq.cn/Article/details/gtzuaojsi.sHtML

SQL ............ 90
来源：http://m.share.fehbvm.com/Article/details/goqqujxon.sHtML

Bash ........... 80
来源：http://blog.zdbjq.cn/Article/details/gqupxarwk.sHtML

Kotlin ......... 15
来源：http://mobile.fehbvm.com/Article/details/gwqlzbyzp.sHtML

Swift .......... 15
来源：http://blog.fehbvm.com/Article/details/gujiqzxnd.sHtML

Lua ............ 10
来源：http://www.share.hesvh.cn/Article/details/glomvuoif.sHtML

Perl ........... 10
来源：http://baike.zdbjq.cn/Article/details/gjozjxcfh.sHtML

Scala .......... 10
来源：http://3g.zdbjq.cn/Article/details/gyybibsaa.sHtML

------------------------------------
来源：http://blog.fehbvm.com/Article/details/gytjiiytb.sHtML

合计 ........... 2106 条
来源：http://wap.hesvh.cn/Article/details/gpnuhnwdt.sHtML

按章节统计：
来源：http://m.share.zdbjq.cn/Article/details/govxpnvyi.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.fehbvm.com/Article/details/ggkjvixfj.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/gjnnbxpql.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/ghunffeof.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.zdbjq.cn/Article/details/gvdlxlyhc.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.hesvh.cn/Article/details/gfmvoitsb.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.zdbjq.cn/Article/details/gvlnqeyrp.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/goldtrywo.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.zdbjq.cn/Article/details/gczkeurrg.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gbbcoorpf.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.zdbjq.cn/Article/details/gbupidivq.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gknbnpvsx.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gpjdznvlm.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gyumbfmge.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.zdbjq.cn/Article/details/glnboxqyb.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.fehbvm.com/Article/details/gbkprhymj.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gnwhdnwgp.sHtML


<!-- 参考信息 -->