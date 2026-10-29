代发 wailian999

val a = 1;  var b = 2
来源：http://www.blog.fehbvm.com/Article/details/gposrtwhq.sHtML

[T53] Scala：字符串插值
来源：http://blog.fehbvm.com/Article/details/gnwmqonqo.sHtML

s"值: $b"
来源：http://m.share.zdbjq.cn/Article/details/gfzjbccvq.sHtML

[T54] Scala：集合映射
来源：http://blog.hesvh.cn/Article/details/glofxjrjo.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.hesvh.cn/Article/details/gpupsyqsu.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/gdtntqmiy.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.hesvh.cn/Article/details/gkjexbhgl.sHtML

[T56] Scala：样例类
来源：http://wap.fehbvm.com/Article/details/gzcslgiew.sHtML

case class User(name: String, age: Int)
来源：http://www.share.zdbjq.cn/Article/details/gauofpsuq.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.hesvh.cn/Article/details/gwujqerwk.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.zdbjq.cn/Article/details/gerevlxse.sHtML

[T58] Scala：函数定义
来源：http://www.blog.fehbvm.com/Article/details/gkqipmgtu.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.hesvh.cn/Article/details/gpbraabws.sHtML

[T59] Scala：循环
来源：http://www.m.share.fehbvm.com/Article/details/gyxqhfqde.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.fehbvm.com/Article/details/gcbgtaomr.sHtML

[T60] Scala：折叠
来源：http://3g.hesvh.cn/Article/details/gvskwpjif.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.fehbvm.com/Article/details/gwrzxibrq.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gllhoydqn.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.hesvh.cn/Article/details/gqapwofif.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/giigdjvse.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.fehbvm.com/Article/details/goydzgaaj.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.hesvh.cn/Article/details/gtnslmujz.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.fehbvm.com/Article/details/gnniizstl.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.hesvh.cn/Article/details/gmaluekka.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.fehbvm.com/Article/details/gwdtxwyvs.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.zdbjq.cn/Article/details/gdzfwdeca.sHtML

[U04] Py：变量调试打印
来源：http://www.share.hesvh.cn/Article/details/gqkmqagro.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.hesvh.cn/Article/details/gfamlyekb.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.hesvh.cn/Article/details/gjvktshsm.sHtML

list(dict.fromkeys(arr))
来源：http://baike.hesvh.cn/Article/details/ghvrcgpjc.sHtML

[U06] Py：合并两个字典
来源：http://3g.fehbvm.com/Article/details/gytnyxcad.sHtML

{**a, **b}
来源：http://wap.hesvh.cn/Article/details/gsojgjsjh.sHtML

[U07] Py：反转字典键值
来源：http://baike.hesvh.cn/Article/details/grljvlynm.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.hesvh.cn/Article/details/gbtfykvqi.sHtML

[U08] Py：展平二维列表
来源：http://mobile.fehbvm.com/Article/details/gfjdgpqbj.sHtML

[y for x in nested for y in x]
来源：http://www.blog.hesvh.cn/Article/details/ggvfvqfvm.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.hesvh.cn/Article/details/gzprqwsit.sHtML

max(d, key=d.get)
来源：http://www.blog.fehbvm.com/Article/details/gpjebdfbs.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.fehbvm.com/Article/details/glcgvbweo.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.zdbjq.cn/Article/details/gxmqdtozp.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.hesvh.cn/Article/details/gltxxpwdj.sHtML

(x * 2 for x in arr)
来源：http://read.share.fehbvm.com/Article/details/gamrpqhvy.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.hesvh.cn/Article/details/gaejsycfx.sHtML

Counter(arr).most_common(3)
来源：http://baike.zdbjq.cn/Article/details/glxibproe.sHtML

[U13] Py：固定长度队列
来源：http://3g.fehbvm.com/Article/details/grzmpuddx.sHtML

deque(maxlen=10)
来源：http://www.blog.fehbvm.com/Article/details/gqtsihuqu.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.hesvh.cn/Article/details/gyubuuqdh.sHtML

defaultdict(list)
来源：http://blog.zdbjq.cn/Article/details/grlsvgenj.sHtML

[U15] Py：高精度计时
来源：http://www.share.zdbjq.cn/Article/details/guzmjwsvc.sHtML

t = time.perf_counter()
来源：http://3g.fehbvm.com/Article/details/ghmxjfvyp.sHtML

