代发 wailian999

val a = 1;  var b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjdzmullg.sHtML

[T53] Scala：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gqdjndwgv.sHtML

s"值: $b"
来源：http://www.share.fanxiaobao.xyz/Article/details/glllinxfa.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gspyysxfn.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gggeacyfp.sHtML

[T55] Scala：集合过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gcaroxmii.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvycfvwvd.sHtML

[T56] Scala：样例类
来源：http://m.share.fanxiaobao.xyz/Article/details/gfkhyeqja.sHtML

case class User(name: String, age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/ggkazeuds.sHtML

[T57] Scala：模式匹配
来源：http://blog.fanxiaobao.xyz/Article/details/glmqrhuwe.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gubaecsaj.sHtML

[T58] Scala：函数定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gpdaijled.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.fanxiaobao.xyz/Article/details/gosniwyfh.sHtML

[T59] Scala：循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gprgzuqfn.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.fanxiaobao.xyz/Article/details/gwzkspwpb.sHtML

[T60] Scala：折叠
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvhojliy.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvlcnklyh.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gmqokxttf.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gnbaykhsj.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjrhosytq.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.fanxiaobao.xyz/Article/details/gucvamzwk.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.fanxiaobao.xyz/Article/details/golmpktvs.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fanxiaobao.xyz/Article/details/gynoeqypu.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.fanxiaobao.xyz/Article/details/geptuhsmu.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.fanxiaobao.xyz/Article/details/gvybvomfy.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.fanxiaobao.xyz/Article/details/gxmbmsyfn.sHtML

[U04] Py：变量调试打印
来源：http://blog.fanxiaobao.xyz/Article/details/gyqodwibf.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.fanxiaobao.xyz/Article/details/gricfespz.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.fanxiaobao.xyz/Article/details/grkrsjgzh.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwhbusokw.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gvlyughdp.sHtML

{**a, **b}
来源：http://3g.fanxiaobao.xyz/Article/details/gtdpxajit.sHtML

[U07] Py：反转字典键值
来源：http://baike.fanxiaobao.xyz/Article/details/gfigxwdxj.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.fanxiaobao.xyz/Article/details/getutjzhp.sHtML

[U08] Py：展平二维列表
来源：http://wap.fanxiaobao.xyz/Article/details/gwdgiincf.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gogwwyiwm.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grghbvfol.sHtML

max(d, key=d.get)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmdskiwaa.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggshgexxn.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.fanxiaobao.xyz/Article/details/gfvfitayv.sHtML

[U11] Py：生成器表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gluozgvbt.sHtML

(x * 2 for x in arr)
来源：http://3g.fanxiaobao.xyz/Article/details/guivfvavg.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gvaxqqasi.sHtML

Counter(arr).most_common(3)
来源：http://wap.fanxiaobao.xyz/Article/details/gaeszmuqd.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.fanxiaobao.xyz/Article/details/guzbiskyo.sHtML

deque(maxlen=10)
来源：http://baike.fanxiaobao.xyz/Article/details/gghujlcqx.sHtML

[U14] Py：分组收集到列表
来源：http://baike.fanxiaobao.xyz/Article/details/gxicwgtbj.sHtML

defaultdict(list)
来源：http://www.share.fanxiaobao.xyz/Article/details/glvqjhhug.sHtML

[U15] Py：高精度计时
来源：http://m.share.fanxiaobao.xyz/Article/details/gdvlcyonm.sHtML

t = time.perf_counter()
来源：http://read.share.fanxiaobao.xyz/Article/details/gqsfkncqt.sHtML

[U16] Py：命令行参数解析
来源：http://blog.fanxiaobao.xyz/Article/details/gzvtxxote.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.fanxiaobao.xyz/Article/details/godrutbgz.sHtML

[U17] Py：初始化日志
来源：http://blog.fanxiaobao.xyz/Article/details/gekplvbqh.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcijgpmaj.sHtML

[U18] Py：预编译正则
来源：http://www.share.fanxiaobao.xyz/Article/details/gbpfkdrpg.sHtML

pat = re.compile(r"\d+")
来源：http://baike.fanxiaobao.xyz/Article/details/gvnivcrys.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.fanxiaobao.xyz/Article/details/gxwbyjrco.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjhimlckp.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.fanxiaobao.xyz/Article/details/gienpfhbd.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.fanxiaobao.xyz/Article/details/gsxzaoxfk.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.fanxiaobao.xyz/Article/details/gmdhqakkg.sHtML

@contextlib.contextmanager
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gakpegnqu.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.fanxiaobao.xyz/Article/details/gihbxvgop.sHtML

list(zip(*m))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqyhmbitx.sHtML

[U23] Py：分块读取大文件
来源：http://blog.fanxiaobao.xyz/Article/details/gktnqeteb.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.fanxiaobao.xyz/Article/details/gnckjrhfl.sHtML

[U24] Py：路径操作
来源：http://baike.fanxiaobao.xyz/Article/details/guhgqfhtn.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.fanxiaobao.xyz/Article/details/gkwubcadj.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.fanxiaobao.xyz/Article/details/gwajnyffw.sHtML

csv.DictReader(f)
来源：http://wap.fanxiaobao.xyz/Article/details/gyhasmbku.sHtML

[U26] Py：并发下载
来源：http://mobile.fanxiaobao.xyz/Article/details/ggwqhlsfx.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.fanxiaobao.xyz/Article/details/geqkqecyu.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.fanxiaobao.xyz/Article/details/grkgztzvr.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.fanxiaobao.xyz/Article/details/gzozupvaq.sHtML

[U28] Py：类型别名
来源：http://m.share.fanxiaobao.xyz/Article/details/gwvjqqxzi.sHtML

UserId = int
来源：http://mobile.fanxiaobao.xyz/Article/details/goiiwgzkb.sHtML

[U29] Py：属性校验
来源：http://mobile.fanxiaobao.xyz/Article/details/gztcfarap.sHtML

@property 与 @x.setter 配合
来源：http://mobile.fanxiaobao.xyz/Article/details/gerqydkzi.sHtML

[U30] Py：数据类
来源：http://m.share.fanxiaobao.xyz/Article/details/gbrsgemdo.sHtML

@dataclass(slots=True)
来源：http://wap.fanxiaobao.xyz/Article/details/ggcxvzhcv.sHtML

[U31] Py：单测
来源：http://blog.fanxiaobao.xyz/Article/details/grhysraji.sHtML

python -m pytest -q
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjgepbxz.sHtML

[U32] Py：代码格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gxvuzbspg.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcvttfbpv.sHtML

[U33] Py：打包发布
来源：http://m.share.fanxiaobao.xyz/Article/details/gqsriloac.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.fanxiaobao.xyz/Article/details/geqhqiymo.sHtML

[U34] Py：判断编码
来源：http://mobile.fanxiaobao.xyz/Article/details/gickspkep.sHtML

chardet.detect(raw)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcyygjqbl.sHtML

[U35] Py：发送邮件
来源：http://3g.fanxiaobao.xyz/Article/details/grsbcmbfz.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.fanxiaobao.xyz/Article/details/gufdubzmw.sHtML

[U36] Py：定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/grvxcfvev.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.fanxiaobao.xyz/Article/details/gphsibmzj.sHtML

[U37] Py：读写 Excel
来源：http://read.share.fanxiaobao.xyz/Article/details/gyjrhtkcn.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.fanxiaobao.xyz/Article/details/gxhinskrj.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.fanxiaobao.xyz/Article/details/ghrwxijlq.sHtML

Path(__file__).resolve().parent
来源：http://wap.fanxiaobao.xyz/Article/details/gyhqznvjm.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.fanxiaobao.xyz/Article/details/gosngbehu.sHtML

sys.stdout.isatty()
来源：http://www.blog.fanxiaobao.xyz/Article/details/govogozwx.sHtML

[U40] Py：打印到标准错误
来源：http://3g.fanxiaobao.xyz/Article/details/gklxqeebq.sHtML

print("err", file=sys.stderr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gswpsrpcl.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.fanxiaobao.xyz/Article/details/gukdajgzr.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.fanxiaobao.xyz/Article/details/grwpuszyd.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.fanxiaobao.xyz/Article/details/gjmvtqens.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.fanxiaobao.xyz/Article/details/gphajhsjv.sHtML

[U43] PHP：声明命名空间
来源：http://wap.fanxiaobao.xyz/Article/details/grecvssph.sHtML

namespace App\Http;
来源：http://read.share.fanxiaobao.xyz/Article/details/geaxavkbw.sHtML

[U44] PHP：开启严格类型
来源：http://baike.fanxiaobao.xyz/Article/details/getcfqyfx.sHtML

declare(strict_types=1);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbimwvqhk.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/guugvalpo.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gokbabbww.sHtML

[U46] PHP：可空类型
来源：http://wap.fanxiaobao.xyz/Article/details/gjscugslc.sHtML

?string $name = null
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpsqwrhbu.sHtML

[U47] PHP：联合类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcusruwit.sHtML

int|string $id
来源：http://3g.fanxiaobao.xyz/Article/details/gkdaicgkn.sHtML

[U48] PHP：纯枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gsiutgyqh.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gowoelgtl.sHtML

[U49] PHP：只读属性
来源：http://baike.fanxiaobao.xyz/Article/details/glouarbzz.sHtML

public readonly string $name
来源：http://wap.fanxiaobao.xyz/Article/details/gvarmzeny.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.fanxiaobao.xyz/Article/details/geqhqnupo.sHtML

public function __construct(private int $id) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gxilzysgc.sHtML

[U51] PHP：数组解构
来源：http://blog.fanxiaobao.xyz/Article/details/gaghnfmba.sHtML

[$a, $b] = $arr;
来源：http://3g.fanxiaobao.xyz/Article/details/gwwdkrubj.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/grbmcwvkg.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpqrbtsex.sHtML

[U53] PHP：空合并运算符
来源：http://3g.fanxiaobao.xyz/Article/details/gxvkbamhp.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.fanxiaobao.xyz/Article/details/gwxjpghuv.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gylndruql.sHtML

$obj?->method()
来源：http://mobile.fanxiaobao.xyz/Article/details/gipugskvb.sHtML

[U55] PHP：match 表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gqznndbti.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.fanxiaobao.xyz/Article/details/guxnzictw.sHtML

[U56] PHP：命名参数
来源：http://3g.fanxiaobao.xyz/Article/details/gpgpqelcj.sHtML

f(a: 1, b: 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkgkgxtwu.sHtML

[U57] PHP：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/glxrwsoct.sHtML

"值: {$a}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbuxaiakl.sHtML

[U58] PHP：数组三件套
来源：http://baike.fanxiaobao.xyz/Article/details/glbqypfjr.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.fanxiaobao.xyz/Article/details/gdgduvwtj.sHtML

[U59] PHP：自定义排序
来源：http://baike.fanxiaobao.xyz/Article/details/gpxughzmw.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyeeyegun.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjflcgqjy.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.fanxiaobao.xyz/Article/details/gohuhyhrp.sHtML

[U61] PHP：正则
来源：http://wap.fanxiaobao.xyz/Article/details/gesynxmfd.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmnpvbfkj.sHtML

[U62] PHP：日期对象
来源：http://www.share.fanxiaobao.xyz/Article/details/ggwfbtdtd.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.fanxiaobao.xyz/Article/details/gkpuptavt.sHtML

[U63] PHP：文件读写
来源：http://3g.fanxiaobao.xyz/Article/details/getwolaid.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.fanxiaobao.xyz/Article/details/gyjreuvsa.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gruriefuk.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzynvtybl.sHtML

[U65] PHP：会话
来源：http://baike.fanxiaobao.xyz/Article/details/gjafilvwy.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gxpltpfff.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.fanxiaobao.xyz/Article/details/gaxanabgm.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.fanxiaobao.xyz/Article/details/gqbetnzzd.sHtML

[U67] PHP：处理文件上传
来源：http://baike.fanxiaobao.xyz/Article/details/gvwnjcpgp.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.fanxiaobao.xyz/Article/details/gmqmcimox.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gcneeconn.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.fanxiaobao.xyz/Article/details/glgkvldgk.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gciuvpnwl.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghtxclztn.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gdhztkosq.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.fanxiaobao.xyz/Article/details/gzrdohorq.sHtML

[U71] PHP：抛出异常
来源：http://wap.fanxiaobao.xyz/Article/details/gcfnqfjua.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.fanxiaobao.xyz/Article/details/gvfeynqng.sHtML

[U72] PHP：写错误日志
来源：http://wap.fanxiaobao.xyz/Article/details/gqissfhlx.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkimmvxqt.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.fanxiaobao.xyz/Article/details/gklydeavx.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.fanxiaobao.xyz/Article/details/gfhrkkfcb.sHtML

[U74] PHP：读取环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/gvgvwagdn.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbnifxxhi.sHtML

[U75] PHP：依赖注入
来源：http://3g.fanxiaobao.xyz/Article/details/geblzcwht.sHtML

composer require psr/container
来源：http://read.share.fanxiaobao.xyz/Article/details/gwhwnoptg.sHtML

[U76] PHP：简单路由
来源：http://blog.fanxiaobao.xyz/Article/details/gbgrwlqmb.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.fanxiaobao.xyz/Article/details/gbjlwkobk.sHtML

[U77] PHP：模板渲染
来源：http://blog.fanxiaobao.xyz/Article/details/gqoulneaa.sHtML

composer require twig/twig
来源：http://read.share.fanxiaobao.xyz/Article/details/gzfvlzpxk.sHtML

[U78] PHP：单元测试
来源：http://m.share.fanxiaobao.xyz/Article/details/gwszvhmkr.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghybxsftq.sHtML

[U79] PHP：静态分析
来源：http://3g.fanxiaobao.xyz/Article/details/gsbqooeri.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.fanxiaobao.xyz/Article/details/grjkfcttz.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.fanxiaobao.xyz/Article/details/gwhnbotnu.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdjsfmteh.sHtML

[U81] JS：初始化项目
来源：http://mobile.fanxiaobao.xyz/Article/details/glvoqstlz.sHtML

npm init -y;  npm i express
来源：http://m.share.fanxiaobao.xyz/Article/details/gehacuivj.sHtML

[U82] JS：package.json 脚本
来源：http://blog.fanxiaobao.xyz/Article/details/gmxarhrbz.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdmuduhti.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.fanxiaobao.xyz/Article/details/gbqnjeyga.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glvzkqlov.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.fanxiaobao.xyz/Article/details/gzyeaxxxg.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.fanxiaobao.xyz/Article/details/gflqadrhr.sHtML

[U85] JS：可选链
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwwuqelnx.sHtML

a?.b?.c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjmloxqog.sHtML

[U86] JS：空值合并
来源：http://www.share.fanxiaobao.xyz/Article/details/glkctixoq.sHtML

a ?? b
来源：http://wap.fanxiaobao.xyz/Article/details/ggirmnnch.sHtML

[U87] JS：解构默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/gmeaexdls.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.fanxiaobao.xyz/Article/details/gioqdforu.sHtML

[U88] JS：对象展开合并
来源：http://wap.fanxiaobao.xyz/Article/details/ggziwdxqn.sHtML

{ ...a, ...b }
来源：http://wap.fanxiaobao.xyz/Article/details/guizvojbs.sHtML

[U89] JS：数组去重
来源：http://read.share.fanxiaobao.xyz/Article/details/gokpetlau.sHtML

[...new Set(arr)]
来源：http://blog.fanxiaobao.xyz/Article/details/gqnkwrhrx.sHtML

[U90] JS：数字数组排序
来源：http://3g.fanxiaobao.xyz/Article/details/gmjafityw.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gstdupcho.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gvmcnchhl.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.fanxiaobao.xyz/Article/details/grjsrvmbk.sHtML

[U92] JS：深拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gjmetkvin.sHtML

structuredClone(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/genoifpkx.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnapwtril.sHtML

`共 ${n} 条`
来源：http://m.share.fanxiaobao.xyz/Article/details/gqquxderv.sHtML

[U94] JS：箭头函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gxtvrspps.sHtML

const double = x => x * 2;
来源：http://3g.fanxiaobao.xyz/Article/details/gvlivyutr.sHtML

[U95] JS：Promise 包装
来源：http://baike.fanxiaobao.xyz/Article/details/gtoexopin.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.fanxiaobao.xyz/Article/details/gauhkmeet.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbpomkzkj.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxaptezrq.sHtML

[U97] JS：并发请求
来源：http://baike.fanxiaobao.xyz/Article/details/grdoltdou.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fanxiaobao.xyz/Article/details/gxasticrv.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/gtmptrgzb.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.fanxiaobao.xyz/Article/details/gfqolhcjw.sHtML

[U99] JS：事件监听
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyqcnbxrm.sHtML

el.addEventListener("click", e => {})
来源：http://baike.fanxiaobao.xyz/Article/details/gxkexjhmp.sHtML

[U100] JS：DOM 查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gxetkncvo.sHtML

document.querySelector(".item")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaxzxfsxg.sHtML

[U101] JS：classList 操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gjuuqhkow.sHtML

el.classList.toggle("active")
来源：http://read.share.fanxiaobao.xyz/Article/details/ghkpyvbud.sHtML

[U102] JS：本地存储
来源：http://www.share.fanxiaobao.xyz/Article/details/gxfxxfwze.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.fanxiaobao.xyz/Article/details/gqjwdmoqf.sHtML

[U103] JS：定时器
来源：http://blog.fanxiaobao.xyz/Article/details/gywphlguc.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.fanxiaobao.xyz/Article/details/grdiyqbsr.sHtML

[U104] JS：防抖
来源：http://3g.fanxiaobao.xyz/Article/details/gdmbhsnkw.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fanxiaobao.xyz/Article/details/gukupnblj.sHtML

[U105] JS：节流
来源：http://mobile.fanxiaobao.xyz/Article/details/gyavwuyib.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.fanxiaobao.xyz/Article/details/gxghkzoni.sHtML

[U106] JS：日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gmotsbfvp.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.fanxiaobao.xyz/Article/details/gvlkqhdwt.sHtML

[U107] JS：数字千分位
来源：http://mobile.fanxiaobao.xyz/Article/details/gexielpiq.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzzrpvbhd.sHtML

[U108] JS：随机整数
来源：http://3g.fanxiaobao.xyz/Article/details/gryxnbnaf.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.fanxiaobao.xyz/Article/details/gaqqomsrk.sHtML

[U109] JS：数组分组
来源：http://blog.fanxiaobao.xyz/Article/details/gyuiartlq.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.fanxiaobao.xyz/Article/details/geouzjifn.sHtML

[U110] JS：数组分块
来源：http://mobile.fanxiaobao.xyz/Article/details/ggjzqdsis.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwupbfdvy.sHtML

[U111] JS：对象转 Map
来源：http://blog.fanxiaobao.xyz/Article/details/grzxcvmas.sHtML

new Map(Object.entries(obj))
来源：http://m.share.fanxiaobao.xyz/Article/details/gbmkevthl.sHtML

[U112] JS：字符串补位
来源：http://mobile.fanxiaobao.xyz/Article/details/gscanpkse.sHtML

"7".padStart(3, "0")
来源：http://wap.fanxiaobao.xyz/Article/details/gpizznijr.sHtML

[U113] JS：正则替换全部
来源：http://baike.fanxiaobao.xyz/Article/details/gdmkihmbl.sHtML

s.replaceAll("a", "b")
来源：http://read.share.fanxiaobao.xyz/Article/details/gkqvjduqo.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gxddshrah.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gsuvaxycy.sHtML

[U115] JS：生成 UUID
来源：http://www.share.fanxiaobao.xyz/Article/details/gjvseeaxx.sHtML

crypto.randomUUID()
来源：http://3g.fanxiaobao.xyz/Article/details/gsogohhko.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.fanxiaobao.xyz/Article/details/gywwuxiah.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyihlrzcc.sHtML

[U117] JS：单元测试
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvyytmfuh.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.fanxiaobao.xyz/Article/details/gqauzljgx.sHtML

[U118] JS：开发服务器
来源：http://baike.fanxiaobao.xyz/Article/details/gvnapzidj.sHtML

npm i -D vite;  npx vite
来源：http://www.share.fanxiaobao.xyz/Article/details/gesjnlyfw.sHtML

[U119] JS：生产构建
来源：http://mobile.fanxiaobao.xyz/Article/details/gelccamsg.sHtML

npx vite build
来源：http://wap.fanxiaobao.xyz/Article/details/gpxwljibm.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.fanxiaobao.xyz/Article/details/gzbxqqaiv.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.fanxiaobao.xyz/Article/details/ghvqhhgkm.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcavqbmfm.sHtML

统计汇总
来源：http://blog.fanxiaobao.xyz/Article/details/gtjdhepry.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gbbasktrk.sHtML

按语言统计（条）：
来源：http://baike.fanxiaobao.xyz/Article/details/ggzxlujze.sHtML

Python ......... 252
来源：http://www.blog.fanxiaobao.xyz/Article/details/graupvkzm.sHtML

PHP ............ 252
来源：http://baike.fanxiaobao.xyz/Article/details/gsdamzrqa.sHtML

JavaScript ..... 252
来源：http://wap.fanxiaobao.xyz/Article/details/gadmctqgn.sHtML

TypeScript ..... 212
来源：http://wap.fanxiaobao.xyz/Article/details/gxgmwxpqh.sHtML

Java ........... 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gjhofntgc.sHtML

Go ............. 212
来源：http://baike.fanxiaobao.xyz/Article/details/gztgphwml.sHtML

Ruby ........... 212
来源：http://wap.fanxiaobao.xyz/Article/details/gaannswkg.sHtML

C# ............. 212
来源：http://wap.fanxiaobao.xyz/Article/details/gttydvolv.sHtML

C .............. 30
来源：http://read.share.fanxiaobao.xyz/Article/details/gyehfkzgj.sHtML

C++ ............ 30
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gicslengj.sHtML

SQL ............ 90
来源：http://baike.fanxiaobao.xyz/Article/details/gacabavsy.sHtML

Bash ........... 80
来源：http://baike.fanxiaobao.xyz/Article/details/gltqeudzw.sHtML

Kotlin ......... 15
来源：http://wap.fanxiaobao.xyz/Article/details/gfwdfpwjh.sHtML

Swift .......... 15
来源：http://wap.fanxiaobao.xyz/Article/details/gqcjermpf.sHtML

Lua ............ 10
来源：http://m.share.fanxiaobao.xyz/Article/details/ghmdcyfin.sHtML

Perl ........... 10
来源：http://wap.fanxiaobao.xyz/Article/details/gclhcqvnu.sHtML

Scala .......... 10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gukiproqs.sHtML

------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/gizaifywo.sHtML

合计 ........... 2106 条
来源：http://www.share.fanxiaobao.xyz/Article/details/geekntrxa.sHtML

按章节统计：
来源：http://blog.fanxiaobao.xyz/Article/details/gpafutmzu.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.fanxiaobao.xyz/Article/details/gneczhvpb.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnxdkfmjo.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.fanxiaobao.xyz/Article/details/glfgfjdsu.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.fanxiaobao.xyz/Article/details/gcsrmaqzx.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.fanxiaobao.xyz/Article/details/gmtkepwuo.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.fanxiaobao.xyz/Article/details/gpnqcrpog.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.fanxiaobao.xyz/Article/details/gqensoyoe.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.fanxiaobao.xyz/Article/details/gkizundpa.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gvmgumcjs.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.fanxiaobao.xyz/Article/details/gxvjkfhdr.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/gheiphmmy.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gbswpdnli.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/gilmqcwiq.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.fanxiaobao.xyz/Article/details/gmylqzmfp.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.fanxiaobao.xyz/Article/details/gfsaqsmnf.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxipydyhy.sHtML


<!-- 参考信息 -->