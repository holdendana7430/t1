代发 wailian999

while (my $line = <$fh>) { print $line; }
来源：http://read.share.zdbjq.cn/Article/details/ggbekdclw.sHtML

[T51] Scala：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gcsprjdsk.sHtML

println("Hello")
来源：http://3g.fehbvm.com/Article/details/grdvhgpmt.sHtML

[T52] Scala：变量
来源：http://read.share.fehbvm.com/Article/details/ggahsqpzf.sHtML

val a = 1;  var b = 2
来源：http://www.share.zdbjq.cn/Article/details/ggywepqmf.sHtML

[T53] Scala：字符串插值
来源：http://blog.hesvh.cn/Article/details/gzdsldoiy.sHtML

s"值: $b"
来源：http://m.share.fehbvm.com/Article/details/gxumworrn.sHtML

[T54] Scala：集合映射
来源：http://read.share.zdbjq.cn/Article/details/galizamlv.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.zdbjq.cn/Article/details/gogzigjnd.sHtML

[T55] Scala：集合过滤
来源：http://wap.fehbvm.com/Article/details/gzryekxhi.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.fehbvm.com/Article/details/gynkatvus.sHtML

[T56] Scala：样例类
来源：http://read.share.fehbvm.com/Article/details/gzdhjfcio.sHtML

case class User(name: String, age: Int)
来源：http://m.share.hesvh.cn/Article/details/gkjstwhzx.sHtML

[T57] Scala：模式匹配
来源：http://mobile.zdbjq.cn/Article/details/goyxkudtq.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.hesvh.cn/Article/details/gfhmekcpo.sHtML

[T58] Scala：函数定义
来源：http://3g.zdbjq.cn/Article/details/gidllizif.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.zdbjq.cn/Article/details/gtdbtmjhw.sHtML

[T59] Scala：循环
来源：http://blog.hesvh.cn/Article/details/gslfovxrr.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.zdbjq.cn/Article/details/gudqhpkso.sHtML

[T60] Scala：折叠
来源：http://www.blog.zdbjq.cn/Article/details/gujimjbhr.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.hesvh.cn/Article/details/gkloyayko.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gfiyoxygf.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.zdbjq.cn/Article/details/guwatqpsp.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gmzgfmrxn.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.fehbvm.com/Article/details/gkhhatgbf.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.hesvh.cn/Article/details/gdgubjjvk.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.zdbjq.cn/Article/details/guxgoislz.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.zdbjq.cn/Article/details/gvpthzunk.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.hesvh.cn/Article/details/guhtczttd.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.fehbvm.com/Article/details/gnviunmnz.sHtML

[U04] Py：变量调试打印
来源：http://blog.zdbjq.cn/Article/details/gpklwhyhw.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.hesvh.cn/Article/details/gdltkdofz.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.hesvh.cn/Article/details/gulgxakoz.sHtML

list(dict.fromkeys(arr))
来源：http://blog.zdbjq.cn/Article/details/gglxobhhp.sHtML

[U06] Py：合并两个字典
来源：http://m.share.zdbjq.cn/Article/details/gifbeysex.sHtML

{**a, **b}
来源：http://www.blog.hesvh.cn/Article/details/gqksehiwy.sHtML

[U07] Py：反转字典键值
来源：http://www.share.zdbjq.cn/Article/details/gzsqwgsfs.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.zdbjq.cn/Article/details/gmhphbvpt.sHtML

[U08] Py：展平二维列表
来源：http://wap.hesvh.cn/Article/details/gcyddzido.sHtML

[y for x in nested for y in x]
来源：http://blog.fehbvm.com/Article/details/giopnpyoe.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.zdbjq.cn/Article/details/ghlymkqkv.sHtML

max(d, key=d.get)
来源：http://mobile.fehbvm.com/Article/details/gxeojwsgt.sHtML

[U10] Py：按值排序字典
来源：http://read.share.zdbjq.cn/Article/details/gepixhjyz.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.fehbvm.com/Article/details/gmlemghtq.sHtML

[U11] Py：生成器表达式
来源：http://blog.zdbjq.cn/Article/details/gjgfwrmqa.sHtML

(x * 2 for x in arr)
来源：http://wap.fehbvm.com/Article/details/gjvmuyypb.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.zdbjq.cn/Article/details/glhfhfxpf.sHtML

Counter(arr).most_common(3)
来源：http://wap.hesvh.cn/Article/details/gzwkexmjj.sHtML

