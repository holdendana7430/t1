代发 wailian999

case class User(name: String, age: Int)
来源：http://blog.fanxiaobao.xyz/Article/details/ggmbphnbs.sHtML

[T57] Scala：模式匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gnjckukth.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.fanxiaobao.xyz/Article/details/gyosntldq.sHtML

[T58] Scala：函数定义
来源：http://wap.fanxiaobao.xyz/Article/details/gzhpdbihm.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.fanxiaobao.xyz/Article/details/gqkfebxhm.sHtML

[T59] Scala：循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gvrnbapmg.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghgsnjoxa.sHtML

[T60] Scala：折叠
来源：http://www.share.fanxiaobao.xyz/Article/details/gvkxcuzxi.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbjsowjlb.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gugdtvyek.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gxzbhorby.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzntjbnfz.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gstixyvxq.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.fanxiaobao.xyz/Article/details/gamabavez.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.fanxiaobao.xyz/Article/details/gfkupramq.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gegyvldbe.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.fanxiaobao.xyz/Article/details/gdtbabgno.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.fanxiaobao.xyz/Article/details/givemvgad.sHtML

[U04] Py：变量调试打印
来源：http://blog.fanxiaobao.xyz/Article/details/gwvrlhauh.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.fanxiaobao.xyz/Article/details/gsrkymnri.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.fanxiaobao.xyz/Article/details/gxunvryqw.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.fanxiaobao.xyz/Article/details/goprydizt.sHtML

[U06] Py：合并两个字典
来源：http://blog.fanxiaobao.xyz/Article/details/gfclmmrda.sHtML

{**a, **b}
来源：http://mobile.fanxiaobao.xyz/Article/details/gryhojsgs.sHtML

[U07] Py：反转字典键值
来源：http://3g.fanxiaobao.xyz/Article/details/gtuuhxvud.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.fanxiaobao.xyz/Article/details/gcypnryym.sHtML

[U08] Py：展平二维列表
来源：http://3g.fanxiaobao.xyz/Article/details/glfarofhu.sHtML

[y for x in nested for y in x]
来源：http://www.share.fanxiaobao.xyz/Article/details/gzaekkxfs.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.fanxiaobao.xyz/Article/details/gfgpssbjp.sHtML

max(d, key=d.get)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzoewyvnn.sHtML

[U10] Py：按值排序字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gqhkyoqqw.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvoayhnns.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzkedmadc.sHtML