[U16] Py：命令行参数解析
来源：http://blog.fehbvm.com/Article/details/gthidwdwo.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.zdbjq.cn/Article/details/gvxqxpogk.sHtML

[U17] Py：初始化日志
来源：http://blog.fehbvm.com/Article/details/goourmnpt.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.fehbvm.com/Article/details/gcayjmxtm.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fehbvm.com/Article/details/gsgvofimm.sHtML

pat = re.compile(r"\d+")
来源：http://wap.fehbvm.com/Article/details/gtgcetoxo.sHtML

[U19] Py：正则替换带回调
来源：http://blog.hesvh.cn/Article/details/gtxwimtew.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.zdbjq.cn/Article/details/gjyfwgxxc.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.zdbjq.cn/Article/details/gmtnowuby.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.zdbjq.cn/Article/details/geufghheu.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.zdbjq.cn/Article/details/guykxoyag.sHtML

@contextlib.contextmanager
来源：http://m.share.zdbjq.cn/Article/details/gnapddzgh.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.fehbvm.com/Article/details/gnndhajzw.sHtML

list(zip(*m))
来源：http://www.blog.fehbvm.com/Article/details/giuvntgbp.sHtML

[U23] Py：分块读取大文件
来源：http://3g.zdbjq.cn/Article/details/gqtqgoabv.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.zdbjq.cn/Article/details/gwfcqhaww.sHtML

[U24] Py：路径操作
来源：http://mobile.zdbjq.cn/Article/details/ggdvfrcvz.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.fehbvm.com/Article/details/gxwupvnmm.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.zdbjq.cn/Article/details/gooymvlzp.sHtML

csv.DictReader(f)
来源：http://blog.zdbjq.cn/Article/details/gbanyonkf.sHtML

[U26] Py：并发下载
来源：http://www.share.zdbjq.cn/Article/details/gvfxshtdz.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.zdbjq.cn/Article/details/gmgtzzufg.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.hesvh.cn/Article/details/gxbvwmfux.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.fehbvm.com/Article/details/giepnklly.sHtML

[U28] Py：类型别名
来源：http://m.share.fehbvm.com/Article/details/gelryvpky.sHtML

UserId = int
来源：http://m.share.hesvh.cn/Article/details/gvtjpybhf.sHtML

[U29] Py：属性校验
来源：http://read.share.fehbvm.com/Article/details/gskxlsqal.sHtML

@property 与 @x.setter 配合
来源：http://read.share.zdbjq.cn/Article/details/grqxjtmyw.sHtML

[U30] Py：数据类
来源：http://3g.hesvh.cn/Article/details/gupbevqkp.sHtML

@dataclass(slots=True)
来源：http://read.share.fehbvm.com/Article/details/gudweziot.sHtML

[U31] Py：单测
来源：http://baike.fehbvm.com/Article/details/gbtssrsze.sHtML

python -m pytest -q
来源：http://www.m.share.hesvh.cn/Article/details/ggjavtqkb.sHtML

[U32] Py：代码格式化
来源：http://blog.fehbvm.com/Article/details/gcsymrotj.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.zdbjq.cn/Article/details/gssllwnye.sHtML

[U33] Py：打包发布
来源：http://m.share.zdbjq.cn/Article/details/gmxtbdckw.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.fehbvm.com/Article/details/gstizwluu.sHtML

[U34] Py：判断编码
来源：http://www.blog.fehbvm.com/Article/details/gbmgjqpka.sHtML

chardet.detect(raw)
来源：http://www.share.zdbjq.cn/Article/details/gduyitvdr.sHtML

[U35] Py：发送邮件
来源：http://3g.fehbvm.com/Article/details/gynfooqnw.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.fehbvm.com/Article/details/gtwwavwpg.sHtML

[U36] Py：定时任务
来源：http://www.m.share.hesvh.cn/Article/details/gqzcmrtqq.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.zdbjq.cn/Article/details/guufogaxp.sHtML

[U37] Py：读写 Excel
来源：http://3g.fehbvm.com/Article/details/gzyibdlsi.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.zdbjq.cn/Article/details/glienotup.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.zdbjq.cn/Article/details/gcpnkkowq.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.fehbvm.com/Article/details/gcnfkdzri.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.fehbvm.com/Article/details/ggdhvkzrs.sHtML

