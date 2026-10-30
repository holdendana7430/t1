代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gwqacpjoj.sHtML

[T55] Scala：集合过滤
来源：http://blog.fanxiaobao.xyz/Article/details/ghnxoivaf.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjlhvgvjm.sHtML

[T56] Scala：样例类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaacreebs.sHtML

case class User(name: String, age: Int)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcrhxhjtr.sHtML

[T57] Scala：模式匹配
来源：http://baike.fanxiaobao.xyz/Article/details/glpkdiitk.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.fanxiaobao.xyz/Article/details/gldpgnorl.sHtML

[T58] Scala：函数定义
来源：http://3g.fanxiaobao.xyz/Article/details/gsbmapvte.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.fanxiaobao.xyz/Article/details/gicwtqwjt.sHtML

[T59] Scala：循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gebzfyehv.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsgskaveo.sHtML

[T60] Scala：折叠
来源：http://blog.fanxiaobao.xyz/Article/details/gdcriqlwo.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghvxwymij.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/glrrpssec.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gfeyopftm.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/ghdnhijao.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.fanxiaobao.xyz/Article/details/gvlbqgmyk.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcjlyokqb.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gohoixfiz.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gxuvgziri.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvqxblvsb.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjtecagjp.sHtML

[U04] Py：变量调试打印
来源：http://wap.fanxiaobao.xyz/Article/details/glorhxouy.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkchegnte.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqlnvkfiy.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gptefrbyb.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gwftlsgbr.sHtML

{**a, **b}
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghthnkclf.sHtML

[U07] Py：反转字典键值
来源：http://m.share.fanxiaobao.xyz/Article/details/gsmwaejhj.sHtML

{v: k for k, v in d.items()}
来源：http://baike.fanxiaobao.xyz/Article/details/gxwnguwht.sHtML

[U08] Py：展平二维列表
来源：http://3g.fanxiaobao.xyz/Article/details/gcgzlbped.sHtML

[y for x in nested for y in x]
来源：http://www.share.fanxiaobao.xyz/Article/details/gerczhqvh.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.fanxiaobao.xyz/Article/details/gsvithjsg.sHtML

max(d, key=d.get)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbarpejug.sHtML

[U10] Py：按值排序字典
来源：http://baike.fanxiaobao.xyz/Article/details/gtcuannck.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.fanxiaobao.xyz/Article/details/gchaffzjw.sHtML

[U11] Py：生成器表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gblmbytxu.sHtML

