代发 wailian999

case class User(name: String, age: Int)
来源：http://www.share.fanxiaobao.xyz/Article/details/grdyktksc.sHtML

[T57] Scala：模式匹配
来源：http://blog.fanxiaobao.xyz/Article/details/ggwofotqd.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghgdwtrml.sHtML

[T58] Scala：函数定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gqzkvdhmi.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.fanxiaobao.xyz/Article/details/gycodujwr.sHtML

[T59] Scala：循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmpuljbad.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.fanxiaobao.xyz/Article/details/gndzxswox.sHtML

[T60] Scala：折叠
来源：http://m.share.fanxiaobao.xyz/Article/details/gcybxknod.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvoyvitrq.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/giwzgcozz.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gqlmfqzfm.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gfizfpvcd.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.fanxiaobao.xyz/Article/details/gjikyqkyb.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.fanxiaobao.xyz/Article/details/gpmizmeiv.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.fanxiaobao.xyz/Article/details/gszblefjj.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gihovembw.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.fanxiaobao.xyz/Article/details/gpcvfgofg.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.fanxiaobao.xyz/Article/details/gmglvlvdg.sHtML

[U04] Py：变量调试打印
来源：http://mobile.fanxiaobao.xyz/Article/details/gleynkurb.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzjxzvbcc.sHtML

[U05] Py：列表去重且保序
来源：http://wap.fanxiaobao.xyz/Article/details/gntqbzwtb.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdyzhmern.sHtML

[U06] Py：合并两个字典
来源：http://m.share.fanxiaobao.xyz/Article/details/gttiuyebb.sHtML

{**a, **b}
来源：http://read.share.fanxiaobao.xyz/Article/details/gxkqplfki.sHtML

[U07] Py：反转字典键值
来源：http://3g.fanxiaobao.xyz/Article/details/gcasrjtcd.sHtML

{v: k for k, v in d.items()}
来源：http://baike.fanxiaobao.xyz/Article/details/gvzhekrbb.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpekojfbv.sHtML

[y for x in nested for y in x]
来源：http://blog.fanxiaobao.xyz/Article/details/gbrfkxmpq.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.fanxiaobao.xyz/Article/details/gjxwfxmpu.sHtML

max(d, key=d.get)
来源：http://mobile.fanxiaobao.xyz/Article/details/guuyploso.sHtML

[U10] Py：按值排序字典
来源：http://blog.fanxiaobao.xyz/Article/details/grdpdrlzc.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.fanxiaobao.xyz/Article/details/gwzoovrxy.sHtML

[U11] Py：生成器表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gpedoyhtu.sHtML