[U13] Py：固定长度队列
来源：http://m.share.fehbvm.com/Article/details/gcqgkydgo.sHtML

deque(maxlen=10)
来源：http://www.blog.fehbvm.com/Article/details/gtroqsswx.sHtML

[U14] Py：分组收集到列表
来源：http://wap.fehbvm.com/Article/details/gukpblwqk.sHtML

defaultdict(list)
来源：http://3g.fehbvm.com/Article/details/gxxwazgqb.sHtML

[U15] Py：高精度计时
来源：http://wap.hesvh.cn/Article/details/gfmftegli.sHtML

t = time.perf_counter()
来源：http://baike.fehbvm.com/Article/details/gzhnyiyzu.sHtML

[U16] Py：命令行参数解析
来源：http://blog.fehbvm.com/Article/details/gkzrkepwh.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.fehbvm.com/Article/details/ghwdvqeyl.sHtML

[U17] Py：初始化日志
来源：http://www.blog.fehbvm.com/Article/details/ghsyzribl.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.hesvh.cn/Article/details/ggmrorujr.sHtML

[U18] Py：预编译正则
来源：http://3g.hesvh.cn/Article/details/gpgjwzbgr.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.hesvh.cn/Article/details/gsjrfqndc.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.hesvh.cn/Article/details/gbmdnhgxx.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.fehbvm.com/Article/details/gukcecgvw.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.zdbjq.cn/Article/details/gfdifnsvp.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.zdbjq.cn/Article/details/gyhavteql.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.hesvh.cn/Article/details/grofedcvb.sHtML

@contextlib.contextmanager
来源：http://read.share.fehbvm.com/Article/details/gymcmmmxv.sHtML

[U22] Py：矩阵转置
来源：http://m.share.zdbjq.cn/Article/details/gttjesjsy.sHtML

list(zip(*m))
来源：http://www.share.fehbvm.com/Article/details/gzrgrltuu.sHtML

[U23] Py：分块读取大文件
来源：http://blog.zdbjq.cn/Article/details/gjegdjylq.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.zdbjq.cn/Article/details/gifaiclvs.sHtML

[U24] Py：路径操作
来源：http://m.share.fehbvm.com/Article/details/gaotyvojj.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.fehbvm.com/Article/details/gmyudftnq.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.fehbvm.com/Article/details/gpsitlnxl.sHtML

csv.DictReader(f)
来源：http://mobile.hesvh.cn/Article/details/gnpgscqcn.sHtML

[U26] Py：并发下载
来源：http://wap.zdbjq.cn/Article/details/gttvgkimn.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.fehbvm.com/Article/details/glbodnctg.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.hesvh.cn/Article/details/gukiuxsue.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.zdbjq.cn/Article/details/gpujmwrcn.sHtML

[U28] Py：类型别名
来源：http://wap.fehbvm.com/Article/details/goevcptvi.sHtML

UserId = int
来源：http://baike.zdbjq.cn/Article/details/gpqpiygvf.sHtML

[U29] Py：属性校验
来源：http://www.share.zdbjq.cn/Article/details/gylkadgux.sHtML

@property 与 @x.setter 配合
来源：http://baike.hesvh.cn/Article/details/gtdhdxpos.sHtML

[U30] Py：数据类
来源：http://mobile.zdbjq.cn/Article/details/ggygqowwd.sHtML

@dataclass(slots=True)
来源：http://3g.hesvh.cn/Article/details/gqupphczv.sHtML

[U31] Py：单测
来源：http://3g.fehbvm.com/Article/details/gsoscamye.sHtML

python -m pytest -q
来源：http://m.share.fehbvm.com/Article/details/ghyeucjda.sHtML

[U32] Py：代码格式化
来源：http://www.share.fehbvm.com/Article/details/gjcwkagla.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.hesvh.cn/Article/details/gvwklyptz.sHtML

[U33] Py：打包发布
来源：http://www.m.share.zdbjq.cn/Article/details/gqeglvyzc.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.hesvh.cn/Article/details/gcrtdhsri.sHtML

[U34] Py：判断编码
来源：http://www.blog.zdbjq.cn/Article/details/gclylwsqk.sHtML

chardet.detect(raw)
来源：http://www.blog.zdbjq.cn/Article/details/guustgybz.sHtML

[U35] Py：发送邮件
来源：http://wap.zdbjq.cn/Article/details/gulysnliu.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.zdbjq.cn/Article/details/gsjdmbkge.sHtML