(x * 2 for x in arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzgsixcws.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.fanxiaobao.xyz/Article/details/giowvtcri.sHtML

Counter(arr).most_common(3)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghjdpmjyx.sHtML

[U13] Py：固定长度队列
来源：http://blog.fanxiaobao.xyz/Article/details/gylcgrkix.sHtML

deque(maxlen=10)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwmfwwxkx.sHtML

[U14] Py：分组收集到列表
来源：http://3g.fanxiaobao.xyz/Article/details/garnbccpf.sHtML

defaultdict(list)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goosoczoy.sHtML

[U15] Py：高精度计时
来源：http://www.share.fanxiaobao.xyz/Article/details/gwgzxtivd.sHtML

t = time.perf_counter()
来源：http://blog.fanxiaobao.xyz/Article/details/gbuuyrdww.sHtML

[U16] Py：命令行参数解析
来源：http://3g.fanxiaobao.xyz/Article/details/glsfblalc.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.fanxiaobao.xyz/Article/details/gpopdowgu.sHtML

[U17] Py：初始化日志
来源：http://blog.fanxiaobao.xyz/Article/details/ghbegcfvu.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdlumimnl.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghxiewsdo.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/ggiighpql.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyxdciino.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.fanxiaobao.xyz/Article/details/grdasdgcy.sHtML

[U20] Py：缓存函数结果
来源：http://blog.fanxiaobao.xyz/Article/details/gnivlnfiu.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkphdbceg.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.fanxiaobao.xyz/Article/details/gsgrmyivp.sHtML

@contextlib.contextmanager
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbybyngjk.sHtML

[U22] Py：矩阵转置
来源：http://baike.fanxiaobao.xyz/Article/details/gjoirjguv.sHtML

list(zip(*m))
来源：http://baike.fanxiaobao.xyz/Article/details/gdfcflcto.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.fanxiaobao.xyz/Article/details/grvycdrvh.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.fanxiaobao.xyz/Article/details/gewlstmwh.sHtML

[U24] Py：路径操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gotifqwjj.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.fanxiaobao.xyz/Article/details/ggrkswpwz.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gioagvzou.sHtML

csv.DictReader(f)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gancebkwv.sHtML

[U26] Py：并发下载
来源：http://mobile.fanxiaobao.xyz/Article/details/gbpuyzjnd.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtbiiqxot.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcujwedhw.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.fanxiaobao.xyz/Article/details/gaitwmbmw.sHtML

[U28] Py：类型别名
来源：http://m.share.fanxiaobao.xyz/Article/details/gsezbxxnh.sHtML

UserId = int
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzhofwkjp.sHtML

[U29] Py：属性校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyvmnaraj.sHtML

@property 与 @x.setter 配合
来源：http://wap.fanxiaobao.xyz/Article/details/gpjfhkams.sHtML

[U30] Py：数据类
来源：http://m.share.fanxiaobao.xyz/Article/details/gjkqshrhw.sHtML

@dataclass(slots=True)
来源：http://wap.fanxiaobao.xyz/Article/details/gbjvnwjux.sHtML

[U31] Py：单测
来源：http://www.share.fanxiaobao.xyz/Article/details/gpdspzfkw.sHtML

python -m pytest -q
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmtrqkzjc.sHtML

[U32] Py：代码格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gsogchjza.sHtML

ruff format . && ruff check --fix .
来源：http://3g.fanxiaobao.xyz/Article/details/gjhgcnqrd.sHtML

[U33] Py：打包发布
来源：http://3g.fanxiaobao.xyz/Article/details/gtuktphnu.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.fanxiaobao.xyz/Article/details/gruulitah.sHtML

[U34] Py：判断编码
来源：http://m.share.fanxiaobao.xyz/Article/details/ghaubyccc.sHtML

chardet.detect(raw)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcfjozkqo.sHtML

[U35] Py：发送邮件
来源：http://mobile.fanxiaobao.xyz/Article/details/gzywoxvki.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.fanxiaobao.xyz/Article/details/gregsrxsd.sHtML

[U36] Py：定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gojlyyyml.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcnujcyzo.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyulinpjb.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.fanxiaobao.xyz/Article/details/grplpxzxg.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.fanxiaobao.xyz/Article/details/gkppcitra.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmcsnsayw.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.fanxiaobao.xyz/Article/details/gznalkdix.sHtML

sys.stdout.isatty()
来源：http://m.share.fanxiaobao.xyz/Article/details/gicssbkhj.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gggygawyq.sHtML

print("err", file=sys.stderr)
来源：http://wap.fanxiaobao.xyz/Article/details/gjuqzzomb.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.fanxiaobao.xyz/Article/details/gpcakeszj.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtyakstyd.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghaghjudj.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnakjclnq.sHtML

[U43] PHP：声明命名空间
来源：http://wap.fanxiaobao.xyz/Article/details/gtfsevszg.sHtML

namespace App\Http;
来源：http://mobile.fanxiaobao.xyz/Article/details/gsbbpnwff.sHtML

[U44] PHP：开启严格类型
来源：http://baike.fanxiaobao.xyz/Article/details/gisfflivu.sHtML

declare(strict_types=1);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghnfasfid.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.fanxiaobao.xyz/Article/details/ggejejxyr.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwvyqmjpu.sHtML

[U46] PHP：可空类型
来源：http://baike.fanxiaobao.xyz/Article/details/gfzicrwxk.sHtML

?string $name = null
来源：http://www.share.fanxiaobao.xyz/Article/details/ghnenwpqe.sHtML

[U47] PHP：联合类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gsntaoztv.sHtML

int|string $id
来源：http://3g.fanxiaobao.xyz/Article/details/gvhvbmhmo.sHtML

[U48] PHP：纯枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gtcqmpsxy.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvihkqrrr.sHtML

[U49] PHP：只读属性
来源：http://mobile.fanxiaobao.xyz/Article/details/govauslqp.sHtML

public readonly string $name
来源：http://mobile.fanxiaobao.xyz/Article/details/gbpirtiwi.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glymhrzaa.sHtML

public function __construct(private int $id) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gflbaxmxx.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzewyaxpz.sHtML

[$a, $b] = $arr;
来源：http://baike.fanxiaobao.xyz/Article/details/gjhudqfva.sHtML

[U52] PHP：箭头函数
来源：http://baike.fanxiaobao.xyz/Article/details/ghdcrdila.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.fanxiaobao.xyz/Article/details/gxbzalmml.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.fanxiaobao.xyz/Article/details/gavubkirw.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkdtxyhjz.sHtML

[U54] PHP：空安全调用
来源：http://m.share.fanxiaobao.xyz/Article/details/gewnjwjsn.sHtML

$obj?->method()
来源：http://read.share.fanxiaobao.xyz/Article/details/gzvphsrcw.sHtML

[U55] PHP：match 表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwhjbmos.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.fanxiaobao.xyz/Article/details/gpotbkxwp.sHtML

[U56] PHP：命名参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gseajleiq.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxsyduzpk.sHtML

[U57] PHP：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gykqcnoqu.sHtML

"值: {$a}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gpdrexukg.sHtML

[U58] PHP：数组三件套
来源：http://m.share.fanxiaobao.xyz/Article/details/gxbzcavmc.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwgokxnow.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gplfugibe.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fanxiaobao.xyz/Article/details/gvswiardf.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.fanxiaobao.xyz/Article/details/ghqjowqou.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.fanxiaobao.xyz/Article/details/gpebbfwrs.sHtML

[U61] PHP：正则
来源：http://m.share.fanxiaobao.xyz/Article/details/gcimwjtrn.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fanxiaobao.xyz/Article/details/gsnehntra.sHtML

[U62] PHP：日期对象
来源：http://3g.fanxiaobao.xyz/Article/details/ghkfhjkbf.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxwzhbfba.sHtML

[U63] PHP：文件读写
来源：http://wap.fanxiaobao.xyz/Article/details/gbmwtyssc.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.fanxiaobao.xyz/Article/details/gbbfhowzw.sHtML

[U64] PHP：目录遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gihcsausc.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.fanxiaobao.xyz/Article/details/gbyqgttbx.sHtML

[U65] PHP：会话
来源：http://mobile.fanxiaobao.xyz/Article/details/gfedezyyn.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gsbwunoqs.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.fanxiaobao.xyz/Article/details/gdrzlesgd.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glqwfeaxv.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.fanxiaobao.xyz/Article/details/gbdovlaxy.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.fanxiaobao.xyz/Article/details/ghebmkpio.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.fanxiaobao.xyz/Article/details/grryqhftf.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyyejtygo.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gdodbahgx.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gncvotusq.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gtdqjwejf.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.fanxiaobao.xyz/Article/details/gaiipptzu.sHtML

[U71] PHP：抛出异常
来源：http://m.share.fanxiaobao.xyz/Article/details/gakiafjsg.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.fanxiaobao.xyz/Article/details/gfodlavyj.sHtML

[U72] PHP：写错误日志
来源：http://www.share.fanxiaobao.xyz/Article/details/ghjrthwvp.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfiaybjho.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.fanxiaobao.xyz/Article/details/gsquidytl.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.fanxiaobao.xyz/Article/details/gndvhexjy.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxseumlb.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.fanxiaobao.xyz/Article/details/ggwzooxzf.sHtML

[U75] PHP：依赖注入
来源：http://baike.fanxiaobao.xyz/Article/details/gbhlbytxs.sHtML

composer require psr/container
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gitpzjnrl.sHtML

[U76] PHP：简单路由
来源：http://wap.fanxiaobao.xyz/Article/details/gaunyucgf.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzgylmeah.sHtML

[U77] PHP：模板渲染
来源：http://mobile.fanxiaobao.xyz/Article/details/gppnfjnlf.sHtML

composer require twig/twig
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqfgpurwu.sHtML

[U78] PHP：单元测试
来源：http://wap.fanxiaobao.xyz/Article/details/gduvcehvd.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.fanxiaobao.xyz/Article/details/gcsanqjnp.sHtML

[U79] PHP：静态分析
来源：http://wap.fanxiaobao.xyz/Article/details/gnvpxdhym.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.fanxiaobao.xyz/Article/details/gozjtwxqv.sHtML

[U80] PHP：代码规范修复
来源：http://blog.fanxiaobao.xyz/Article/details/glfkwbfuj.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.fanxiaobao.xyz/Article/details/glbmsipcg.sHtML

[U81] JS：初始化项目
来源：http://blog.fanxiaobao.xyz/Article/details/gkknkqpuf.sHtML

npm init -y;  npm i express
来源：http://mobile.fanxiaobao.xyz/Article/details/ghuhunrgn.sHtML

[U82] JS：package.json 脚本
来源：http://baike.fanxiaobao.xyz/Article/details/gkicigkua.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.fanxiaobao.xyz/Article/details/gkpmtvuuv.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.fanxiaobao.xyz/Article/details/geezswhrx.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.fanxiaobao.xyz/Article/details/gsrvewivx.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.fanxiaobao.xyz/Article/details/giitkvuzi.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.fanxiaobao.xyz/Article/details/gqlousnre.sHtML

[U85] JS：可选链
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfklzldsz.sHtML

a?.b?.c
来源：http://m.share.fanxiaobao.xyz/Article/details/gzfyyiuut.sHtML

[U86] JS：空值合并
来源：http://baike.fanxiaobao.xyz/Article/details/gfzcpsgph.sHtML

a ?? b
来源：http://wap.fanxiaobao.xyz/Article/details/gwttgigrj.sHtML

[U87] JS：解构默认值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpazdpnah.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbohjkvci.sHtML

[U88] JS：对象展开合并
来源：http://blog.fanxiaobao.xyz/Article/details/gyjzptdaq.sHtML

{ ...a, ...b }
来源：http://wap.fanxiaobao.xyz/Article/details/gmtmvekqn.sHtML

[U89] JS：数组去重
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqfqscei.sHtML

[...new Set(arr)]
来源：http://blog.fanxiaobao.xyz/Article/details/gwvcbkzay.sHtML

[U90] JS：数字数组排序
来源：http://baike.fanxiaobao.xyz/Article/details/gbllvfuin.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.fanxiaobao.xyz/Article/details/gzbsdnrhx.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmpyvjtig.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.fanxiaobao.xyz/Article/details/gdcxfykrb.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grlvlsccd.sHtML

structuredClone(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/grdwlthvu.sHtML

[U93] JS：模板字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gjcamkxrl.sHtML

`共 ${n} 条`
来源：http://3g.fanxiaobao.xyz/Article/details/gftcslzjq.sHtML

[U94] JS：箭头函数
来源：http://wap.fanxiaobao.xyz/Article/details/gfvfioybv.sHtML

const double = x => x * 2;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyifoyfrw.sHtML

[U95] JS：Promise 包装
来源：http://read.share.fanxiaobao.xyz/Article/details/gqtfpfvpn.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.fanxiaobao.xyz/Article/details/gcyacxzxc.sHtML

[U96] JS：async/await 与异常
来源：http://baike.fanxiaobao.xyz/Article/details/gmivcrowa.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbfyasujl.sHtML

[U97] JS：并发请求
来源：http://wap.fanxiaobao.xyz/Article/details/gvbeydzdr.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fanxiaobao.xyz/Article/details/gwvizwmqg.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gjfcsxcqc.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.fanxiaobao.xyz/Article/details/gyzdoroid.sHtML

[U99] JS：事件监听
来源：http://mobile.fanxiaobao.xyz/Article/details/gxglioyre.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvkmsuqiu.sHtML

[U100] JS：DOM 查询
来源：http://baike.fanxiaobao.xyz/Article/details/glfjkwfhe.sHtML

document.querySelector(".item")
来源：http://baike.fanxiaobao.xyz/Article/details/gddtsptsh.sHtML

[U101] JS：classList 操作
来源：http://3g.fanxiaobao.xyz/Article/details/gzmnpxmtb.sHtML

el.classList.toggle("active")
来源：http://3g.fanxiaobao.xyz/Article/details/gykxpaduw.sHtML

[U102] JS：本地存储
来源：http://mobile.fanxiaobao.xyz/Article/details/gkyaedubg.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdspctglr.sHtML

[U103] JS：定时器
来源：http://mobile.fanxiaobao.xyz/Article/details/goolcltgg.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnaydbhrv.sHtML

[U104] JS：防抖
来源：http://www.share.fanxiaobao.xyz/Article/details/grjwetwkb.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fanxiaobao.xyz/Article/details/gfnleurtz.sHtML

[U105] JS：节流
来源：http://read.share.fanxiaobao.xyz/Article/details/gamyelgar.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.fanxiaobao.xyz/Article/details/gldfahrnp.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkqenahav.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.fanxiaobao.xyz/Article/details/grrwiileg.sHtML

[U107] JS：数字千分位
来源：http://m.share.fanxiaobao.xyz/Article/details/gwndkqavo.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.fanxiaobao.xyz/Article/details/gdicyiusj.sHtML

[U108] JS：随机整数
来源：http://m.share.fanxiaobao.xyz/Article/details/gmznfjyza.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnlcltolg.sHtML

[U109] JS：数组分组
来源：http://blog.fanxiaobao.xyz/Article/details/gipmghhhw.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.fanxiaobao.xyz/Article/details/gebttxwpe.sHtML

[U110] JS：数组分块
来源：http://read.share.fanxiaobao.xyz/Article/details/gtwvszijm.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.fanxiaobao.xyz/Article/details/gjfglvsvk.sHtML

[U111] JS：对象转 Map
来源：http://m.share.fanxiaobao.xyz/Article/details/gkikxnlbz.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtumpgjcj.sHtML

[U112] JS：字符串补位
来源：http://baike.fanxiaobao.xyz/Article/details/gtddtbtyz.sHtML

"7".padStart(3, "0")
来源：http://blog.fanxiaobao.xyz/Article/details/gynxwizkb.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaoicwlcq.sHtML

s.replaceAll("a", "b")
来源：http://blog.fanxiaobao.xyz/Article/details/gbhrczhst.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gjmlakaan.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohxjdglg.sHtML

[U115] JS：生成 UUID
来源：http://baike.fanxiaobao.xyz/Article/details/gzqqonuoe.sHtML

crypto.randomUUID()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmhklddtt.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.fanxiaobao.xyz/Article/details/giafsjhob.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghejvwtns.sHtML

[U117] JS：单元测试
来源：http://www.share.fanxiaobao.xyz/Article/details/gfkuxfuij.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.fanxiaobao.xyz/Article/details/gwvuzjmvq.sHtML

[U118] JS：开发服务器
来源：http://www.share.fanxiaobao.xyz/Article/details/guiclvpgb.sHtML

npm i -D vite;  npx vite
来源：http://m.share.fanxiaobao.xyz/Article/details/girjsyzky.sHtML

[U119] JS：生产构建
来源：http://wap.fanxiaobao.xyz/Article/details/gwdiyglro.sHtML

npx vite build
来源：http://wap.fanxiaobao.xyz/Article/details/gjfbujxrr.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gshymatac.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.fanxiaobao.xyz/Article/details/gnpuaivvp.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gpiytlaqr.sHtML

统计汇总
来源：http://read.share.fanxiaobao.xyz/Article/details/ggwsvzkqy.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gvcxgpvzk.sHtML

按语言统计（条）：
来源：http://3g.fanxiaobao.xyz/Article/details/gslozpexo.sHtML

Python ......... 252
来源：http://read.share.fanxiaobao.xyz/Article/details/gthpujmuz.sHtML

PHP ............ 252
来源：http://3g.fanxiaobao.xyz/Article/details/gvfyshwhp.sHtML

JavaScript ..... 252
来源：http://www.share.fanxiaobao.xyz/Article/details/gzfuckhql.sHtML

TypeScript ..... 212
来源：http://3g.fanxiaobao.xyz/Article/details/gxvtgyryl.sHtML

Java ........... 212
来源：http://mobile.fanxiaobao.xyz/Article/details/girxzcjtw.sHtML

Go ............. 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gotfwymfn.sHtML

Ruby ........... 212
来源：http://wap.fanxiaobao.xyz/Article/details/gdcnovstx.sHtML

C# ............. 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqzkjrsqe.sHtML

C .............. 30
来源：http://mobile.fanxiaobao.xyz/Article/details/gxgmdcrqh.sHtML

C++ ............ 30
来源：http://3g.fanxiaobao.xyz/Article/details/gmwhzmciw.sHtML

SQL ............ 90
来源：http://baike.fanxiaobao.xyz/Article/details/gevsaqqkr.sHtML

Bash ........... 80
来源：http://wap.fanxiaobao.xyz/Article/details/gzvrnqkfu.sHtML

Kotlin ......... 15
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcnbkqbvw.sHtML

Swift .......... 15
来源：http://baike.fanxiaobao.xyz/Article/details/gebnphebe.sHtML

Lua ............ 10
来源：http://mobile.fanxiaobao.xyz/Article/details/gifxqlore.sHtML

Perl ........... 10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/getgpeqlf.sHtML

Scala .......... 10
来源：http://baike.fanxiaobao.xyz/Article/details/gvsiszpjf.sHtML

------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/ggspwsfyo.sHtML

合计 ........... 2106 条
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcwppbcba.sHtML

按章节统计：
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdwoojstq.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.fanxiaobao.xyz/Article/details/gglrkjkyi.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.fanxiaobao.xyz/Article/details/grwrdamnz.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.fanxiaobao.xyz/Article/details/gshijemxb.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.fanxiaobao.xyz/Article/details/ggdsdtwol.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.fanxiaobao.xyz/Article/details/gybrtcmoz.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.fanxiaobao.xyz/Article/details/gbnnddxyo.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.fanxiaobao.xyz/Article/details/gutgnweyl.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gczrqpamt.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/gekqbymjg.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.fanxiaobao.xyz/Article/details/guekvgwnm.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gzovsrrig.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnssguvkz.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/gcceqlrqo.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.fanxiaobao.xyz/Article/details/griiiloww.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.fanxiaobao.xyz/Article/details/gjevokszk.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/guhvtzrrq.sHtML

Q SQL 专题                              90
来源：http://blog.fanxiaobao.xyz/Article/details/gyadlnqjt.sHtML

R Bash 专题                             80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtmpidnpc.sHtML

S C / C++ 专题                          60
来源：http://m.share.fanxiaobao.xyz/Article/details/gmyhhflqb.sHtML

T 其他语言补充                          60
来源：http://wap.fanxiaobao.xyz/Article/details/gizinzpmd.sHtML

U 高频实用片段                         120
来源：http://baike.fanxiaobao.xyz/Article/details/gqlojsqnr.sHtML

------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/gflqslmaa.sHtML

合计                                  2106 条
来源：http://www.blog.fanxiaobao.xyz/Article/details/gppbeoxrg.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/gdjbssodf.sHtML


<!-- 参考信息 -->