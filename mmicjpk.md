代发 wailian999

while (my $line = <$fh>) { print $line; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwsbnkaoq.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glkqkhzjy.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gucvtdsbj.sHtML

[T52] Scala：变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gzfipmsbp.sHtML

val a = 1;  var b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggpnsbbvd.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gkvlvvnvf.sHtML

s"值: $b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gdjoniqcg.sHtML

[T54] Scala：集合映射
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsdwwhroj.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gfyzdrvsg.sHtML

[T55] Scala：集合过滤
来源：http://blog.fanxiaobao.xyz/Article/details/grbaqbbla.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/glyzwxxoy.sHtML

[T56] Scala：样例类
来源：http://blog.fanxiaobao.xyz/Article/details/guptcrppe.sHtML

case class User(name: String, age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/gsxbxeqrd.sHtML

[T57] Scala：模式匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gbbtoiwut.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.fanxiaobao.xyz/Article/details/giwddsdft.sHtML

[T58] Scala：函数定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gcnqxwmzz.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkukouzrp.sHtML

[T59] Scala：循环
来源：http://wap.fanxiaobao.xyz/Article/details/gbscsruhl.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtnqwavmu.sHtML

[T60] Scala：折叠
来源：http://blog.fanxiaobao.xyz/Article/details/gueyeknki.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.fanxiaobao.xyz/Article/details/gkmmmxsva.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gtrmxrdmf.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqxepvjih.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/goqsibzml.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.fanxiaobao.xyz/Article/details/gxuibwvpg.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.fanxiaobao.xyz/Article/details/gnjkevsik.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghqkmhoee.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gppgdsupg.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fanxiaobao.xyz/Article/details/gqvrsrwli.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.fanxiaobao.xyz/Article/details/gpmfykugn.sHtML

[U04] Py：变量调试打印
来源：http://wap.fanxiaobao.xyz/Article/details/gsexvuiuz.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.fanxiaobao.xyz/Article/details/gfdkzdmao.sHtML

[U05] Py：列表去重且保序
来源：http://baike.fanxiaobao.xyz/Article/details/gkjhzxnlp.sHtML

list(dict.fromkeys(arr))
来源：http://blog.fanxiaobao.xyz/Article/details/gdlanoalj.sHtML

[U06] Py：合并两个字典
来源：http://wap.fanxiaobao.xyz/Article/details/gykeexvgo.sHtML

{**a, **b}
来源：http://baike.fanxiaobao.xyz/Article/details/gurofhkmi.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gctbqrozl.sHtML

{v: k for k, v in d.items()}
来源：http://wap.fanxiaobao.xyz/Article/details/gzvswcljx.sHtML

[U08] Py：展平二维列表
来源：http://blog.fanxiaobao.xyz/Article/details/gbadwiinx.sHtML

[y for x in nested for y in x]
来源：http://mobile.fanxiaobao.xyz/Article/details/gheykibgb.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.fanxiaobao.xyz/Article/details/ghgomrkgj.sHtML

max(d, key=d.get)
来源：http://mobile.fanxiaobao.xyz/Article/details/gohaiawas.sHtML

[U10] Py：按值排序字典
来源：http://3g.fanxiaobao.xyz/Article/details/gdhotuitz.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.fanxiaobao.xyz/Article/details/gjolkzeko.sHtML

[U11] Py：生成器表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gzzbffyod.sHtML

(x * 2 for x in arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gwaaidixq.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.fanxiaobao.xyz/Article/details/gpnmuapbs.sHtML

Counter(arr).most_common(3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwfwkipup.sHtML

[U13] Py：固定长度队列
来源：http://3g.fanxiaobao.xyz/Article/details/geplqtwhl.sHtML

deque(maxlen=10)
来源：http://read.share.fanxiaobao.xyz/Article/details/gryndmjoj.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.fanxiaobao.xyz/Article/details/gbwrqdgul.sHtML

defaultdict(list)
来源：http://3g.fanxiaobao.xyz/Article/details/gapstrxmv.sHtML

[U15] Py：高精度计时
来源：http://baike.fanxiaobao.xyz/Article/details/gzvgxdggo.sHtML

t = time.perf_counter()
来源：http://blog.fanxiaobao.xyz/Article/details/guewdctss.sHtML

[U16] Py：命令行参数解析
来源：http://wap.fanxiaobao.xyz/Article/details/gmgwlagtp.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkepmrwjz.sHtML

[U17] Py：初始化日志
来源：http://read.share.fanxiaobao.xyz/Article/details/guatadujd.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggshdohhs.sHtML

[U18] Py：预编译正则
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwggysbap.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/gvvnkkjma.sHtML

[U19] Py：正则替换带回调
来源：http://3g.fanxiaobao.xyz/Article/details/gqzlvsest.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqovbgngt.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.fanxiaobao.xyz/Article/details/gbzmzpkrz.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.fanxiaobao.xyz/Article/details/ginsspdft.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcsulrwhl.sHtML

@contextlib.contextmanager
来源：http://m.share.fanxiaobao.xyz/Article/details/gqbibyebk.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.fanxiaobao.xyz/Article/details/gelpkkccy.sHtML

list(zip(*m))
来源：http://baike.fanxiaobao.xyz/Article/details/gtmqbhgbh.sHtML

[U23] Py：分块读取大文件
来源：http://3g.fanxiaobao.xyz/Article/details/gtthhakir.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.fanxiaobao.xyz/Article/details/gjenqqxbc.sHtML

[U24] Py：路径操作
来源：http://wap.fanxiaobao.xyz/Article/details/glstkckrw.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdiibgpjn.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.fanxiaobao.xyz/Article/details/gxcqkkzhv.sHtML

csv.DictReader(f)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxuyfyoyz.sHtML

[U26] Py：并发下载
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbwpppnwd.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.fanxiaobao.xyz/Article/details/gzzztqkrj.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.fanxiaobao.xyz/Article/details/gppmiupmp.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.fanxiaobao.xyz/Article/details/gajacaeet.sHtML

[U28] Py：类型别名
来源：http://read.share.fanxiaobao.xyz/Article/details/gnrhvwmuw.sHtML

UserId = int
来源：http://www.share.fanxiaobao.xyz/Article/details/gzqdancjr.sHtML

[U29] Py：属性校验
来源：http://wap.fanxiaobao.xyz/Article/details/grogmeuyn.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkzeoglbi.sHtML

[U30] Py：数据类
来源：http://baike.fanxiaobao.xyz/Article/details/gvceldtym.sHtML

@dataclass(slots=True)
来源：http://baike.fanxiaobao.xyz/Article/details/gzkdfprwc.sHtML

[U31] Py：单测
来源：http://3g.fanxiaobao.xyz/Article/details/gjqmvlfdo.sHtML

python -m pytest -q
来源：http://blog.fanxiaobao.xyz/Article/details/gidhpgiui.sHtML

[U32] Py：代码格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gescltyom.sHtML

ruff format . && ruff check --fix .
来源：http://blog.fanxiaobao.xyz/Article/details/gumkweaij.sHtML

[U33] Py：打包发布
来源：http://blog.fanxiaobao.xyz/Article/details/gkncpovjz.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.fanxiaobao.xyz/Article/details/gvsjyitgo.sHtML

[U34] Py：判断编码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbwxpplpu.sHtML

chardet.detect(raw)
来源：http://blog.fanxiaobao.xyz/Article/details/galhaonfx.sHtML

[U35] Py：发送邮件
来源：http://mobile.fanxiaobao.xyz/Article/details/gwigaktbe.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.fanxiaobao.xyz/Article/details/gaqtuifve.sHtML

[U36] Py：定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gvwefdyao.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnveyqpra.sHtML

[U37] Py：读写 Excel
来源：http://blog.fanxiaobao.xyz/Article/details/gpeeqejkr.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.fanxiaobao.xyz/Article/details/gsfzhvjxp.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.fanxiaobao.xyz/Article/details/gbhmluuny.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbeamhpmk.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.fanxiaobao.xyz/Article/details/gecuhcfbn.sHtML

sys.stdout.isatty()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpuwvjhqs.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjcxmlskz.sHtML

print("err", file=sys.stderr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcbkubxky.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.fanxiaobao.xyz/Article/details/gupsriizw.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gffxpxtxp.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.fanxiaobao.xyz/Article/details/gwqkxfubq.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.fanxiaobao.xyz/Article/details/gqzqqhjjh.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.fanxiaobao.xyz/Article/details/gbeygvfem.sHtML

namespace App\Http;
来源：http://blog.fanxiaobao.xyz/Article/details/gxpsytncl.sHtML

[U44] PHP：开启严格类型
来源：http://blog.fanxiaobao.xyz/Article/details/gnrniqdnz.sHtML

declare(strict_types=1);
来源：http://3g.fanxiaobao.xyz/Article/details/gxkmrvuwe.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.fanxiaobao.xyz/Article/details/ghpnrtvky.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/glmibcrqo.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gajoqyxez.sHtML

?string $name = null
来源：http://mobile.fanxiaobao.xyz/Article/details/gtevyhsnt.sHtML

[U47] PHP：联合类型
来源：http://blog.fanxiaobao.xyz/Article/details/gefgieeax.sHtML

int|string $id
来源：http://baike.fanxiaobao.xyz/Article/details/grxngsenv.sHtML

[U48] PHP：纯枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gqmmxyysj.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkuvzjdjd.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goyknzhzg.sHtML

public readonly string $name
来源：http://baike.fanxiaobao.xyz/Article/details/gjcgaqoig.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.fanxiaobao.xyz/Article/details/gkgtuqzov.sHtML

public function __construct(private int $id) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gxenzyjmx.sHtML

[U51] PHP：数组解构
来源：http://read.share.fanxiaobao.xyz/Article/details/gkbmqiyby.sHtML

[$a, $b] = $arr;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzduuwqow.sHtML

[U52] PHP：箭头函数
来源：http://3g.fanxiaobao.xyz/Article/details/gezbwkuao.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjynsycnt.sHtML

[U53] PHP：空合并运算符
来源：http://baike.fanxiaobao.xyz/Article/details/gytwgheqq.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.fanxiaobao.xyz/Article/details/gotlhvuuc.sHtML

[U54] PHP：空安全调用
来源：http://blog.fanxiaobao.xyz/Article/details/gurkpsbxp.sHtML

$obj?->method()
来源：http://baike.fanxiaobao.xyz/Article/details/gutrgkpyf.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkkxtstkp.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.fanxiaobao.xyz/Article/details/gkvbermbp.sHtML

[U56] PHP：命名参数
来源：http://wap.fanxiaobao.xyz/Article/details/gnfinvljy.sHtML

f(a: 1, b: 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gzjbxyzva.sHtML

[U57] PHP：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gdcdcxlpx.sHtML

"值: {$a}"
来源：http://3g.fanxiaobao.xyz/Article/details/gwocwyyup.sHtML

[U58] PHP：数组三件套
来源：http://read.share.fanxiaobao.xyz/Article/details/gjscqhibm.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.fanxiaobao.xyz/Article/details/gmqoxizng.sHtML

[U59] PHP：自定义排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gzfwbmlhj.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gybtvywst.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcmfkhafw.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.fanxiaobao.xyz/Article/details/glcbtdxif.sHtML

[U61] PHP：正则
来源：http://blog.fanxiaobao.xyz/Article/details/gauveddqh.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.fanxiaobao.xyz/Article/details/gozvxicgq.sHtML

[U62] PHP：日期对象
来源：http://blog.fanxiaobao.xyz/Article/details/gdvnqpskg.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyjdjnkns.sHtML

[U63] PHP：文件读写
来源：http://www.share.fanxiaobao.xyz/Article/details/gknqvbfya.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.fanxiaobao.xyz/Article/details/gjmgejgav.sHtML

[U64] PHP：目录遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gwpgibczp.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.fanxiaobao.xyz/Article/details/ggguvuymf.sHtML

[U65] PHP：会话
来源：http://read.share.fanxiaobao.xyz/Article/details/gzlmnxugw.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gtchpbdeh.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.fanxiaobao.xyz/Article/details/gsvgvfnjg.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.fanxiaobao.xyz/Article/details/gjchyhnnk.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.fanxiaobao.xyz/Article/details/givpzlpqs.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.fanxiaobao.xyz/Article/details/glazadggz.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gqtbvmuvm.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.fanxiaobao.xyz/Article/details/gsgzblfrh.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.fanxiaobao.xyz/Article/details/gomjdlzjw.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.fanxiaobao.xyz/Article/details/guxwutube.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gwskjpibr.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.fanxiaobao.xyz/Article/details/glfnlpjxg.sHtML

[U71] PHP：抛出异常
来源：http://mobile.fanxiaobao.xyz/Article/details/gozaqmzxw.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtxbgwsuv.sHtML

[U72] PHP：写错误日志
来源：http://blog.fanxiaobao.xyz/Article/details/gasuklfyq.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.fanxiaobao.xyz/Article/details/gogxrlluv.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.fanxiaobao.xyz/Article/details/gipqbzmjm.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.fanxiaobao.xyz/Article/details/gkhumlwps.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gsrdfpzjh.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfsqkehib.sHtML

[U75] PHP：依赖注入
来源：http://read.share.fanxiaobao.xyz/Article/details/gzvcufwxi.sHtML

composer require psr/container
来源：http://mobile.fanxiaobao.xyz/Article/details/gkrkevgtm.sHtML

[U76] PHP：简单路由
来源：http://baike.fanxiaobao.xyz/Article/details/gtcoduwje.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.fanxiaobao.xyz/Article/details/gpsrcgdpg.sHtML

[U77] PHP：模板渲染
来源：http://wap.fanxiaobao.xyz/Article/details/ghrkmxbmh.sHtML

composer require twig/twig
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gayhxonku.sHtML

[U78] PHP：单元测试
来源：http://wap.fanxiaobao.xyz/Article/details/gwcpgoaxr.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.fanxiaobao.xyz/Article/details/gohncpbpp.sHtML

[U79] PHP：静态分析
来源：http://baike.fanxiaobao.xyz/Article/details/gylogrbgd.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.fanxiaobao.xyz/Article/details/gtgvxpqvo.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.fanxiaobao.xyz/Article/details/gzlsgdtsh.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcccncipn.sHtML

[U81] JS：初始化项目
来源：http://www.blog.fanxiaobao.xyz/Article/details/girvouhyt.sHtML

npm init -y;  npm i express
来源：http://read.share.fanxiaobao.xyz/Article/details/gubcojwck.sHtML

[U82] JS：package.json 脚本
来源：http://baike.fanxiaobao.xyz/Article/details/gllkqqfvp.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.fanxiaobao.xyz/Article/details/glvjpsdrw.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.fanxiaobao.xyz/Article/details/galiygwav.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.fanxiaobao.xyz/Article/details/gpkarcqre.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.fanxiaobao.xyz/Article/details/ghrdweelc.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.fanxiaobao.xyz/Article/details/gvbjsfrfc.sHtML

[U85] JS：可选链
来源：http://www.share.fanxiaobao.xyz/Article/details/gwhsxdwry.sHtML

a?.b?.c
来源：http://baike.fanxiaobao.xyz/Article/details/grdvoectb.sHtML

[U86] JS：空值合并
来源：http://baike.fanxiaobao.xyz/Article/details/gmtlcpyqt.sHtML

a ?? b
来源：http://wap.fanxiaobao.xyz/Article/details/gzldomjew.sHtML

[U87] JS：解构默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/gvmufyduf.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.fanxiaobao.xyz/Article/details/gpbcipxsg.sHtML

[U88] JS：对象展开合并
来源：http://blog.fanxiaobao.xyz/Article/details/gtnymccys.sHtML

{ ...a, ...b }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcabgmhla.sHtML

[U89] JS：数组去重
来源：http://m.share.fanxiaobao.xyz/Article/details/gmyvgdoay.sHtML

[...new Set(arr)]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpskaqwbv.sHtML

[U90] JS：数字数组排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gaxfhjzer.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gawwulebn.sHtML

[U91] JS：对象键值遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gbftdsosy.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.fanxiaobao.xyz/Article/details/gjtuhxoic.sHtML

[U92] JS：深拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gzthuvusg.sHtML

structuredClone(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/glnwumdzz.sHtML

[U93] JS：模板字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gzzzhgmuf.sHtML

`共 ${n} 条`
来源：http://blog.fanxiaobao.xyz/Article/details/ghdcpecrg.sHtML

[U94] JS：箭头函数
来源：http://3g.fanxiaobao.xyz/Article/details/gzlqzhwsa.sHtML

const double = x => x * 2;
来源：http://baike.fanxiaobao.xyz/Article/details/gbgrkzjso.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmssjbcdy.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.fanxiaobao.xyz/Article/details/gkxojgymj.sHtML

[U96] JS：async/await 与异常
来源：http://blog.fanxiaobao.xyz/Article/details/grflckreb.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.fanxiaobao.xyz/Article/details/gtmkvpagf.sHtML

[U97] JS：并发请求
来源：http://mobile.fanxiaobao.xyz/Article/details/gapahnceg.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fanxiaobao.xyz/Article/details/gcehkiphw.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/gngoytexc.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.fanxiaobao.xyz/Article/details/grjzurcjg.sHtML

[U99] JS：事件监听
来源：http://read.share.fanxiaobao.xyz/Article/details/gcccqgpwo.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.fanxiaobao.xyz/Article/details/gqktogayw.sHtML

[U100] JS：DOM 查询
来源：http://wap.fanxiaobao.xyz/Article/details/gwtravgqv.sHtML

document.querySelector(".item")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbynrzkso.sHtML

[U101] JS：classList 操作
来源：http://wap.fanxiaobao.xyz/Article/details/giallzols.sHtML

el.classList.toggle("active")
来源：http://www.share.fanxiaobao.xyz/Article/details/glzqafzsk.sHtML

[U102] JS：本地存储
来源：http://m.share.fanxiaobao.xyz/Article/details/gznlutetp.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.fanxiaobao.xyz/Article/details/gmyldsfsc.sHtML

[U103] JS：定时器
来源：http://3g.fanxiaobao.xyz/Article/details/gqsyskrlw.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwqhefaow.sHtML

[U104] JS：防抖
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdrtkhvnm.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gacfdaknl.sHtML

[U105] JS：节流
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjrxxdkcr.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkzklgfkm.sHtML

[U106] JS：日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gthrdwqlx.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.fanxiaobao.xyz/Article/details/gvavmmbho.sHtML

[U107] JS：数字千分位
来源：http://baike.fanxiaobao.xyz/Article/details/grmcotvfu.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.fanxiaobao.xyz/Article/details/gttzofrmd.sHtML

[U108] JS：随机整数
来源：http://baike.fanxiaobao.xyz/Article/details/ggvacxgdo.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.fanxiaobao.xyz/Article/details/ggsuvwytn.sHtML

[U109] JS：数组分组
来源：http://baike.fanxiaobao.xyz/Article/details/gxepjpdqz.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.fanxiaobao.xyz/Article/details/gxrtsriha.sHtML

[U110] JS：数组分块
来源：http://www.m.share.fanxiaobao.xyz/Article/details/garvfxhdq.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.fanxiaobao.xyz/Article/details/gtgvrddvm.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfhtwhooc.sHtML

new Map(Object.entries(obj))
来源：http://read.share.fanxiaobao.xyz/Article/details/gcionvpax.sHtML

[U112] JS：字符串补位
来源：http://baike.fanxiaobao.xyz/Article/details/gehnrrxiv.sHtML

"7".padStart(3, "0")
来源：http://blog.fanxiaobao.xyz/Article/details/ggqycsjnn.sHtML

[U113] JS：正则替换全部
来源：http://www.share.fanxiaobao.xyz/Article/details/ggeflwfhp.sHtML

s.replaceAll("a", "b")
来源：http://wap.fanxiaobao.xyz/Article/details/gkndjhhfk.sHtML

[U114] JS：JSON 深比较
来源：http://baike.fanxiaobao.xyz/Article/details/gcevdrtij.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fanxiaobao.xyz/Article/details/gtmbckfhe.sHtML

[U115] JS：生成 UUID
来源：http://baike.fanxiaobao.xyz/Article/details/gnmmdxzcw.sHtML

crypto.randomUUID()
来源：http://m.share.fanxiaobao.xyz/Article/details/gqgrrblxx.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.fanxiaobao.xyz/Article/details/gccpmqiwk.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkfgdgzct.sHtML

[U117] JS：单元测试
来源：http://m.share.fanxiaobao.xyz/Article/details/gvklzokny.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gahfhodal.sHtML

[U118] JS：开发服务器
来源：http://baike.fanxiaobao.xyz/Article/details/gjyqukbby.sHtML

npm i -D vite;  npx vite
来源：http://wap.fanxiaobao.xyz/Article/details/gynfybtay.sHtML

[U119] JS：生产构建
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmtrloyvz.sHtML

npx vite build
来源：http://m.share.fanxiaobao.xyz/Article/details/gumiomqvr.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtlivhxyq.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqdonsxvw.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gmabkvjax.sHtML

统计汇总
来源：http://mobile.fanxiaobao.xyz/Article/details/gwganmjmy.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gkhsckmth.sHtML

按语言统计（条）：
来源：http://blog.fanxiaobao.xyz/Article/details/giirlblay.sHtML

Python ......... 252
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmkyhaxhh.sHtML

PHP ............ 252
来源：http://www.blog.fanxiaobao.xyz/Article/details/giyvmysnb.sHtML

JavaScript ..... 252
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfkwltulc.sHtML

TypeScript ..... 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdkjllqba.sHtML

Java ........... 212
来源：http://baike.fanxiaobao.xyz/Article/details/gbhqmbesy.sHtML

Go ............. 212
来源：http://read.share.fanxiaobao.xyz/Article/details/ggjrucwdp.sHtML

Ruby ........... 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsxoggdnu.sHtML

C# ............. 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gntfkxltt.sHtML

C .............. 30
来源：http://3g.fanxiaobao.xyz/Article/details/gkxomvxlz.sHtML

C++ ............ 30
来源：http://www.blog.fanxiaobao.xyz/Article/details/grepgnqaj.sHtML

SQL ............ 90
来源：http://baike.fanxiaobao.xyz/Article/details/gcmevvshs.sHtML

Bash ........... 80
来源：http://3g.fanxiaobao.xyz/Article/details/gcwyplyhb.sHtML

Kotlin ......... 15
来源：http://wap.fanxiaobao.xyz/Article/details/ggsbyuayu.sHtML

Swift .......... 15
来源：http://blog.fanxiaobao.xyz/Article/details/gfpkwywca.sHtML

Lua ............ 10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggehexpbm.sHtML

Perl ........... 10
来源：http://blog.fanxiaobao.xyz/Article/details/gvuzoutwe.sHtML

Scala .......... 10
来源：http://blog.fanxiaobao.xyz/Article/details/gerdcnnam.sHtML

------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtysgjxgt.sHtML

合计 ........... 2106 条
来源：http://www.share.fanxiaobao.xyz/Article/details/gwhxwygxq.sHtML

按章节统计：
来源：http://baike.fanxiaobao.xyz/Article/details/gqcvxyiih.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqtefsdql.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.fanxiaobao.xyz/Article/details/gignyjnbn.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gromnpnyh.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.fanxiaobao.xyz/Article/details/gftlzmfjp.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzfwpnclv.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.fanxiaobao.xyz/Article/details/gmhuupxxg.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.fanxiaobao.xyz/Article/details/gdimuyqjr.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.fanxiaobao.xyz/Article/details/gastojszi.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gckskyppj.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.fanxiaobao.xyz/Article/details/gyuggaeeq.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/gkiyohjqc.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/gtammmpwg.sHtML


<!-- 参考信息 -->