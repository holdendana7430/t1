代发 wailian999

val a = 1;  var b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gxuqjljlp.sHtML

[T53] Scala：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gjcqdqozs.sHtML

s"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/glyovjeit.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gswawpdqs.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gngmtklhy.sHtML

[T55] Scala：集合过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gaoonxatg.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/grsjyjjom.sHtML

[T56] Scala：样例类
来源：http://read.share.fanxiaobao.xyz/Article/details/gegxbmaxx.sHtML

case class User(name: String, age: Int)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghgogqjmo.sHtML

[T57] Scala：模式匹配
来源：http://3g.fanxiaobao.xyz/Article/details/goddayffh.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.fanxiaobao.xyz/Article/details/gdylmusof.sHtML

[T58] Scala：函数定义
来源：http://3g.fanxiaobao.xyz/Article/details/gdfngmhid.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.fanxiaobao.xyz/Article/details/glncjmllh.sHtML

[T59] Scala：循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gxvcyoejx.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.fanxiaobao.xyz/Article/details/glsrgxhff.sHtML

[T60] Scala：折叠
来源：http://wap.fanxiaobao.xyz/Article/details/gojaoszjk.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.fanxiaobao.xyz/Article/details/ggyotopok.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gplhdhvur.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/guaokceab.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gabotxvgl.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.fanxiaobao.xyz/Article/details/gemmjvrmb.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.fanxiaobao.xyz/Article/details/gvwybdyim.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.fanxiaobao.xyz/Article/details/gpqjofqmy.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwqglhrow.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzzwlskay.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.fanxiaobao.xyz/Article/details/gfnrvurcq.sHtML

[U04] Py：变量调试打印
来源：http://m.share.fanxiaobao.xyz/Article/details/ggippouug.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fanxiaobao.xyz/Article/details/gbjwbxidf.sHtML

[U05] Py：列表去重且保序
来源：http://blog.fanxiaobao.xyz/Article/details/gkynaeqwk.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.fanxiaobao.xyz/Article/details/geirmuscv.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gikgbbzjz.sHtML

{**a, **b}
来源：http://m.share.fanxiaobao.xyz/Article/details/gsvcwlwyi.sHtML

[U07] Py：反转字典键值
来源：http://wap.fanxiaobao.xyz/Article/details/gltelfmhc.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fanxiaobao.xyz/Article/details/grrmdhynm.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gipblwoox.sHtML

[y for x in nested for y in x]
来源：http://www.share.fanxiaobao.xyz/Article/details/gxjyrsjnw.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.fanxiaobao.xyz/Article/details/gyuvswgzv.sHtML

max(d, key=d.get)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvtefzpaz.sHtML

[U10] Py：按值排序字典
来源：http://m.share.fanxiaobao.xyz/Article/details/gstctyofz.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.fanxiaobao.xyz/Article/details/gyxsohubd.sHtML

[U11] Py：生成器表达式
来源：http://baike.fanxiaobao.xyz/Article/details/ghfzjwpkz.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gggsenloi.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.fanxiaobao.xyz/Article/details/ghqiaszdn.sHtML