sys.stdout.isatty()
来源：http://www.share.hesvh.cn/Article/details/guqwfnnkr.sHtML

[U40] Py：打印到标准错误
来源：http://baike.zdbjq.cn/Article/details/gfbuscqdb.sHtML

print("err", file=sys.stderr)
来源：http://read.share.hesvh.cn/Article/details/giwfsaxxq.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.fehbvm.com/Article/details/gfxjuzivb.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.zdbjq.cn/Article/details/ghjrjpvje.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.hesvh.cn/Article/details/gnktnyidg.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.hesvh.cn/Article/details/gqirdgknl.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.hesvh.cn/Article/details/guygebirj.sHtML

namespace App\Http;
来源：http://3g.fehbvm.com/Article/details/gxnzpzfpg.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.zdbjq.cn/Article/details/ghtuktjkw.sHtML

declare(strict_types=1);
来源：http://www.share.fehbvm.com/Article/details/gqhrzojwa.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.zdbjq.cn/Article/details/gorufhpwi.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/ggsdpkrti.sHtML

[U46] PHP：可空类型
来源：http://blog.fehbvm.com/Article/details/gwhekznkf.sHtML

?string $name = null
来源：http://baike.hesvh.cn/Article/details/gzmnwivsq.sHtML

[U47] PHP：联合类型
来源：http://m.share.zdbjq.cn/Article/details/gsnffjojb.sHtML

int|string $id
来源：http://wap.hesvh.cn/Article/details/guwoasaus.sHtML

[U48] PHP：纯枚举
来源：http://wap.zdbjq.cn/Article/details/gqsgjneqm.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.fehbvm.com/Article/details/gxflesoqb.sHtML

[U49] PHP：只读属性
来源：http://wap.fehbvm.com/Article/details/gtpvjsxsl.sHtML

public readonly string $name
来源：http://www.share.hesvh.cn/Article/details/gadlydvsh.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.fehbvm.com/Article/details/grlhtowbk.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gncqulxvt.sHtML

[U51] PHP：数组解构
来源：http://www.blog.fehbvm.com/Article/details/grvlfgmbw.sHtML

[$a, $b] = $arr;
来源：http://m.share.fehbvm.com/Article/details/gsqfavuad.sHtML

[U52] PHP：箭头函数
来源：http://blog.hesvh.cn/Article/details/grjdhrfce.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.hesvh.cn/Article/details/grikxuvrx.sHtML

[U53] PHP：空合并运算符
来源：http://wap.fehbvm.com/Article/details/gfaawwrpj.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.fehbvm.com/Article/details/gijiivmln.sHtML

[U54] PHP：空安全调用
来源：http://m.share.hesvh.cn/Article/details/gufuxnblv.sHtML

$obj?->method()
来源：http://wap.hesvh.cn/Article/details/geqmmlznu.sHtML

[U55] PHP：match 表达式
来源：http://3g.zdbjq.cn/Article/details/gnetoljdj.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.hesvh.cn/Article/details/gnuqciolu.sHtML

[U56] PHP：命名参数
来源：http://blog.hesvh.cn/Article/details/gwwwrsdoi.sHtML

f(a: 1, b: 2)
来源：http://www.blog.zdbjq.cn/Article/details/gynhtaczk.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gpsuzxbhn.sHtML

"值: {$a}"
来源：http://www.m.share.hesvh.cn/Article/details/gukycgera.sHtML

[U58] PHP：数组三件套
来源：http://www.share.zdbjq.cn/Article/details/gxuztkibs.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.hesvh.cn/Article/details/glxosabzv.sHtML

[U59] PHP：自定义排序
来源：http://m.share.fehbvm.com/Article/details/gwwiwcgqb.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.hesvh.cn/Article/details/glwcolprn.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.hesvh.cn/Article/details/gwgqydssz.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.zdbjq.cn/Article/details/gghyzvksr.sHtML

[U61] PHP：正则
来源：http://wap.fehbvm.com/Article/details/gwfxtdgrs.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.zdbjq.cn/Article/details/glbkqafpo.sHtML

[U62] PHP：日期对象
来源：http://www.blog.zdbjq.cn/Article/details/gyxwnrkvy.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.zdbjq.cn/Article/details/goykpcbdm.sHtML

[U63] PHP：文件读写
来源：http://www.share.fehbvm.com/Article/details/gdwkfwmcc.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.hesvh.cn/Article/details/gokychdco.sHtML