(x * 2 for x in arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gfpeycpkn.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.fanxiaobao.xyz/Article/details/grjlhvfsu.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjngahsan.sHtML

[U13] Py：固定长度队列
来源：http://wap.fanxiaobao.xyz/Article/details/gzijbnxxx.sHtML

deque(maxlen=10)
来源：http://m.share.fanxiaobao.xyz/Article/details/gyfrccgyd.sHtML

[U14] Py：分组收集到列表
来源：http://blog.fanxiaobao.xyz/Article/details/gudggcfoy.sHtML

defaultdict(list)
来源：http://3g.fanxiaobao.xyz/Article/details/gjmurjqxp.sHtML

[U15] Py：高精度计时
来源：http://www.share.fanxiaobao.xyz/Article/details/grtmbudqm.sHtML

t = time.perf_counter()
来源：http://baike.fanxiaobao.xyz/Article/details/gakjzmygg.sHtML

[U16] Py：命令行参数解析
来源：http://blog.fanxiaobao.xyz/Article/details/gbevmkidc.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.fanxiaobao.xyz/Article/details/ghovcdvlk.sHtML

[U17] Py：初始化日志
来源：http://3g.fanxiaobao.xyz/Article/details/gpunblivl.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmzbchrcj.sHtML

[U18] Py：预编译正则
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghmntmvox.sHtML

pat = re.compile(r"\d+")
来源：http://3g.fanxiaobao.xyz/Article/details/gomksdxsv.sHtML

[U19] Py：正则替换带回调
来源：http://3g.fanxiaobao.xyz/Article/details/gesdcoosq.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gefxpyqes.sHtML

[U20] Py：缓存函数结果
来源：http://wap.fanxiaobao.xyz/Article/details/gyciyycwj.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdqdvdxxa.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.fanxiaobao.xyz/Article/details/gkoxifase.sHtML

@contextlib.contextmanager
来源：http://blog.fanxiaobao.xyz/Article/details/gnqyqogio.sHtML

[U22] Py：矩阵转置
来源：http://www.share.fanxiaobao.xyz/Article/details/gljunsgfz.sHtML

list(zip(*m))
来源：http://mobile.fanxiaobao.xyz/Article/details/gjypthiht.sHtML

[U23] Py：分块读取大文件
来源：http://3g.fanxiaobao.xyz/Article/details/gmgugdjmd.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.fanxiaobao.xyz/Article/details/gahgwulhq.sHtML

[U24] Py：路径操作
来源：http://blog.fanxiaobao.xyz/Article/details/gncrjjwpv.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.fanxiaobao.xyz/Article/details/gbytyvdzn.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfiiljzja.sHtML

csv.DictReader(f)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdmkirznx.sHtML

[U26] Py：并发下载
来源：http://baike.fanxiaobao.xyz/Article/details/glxxvpxfl.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gglimevnb.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.fanxiaobao.xyz/Article/details/gfzjxyucj.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfvwnpdzf.sHtML

[U28] Py：类型别名
来源：http://blog.fanxiaobao.xyz/Article/details/ggegefgeo.sHtML

UserId = int
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gubwqkxmu.sHtML

[U29] Py：属性校验
来源：http://3g.fanxiaobao.xyz/Article/details/gukeismqb.sHtML

@property 与 @x.setter 配合
来源：http://mobile.fanxiaobao.xyz/Article/details/glvmmqsmx.sHtML

[U30] Py：数据类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwplnmmzg.sHtML

@dataclass(slots=True)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmrrfcelv.sHtML

[U31] Py：单测
来源：http://baike.fanxiaobao.xyz/Article/details/gmajurgia.sHtML

python -m pytest -q
来源：http://m.share.fanxiaobao.xyz/Article/details/gbxspbjiz.sHtML

[U32] Py：代码格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gdmmpiznk.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.fanxiaobao.xyz/Article/details/gdmzelcyx.sHtML

[U33] Py：打包发布
来源：http://3g.fanxiaobao.xyz/Article/details/grenslmuk.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.fanxiaobao.xyz/Article/details/gtpjnukym.sHtML

[U34] Py：判断编码
来源：http://baike.fanxiaobao.xyz/Article/details/gwuphdhae.sHtML

chardet.detect(raw)
来源：http://blog.fanxiaobao.xyz/Article/details/grunpivqf.sHtML

[U35] Py：发送邮件
来源：http://www.share.fanxiaobao.xyz/Article/details/gxxsuhxyu.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnjbwjzdq.sHtML

[U36] Py：定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gqzgfcemn.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.fanxiaobao.xyz/Article/details/goayavyjz.sHtML

[U37] Py：读写 Excel
来源：http://read.share.fanxiaobao.xyz/Article/details/gkaeizzru.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.fanxiaobao.xyz/Article/details/gnuaseiog.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.fanxiaobao.xyz/Article/details/gnzapfmcj.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.fanxiaobao.xyz/Article/details/grbzdkwjv.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.fanxiaobao.xyz/Article/details/gekcazvnt.sHtML

sys.stdout.isatty()
来源：http://mobile.fanxiaobao.xyz/Article/details/ghjgjstqm.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gsoehvnoa.sHtML

print("err", file=sys.stderr)
来源：http://3g.fanxiaobao.xyz/Article/details/ghnkbhkhi.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.fanxiaobao.xyz/Article/details/gqxisgwsh.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giladyjgg.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.fanxiaobao.xyz/Article/details/ghsgaerrv.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.fanxiaobao.xyz/Article/details/guntbveat.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/gqjjljndv.sHtML

namespace App\Http;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpjijvgfu.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gydkmskbb.sHtML

declare(strict_types=1);
来源：http://www.share.fanxiaobao.xyz/Article/details/gglwenfxs.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.fanxiaobao.xyz/Article/details/gkkfbqgqq.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gahcaqkqm.sHtML

[U46] PHP：可空类型
来源：http://www.share.fanxiaobao.xyz/Article/details/glvwzcyba.sHtML

?string $name = null
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gabieptok.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjhowhdkm.sHtML

int|string $id
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvtmjrqmz.sHtML

[U48] PHP：纯枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gjfjlplzo.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gkkkhckal.sHtML

[U49] PHP：只读属性
来源：http://m.share.fanxiaobao.xyz/Article/details/ggkmbtfly.sHtML

public readonly string $name
来源：http://m.share.fanxiaobao.xyz/Article/details/gtkubmxka.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.fanxiaobao.xyz/Article/details/grutuqutm.sHtML

public function __construct(private int $id) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/ghexpydtr.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqigqmcvf.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqgawoopb.sHtML

[U52] PHP：箭头函数
来源：http://wap.fanxiaobao.xyz/Article/details/gbsjfkjwz.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.fanxiaobao.xyz/Article/details/glfjdmste.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.fanxiaobao.xyz/Article/details/gggmmnyga.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.fanxiaobao.xyz/Article/details/gkmstongb.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjcfdsfxo.sHtML

$obj?->method()
来源：http://www.share.fanxiaobao.xyz/Article/details/gmivzheba.sHtML

[U55] PHP：match 表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gqzzgzbvz.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.fanxiaobao.xyz/Article/details/gzoypqfmz.sHtML

[U56] PHP：命名参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gzfwplwet.sHtML

f(a: 1, b: 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gcrxybvmy.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glehyyyvg.sHtML

"值: {$a}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gayrjrhdx.sHtML

[U58] PHP：数组三件套
来源：http://www.share.fanxiaobao.xyz/Article/details/grnxfkdax.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.fanxiaobao.xyz/Article/details/gorsyiwtv.sHtML

[U59] PHP：自定义排序
来源：http://wap.fanxiaobao.xyz/Article/details/gofuxdrmp.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fanxiaobao.xyz/Article/details/gnirxnfdr.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.fanxiaobao.xyz/Article/details/gssqhpvpu.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.fanxiaobao.xyz/Article/details/gvuknstza.sHtML

[U61] PHP：正则
来源：http://www.share.fanxiaobao.xyz/Article/details/gfkhskjko.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.fanxiaobao.xyz/Article/details/gyupcamnb.sHtML

[U62] PHP：日期对象
来源：http://mobile.fanxiaobao.xyz/Article/details/gsmvuljal.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.fanxiaobao.xyz/Article/details/gddfqzamh.sHtML

[U63] PHP：文件读写
来源：http://mobile.fanxiaobao.xyz/Article/details/gmbhfirwb.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.fanxiaobao.xyz/Article/details/gzrvpltkp.sHtML

[U64] PHP：目录遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gdwdxinnx.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.fanxiaobao.xyz/Article/details/gpaifpfhu.sHtML

[U65] PHP：会话
来源：http://baike.fanxiaobao.xyz/Article/details/grjdghbtt.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gxczudhpt.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.fanxiaobao.xyz/Article/details/gwxibvwvz.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.fanxiaobao.xyz/Article/details/gviagmirn.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.fanxiaobao.xyz/Article/details/glonjhved.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.fanxiaobao.xyz/Article/details/grurwdcnv.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.fanxiaobao.xyz/Article/details/ggfnqbelq.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.fanxiaobao.xyz/Article/details/gwtfhvqkg.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.fanxiaobao.xyz/Article/details/gissxqvfv.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.fanxiaobao.xyz/Article/details/givrewivt.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gsztzoziz.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.fanxiaobao.xyz/Article/details/gdjtixxcw.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glehugckl.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.fanxiaobao.xyz/Article/details/gyrnxmjwi.sHtML

[U72] PHP：写错误日志
来源：http://mobile.fanxiaobao.xyz/Article/details/girmpexft.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.fanxiaobao.xyz/Article/details/gjdlmkctj.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.fanxiaobao.xyz/Article/details/gpjqibszj.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghjzkkcyy.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/ggzmvbepq.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.fanxiaobao.xyz/Article/details/gxmzhekwt.sHtML

[U75] PHP：依赖注入
来源：http://m.share.fanxiaobao.xyz/Article/details/gznlacnse.sHtML

composer require psr/container
来源：http://m.share.fanxiaobao.xyz/Article/details/gonthixkl.sHtML

[U76] PHP：简单路由
来源：http://3g.fanxiaobao.xyz/Article/details/guxkwqwzx.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtipgnwyp.sHtML

[U77] PHP：模板渲染
来源：http://wap.fanxiaobao.xyz/Article/details/gevbqynmt.sHtML

composer require twig/twig
来源：http://m.share.fanxiaobao.xyz/Article/details/geafkwamg.sHtML

[U78] PHP：单元测试
来源：http://blog.fanxiaobao.xyz/Article/details/gfolvqwjm.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.fanxiaobao.xyz/Article/details/gfsmliftm.sHtML

[U79] PHP：静态分析
来源：http://mobile.fanxiaobao.xyz/Article/details/gplwskpzg.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqeephpuf.sHtML

[U80] PHP：代码规范修复
来源：http://3g.fanxiaobao.xyz/Article/details/gazizdgry.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.fanxiaobao.xyz/Article/details/gcdorqmqi.sHtML

[U81] JS：初始化项目
来源：http://baike.fanxiaobao.xyz/Article/details/gkaoknnpq.sHtML

npm init -y;  npm i express
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gouwgwmze.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.fanxiaobao.xyz/Article/details/geyzcesco.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.fanxiaobao.xyz/Article/details/gjhjftnsf.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.fanxiaobao.xyz/Article/details/gizpigxzw.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.fanxiaobao.xyz/Article/details/gzhpvgndk.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.fanxiaobao.xyz/Article/details/gwajwvoxx.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grolczqkt.sHtML

[U85] JS：可选链
来源：http://m.share.fanxiaobao.xyz/Article/details/gscuysmgg.sHtML

a?.b?.c
来源：http://mobile.fanxiaobao.xyz/Article/details/gghfvynve.sHtML

[U86] JS：空值合并
来源：http://read.share.fanxiaobao.xyz/Article/details/gsstuublk.sHtML

a ?? b
来源：http://mobile.fanxiaobao.xyz/Article/details/gstinvvgo.sHtML

[U87] JS：解构默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/ghrlenlef.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.fanxiaobao.xyz/Article/details/gzswtcvbr.sHtML

[U88] JS：对象展开合并
来源：http://m.share.fanxiaobao.xyz/Article/details/gqquayzmc.sHtML

{ ...a, ...b }
来源：http://mobile.fanxiaobao.xyz/Article/details/gsttcphom.sHtML

[U89] JS：数组去重
来源：http://blog.fanxiaobao.xyz/Article/details/gcareyvvc.sHtML

[...new Set(arr)]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsaykqdxz.sHtML

[U90] JS：数字数组排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gmypumdxq.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.fanxiaobao.xyz/Article/details/grpvndimy.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/grcljmett.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.fanxiaobao.xyz/Article/details/gmpngazcq.sHtML

[U92] JS：深拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggxkckqgy.sHtML

structuredClone(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwjcwfqho.sHtML

[U93] JS：模板字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gnqsqocjf.sHtML

`共 ${n} 条`
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbwjevyug.sHtML

[U94] JS：箭头函数
来源：http://baike.fanxiaobao.xyz/Article/details/gfdkahrpj.sHtML

const double = x => x * 2;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdyhbjbfx.sHtML

[U95] JS：Promise 包装
来源：http://m.share.fanxiaobao.xyz/Article/details/guixzvrdg.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.fanxiaobao.xyz/Article/details/gasptzavi.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.fanxiaobao.xyz/Article/details/gnyaoncvz.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gywvakyet.sHtML

[U97] JS：并发请求
来源：http://mobile.fanxiaobao.xyz/Article/details/gwepvpqzt.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fanxiaobao.xyz/Article/details/gezwvcxbr.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/gfjeysrcr.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.fanxiaobao.xyz/Article/details/grcvktcxs.sHtML

[U99] JS：事件监听
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gulablgzi.sHtML

el.addEventListener("click", e => {})
来源：http://3g.fanxiaobao.xyz/Article/details/gwopwxhsl.sHtML

[U100] JS：DOM 查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gtjpjnyas.sHtML

document.querySelector(".item")
来源：http://wap.fanxiaobao.xyz/Article/details/gwswrprkf.sHtML

[U101] JS：classList 操作
来源：http://3g.fanxiaobao.xyz/Article/details/gxuhyargr.sHtML

el.classList.toggle("active")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gysgtnlon.sHtML

[U102] JS：本地存储
来源：http://blog.fanxiaobao.xyz/Article/details/gchnogdbb.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.fanxiaobao.xyz/Article/details/gyjmtwvut.sHtML

[U103] JS：定时器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjmiqvciw.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.fanxiaobao.xyz/Article/details/gifkorsfh.sHtML

[U104] JS：防抖
来源：http://3g.fanxiaobao.xyz/Article/details/gewxpydlu.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fanxiaobao.xyz/Article/details/glmwiiztj.sHtML

[U105] JS：节流
来源：http://wap.fanxiaobao.xyz/Article/details/gufllibgt.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gxqzoibnh.sHtML

[U106] JS：日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gzblzkoyo.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.fanxiaobao.xyz/Article/details/grjhutrrg.sHtML

[U107] JS：数字千分位
来源：http://read.share.fanxiaobao.xyz/Article/details/gssmlckjc.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.fanxiaobao.xyz/Article/details/gevehwfid.sHtML

[U108] JS：随机整数
来源：http://www.share.fanxiaobao.xyz/Article/details/gstlavxoj.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggbvxhtuc.sHtML

[U109] JS：数组分组
来源：http://mobile.fanxiaobao.xyz/Article/details/ghjcpwdzs.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnfwspzzy.sHtML

[U110] JS：数组分块
来源：http://3g.fanxiaobao.xyz/Article/details/gcwqgmmta.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.fanxiaobao.xyz/Article/details/gwwyczbmv.sHtML

[U111] JS：对象转 Map
来源：http://3g.fanxiaobao.xyz/Article/details/ghkjtzwuu.sHtML

new Map(Object.entries(obj))
来源：http://blog.fanxiaobao.xyz/Article/details/goznyxwya.sHtML

[U112] JS：字符串补位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfohejkhj.sHtML

"7".padStart(3, "0")
来源：http://blog.fanxiaobao.xyz/Article/details/gviosxiyh.sHtML

[U113] JS：正则替换全部
来源：http://wap.fanxiaobao.xyz/Article/details/gsefgxkli.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggrgrwwap.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gqbdaovnw.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdmksefgf.sHtML

[U115] JS：生成 UUID
来源：http://mobile.fanxiaobao.xyz/Article/details/gifovjqdb.sHtML

crypto.randomUUID()
来源：http://blog.fanxiaobao.xyz/Article/details/gjmxpnkes.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.fanxiaobao.xyz/Article/details/gbidnfhzh.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gznukqqkv.sHtML

[U117] JS：单元测试
来源：http://3g.fanxiaobao.xyz/Article/details/gofvffwpu.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.fanxiaobao.xyz/Article/details/gubmpyzki.sHtML

[U118] JS：开发服务器
来源：http://blog.fanxiaobao.xyz/Article/details/grseoalpe.sHtML

npm i -D vite;  npx vite
来源：http://3g.fanxiaobao.xyz/Article/details/goxjpyjwk.sHtML

[U119] JS：生产构建
来源：http://m.share.fanxiaobao.xyz/Article/details/gpvvryjqo.sHtML

npx vite build
来源：http://mobile.fanxiaobao.xyz/Article/details/gzsuvllpt.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.fanxiaobao.xyz/Article/details/gbuoxjhqe.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.fanxiaobao.xyz/Article/details/geftweglv.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/galsntipk.sHtML

统计汇总
来源：http://blog.fanxiaobao.xyz/Article/details/grtmsshoh.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gubbsiped.sHtML

按语言统计（条）：
来源：http://mobile.fanxiaobao.xyz/Article/details/gwifneequ.sHtML

Python ......... 252
来源：http://www.share.fanxiaobao.xyz/Article/details/gbempsdnw.sHtML

PHP ............ 252
来源：http://www.share.fanxiaobao.xyz/Article/details/ghknkjevb.sHtML

JavaScript ..... 252
来源：http://wap.fanxiaobao.xyz/Article/details/gsfygeoey.sHtML

TypeScript ..... 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gltbcbwwd.sHtML

Java ........... 212
来源：http://blog.fanxiaobao.xyz/Article/details/gvhdbfrxc.sHtML

Go ............. 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gvtxpnazt.sHtML

Ruby ........... 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gffnctkhj.sHtML

C# ............. 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gmdxvwzdn.sHtML

C .............. 30
来源：http://mobile.fanxiaobao.xyz/Article/details/gwhuthyeu.sHtML

C++ ............ 30
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaxymfbuw.sHtML

SQL ............ 90
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ganqptbnc.sHtML

Bash ........... 80
来源：http://wap.fanxiaobao.xyz/Article/details/grheyethi.sHtML

Kotlin ......... 15
来源：http://baike.fanxiaobao.xyz/Article/details/gpvkqwnbn.sHtML

Swift .......... 15
来源：http://www.share.fanxiaobao.xyz/Article/details/gwpppmbui.sHtML

Lua ............ 10
来源：http://wap.fanxiaobao.xyz/Article/details/gtqgbvrgf.sHtML

Perl ........... 10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvqyyhzxp.sHtML

Scala .......... 10
来源：http://mobile.fanxiaobao.xyz/Article/details/gumnrlfxx.sHtML

------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grthqgwja.sHtML

合计 ........... 2106 条
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywcqoeaq.sHtML

按章节统计：
来源：http://baike.fanxiaobao.xyz/Article/details/gjfyjihmh.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.fanxiaobao.xyz/Article/details/gaajxrqja.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.fanxiaobao.xyz/Article/details/gpjqngovi.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.fanxiaobao.xyz/Article/details/gblojvbet.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.fanxiaobao.xyz/Article/details/ggeztvmfp.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohfricls.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.fanxiaobao.xyz/Article/details/ggusxlyuy.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.fanxiaobao.xyz/Article/details/gtfvelkax.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.fanxiaobao.xyz/Article/details/gkyhlnjhk.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/gdewfujet.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.fanxiaobao.xyz/Article/details/gthdqbvru.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwbmauexx.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/gnvqzlrge.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/galtqkozp.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.fanxiaobao.xyz/Article/details/gxdtkaoyh.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.fanxiaobao.xyz/Article/details/giqlbfzrs.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/grrdjahyo.sHtML

Q SQL 专题                              90
来源：http://read.share.fanxiaobao.xyz/Article/details/gzzphyeln.sHtML

R Bash 专题                             80
来源：http://baike.fanxiaobao.xyz/Article/details/gawftmaly.sHtML

S C / C++ 专题                          60
来源：http://wap.fanxiaobao.xyz/Article/details/gfznfmceo.sHtML

T 其他语言补充                          60
来源：http://wap.fanxiaobao.xyz/Article/details/gikycnclv.sHtML


<!-- 参考信息 -->