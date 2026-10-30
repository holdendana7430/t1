代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcjcyfwyk.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqdlapzri.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gksrihpke.sHtML

[T56] Scala：样例类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjcdkobg.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtkqdelwv.sHtML

[T57] Scala：模式匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gjrntxbeh.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.fanxiaobao.xyz/Article/details/giteazlsm.sHtML

[T58] Scala：函数定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gkgejbdzg.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.fanxiaobao.xyz/Article/details/gjamqbyyp.sHtML

[T59] Scala：循环
来源：http://blog.fanxiaobao.xyz/Article/details/gaqehvgkw.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/groewulmi.sHtML

[T60] Scala：折叠
来源：http://baike.fanxiaobao.xyz/Article/details/giruiegmh.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.fanxiaobao.xyz/Article/details/gasonwhhe.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/ggoljxbwy.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gpcfztohs.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/guvovongt.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.fanxiaobao.xyz/Article/details/gjtlwlwvs.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.fanxiaobao.xyz/Article/details/gymzffrsl.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.fanxiaobao.xyz/Article/details/gyiautyya.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gcbpwadsl.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.fanxiaobao.xyz/Article/details/gznvyqqka.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.fanxiaobao.xyz/Article/details/gnwzuwqym.sHtML

[U04] Py：变量调试打印
来源：http://m.share.fanxiaobao.xyz/Article/details/gomaozkwa.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.fanxiaobao.xyz/Article/details/glzaxnnrn.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.fanxiaobao.xyz/Article/details/gavqcsnmd.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvxkeqlw.sHtML

[U06] Py：合并两个字典
来源：http://baike.fanxiaobao.xyz/Article/details/gtzrsmirw.sHtML

{**a, **b}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gotdklwue.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goguuntgo.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fanxiaobao.xyz/Article/details/gvtafsbbn.sHtML

[U08] Py：展平二维列表
来源：http://mobile.fanxiaobao.xyz/Article/details/gnvmsmnla.sHtML

[y for x in nested for y in x]
来源：http://m.share.fanxiaobao.xyz/Article/details/gbguohogk.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.fanxiaobao.xyz/Article/details/goyifkudc.sHtML

max(d, key=d.get)
来源：http://wap.fanxiaobao.xyz/Article/details/ggqakpzsg.sHtML

[U10] Py：按值排序字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gojbhagiu.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvuhbfxil.sHtML

[U11] Py：生成器表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gsrrtjlto.sHtML

