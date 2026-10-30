代发 wailian999

val a = 1;  var b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gsfiursro.sHtML

[T53] Scala：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gltuvmmbc.sHtML

s"值: $b"
来源：http://wap.fanxiaobao.xyz/Article/details/gltgpunkn.sHtML

[T54] Scala：集合映射
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaxfskhar.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gihjhrhyn.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gfzuavdgl.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbdmwypkv.sHtML

[T56] Scala：样例类
来源：http://mobile.fanxiaobao.xyz/Article/details/gzoyeaiad.sHtML

case class User(name: String, age: Int)
来源：http://blog.fanxiaobao.xyz/Article/details/gxdufkmmn.sHtML

[T57] Scala：模式匹配
来源：http://blog.fanxiaobao.xyz/Article/details/grvmanupw.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.fanxiaobao.xyz/Article/details/gxmwxkbph.sHtML

[T58] Scala：函数定义
来源：http://mobile.fanxiaobao.xyz/Article/details/ghtvermoh.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.fanxiaobao.xyz/Article/details/gbtscpfgy.sHtML

[T59] Scala：循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gkrmiapzx.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpneqeqqu.sHtML

[T60] Scala：折叠
来源：http://3g.fanxiaobao.xyz/Article/details/gjnzeaatv.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glvpsyqiw.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjwlzjdoj.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghzqbzwwz.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjdoevjsg.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.fanxiaobao.xyz/Article/details/gppocxxju.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.fanxiaobao.xyz/Article/details/gnrauhuzl.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.fanxiaobao.xyz/Article/details/gxipcjxhi.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/ghxmbesen.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.fanxiaobao.xyz/Article/details/gnppyzaid.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.fanxiaobao.xyz/Article/details/gzfgacvwo.sHtML

[U04] Py：变量调试打印
来源：http://baike.fanxiaobao.xyz/Article/details/grhtrcdep.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.fanxiaobao.xyz/Article/details/guvdhoqyk.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.fanxiaobao.xyz/Article/details/gkqmpzqvj.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnrpmtkad.sHtML

[U06] Py：合并两个字典
来源：http://wap.fanxiaobao.xyz/Article/details/gbdvaticc.sHtML

{**a, **b}
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzoffhxc.sHtML

[U07] Py：反转字典键值
来源：http://m.share.fanxiaobao.xyz/Article/details/ghntgcvvx.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.fanxiaobao.xyz/Article/details/gkmrqlzcr.sHtML

[U08] Py：展平二维列表
来源：http://m.share.fanxiaobao.xyz/Article/details/grunkcdwn.sHtML

[y for x in nested for y in x]
来源：http://m.share.fanxiaobao.xyz/Article/details/gjrltxuaj.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.fanxiaobao.xyz/Article/details/gpeuinjkh.sHtML

max(d, key=d.get)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkvosfwed.sHtML

[U10] Py：按值排序字典
来源：http://3g.fanxiaobao.xyz/Article/details/gbuwblxph.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.fanxiaobao.xyz/Article/details/gypmrbqqi.sHtML

[U11] Py：生成器表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gbgznmtdf.sHtML

(x * 2 for x in arr)
来源：http://3g.fanxiaobao.xyz/Article/details/guyumwxjc.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.fanxiaobao.xyz/Article/details/gkbwjbqtw.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gombpxojt.sHtML

[U13] Py：固定长度队列
来源：http://wap.fanxiaobao.xyz/Article/details/grrjbehqx.sHtML

deque(maxlen=10)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbfplxhuc.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsydmbech.sHtML

defaultdict(list)
来源：http://wap.fanxiaobao.xyz/Article/details/gcxpdzgoc.sHtML

[U15] Py：高精度计时
来源：http://mobile.fanxiaobao.xyz/Article/details/gucvqrnrc.sHtML

t = time.perf_counter()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfakhzpiy.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.fanxiaobao.xyz/Article/details/gwascquxh.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.fanxiaobao.xyz/Article/details/gwrzggzky.sHtML

