代发 wailian999

[T49] Perl：函数
来源：http://wap.zdbjq.cn/Article/details/gvurygfrj.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/gyadmbqwc.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gndigacab.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.zdbjq.cn/Article/details/gtcusfuim.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.zdbjq.cn/Article/details/grhdxtdbt.sHtML

[T51] Scala：Hello World
来源：http://www.blog.fehbvm.com/Article/details/ghmbbegmm.sHtML

println("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gzjvdbbnw.sHtML

[T52] Scala：变量
来源：http://www.share.hesvh.cn/Article/details/gknqhyvnl.sHtML

val a = 1;  var b = 2
来源：http://m.share.hesvh.cn/Article/details/gybnyikdg.sHtML

[T53] Scala：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gbdtctdnj.sHtML

s"值: $b"
来源：http://blog.hesvh.cn/Article/details/gjplbhtyp.sHtML

[T54] Scala：集合映射
来源：http://read.share.hesvh.cn/Article/details/gzpdsbjpa.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.hesvh.cn/Article/details/gppuitgps.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fehbvm.com/Article/details/gwzgpgjio.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.fehbvm.com/Article/details/gusivpaub.sHtML

[T56] Scala：样例类
来源：http://3g.hesvh.cn/Article/details/gfmhqxfbk.sHtML

case class User(name: String, age: Int)
来源：http://wap.hesvh.cn/Article/details/gmgxipqay.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fehbvm.com/Article/details/gbztydyxs.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.hesvh.cn/Article/details/gkbdojnql.sHtML

[T58] Scala：函数定义
来源：http://m.share.zdbjq.cn/Article/details/gldnunmzw.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.fehbvm.com/Article/details/gmrvuxjyu.sHtML

[T59] Scala：循环
来源：http://www.share.zdbjq.cn/Article/details/gtycoxvzm.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.hesvh.cn/Article/details/gvezlplhr.sHtML

[T60] Scala：折叠
来源：http://3g.zdbjq.cn/Article/details/givzevmtk.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.zdbjq.cn/Article/details/gxjlmythk.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gnrbbdkhu.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fehbvm.com/Article/details/gkkqbttup.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gmsgbkrpj.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.zdbjq.cn/Article/details/gnesdiqpu.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.fehbvm.com/Article/details/gyhbhmdwr.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.zdbjq.cn/Article/details/glwfsedyw.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.fehbvm.com/Article/details/gmgebidfq.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.fehbvm.com/Article/details/gupsqezcb.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.zdbjq.cn/Article/details/gjjuleapk.sHtML

[U04] Py：变量调试打印
来源：http://read.share.zdbjq.cn/Article/details/girylzqht.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.fehbvm.com/Article/details/gbqyutadw.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.hesvh.cn/Article/details/gmfuasxqm.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.hesvh.cn/Article/details/geyipqmdu.sHtML

[U06] Py：合并两个字典
来源：http://wap.fehbvm.com/Article/details/ghsxmlfwv.sHtML

{**a, **b}
来源：http://wap.zdbjq.cn/Article/details/gdtflcnkl.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.hesvh.cn/Article/details/gkfqrcndp.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.hesvh.cn/Article/details/ghtntixrf.sHtML

[U08] Py：展平二维列表
来源：http://read.share.zdbjq.cn/Article/details/ggkqmfzhj.sHtML

[y for x in nested for y in x]
来源：http://www.blog.zdbjq.cn/Article/details/gtsomdjol.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.fehbvm.com/Article/details/gufrjfexl.sHtML

max(d, key=d.get)
来源：http://wap.hesvh.cn/Article/details/gwtcwfhmw.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.hesvh.cn/Article/details/gfutqgfpq.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.zdbjq.cn/Article/details/gvlsscmau.sHtML

[U11] Py：生成器表达式
来源：http://www.share.hesvh.cn/Article/details/gqlugizxf.sHtML

(x * 2 for x in arr)
来源：http://read.share.zdbjq.cn/Article/details/gfazhtlhk.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.fehbvm.com/Article/details/gttsxtyyx.sHtML

Counter(arr).most_common(3)
来源：http://blog.zdbjq.cn/Article/details/glijcxlog.sHtML

[U13] Py：固定长度队列
来源：http://baike.zdbjq.cn/Article/details/gqhfpicxg.sHtML

deque(maxlen=10)
来源：http://blog.hesvh.cn/Article/details/ghuhmmvld.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.hesvh.cn/Article/details/gnujzgygf.sHtML

defaultdict(list)
来源：http://blog.fehbvm.com/Article/details/gohstmsnt.sHtML

[U15] Py：高精度计时
来源：http://read.share.hesvh.cn/Article/details/gvrkfsnxj.sHtML

t = time.perf_counter()
来源：http://www.share.hesvh.cn/Article/details/gqgrmlnfh.sHtML

[U16] Py：命令行参数解析
来源：http://baike.fehbvm.com/Article/details/gingkisuu.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.fehbvm.com/Article/details/gottcjljz.sHtML

[U17] Py：初始化日志
来源：http://read.share.fehbvm.com/Article/details/gdwvwarzo.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.hesvh.cn/Article/details/gsofrykid.sHtML

[U18] Py：预编译正则
来源：http://read.share.fehbvm.com/Article/details/gbhlbvivi.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.fehbvm.com/Article/details/gogbrpccv.sHtML

[U19] Py：正则替换带回调
来源：http://wap.fehbvm.com/Article/details/gjdvnpius.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.hesvh.cn/Article/details/ghbjawwyo.sHtML

[U20] Py：缓存函数结果
来源：http://3g.fehbvm.com/Article/details/gzpohrvch.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.hesvh.cn/Article/details/ghaqkhejp.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.fehbvm.com/Article/details/gpzlucafy.sHtML

@contextlib.contextmanager
来源：http://blog.fehbvm.com/Article/details/ganhnqlyy.sHtML

[U22] Py：矩阵转置
来源：http://mobile.hesvh.cn/Article/details/gvftiwmoe.sHtML

list(zip(*m))
来源：http://www.share.zdbjq.cn/Article/details/ggthsxlaa.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.hesvh.cn/Article/details/gwksyqpzf.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.hesvh.cn/Article/details/gkftkpopk.sHtML

[U24] Py：路径操作
来源：http://mobile.zdbjq.cn/Article/details/gvdkcuczy.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.fehbvm.com/Article/details/gfgomprtr.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.zdbjq.cn/Article/details/gpaeqnwwd.sHtML

csv.DictReader(f)
来源：http://3g.fehbvm.com/Article/details/gvvkjolna.sHtML

[U26] Py：并发下载
来源：http://www.share.zdbjq.cn/Article/details/glhgnrqwq.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.zdbjq.cn/Article/details/gfdluzysv.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.fehbvm.com/Article/details/gxqqzgqcw.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.hesvh.cn/Article/details/gaccliyxb.sHtML

[U28] Py：类型别名
来源：http://blog.fehbvm.com/Article/details/gvsmxixsm.sHtML

UserId = int
来源：http://baike.fehbvm.com/Article/details/gjozwyahx.sHtML

[U29] Py：属性校验
来源：http://www.blog.hesvh.cn/Article/details/gkfcxhgti.sHtML

@property 与 @x.setter 配合
来源：http://wap.fehbvm.com/Article/details/gusztxqrw.sHtML

[U30] Py：数据类
来源：http://baike.zdbjq.cn/Article/details/gpohdjigw.sHtML

@dataclass(slots=True)
来源：http://www.m.share.hesvh.cn/Article/details/gnopgnjjg.sHtML

[U31] Py：单测
来源：http://blog.hesvh.cn/Article/details/govvcxznk.sHtML

python -m pytest -q
来源：http://www.blog.fehbvm.com/Article/details/gpstrqmud.sHtML

[U32] Py：代码格式化
来源：http://read.share.hesvh.cn/Article/details/gthclamox.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.zdbjq.cn/Article/details/gowbdhfok.sHtML

[U33] Py：打包发布
来源：http://www.share.fehbvm.com/Article/details/ghzgtmcfn.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.zdbjq.cn/Article/details/gssslgtgd.sHtML

[U34] Py：判断编码
来源：http://wap.fehbvm.com/Article/details/gblsxjvuu.sHtML

chardet.detect(raw)
来源：http://www.share.fehbvm.com/Article/details/gagxljzko.sHtML

[U35] Py：发送邮件
来源：http://wap.zdbjq.cn/Article/details/gbyodjoff.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.fehbvm.com/Article/details/gkqtwocrr.sHtML

[U36] Py：定时任务
来源：http://baike.fehbvm.com/Article/details/gqhcoqzfy.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.zdbjq.cn/Article/details/gxnjqboep.sHtML

[U37] Py：读写 Excel
来源：http://www.share.hesvh.cn/Article/details/gppvolzud.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.fehbvm.com/Article/details/gfpgtcnhm.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.zdbjq.cn/Article/details/gesveefor.sHtML

Path(__file__).resolve().parent
来源：http://m.share.zdbjq.cn/Article/details/gcabvamft.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.zdbjq.cn/Article/details/gsoblsdwn.sHtML

sys.stdout.isatty()
来源：http://read.share.fehbvm.com/Article/details/gowjkxdme.sHtML

[U40] Py：打印到标准错误
来源：http://baike.hesvh.cn/Article/details/glwvyokky.sHtML

print("err", file=sys.stderr)
来源：http://3g.hesvh.cn/Article/details/gkdxicudz.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.zdbjq.cn/Article/details/gdvthndly.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.zdbjq.cn/Article/details/gaspugddq.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.zdbjq.cn/Article/details/glccpubzh.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.hesvh.cn/Article/details/gchxfqspo.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.zdbjq.cn/Article/details/gswmmouvc.sHtML

namespace App\Http;
来源：http://www.m.share.zdbjq.cn/Article/details/gmtvbsvvr.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.zdbjq.cn/Article/details/giajdalga.sHtML

declare(strict_types=1);
来源：http://www.m.share.zdbjq.cn/Article/details/gdqtgdcrh.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.zdbjq.cn/Article/details/gizdvsmnw.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/goyuwevju.sHtML

[U46] PHP：可空类型
来源：http://3g.hesvh.cn/Article/details/grjdjuaoy.sHtML

?string $name = null
来源：http://wap.fehbvm.com/Article/details/gupwvzmbv.sHtML

[U47] PHP：联合类型
来源：http://www.share.fehbvm.com/Article/details/gjczlqljn.sHtML

int|string $id
来源：http://m.share.fehbvm.com/Article/details/gcrnxzhoy.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.fehbvm.com/Article/details/gxsoewcgo.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.fehbvm.com/Article/details/gftxzjrno.sHtML

[U49] PHP：只读属性
来源：http://www.share.hesvh.cn/Article/details/gabysonxv.sHtML

public readonly string $name
来源：http://www.blog.hesvh.cn/Article/details/gplsjvkdh.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.zdbjq.cn/Article/details/gdqkxuhwv.sHtML

public function __construct(private int $id) {}
来源：http://blog.hesvh.cn/Article/details/gohobdvtq.sHtML

[U51] PHP：数组解构
来源：http://m.share.fehbvm.com/Article/details/gvyjyvqmc.sHtML

[$a, $b] = $arr;
来源：http://www.blog.zdbjq.cn/Article/details/gqujgmspe.sHtML

[U52] PHP：箭头函数
来源：http://wap.hesvh.cn/Article/details/gvzbekuex.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.hesvh.cn/Article/details/gdvjfubuf.sHtML

[U53] PHP：空合并运算符
来源：http://wap.hesvh.cn/Article/details/gbwfamfzm.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.hesvh.cn/Article/details/gtuqpaxtx.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.zdbjq.cn/Article/details/ggzmneedg.sHtML

$obj?->method()
来源：http://3g.hesvh.cn/Article/details/gxcfkvyph.sHtML

[U55] PHP：match 表达式
来源：http://mobile.zdbjq.cn/Article/details/gnvspgrve.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.hesvh.cn/Article/details/gdkqprjlc.sHtML

[U56] PHP：命名参数
来源：http://read.share.zdbjq.cn/Article/details/gxbxugvjc.sHtML

f(a: 1, b: 2)
来源：http://wap.zdbjq.cn/Article/details/gpopavjar.sHtML

[U57] PHP：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gyentallo.sHtML

"值: {$a}"
来源：http://blog.fehbvm.com/Article/details/gezivmrzj.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.zdbjq.cn/Article/details/gfhxphtfv.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.hesvh.cn/Article/details/gspsafllr.sHtML

[U59] PHP：自定义排序
来源：http://blog.fehbvm.com/Article/details/gneauvhji.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fehbvm.com/Article/details/gnaixkggw.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.fehbvm.com/Article/details/gricynjfx.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.fehbvm.com/Article/details/gjsopuaes.sHtML

[U61] PHP：正则
来源：http://wap.fehbvm.com/Article/details/galhgeqig.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gcnjkadyu.sHtML

[U62] PHP：日期对象
来源：http://m.share.zdbjq.cn/Article/details/glcqefhby.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.fehbvm.com/Article/details/gzigeiwrl.sHtML

[U63] PHP：文件读写
来源：http://m.share.hesvh.cn/Article/details/gtmslzacm.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.zdbjq.cn/Article/details/gjbewqabz.sHtML

[U64] PHP：目录遍历
来源：http://baike.zdbjq.cn/Article/details/gahrsgjnr.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.hesvh.cn/Article/details/gxlabgkqj.sHtML

[U65] PHP：会话
来源：http://www.m.share.zdbjq.cn/Article/details/gnldxegak.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gtabwuybq.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.zdbjq.cn/Article/details/gggrnsjcg.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.hesvh.cn/Article/details/gfujexkca.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.fehbvm.com/Article/details/gdnmhwvzk.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.hesvh.cn/Article/details/gcpcpnodz.sHtML

[U68] PHP：PDO 连接
来源：http://wap.hesvh.cn/Article/details/gfiankwpu.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.fehbvm.com/Article/details/grayqrmkt.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.hesvh.cn/Article/details/gncgudtbp.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.fehbvm.com/Article/details/gydybwkuv.sHtML

[U70] PHP：PDO 事务
来源：http://baike.hesvh.cn/Article/details/gavepmywu.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.hesvh.cn/Article/details/gnxeykkvz.sHtML

[U71] PHP：抛出异常
来源：http://3g.hesvh.cn/Article/details/gfpokqnmy.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.hesvh.cn/Article/details/gmishserf.sHtML

[U72] PHP：写错误日志
来源：http://3g.hesvh.cn/Article/details/gdzhkczay.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.hesvh.cn/Article/details/gpmhkknmz.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.zdbjq.cn/Article/details/gmyeveyaw.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.zdbjq.cn/Article/details/gayrodlly.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.zdbjq.cn/Article/details/glawiuhxh.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.zdbjq.cn/Article/details/gbrdvuyjg.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.fehbvm.com/Article/details/gtajpixju.sHtML

composer require psr/container
来源：http://read.share.hesvh.cn/Article/details/gcxhfdele.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.zdbjq.cn/Article/details/gkuievyyr.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.zdbjq.cn/Article/details/gvorjeefp.sHtML

[U77] PHP：模板渲染
来源：http://blog.fehbvm.com/Article/details/gllklcucm.sHtML

composer require twig/twig
来源：http://read.share.fehbvm.com/Article/details/gozhukcrm.sHtML

[U78] PHP：单元测试
来源：http://www.share.hesvh.cn/Article/details/grtwjpjpp.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.fehbvm.com/Article/details/gppehmywb.sHtML

[U79] PHP：静态分析
来源：http://mobile.fehbvm.com/Article/details/ghggqwqav.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.zdbjq.cn/Article/details/ghhyolguv.sHtML

[U80] PHP：代码规范修复
来源：http://baike.fehbvm.com/Article/details/gpuvzcbbe.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.hesvh.cn/Article/details/gtwzoegyf.sHtML

[U81] JS：初始化项目
来源：http://www.share.zdbjq.cn/Article/details/gpbtkyunv.sHtML

npm init -y;  npm i express
来源：http://www.m.share.hesvh.cn/Article/details/gampbczpq.sHtML

[U82] JS：package.json 脚本
来源：http://baike.zdbjq.cn/Article/details/gmjsjxwbq.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.fehbvm.com/Article/details/gmmnjhbok.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.zdbjq.cn/Article/details/gwrgugtet.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.hesvh.cn/Article/details/gpipvsjfm.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.hesvh.cn/Article/details/gqujbgoek.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.hesvh.cn/Article/details/gknjnojrw.sHtML

[U85] JS：可选链
来源：http://3g.fehbvm.com/Article/details/gwadcston.sHtML

a?.b?.c
来源：http://baike.zdbjq.cn/Article/details/gkjozxoyt.sHtML

[U86] JS：空值合并
来源：http://www.blog.fehbvm.com/Article/details/gdlalsbfv.sHtML

a ?? b
来源：http://www.blog.hesvh.cn/Article/details/gbyzuhspw.sHtML

[U87] JS：解构默认值
来源：http://m.share.zdbjq.cn/Article/details/grmysruzu.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.fehbvm.com/Article/details/gfrfhxmxv.sHtML

[U88] JS：对象展开合并
来源：http://wap.fehbvm.com/Article/details/gilorpsvs.sHtML

{ ...a, ...b }
来源：http://www.m.share.hesvh.cn/Article/details/gorwlebwa.sHtML

[U89] JS：数组去重
来源：http://read.share.fehbvm.com/Article/details/guaisuyhz.sHtML

[...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/gfijbliur.sHtML

[U90] JS：数字数组排序
来源：http://wap.hesvh.cn/Article/details/glcnpkopw.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/gowxzjuny.sHtML

[U91] JS：对象键值遍历
来源：http://baike.fehbvm.com/Article/details/gwqxbjrkc.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.fehbvm.com/Article/details/ghpxveimn.sHtML

[U92] JS：深拷贝
来源：http://m.share.zdbjq.cn/Article/details/gbymsjyra.sHtML

structuredClone(obj)
来源：http://www.share.fehbvm.com/Article/details/gclxpdkll.sHtML

[U93] JS：模板字符串
来源：http://www.share.hesvh.cn/Article/details/ggkvdrzac.sHtML

`共 ${n} 条`
来源：http://www.share.fehbvm.com/Article/details/gltakopmf.sHtML

[U94] JS：箭头函数
来源：http://3g.hesvh.cn/Article/details/gfndcxpyn.sHtML

const double = x => x * 2;
来源：http://3g.zdbjq.cn/Article/details/gymainija.sHtML

[U95] JS：Promise 包装
来源：http://baike.zdbjq.cn/Article/details/gswrsmbjf.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.zdbjq.cn/Article/details/gcwmstigw.sHtML

[U96] JS：async/await 与异常
来源：http://3g.zdbjq.cn/Article/details/gzybebzsr.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/gwovcvjho.sHtML

[U97] JS：并发请求
来源：http://www.m.share.fehbvm.com/Article/details/ghyssxgpb.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/gmhyysizk.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.fehbvm.com/Article/details/glldsvvtz.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.zdbjq.cn/Article/details/gsfqbsjtc.sHtML

[U99] JS：事件监听
来源：http://wap.fehbvm.com/Article/details/gcuaniutm.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.zdbjq.cn/Article/details/gymypwyrw.sHtML

[U100] JS：DOM 查询
来源：http://mobile.fehbvm.com/Article/details/gamoesvij.sHtML

document.querySelector(".item")
来源：http://blog.hesvh.cn/Article/details/gbrohsyub.sHtML

[U101] JS：classList 操作
来源：http://blog.zdbjq.cn/Article/details/geflkumwx.sHtML

el.classList.toggle("active")
来源：http://www.blog.hesvh.cn/Article/details/grrgxrnrz.sHtML

[U102] JS：本地存储
来源：http://3g.fehbvm.com/Article/details/gfyfrcnvs.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.zdbjq.cn/Article/details/gjkilbvyq.sHtML

[U103] JS：定时器
来源：http://mobile.zdbjq.cn/Article/details/gszyekwju.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.zdbjq.cn/Article/details/gbynaofeu.sHtML

[U104] JS：防抖
来源：http://www.m.share.fehbvm.com/Article/details/gvvuftvfx.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/gajfsxybj.sHtML

[U105] JS：节流
来源：http://mobile.zdbjq.cn/Article/details/ghbqbztpd.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.hesvh.cn/Article/details/godjdrzzn.sHtML

[U106] JS：日期格式化
来源：http://wap.hesvh.cn/Article/details/gdfcwevov.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.zdbjq.cn/Article/details/gjsnzcprv.sHtML

[U107] JS：数字千分位
来源：http://m.share.hesvh.cn/Article/details/gvyzyqioq.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.fehbvm.com/Article/details/gnluzmdef.sHtML

[U108] JS：随机整数
来源：http://3g.hesvh.cn/Article/details/gsyyxnmkj.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.fehbvm.com/Article/details/gwuxhlthh.sHtML

[U109] JS：数组分组
来源：http://mobile.zdbjq.cn/Article/details/gzchfyjze.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.hesvh.cn/Article/details/gbdoxhhlf.sHtML

[U110] JS：数组分块
来源：http://www.blog.hesvh.cn/Article/details/gmtecensd.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.fehbvm.com/Article/details/gzhliailj.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.zdbjq.cn/Article/details/gagbsrgon.sHtML

new Map(Object.entries(obj))
来源：http://mobile.zdbjq.cn/Article/details/gfkiiwksx.sHtML

[U112] JS：字符串补位
来源：http://baike.zdbjq.cn/Article/details/glvntqpym.sHtML

"7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gptsuyxpr.sHtML

[U113] JS：正则替换全部
来源：http://www.share.hesvh.cn/Article/details/gyiuocxje.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gvwwcdxoa.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.zdbjq.cn/Article/details/gcqtuuqyb.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fehbvm.com/Article/details/gzruhysew.sHtML

[U115] JS：生成 UUID
来源：http://blog.hesvh.cn/Article/details/glrsrawnw.sHtML

crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/gxhwxepxt.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.fehbvm.com/Article/details/gjxcsbhqw.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.fehbvm.com/Article/details/geaefmgsi.sHtML

[U117] JS：单元测试
来源：http://m.share.zdbjq.cn/Article/details/glcngrkrh.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.hesvh.cn/Article/details/gjdcbqput.sHtML

[U118] JS：开发服务器
来源：http://www.share.fehbvm.com/Article/details/gtjjckosp.sHtML

npm i -D vite;  npx vite
来源：http://wap.hesvh.cn/Article/details/gehchgfgc.sHtML

[U119] JS：生产构建
来源：http://wap.zdbjq.cn/Article/details/gefcyebqh.sHtML

npx vite build
来源：http://baike.zdbjq.cn/Article/details/gjhbcvpct.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.hesvh.cn/Article/details/grdxdhgvo.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.fehbvm.com/Article/details/gvycsygip.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gqhdyvzze.sHtML

统计汇总
来源：http://www.share.fehbvm.com/Article/details/gpnlswrmv.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gqzpzlscp.sHtML

按语言统计（条）：
来源：http://3g.hesvh.cn/Article/details/gkfjazvpu.sHtML

Python ......... 252
来源：http://blog.hesvh.cn/Article/details/gcslfefar.sHtML

PHP ............ 252
来源：http://m.share.hesvh.cn/Article/details/gcmgpbmlh.sHtML

JavaScript ..... 252
来源：http://m.share.fehbvm.com/Article/details/geqlvluyv.sHtML

TypeScript ..... 212
来源：http://mobile.zdbjq.cn/Article/details/gfrccbvcp.sHtML

Java ........... 212
来源：http://m.share.fehbvm.com/Article/details/ghggbqmrh.sHtML

Go ............. 212
来源：http://3g.hesvh.cn/Article/details/gwpsvmpst.sHtML

Ruby ........... 212
来源：http://wap.fehbvm.com/Article/details/gnpjdhfxa.sHtML

C# ............. 212
来源：http://read.share.zdbjq.cn/Article/details/grqqldppp.sHtML

C .............. 30
来源：http://baike.fehbvm.com/Article/details/gricjkias.sHtML

C++ ............ 30
来源：http://read.share.fehbvm.com/Article/details/gjrgegnjz.sHtML

SQL ............ 90
来源：http://www.blog.fehbvm.com/Article/details/ghqtdrahy.sHtML

Bash ........... 80
来源：http://baike.fehbvm.com/Article/details/gawjxpvpw.sHtML

Kotlin ......... 15
来源：http://www.share.fehbvm.com/Article/details/gahuwueez.sHtML

Swift .......... 15
来源：http://blog.hesvh.cn/Article/details/gxfdgnycu.sHtML

Lua ............ 10
来源：http://read.share.hesvh.cn/Article/details/ggitizkmr.sHtML

Perl ........... 10
来源：http://mobile.hesvh.cn/Article/details/gpiruaehx.sHtML

Scala .......... 10
来源：http://www.m.share.zdbjq.cn/Article/details/gzwqvsxcp.sHtML

------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gszpiheqm.sHtML

合计 ........... 2106 条
来源：http://mobile.hesvh.cn/Article/details/gbljbwkpm.sHtML

按章节统计：
来源：http://m.share.hesvh.cn/Article/details/ghaadwtxw.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.zdbjq.cn/Article/details/guuzovaml.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.fehbvm.com/Article/details/gbmvyjysd.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.fehbvm.com/Article/details/gkqqqghpr.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.fehbvm.com/Article/details/gidqzzmlh.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.fehbvm.com/Article/details/gihqrqmdm.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.hesvh.cn/Article/details/gotabixky.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/gwvjucdny.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.fehbvm.com/Article/details/gjvekjgpa.sHtML


<!-- 参考信息 -->