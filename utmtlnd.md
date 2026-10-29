代发 wailian999

while (my $line = <$fh>) { print $line; }
来源：http://blog.fehbvm.com/Article/details/gezhtoueb.sHtML

[T51] Scala：Hello World
来源：http://www.share.hesvh.cn/Article/details/ggxodsznt.sHtML

println("Hello")
来源：http://mobile.zdbjq.cn/Article/details/geicjnclb.sHtML

[T52] Scala：变量
来源：http://baike.fehbvm.com/Article/details/gshwvxrqc.sHtML

val a = 1;  var b = 2
来源：http://read.share.fehbvm.com/Article/details/gbbfpxmwx.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gcsutrkby.sHtML

s"值: $b"
来源：http://mobile.hesvh.cn/Article/details/gxzdjuphd.sHtML

[T54] Scala：集合映射
来源：http://mobile.hesvh.cn/Article/details/gukpwjqmh.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gumtnapjo.sHtML

[T55] Scala：集合过滤
来源：http://blog.hesvh.cn/Article/details/gdzphhnvw.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.hesvh.cn/Article/details/grmoyjnvj.sHtML

[T56] Scala：样例类
来源：http://wap.hesvh.cn/Article/details/gzyvwotre.sHtML

case class User(name: String, age: Int)
来源：http://m.share.fehbvm.com/Article/details/gfegtbevc.sHtML

[T57] Scala：模式匹配
来源：http://baike.hesvh.cn/Article/details/gydlbuynp.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.hesvh.cn/Article/details/gplhssfix.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.zdbjq.cn/Article/details/gkymqkcnn.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.hesvh.cn/Article/details/gqdlxbkkb.sHtML

[T59] Scala：循环
来源：http://m.share.zdbjq.cn/Article/details/gkqbwwyyb.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.zdbjq.cn/Article/details/gzmozxlry.sHtML

[T60] Scala：折叠
来源：http://read.share.zdbjq.cn/Article/details/gknxamxci.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.hesvh.cn/Article/details/gulzvykub.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gjqrncjnp.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fehbvm.com/Article/details/gxmtdpygq.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gerzyanef.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.hesvh.cn/Article/details/glssdsdfy.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.hesvh.cn/Article/details/ghictmwzo.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.hesvh.cn/Article/details/gleigyowl.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.hesvh.cn/Article/details/ggfzupvos.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.zdbjq.cn/Article/details/gaokxwxsr.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.zdbjq.cn/Article/details/grhkcyklt.sHtML

[U04] Py：变量调试打印
来源：http://3g.hesvh.cn/Article/details/gzbswcdmc.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.fehbvm.com/Article/details/gdhwdxcsz.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.zdbjq.cn/Article/details/gnsxqfmzs.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.hesvh.cn/Article/details/gbvohhcod.sHtML

[U06] Py：合并两个字典
来源：http://mobile.hesvh.cn/Article/details/gsvplannj.sHtML

{**a, **b}
来源：http://m.share.zdbjq.cn/Article/details/guwdbsqxi.sHtML

[U07] Py：反转字典键值
来源：http://read.share.fehbvm.com/Article/details/gfsgftxxu.sHtML

{v: k for k, v in d.items()}
来源：http://wap.zdbjq.cn/Article/details/glomenqqm.sHtML

[U08] Py：展平二维列表
来源：http://www.share.zdbjq.cn/Article/details/gigdvfdcr.sHtML

[y for x in nested for y in x]
来源：http://read.share.zdbjq.cn/Article/details/gimzudmji.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.fehbvm.com/Article/details/gbtkioqwq.sHtML

max(d, key=d.get)
来源：http://www.m.share.hesvh.cn/Article/details/gjktqacmo.sHtML

[U10] Py：按值排序字典
来源：http://www.share.fehbvm.com/Article/details/genbvxctj.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.zdbjq.cn/Article/details/gppbzpinf.sHtML

[U11] Py：生成器表达式
来源：http://baike.zdbjq.cn/Article/details/gjmhxbkkw.sHtML

(x * 2 for x in arr)
来源：http://3g.hesvh.cn/Article/details/gpqgxbyck.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.fehbvm.com/Article/details/giibfmgtc.sHtML

Counter(arr).most_common(3)
来源：http://read.share.hesvh.cn/Article/details/ggtbnwkux.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.zdbjq.cn/Article/details/gqceaezdv.sHtML