[U17] Py：初始化日志
来源：http://3g.fanxiaobao.xyz/Article/details/gqrfsngpj.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gngaqtoas.sHtML

[U18] Py：预编译正则
来源：http://baike.fanxiaobao.xyz/Article/details/gkdcvmzeg.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnrlkkyji.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqhvxtnoo.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.fanxiaobao.xyz/Article/details/gasbdsqqp.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.fanxiaobao.xyz/Article/details/gxpciakkj.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.fanxiaobao.xyz/Article/details/gskgpooqj.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbxnyrpcd.sHtML

@contextlib.contextmanager
来源：http://m.share.fanxiaobao.xyz/Article/details/gdhnnqoow.sHtML

[U22] Py：矩阵转置
来源：http://read.share.fanxiaobao.xyz/Article/details/gqrghnkmp.sHtML

list(zip(*m))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyrikefxn.sHtML

[U23] Py：分块读取大文件
来源：http://blog.fanxiaobao.xyz/Article/details/genehqskz.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.fanxiaobao.xyz/Article/details/goyzguvri.sHtML

[U24] Py：路径操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwieienxq.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxttlnxvk.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.fanxiaobao.xyz/Article/details/gvasixetm.sHtML

csv.DictReader(f)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcrtdnvvz.sHtML

[U26] Py：并发下载
来源：http://mobile.fanxiaobao.xyz/Article/details/gdplfubov.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqqtnlzbb.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.fanxiaobao.xyz/Article/details/gbhuvmahc.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.fanxiaobao.xyz/Article/details/gpmatvndl.sHtML

[U28] Py：类型别名
来源：http://www.share.fanxiaobao.xyz/Article/details/ghtrlbfyw.sHtML

UserId = int
来源：http://baike.fanxiaobao.xyz/Article/details/gdqkqtfrq.sHtML

[U29] Py：属性校验
来源：http://www.share.fanxiaobao.xyz/Article/details/gdorevrpq.sHtML

@property 与 @x.setter 配合
来源：http://blog.fanxiaobao.xyz/Article/details/gwzyqpdyc.sHtML

[U30] Py：数据类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gonwcmbek.sHtML