Counter(arr).most_common(3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsvfyvosb.sHtML

[U13] Py：固定长度队列
来源：http://read.share.fanxiaobao.xyz/Article/details/gxtwxbogy.sHtML

deque(maxlen=10)
来源：http://blog.fanxiaobao.xyz/Article/details/gflvzkqra.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.fanxiaobao.xyz/Article/details/giwvwaocr.sHtML

defaultdict(list)
来源：http://mobile.fanxiaobao.xyz/Article/details/gylhbsjcq.sHtML

[U15] Py：高精度计时
来源：http://read.share.fanxiaobao.xyz/Article/details/gxfdlwgsr.sHtML

t = time.perf_counter()
来源：http://mobile.fanxiaobao.xyz/Article/details/gawbiuldl.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.fanxiaobao.xyz/Article/details/gkqftpfjx.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.fanxiaobao.xyz/Article/details/gkwdpiicg.sHtML

[U17] Py：初始化日志
来源：http://blog.fanxiaobao.xyz/Article/details/gtxzlocra.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaanptnkf.sHtML

[U18] Py：预编译正则
来源：http://read.share.fanxiaobao.xyz/Article/details/gpomygiut.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/gmpxrudgb.sHtML

[U19] Py：正则替换带回调
来源：http://wap.fanxiaobao.xyz/Article/details/gdugjzkma.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.fanxiaobao.xyz/Article/details/gamaygxnd.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.fanxiaobao.xyz/Article/details/gbqywnmcp.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaxfgisfo.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.fanxiaobao.xyz/Article/details/gseujezjh.sHtML

@contextlib.contextmanager
来源：http://wap.fanxiaobao.xyz/Article/details/gfzwfvclr.sHtML

[U22] Py：矩阵转置
来源：http://blog.fanxiaobao.xyz/Article/details/glddwmfvo.sHtML

list(zip(*m))
来源：http://m.share.fanxiaobao.xyz/Article/details/gfbjjzjmi.sHtML

[U23] Py：分块读取大文件
来源：http://wap.fanxiaobao.xyz/Article/details/gjrpjwxce.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.fanxiaobao.xyz/Article/details/guglltctw.sHtML

[U24] Py：路径操作
来源：http://baike.fanxiaobao.xyz/Article/details/gtqipgict.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggmaqrxrj.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.fanxiaobao.xyz/Article/details/gyolbccnv.sHtML

csv.DictReader(f)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzgbpxrdx.sHtML

[U26] Py：并发下载
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwndwnikc.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvwctxerj.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fanxiaobao.xyz/Article/details/ghfjyxasr.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.fanxiaobao.xyz/Article/details/guggajadz.sHtML

[U28] Py：类型别名
来源：http://baike.fanxiaobao.xyz/Article/details/gkrhyjdry.sHtML

UserId = int
来源：http://www.share.fanxiaobao.xyz/Article/details/gqotojqqm.sHtML

[U29] Py：属性校验
来源：http://m.share.fanxiaobao.xyz/Article/details/ghqitwcsm.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmxsmldzs.sHtML

[U30] Py：数据类
来源：http://3g.fanxiaobao.xyz/Article/details/gaawtsvmv.sHtML

@dataclass(slots=True)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grhfqpsgc.sHtML

[U31] Py：单测
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxvwisaxz.sHtML

python -m pytest -q
来源：http://www.share.fanxiaobao.xyz/Article/details/gxkyrvcls.sHtML

[U32] Py：代码格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gotayqtpp.sHtML

ruff format . && ruff check --fix .
来源：http://3g.fanxiaobao.xyz/Article/details/gqygukaki.sHtML

[U33] Py：打包发布
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gedosuapz.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjnjpwgzc.sHtML

[U34] Py：判断编码
来源：http://blog.fanxiaobao.xyz/Article/details/glzbaltiy.sHtML

chardet.detect(raw)
来源：http://3g.fanxiaobao.xyz/Article/details/ggvgumrrp.sHtML

[U35] Py：发送邮件
来源：http://www.share.fanxiaobao.xyz/Article/details/gqzrzjxyk.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.fanxiaobao.xyz/Article/details/grodsgais.sHtML

[U36] Py：定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/ghbqqpmsf.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.fanxiaobao.xyz/Article/details/ganygziku.sHtML

[U37] Py：读写 Excel
来源：http://wap.fanxiaobao.xyz/Article/details/grjdirstw.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.fanxiaobao.xyz/Article/details/graenwewj.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fanxiaobao.xyz/Article/details/grkyhpkts.sHtML

Path(__file__).resolve().parent
来源：http://read.share.fanxiaobao.xyz/Article/details/gbzwdkcsz.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.fanxiaobao.xyz/Article/details/goyswdgic.sHtML

sys.stdout.isatty()
来源：http://mobile.fanxiaobao.xyz/Article/details/gjibmbbaf.sHtML

[U40] Py：打印到标准错误
来源：http://wap.fanxiaobao.xyz/Article/details/ghqgjmsnb.sHtML

print("err", file=sys.stderr)
来源：http://wap.fanxiaobao.xyz/Article/details/gdhaesoil.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.fanxiaobao.xyz/Article/details/gcokguqen.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.fanxiaobao.xyz/Article/details/gveunruan.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.fanxiaobao.xyz/Article/details/ghdipilvd.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzszsceds.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/gjlzofaxz.sHtML

namespace App\Http;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtcrocjhe.sHtML

[U44] PHP：开启严格类型
来源：http://baike.fanxiaobao.xyz/Article/details/gbewejqtk.sHtML

declare(strict_types=1);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzukbggvv.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghncfpqkr.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gasrneviv.sHtML

[U46] PHP：可空类型
来源：http://baike.fanxiaobao.xyz/Article/details/gnouorhzw.sHtML

?string $name = null
来源：http://read.share.fanxiaobao.xyz/Article/details/gpzmzxceh.sHtML

[U47] PHP：联合类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gydyrocde.sHtML

int|string $id
来源：http://3g.fanxiaobao.xyz/Article/details/gcwxtaxjt.sHtML

[U48] PHP：纯枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gzllijapp.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gfbaeyafb.sHtML

[U49] PHP：只读属性
来源：http://www.share.fanxiaobao.xyz/Article/details/gaalfeenj.sHtML

public readonly string $name
来源：http://blog.fanxiaobao.xyz/Article/details/gfixieqfu.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.fanxiaobao.xyz/Article/details/gnrvmisuv.sHtML

public function __construct(private int $id) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gcmtbvtpd.sHtML

[U51] PHP：数组解构
来源：http://m.share.fanxiaobao.xyz/Article/details/guqnkmhlz.sHtML

[$a, $b] = $arr;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjnxexfgz.sHtML

[U52] PHP：箭头函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gfvscgtmn.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.fanxiaobao.xyz/Article/details/gvradehld.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.fanxiaobao.xyz/Article/details/glryzmbra.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.fanxiaobao.xyz/Article/details/gftlbwvdv.sHtML

[U54] PHP：空安全调用
来源：http://3g.fanxiaobao.xyz/Article/details/ghdkpbcxh.sHtML

$obj?->method()
来源：http://www.blog.fanxiaobao.xyz/Article/details/grtvlozrk.sHtML

[U55] PHP：match 表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gnvqwztgo.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.fanxiaobao.xyz/Article/details/ggfitvemo.sHtML

[U56] PHP：命名参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmjeygsz.sHtML

f(a: 1, b: 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxoxhpdjs.sHtML

[U57] PHP：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/glnrsdgue.sHtML

"值: {$a}"
来源：http://wap.fanxiaobao.xyz/Article/details/gxsrvsezq.sHtML

[U58] PHP：数组三件套
来源：http://wap.fanxiaobao.xyz/Article/details/gvuwhaxnz.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.fanxiaobao.xyz/Article/details/gkaonhvrp.sHtML

[U59] PHP：自定义排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gkqpeydrd.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fanxiaobao.xyz/Article/details/gqsorxhgi.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.fanxiaobao.xyz/Article/details/gfejtdhtq.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.fanxiaobao.xyz/Article/details/gfjnkyikt.sHtML

[U61] PHP：正则
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbnaomfwi.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.fanxiaobao.xyz/Article/details/gryqrorhw.sHtML

[U62] PHP：日期对象
来源：http://wap.fanxiaobao.xyz/Article/details/gwfgutnpg.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.fanxiaobao.xyz/Article/details/gihoidpwv.sHtML

[U63] PHP：文件读写
来源：http://baike.fanxiaobao.xyz/Article/details/ggkopzety.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.fanxiaobao.xyz/Article/details/gxupjdmmz.sHtML

[U64] PHP：目录遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gsmupfqff.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.fanxiaobao.xyz/Article/details/gcmdlocvt.sHtML

[U65] PHP：会话
来源：http://www.share.fanxiaobao.xyz/Article/details/ghtmbmbrd.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/guxsvmhlp.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.fanxiaobao.xyz/Article/details/gbgykgiod.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdgoacpfq.sHtML

[U67] PHP：处理文件上传
来源：http://3g.fanxiaobao.xyz/Article/details/gjknmjcdc.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glgryqjyf.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giclqykpl.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.fanxiaobao.xyz/Article/details/gkamhdjib.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjlatrwmz.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.fanxiaobao.xyz/Article/details/gztwmkucr.sHtML

[U70] PHP：PDO 事务
来源：http://baike.fanxiaobao.xyz/Article/details/gbbfpoowh.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpluweaji.sHtML

[U71] PHP：抛出异常
来源：http://read.share.fanxiaobao.xyz/Article/details/gtjixlozi.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvvvlvyji.sHtML

[U72] PHP：写错误日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gxlbtazby.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqfgntfuu.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwrywlncx.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.fanxiaobao.xyz/Article/details/gjgqjqhlj.sHtML

[U74] PHP：读取环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/gdkeomohk.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.fanxiaobao.xyz/Article/details/gcmttdxpt.sHtML

[U75] PHP：依赖注入
来源：http://baike.fanxiaobao.xyz/Article/details/gwtpsvzph.sHtML

composer require psr/container
来源：http://www.share.fanxiaobao.xyz/Article/details/goqduhwtn.sHtML

[U76] PHP：简单路由
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtrfbvpab.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.fanxiaobao.xyz/Article/details/gaecvsjfi.sHtML

[U77] PHP：模板渲染
来源：http://3g.fanxiaobao.xyz/Article/details/gzzpuuika.sHtML

composer require twig/twig
来源：http://wap.fanxiaobao.xyz/Article/details/gaqcqqgfz.sHtML

[U78] PHP：单元测试
来源：http://wap.fanxiaobao.xyz/Article/details/gdzkloamk.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.fanxiaobao.xyz/Article/details/gnkxcflmo.sHtML

[U79] PHP：静态分析
来源：http://wap.fanxiaobao.xyz/Article/details/gzchbwvsd.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.fanxiaobao.xyz/Article/details/gjdvornte.sHtML

[U80] PHP：代码规范修复
来源：http://3g.fanxiaobao.xyz/Article/details/gafnvgpqp.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtsdittsc.sHtML

[U81] JS：初始化项目
来源：http://read.share.fanxiaobao.xyz/Article/details/gmegbxgud.sHtML

npm init -y;  npm i express
来源：http://3g.fanxiaobao.xyz/Article/details/gvokmgzrj.sHtML

[U82] JS：package.json 脚本
来源：http://wap.fanxiaobao.xyz/Article/details/ggrlucexi.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxttlhqog.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.fanxiaobao.xyz/Article/details/gndbvvszd.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.fanxiaobao.xyz/Article/details/gegtwbxpa.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.fanxiaobao.xyz/Article/details/glnhwzjla.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcbsuveil.sHtML

[U85] JS：可选链
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gngdrlmqt.sHtML

a?.b?.c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxfiquujr.sHtML

[U86] JS：空值合并
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwvdeiqtk.sHtML

a ?? b
来源：http://read.share.fanxiaobao.xyz/Article/details/gnmfgdpfg.sHtML

[U87] JS：解构默认值
来源：http://wap.fanxiaobao.xyz/Article/details/gqqugcxdb.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.fanxiaobao.xyz/Article/details/gppybtlzg.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.fanxiaobao.xyz/Article/details/gftipbgfn.sHtML

{ ...a, ...b }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwgaaoems.sHtML

[U89] JS：数组去重
来源：http://wap.fanxiaobao.xyz/Article/details/ghzayyfru.sHtML

[...new Set(arr)]
来源：http://www.share.fanxiaobao.xyz/Article/details/gnhhpfxzh.sHtML

[U90] JS：数字数组排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gfvmkrgvd.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwtappkds.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gafyxfxzl.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.fanxiaobao.xyz/Article/details/gzgqtycgo.sHtML

[U92] JS：深拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gjvzufppo.sHtML

structuredClone(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gosutmwal.sHtML

[U93] JS：模板字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gwklbqbmc.sHtML

`共 ${n} 条`
来源：http://www.share.fanxiaobao.xyz/Article/details/geltwqslw.sHtML

[U94] JS：箭头函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvordtmpw.sHtML

const double = x => x * 2;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxigdlmvp.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gghmnrtal.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.fanxiaobao.xyz/Article/details/givqgdtrf.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.fanxiaobao.xyz/Article/details/gmygnvawq.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpatqzxwz.sHtML

[U97] JS：并发请求
来源：http://read.share.fanxiaobao.xyz/Article/details/gewtlzpud.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guasibzkl.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqxwoqhnx.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.fanxiaobao.xyz/Article/details/gdveayjie.sHtML

[U99] JS：事件监听
来源：http://3g.fanxiaobao.xyz/Article/details/gfmpzzzzj.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grgmvejya.sHtML

[U100] JS：DOM 查询
来源：http://3g.fanxiaobao.xyz/Article/details/gdcmhnczj.sHtML

document.querySelector(".item")
来源：http://www.share.fanxiaobao.xyz/Article/details/gihmmdiwd.sHtML

[U101] JS：classList 操作
来源：http://3g.fanxiaobao.xyz/Article/details/gfbrcsdlb.sHtML

el.classList.toggle("active")
来源：http://www.share.fanxiaobao.xyz/Article/details/gyrqlkcua.sHtML

[U102] JS：本地存储
来源：http://blog.fanxiaobao.xyz/Article/details/gkpcaiwac.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.fanxiaobao.xyz/Article/details/giziwmset.sHtML

[U103] JS：定时器
来源：http://www.share.fanxiaobao.xyz/Article/details/gemiwnxkd.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvskzznjk.sHtML

[U104] JS：防抖
来源：http://m.share.fanxiaobao.xyz/Article/details/gqkrlgmxy.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gngghxbhb.sHtML

[U105] JS：节流
来源：http://3g.fanxiaobao.xyz/Article/details/giksbkscb.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gfglozntg.sHtML

[U106] JS：日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/glkqmvcqh.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpjrobkfg.sHtML

[U107] JS：数字千分位
来源：http://baike.fanxiaobao.xyz/Article/details/gqsghuxol.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.fanxiaobao.xyz/Article/details/guknjurmm.sHtML

[U108] JS：随机整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfyaxsaqj.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdmeaammj.sHtML

[U109] JS：数组分组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwtrezwbz.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnianotfi.sHtML

[U110] JS：数组分块
来源：http://www.share.fanxiaobao.xyz/Article/details/gaeybtqlc.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.fanxiaobao.xyz/Article/details/gurckcfze.sHtML

[U111] JS：对象转 Map
来源：http://mobile.fanxiaobao.xyz/Article/details/gehzywril.sHtML

new Map(Object.entries(obj))
来源：http://www.share.fanxiaobao.xyz/Article/details/gmwiputdx.sHtML

[U112] JS：字符串补位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyoxtuciu.sHtML

"7".padStart(3, "0")
来源：http://www.share.fanxiaobao.xyz/Article/details/gpvcsugkc.sHtML

[U113] JS：正则替换全部
来源：http://3g.fanxiaobao.xyz/Article/details/gwvivvepq.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjzhcxrmp.sHtML

[U114] JS：JSON 深比较
来源：http://baike.fanxiaobao.xyz/Article/details/gckelkuep.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fanxiaobao.xyz/Article/details/glvvumors.sHtML

[U115] JS：生成 UUID
来源：http://wap.fanxiaobao.xyz/Article/details/gvvsutwdv.sHtML

crypto.randomUUID()
来源：http://wap.fanxiaobao.xyz/Article/details/gudytvfnh.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.fanxiaobao.xyz/Article/details/gkysueqqt.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gmiorjgcw.sHtML

[U117] JS：单元测试
来源：http://3g.fanxiaobao.xyz/Article/details/gufkivdyf.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.fanxiaobao.xyz/Article/details/gwwwajzoz.sHtML

[U118] JS：开发服务器
来源：http://m.share.fanxiaobao.xyz/Article/details/gidxhhoyz.sHtML

npm i -D vite;  npx vite
来源：http://baike.fanxiaobao.xyz/Article/details/gyncikzzl.sHtML

[U119] JS：生产构建
来源：http://blog.fanxiaobao.xyz/Article/details/gaslvgdlk.sHtML

npx vite build
来源：http://mobile.fanxiaobao.xyz/Article/details/giibsjeux.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.fanxiaobao.xyz/Article/details/gewwtxsdg.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.fanxiaobao.xyz/Article/details/gbzcbcotd.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/glbszbbuz.sHtML

统计汇总
来源：http://m.share.fanxiaobao.xyz/Article/details/gihcfivxu.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gzsjofwnt.sHtML

按语言统计（条）：
来源：http://baike.fanxiaobao.xyz/Article/details/gurwewccw.sHtML

Python ......... 252
来源：http://baike.fanxiaobao.xyz/Article/details/giqjuazat.sHtML

PHP ............ 252
来源：http://wap.fanxiaobao.xyz/Article/details/gonbxgznj.sHtML

JavaScript ..... 252
来源：http://mobile.fanxiaobao.xyz/Article/details/ggiucoeog.sHtML

TypeScript ..... 212
来源：http://blog.fanxiaobao.xyz/Article/details/gnpapbzgu.sHtML

Java ........... 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gxeylnxsw.sHtML

Go ............. 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxyntbciy.sHtML

Ruby ........... 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gprrfryjg.sHtML

C# ............. 212
来源：http://mobile.fanxiaobao.xyz/Article/details/goapgbbst.sHtML

C .............. 30
来源：http://www.share.fanxiaobao.xyz/Article/details/gayykcivm.sHtML

C++ ............ 30
来源：http://read.share.fanxiaobao.xyz/Article/details/gkkfjflns.sHtML

SQL ............ 90
来源：http://baike.fanxiaobao.xyz/Article/details/gmxqmxqya.sHtML

Bash ........... 80
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghqtafdgh.sHtML

Kotlin ......... 15
来源：http://baike.fanxiaobao.xyz/Article/details/giqjozrin.sHtML

Swift .......... 15
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbqfzslzb.sHtML

Lua ............ 10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gchbbmfqy.sHtML

Perl ........... 10
来源：http://m.share.fanxiaobao.xyz/Article/details/gpjojfnif.sHtML

Scala .......... 10
来源：http://read.share.fanxiaobao.xyz/Article/details/gmoobkliy.sHtML

------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/glaxnluwp.sHtML

合计 ........... 2106 条
来源：http://wap.fanxiaobao.xyz/Article/details/grmkmdtte.sHtML

按章节统计：
来源：http://read.share.fanxiaobao.xyz/Article/details/gzbuldfiz.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmuvllhl.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.fanxiaobao.xyz/Article/details/gaaeuwyxh.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.fanxiaobao.xyz/Article/details/gumeatziz.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.fanxiaobao.xyz/Article/details/geeadomkc.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.fanxiaobao.xyz/Article/details/gipkjqitk.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdaychxvy.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.fanxiaobao.xyz/Article/details/gqelosmsa.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.fanxiaobao.xyz/Article/details/gshdkrjzf.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/gqgqyreju.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.fanxiaobao.xyz/Article/details/gbjpjrcwe.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/gbsvjhura.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gkaqsnfhg.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/gfptbqvog.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjovzmbm.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.fanxiaobao.xyz/Article/details/gfzmcpeyn.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gxtiwodwl.sHtML


<!-- 参考信息 -->