(x * 2 for x in arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfrvzmskh.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gnknkgect.sHtML

Counter(arr).most_common(3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gztoipicz.sHtML

[U13] Py：固定长度队列
来源：http://read.share.fanxiaobao.xyz/Article/details/gevapatqu.sHtML

deque(maxlen=10)
来源：http://baike.fanxiaobao.xyz/Article/details/gmzuhnysj.sHtML

[U14] Py：分组收集到列表
来源：http://baike.fanxiaobao.xyz/Article/details/gtujjpyld.sHtML

defaultdict(list)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvlignpjc.sHtML

[U15] Py：高精度计时
来源：http://m.share.fanxiaobao.xyz/Article/details/gmylltgcs.sHtML

t = time.perf_counter()
来源：http://mobile.fanxiaobao.xyz/Article/details/grlmfsztk.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fanxiaobao.xyz/Article/details/gguddoxbw.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.fanxiaobao.xyz/Article/details/gqdgkubws.sHtML

[U17] Py：初始化日志
来源：http://mobile.fanxiaobao.xyz/Article/details/galvhrzjo.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmhuhqdvv.sHtML

[U18] Py：预编译正则
来源：http://read.share.fanxiaobao.xyz/Article/details/gjvndgrfv.sHtML

pat = re.compile(r"\d+")
来源：http://wap.fanxiaobao.xyz/Article/details/gmtfcgazl.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.fanxiaobao.xyz/Article/details/glyvmgjil.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.fanxiaobao.xyz/Article/details/gyhdhdvxp.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.fanxiaobao.xyz/Article/details/gpkyedvwn.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.fanxiaobao.xyz/Article/details/gnnhotxzq.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.fanxiaobao.xyz/Article/details/gkvostxcq.sHtML

@contextlib.contextmanager
来源：http://mobile.fanxiaobao.xyz/Article/details/giufljqqn.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gngkyauvv.sHtML

list(zip(*m))
来源：http://read.share.fanxiaobao.xyz/Article/details/gurpyspvn.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gvuffcjyd.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.fanxiaobao.xyz/Article/details/gxgthrpds.sHtML

[U24] Py：路径操作
来源：http://baike.fanxiaobao.xyz/Article/details/gncsjnrrg.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzjdooaew.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.fanxiaobao.xyz/Article/details/gfizlnebp.sHtML

csv.DictReader(f)
来源：http://blog.fanxiaobao.xyz/Article/details/gmvapynvm.sHtML

[U26] Py：并发下载
来源：http://www.blog.fanxiaobao.xyz/Article/details/gttsjosjs.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.fanxiaobao.xyz/Article/details/gknkqpmpc.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.fanxiaobao.xyz/Article/details/gtfsfpgvm.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzffvmlnr.sHtML

[U28] Py：类型别名
来源：http://baike.fanxiaobao.xyz/Article/details/gsygxglll.sHtML

UserId = int
来源：http://baike.fanxiaobao.xyz/Article/details/gmekuzedo.sHtML

[U29] Py：属性校验
来源：http://3g.fanxiaobao.xyz/Article/details/gecflmmyf.sHtML

@property 与 @x.setter 配合
来源：http://mobile.fanxiaobao.xyz/Article/details/giygxadai.sHtML

[U30] Py：数据类
来源：http://baike.fanxiaobao.xyz/Article/details/gkkcpdcon.sHtML

@dataclass(slots=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/gejvkozyk.sHtML

[U31] Py：单测
来源：http://mobile.fanxiaobao.xyz/Article/details/gpssmkvch.sHtML

python -m pytest -q
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjgdcbggv.sHtML

[U32] Py：代码格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gfbfwbvdw.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnmnwqjsh.sHtML

[U33] Py：打包发布
来源：http://read.share.fanxiaobao.xyz/Article/details/gvvrycbkh.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.fanxiaobao.xyz/Article/details/gkktydndn.sHtML

[U34] Py：判断编码
来源：http://3g.fanxiaobao.xyz/Article/details/gnnnxahar.sHtML

chardet.detect(raw)
来源：http://mobile.fanxiaobao.xyz/Article/details/grhxwaooz.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfcanotta.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.fanxiaobao.xyz/Article/details/gjybgnnge.sHtML

[U36] Py：定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gznxsxlnd.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.fanxiaobao.xyz/Article/details/giolsikvg.sHtML

[U37] Py：读写 Excel
来源：http://www.share.fanxiaobao.xyz/Article/details/gnjnftzbw.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.fanxiaobao.xyz/Article/details/gubbxqnzw.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzxrtbhhc.sHtML

Path(__file__).resolve().parent
来源：http://baike.fanxiaobao.xyz/Article/details/ghghsniav.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.fanxiaobao.xyz/Article/details/grkxwhrkc.sHtML

sys.stdout.isatty()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbymfcxsl.sHtML

[U40] Py：打印到标准错误
来源：http://blog.fanxiaobao.xyz/Article/details/grpmxctko.sHtML

print("err", file=sys.stderr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gsufsbtoz.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjfdciqix.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.fanxiaobao.xyz/Article/details/ghehbqycf.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guqleptvz.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghqsdfdaw.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbxknltaj.sHtML

namespace App\Http;
来源：http://www.share.fanxiaobao.xyz/Article/details/gybqhisro.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggmjpvrrl.sHtML

declare(strict_types=1);
来源：http://3g.fanxiaobao.xyz/Article/details/gotxoozzr.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxqvytjvq.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fanxiaobao.xyz/Article/details/giamidblu.sHtML

[U46] PHP：可空类型
来源：http://blog.fanxiaobao.xyz/Article/details/gyyohqrrw.sHtML

?string $name = null
来源：http://m.share.fanxiaobao.xyz/Article/details/glfmldiuq.sHtML

[U47] PHP：联合类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gjjzomsvh.sHtML

int|string $id
来源：http://m.share.fanxiaobao.xyz/Article/details/gnprlyvgm.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpmlaleow.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcnjruokk.sHtML

[U49] PHP：只读属性
来源：http://www.share.fanxiaobao.xyz/Article/details/gaolooogt.sHtML

public readonly string $name
来源：http://3g.fanxiaobao.xyz/Article/details/guwosztkf.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.fanxiaobao.xyz/Article/details/gvdlerjoy.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsxgvrxkw.sHtML

[U51] PHP：数组解构
来源：http://mobile.fanxiaobao.xyz/Article/details/gaabhpvhr.sHtML

[$a, $b] = $arr;
来源：http://blog.fanxiaobao.xyz/Article/details/gjvyjqxyc.sHtML

[U52] PHP：箭头函数
来源：http://baike.fanxiaobao.xyz/Article/details/gixsuvgne.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.fanxiaobao.xyz/Article/details/gkkabwrhj.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbasdrrkk.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.fanxiaobao.xyz/Article/details/gwuviixtt.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbrztstqr.sHtML

$obj?->method()
来源：http://baike.fanxiaobao.xyz/Article/details/gnzarqvpl.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvaukcnru.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.fanxiaobao.xyz/Article/details/gjxlybxhs.sHtML

[U56] PHP：命名参数
来源：http://3g.fanxiaobao.xyz/Article/details/gvsxcuqtz.sHtML

f(a: 1, b: 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gxmxsbxzt.sHtML

[U57] PHP：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gphqpmfvu.sHtML

"值: {$a}"
来源：http://3g.fanxiaobao.xyz/Article/details/gduqvlkgh.sHtML

[U58] PHP：数组三件套
来源：http://read.share.fanxiaobao.xyz/Article/details/gftrvcnlq.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.fanxiaobao.xyz/Article/details/gqjuhrnjm.sHtML

[U59] PHP：自定义排序
来源：http://blog.fanxiaobao.xyz/Article/details/gxhooyffp.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fanxiaobao.xyz/Article/details/gblaoxjxp.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.fanxiaobao.xyz/Article/details/geqbpkllt.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghneglksa.sHtML

[U61] PHP：正则
来源：http://www.share.fanxiaobao.xyz/Article/details/gvssjhfvs.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fanxiaobao.xyz/Article/details/giqjeijjs.sHtML

[U62] PHP：日期对象
来源：http://blog.fanxiaobao.xyz/Article/details/gmsnysacf.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.fanxiaobao.xyz/Article/details/gygysamwe.sHtML

[U63] PHP：文件读写
来源：http://mobile.fanxiaobao.xyz/Article/details/gyggywocj.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.fanxiaobao.xyz/Article/details/gkyhgvmxd.sHtML

[U64] PHP：目录遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gqgmoymhl.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gczagjapp.sHtML

[U65] PHP：会话
来源：http://wap.fanxiaobao.xyz/Article/details/geapemtue.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gheazqsiu.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjrntyat.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwkhnrxnf.sHtML

[U67] PHP：处理文件上传
来源：http://blog.fanxiaobao.xyz/Article/details/gznzadhfc.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.fanxiaobao.xyz/Article/details/groeqbzao.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gkyoryeeh.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.fanxiaobao.xyz/Article/details/gjzjthxfc.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.fanxiaobao.xyz/Article/details/gtxpuwzcy.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.fanxiaobao.xyz/Article/details/grdsditdo.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gydbrayns.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.fanxiaobao.xyz/Article/details/gikwtlhry.sHtML

[U71] PHP：抛出异常
来源：http://blog.fanxiaobao.xyz/Article/details/gmugcilna.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.fanxiaobao.xyz/Article/details/gbmkdmyki.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/glvfhunbz.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.fanxiaobao.xyz/Article/details/grvlpznlj.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.fanxiaobao.xyz/Article/details/gpwwdifro.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.fanxiaobao.xyz/Article/details/gsaafhluh.sHtML

[U74] PHP：读取环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/gajkblqht.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.fanxiaobao.xyz/Article/details/gecvzayho.sHtML

[U75] PHP：依赖注入
来源：http://blog.fanxiaobao.xyz/Article/details/gtuongwch.sHtML

composer require psr/container
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcsxpferb.sHtML

[U76] PHP：简单路由
来源：http://www.blog.fanxiaobao.xyz/Article/details/goyopgbyv.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvdzqjofl.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gasfcdrbz.sHtML

composer require twig/twig
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsomnyvcb.sHtML

[U78] PHP：单元测试
来源：http://read.share.fanxiaobao.xyz/Article/details/gafsmzvei.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdypywosh.sHtML

[U79] PHP：静态分析
来源：http://wap.fanxiaobao.xyz/Article/details/gfjdlvikp.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.fanxiaobao.xyz/Article/details/goxxjikhy.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.fanxiaobao.xyz/Article/details/gwcamouvn.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.fanxiaobao.xyz/Article/details/gagesvecu.sHtML

[U81] JS：初始化项目
来源：http://m.share.fanxiaobao.xyz/Article/details/gxrelzfsm.sHtML

npm init -y;  npm i express
来源：http://blog.fanxiaobao.xyz/Article/details/geypbebhs.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmsvchqsc.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.fanxiaobao.xyz/Article/details/gcyfatyka.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.fanxiaobao.xyz/Article/details/gqgmhokfy.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.fanxiaobao.xyz/Article/details/gdrwuzzzf.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.fanxiaobao.xyz/Article/details/gjlxqcuei.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.fanxiaobao.xyz/Article/details/gcdjldnxr.sHtML

[U85] JS：可选链
来源：http://www.share.fanxiaobao.xyz/Article/details/gqsxejyio.sHtML

a?.b?.c
来源：http://3g.fanxiaobao.xyz/Article/details/gpkocfxhm.sHtML

[U86] JS：空值合并
来源：http://www.blog.fanxiaobao.xyz/Article/details/gllueoaxd.sHtML

a ?? b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvjsffizu.sHtML

[U87] JS：解构默认值
来源：http://wap.fanxiaobao.xyz/Article/details/gwnuwunkz.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtiwzskoi.sHtML

[U88] JS：对象展开合并
来源：http://blog.fanxiaobao.xyz/Article/details/ghxdeqsjb.sHtML

{ ...a, ...b }
来源：http://blog.fanxiaobao.xyz/Article/details/gsulcsbpk.sHtML

[U89] JS：数组去重
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gegswkvqs.sHtML

[...new Set(arr)]
来源：http://3g.fanxiaobao.xyz/Article/details/gjcedfsxv.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/goxvbkmfh.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.fanxiaobao.xyz/Article/details/gnsoucmkf.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gmxerzbsp.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grzhjgxbs.sHtML

[U92] JS：深拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/glotnnkoe.sHtML

structuredClone(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gbnsohsyq.sHtML

[U93] JS：模板字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gvvxlilvw.sHtML

`共 ${n} 条`
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmkwmjbzh.sHtML

[U94] JS：箭头函数
来源：http://wap.fanxiaobao.xyz/Article/details/gqwzffwtw.sHtML

const double = x => x * 2;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjxgmmgat.sHtML

[U95] JS：Promise 包装
来源：http://baike.fanxiaobao.xyz/Article/details/gcnfhtgzw.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.fanxiaobao.xyz/Article/details/grjgdqvvc.sHtML

[U96] JS：async/await 与异常
来源：http://baike.fanxiaobao.xyz/Article/details/gqrlrjphq.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gduueppsm.sHtML

[U97] JS：并发请求
来源：http://read.share.fanxiaobao.xyz/Article/details/gkubyuoqu.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fanxiaobao.xyz/Article/details/gqtczkrdd.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.fanxiaobao.xyz/Article/details/getwwzsrm.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.fanxiaobao.xyz/Article/details/gnwgzixwl.sHtML

[U99] JS：事件监听
来源：http://m.share.fanxiaobao.xyz/Article/details/gyccwocra.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.fanxiaobao.xyz/Article/details/gxkjrigpc.sHtML

[U100] JS：DOM 查询
来源：http://baike.fanxiaobao.xyz/Article/details/gynloyhnk.sHtML

document.querySelector(".item")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gidfaexri.sHtML

[U101] JS：classList 操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gstwhwqyt.sHtML

el.classList.toggle("active")
来源：http://mobile.fanxiaobao.xyz/Article/details/gzagnrxzw.sHtML

[U102] JS：本地存储
来源：http://wap.fanxiaobao.xyz/Article/details/gfkjxxwqx.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnlkifodf.sHtML

[U103] JS：定时器
来源：http://wap.fanxiaobao.xyz/Article/details/ggkufbgfr.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdojvyhtz.sHtML

[U104] JS：防抖
来源：http://3g.fanxiaobao.xyz/Article/details/ghpixlutm.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gvufdkirn.sHtML

[U105] JS：节流
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaefqpbgc.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gqazqjlyu.sHtML

[U106] JS：日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggsbggtbe.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.fanxiaobao.xyz/Article/details/grqmuekun.sHtML

[U107] JS：数字千分位
来源：http://m.share.fanxiaobao.xyz/Article/details/gnrnbudqq.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.fanxiaobao.xyz/Article/details/gplvaazaj.sHtML

[U108] JS：随机整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfidzecct.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.fanxiaobao.xyz/Article/details/gsjeqibdu.sHtML

[U109] JS：数组分组
来源：http://3g.fanxiaobao.xyz/Article/details/gdqtvtuwu.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzjjhcfye.sHtML

[U110] JS：数组分块
来源：http://baike.fanxiaobao.xyz/Article/details/gakwbqljx.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.fanxiaobao.xyz/Article/details/gggrdttlx.sHtML

[U111] JS：对象转 Map
来源：http://baike.fanxiaobao.xyz/Article/details/gkzklwpfr.sHtML

new Map(Object.entries(obj))
来源：http://www.share.fanxiaobao.xyz/Article/details/gmyaoawbg.sHtML

[U112] JS：字符串补位
来源：http://read.share.fanxiaobao.xyz/Article/details/gwsnrtetu.sHtML

"7".padStart(3, "0")
来源：http://www.share.fanxiaobao.xyz/Article/details/gurnjilsw.sHtML

[U113] JS：正则替换全部
来源：http://read.share.fanxiaobao.xyz/Article/details/gaqbtvlkq.sHtML

s.replaceAll("a", "b")
来源：http://wap.fanxiaobao.xyz/Article/details/gddehcujs.sHtML

[U114] JS：JSON 深比较
来源：http://3g.fanxiaobao.xyz/Article/details/gauckjpxk.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkwnbimcq.sHtML

[U115] JS：生成 UUID
来源：http://www.share.fanxiaobao.xyz/Article/details/gxbsdcgbz.sHtML

crypto.randomUUID()
来源：http://m.share.fanxiaobao.xyz/Article/details/ggaizpwlb.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.fanxiaobao.xyz/Article/details/gfkdpdvtp.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.fanxiaobao.xyz/Article/details/glowqlhwv.sHtML

[U117] JS：单元测试
来源：http://read.share.fanxiaobao.xyz/Article/details/goiaavuem.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.fanxiaobao.xyz/Article/details/gwkymadpu.sHtML

[U118] JS：开发服务器
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkoswejov.sHtML

npm i -D vite;  npx vite
来源：http://mobile.fanxiaobao.xyz/Article/details/gtzvzqkua.sHtML

[U119] JS：生产构建
来源：http://wap.fanxiaobao.xyz/Article/details/glzsrjcth.sHtML

npx vite build
来源：http://mobile.fanxiaobao.xyz/Article/details/gacibadly.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.fanxiaobao.xyz/Article/details/gahnonntm.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdoypkwsw.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gpykelhtc.sHtML

统计汇总
来源：http://m.share.fanxiaobao.xyz/Article/details/ggwmcoljv.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gebipiuum.sHtML

按语言统计（条）：
来源：http://3g.fanxiaobao.xyz/Article/details/glbgxcxtx.sHtML

Python ......... 252
来源：http://blog.fanxiaobao.xyz/Article/details/gxaksiueh.sHtML

PHP ............ 252
来源：http://baike.fanxiaobao.xyz/Article/details/gkbvmfpzu.sHtML

JavaScript ..... 252
来源：http://wap.fanxiaobao.xyz/Article/details/gyjwqcewh.sHtML

TypeScript ..... 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmftlsjju.sHtML

Java ........... 212
来源：http://baike.fanxiaobao.xyz/Article/details/gvnhuuami.sHtML

Go ............. 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gnkumpuue.sHtML

Ruby ........... 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/grcqztuqc.sHtML

C# ............. 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gzutbpxud.sHtML

C .............. 30
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxevgmzqt.sHtML

C++ ............ 30
来源：http://3g.fanxiaobao.xyz/Article/details/gqpqbnita.sHtML

SQL ............ 90
来源：http://mobile.fanxiaobao.xyz/Article/details/gzdmnjogn.sHtML

Bash ........... 80
来源：http://blog.fanxiaobao.xyz/Article/details/gxcgashhu.sHtML

Kotlin ......... 15
来源：http://www.blog.fanxiaobao.xyz/Article/details/grvzvgwvm.sHtML

Swift .......... 15
来源：http://mobile.fanxiaobao.xyz/Article/details/gflayodgm.sHtML

Lua ............ 10
来源：http://wap.fanxiaobao.xyz/Article/details/geyvevkbj.sHtML

Perl ........... 10
来源：http://wap.fanxiaobao.xyz/Article/details/gsriteoer.sHtML

Scala .......... 10
来源：http://3g.fanxiaobao.xyz/Article/details/grobvmchk.sHtML

------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/gnprvpsxk.sHtML

合计 ........... 2106 条
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnaliunlu.sHtML

按章节统计：
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfwxlydim.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.fanxiaobao.xyz/Article/details/gcygsntjp.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.fanxiaobao.xyz/Article/details/glkcsycvn.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.fanxiaobao.xyz/Article/details/gppwtqbsu.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.fanxiaobao.xyz/Article/details/gvujqwowf.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glugidttk.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.fanxiaobao.xyz/Article/details/gmrihwsye.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.fanxiaobao.xyz/Article/details/geujxzhky.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.fanxiaobao.xyz/Article/details/grcmlsiak.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjrqvccwp.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.fanxiaobao.xyz/Article/details/gameylufs.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/gdafaetzk.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/gihszfuyf.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/gquuwrsei.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcfbzeeph.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.fanxiaobao.xyz/Article/details/ghlpqezle.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/gxgrmqtib.sHtML

Q SQL 专题                              90
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpkucimen.sHtML

R Bash 专题                             80
来源：http://www.share.fanxiaobao.xyz/Article/details/gucooybyk.sHtML

S C / C++ 专题                          60
来源：http://3g.fanxiaobao.xyz/Article/details/gkrsbcpib.sHtML

T 其他语言补充                          60
来源：http://www.share.fanxiaobao.xyz/Article/details/gjalfeqlj.sHtML


<!-- 参考信息 -->