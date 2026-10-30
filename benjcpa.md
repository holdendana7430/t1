代发 wailian999

val a = 1;  var b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gdytpsclv.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkbiyrwlp.sHtML

s"值: $b"
来源：http://wap.fanxiaobao.xyz/Article/details/gqqeojnzm.sHtML

[T54] Scala：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/gdkeowtip.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsnqhrjef.sHtML

[T55] Scala：集合过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gjvgzrsly.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gnqucyotn.sHtML

[T56] Scala：样例类
来源：http://www.blog.fanxiaobao.xyz/Article/details/grkfqxovl.sHtML

case class User(name: String, age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/gclicjwpp.sHtML

[T57] Scala：模式匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gnixwibww.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjoforsjj.sHtML

[T58] Scala：函数定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gnxqqfzsc.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.fanxiaobao.xyz/Article/details/gqenbcjve.sHtML

[T59] Scala：循环
来源：http://blog.fanxiaobao.xyz/Article/details/gtuuogdjx.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbtehrkfg.sHtML

[T60] Scala：折叠
来源：http://www.share.fanxiaobao.xyz/Article/details/gyqaadral.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.fanxiaobao.xyz/Article/details/gtizmdlgg.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gakgslccv.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gcwaquije.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/ggdlxwcwr.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.fanxiaobao.xyz/Article/details/giwuvbfli.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghcecjjaq.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fanxiaobao.xyz/Article/details/gbklxydob.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gggmfaapz.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.fanxiaobao.xyz/Article/details/gpkpdfhtt.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.fanxiaobao.xyz/Article/details/gqyyjhgna.sHtML

[U04] Py：变量调试打印
来源：http://www.share.fanxiaobao.xyz/Article/details/gvvkrbkmz.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gydmgyzgh.sHtML

[U05] Py：列表去重且保序
来源：http://baike.fanxiaobao.xyz/Article/details/gpelqwxos.sHtML

list(dict.fromkeys(arr))
来源：http://3g.fanxiaobao.xyz/Article/details/gzfbxcvyi.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gejbcxqtm.sHtML

{**a, **b}
来源：http://m.share.fanxiaobao.xyz/Article/details/gybtjcwgk.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtmtcfulh.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fanxiaobao.xyz/Article/details/gdegzxnwz.sHtML

[U08] Py：展平二维列表
来源：http://read.share.fanxiaobao.xyz/Article/details/guzmcpogm.sHtML

[y for x in nested for y in x]
来源：http://baike.fanxiaobao.xyz/Article/details/glimofpgz.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.fanxiaobao.xyz/Article/details/gubhrdaaq.sHtML

max(d, key=d.get)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grfsqepdh.sHtML

[U10] Py：按值排序字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gwpdxhgzb.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.fanxiaobao.xyz/Article/details/gghwgnpvj.sHtML

[U11] Py：生成器表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gfnxrrtmk.sHtML

(x * 2 for x in arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gguzdcqct.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gbuhljjwk.sHtML

Counter(arr).most_common(3)
来源：http://baike.fanxiaobao.xyz/Article/details/grigjrcxk.sHtML

[U13] Py：固定长度队列
来源：http://www.share.fanxiaobao.xyz/Article/details/gremmmdsk.sHtML

deque(maxlen=10)
来源：http://www.share.fanxiaobao.xyz/Article/details/gddvudlpm.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.fanxiaobao.xyz/Article/details/ghztumhir.sHtML

defaultdict(list)
来源：http://blog.fanxiaobao.xyz/Article/details/grhxzpbdd.sHtML

[U15] Py：高精度计时
来源：http://blog.fanxiaobao.xyz/Article/details/glznadnqh.sHtML

t = time.perf_counter()
来源：http://mobile.fanxiaobao.xyz/Article/details/gzhnxltob.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fanxiaobao.xyz/Article/details/gkubvsyzs.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.fanxiaobao.xyz/Article/details/gzgrgzqki.sHtML

[U17] Py：初始化日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gxglohivp.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.fanxiaobao.xyz/Article/details/gtlnwexeb.sHtML

[U18] Py：预编译正则
来源：http://mobile.fanxiaobao.xyz/Article/details/gcjicwjpt.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcnkisgcu.sHtML

[U19] Py：正则替换带回调
来源：http://3g.fanxiaobao.xyz/Article/details/gqqixvpeq.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.fanxiaobao.xyz/Article/details/gpqaxbyrx.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmswnywyz.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.fanxiaobao.xyz/Article/details/gabwgzyyh.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.fanxiaobao.xyz/Article/details/gdmsmrgqa.sHtML

@contextlib.contextmanager
来源：http://www.blog.fanxiaobao.xyz/Article/details/gezgxxsgp.sHtML

[U22] Py：矩阵转置
来源：http://mobile.fanxiaobao.xyz/Article/details/ggtxlfsmt.sHtML

list(zip(*m))
来源：http://www.blog.fanxiaobao.xyz/Article/details/grgdkuzel.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gkzjfmzee.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.fanxiaobao.xyz/Article/details/glsaeqolf.sHtML

[U24] Py：路径操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gtlnwrgfe.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmcnimgbs.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.fanxiaobao.xyz/Article/details/gvzdsintr.sHtML

csv.DictReader(f)
来源：http://baike.fanxiaobao.xyz/Article/details/gofwursjy.sHtML

[U26] Py：并发下载
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gurcckyzs.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxhnlwfye.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.fanxiaobao.xyz/Article/details/gorhbkkly.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.fanxiaobao.xyz/Article/details/gakzxkhyf.sHtML

[U28] Py：类型别名
来源：http://blog.fanxiaobao.xyz/Article/details/gqrbxfrxp.sHtML

UserId = int
来源：http://wap.fanxiaobao.xyz/Article/details/gsgvvxcmx.sHtML

[U29] Py：属性校验
来源：http://wap.fanxiaobao.xyz/Article/details/gnlsteayd.sHtML

@property 与 @x.setter 配合
来源：http://blog.fanxiaobao.xyz/Article/details/gizsxujhg.sHtML

[U30] Py：数据类
来源：http://blog.fanxiaobao.xyz/Article/details/gmuohykja.sHtML

@dataclass(slots=True)
来源：http://baike.fanxiaobao.xyz/Article/details/giwnnlmke.sHtML

[U31] Py：单测
来源：http://blog.fanxiaobao.xyz/Article/details/gjhxspfll.sHtML

python -m pytest -q
来源：http://m.share.fanxiaobao.xyz/Article/details/gyoxhsizg.sHtML

[U32] Py：代码格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gsffktcql.sHtML

ruff format . && ruff check --fix .
来源：http://blog.fanxiaobao.xyz/Article/details/glpvlrtva.sHtML

[U33] Py：打包发布
来源：http://blog.fanxiaobao.xyz/Article/details/gnahbgwfq.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.fanxiaobao.xyz/Article/details/gpypyswix.sHtML

[U34] Py：判断编码
来源：http://mobile.fanxiaobao.xyz/Article/details/gvqldjhjm.sHtML

chardet.detect(raw)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdnljywrf.sHtML

[U35] Py：发送邮件
来源：http://mobile.fanxiaobao.xyz/Article/details/ghbsbyudz.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.fanxiaobao.xyz/Article/details/gypuijvza.sHtML

[U36] Py：定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/gyyzgpnna.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grarxsjjr.sHtML

[U37] Py：读写 Excel
来源：http://mobile.fanxiaobao.xyz/Article/details/gjihbpqjx.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.fanxiaobao.xyz/Article/details/gadrgmbxd.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.fanxiaobao.xyz/Article/details/gumdjrnus.sHtML

Path(__file__).resolve().parent
来源：http://wap.fanxiaobao.xyz/Article/details/gshnxwbzc.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gckljcagz.sHtML

sys.stdout.isatty()
来源：http://baike.fanxiaobao.xyz/Article/details/gpllyxfaa.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.fanxiaobao.xyz/Article/details/galnjwwga.sHtML

print("err", file=sys.stderr)
来源：http://blog.fanxiaobao.xyz/Article/details/guvdnkutl.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.fanxiaobao.xyz/Article/details/gadmjxjix.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.fanxiaobao.xyz/Article/details/gvbfbfnaf.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjkimyvwv.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gogkrtkiz.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxhucogek.sHtML

namespace App\Http;
来源：http://baike.fanxiaobao.xyz/Article/details/gvjyiqjpt.sHtML

[U44] PHP：开启严格类型
来源：http://baike.fanxiaobao.xyz/Article/details/gdrkaixtd.sHtML

declare(strict_types=1);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdnfuzopp.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gahrrhxrz.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtocisnsr.sHtML

[U46] PHP：可空类型
来源：http://blog.fanxiaobao.xyz/Article/details/gqwxufpyh.sHtML

?string $name = null
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glfbrhwvd.sHtML

[U47] PHP：联合类型
来源：http://blog.fanxiaobao.xyz/Article/details/gezylhfjq.sHtML

int|string $id
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gozusoijv.sHtML

[U48] PHP：纯枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gcuylmybd.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gjizqtqqh.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtppthikn.sHtML

public readonly string $name
来源：http://mobile.fanxiaobao.xyz/Article/details/grcxalhbw.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.fanxiaobao.xyz/Article/details/gfkuuunei.sHtML

public function __construct(private int $id) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gllqrgcpi.sHtML

[U51] PHP：数组解构
来源：http://m.share.fanxiaobao.xyz/Article/details/gdudpmxve.sHtML

[$a, $b] = $arr;
来源：http://wap.fanxiaobao.xyz/Article/details/gmoqnnhyl.sHtML

[U52] PHP：箭头函数
来源：http://wap.fanxiaobao.xyz/Article/details/gupwnybdh.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.fanxiaobao.xyz/Article/details/gxlwwoyyv.sHtML

[U53] PHP：空合并运算符
来源：http://3g.fanxiaobao.xyz/Article/details/gsbuslxvr.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.fanxiaobao.xyz/Article/details/gzpjrmhkp.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzexrwnqe.sHtML

$obj?->method()
来源：http://read.share.fanxiaobao.xyz/Article/details/ggbipouaw.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ginaqewqv.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.fanxiaobao.xyz/Article/details/gqttzpfqo.sHtML

[U56] PHP：命名参数
来源：http://blog.fanxiaobao.xyz/Article/details/gcghgcutx.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcsrkspnn.sHtML

[U57] PHP：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/ggvrjputu.sHtML

"值: {$a}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gfgboaqzz.sHtML

[U58] PHP：数组三件套
来源：http://www.share.fanxiaobao.xyz/Article/details/gtvmhnxjl.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.fanxiaobao.xyz/Article/details/ganlatewy.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gftcvuznn.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtqqhbgiu.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.fanxiaobao.xyz/Article/details/gzajctrly.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.fanxiaobao.xyz/Article/details/grkcxekmk.sHtML

[U61] PHP：正则
来源：http://mobile.fanxiaobao.xyz/Article/details/grzokulln.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmeuyujkl.sHtML

[U62] PHP：日期对象
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzwxrtcgs.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.fanxiaobao.xyz/Article/details/gcytudtlr.sHtML

[U63] PHP：文件读写
来源：http://blog.fanxiaobao.xyz/Article/details/gabrabbbr.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.fanxiaobao.xyz/Article/details/gwgeqfrow.sHtML

[U64] PHP：目录遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gewhcevys.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghputpdoo.sHtML

[U65] PHP：会话
来源：http://m.share.fanxiaobao.xyz/Article/details/gzhdmpggf.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwceyihrd.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.fanxiaobao.xyz/Article/details/gqnyhhfkb.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmscacssa.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.fanxiaobao.xyz/Article/details/gneepvihy.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.fanxiaobao.xyz/Article/details/gomjihefg.sHtML

[U68] PHP：PDO 连接
来源：http://wap.fanxiaobao.xyz/Article/details/gbrzxxxhp.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyxjsyhmc.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpowqnosj.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.fanxiaobao.xyz/Article/details/gufmopbhe.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnzrxbwzp.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.fanxiaobao.xyz/Article/details/gxdvgdtjq.sHtML

[U71] PHP：抛出异常
来源：http://blog.fanxiaobao.xyz/Article/details/gawjqmlnu.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.fanxiaobao.xyz/Article/details/gmxvaeyaa.sHtML

[U72] PHP：写错误日志
来源：http://mobile.fanxiaobao.xyz/Article/details/ghxencllt.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.fanxiaobao.xyz/Article/details/gmbrsgxfv.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.fanxiaobao.xyz/Article/details/gqeaduvzd.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.fanxiaobao.xyz/Article/details/gvbghiwml.sHtML

[U74] PHP：读取环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/gtoydiodt.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.fanxiaobao.xyz/Article/details/gzysrsmoo.sHtML

[U75] PHP：依赖注入
来源：http://baike.fanxiaobao.xyz/Article/details/gglguwbdf.sHtML

composer require psr/container
来源：http://m.share.fanxiaobao.xyz/Article/details/gckjltsfq.sHtML

[U76] PHP：简单路由
来源：http://m.share.fanxiaobao.xyz/Article/details/gtcqqqhru.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grhjlouzy.sHtML

[U77] PHP：模板渲染
来源：http://baike.fanxiaobao.xyz/Article/details/ghltothlg.sHtML

composer require twig/twig
来源：http://blog.fanxiaobao.xyz/Article/details/gunsqbkcj.sHtML

[U78] PHP：单元测试
来源：http://3g.fanxiaobao.xyz/Article/details/gteaprdds.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grodtbgcn.sHtML

[U79] PHP：静态分析
来源：http://read.share.fanxiaobao.xyz/Article/details/geazbotxy.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.fanxiaobao.xyz/Article/details/gpbpsaejg.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.fanxiaobao.xyz/Article/details/goeidqbsc.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.fanxiaobao.xyz/Article/details/gvkreuyvu.sHtML

[U81] JS：初始化项目
来源：http://mobile.fanxiaobao.xyz/Article/details/glzlulgao.sHtML

npm init -y;  npm i express
来源：http://mobile.fanxiaobao.xyz/Article/details/ggtlbvsor.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzrgysuty.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gazzjpnvs.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.fanxiaobao.xyz/Article/details/gnajpvdwp.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfsnonwul.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.fanxiaobao.xyz/Article/details/ggjbplidp.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.fanxiaobao.xyz/Article/details/gadwuqvlc.sHtML

[U85] JS：可选链
来源：http://m.share.fanxiaobao.xyz/Article/details/gsaehlqrr.sHtML

a?.b?.c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwfvvxvgd.sHtML

[U86] JS：空值合并
来源：http://read.share.fanxiaobao.xyz/Article/details/gllpbstod.sHtML

a ?? b
来源：http://read.share.fanxiaobao.xyz/Article/details/gnjvjdjls.sHtML

[U87] JS：解构默认值
来源：http://baike.fanxiaobao.xyz/Article/details/gvpvhzvbk.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gefieaesl.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqinhaszb.sHtML

{ ...a, ...b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbzzttedx.sHtML

[U89] JS：数组去重
来源：http://www.share.fanxiaobao.xyz/Article/details/gdwhkweqg.sHtML

[...new Set(arr)]
来源：http://baike.fanxiaobao.xyz/Article/details/gpymsapyl.sHtML

[U90] JS：数字数组排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gkxpsqmpf.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.fanxiaobao.xyz/Article/details/gidfqxsjx.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfnqutgte.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.fanxiaobao.xyz/Article/details/gnkzffsge.sHtML

[U92] JS：深拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvjbqjcji.sHtML

structuredClone(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gyfgqaebt.sHtML

[U93] JS：模板字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gkcqozvfe.sHtML

`共 ${n} 条`
来源：http://3g.fanxiaobao.xyz/Article/details/gkfdibltf.sHtML

[U94] JS：箭头函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gbnwuaqgn.sHtML

const double = x => x * 2;
来源：http://wap.fanxiaobao.xyz/Article/details/gnzyvlgxl.sHtML

[U95] JS：Promise 包装
来源：http://wap.fanxiaobao.xyz/Article/details/gjnomuezw.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcebhdnsh.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.fanxiaobao.xyz/Article/details/gievejyek.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.fanxiaobao.xyz/Article/details/grutrzojd.sHtML

[U97] JS：并发请求
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grkywwwaz.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fanxiaobao.xyz/Article/details/gtsexhghq.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdxxvzrcq.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.fanxiaobao.xyz/Article/details/gvvzhormo.sHtML

[U99] JS：事件监听
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjekukbyk.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.fanxiaobao.xyz/Article/details/gligdmojt.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggaeqtgku.sHtML

document.querySelector(".item")
来源：http://3g.fanxiaobao.xyz/Article/details/gaedhgchg.sHtML

[U101] JS：classList 操作
来源：http://blog.fanxiaobao.xyz/Article/details/gyfvfvkgf.sHtML

el.classList.toggle("active")
来源：http://m.share.fanxiaobao.xyz/Article/details/gswbpugai.sHtML

[U102] JS：本地存储
来源：http://3g.fanxiaobao.xyz/Article/details/gjzuvuwnb.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.fanxiaobao.xyz/Article/details/gqhtztrwo.sHtML

[U103] JS：定时器
来源：http://blog.fanxiaobao.xyz/Article/details/gzwidbhho.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.fanxiaobao.xyz/Article/details/gfizioiaa.sHtML

[U104] JS：防抖
来源：http://www.share.fanxiaobao.xyz/Article/details/gctukhcap.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fanxiaobao.xyz/Article/details/gvllvwevm.sHtML

[U105] JS：节流
来源：http://mobile.fanxiaobao.xyz/Article/details/guzmybnrp.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.fanxiaobao.xyz/Article/details/gazfszopc.sHtML

[U106] JS：日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gejfxlcqg.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.fanxiaobao.xyz/Article/details/gqdvpnruf.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjtfidsqp.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grngafatc.sHtML

[U108] JS：随机整数
来源：http://read.share.fanxiaobao.xyz/Article/details/gjorqvwgr.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.fanxiaobao.xyz/Article/details/gfcnxcctn.sHtML

[U109] JS：数组分组
来源：http://baike.fanxiaobao.xyz/Article/details/gaputwtnw.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.fanxiaobao.xyz/Article/details/gpyxyqraa.sHtML

[U110] JS：数组分块
来源：http://www.share.fanxiaobao.xyz/Article/details/gshroqqwa.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.fanxiaobao.xyz/Article/details/gvdxfieof.sHtML

[U111] JS：对象转 Map
来源：http://read.share.fanxiaobao.xyz/Article/details/gmqbsynqf.sHtML

new Map(Object.entries(obj))
来源：http://3g.fanxiaobao.xyz/Article/details/gxlnsfvcn.sHtML

[U112] JS：字符串补位
来源：http://www.share.fanxiaobao.xyz/Article/details/ghjnottnk.sHtML

"7".padStart(3, "0")
来源：http://wap.fanxiaobao.xyz/Article/details/gbkpebpbv.sHtML

[U113] JS：正则替换全部
来源：http://wap.fanxiaobao.xyz/Article/details/gewcnpiil.sHtML

s.replaceAll("a", "b")
来源：http://baike.fanxiaobao.xyz/Article/details/gmvqgeufr.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gwjwgvnoa.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxjvwpfak.sHtML

[U115] JS：生成 UUID
来源：http://3g.fanxiaobao.xyz/Article/details/gwfntqety.sHtML

crypto.randomUUID()
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggbaibfem.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnaxekfiv.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gxaabapke.sHtML

[U117] JS：单元测试
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsfficoqb.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.fanxiaobao.xyz/Article/details/gpqacrgtf.sHtML

[U118] JS：开发服务器
来源：http://mobile.fanxiaobao.xyz/Article/details/gwqrelktl.sHtML

npm i -D vite;  npx vite
来源：http://wap.fanxiaobao.xyz/Article/details/gsnoinzni.sHtML

[U119] JS：生产构建
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqcjybzig.sHtML

npx vite build
来源：http://mobile.fanxiaobao.xyz/Article/details/gzygbplnc.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbvpopepa.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.fanxiaobao.xyz/Article/details/gyaewednw.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gyltivqxu.sHtML

统计汇总
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtszyfcyy.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gwdbczwcz.sHtML

按语言统计（条）：
来源：http://mobile.fanxiaobao.xyz/Article/details/ghckerhlr.sHtML

Python ......... 252
来源：http://mobile.fanxiaobao.xyz/Article/details/gvjmavllh.sHtML

PHP ............ 252
来源：http://baike.fanxiaobao.xyz/Article/details/gdsorlitr.sHtML

JavaScript ..... 252
来源：http://wap.fanxiaobao.xyz/Article/details/glnlxygml.sHtML

TypeScript ..... 212
来源：http://blog.fanxiaobao.xyz/Article/details/gchxcseqe.sHtML

Java ........... 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gozqmcmjp.sHtML

Go ............. 212
来源：http://blog.fanxiaobao.xyz/Article/details/gboqrhvuo.sHtML

Ruby ........... 212
来源：http://m.share.fanxiaobao.xyz/Article/details/ghhvynoph.sHtML

C# ............. 212
来源：http://blog.fanxiaobao.xyz/Article/details/gkxjvhtuv.sHtML

C .............. 30
来源：http://www.share.fanxiaobao.xyz/Article/details/gpphnxdju.sHtML

C++ ............ 30
来源：http://baike.fanxiaobao.xyz/Article/details/gleiztfbk.sHtML

SQL ............ 90
来源：http://read.share.fanxiaobao.xyz/Article/details/gilyzganc.sHtML

Bash ........... 80
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnxtsvmbe.sHtML

Kotlin ......... 15
来源：http://baike.fanxiaobao.xyz/Article/details/gdfudmubk.sHtML

Swift .......... 15
来源：http://baike.fanxiaobao.xyz/Article/details/gjhhaqked.sHtML

Lua ............ 10
来源：http://baike.fanxiaobao.xyz/Article/details/gowtdapxr.sHtML

Perl ........... 10
来源：http://m.share.fanxiaobao.xyz/Article/details/gthjcates.sHtML

Scala .......... 10
来源：http://mobile.fanxiaobao.xyz/Article/details/gfsozpbpm.sHtML

------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/grahedsud.sHtML

合计 ........... 2106 条
来源：http://baike.fanxiaobao.xyz/Article/details/gzgttmiet.sHtML

按章节统计：
来源：http://baike.fanxiaobao.xyz/Article/details/gpuzvcvrw.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyvuswswt.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.fanxiaobao.xyz/Article/details/gdudvlhxi.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.fanxiaobao.xyz/Article/details/gftjlsegi.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.fanxiaobao.xyz/Article/details/gtkwuxwmm.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.fanxiaobao.xyz/Article/details/gndaynohe.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.fanxiaobao.xyz/Article/details/gqjtheevv.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.fanxiaobao.xyz/Article/details/gacuzfwvd.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzsjsualy.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/gspagmqdq.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guvzpfbkk.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gpbicldqa.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gcnffouub.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gmxemomuf.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.fanxiaobao.xyz/Article/details/gtamvmtis.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.fanxiaobao.xyz/Article/details/gruxbsugf.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gvkcwsbmu.sHtML


<!-- 参考信息 -->