(x * 2 for x in arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gnsuykdga.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.fanxiaobao.xyz/Article/details/gvufdaqnw.sHtML

Counter(arr).most_common(3)
来源：http://blog.fanxiaobao.xyz/Article/details/gjbwxjznr.sHtML

[U13] Py：固定长度队列
来源：http://m.share.fanxiaobao.xyz/Article/details/gsawgzlsg.sHtML

deque(maxlen=10)
来源：http://wap.fanxiaobao.xyz/Article/details/gstbzonsn.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.fanxiaobao.xyz/Article/details/gwazjiajo.sHtML

defaultdict(list)
来源：http://wap.fanxiaobao.xyz/Article/details/glvvljftk.sHtML

[U15] Py：高精度计时
来源：http://3g.fanxiaobao.xyz/Article/details/gvspovrjf.sHtML

t = time.perf_counter()
来源：http://blog.fanxiaobao.xyz/Article/details/gqsiqlpgn.sHtML

[U16] Py：命令行参数解析
来源：http://wap.fanxiaobao.xyz/Article/details/gsbuszzts.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkbaqzryt.sHtML

[U17] Py：初始化日志
来源：http://read.share.fanxiaobao.xyz/Article/details/goscyiqkd.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.fanxiaobao.xyz/Article/details/gqlcvyjsn.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grqxcxyer.sHtML

pat = re.compile(r"\d+")
来源：http://wap.fanxiaobao.xyz/Article/details/gxvmnvejt.sHtML

[U19] Py：正则替换带回调
来源：http://3g.fanxiaobao.xyz/Article/details/ginqdnpnc.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkxswiypf.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.fanxiaobao.xyz/Article/details/givcxfrmb.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.fanxiaobao.xyz/Article/details/gyntywjft.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.fanxiaobao.xyz/Article/details/gwvqxpmzf.sHtML

@contextlib.contextmanager
来源：http://mobile.fanxiaobao.xyz/Article/details/gllrrmfnu.sHtML

[U22] Py：矩阵转置
来源：http://www.share.fanxiaobao.xyz/Article/details/gvzztflzc.sHtML

list(zip(*m))
来源：http://baike.fanxiaobao.xyz/Article/details/gjadkfiyq.sHtML

[U23] Py：分块读取大文件
来源：http://3g.fanxiaobao.xyz/Article/details/grjgtfety.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.fanxiaobao.xyz/Article/details/gebbowkcu.sHtML

[U24] Py：路径操作
来源：http://m.share.fanxiaobao.xyz/Article/details/ggmzzggun.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkptkijyr.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.fanxiaobao.xyz/Article/details/gyluqzcby.sHtML

csv.DictReader(f)
来源：http://baike.fanxiaobao.xyz/Article/details/gonyfxemx.sHtML

[U26] Py：并发下载
来源：http://blog.fanxiaobao.xyz/Article/details/ggmpgkzly.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.fanxiaobao.xyz/Article/details/gmvmvyvni.sHtML

[U27] Py：异步 HTTP
来源：http://wap.fanxiaobao.xyz/Article/details/gudpwzwmx.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.fanxiaobao.xyz/Article/details/gwdrjuwjf.sHtML

[U28] Py：类型别名
来源：http://read.share.fanxiaobao.xyz/Article/details/gvtxikqfn.sHtML

UserId = int
来源：http://m.share.fanxiaobao.xyz/Article/details/gegylopqw.sHtML

[U29] Py：属性校验
来源：http://baike.fanxiaobao.xyz/Article/details/gbvzypmbi.sHtML

@property 与 @x.setter 配合
来源：http://wap.fanxiaobao.xyz/Article/details/gwiabdtlr.sHtML

[U30] Py：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/gkmdnsfpl.sHtML

@dataclass(slots=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvbbhnyrx.sHtML

[U31] Py：单测
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqorludoj.sHtML

python -m pytest -q
来源：http://m.share.fanxiaobao.xyz/Article/details/gaobdixix.sHtML

[U32] Py：代码格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gbegeaail.sHtML

ruff format . && ruff check --fix .
来源：http://baike.fanxiaobao.xyz/Article/details/ghqyflgfp.sHtML

[U33] Py：打包发布
来源：http://wap.fanxiaobao.xyz/Article/details/gbbwuwwyu.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcgqxjhgt.sHtML

[U34] Py：判断编码
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghlrcwpdh.sHtML

chardet.detect(raw)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzraonzle.sHtML

[U35] Py：发送邮件
来源：http://mobile.fanxiaobao.xyz/Article/details/geszwiucp.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.fanxiaobao.xyz/Article/details/gibbxafyd.sHtML

[U36] Py：定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/gytuddzjn.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.fanxiaobao.xyz/Article/details/geeykbcpg.sHtML

[U37] Py：读写 Excel
来源：http://read.share.fanxiaobao.xyz/Article/details/gdphbbdsr.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.fanxiaobao.xyz/Article/details/gjdohzbvs.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.fanxiaobao.xyz/Article/details/gehvqjjox.sHtML

Path(__file__).resolve().parent
来源：http://www.share.fanxiaobao.xyz/Article/details/giogloxjq.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdaknidwj.sHtML

sys.stdout.isatty()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grapiftaq.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.fanxiaobao.xyz/Article/details/gjnugdzqk.sHtML

print("err", file=sys.stderr)
来源：http://m.share.fanxiaobao.xyz/Article/details/giessktkg.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.fanxiaobao.xyz/Article/details/gjwnxmldp.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.fanxiaobao.xyz/Article/details/ghosaogwv.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtgubliku.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggclueivk.sHtML

[U43] PHP：声明命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/gahyrnitc.sHtML

namespace App\Http;
来源：http://mobile.fanxiaobao.xyz/Article/details/grbxwwsui.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.fanxiaobao.xyz/Article/details/glrsmxtym.sHtML

declare(strict_types=1);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqpmeoefy.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gjpknfrci.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjmebloer.sHtML

[U46] PHP：可空类型
来源：http://mobile.fanxiaobao.xyz/Article/details/ghgcpdzcr.sHtML

?string $name = null
来源：http://read.share.fanxiaobao.xyz/Article/details/gfkqwlmnw.sHtML

[U47] PHP：联合类型
来源：http://wap.fanxiaobao.xyz/Article/details/ggsmvryve.sHtML

int|string $id
来源：http://www.share.fanxiaobao.xyz/Article/details/gjgahomig.sHtML

[U48] PHP：纯枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gpjgpgnig.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.fanxiaobao.xyz/Article/details/glrlxtqmi.sHtML

[U49] PHP：只读属性
来源：http://m.share.fanxiaobao.xyz/Article/details/gveqgsdxu.sHtML

public readonly string $name
来源：http://blog.fanxiaobao.xyz/Article/details/gppjvfean.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.fanxiaobao.xyz/Article/details/gjkoebapo.sHtML

public function __construct(private int $id) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/giixywije.sHtML

[U51] PHP：数组解构
来源：http://baike.fanxiaobao.xyz/Article/details/gujytfjng.sHtML

[$a, $b] = $arr;
来源：http://read.share.fanxiaobao.xyz/Article/details/gadiaqlrd.sHtML

[U52] PHP：箭头函数
来源：http://blog.fanxiaobao.xyz/Article/details/gdjjhzbns.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwqcypakg.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.fanxiaobao.xyz/Article/details/gcrcmiiyn.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.fanxiaobao.xyz/Article/details/gnyvinsjh.sHtML

[U54] PHP：空安全调用
来源：http://m.share.fanxiaobao.xyz/Article/details/gwbqdvihw.sHtML

$obj?->method()
来源：http://m.share.fanxiaobao.xyz/Article/details/gaivmybhm.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/glwxcptrj.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.fanxiaobao.xyz/Article/details/ggpadbslf.sHtML

[U56] PHP：命名参数
来源：http://wap.fanxiaobao.xyz/Article/details/gksbnliej.sHtML

f(a: 1, b: 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gdjugnwex.sHtML

[U57] PHP：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gzikemnjz.sHtML

"值: {$a}"
来源：http://blog.fanxiaobao.xyz/Article/details/gaupiykib.sHtML

[U58] PHP：数组三件套
来源：http://read.share.fanxiaobao.xyz/Article/details/gzpuvsufc.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbjbgdgon.sHtML

[U59] PHP：自定义排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gncgannfn.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fanxiaobao.xyz/Article/details/gfjtvdhzl.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.fanxiaobao.xyz/Article/details/gcsdyekoc.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.fanxiaobao.xyz/Article/details/giiimwepq.sHtML

[U61] PHP：正则
来源：http://blog.fanxiaobao.xyz/Article/details/gmesecxxf.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.fanxiaobao.xyz/Article/details/goorpsplf.sHtML

[U62] PHP：日期对象
来源：http://read.share.fanxiaobao.xyz/Article/details/gfkisiedn.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.fanxiaobao.xyz/Article/details/gfvyqhwpy.sHtML

[U63] PHP：文件读写
来源：http://3g.fanxiaobao.xyz/Article/details/gnbejxszp.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gozsldjdw.sHtML

[U64] PHP：目录遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gkgoafajc.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzyvafftx.sHtML

[U65] PHP：会话
来源：http://read.share.fanxiaobao.xyz/Article/details/gnfeytlgt.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqafjzgpk.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.fanxiaobao.xyz/Article/details/grkqgvinr.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.fanxiaobao.xyz/Article/details/gsxqrobnv.sHtML

[U67] PHP：处理文件上传
来源：http://3g.fanxiaobao.xyz/Article/details/gmuzytwhg.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcqwafwfo.sHtML

[U68] PHP：PDO 连接
来源：http://wap.fanxiaobao.xyz/Article/details/gdvlzaqrh.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjelbwvjv.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.fanxiaobao.xyz/Article/details/grnbtfsug.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gjaggfmaz.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gjjzkpyuh.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.fanxiaobao.xyz/Article/details/gypqquhuc.sHtML

[U71] PHP：抛出异常
来源：http://www.share.fanxiaobao.xyz/Article/details/gwuhewmnc.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.fanxiaobao.xyz/Article/details/gysdnuhoo.sHtML

[U72] PHP：写错误日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gmjzfaqtu.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.fanxiaobao.xyz/Article/details/glxhfdfgu.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.fanxiaobao.xyz/Article/details/gelsprydt.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.fanxiaobao.xyz/Article/details/gjhgiurez.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gugyaravq.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.fanxiaobao.xyz/Article/details/gedfzrzob.sHtML

[U75] PHP：依赖注入
来源：http://blog.fanxiaobao.xyz/Article/details/geqhivbnj.sHtML

composer require psr/container
来源：http://3g.fanxiaobao.xyz/Article/details/gfebtntel.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxgtmxveb.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtbindjzb.sHtML

[U77] PHP：模板渲染
来源：http://wap.fanxiaobao.xyz/Article/details/gtpubitoj.sHtML

composer require twig/twig
来源：http://wap.fanxiaobao.xyz/Article/details/gbczjjrsc.sHtML

[U78] PHP：单元测试
来源：http://baike.fanxiaobao.xyz/Article/details/goetpnjzt.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.fanxiaobao.xyz/Article/details/gepklleef.sHtML

[U79] PHP：静态分析
来源：http://wap.fanxiaobao.xyz/Article/details/gxruepzds.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.fanxiaobao.xyz/Article/details/gnysarnxx.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggxpyvsbc.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.fanxiaobao.xyz/Article/details/gthtcrxtl.sHtML

[U81] JS：初始化项目
来源：http://m.share.fanxiaobao.xyz/Article/details/gkpicwgdk.sHtML

npm init -y;  npm i express
来源：http://blog.fanxiaobao.xyz/Article/details/guqpkxjxs.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcaywaska.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzkjthcyy.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gazgmgnep.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gygpuhmyx.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.fanxiaobao.xyz/Article/details/gsivachey.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.fanxiaobao.xyz/Article/details/guxdozrgv.sHtML

[U85] JS：可选链
来源：http://baike.fanxiaobao.xyz/Article/details/gyvpybkwk.sHtML

a?.b?.c
来源：http://mobile.fanxiaobao.xyz/Article/details/gbuwhcnft.sHtML

[U86] JS：空值合并
来源：http://www.blog.fanxiaobao.xyz/Article/details/grwseppve.sHtML

a ?? b
来源：http://blog.fanxiaobao.xyz/Article/details/gbgyjthwp.sHtML

[U87] JS：解构默认值
来源：http://3g.fanxiaobao.xyz/Article/details/ghhuvdbqe.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.fanxiaobao.xyz/Article/details/gvwnieyzw.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.fanxiaobao.xyz/Article/details/gytfmujsv.sHtML

{ ...a, ...b }
来源：http://mobile.fanxiaobao.xyz/Article/details/grcqhgqzc.sHtML

[U89] JS：数组去重
来源：http://3g.fanxiaobao.xyz/Article/details/gejqkluhp.sHtML

[...new Set(arr)]
来源：http://wap.fanxiaobao.xyz/Article/details/ghkmwioxz.sHtML

[U90] JS：数字数组排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gsmyhvzan.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghxqrrdrq.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gwcpkfybk.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giqvcmulq.sHtML

[U92] JS：深拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/guvovkgtu.sHtML

structuredClone(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggvrwlhlp.sHtML

[U93] JS：模板字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gpzntpgtj.sHtML

`共 ${n} 条`
来源：http://www.share.fanxiaobao.xyz/Article/details/grwxisoep.sHtML

[U94] JS：箭头函数
来源：http://m.share.fanxiaobao.xyz/Article/details/ghbejwaot.sHtML

const double = x => x * 2;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtszeckfz.sHtML

[U95] JS：Promise 包装
来源：http://m.share.fanxiaobao.xyz/Article/details/gtkucgbfw.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.fanxiaobao.xyz/Article/details/gzlwsxpgp.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.fanxiaobao.xyz/Article/details/gfzdwbkjg.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.fanxiaobao.xyz/Article/details/glnjuhhcz.sHtML

[U97] JS：并发请求
来源：http://mobile.fanxiaobao.xyz/Article/details/gtghsprft.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fanxiaobao.xyz/Article/details/gegyewpkk.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/gvctxgfwm.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbflrgugk.sHtML

[U99] JS：事件监听
来源：http://baike.fanxiaobao.xyz/Article/details/gvsryabpd.sHtML

el.addEventListener("click", e => {})
来源：http://baike.fanxiaobao.xyz/Article/details/gsdwumqaj.sHtML

[U100] JS：DOM 查询
来源：http://baike.fanxiaobao.xyz/Article/details/gqpegzknw.sHtML

document.querySelector(".item")
来源：http://m.share.fanxiaobao.xyz/Article/details/grijocpqm.sHtML

[U101] JS：classList 操作
来源：http://3g.fanxiaobao.xyz/Article/details/gkhcygabd.sHtML

el.classList.toggle("active")
来源：http://wap.fanxiaobao.xyz/Article/details/gfuclrnvf.sHtML

[U102] JS：本地存储
来源：http://mobile.fanxiaobao.xyz/Article/details/gindscvpl.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.fanxiaobao.xyz/Article/details/gjjqlobpz.sHtML

[U103] JS：定时器
来源：http://wap.fanxiaobao.xyz/Article/details/gyanyvrye.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.fanxiaobao.xyz/Article/details/grrgihdtb.sHtML

[U104] JS：防抖
来源：http://www.share.fanxiaobao.xyz/Article/details/glbxadpmy.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gewgptaao.sHtML

[U105] JS：节流
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guktgycos.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gyynwfbay.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfwlxggau.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.fanxiaobao.xyz/Article/details/gzllsrdob.sHtML

[U107] JS：数字千分位
来源：http://m.share.fanxiaobao.xyz/Article/details/gudwzssve.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.fanxiaobao.xyz/Article/details/gxymaybdo.sHtML

[U108] JS：随机整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsrayjvrk.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.fanxiaobao.xyz/Article/details/gkpthdjnj.sHtML

[U109] JS：数组分组
来源：http://baike.fanxiaobao.xyz/Article/details/guugcegud.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gatsqneov.sHtML

[U110] JS：数组分块
来源：http://www.share.fanxiaobao.xyz/Article/details/gmxoujyax.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.fanxiaobao.xyz/Article/details/gyzwjgaog.sHtML

[U111] JS：对象转 Map
来源：http://mobile.fanxiaobao.xyz/Article/details/gzblzgyyw.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfaegxutk.sHtML

[U112] JS：字符串补位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkecfqqof.sHtML

"7".padStart(3, "0")
来源：http://mobile.fanxiaobao.xyz/Article/details/gnohquins.sHtML

[U113] JS：正则替换全部
来源：http://blog.fanxiaobao.xyz/Article/details/gtwjexaiq.sHtML

s.replaceAll("a", "b")
来源：http://blog.fanxiaobao.xyz/Article/details/ghrutdpna.sHtML

[U114] JS：JSON 深比较
来源：http://3g.fanxiaobao.xyz/Article/details/girnjoqsg.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwoxdbijp.sHtML

[U115] JS：生成 UUID
来源：http://baike.fanxiaobao.xyz/Article/details/gxfcbvfbu.sHtML

crypto.randomUUID()
来源：http://blog.fanxiaobao.xyz/Article/details/gdnpewiju.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.fanxiaobao.xyz/Article/details/goprirusa.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtsgthgiy.sHtML

[U117] JS：单元测试
来源：http://m.share.fanxiaobao.xyz/Article/details/gbxqskjoi.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.fanxiaobao.xyz/Article/details/gxfuitfkr.sHtML

[U118] JS：开发服务器
来源：http://www.share.fanxiaobao.xyz/Article/details/gxmyxtppt.sHtML

npm i -D vite;  npx vite
来源：http://blog.fanxiaobao.xyz/Article/details/gwvvrsnqa.sHtML

[U119] JS：生产构建
来源：http://baike.fanxiaobao.xyz/Article/details/glcqjrfmy.sHtML

npx vite build
来源：http://m.share.fanxiaobao.xyz/Article/details/gyypkoyoe.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.fanxiaobao.xyz/Article/details/gxeoyehjq.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.fanxiaobao.xyz/Article/details/gicgryimr.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gjymfcntd.sHtML

统计汇总
来源：http://m.share.fanxiaobao.xyz/Article/details/gximtwfts.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gqujsejvl.sHtML

按语言统计（条）：
来源：http://www.share.fanxiaobao.xyz/Article/details/gnsruieho.sHtML

Python ......... 252
来源：http://mobile.fanxiaobao.xyz/Article/details/gjlpicacq.sHtML

PHP ............ 252
来源：http://blog.fanxiaobao.xyz/Article/details/gyqnmzkbr.sHtML

JavaScript ..... 252
来源：http://wap.fanxiaobao.xyz/Article/details/guwbcsudx.sHtML

TypeScript ..... 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gjilrfxrx.sHtML

Java ........... 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gqfukkpys.sHtML

Go ............. 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsiplmapu.sHtML

Ruby ........... 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gtwifnenr.sHtML

C# ............. 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gxvwmamrr.sHtML

C .............. 30
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqfimgmn.sHtML

C++ ............ 30
来源：http://blog.fanxiaobao.xyz/Article/details/gfwxvlumy.sHtML

SQL ............ 90
来源：http://baike.fanxiaobao.xyz/Article/details/gsawbebfi.sHtML

Bash ........... 80
来源：http://baike.fanxiaobao.xyz/Article/details/gkxgsxfrc.sHtML

Kotlin ......... 15
来源：http://blog.fanxiaobao.xyz/Article/details/gfdjvzfmn.sHtML

Swift .......... 15
来源：http://baike.fanxiaobao.xyz/Article/details/gdzkbwuwi.sHtML

Lua ............ 10
来源：http://blog.fanxiaobao.xyz/Article/details/gtskeiyig.sHtML

Perl ........... 10
来源：http://mobile.fanxiaobao.xyz/Article/details/gvsmkotgl.sHtML

Scala .......... 10
来源：http://baike.fanxiaobao.xyz/Article/details/gmdbvtmer.sHtML

------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/gdbpuzscu.sHtML

合计 ........... 2106 条
来源：http://m.share.fanxiaobao.xyz/Article/details/ginadzbhh.sHtML

按章节统计：
来源：http://mobile.fanxiaobao.xyz/Article/details/gaojswuuk.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.fanxiaobao.xyz/Article/details/guvvvqsof.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.fanxiaobao.xyz/Article/details/gaywgxrmy.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.fanxiaobao.xyz/Article/details/gmeydbyfc.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwomefric.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.fanxiaobao.xyz/Article/details/gfrdnqqti.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glefqlqac.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.fanxiaobao.xyz/Article/details/ghhlekfzk.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.fanxiaobao.xyz/Article/details/ghrqwutdu.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkbljpprv.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.fanxiaobao.xyz/Article/details/gublcwexf.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/grghmswgg.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gurwurfru.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/gcigejuki.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.fanxiaobao.xyz/Article/details/guywkhzan.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwjsfhmfq.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gllqjdjik.sHtML

Q SQL 专题                              90
来源：http://baike.fanxiaobao.xyz/Article/details/gfioxrdgt.sHtML

R Bash 专题                             80
来源：http://baike.fanxiaobao.xyz/Article/details/giocgtilg.sHtML

S C / C++ 专题                          60
来源：http://www.share.fanxiaobao.xyz/Article/details/gupiunbaj.sHtML

T 其他语言补充                          60
来源：http://m.share.fanxiaobao.xyz/Article/details/gnfvkopxo.sHtML

U 高频实用片段                         120
来源：http://blog.fanxiaobao.xyz/Article/details/gvewmumno.sHtML

------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/gvdjnxauq.sHtML

合计                                  2106 条
来源：http://blog.fanxiaobao.xyz/Article/details/gpjsngszb.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/gygmxciul.sHtML


<!-- 参考信息 -->