deque(maxlen=10)
来源：http://baike.hesvh.cn/Article/details/gkdkocgak.sHtML

[U14] Py：分组收集到列表
来源：http://wap.hesvh.cn/Article/details/grxjfaqsb.sHtML

defaultdict(list)
来源：http://blog.zdbjq.cn/Article/details/geffddujh.sHtML

[U15] Py：高精度计时
来源：http://baike.fehbvm.com/Article/details/gheuhesvc.sHtML

t = time.perf_counter()
来源：http://baike.hesvh.cn/Article/details/gvhdrnxuw.sHtML

[U16] Py：命令行参数解析
来源：http://wap.hesvh.cn/Article/details/gvkfxebpf.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.fehbvm.com/Article/details/giqmthvjj.sHtML

[U17] Py：初始化日志
来源：http://m.share.hesvh.cn/Article/details/gfqhkgfnr.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.zdbjq.cn/Article/details/gmysywtmi.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.hesvh.cn/Article/details/gcycklflm.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.zdbjq.cn/Article/details/gavaslili.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.fehbvm.com/Article/details/gkkujvuxw.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.zdbjq.cn/Article/details/gmculvofu.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.fehbvm.com/Article/details/gxiyjhmbk.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.hesvh.cn/Article/details/gpipazpyc.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.zdbjq.cn/Article/details/gcxdhxscs.sHtML

@contextlib.contextmanager
来源：http://baike.zdbjq.cn/Article/details/gikdegtes.sHtML

[U22] Py：矩阵转置
来源：http://mobile.zdbjq.cn/Article/details/gwyrpipkd.sHtML

list(zip(*m))
来源：http://wap.zdbjq.cn/Article/details/gdplhmxol.sHtML

[U23] Py：分块读取大文件
来源：http://wap.fehbvm.com/Article/details/gojmgdbdt.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.zdbjq.cn/Article/details/gjqfmcxvv.sHtML

[U24] Py：路径操作
来源：http://www.m.share.fehbvm.com/Article/details/gkxftocmy.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.fehbvm.com/Article/details/gmkwkvysd.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.hesvh.cn/Article/details/gggpastyu.sHtML

csv.DictReader(f)
来源：http://www.m.share.hesvh.cn/Article/details/ggakxkxqw.sHtML

[U26] Py：并发下载
来源：http://3g.zdbjq.cn/Article/details/gooztswfo.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.zdbjq.cn/Article/details/gyxyhntup.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.fehbvm.com/Article/details/gfrgtpabh.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.hesvh.cn/Article/details/gfaxecaif.sHtML

[U28] Py：类型别名
来源：http://mobile.zdbjq.cn/Article/details/gkuqfrtqh.sHtML

UserId = int
来源：http://blog.zdbjq.cn/Article/details/gorbonlnk.sHtML

[U29] Py：属性校验
来源：http://baike.zdbjq.cn/Article/details/gylgtqwvj.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.hesvh.cn/Article/details/gtnfwjkel.sHtML

[U30] Py：数据类
来源：http://www.m.share.fehbvm.com/Article/details/gzlebzxaw.sHtML

@dataclass(slots=True)
来源：http://m.share.hesvh.cn/Article/details/gvrohvdmo.sHtML

[U31] Py：单测
来源：http://wap.hesvh.cn/Article/details/gfujddxkv.sHtML

python -m pytest -q
来源：http://wap.fehbvm.com/Article/details/gzkutvhrf.sHtML

[U32] Py：代码格式化
来源：http://m.share.zdbjq.cn/Article/details/gnnbagwut.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.zdbjq.cn/Article/details/gcieiqkar.sHtML

[U33] Py：打包发布
来源：http://www.share.hesvh.cn/Article/details/gqxdylzjn.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.hesvh.cn/Article/details/gimrovcpl.sHtML

[U34] Py：判断编码
来源：http://www.m.share.zdbjq.cn/Article/details/gjeqmpazy.sHtML

chardet.detect(raw)
来源：http://baike.zdbjq.cn/Article/details/gdkdotrgo.sHtML

[U35] Py：发送邮件
来源：http://read.share.fehbvm.com/Article/details/gqltfnyzd.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.fehbvm.com/Article/details/gfozxhqsz.sHtML

[U36] Py：定时任务
来源：http://m.share.zdbjq.cn/Article/details/glgspnasb.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.hesvh.cn/Article/details/gcpulaxiz.sHtML