[U36] Py：定时任务
来源：http://baike.fehbvm.com/Article/details/gfbtmynwl.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.zdbjq.cn/Article/details/gzubulojq.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.fehbvm.com/Article/details/gtxsbyieb.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.fehbvm.com/Article/details/gvlnuiits.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.fehbvm.com/Article/details/gajeiewwx.sHtML

Path(__file__).resolve().parent
来源：http://blog.fehbvm.com/Article/details/gdghyzuek.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.hesvh.cn/Article/details/gpqyaekda.sHtML

sys.stdout.isatty()
来源：http://read.share.zdbjq.cn/Article/details/gerqftdrk.sHtML

[U40] Py：打印到标准错误
来源：http://blog.fehbvm.com/Article/details/gcoblpydb.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.hesvh.cn/Article/details/gmgetasww.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.zdbjq.cn/Article/details/gutwkcjhk.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.zdbjq.cn/Article/details/gcthgwekd.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.fehbvm.com/Article/details/gopuxpqcj.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.fehbvm.com/Article/details/gbrclgjxx.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.fehbvm.com/Article/details/gpxulriup.sHtML

namespace App\Http;
来源：http://mobile.hesvh.cn/Article/details/ghmnxcigk.sHtML

[U44] PHP：开启严格类型
来源：http://baike.hesvh.cn/Article/details/gpvhpcqre.sHtML

declare(strict_types=1);
来源：http://www.share.hesvh.cn/Article/details/gidngdtej.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.fehbvm.com/Article/details/gvfffbolv.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/ghbvtassp.sHtML

[U46] PHP：可空类型
来源：http://blog.fehbvm.com/Article/details/gghoffrgj.sHtML

?string $name = null
来源：http://3g.fehbvm.com/Article/details/gxivwawjh.sHtML

[U47] PHP：联合类型
来源：http://mobile.hesvh.cn/Article/details/gktorenmt.sHtML

int|string $id
来源：http://www.blog.zdbjq.cn/Article/details/gcqkdqohs.sHtML

[U48] PHP：纯枚举
来源：http://baike.fehbvm.com/Article/details/gdkfohkpd.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.hesvh.cn/Article/details/gdlklrpmw.sHtML

[U49] PHP：只读属性
来源：http://m.share.hesvh.cn/Article/details/geabsfiex.sHtML

public readonly string $name
来源：http://mobile.fehbvm.com/Article/details/goinxryoe.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.hesvh.cn/Article/details/gixqwwkld.sHtML

public function __construct(private int $id) {}
来源：http://www.share.hesvh.cn/Article/details/gfdzpjvvi.sHtML

[U51] PHP：数组解构
来源：http://wap.fehbvm.com/Article/details/ghsuucxyw.sHtML

[$a, $b] = $arr;
来源：http://www.blog.hesvh.cn/Article/details/gwpxtmmfi.sHtML

[U52] PHP：箭头函数
来源：http://baike.hesvh.cn/Article/details/gvxtaaoso.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.hesvh.cn/Article/details/gvmjpljtw.sHtML

[U53] PHP：空合并运算符
来源：http://blog.fehbvm.com/Article/details/gubowuqdr.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.zdbjq.cn/Article/details/gynuidmox.sHtML

[U54] PHP：空安全调用
来源：http://m.share.fehbvm.com/Article/details/geawjqbdh.sHtML

$obj?->method()
来源：http://mobile.hesvh.cn/Article/details/gpbfwxsux.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gbkjrgvhr.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.hesvh.cn/Article/details/gmatrabnm.sHtML

[U56] PHP：命名参数
来源：http://read.share.fehbvm.com/Article/details/gwclorevz.sHtML

f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/glqfbokxg.sHtML

[U57] PHP：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gbvunscsk.sHtML

"值: {$a}"
来源：http://www.blog.zdbjq.cn/Article/details/gnwhciwic.sHtML

[U58] PHP：数组三件套
来源：http://read.share.zdbjq.cn/Article/details/grmmqgkxg.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.fehbvm.com/Article/details/gfqydhfjw.sHtML

[U59] PHP：自定义排序
来源：http://wap.hesvh.cn/Article/details/gxmdbvhav.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.hesvh.cn/Article/details/goboxsjuu.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.fehbvm.com/Article/details/ghtavklgw.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.zdbjq.cn/Article/details/gbtbiyybb.sHtML

[U61] PHP：正则
来源：http://www.share.hesvh.cn/Article/details/gifptxxen.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.fehbvm.com/Article/details/gvwbcyhvd.sHtML