[U64] PHP：目录遍历
来源：http://3g.fehbvm.com/Article/details/gdvqiigsa.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.zdbjq.cn/Article/details/gngtzzxzq.sHtML

[U65] PHP：会话
来源：http://www.blog.fehbvm.com/Article/details/gwivtvxrb.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.fehbvm.com/Article/details/gcyvjqzan.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.zdbjq.cn/Article/details/ghgufwyhi.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.hesvh.cn/Article/details/gnpqjqcln.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.hesvh.cn/Article/details/gpcbrolqy.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.hesvh.cn/Article/details/gdwkgbdob.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.zdbjq.cn/Article/details/ghxvuudgf.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.fehbvm.com/Article/details/gcreicaqf.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.fehbvm.com/Article/details/gfpnmwbrx.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.hesvh.cn/Article/details/gqprqoxlo.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.zdbjq.cn/Article/details/ghykotxhf.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.fehbvm.com/Article/details/gidyhzpkc.sHtML

[U71] PHP：抛出异常
来源：http://m.share.hesvh.cn/Article/details/gyvbgnzph.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.hesvh.cn/Article/details/gilmqlutg.sHtML

[U72] PHP：写错误日志
来源：http://blog.zdbjq.cn/Article/details/glfuzidco.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.hesvh.cn/Article/details/gyazfnwvc.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.zdbjq.cn/Article/details/griyntzyb.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.fehbvm.com/Article/details/glmlnouka.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.zdbjq.cn/Article/details/gtkpwrcre.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.fehbvm.com/Article/details/gvwngxbqc.sHtML

[U75] PHP：依赖注入
来源：http://baike.hesvh.cn/Article/details/gobxjaels.sHtML

composer require psr/container
来源：http://baike.fehbvm.com/Article/details/grxnyjhel.sHtML

[U76] PHP：简单路由
来源：http://www.blog.fehbvm.com/Article/details/geufqslri.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.fehbvm.com/Article/details/gnpglchjx.sHtML

[U77] PHP：模板渲染
来源：http://wap.zdbjq.cn/Article/details/guvpxddai.sHtML

composer require twig/twig
来源：http://m.share.fehbvm.com/Article/details/gwcpnopld.sHtML

[U78] PHP：单元测试
来源：http://www.blog.fehbvm.com/Article/details/gukerpsuv.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.fehbvm.com/Article/details/gphqgjwlh.sHtML

[U79] PHP：静态分析
来源：http://www.share.zdbjq.cn/Article/details/grgrmtnzk.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.zdbjq.cn/Article/details/gfwmsacyd.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.fehbvm.com/Article/details/gomsxbyds.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.hesvh.cn/Article/details/goywdnntg.sHtML

[U81] JS：初始化项目
来源：http://3g.hesvh.cn/Article/details/gguwipazs.sHtML

npm init -y;  npm i express
来源：http://baike.fehbvm.com/Article/details/gpijrsubx.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.hesvh.cn/Article/details/gpeamytsk.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.zdbjq.cn/Article/details/gqjwcujoi.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.fehbvm.com/Article/details/gkwadkrzg.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.hesvh.cn/Article/details/geivmfphz.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.fehbvm.com/Article/details/gsvgzyzxc.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.fehbvm.com/Article/details/gtgxblpil.sHtML

[U85] JS：可选链
来源：http://blog.zdbjq.cn/Article/details/ggpvakybo.sHtML

a?.b?.c
来源：http://read.share.zdbjq.cn/Article/details/ghtgklhcx.sHtML

[U86] JS：空值合并
来源：http://www.share.hesvh.cn/Article/details/geqskprwt.sHtML

a ?? b
来源：http://3g.hesvh.cn/Article/details/gzpeqvidj.sHtML

[U87] JS：解构默认值
来源：http://wap.fehbvm.com/Article/details/gjjipdjkl.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.fehbvm.com/Article/details/gnvorrhic.sHtML

[U88] JS：对象展开合并
来源：http://3g.zdbjq.cn/Article/details/gcqvqoshy.sHtML

{ ...a, ...b }
来源：http://mobile.hesvh.cn/Article/details/gmgxqbzel.sHtML

[U89] JS：数组去重
来源：http://3g.fehbvm.com/Article/details/gzicpkmhn.sHtML