[U37] Py：读写 Excel
来源：http://3g.hesvh.cn/Article/details/gobtctpnw.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.fehbvm.com/Article/details/gpklosbai.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.zdbjq.cn/Article/details/grrznrwue.sHtML

Path(__file__).resolve().parent
来源：http://mobile.hesvh.cn/Article/details/gzwplqdmz.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.fehbvm.com/Article/details/gozfqrzgf.sHtML

sys.stdout.isatty()
来源：http://blog.fehbvm.com/Article/details/ghujjhwcz.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.hesvh.cn/Article/details/gtdtserie.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.hesvh.cn/Article/details/gelrmjhwo.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.zdbjq.cn/Article/details/gpcfsbcfj.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.hesvh.cn/Article/details/gjxkujqqv.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.fehbvm.com/Article/details/gwjrfeppb.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.hesvh.cn/Article/details/gynynuirh.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.hesvh.cn/Article/details/grkjnyfss.sHtML

namespace App\Http;
来源：http://wap.hesvh.cn/Article/details/gnpuqqvxg.sHtML

[U44] PHP：开启严格类型
来源：http://3g.fehbvm.com/Article/details/gmznopkal.sHtML

declare(strict_types=1);
来源：http://wap.zdbjq.cn/Article/details/glgkdmfke.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.fehbvm.com/Article/details/gufdkdmvg.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gnaimtbyd.sHtML

[U46] PHP：可空类型
来源：http://blog.hesvh.cn/Article/details/gbsjpsyqf.sHtML

?string $name = null
来源：http://m.share.zdbjq.cn/Article/details/gvaeshqhm.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.zdbjq.cn/Article/details/gayjngqyx.sHtML

int|string $id
来源：http://mobile.hesvh.cn/Article/details/ggvlugotl.sHtML

[U48] PHP：纯枚举
来源：http://blog.zdbjq.cn/Article/details/gmsyxdscg.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.fehbvm.com/Article/details/gbpgtzqjr.sHtML

[U49] PHP：只读属性
来源：http://www.blog.hesvh.cn/Article/details/gqvzbmxhn.sHtML

public readonly string $name
来源：http://mobile.hesvh.cn/Article/details/gyvfnyxji.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.zdbjq.cn/Article/details/glkghvens.sHtML

public function __construct(private int $id) {}
来源：http://wap.fehbvm.com/Article/details/ggfkujlpa.sHtML

[U51] PHP：数组解构
来源：http://3g.zdbjq.cn/Article/details/gcjuvuhgp.sHtML

[$a, $b] = $arr;
来源：http://www.share.zdbjq.cn/Article/details/gtvvgxved.sHtML

[U52] PHP：箭头函数
来源：http://www.share.fehbvm.com/Article/details/gyglpbzzl.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.zdbjq.cn/Article/details/gtxqilyfi.sHtML

[U53] PHP：空合并运算符
来源：http://blog.zdbjq.cn/Article/details/gxwmrkzuz.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.zdbjq.cn/Article/details/gqbmeedct.sHtML

[U54] PHP：空安全调用
来源：http://3g.hesvh.cn/Article/details/gpgpdgozv.sHtML

$obj?->method()
来源：http://wap.zdbjq.cn/Article/details/gixmcvyqh.sHtML

[U55] PHP：match 表达式
来源：http://3g.fehbvm.com/Article/details/gzxcrnzsc.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.fehbvm.com/Article/details/gdsspvyrb.sHtML

[U56] PHP：命名参数
来源：http://wap.zdbjq.cn/Article/details/gbzckhthu.sHtML

f(a: 1, b: 2)
来源：http://read.share.fehbvm.com/Article/details/gonubfjnt.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gtybthbst.sHtML

"值: {$a}"
来源：http://wap.zdbjq.cn/Article/details/gopxyldri.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.hesvh.cn/Article/details/gyseziilb.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.zdbjq.cn/Article/details/glzxjonhb.sHtML

[U59] PHP：自定义排序
来源：http://read.share.fehbvm.com/Article/details/gwwcvfvzs.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.zdbjq.cn/Article/details/gzjfipgxc.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.hesvh.cn/Article/details/geojsufnb.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.zdbjq.cn/Article/details/gbfxkzjmx.sHtML

[U61] PHP：正则
来源：http://www.blog.zdbjq.cn/Article/details/grasasgqf.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gapcvupxm.sHtML

