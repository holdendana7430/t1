代发 wailian999

val a = 1;  var b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gvtyddvvt.sHtML

[T53] Scala：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gijluiazk.sHtML

s"值: $b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gcptfxfdn.sHtML

[T54] Scala：集合映射
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvvimzqvr.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsihgfxue.sHtML

[T55] Scala：集合过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gwierqcxc.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gjxfgyfrr.sHtML

[T56] Scala：样例类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gipxcfgux.sHtML

case class User(name: String, age: Int)
来源：http://www.share.fanxiaobao.xyz/Article/details/gerhvhpxn.sHtML

[T57] Scala：模式匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gmubkaxjl.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.fanxiaobao.xyz/Article/details/grhqsizxn.sHtML

[T58] Scala：函数定义
来源：http://www.share.fanxiaobao.xyz/Article/details/ggwjuqlci.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.fanxiaobao.xyz/Article/details/glgaokxrh.sHtML

[T59] Scala：循环
来源：http://baike.fanxiaobao.xyz/Article/details/gmhtjaipl.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.fanxiaobao.xyz/Article/details/goisarfzr.sHtML

[T60] Scala：折叠
来源：http://m.share.fanxiaobao.xyz/Article/details/gbridnpim.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.fanxiaobao.xyz/Article/details/goeirashb.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gphvtkmpt.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gjqrgelhw.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/grunxwwhl.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.fanxiaobao.xyz/Article/details/gzqghfhin.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.fanxiaobao.xyz/Article/details/gtgnhtryn.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzofahtpi.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gucsjisha.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fanxiaobao.xyz/Article/details/gtzkesxjn.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grtsgwsdk.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaabhkgmj.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.fanxiaobao.xyz/Article/details/gajtojdco.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvhrdauxp.sHtML

list(dict.fromkeys(arr))
来源：http://3g.fanxiaobao.xyz/Article/details/gminmhkaq.sHtML

[U06] Py：合并两个字典
来源：http://m.share.fanxiaobao.xyz/Article/details/gehpwosfk.sHtML

{**a, **b}
来源：http://m.share.fanxiaobao.xyz/Article/details/ghfdxajol.sHtML

[U07] Py：反转字典键值
来源：http://3g.fanxiaobao.xyz/Article/details/gihmdptot.sHtML

{v: k for k, v in d.items()}
来源：http://3g.fanxiaobao.xyz/Article/details/gpjihhecs.sHtML

[U08] Py：展平二维列表
来源：http://m.share.fanxiaobao.xyz/Article/details/gxwncyhup.sHtML

[y for x in nested for y in x]
来源：http://blog.fanxiaobao.xyz/Article/details/gpynpgqny.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.fanxiaobao.xyz/Article/details/guklrctpo.sHtML

max(d, key=d.get)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghgowdymn.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpqknotbv.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghonnjioa.sHtML

[U11] Py：生成器表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gedqgqrpa.sHtML