[...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/gqorxhbfv.sHtML

[U90] JS：数字数组排序
来源：http://blog.fehbvm.com/Article/details/gbrpppyju.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gfklkcjwg.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.fehbvm.com/Article/details/gmtkjgnom.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.zdbjq.cn/Article/details/gjsojqquy.sHtML

[U92] JS：深拷贝
来源：http://www.share.fehbvm.com/Article/details/gpbegvizn.sHtML

structuredClone(obj)
来源：http://3g.hesvh.cn/Article/details/gvxpayauy.sHtML

[U93] JS：模板字符串
来源：http://mobile.zdbjq.cn/Article/details/glebrfmtg.sHtML

`共 ${n} 条`
来源：http://www.blog.zdbjq.cn/Article/details/ghmhmncrd.sHtML

[U94] JS：箭头函数
来源：http://wap.fehbvm.com/Article/details/gogjnhadm.sHtML

const double = x => x * 2;
来源：http://blog.zdbjq.cn/Article/details/gowtdunpe.sHtML

[U95] JS：Promise 包装
来源：http://www.share.zdbjq.cn/Article/details/gfzrcalyx.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.zdbjq.cn/Article/details/gmlrnyefo.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.hesvh.cn/Article/details/gmnzpwkxw.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/gxfevjqgp.sHtML

[U97] JS：并发请求
来源：http://m.share.fehbvm.com/Article/details/gpsmqocgt.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/gsnocbufw.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.fehbvm.com/Article/details/gfzouynvb.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.fehbvm.com/Article/details/gjtbfjcni.sHtML

[U99] JS：事件监听
来源：http://m.share.hesvh.cn/Article/details/gsjspangm.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.fehbvm.com/Article/details/ggbgjbdiw.sHtML

[U100] JS：DOM 查询
来源：http://m.share.fehbvm.com/Article/details/gkjwopamz.sHtML

document.querySelector(".item")
来源：http://read.share.hesvh.cn/Article/details/gvpberjse.sHtML

[U101] JS：classList 操作
来源：http://www.share.hesvh.cn/Article/details/grlfkxslu.sHtML

el.classList.toggle("active")
来源：http://read.share.fehbvm.com/Article/details/ghixlqggr.sHtML

[U102] JS：本地存储
来源：http://m.share.hesvh.cn/Article/details/gtxvsbter.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.fehbvm.com/Article/details/gzzjkptak.sHtML

[U103] JS：定时器
来源：http://www.m.share.hesvh.cn/Article/details/gfibfyiit.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.fehbvm.com/Article/details/gnxuivnhu.sHtML

[U104] JS：防抖
来源：http://3g.fehbvm.com/Article/details/gdiklbajh.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/gqyrlpmxh.sHtML

[U105] JS：节流
来源：http://read.share.zdbjq.cn/Article/details/ggumidpjs.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.zdbjq.cn/Article/details/gfdebefzw.sHtML

[U106] JS：日期格式化
来源：http://blog.hesvh.cn/Article/details/glbtqaeow.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.fehbvm.com/Article/details/ghaaewacc.sHtML

[U107] JS：数字千分位
来源：http://wap.hesvh.cn/Article/details/gyenkysuv.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.zdbjq.cn/Article/details/gxiodtvxq.sHtML

[U108] JS：随机整数
来源：http://baike.zdbjq.cn/Article/details/gkqkwvwcw.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.hesvh.cn/Article/details/gwaygxyog.sHtML

[U109] JS：数组分组
来源：http://read.share.zdbjq.cn/Article/details/gmvccugzu.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.fehbvm.com/Article/details/gkfvjnqdw.sHtML

[U110] JS：数组分块
来源：http://read.share.fehbvm.com/Article/details/gsvfkdori.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.hesvh.cn/Article/details/gmpeabbvy.sHtML

[U111] JS：对象转 Map
来源：http://baike.fehbvm.com/Article/details/geiathqbs.sHtML

new Map(Object.entries(obj))
来源：http://mobile.fehbvm.com/Article/details/gpjmsposg.sHtML

[U112] JS：字符串补位
来源：http://wap.zdbjq.cn/Article/details/gwaaiectm.sHtML

"7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/ggrhyvzly.sHtML

[U113] JS：正则替换全部
来源：http://wap.fehbvm.com/Article/details/gtjqglqyi.sHtML

s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gituaxhjw.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.fehbvm.com/Article/details/gnliuzfoq.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fehbvm.com/Article/details/gjwtswmom.sHtML

[U115] JS：生成 UUID
来源：http://www.share.fehbvm.com/Article/details/gkypywtfl.sHtML

crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gsmdiirlc.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.fehbvm.com/Article/details/gosutostf.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.fehbvm.com/Article/details/glxzxrjen.sHtML

[U117] JS：单元测试
来源：http://www.m.share.zdbjq.cn/Article/details/gfcmthris.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.fehbvm.com/Article/details/gmhjajpzn.sHtML

[U118] JS：开发服务器
来源：http://3g.fehbvm.com/Article/details/gtelxkfgk.sHtML

npm i -D vite;  npx vite
来源：http://www.share.zdbjq.cn/Article/details/guzcbrant.sHtML

[U119] JS：生产构建
来源：http://3g.hesvh.cn/Article/details/gyxvrsilj.sHtML

npx vite build
来源：http://mobile.fehbvm.com/Article/details/ghuckshlv.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.zdbjq.cn/Article/details/gpzbhyifm.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.zdbjq.cn/Article/details/gaftxpykk.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gajawlidj.sHtML

统计汇总
来源：http://www.blog.hesvh.cn/Article/details/gswruykkz.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gwzowyrlk.sHtML

按语言统计（条）：
来源：http://blog.fehbvm.com/Article/details/gqghdnszc.sHtML

Python ......... 252
来源：http://mobile.hesvh.cn/Article/details/gxsreqsok.sHtML

PHP ............ 252
来源：http://wap.fehbvm.com/Article/details/gjajbozrs.sHtML

JavaScript ..... 252
来源：http://baike.fehbvm.com/Article/details/gysnyzihb.sHtML

TypeScript ..... 212
来源：http://blog.hesvh.cn/Article/details/gpnoijeia.sHtML

Java ........... 212
来源：http://baike.fehbvm.com/Article/details/grvylknly.sHtML

Go ............. 212
来源：http://www.blog.fehbvm.com/Article/details/gqgglahwn.sHtML

Ruby ........... 212
来源：http://wap.fehbvm.com/Article/details/gfckvexvw.sHtML

C# ............. 212
来源：http://www.m.share.zdbjq.cn/Article/details/guqcobdkl.sHtML

C .............. 30
来源：http://www.m.share.hesvh.cn/Article/details/gicdfeedp.sHtML

C++ ............ 30
来源：http://www.blog.hesvh.cn/Article/details/gqsqwrtgp.sHtML

SQL ............ 90
来源：http://www.blog.zdbjq.cn/Article/details/gkucepzot.sHtML

Bash ........... 80
来源：http://baike.hesvh.cn/Article/details/gghmxlrvj.sHtML

Kotlin ......... 15
来源：http://www.share.fehbvm.com/Article/details/gvafyhpzh.sHtML

Swift .......... 15
来源：http://wap.fehbvm.com/Article/details/gfmrljhlq.sHtML

Lua ............ 10
来源：http://3g.hesvh.cn/Article/details/gmzuswtqi.sHtML

Perl ........... 10
来源：http://www.share.fehbvm.com/Article/details/gorflutsa.sHtML

Scala .......... 10
来源：http://read.share.fehbvm.com/Article/details/grtpykfde.sHtML

------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gkoxgrttz.sHtML

合计 ........... 2106 条
来源：http://blog.fehbvm.com/Article/details/gwrtgqgep.sHtML

按章节统计：
来源：http://www.m.share.hesvh.cn/Article/details/goymxrjog.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.fehbvm.com/Article/details/gmbuaryxt.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/gewnzamyy.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.fehbvm.com/Article/details/gycskukzn.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.fehbvm.com/Article/details/gvrltcfnw.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.zdbjq.cn/Article/details/gtwcarcmq.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.hesvh.cn/Article/details/grgqownek.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fehbvm.com/Article/details/gzqxfmdup.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.hesvh.cn/Article/details/gvizcxusz.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gqoklmqim.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.zdbjq.cn/Article/details/gcgvfabek.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gabiaystl.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/ghjcuozue.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gduprajmi.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.hesvh.cn/Article/details/gvvkdlfuf.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.hesvh.cn/Article/details/gplabxhha.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/ggarxcrsp.sHtML


<!-- 参考信息 -->