[U62] PHP：日期对象
来源：http://mobile.zdbjq.cn/Article/details/grjuinoub.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.zdbjq.cn/Article/details/ghzxehlxy.sHtML

[U63] PHP：文件读写
来源：http://wap.fehbvm.com/Article/details/gspujkyzi.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.zdbjq.cn/Article/details/gqsnuxwhx.sHtML

[U64] PHP：目录遍历
来源：http://wap.zdbjq.cn/Article/details/gfvcqiokb.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.hesvh.cn/Article/details/giqxmlykd.sHtML

[U65] PHP：会话
来源：http://baike.hesvh.cn/Article/details/gisrzhoxx.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gyvxmgylq.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.zdbjq.cn/Article/details/gyxcjiifk.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.zdbjq.cn/Article/details/ggbpaxerm.sHtML

[U67] PHP：处理文件上传
来源：http://baike.hesvh.cn/Article/details/gepnqepkw.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.fehbvm.com/Article/details/gyodeeuxc.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.hesvh.cn/Article/details/gdfhgdrff.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.fehbvm.com/Article/details/gaaizysnd.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.hesvh.cn/Article/details/giieretob.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.zdbjq.cn/Article/details/govubyktf.sHtML

[U70] PHP：PDO 事务
来源：http://wap.fehbvm.com/Article/details/gthiinqmc.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.fehbvm.com/Article/details/givaulrjn.sHtML

[U71] PHP：抛出异常
来源：http://m.share.hesvh.cn/Article/details/gbfgdaggb.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.zdbjq.cn/Article/details/ghfsgfnpu.sHtML

[U72] PHP：写错误日志
来源：http://www.share.zdbjq.cn/Article/details/grgbcheal.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.hesvh.cn/Article/details/gzbpcrsbp.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.fehbvm.com/Article/details/gpzkzztuu.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.hesvh.cn/Article/details/gmxnamigc.sHtML

[U74] PHP：读取环境变量
来源：http://blog.zdbjq.cn/Article/details/gcpdbxvdl.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.fehbvm.com/Article/details/gblziczzb.sHtML

[U75] PHP：依赖注入
来源：http://blog.zdbjq.cn/Article/details/gugvpvvkl.sHtML

composer require psr/container
来源：http://www.share.fehbvm.com/Article/details/gkfifgwdb.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.fehbvm.com/Article/details/gnwohrygl.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.zdbjq.cn/Article/details/grghbzzvn.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.fehbvm.com/Article/details/gxpjvoxdn.sHtML

composer require twig/twig
来源：http://3g.fehbvm.com/Article/details/gksednnuh.sHtML

[U78] PHP：单元测试
来源：http://www.share.zdbjq.cn/Article/details/gxvkercyx.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.hesvh.cn/Article/details/gnbkdcknt.sHtML

[U79] PHP：静态分析
来源：http://baike.hesvh.cn/Article/details/gfhbbivqd.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.zdbjq.cn/Article/details/gqpvtysnp.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.fehbvm.com/Article/details/gjncgyxhj.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.hesvh.cn/Article/details/gktdfzwkv.sHtML

[U81] JS：初始化项目
来源：http://blog.hesvh.cn/Article/details/gvutakcup.sHtML

npm init -y;  npm i express
来源：http://www.share.hesvh.cn/Article/details/gyuxanclv.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.hesvh.cn/Article/details/gyuwqzive.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.zdbjq.cn/Article/details/glrwtqinr.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.fehbvm.com/Article/details/gozdkxxri.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.fehbvm.com/Article/details/gesscbgnr.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.zdbjq.cn/Article/details/gocifjfjd.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.fehbvm.com/Article/details/gyrtlaeip.sHtML

[U85] JS：可选链
来源：http://wap.fehbvm.com/Article/details/gnibpmnst.sHtML

a?.b?.c
来源：http://www.blog.hesvh.cn/Article/details/gqrygatqa.sHtML

[U86] JS：空值合并
来源：http://mobile.zdbjq.cn/Article/details/gfozunqoj.sHtML

a ?? b
来源：http://3g.fehbvm.com/Article/details/gqtzrqpgc.sHtML

[U87] JS：解构默认值
来源：http://wap.fehbvm.com/Article/details/gsuwjbjte.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.zdbjq.cn/Article/details/gtmhkwhri.sHtML

[U88] JS：对象展开合并
来源：http://m.share.hesvh.cn/Article/details/goukqinah.sHtML