[U62] PHP：日期对象
来源：http://mobile.zdbjq.cn/Article/details/ggjxlchsy.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.fehbvm.com/Article/details/gijvztbwa.sHtML

[U63] PHP：文件读写
来源：http://www.blog.zdbjq.cn/Article/details/gixishfil.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.zdbjq.cn/Article/details/gyhxibcaf.sHtML

[U64] PHP：目录遍历
来源：http://read.share.fehbvm.com/Article/details/gswmdwjsj.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.fehbvm.com/Article/details/gcaopwemf.sHtML

[U65] PHP：会话
来源：http://wap.fehbvm.com/Article/details/ghhgjaepw.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gbtmpumsp.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.zdbjq.cn/Article/details/gysqbrcnr.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.zdbjq.cn/Article/details/gjfzhicii.sHtML

[U67] PHP：处理文件上传
来源：http://wap.zdbjq.cn/Article/details/gzigwupsn.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.hesvh.cn/Article/details/gfzlkmmqm.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.hesvh.cn/Article/details/gwygtsnvy.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.hesvh.cn/Article/details/glddrfscv.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.zdbjq.cn/Article/details/gjlrbacdr.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.hesvh.cn/Article/details/gjcqadnxk.sHtML

[U70] PHP：PDO 事务
来源：http://blog.fehbvm.com/Article/details/gaotcdwkr.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.zdbjq.cn/Article/details/gzylzllll.sHtML

[U71] PHP：抛出异常
来源：http://wap.fehbvm.com/Article/details/ghviarzks.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.hesvh.cn/Article/details/ghwyijueu.sHtML

[U72] PHP：写错误日志
来源：http://wap.zdbjq.cn/Article/details/grswuahgx.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.hesvh.cn/Article/details/gcqacvyfs.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.hesvh.cn/Article/details/gzymytoqk.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.zdbjq.cn/Article/details/ggdsohmvu.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.fehbvm.com/Article/details/glcrfxnjx.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.fehbvm.com/Article/details/ghzzohvyz.sHtML

[U75] PHP：依赖注入
来源：http://wap.fehbvm.com/Article/details/gqtrwuker.sHtML

composer require psr/container
来源：http://read.share.zdbjq.cn/Article/details/gavvaijkv.sHtML

[U76] PHP：简单路由
来源：http://www.share.fehbvm.com/Article/details/gsijhrnxk.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.fehbvm.com/Article/details/gzddvkxxr.sHtML

[U77] PHP：模板渲染
来源：http://m.share.fehbvm.com/Article/details/ghxhvdnvs.sHtML

composer require twig/twig
来源：http://www.m.share.hesvh.cn/Article/details/ggydvrkvz.sHtML

[U78] PHP：单元测试
来源：http://m.share.fehbvm.com/Article/details/gfrxxetrt.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.zdbjq.cn/Article/details/gulmbiqwa.sHtML

[U79] PHP：静态分析
来源：http://www.share.hesvh.cn/Article/details/gltqwwvzq.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.hesvh.cn/Article/details/gjxatyazp.sHtML

[U80] PHP：代码规范修复
来源：http://baike.zdbjq.cn/Article/details/gsfqghxyn.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.zdbjq.cn/Article/details/gwkjqkubk.sHtML

[U81] JS：初始化项目
来源：http://wap.fehbvm.com/Article/details/getukmgix.sHtML

npm init -y;  npm i express
来源：http://3g.hesvh.cn/Article/details/gvuznfvjc.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.zdbjq.cn/Article/details/gipcqysws.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.zdbjq.cn/Article/details/ggaszijhe.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.zdbjq.cn/Article/details/gosujbpjb.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.zdbjq.cn/Article/details/guyerhjcy.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.zdbjq.cn/Article/details/gzvyipqiy.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.zdbjq.cn/Article/details/gagvhsdpx.sHtML

[U85] JS：可选链
来源：http://mobile.fehbvm.com/Article/details/giiunirnx.sHtML

a?.b?.c
来源：http://baike.hesvh.cn/Article/details/gjxvggxqd.sHtML

[U86] JS：空值合并
来源：http://www.m.share.hesvh.cn/Article/details/ggesiskvg.sHtML

a ?? b
来源：http://3g.hesvh.cn/Article/details/gwpbjwkei.sHtML

[U87] JS：解构默认值
来源：http://blog.hesvh.cn/Article/details/gagwovztc.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.hesvh.cn/Article/details/gbqtieooh.sHtML