(x * 2 for x in arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gusobttmh.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.fanxiaobao.xyz/Article/details/gfiqshvzj.sHtML

Counter(arr).most_common(3)
来源：http://baike.fanxiaobao.xyz/Article/details/gxgrvdkip.sHtML

[U13] Py：固定长度队列
来源：http://3g.fanxiaobao.xyz/Article/details/gbpwyaktd.sHtML

deque(maxlen=10)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwqlwpuxl.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grokwdptx.sHtML

defaultdict(list)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxbaphkbl.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdotnzzby.sHtML

t = time.perf_counter()
来源：http://blog.fanxiaobao.xyz/Article/details/gvrymewts.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.fanxiaobao.xyz/Article/details/gscyjfrrf.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gufgufvqn.sHtML

[U17] Py：初始化日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gitfdywlq.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.fanxiaobao.xyz/Article/details/ggqehtpfd.sHtML

[U18] Py：预编译正则
来源：http://www.share.fanxiaobao.xyz/Article/details/gbevzstkf.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gagqrbnko.sHtML

[U19] Py：正则替换带回调
来源：http://3g.fanxiaobao.xyz/Article/details/gdpateoru.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gazlhdngv.sHtML

[U20] Py：缓存函数结果
来源：http://3g.fanxiaobao.xyz/Article/details/gybjvewav.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxmnheouo.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnmlaxvwy.sHtML

@contextlib.contextmanager
来源：http://read.share.fanxiaobao.xyz/Article/details/guloysyzj.sHtML

[U22] Py：矩阵转置
来源：http://wap.fanxiaobao.xyz/Article/details/grqdzfuli.sHtML

list(zip(*m))
来源：http://wap.fanxiaobao.xyz/Article/details/glfcswrmw.sHtML

[U23] Py：分块读取大文件
来源：http://3g.fanxiaobao.xyz/Article/details/grppitqdx.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.fanxiaobao.xyz/Article/details/glnppcvyz.sHtML

[U24] Py：路径操作
来源：http://blog.fanxiaobao.xyz/Article/details/gzqphiuqp.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpgjnjokv.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.fanxiaobao.xyz/Article/details/gacawgtqm.sHtML

csv.DictReader(f)
来源：http://mobile.fanxiaobao.xyz/Article/details/gowwhkoca.sHtML

[U26] Py：并发下载
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxmutcmqu.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.fanxiaobao.xyz/Article/details/gdxblppxj.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.fanxiaobao.xyz/Article/details/gzqbjwllx.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.fanxiaobao.xyz/Article/details/gxutawola.sHtML

[U28] Py：类型别名
来源：http://mobile.fanxiaobao.xyz/Article/details/glukoaigt.sHtML

UserId = int
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjcyitkjn.sHtML

[U29] Py：属性校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghhjojzro.sHtML

@property 与 @x.setter 配合
来源：http://wap.fanxiaobao.xyz/Article/details/gxdbafrgw.sHtML

[U30] Py：数据类
来源：http://blog.fanxiaobao.xyz/Article/details/ghfbxjbbq.sHtML

@dataclass(slots=True)
来源：http://wap.fanxiaobao.xyz/Article/details/gkpxxsqje.sHtML

[U31] Py：单测
来源：http://wap.fanxiaobao.xyz/Article/details/ginobaprd.sHtML

python -m pytest -q
来源：http://www.share.fanxiaobao.xyz/Article/details/gecggxrnc.sHtML

[U32] Py：代码格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gxfqlsvoj.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyjwovcns.sHtML

[U33] Py：打包发布
来源：http://wap.fanxiaobao.xyz/Article/details/ghsbalajd.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.fanxiaobao.xyz/Article/details/gdztxsebz.sHtML

[U34] Py：判断编码
来源：http://www.share.fanxiaobao.xyz/Article/details/gmqfacvbl.sHtML

chardet.detect(raw)
来源：http://blog.fanxiaobao.xyz/Article/details/gjzidlhks.sHtML

[U35] Py：发送邮件
来源：http://read.share.fanxiaobao.xyz/Article/details/gycocemql.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkubdwowz.sHtML

[U36] Py：定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/gtocgthst.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.fanxiaobao.xyz/Article/details/gorcvhpmb.sHtML

[U37] Py：读写 Excel
来源：http://mobile.fanxiaobao.xyz/Article/details/gooroouqy.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.fanxiaobao.xyz/Article/details/giawknwgk.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqkppbaxa.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtgyunzmi.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.fanxiaobao.xyz/Article/details/gedhfkgff.sHtML

sys.stdout.isatty()
来源：http://m.share.fanxiaobao.xyz/Article/details/ghdvqqbhb.sHtML

[U40] Py：打印到标准错误
来源：http://3g.fanxiaobao.xyz/Article/details/gyjkchiag.sHtML

print("err", file=sys.stderr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtnbsqppr.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.fanxiaobao.xyz/Article/details/gftcswpkd.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.fanxiaobao.xyz/Article/details/gcskmkcyj.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcylvdnxi.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbuwsuxvx.sHtML

[U43] PHP：声明命名空间
来源：http://wap.fanxiaobao.xyz/Article/details/gmdzhnurt.sHtML

namespace App\Http;
来源：http://wap.fanxiaobao.xyz/Article/details/gipneqtqh.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gosbvqojm.sHtML

declare(strict_types=1);
来源：http://wap.fanxiaobao.xyz/Article/details/gcpgmtflz.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.fanxiaobao.xyz/Article/details/gjkajxvab.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdqncmtep.sHtML

[U46] PHP：可空类型
来源：http://baike.fanxiaobao.xyz/Article/details/gubpfuass.sHtML

?string $name = null
来源：http://wap.fanxiaobao.xyz/Article/details/gofyplhau.sHtML

[U47] PHP：联合类型
来源：http://wap.fanxiaobao.xyz/Article/details/ghvrtlvlg.sHtML

int|string $id
来源：http://m.share.fanxiaobao.xyz/Article/details/gahtqomgy.sHtML

[U48] PHP：纯枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gkyzuwuyr.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcbktlduc.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvujtdjoz.sHtML

public readonly string $name
来源：http://baike.fanxiaobao.xyz/Article/details/glqxwkyof.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.fanxiaobao.xyz/Article/details/glrwiwpau.sHtML

public function __construct(private int $id) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gflshvonf.sHtML

[U51] PHP：数组解构
来源：http://baike.fanxiaobao.xyz/Article/details/gqivhxxbq.sHtML

[$a, $b] = $arr;
来源：http://3g.fanxiaobao.xyz/Article/details/gojcqivik.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gogurkvox.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gashpjxok.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.fanxiaobao.xyz/Article/details/gqqkpnbih.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnagcaxrr.sHtML

[U54] PHP：空安全调用
来源：http://mobile.fanxiaobao.xyz/Article/details/gselzjibx.sHtML

$obj?->method()
来源：http://m.share.fanxiaobao.xyz/Article/details/ggqplarue.sHtML

[U55] PHP：match 表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/giptvmcuk.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.fanxiaobao.xyz/Article/details/glqqhnhwz.sHtML

[U56] PHP：命名参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gqlriktiv.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkqjigrwp.sHtML

[U57] PHP：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gofnppwln.sHtML

"值: {$a}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gonfnjchw.sHtML

[U58] PHP：数组三件套
来源：http://read.share.fanxiaobao.xyz/Article/details/goyeykqtx.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.fanxiaobao.xyz/Article/details/ginjpmegh.sHtML

[U59] PHP：自定义排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gmdorghnz.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fanxiaobao.xyz/Article/details/gevvullsg.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.fanxiaobao.xyz/Article/details/gjgvrqnuv.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghkwsaewp.sHtML

[U61] PHP：正则
来源：http://3g.fanxiaobao.xyz/Article/details/gsdecmaeb.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfyevbzkq.sHtML

[U62] PHP：日期对象
来源：http://m.share.fanxiaobao.xyz/Article/details/grqqbgfaf.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.fanxiaobao.xyz/Article/details/gygslpgll.sHtML

[U63] PHP：文件读写
来源：http://mobile.fanxiaobao.xyz/Article/details/gagqwoeai.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.fanxiaobao.xyz/Article/details/gavwkctjq.sHtML

[U64] PHP：目录遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gwttxsqlz.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.fanxiaobao.xyz/Article/details/giahldrff.sHtML

[U65] PHP：会话
来源：http://www.blog.fanxiaobao.xyz/Article/details/gncmygcyk.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/guadjfpuf.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.fanxiaobao.xyz/Article/details/grbsppfji.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggijswgrz.sHtML

[U67] PHP：处理文件上传
来源：http://blog.fanxiaobao.xyz/Article/details/gfytbuxtj.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gspuwzaba.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gshmyhokn.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.fanxiaobao.xyz/Article/details/gtdnrwwos.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gqjciabye.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbogkurdx.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwlgnvpft.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.fanxiaobao.xyz/Article/details/gemwgfyea.sHtML

[U71] PHP：抛出异常
来源：http://mobile.fanxiaobao.xyz/Article/details/gkhpzcdgh.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.fanxiaobao.xyz/Article/details/gzlnijvyq.sHtML

[U72] PHP：写错误日志
来源：http://wap.fanxiaobao.xyz/Article/details/gxfoxmrth.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.fanxiaobao.xyz/Article/details/gpmumxszm.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.fanxiaobao.xyz/Article/details/grvaibqfo.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkpdfclmp.sHtML

[U74] PHP：读取环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/gedsiojmp.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.fanxiaobao.xyz/Article/details/giwvjrtba.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gutqzgtha.sHtML

composer require psr/container
来源：http://3g.fanxiaobao.xyz/Article/details/gdwfoohhe.sHtML

[U76] PHP：简单路由
来源：http://wap.fanxiaobao.xyz/Article/details/gepbnlbcb.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.fanxiaobao.xyz/Article/details/gglbrmwjm.sHtML

[U77] PHP：模板渲染
来源：http://baike.fanxiaobao.xyz/Article/details/gwlswqpgm.sHtML

composer require twig/twig
来源：http://3g.fanxiaobao.xyz/Article/details/geywnutts.sHtML

[U78] PHP：单元测试
来源：http://blog.fanxiaobao.xyz/Article/details/gxctafzyq.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.fanxiaobao.xyz/Article/details/gzjvopsmu.sHtML

[U79] PHP：静态分析
来源：http://read.share.fanxiaobao.xyz/Article/details/ghxbnwvil.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.fanxiaobao.xyz/Article/details/gdwkdffqj.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.fanxiaobao.xyz/Article/details/gvexaekqb.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.fanxiaobao.xyz/Article/details/givgalrtd.sHtML

[U81] JS：初始化项目
来源：http://baike.fanxiaobao.xyz/Article/details/gvmlvqibj.sHtML

npm init -y;  npm i express
来源：http://www.share.fanxiaobao.xyz/Article/details/gvaiudpku.sHtML

[U82] JS：package.json 脚本
来源：http://3g.fanxiaobao.xyz/Article/details/gofxmzrwj.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxhzmctld.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geiczbuaw.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.fanxiaobao.xyz/Article/details/gjglwlxui.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.fanxiaobao.xyz/Article/details/gdrrnsadl.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.fanxiaobao.xyz/Article/details/goomkyrwt.sHtML

[U85] JS：可选链
来源：http://www.share.fanxiaobao.xyz/Article/details/gmugpukfx.sHtML

a?.b?.c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghejzdnwr.sHtML

[U86] JS：空值合并
来源：http://www.share.fanxiaobao.xyz/Article/details/gxmdiawrm.sHtML

a ?? b
来源：http://read.share.fanxiaobao.xyz/Article/details/grlbeimdj.sHtML

[U87] JS：解构默认值
来源：http://baike.fanxiaobao.xyz/Article/details/guisqxypk.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.fanxiaobao.xyz/Article/details/gpbtzhopp.sHtML

[U88] JS：对象展开合并
来源：http://3g.fanxiaobao.xyz/Article/details/gpdayxdtg.sHtML

{ ...a, ...b }
来源：http://read.share.fanxiaobao.xyz/Article/details/guvlycppc.sHtML

[U89] JS：数组去重
来源：http://m.share.fanxiaobao.xyz/Article/details/gokloisfi.sHtML

[...new Set(arr)]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqwugufds.sHtML

[U90] JS：数字数组排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gcavkdgsr.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.fanxiaobao.xyz/Article/details/gepdxrbug.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grzftfbjx.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.fanxiaobao.xyz/Article/details/gmywwyqwo.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdpegvftk.sHtML

structuredClone(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/gwrhigcqn.sHtML

[U93] JS：模板字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gfadlplgb.sHtML

`共 ${n} 条`
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsrbrcuzv.sHtML

[U94] JS：箭头函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gqgkimdpn.sHtML

const double = x => x * 2;
来源：http://baike.fanxiaobao.xyz/Article/details/gmlcexokx.sHtML

[U95] JS：Promise 包装
来源：http://www.share.fanxiaobao.xyz/Article/details/grtpnxmja.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.fanxiaobao.xyz/Article/details/gwxeuzlaz.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.fanxiaobao.xyz/Article/details/gvbaqikim.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtnkxegfy.sHtML

[U97] JS：并发请求
来源：http://3g.fanxiaobao.xyz/Article/details/gqmpiuczh.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fanxiaobao.xyz/Article/details/gjhzixxcr.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.fanxiaobao.xyz/Article/details/goawakwrb.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.fanxiaobao.xyz/Article/details/gfqowxrmd.sHtML

[U99] JS：事件监听
来源：http://blog.fanxiaobao.xyz/Article/details/giahooxvq.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.fanxiaobao.xyz/Article/details/goqqtqcbc.sHtML

[U100] JS：DOM 查询
来源：http://baike.fanxiaobao.xyz/Article/details/gutfcnlmo.sHtML

document.querySelector(".item")
来源：http://mobile.fanxiaobao.xyz/Article/details/ghfaltbga.sHtML

[U101] JS：classList 操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gffqremav.sHtML

el.classList.toggle("active")
来源：http://wap.fanxiaobao.xyz/Article/details/gfzzvagcu.sHtML

[U102] JS：本地存储
来源：http://www.share.fanxiaobao.xyz/Article/details/gbccpblxz.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.fanxiaobao.xyz/Article/details/gpttpjpmr.sHtML

[U103] JS：定时器
来源：http://read.share.fanxiaobao.xyz/Article/details/gupanqyzw.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.fanxiaobao.xyz/Article/details/grybggwwx.sHtML

[U104] JS：防抖
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpbzipzjk.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzvvmhwip.sHtML

[U105] JS：节流
来源：http://mobile.fanxiaobao.xyz/Article/details/gygzbghwu.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gpctwpjhg.sHtML

[U106] JS：日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gtbryfsop.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.fanxiaobao.xyz/Article/details/gwuihccjo.sHtML

[U107] JS：数字千分位
来源：http://baike.fanxiaobao.xyz/Article/details/gnlxrbhsk.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.fanxiaobao.xyz/Article/details/glzvrfnsx.sHtML

[U108] JS：随机整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsoikhzuh.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.fanxiaobao.xyz/Article/details/gzmybyeku.sHtML

[U109] JS：数组分组
来源：http://3g.fanxiaobao.xyz/Article/details/gbycjeojn.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkdkkrjkr.sHtML

[U110] JS：数组分块
来源：http://baike.fanxiaobao.xyz/Article/details/guhnemkdg.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.fanxiaobao.xyz/Article/details/gvonovclr.sHtML

[U111] JS：对象转 Map
来源：http://mobile.fanxiaobao.xyz/Article/details/gxacqpytv.sHtML

new Map(Object.entries(obj))
来源：http://m.share.fanxiaobao.xyz/Article/details/gajlaoocn.sHtML

[U112] JS：字符串补位
来源：http://m.share.fanxiaobao.xyz/Article/details/gdockywpn.sHtML

"7".padStart(3, "0")
来源：http://blog.fanxiaobao.xyz/Article/details/gmobtypxb.sHtML

[U113] JS：正则替换全部
来源：http://mobile.fanxiaobao.xyz/Article/details/gjbktpcea.sHtML

s.replaceAll("a", "b")
来源：http://baike.fanxiaobao.xyz/Article/details/gahoiwexw.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gkbhhvean.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fanxiaobao.xyz/Article/details/gaqmxvugu.sHtML

[U115] JS：生成 UUID
来源：http://baike.fanxiaobao.xyz/Article/details/gtfhrigrz.sHtML

crypto.randomUUID()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsqglpstd.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.fanxiaobao.xyz/Article/details/ghschdtdc.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkxqkhnnv.sHtML

[U117] JS：单元测试
来源：http://3g.fanxiaobao.xyz/Article/details/gstpnvwmg.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsfxfexdb.sHtML

[U118] JS：开发服务器
来源：http://www.share.fanxiaobao.xyz/Article/details/grcoabeuo.sHtML

npm i -D vite;  npx vite
来源：http://3g.fanxiaobao.xyz/Article/details/ggxwjdiig.sHtML

[U119] JS：生产构建
来源：http://www.blog.fanxiaobao.xyz/Article/details/gomkvjmoj.sHtML

npx vite build
来源：http://mobile.fanxiaobao.xyz/Article/details/gbbbrxatz.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.fanxiaobao.xyz/Article/details/gzdcocmwv.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.fanxiaobao.xyz/Article/details/gfwxhlvaq.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gqxruscas.sHtML

统计汇总
来源：http://wap.fanxiaobao.xyz/Article/details/gyrpyoana.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gnkkjyuyu.sHtML

按语言统计（条）：
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gebqgtrro.sHtML

Python ......... 252
来源：http://wap.fanxiaobao.xyz/Article/details/gohgqhkij.sHtML

PHP ............ 252
来源：http://blog.fanxiaobao.xyz/Article/details/gnyfxbvpf.sHtML

JavaScript ..... 252
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfofxrbjb.sHtML

TypeScript ..... 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwwsirwwf.sHtML

Java ........... 212
来源：http://3g.fanxiaobao.xyz/Article/details/gfwymixil.sHtML

Go ............. 212
来源：http://baike.fanxiaobao.xyz/Article/details/gpgwprozd.sHtML

Ruby ........... 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gopbuzyzf.sHtML

C# ............. 212
来源：http://wap.fanxiaobao.xyz/Article/details/gtsanfick.sHtML

C .............. 30
来源：http://www.share.fanxiaobao.xyz/Article/details/gncwnvakj.sHtML

C++ ............ 30
来源：http://wap.fanxiaobao.xyz/Article/details/gbjpmuexp.sHtML

SQL ............ 90
来源：http://3g.fanxiaobao.xyz/Article/details/gfgjgftcj.sHtML

Bash ........... 80
来源：http://blog.fanxiaobao.xyz/Article/details/gqjyuqjwq.sHtML

Kotlin ......... 15
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjsndcunr.sHtML

Swift .......... 15
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwzokbqbc.sHtML

Lua ............ 10
来源：http://m.share.fanxiaobao.xyz/Article/details/gxhbwyuax.sHtML

Perl ........... 10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjoldswkx.sHtML

Scala .......... 10
来源：http://wap.fanxiaobao.xyz/Article/details/gihcpudcf.sHtML

------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/glpwmkvel.sHtML

合计 ........... 2106 条
来源：http://baike.fanxiaobao.xyz/Article/details/glrfkxfxw.sHtML

按章节统计：
来源：http://blog.fanxiaobao.xyz/Article/details/ggoltfgcj.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.fanxiaobao.xyz/Article/details/gofkrvvgn.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggixosrey.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.fanxiaobao.xyz/Article/details/gqmorqkmq.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.fanxiaobao.xyz/Article/details/ggmdxnzpu.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.fanxiaobao.xyz/Article/details/gqsxzdrbq.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.fanxiaobao.xyz/Article/details/gzfpjjxoz.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.fanxiaobao.xyz/Article/details/gbqpwqjcl.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.fanxiaobao.xyz/Article/details/gtapefvsq.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/gedqvnyps.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.fanxiaobao.xyz/Article/details/ghfemdaqi.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gvvsikvlw.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gcxndgozq.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/geboolaoz.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.fanxiaobao.xyz/Article/details/gizwledwe.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.fanxiaobao.xyz/Article/details/gpdwappug.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/ggzijzjab.sHtML


<!-- 参考信息 -->