{ ...a, ...b }
来源：http://m.share.zdbjq.cn/Article/details/gvfgltzsv.sHtML

[U89] JS：数组去重
来源：http://www.m.share.fehbvm.com/Article/details/gkozjkpvh.sHtML

[...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gvtjdfoqm.sHtML

[U90] JS：数字数组排序
来源：http://m.share.hesvh.cn/Article/details/gvuzdwsxz.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/gvpcuhzmy.sHtML

[U91] JS：对象键值遍历
来源：http://blog.fehbvm.com/Article/details/grijhzhsx.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.hesvh.cn/Article/details/ggaqjasya.sHtML

[U92] JS：深拷贝
来源：http://www.blog.hesvh.cn/Article/details/gxvlorrfz.sHtML

structuredClone(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gupqtkxkc.sHtML

[U93] JS：模板字符串
来源：http://wap.fehbvm.com/Article/details/grzhieqqs.sHtML

`共 ${n} 条`
来源：http://m.share.hesvh.cn/Article/details/gtfjpqjbo.sHtML

[U94] JS：箭头函数
来源：http://www.blog.hesvh.cn/Article/details/gragltpfl.sHtML

const double = x => x * 2;
来源：http://baike.zdbjq.cn/Article/details/gcrbsdlil.sHtML

[U95] JS：Promise 包装
来源：http://baike.fehbvm.com/Article/details/gdzddtveu.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.zdbjq.cn/Article/details/grseljyak.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.fehbvm.com/Article/details/gmkrutxpn.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/gkaktdkra.sHtML

[U97] JS：并发请求
来源：http://m.share.zdbjq.cn/Article/details/garafezti.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/gyjspgeoh.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.fehbvm.com/Article/details/gmdghmlsm.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.fehbvm.com/Article/details/gnbvvajdl.sHtML

[U99] JS：事件监听
来源：http://www.m.share.fehbvm.com/Article/details/gprenysze.sHtML

el.addEventListener("click", e => {})
来源：http://wap.hesvh.cn/Article/details/gpgsolwjl.sHtML

[U100] JS：DOM 查询
来源：http://mobile.hesvh.cn/Article/details/gohvmgplx.sHtML

document.querySelector(".item")
来源：http://m.share.hesvh.cn/Article/details/gbnzimzhn.sHtML

[U101] JS：classList 操作
来源：http://wap.hesvh.cn/Article/details/gqrmbzcig.sHtML

el.classList.toggle("active")
来源：http://mobile.hesvh.cn/Article/details/ggnpkmnrm.sHtML

[U102] JS：本地存储
来源：http://mobile.fehbvm.com/Article/details/gffcqrpng.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.fehbvm.com/Article/details/gqplprwcb.sHtML

[U103] JS：定时器
来源：http://mobile.fehbvm.com/Article/details/gcxafebzk.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.fehbvm.com/Article/details/geetwckyq.sHtML

[U104] JS：防抖
来源：http://www.m.share.zdbjq.cn/Article/details/gpkexwluf.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/gzlvvmpat.sHtML

[U105] JS：节流
来源：http://baike.hesvh.cn/Article/details/goswffiah.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.zdbjq.cn/Article/details/glzhmsoyj.sHtML

[U106] JS：日期格式化
来源：http://read.share.zdbjq.cn/Article/details/gnlouiqqk.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.hesvh.cn/Article/details/gtmztzfmt.sHtML

[U107] JS：数字千分位
来源：http://m.share.fehbvm.com/Article/details/glxqqnxem.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.zdbjq.cn/Article/details/ggjhfmasf.sHtML

[U108] JS：随机整数
来源：http://m.share.zdbjq.cn/Article/details/gwnlwydvw.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.hesvh.cn/Article/details/gtdgjugqx.sHtML

[U109] JS：数组分组
来源：http://www.share.fehbvm.com/Article/details/gjejmbvkp.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.zdbjq.cn/Article/details/gpoatvdsq.sHtML

[U110] JS：数组分块
来源：http://www.share.fehbvm.com/Article/details/gfokiliae.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.hesvh.cn/Article/details/gupnstjsp.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.hesvh.cn/Article/details/grvkwalth.sHtML

new Map(Object.entries(obj))
来源：http://read.share.zdbjq.cn/Article/details/ghhhtaiwr.sHtML

[U112] JS：字符串补位
来源：http://mobile.zdbjq.cn/Article/details/gkdkrnaos.sHtML

"7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/guhdarpub.sHtML

[U113] JS：正则替换全部
来源：http://m.share.fehbvm.com/Article/details/gygkxbxnn.sHtML

s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gqntbbdlw.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.fehbvm.com/Article/details/gokqeftnm.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/gpqmvngrl.sHtML

[U115] JS：生成 UUID
来源：http://baike.hesvh.cn/Article/details/gdiegoczf.sHtML

crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/goprdvbec.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.fehbvm.com/Article/details/gjxnbmqts.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.fehbvm.com/Article/details/gdhmdtooe.sHtML

[U117] JS：单元测试
来源：http://www.blog.hesvh.cn/Article/details/gwecsydfm.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.fehbvm.com/Article/details/gvskwgoyg.sHtML

[U118] JS：开发服务器
来源：http://wap.hesvh.cn/Article/details/gndrxafcj.sHtML

npm i -D vite;  npx vite
来源：http://mobile.fehbvm.com/Article/details/gfiovfgwa.sHtML

[U119] JS：生产构建
来源：http://3g.zdbjq.cn/Article/details/gohsmktxc.sHtML

npx vite build
来源：http://www.blog.hesvh.cn/Article/details/gegbqkvjd.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.fehbvm.com/Article/details/gegsaxgwq.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.zdbjq.cn/Article/details/gxrkohuej.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gvfwyufxc.sHtML

统计汇总
来源：http://mobile.zdbjq.cn/Article/details/gwyowrvns.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/guxrznnvz.sHtML

按语言统计（条）：
来源：http://www.share.fehbvm.com/Article/details/gndkvljqb.sHtML

Python ......... 252
来源：http://mobile.zdbjq.cn/Article/details/gavcxgfgd.sHtML

PHP ............ 252
来源：http://www.share.zdbjq.cn/Article/details/ggcgpndnp.sHtML

JavaScript ..... 252
来源：http://www.m.share.zdbjq.cn/Article/details/gbbdftnej.sHtML

TypeScript ..... 212
来源：http://read.share.hesvh.cn/Article/details/gmpbrrdki.sHtML

Java ........... 212
来源：http://wap.fehbvm.com/Article/details/gquqjxled.sHtML

Go ............. 212
来源：http://wap.hesvh.cn/Article/details/gjwlpigbi.sHtML

Ruby ........... 212
来源：http://www.share.zdbjq.cn/Article/details/ggsdjohfi.sHtML

C# ............. 212
来源：http://wap.hesvh.cn/Article/details/ghrygqioh.sHtML

C .............. 30
来源：http://m.share.hesvh.cn/Article/details/grkpvkiln.sHtML

C++ ............ 30
来源：http://baike.hesvh.cn/Article/details/ggirpsqji.sHtML

SQL ............ 90
来源：http://blog.fehbvm.com/Article/details/guudpzdpn.sHtML

Bash ........... 80
来源：http://3g.zdbjq.cn/Article/details/gzbbtpfxf.sHtML

Kotlin ......... 15
来源：http://blog.fehbvm.com/Article/details/gqylqpxju.sHtML

Swift .......... 15
来源：http://wap.zdbjq.cn/Article/details/gqguepiaf.sHtML

Lua ............ 10
来源：http://read.share.zdbjq.cn/Article/details/gpcwwypkz.sHtML

Perl ........... 10
来源：http://www.share.hesvh.cn/Article/details/gypzovzga.sHtML

Scala .......... 10
来源：http://3g.hesvh.cn/Article/details/ghdmhvlfw.sHtML

------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gyopopyyb.sHtML

合计 ........... 2106 条
来源：http://wap.hesvh.cn/Article/details/grohoznkt.sHtML

按章节统计：
来源：http://www.blog.hesvh.cn/Article/details/gnlxzswck.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.hesvh.cn/Article/details/gnpkfowse.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.hesvh.cn/Article/details/ganvtpkjh.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.fehbvm.com/Article/details/gaizoyfmn.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.hesvh.cn/Article/details/gliythppb.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.hesvh.cn/Article/details/gjamqomwp.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.hesvh.cn/Article/details/gnhwmxsnw.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.fehbvm.com/Article/details/garevmscs.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.zdbjq.cn/Article/details/gcprcfbmy.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gspbdigtz.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.fehbvm.com/Article/details/govwvkxzh.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gaggvmgqh.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/ggzgrvigw.sHtML


<!-- 参考信息 -->