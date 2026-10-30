代发 wailian999

case class User(name: String, age: Int)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmqilzrqy.sHtML

[T57] Scala：模式匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gvukixxea.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwrxaxacg.sHtML

[T58] Scala：函数定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gklrgqsvc.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.fanxiaobao.xyz/Article/details/guxvovgag.sHtML

[T59] Scala：循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gdnomjadj.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwdivtonp.sHtML

[T60] Scala：折叠
来源：http://read.share.fanxiaobao.xyz/Article/details/gcdogjuvf.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.fanxiaobao.xyz/Article/details/gytcitutv.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gpztlpowq.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghujflecw.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gvzjhjiik.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.fanxiaobao.xyz/Article/details/gcaezsykl.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkqrafmlz.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.fanxiaobao.xyz/Article/details/gicgcddrk.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggmojsyyp.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.fanxiaobao.xyz/Article/details/ggthoxpko.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.fanxiaobao.xyz/Article/details/gsvukcxlj.sHtML

[U04] Py：变量调试打印
来源：http://blog.fanxiaobao.xyz/Article/details/gfrursdun.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.fanxiaobao.xyz/Article/details/guwwbfsqo.sHtML

[U05] Py：列表去重且保序
来源：http://wap.fanxiaobao.xyz/Article/details/gbppzakzw.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.fanxiaobao.xyz/Article/details/gldqdjqrn.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gcqtpkhvs.sHtML

{**a, **b}
来源：http://3g.fanxiaobao.xyz/Article/details/ggqkiszra.sHtML

[U07] Py：反转字典键值
来源：http://m.share.fanxiaobao.xyz/Article/details/gapqsdvtt.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.fanxiaobao.xyz/Article/details/gbxnyzpez.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtswbjxly.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvevnjbfe.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.fanxiaobao.xyz/Article/details/gsjnpiopk.sHtML

max(d, key=d.get)
来源：http://wap.fanxiaobao.xyz/Article/details/groliiyiq.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtjlaforu.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.fanxiaobao.xyz/Article/details/gxrkzzxib.sHtML

[U11] Py：生成器表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gcptoftcm.sHtML