@dataclass(slots=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzzdrxdco.sHtML

[U31] Py：单测
来源：http://3g.fanxiaobao.xyz/Article/details/ggftpocvl.sHtML

python -m pytest -q
来源：http://3g.fanxiaobao.xyz/Article/details/gtugixqyj.sHtML

[U32] Py：代码格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gmjuivrpt.sHtML

ruff format . && ruff check --fix .
来源：http://baike.fanxiaobao.xyz/Article/details/gnywhnmey.sHtML

[U33] Py：打包发布
来源：http://m.share.fanxiaobao.xyz/Article/details/grghormjq.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.fanxiaobao.xyz/Article/details/grpitvuem.sHtML

[U34] Py：判断编码
来源：http://mobile.fanxiaobao.xyz/Article/details/gowrgdmay.sHtML

chardet.detect(raw)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwqkdznpl.sHtML

[U35] Py：发送邮件
来源：http://mobile.fanxiaobao.xyz/Article/details/gmkvomedy.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gozocgaag.sHtML

[U36] Py：定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/getdwlmrp.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxplikrnz.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.fanxiaobao.xyz/Article/details/garghyozx.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.fanxiaobao.xyz/Article/details/gvxrrorlo.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fanxiaobao.xyz/Article/details/gsforirts.sHtML

Path(__file__).resolve().parent
来源：http://3g.fanxiaobao.xyz/Article/details/glxvpnskb.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.fanxiaobao.xyz/Article/details/goxqfcwlm.sHtML

sys.stdout.isatty()
来源：http://baike.fanxiaobao.xyz/Article/details/gfxzuthfc.sHtML

[U40] Py：打印到标准错误
来源：http://wap.fanxiaobao.xyz/Article/details/gkkorrptw.sHtML

print("err", file=sys.stderr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbpovedex.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.fanxiaobao.xyz/Article/details/gwhymapmr.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.fanxiaobao.xyz/Article/details/gntpzbist.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.fanxiaobao.xyz/Article/details/gxiwwkipd.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsvhpixjv.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjqxktqxt.sHtML

namespace App\Http;
来源：http://blog.fanxiaobao.xyz/Article/details/gotwylrru.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.fanxiaobao.xyz/Article/details/ganskoojc.sHtML

declare(strict_types=1);
来源：http://mobile.fanxiaobao.xyz/Article/details/geehcwixy.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gcvfrteue.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fanxiaobao.xyz/Article/details/giunzvxfp.sHtML

[U46] PHP：可空类型
来源：http://wap.fanxiaobao.xyz/Article/details/gwnnwuiuf.sHtML

?string $name = null
来源：http://www.share.fanxiaobao.xyz/Article/details/gxyitqzuu.sHtML

[U47] PHP：联合类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gnkdevfyy.sHtML

int|string $id
来源：http://m.share.fanxiaobao.xyz/Article/details/gpneyqeqi.sHtML

[U48] PHP：纯枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gmnvfytjr.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gezreusoy.sHtML

[U49] PHP：只读属性
来源：http://wap.fanxiaobao.xyz/Article/details/glsbxurik.sHtML

public readonly string $name
来源：http://blog.fanxiaobao.xyz/Article/details/gijhfvtqx.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gicoeujeq.sHtML

public function __construct(private int $id) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gbprjqdfw.sHtML

[U51] PHP：数组解构
来源：http://m.share.fanxiaobao.xyz/Article/details/gvusfxkcp.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfsvecnkv.sHtML

[U52] PHP：箭头函数
来源：http://wap.fanxiaobao.xyz/Article/details/gvqvgvvxj.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.fanxiaobao.xyz/Article/details/gmjkokafd.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.fanxiaobao.xyz/Article/details/gjdwtxxxg.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.fanxiaobao.xyz/Article/details/grxyfdjaq.sHtML

[U54] PHP：空安全调用
来源：http://read.share.fanxiaobao.xyz/Article/details/gqnlsvmra.sHtML

$obj?->method()
来源：http://mobile.fanxiaobao.xyz/Article/details/gpxcxtavu.sHtML

[U55] PHP：match 表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gmmmrdnur.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.fanxiaobao.xyz/Article/details/gachawext.sHtML

[U56] PHP：命名参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gxkulgabk.sHtML

f(a: 1, b: 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzfrkxyqz.sHtML

[U57] PHP：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gkrhugdax.sHtML

"值: {$a}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gorngnaob.sHtML

[U58] PHP：数组三件套
来源：http://www.share.fanxiaobao.xyz/Article/details/gwbnudxas.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjkdjgdmz.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gftqhfryg.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjnnpwamh.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmdawxxzb.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.fanxiaobao.xyz/Article/details/gqyevrmry.sHtML

[U61] PHP：正则
来源：http://mobile.fanxiaobao.xyz/Article/details/gwlidgmsk.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqygiuthk.sHtML

[U62] PHP：日期对象
来源：http://3g.fanxiaobao.xyz/Article/details/gupcyjtik.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaezquoqw.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvaonrrxt.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grdgyrymd.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsxnxqsum.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.fanxiaobao.xyz/Article/details/grnviupda.sHtML

[U65] PHP：会话
来源：http://www.blog.fanxiaobao.xyz/Article/details/glkwuqoew.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/ghwkakhxu.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.fanxiaobao.xyz/Article/details/gnchnvnyj.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gnexqtnpo.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.fanxiaobao.xyz/Article/details/guoyrclhm.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.fanxiaobao.xyz/Article/details/gzqotbkev.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdmyqmyqp.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.fanxiaobao.xyz/Article/details/ggslncndy.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjxmypqcj.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtmuonkzz.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gaxcwhxeo.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.fanxiaobao.xyz/Article/details/gejkjkbxl.sHtML

[U71] PHP：抛出异常
来源：http://blog.fanxiaobao.xyz/Article/details/gzytyeaiw.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.fanxiaobao.xyz/Article/details/gqwuvptjw.sHtML

[U72] PHP：写错误日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gvucexmbf.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.fanxiaobao.xyz/Article/details/geahlocak.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.fanxiaobao.xyz/Article/details/gyhrlonhw.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghwvmweee.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gnhqtqskq.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdyfrxlhy.sHtML

[U75] PHP：依赖注入
来源：http://3g.fanxiaobao.xyz/Article/details/gurzeevgf.sHtML

composer require psr/container
来源：http://m.share.fanxiaobao.xyz/Article/details/gvowvrnug.sHtML

[U76] PHP：简单路由
来源：http://mobile.fanxiaobao.xyz/Article/details/gcpyfkfpf.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.fanxiaobao.xyz/Article/details/ggvasjjfm.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gposxoznd.sHtML

composer require twig/twig
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gippudcoa.sHtML

[U78] PHP：单元测试
来源：http://mobile.fanxiaobao.xyz/Article/details/gcggdzwup.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.fanxiaobao.xyz/Article/details/gvumsvhwy.sHtML

[U79] PHP：静态分析
来源：http://read.share.fanxiaobao.xyz/Article/details/gmkxlbmwk.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.fanxiaobao.xyz/Article/details/gqrskavql.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.fanxiaobao.xyz/Article/details/gubfrbprk.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.fanxiaobao.xyz/Article/details/gtpzborjc.sHtML

[U81] JS：初始化项目
来源：http://baike.fanxiaobao.xyz/Article/details/glypekuvn.sHtML

npm init -y;  npm i express
来源：http://www.share.fanxiaobao.xyz/Article/details/gmlmpjirs.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.fanxiaobao.xyz/Article/details/gflsmtimq.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.fanxiaobao.xyz/Article/details/gfywmexod.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.fanxiaobao.xyz/Article/details/grlnwqwkz.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmxnasotb.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.fanxiaobao.xyz/Article/details/gwjkxalke.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.fanxiaobao.xyz/Article/details/goaeuponm.sHtML

[U85] JS：可选链
来源：http://3g.fanxiaobao.xyz/Article/details/grnaqdlqk.sHtML

a?.b?.c
来源：http://mobile.fanxiaobao.xyz/Article/details/gqewqzzuy.sHtML

[U86] JS：空值合并
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjmxwmleu.sHtML

a ?? b
来源：http://m.share.fanxiaobao.xyz/Article/details/ghxbyipnz.sHtML

[U87] JS：解构默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/gcafyjapj.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghlxpnncu.sHtML

[U88] JS：对象展开合并
来源：http://m.share.fanxiaobao.xyz/Article/details/gwkuvmvlb.sHtML

{ ...a, ...b }
来源：http://wap.fanxiaobao.xyz/Article/details/gvroefafy.sHtML

[U89] JS：数组去重
来源：http://3g.fanxiaobao.xyz/Article/details/gabdvzxdl.sHtML

[...new Set(arr)]
来源：http://mobile.fanxiaobao.xyz/Article/details/gymzkalql.sHtML

[U90] JS：数字数组排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gatopvcil.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gucadopzn.sHtML

[U91] JS：对象键值遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gsemfmtan.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.fanxiaobao.xyz/Article/details/gyxvevsbe.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gltcznnct.sHtML

structuredClone(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmeczejcc.sHtML

[U93] JS：模板字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/glycvuuer.sHtML

`共 ${n} 条`
来源：http://www.share.fanxiaobao.xyz/Article/details/gwfffaect.sHtML

[U94] JS：箭头函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gualmdjgb.sHtML

const double = x => x * 2;
来源：http://3g.fanxiaobao.xyz/Article/details/givvhvlqq.sHtML

[U95] JS：Promise 包装
来源：http://blog.fanxiaobao.xyz/Article/details/gflipscac.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.fanxiaobao.xyz/Article/details/glkbyftww.sHtML

[U96] JS：async/await 与异常
来源：http://blog.fanxiaobao.xyz/Article/details/gqcgkcrvg.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.fanxiaobao.xyz/Article/details/gtrbelgaw.sHtML

[U97] JS：并发请求
来源：http://wap.fanxiaobao.xyz/Article/details/ggdxoqzlm.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fanxiaobao.xyz/Article/details/gbpzxontw.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/geozcbwze.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.fanxiaobao.xyz/Article/details/goquctygz.sHtML

[U99] JS：事件监听
来源：http://www.blog.fanxiaobao.xyz/Article/details/gelscjglf.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gclnvcazj.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggcuwnbnr.sHtML

document.querySelector(".item")
来源：http://www.share.fanxiaobao.xyz/Article/details/gfzfhszye.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxqxtcjfx.sHtML

el.classList.toggle("active")
来源：http://wap.fanxiaobao.xyz/Article/details/gvqarpnzc.sHtML

[U102] JS：本地存储
来源：http://wap.fanxiaobao.xyz/Article/details/gohmtvsfi.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.fanxiaobao.xyz/Article/details/gazbiosme.sHtML

[U103] JS：定时器
来源：http://3g.fanxiaobao.xyz/Article/details/gfynscmjq.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvvnlmojg.sHtML

[U104] JS：防抖
来源：http://www.share.fanxiaobao.xyz/Article/details/ghqrzckvq.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/grgfvloep.sHtML

[U105] JS：节流
来源：http://www.share.fanxiaobao.xyz/Article/details/gskrfeqkc.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.fanxiaobao.xyz/Article/details/glwnhjqkr.sHtML

[U106] JS：日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gmjcquqhj.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.fanxiaobao.xyz/Article/details/gcpulmduq.sHtML

[U107] JS：数字千分位
来源：http://mobile.fanxiaobao.xyz/Article/details/gokfabuwn.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.fanxiaobao.xyz/Article/details/gefowwngw.sHtML

[U108] JS：随机整数
来源：http://wap.fanxiaobao.xyz/Article/details/gfvvrszai.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.fanxiaobao.xyz/Article/details/gncuknila.sHtML

[U109] JS：数组分组
来源：http://m.share.fanxiaobao.xyz/Article/details/gyfgdcudd.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzzrrrrdp.sHtML

[U110] JS：数组分块
来源：http://m.share.fanxiaobao.xyz/Article/details/guhsjoeja.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbaogzvys.sHtML

[U111] JS：对象转 Map
来源：http://mobile.fanxiaobao.xyz/Article/details/gygqezaei.sHtML

new Map(Object.entries(obj))
来源：http://3g.fanxiaobao.xyz/Article/details/goreqrkfr.sHtML

[U112] JS：字符串补位
来源：http://mobile.fanxiaobao.xyz/Article/details/guepuabcz.sHtML

"7".padStart(3, "0")
来源：http://baike.fanxiaobao.xyz/Article/details/gppluhdiv.sHtML

[U113] JS：正则替换全部
来源：http://baike.fanxiaobao.xyz/Article/details/gpswnkyfb.sHtML

s.replaceAll("a", "b")
来源：http://blog.fanxiaobao.xyz/Article/details/guuypxfrb.sHtML

[U114] JS：JSON 深比较
来源：http://3g.fanxiaobao.xyz/Article/details/ggodsengj.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdtlaxdga.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnfpsxeeh.sHtML

crypto.randomUUID()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyjtmyovm.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.fanxiaobao.xyz/Article/details/grrkdyrqw.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxjqhpgkh.sHtML

[U117] JS：单元测试
来源：http://read.share.fanxiaobao.xyz/Article/details/gremopxur.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.fanxiaobao.xyz/Article/details/ggtrtvytg.sHtML

[U118] JS：开发服务器
来源：http://www.share.fanxiaobao.xyz/Article/details/gfzfdjuxl.sHtML

npm i -D vite;  npx vite
来源：http://blog.fanxiaobao.xyz/Article/details/grmoijlta.sHtML

[U119] JS：生产构建
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkmqpzmzu.sHtML

npx vite build
来源：http://wap.fanxiaobao.xyz/Article/details/gywkjubif.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghueaxjkg.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.fanxiaobao.xyz/Article/details/gnudqnkmh.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gjffinmna.sHtML

统计汇总
来源：http://3g.fanxiaobao.xyz/Article/details/gjvxlmuxu.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gicjbvqbu.sHtML

按语言统计（条）：
来源：http://www.blog.fanxiaobao.xyz/Article/details/gebaaoklv.sHtML

Python ......... 252
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqlkjmsfg.sHtML

PHP ............ 252
来源：http://3g.fanxiaobao.xyz/Article/details/gylcyidat.sHtML

JavaScript ..... 252
来源：http://m.share.fanxiaobao.xyz/Article/details/gjzjhuain.sHtML

TypeScript ..... 212
来源：http://blog.fanxiaobao.xyz/Article/details/gspfowurb.sHtML

Java ........... 212
来源：http://blog.fanxiaobao.xyz/Article/details/gdgomelkr.sHtML

Go ............. 212
来源：http://baike.fanxiaobao.xyz/Article/details/garfxxajy.sHtML

Ruby ........... 212
来源：http://3g.fanxiaobao.xyz/Article/details/geejdmcxb.sHtML

C# ............. 212
来源：http://m.share.fanxiaobao.xyz/Article/details/grwcexrvo.sHtML

C .............. 30
来源：http://m.share.fanxiaobao.xyz/Article/details/gsecahbbo.sHtML

C++ ............ 30
来源：http://3g.fanxiaobao.xyz/Article/details/gsndpjhww.sHtML

SQL ............ 90
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjzfpzscg.sHtML

Bash ........... 80
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvfyybuxe.sHtML

Kotlin ......... 15
来源：http://wap.fanxiaobao.xyz/Article/details/gsqjguono.sHtML

Swift .......... 15
来源：http://3g.fanxiaobao.xyz/Article/details/gpaubrlwq.sHtML

Lua ............ 10
来源：http://wap.fanxiaobao.xyz/Article/details/gytdeilnr.sHtML

Perl ........... 10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcvjgbocm.sHtML

Scala .......... 10
来源：http://www.share.fanxiaobao.xyz/Article/details/gafxfesim.sHtML

------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/gusfatbtl.sHtML

合计 ........... 2106 条
来源：http://blog.fanxiaobao.xyz/Article/details/gnpyvndoa.sHtML

按章节统计：
来源：http://read.share.fanxiaobao.xyz/Article/details/givpotybp.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.fanxiaobao.xyz/Article/details/glrixvtkl.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.fanxiaobao.xyz/Article/details/giuvmwpcb.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.fanxiaobao.xyz/Article/details/gjsbjkqjy.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.fanxiaobao.xyz/Article/details/ggzkxxtox.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqqlnrcfr.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.fanxiaobao.xyz/Article/details/gasgglxbr.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.fanxiaobao.xyz/Article/details/ghcimybio.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.fanxiaobao.xyz/Article/details/ghahqvytb.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/ghlqdgtvh.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.fanxiaobao.xyz/Article/details/ghddnyvfj.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/glyaicimq.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/gamgrwpzh.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/glhuxphbz.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.fanxiaobao.xyz/Article/details/gsdylglvm.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.fanxiaobao.xyz/Article/details/ganbixuoe.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gohuwkfwi.sHtML


<!-- 参考信息 -->