[U88] JS：对象展开合并
来源：http://www.share.fehbvm.com/Article/details/gakwldrwq.sHtML

{ ...a, ...b }
来源：http://www.m.share.zdbjq.cn/Article/details/gddtvwhew.sHtML

[U89] JS：数组去重
来源：http://wap.fehbvm.com/Article/details/gomtlpwdp.sHtML

[...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/gtjmxlqas.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.zdbjq.cn/Article/details/glkprvqxl.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/galpfrmbh.sHtML

[U91] JS：对象键值遍历
来源：http://blog.fehbvm.com/Article/details/gewvsabcy.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.fehbvm.com/Article/details/gmbxckhju.sHtML

[U92] JS：深拷贝
来源：http://wap.zdbjq.cn/Article/details/gwklkhuud.sHtML

structuredClone(obj)
来源：http://www.m.share.fehbvm.com/Article/details/ggvjuikva.sHtML

[U93] JS：模板字符串
来源：http://wap.fehbvm.com/Article/details/gjaajskqs.sHtML

`共 ${n} 条`
来源：http://baike.fehbvm.com/Article/details/gpconxroe.sHtML

[U94] JS：箭头函数
来源：http://m.share.zdbjq.cn/Article/details/gvjtmljft.sHtML

const double = x => x * 2;
来源：http://read.share.fehbvm.com/Article/details/gzwthxtxf.sHtML

[U95] JS：Promise 包装
来源：http://3g.fehbvm.com/Article/details/gwbsdxlxd.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.fehbvm.com/Article/details/gotxjpaxq.sHtML

[U96] JS：async/await 与异常
来源：http://blog.hesvh.cn/Article/details/gqhznxaoz.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/gvbhahctp.sHtML

[U97] JS：并发请求
来源：http://baike.fehbvm.com/Article/details/gvmzslwgn.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/gwzwqnvqg.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.fehbvm.com/Article/details/gvwbnkoci.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.fehbvm.com/Article/details/gzivinrzi.sHtML

[U99] JS：事件监听
来源：http://www.m.share.fehbvm.com/Article/details/gcblmpuct.sHtML

el.addEventListener("click", e => {})
来源：http://blog.zdbjq.cn/Article/details/gnhbstzzq.sHtML

[U100] JS：DOM 查询
来源：http://3g.fehbvm.com/Article/details/ghtmohiud.sHtML

document.querySelector(".item")
来源：http://m.share.zdbjq.cn/Article/details/gwxtdejdo.sHtML

[U101] JS：classList 操作
来源：http://3g.fehbvm.com/Article/details/gfcpbgwxh.sHtML

el.classList.toggle("active")
来源：http://baike.fehbvm.com/Article/details/gcwxytpbh.sHtML

[U102] JS：本地存储
来源：http://baike.zdbjq.cn/Article/details/gkwefpmtd.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.fehbvm.com/Article/details/gmwwjtjoq.sHtML

[U103] JS：定时器
来源：http://www.blog.hesvh.cn/Article/details/gavvagfqh.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.fehbvm.com/Article/details/gidvuphom.sHtML

[U104] JS：防抖
来源：http://wap.hesvh.cn/Article/details/govotrjpe.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/gnaubcpuu.sHtML

[U105] JS：节流
来源：http://baike.fehbvm.com/Article/details/ghrumooah.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.hesvh.cn/Article/details/grneyxxak.sHtML

[U106] JS：日期格式化
来源：http://3g.fehbvm.com/Article/details/gxdcydxrd.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.hesvh.cn/Article/details/ggyuusmgz.sHtML

[U107] JS：数字千分位
来源：http://blog.zdbjq.cn/Article/details/gtegvdegt.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.zdbjq.cn/Article/details/gurhcenlk.sHtML

[U108] JS：随机整数
来源：http://3g.hesvh.cn/Article/details/gddeuodsr.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.hesvh.cn/Article/details/gooaerzyx.sHtML

[U109] JS：数组分组
来源：http://read.share.fehbvm.com/Article/details/gzesjargy.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.fehbvm.com/Article/details/gvfyknyfn.sHtML

[U110] JS：数组分块
来源：http://m.share.hesvh.cn/Article/details/gdhnkwpbo.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.fehbvm.com/Article/details/goxezfbzz.sHtML

[U111] JS：对象转 Map
来源：http://blog.fehbvm.com/Article/details/gudvgwypc.sHtML

new Map(Object.entries(obj))
来源：http://baike.hesvh.cn/Article/details/gzyfwfowr.sHtML

[U112] JS：字符串补位
来源：http://m.share.zdbjq.cn/Article/details/gdncdiomd.sHtML

"7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/gpjxbkwox.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.zdbjq.cn/Article/details/gthowmvcg.sHtML

s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gcagcusxf.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.zdbjq.cn/Article/details/gluosldhl.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.hesvh.cn/Article/details/gopyydvse.sHtML

[U115] JS：生成 UUID
来源：http://wap.fehbvm.com/Article/details/gkvykltga.sHtML

crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gjwqplizu.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.hesvh.cn/Article/details/gmumtbynq.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.hesvh.cn/Article/details/gxmzuslzk.sHtML

[U117] JS：单元测试
来源：http://m.share.hesvh.cn/Article/details/gemwyqhmi.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.zdbjq.cn/Article/details/grptydqwt.sHtML

[U118] JS：开发服务器
来源：http://mobile.zdbjq.cn/Article/details/gjfywpagl.sHtML

npm i -D vite;  npx vite
来源：http://blog.fehbvm.com/Article/details/gtcvolrgg.sHtML

[U119] JS：生产构建
来源：http://www.blog.hesvh.cn/Article/details/gswdusqld.sHtML

npx vite build
来源：http://www.blog.hesvh.cn/Article/details/ggbnsnvmm.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.hesvh.cn/Article/details/gtdeqeahr.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.fehbvm.com/Article/details/gsgbildge.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gwvuqtsmv.sHtML

统计汇总
来源：http://3g.zdbjq.cn/Article/details/gfdmicqdc.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gmzkzxqnr.sHtML

按语言统计（条）：
来源：http://3g.zdbjq.cn/Article/details/gdmisvzex.sHtML

Python ......... 252
来源：http://baike.fehbvm.com/Article/details/gfdfoyzgy.sHtML

PHP ............ 252
来源：http://m.share.zdbjq.cn/Article/details/gusatjqim.sHtML

JavaScript ..... 252
来源：http://mobile.fehbvm.com/Article/details/gbdscyzwh.sHtML

TypeScript ..... 212
来源：http://read.share.fehbvm.com/Article/details/gcrpakbax.sHtML

Java ........... 212
来源：http://wap.zdbjq.cn/Article/details/gzrhqgiui.sHtML

Go ............. 212
来源：http://wap.hesvh.cn/Article/details/gpfsqttnm.sHtML

Ruby ........... 212
来源：http://3g.fehbvm.com/Article/details/gqlyewswh.sHtML

C# ............. 212
来源：http://wap.fehbvm.com/Article/details/gzitlibth.sHtML

C .............. 30
来源：http://baike.zdbjq.cn/Article/details/gucstvnmu.sHtML

C++ ............ 30
来源：http://wap.zdbjq.cn/Article/details/gsxmrqiym.sHtML

SQL ............ 90
来源：http://www.share.hesvh.cn/Article/details/ggflzartr.sHtML

Bash ........... 80
来源：http://mobile.zdbjq.cn/Article/details/gwnccltwb.sHtML

Kotlin ......... 15
来源：http://3g.fehbvm.com/Article/details/gdkpbsenk.sHtML

Swift .......... 15
来源：http://3g.hesvh.cn/Article/details/gtuqbdgbn.sHtML

Lua ............ 10
来源：http://www.share.hesvh.cn/Article/details/ghafipgbs.sHtML

Perl ........... 10
来源：http://wap.fehbvm.com/Article/details/giazexnoz.sHtML

Scala .......... 10
来源：http://wap.fehbvm.com/Article/details/gybgowakc.sHtML

------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/glnzrnxks.sHtML

合计 ........... 2106 条
来源：http://wap.hesvh.cn/Article/details/gvesohnby.sHtML

按章节统计：
来源：http://3g.fehbvm.com/Article/details/geyggtmcv.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.hesvh.cn/Article/details/gtaokvlbn.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/gmmcdncpp.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.hesvh.cn/Article/details/glxznizfb.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.fehbvm.com/Article/details/gsbmsccpk.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.fehbvm.com/Article/details/gjqmthwzc.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.fehbvm.com/Article/details/gqbxtflte.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.fehbvm.com/Article/details/gqwlukwca.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.zdbjq.cn/Article/details/gbwqoqzmi.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gqzxbziad.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.hesvh.cn/Article/details/gtjsjpmgf.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gbsmtqthh.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/glrkmrcej.sHtML


<!-- 参考信息 -->