(x * 2 for x in arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gbtiyvoyw.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.fanxiaobao.xyz/Article/details/gcprhzpyk.sHtML

Counter(arr).most_common(3)
来源：http://wap.fanxiaobao.xyz/Article/details/gebvwdrkd.sHtML

[U13] Py：固定长度队列
来源：http://www.share.fanxiaobao.xyz/Article/details/gsdlhzado.sHtML

deque(maxlen=10)
来源：http://wap.fanxiaobao.xyz/Article/details/grbsxdxod.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmchraqgw.sHtML

defaultdict(list)
来源：http://baike.fanxiaobao.xyz/Article/details/gkwppbcir.sHtML

[U15] Py：高精度计时
来源：http://blog.fanxiaobao.xyz/Article/details/grhvhfnxx.sHtML

t = time.perf_counter()
来源：http://www.share.fanxiaobao.xyz/Article/details/gafnehamy.sHtML

[U16] Py：命令行参数解析
来源：http://blog.fanxiaobao.xyz/Article/details/gglgvyqzf.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhbjrkcd.sHtML

[U17] Py：初始化日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gwzlixbbd.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtfxwwxwr.sHtML

[U18] Py：预编译正则
来源：http://mobile.fanxiaobao.xyz/Article/details/gzmmibpvc.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.fanxiaobao.xyz/Article/details/gjnmuwgby.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.fanxiaobao.xyz/Article/details/gtgncjlgk.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.fanxiaobao.xyz/Article/details/gzjjeodgj.sHtML

[U20] Py：缓存函数结果
来源：http://wap.fanxiaobao.xyz/Article/details/gjypcwnuu.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpbsoaejo.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.fanxiaobao.xyz/Article/details/giwblnmuf.sHtML

@contextlib.contextmanager
来源：http://3g.fanxiaobao.xyz/Article/details/ggjmptzgw.sHtML

[U22] Py：矩阵转置
来源：http://mobile.fanxiaobao.xyz/Article/details/goehanvur.sHtML

list(zip(*m))
来源：http://read.share.fanxiaobao.xyz/Article/details/gkbefxinq.sHtML

[U23] Py：分块读取大文件
来源：http://blog.fanxiaobao.xyz/Article/details/gzuvnaboq.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.fanxiaobao.xyz/Article/details/guzfdhunt.sHtML

[U24] Py：路径操作
来源：http://3g.fanxiaobao.xyz/Article/details/gagylacdy.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbbjajfih.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmeliuemy.sHtML

csv.DictReader(f)
来源：http://3g.fanxiaobao.xyz/Article/details/gdserbkxg.sHtML

[U26] Py：并发下载
来源：http://m.share.fanxiaobao.xyz/Article/details/gfrvdkkyd.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmlovpira.sHtML

[U27] Py：异步 HTTP
来源：http://wap.fanxiaobao.xyz/Article/details/gdijvarph.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.fanxiaobao.xyz/Article/details/gewvipowm.sHtML

[U28] Py：类型别名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdzndszrk.sHtML

UserId = int
来源：http://wap.fanxiaobao.xyz/Article/details/gybbdjymz.sHtML

[U29] Py：属性校验
来源：http://baike.fanxiaobao.xyz/Article/details/gjdnsccex.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwpjkqhha.sHtML

[U30] Py：数据类
来源：http://mobile.fanxiaobao.xyz/Article/details/ghvjakzvv.sHtML

@dataclass(slots=True)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtqwcydwt.sHtML

[U31] Py：单测
来源：http://www.blog.fanxiaobao.xyz/Article/details/gloxisncm.sHtML

python -m pytest -q
来源：http://3g.fanxiaobao.xyz/Article/details/gxdkksvlm.sHtML

[U32] Py：代码格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gyemuibvx.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.fanxiaobao.xyz/Article/details/gzrsxymne.sHtML

[U33] Py：打包发布
来源：http://wap.fanxiaobao.xyz/Article/details/gcmpdnvqc.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.fanxiaobao.xyz/Article/details/gltmyqots.sHtML

[U34] Py：判断编码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfaowvumr.sHtML

chardet.detect(raw)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdtvuulrb.sHtML

[U35] Py：发送邮件
来源：http://www.share.fanxiaobao.xyz/Article/details/gjwrozdcu.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggfuznadk.sHtML

[U36] Py：定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/gxidfzeig.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.fanxiaobao.xyz/Article/details/getwrdwfr.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkwjvrtxa.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.fanxiaobao.xyz/Article/details/ghyankfom.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.fanxiaobao.xyz/Article/details/glxguhowk.sHtML

Path(__file__).resolve().parent
来源：http://blog.fanxiaobao.xyz/Article/details/goloiqwdm.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.fanxiaobao.xyz/Article/details/gpcwrrlsv.sHtML

sys.stdout.isatty()
来源：http://blog.fanxiaobao.xyz/Article/details/gcsqyhhsz.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gjqapsrqq.sHtML

print("err", file=sys.stderr)
来源：http://baike.fanxiaobao.xyz/Article/details/gltvillwb.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.fanxiaobao.xyz/Article/details/gryhozaau.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.fanxiaobao.xyz/Article/details/gciiszijn.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqtusuytu.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gukgrhttf.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtrwwezuz.sHtML

namespace App\Http;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxjebxukc.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gzbqxjwzb.sHtML

declare(strict_types=1);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmbnfwiuo.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.fanxiaobao.xyz/Article/details/grqutcogu.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpghfnhzb.sHtML

[U46] PHP：可空类型
来源：http://blog.fanxiaobao.xyz/Article/details/gzhrpbbge.sHtML

?string $name = null
来源：http://wap.fanxiaobao.xyz/Article/details/gfpodchhe.sHtML

[U47] PHP：联合类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gpmsrzbsy.sHtML

int|string $id
来源：http://read.share.fanxiaobao.xyz/Article/details/gcanpmqga.sHtML

[U48] PHP：纯枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gvldrucru.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gebkwjswh.sHtML

[U49] PHP：只读属性
来源：http://read.share.fanxiaobao.xyz/Article/details/gkwgfysmm.sHtML

public readonly string $name
来源：http://blog.fanxiaobao.xyz/Article/details/gesydylfy.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.fanxiaobao.xyz/Article/details/gekkgghoo.sHtML

public function __construct(private int $id) {}
来源：http://baike.fanxiaobao.xyz/Article/details/ghfostexe.sHtML

[U51] PHP：数组解构
来源：http://blog.fanxiaobao.xyz/Article/details/grkyycrky.sHtML

[$a, $b] = $arr;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnaovoojt.sHtML

[U52] PHP：箭头函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gnasbdywf.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gychyxwcj.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.fanxiaobao.xyz/Article/details/gwnufaqlj.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.fanxiaobao.xyz/Article/details/gniqkgykg.sHtML

[U54] PHP：空安全调用
来源：http://wap.fanxiaobao.xyz/Article/details/gdnkqztwy.sHtML

$obj?->method()
来源：http://blog.fanxiaobao.xyz/Article/details/gcvtsjbom.sHtML

[U55] PHP：match 表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gcrnvwxds.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.fanxiaobao.xyz/Article/details/ggstyygnn.sHtML

[U56] PHP：命名参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gcoxqpney.sHtML

f(a: 1, b: 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkzoekncs.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggobqjayg.sHtML

"值: {$a}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gmiqdhavz.sHtML

[U58] PHP：数组三件套
来源：http://3g.fanxiaobao.xyz/Article/details/glenyzlxa.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.fanxiaobao.xyz/Article/details/gxzqopxap.sHtML

[U59] PHP：自定义排序
来源：http://wap.fanxiaobao.xyz/Article/details/gzfcbqlaw.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fanxiaobao.xyz/Article/details/gpdzlzxrb.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.fanxiaobao.xyz/Article/details/gjytbxbrs.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.fanxiaobao.xyz/Article/details/gxykejvpr.sHtML

[U61] PHP：正则
来源：http://www.share.fanxiaobao.xyz/Article/details/gmzwmzzbf.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkyajccim.sHtML

[U62] PHP：日期对象
来源：http://blog.fanxiaobao.xyz/Article/details/gseghgeeq.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfmvmcjip.sHtML

[U63] PHP：文件读写
来源：http://m.share.fanxiaobao.xyz/Article/details/gbupgforh.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gshpedlad.sHtML

[U64] PHP：目录遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gadsoypku.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwqantwea.sHtML

[U65] PHP：会话
来源：http://mobile.fanxiaobao.xyz/Article/details/gttgltvvb.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gshwjmgel.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.fanxiaobao.xyz/Article/details/ghznndrzc.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqqfnkaui.sHtML

[U67] PHP：处理文件上传
来源：http://baike.fanxiaobao.xyz/Article/details/glzzfunbd.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gptfctnkc.sHtML

[U68] PHP：PDO 连接
来源：http://3g.fanxiaobao.xyz/Article/details/gjxnwgmxg.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjcaormbu.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gnjwgtrsb.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.fanxiaobao.xyz/Article/details/gxdxwojph.sHtML

[U70] PHP：PDO 事务
来源：http://blog.fanxiaobao.xyz/Article/details/gpnkibuet.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.fanxiaobao.xyz/Article/details/gczlbybwf.sHtML

[U71] PHP：抛出异常
来源：http://baike.fanxiaobao.xyz/Article/details/gmpxvfvui.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.fanxiaobao.xyz/Article/details/govxegbfd.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbeilzvcb.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.fanxiaobao.xyz/Article/details/gfbwtuque.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.fanxiaobao.xyz/Article/details/gmgezgdoj.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.fanxiaobao.xyz/Article/details/gnhxtropa.sHtML

[U74] PHP：读取环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/gxuzagtox.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqpvhsupk.sHtML

[U75] PHP：依赖注入
来源：http://www.share.fanxiaobao.xyz/Article/details/gxyuznyty.sHtML

composer require psr/container
来源：http://m.share.fanxiaobao.xyz/Article/details/gidnsozrf.sHtML

[U76] PHP：简单路由
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzupuokb.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.fanxiaobao.xyz/Article/details/ghqjkylub.sHtML

[U77] PHP：模板渲染
来源：http://m.share.fanxiaobao.xyz/Article/details/gvkmkivac.sHtML

composer require twig/twig
来源：http://m.share.fanxiaobao.xyz/Article/details/gtgszcrnb.sHtML

[U78] PHP：单元测试
来源：http://blog.fanxiaobao.xyz/Article/details/gkijcmnrw.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.fanxiaobao.xyz/Article/details/gczdkrtyo.sHtML

[U79] PHP：静态分析
来源：http://m.share.fanxiaobao.xyz/Article/details/gvirgaeqk.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.fanxiaobao.xyz/Article/details/geoyacopg.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.fanxiaobao.xyz/Article/details/ghhwgkfsy.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.fanxiaobao.xyz/Article/details/gdczqcnwl.sHtML

[U81] JS：初始化项目
来源：http://blog.fanxiaobao.xyz/Article/details/glpmfozlt.sHtML

npm init -y;  npm i express
来源：http://blog.fanxiaobao.xyz/Article/details/gougwcwvn.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpkyomgdk.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gethkjjbr.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.fanxiaobao.xyz/Article/details/gdhtbhbjx.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.fanxiaobao.xyz/Article/details/gjwenanps.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.fanxiaobao.xyz/Article/details/gusvjduge.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.fanxiaobao.xyz/Article/details/grunwajse.sHtML

[U85] JS：可选链
来源：http://mobile.fanxiaobao.xyz/Article/details/gqmpazzym.sHtML

a?.b?.c
来源：http://wap.fanxiaobao.xyz/Article/details/gyqeyyfbl.sHtML

[U86] JS：空值合并
来源：http://m.share.fanxiaobao.xyz/Article/details/goxciskbh.sHtML

a ?? b
来源：http://m.share.fanxiaobao.xyz/Article/details/gjzqycrez.sHtML

[U87] JS：解构默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/gpdcnshlk.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.fanxiaobao.xyz/Article/details/gbhtyafxj.sHtML

[U88] JS：对象展开合并
来源：http://read.share.fanxiaobao.xyz/Article/details/gtmdwmlwz.sHtML

{ ...a, ...b }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbddguugu.sHtML

[U89] JS：数组去重
来源：http://read.share.fanxiaobao.xyz/Article/details/gotnzsdyc.sHtML

[...new Set(arr)]
来源：http://blog.fanxiaobao.xyz/Article/details/gqerfxqox.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcykwksfk.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.fanxiaobao.xyz/Article/details/guffcaxak.sHtML

[U91] JS：对象键值遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gbyykrygg.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxydlcrlw.sHtML

[U92] JS：深拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gmxeosacw.sHtML

structuredClone(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/grpilgpxy.sHtML

[U93] JS：模板字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gedhvaalf.sHtML

`共 ${n} 条`
来源：http://www.blog.fanxiaobao.xyz/Article/details/gubvpjdtu.sHtML

[U94] JS：箭头函数
来源：http://mobile.fanxiaobao.xyz/Article/details/ggfyxnbqk.sHtML

const double = x => x * 2;
来源：http://blog.fanxiaobao.xyz/Article/details/gmfiicgra.sHtML

[U95] JS：Promise 包装
来源：http://3g.fanxiaobao.xyz/Article/details/gklrqykah.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxygwekgg.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.fanxiaobao.xyz/Article/details/gjdqkojdk.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.fanxiaobao.xyz/Article/details/gqhnnxfbu.sHtML

[U97] JS：并发请求
来源：http://read.share.fanxiaobao.xyz/Article/details/gugmnxhsf.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fanxiaobao.xyz/Article/details/gzkigzjih.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gyyntlqdg.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.fanxiaobao.xyz/Article/details/gwnvlwguv.sHtML

[U99] JS：事件监听
来源：http://3g.fanxiaobao.xyz/Article/details/gqojighni.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.fanxiaobao.xyz/Article/details/guwethbmb.sHtML

[U100] JS：DOM 查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gwjnztmcn.sHtML

document.querySelector(".item")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfwawytah.sHtML

[U101] JS：classList 操作
来源：http://3g.fanxiaobao.xyz/Article/details/gvivbdwza.sHtML

el.classList.toggle("active")
来源：http://wap.fanxiaobao.xyz/Article/details/glcbferdx.sHtML

[U102] JS：本地存储
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gchedtuhg.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.fanxiaobao.xyz/Article/details/gjnbeypzz.sHtML

[U103] JS：定时器
来源：http://www.share.fanxiaobao.xyz/Article/details/gvdypzakp.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpuzgifby.sHtML

[U104] JS：防抖
来源：http://www.share.fanxiaobao.xyz/Article/details/ggnulbxyx.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fanxiaobao.xyz/Article/details/gqznffejw.sHtML

[U105] JS：节流
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxuinlvvf.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gqbcuskly.sHtML

[U106] JS：日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gjkcaetgr.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.fanxiaobao.xyz/Article/details/gblxnepcw.sHtML

[U107] JS：数字千分位
来源：http://baike.fanxiaobao.xyz/Article/details/gylhdujsa.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.fanxiaobao.xyz/Article/details/grkkvwvwl.sHtML

[U108] JS：随机整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfghabjyh.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.fanxiaobao.xyz/Article/details/gryvippgd.sHtML

[U109] JS：数组分组
来源：http://read.share.fanxiaobao.xyz/Article/details/gzxljscgm.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghtxarbli.sHtML

[U110] JS：数组分块
来源：http://mobile.fanxiaobao.xyz/Article/details/glwkbxjet.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.fanxiaobao.xyz/Article/details/gzkwifrmk.sHtML

[U111] JS：对象转 Map
来源：http://blog.fanxiaobao.xyz/Article/details/gslsojlbw.sHtML

new Map(Object.entries(obj))
来源：http://mobile.fanxiaobao.xyz/Article/details/gflkinsbo.sHtML

[U112] JS：字符串补位
来源：http://www.share.fanxiaobao.xyz/Article/details/gnxivifwj.sHtML

"7".padStart(3, "0")
来源：http://baike.fanxiaobao.xyz/Article/details/gjeaqcncd.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnagfdlqv.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmysbjmzd.sHtML

[U114] JS：JSON 深比较
来源：http://3g.fanxiaobao.xyz/Article/details/gbrsbnasq.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fanxiaobao.xyz/Article/details/guichcqyi.sHtML

[U115] JS：生成 UUID
来源：http://baike.fanxiaobao.xyz/Article/details/grvfqkcws.sHtML

crypto.randomUUID()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjsaqzelk.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.fanxiaobao.xyz/Article/details/gzbzmamzu.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gniwizsha.sHtML

[U117] JS：单元测试
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnowhyxgs.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.fanxiaobao.xyz/Article/details/gdjgddokh.sHtML

[U118] JS：开发服务器
来源：http://m.share.fanxiaobao.xyz/Article/details/gqxhwvxna.sHtML

npm i -D vite;  npx vite
来源：http://www.share.fanxiaobao.xyz/Article/details/gvnmyrjnn.sHtML

[U119] JS：生产构建
来源：http://m.share.fanxiaobao.xyz/Article/details/ggypdpltj.sHtML

npx vite build
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfyesaufu.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.fanxiaobao.xyz/Article/details/ggbhsyfbr.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.fanxiaobao.xyz/Article/details/ghrhpyihk.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtfnaxxhr.sHtML

统计汇总
来源：http://blog.fanxiaobao.xyz/Article/details/gthpxoren.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gywtkmphr.sHtML

按语言统计（条）：
来源：http://wap.fanxiaobao.xyz/Article/details/gdeecynfq.sHtML

Python ......... 252
来源：http://m.share.fanxiaobao.xyz/Article/details/gpkdhgcib.sHtML

PHP ............ 252
来源：http://www.blog.fanxiaobao.xyz/Article/details/gepweryfe.sHtML

JavaScript ..... 252
来源：http://3g.fanxiaobao.xyz/Article/details/gfafmoaox.sHtML

TypeScript ..... 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gmrmwhwnf.sHtML

Java ........... 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfxvsaupa.sHtML

Go ............. 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gifiqajod.sHtML

Ruby ........... 212
来源：http://www.share.fanxiaobao.xyz/Article/details/grgpfsvks.sHtML

C# ............. 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxmqyrfw.sHtML

C .............. 30
来源：http://www.blog.fanxiaobao.xyz/Article/details/guzaszytm.sHtML

C++ ............ 30
来源：http://blog.fanxiaobao.xyz/Article/details/gpwqlqekr.sHtML

SQL ............ 90
来源：http://m.share.fanxiaobao.xyz/Article/details/ghfacdwcm.sHtML

Bash ........... 80
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtwxjscdd.sHtML

Kotlin ......... 15
来源：http://mobile.fanxiaobao.xyz/Article/details/ghtvkypty.sHtML

Swift .......... 15
来源：http://3g.fanxiaobao.xyz/Article/details/gtfeoypxv.sHtML

Lua ............ 10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzmoatuiz.sHtML

Perl ........... 10
来源：http://www.share.fanxiaobao.xyz/Article/details/gcmiklvci.sHtML

Scala .......... 10
来源：http://baike.fanxiaobao.xyz/Article/details/glhbxzelu.sHtML

------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/grmeigirb.sHtML

合计 ........... 2106 条
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdmndngsr.sHtML

按章节统计：
来源：http://m.share.fanxiaobao.xyz/Article/details/gelmggtcg.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.fanxiaobao.xyz/Article/details/gqpwrglhg.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.fanxiaobao.xyz/Article/details/gruzzcbja.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghetcaolp.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.fanxiaobao.xyz/Article/details/gxblpcwih.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.fanxiaobao.xyz/Article/details/gjmrcqgbq.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.fanxiaobao.xyz/Article/details/gxhojldrg.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.fanxiaobao.xyz/Article/details/gfbuhnbhz.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.fanxiaobao.xyz/Article/details/gkgdqlinf.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/gnzixkmko.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.fanxiaobao.xyz/Article/details/getbqsaok.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/gqghktakb.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/gmshtixuh.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/gcuqrdfda.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.fanxiaobao.xyz/Article/details/govsasubs.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.fanxiaobao.xyz/Article/details/guoxcwijs.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/glfdmdowf.sHtML

Q SQL 专题                              90
来源：http://www.share.fanxiaobao.xyz/Article/details/gwqqmvrpw.sHtML

R Bash 专题                             80
来源：http://3g.fanxiaobao.xyz/Article/details/gkyquxhne.sHtML

S C / C++ 专题                          60
来源：http://m.share.fanxiaobao.xyz/Article/details/gygythmxm.sHtML

T 其他语言补充                          60
来源：http://www.share.fanxiaobao.xyz/Article/details/gprtpzcvt.sHtML

U 高频实用片段                         120
来源：http://blog.fanxiaobao.xyz/Article/details/gskjkaxwm.sHtML

------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/gkfhdalni.sHtML

合计                                  2106 条
来源：http://mobile.fanxiaobao.xyz/Article/details/gbjtobcld.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/gwgkxyafu.sHtML


<!-- 参考信息 -->