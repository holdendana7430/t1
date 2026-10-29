代发 wailian999

while (my $line = <$fh>) { print $line; }
来源：http://3g.fehbvm.com/Article/details/gfjveqavw.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/giokofzoe.sHtML

println("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gjawyvgzr.sHtML

[T52] Scala：变量
来源：http://baike.hesvh.cn/Article/details/gucgbaghv.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gnvatfkgo.sHtML

[T53] Scala：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gtnwegegy.sHtML

s"值: $b"
来源：http://www.m.share.hesvh.cn/Article/details/gqbhrgwgc.sHtML

[T54] Scala：集合映射
来源：http://baike.hesvh.cn/Article/details/gypogjawd.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.hesvh.cn/Article/details/gktkjdrom.sHtML

[T55] Scala：集合过滤
来源：http://wap.fehbvm.com/Article/details/gakcwekos.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.zdbjq.cn/Article/details/gymezkqis.sHtML

[T56] Scala：样例类
来源：http://m.share.hesvh.cn/Article/details/ghtbydpnp.sHtML

case class User(name: String, age: Int)
来源：http://wap.hesvh.cn/Article/details/gxqahphoj.sHtML

[T57] Scala：模式匹配
来源：http://www.share.hesvh.cn/Article/details/gqvjyrkxl.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fehbvm.com/Article/details/gvqqtygue.sHtML

[T58] Scala：函数定义
来源：http://blog.fehbvm.com/Article/details/gowsqjttg.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.zdbjq.cn/Article/details/gsipbmjzm.sHtML

[T59] Scala：循环
来源：http://m.share.zdbjq.cn/Article/details/gyqbavflh.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.zdbjq.cn/Article/details/ghiavafae.sHtML

[T60] Scala：折叠
来源：http://mobile.fehbvm.com/Article/details/gncfrtqdo.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.fehbvm.com/Article/details/gwfozasjz.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gvwejqdyq.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.hesvh.cn/Article/details/gzsntxvwj.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ghbeorrep.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.zdbjq.cn/Article/details/gvynhdppn.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.fehbvm.com/Article/details/gfasjrhvj.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.zdbjq.cn/Article/details/gjkjzxtlj.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.zdbjq.cn/Article/details/gpswughbg.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.hesvh.cn/Article/details/gqpxadanc.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.fehbvm.com/Article/details/gjozbggyb.sHtML

[U04] Py：变量调试打印
来源：http://mobile.hesvh.cn/Article/details/ggxlifbko.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.hesvh.cn/Article/details/ggyxxdshm.sHtML

[U05] Py：列表去重且保序
来源：http://wap.hesvh.cn/Article/details/gaagjoomj.sHtML

list(dict.fromkeys(arr))
来源：http://blog.zdbjq.cn/Article/details/gqedlwzmd.sHtML

[U06] Py：合并两个字典
来源：http://wap.fehbvm.com/Article/details/gnqcdmqxa.sHtML

{**a, **b}
来源：http://wap.hesvh.cn/Article/details/gbskisfnc.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.hesvh.cn/Article/details/gaxowgxfq.sHtML

{v: k for k, v in d.items()}
来源：http://blog.hesvh.cn/Article/details/gkucwgfab.sHtML

[U08] Py：展平二维列表
来源：http://baike.fehbvm.com/Article/details/gsjdpjboj.sHtML

[y for x in nested for y in x]
来源：http://blog.fehbvm.com/Article/details/gmczoolid.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.fehbvm.com/Article/details/gexpdiwgf.sHtML

max(d, key=d.get)
来源：http://www.blog.hesvh.cn/Article/details/gzwjmtvve.sHtML

[U10] Py：按值排序字典
来源：http://blog.fehbvm.com/Article/details/gidvegtzh.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.hesvh.cn/Article/details/gtqvimdhc.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.zdbjq.cn/Article/details/grxbzvyfa.sHtML

(x * 2 for x in arr)
来源：http://www.share.hesvh.cn/Article/details/ggowphjpl.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.fehbvm.com/Article/details/geumwbqaq.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.hesvh.cn/Article/details/gdmfnsogu.sHtML

[U13] Py：固定长度队列
来源：http://3g.zdbjq.cn/Article/details/glgdrjkxy.sHtML

deque(maxlen=10)
来源：http://www.share.hesvh.cn/Article/details/ghxfooalf.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.fehbvm.com/Article/details/gcomtegmk.sHtML

defaultdict(list)
来源：http://m.share.hesvh.cn/Article/details/gdllzqzzz.sHtML

[U15] Py：高精度计时
来源：http://wap.hesvh.cn/Article/details/gaowaffyw.sHtML

t = time.perf_counter()
来源：http://m.share.zdbjq.cn/Article/details/gexdmtxna.sHtML

[U16] Py：命令行参数解析
来源：http://3g.fehbvm.com/Article/details/gqmfjvsex.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.fehbvm.com/Article/details/gfmnqkkiw.sHtML

[U17] Py：初始化日志
来源：http://www.share.zdbjq.cn/Article/details/gqchlfvcj.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.fehbvm.com/Article/details/gpkywiaof.sHtML

[U18] Py：预编译正则
来源：http://3g.hesvh.cn/Article/details/gxradvwpe.sHtML

pat = re.compile(r"\d+")
来源：http://baike.hesvh.cn/Article/details/gpfxrduow.sHtML

[U19] Py：正则替换带回调
来源：http://baike.hesvh.cn/Article/details/gmcjrycrq.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.zdbjq.cn/Article/details/gnrjmomji.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.hesvh.cn/Article/details/gdajofsww.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.fehbvm.com/Article/details/gugxonddp.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.fehbvm.com/Article/details/gihcvmzoz.sHtML

@contextlib.contextmanager
来源：http://baike.hesvh.cn/Article/details/gtdvvhuro.sHtML

[U22] Py：矩阵转置
来源：http://read.share.fehbvm.com/Article/details/gknmbrxxn.sHtML

list(zip(*m))
来源：http://www.blog.hesvh.cn/Article/details/gcutegpuv.sHtML

[U23] Py：分块读取大文件
来源：http://baike.fehbvm.com/Article/details/gujjnfzws.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.fehbvm.com/Article/details/gjlkxcerc.sHtML

[U24] Py：路径操作
来源：http://baike.fehbvm.com/Article/details/giraeprht.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.zdbjq.cn/Article/details/gakzfdyvd.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.fehbvm.com/Article/details/gnvvxvqfv.sHtML

csv.DictReader(f)
来源：http://mobile.hesvh.cn/Article/details/gqqookbjo.sHtML

[U26] Py：并发下载
来源：http://baike.fehbvm.com/Article/details/grbfdqkow.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.fehbvm.com/Article/details/grcjrkxth.sHtML

[U27] Py：异步 HTTP
来源：http://blog.fehbvm.com/Article/details/gnwakzcxx.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.fehbvm.com/Article/details/ggiecxlmf.sHtML

[U28] Py：类型别名
来源：http://mobile.fehbvm.com/Article/details/gpidjbgwg.sHtML

UserId = int
来源：http://wap.hesvh.cn/Article/details/gfjfqmkpl.sHtML

[U29] Py：属性校验
来源：http://3g.fehbvm.com/Article/details/gfzwukzuo.sHtML

@property 与 @x.setter 配合
来源：http://mobile.zdbjq.cn/Article/details/glrstoaax.sHtML

[U30] Py：数据类
来源：http://baike.hesvh.cn/Article/details/gjvvbejmf.sHtML

@dataclass(slots=True)
来源：http://wap.fehbvm.com/Article/details/ggbmlsxol.sHtML

[U31] Py：单测
来源：http://3g.zdbjq.cn/Article/details/gughrqwfx.sHtML

python -m pytest -q
来源：http://m.share.zdbjq.cn/Article/details/gsqrexnwk.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.fehbvm.com/Article/details/goccdgoop.sHtML

ruff format . && ruff check --fix .
来源：http://blog.fehbvm.com/Article/details/gmgmzuclj.sHtML

[U33] Py：打包发布
来源：http://m.share.hesvh.cn/Article/details/gcrxcgdnc.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.zdbjq.cn/Article/details/gfmwuyhoo.sHtML

[U34] Py：判断编码
来源：http://m.share.fehbvm.com/Article/details/ghevojvcb.sHtML

chardet.detect(raw)
来源：http://mobile.zdbjq.cn/Article/details/goqzcfgdc.sHtML

[U35] Py：发送邮件
来源：http://baike.hesvh.cn/Article/details/gozqmxbjl.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.fehbvm.com/Article/details/guszhtoeq.sHtML

[U36] Py：定时任务
来源：http://www.share.hesvh.cn/Article/details/gdjbupprr.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.zdbjq.cn/Article/details/gnjidpmmu.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.hesvh.cn/Article/details/gcqfeogwr.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.hesvh.cn/Article/details/gtneanmot.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.zdbjq.cn/Article/details/ggjazaslb.sHtML

Path(__file__).resolve().parent
来源：http://wap.hesvh.cn/Article/details/gpaiclzgm.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.hesvh.cn/Article/details/gqpglwsbj.sHtML

sys.stdout.isatty()
来源：http://www.m.share.zdbjq.cn/Article/details/gdpaegshp.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.hesvh.cn/Article/details/geqqxelnl.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.zdbjq.cn/Article/details/gehoevpqz.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.fehbvm.com/Article/details/gntgwqyji.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.hesvh.cn/Article/details/gvutxwsez.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.fehbvm.com/Article/details/gawnlxiej.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.zdbjq.cn/Article/details/gnelqfboh.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.zdbjq.cn/Article/details/gkvvuvivl.sHtML

namespace App\Http;
来源：http://read.share.hesvh.cn/Article/details/gwcgteyft.sHtML

[U44] PHP：开启严格类型
来源：http://blog.fehbvm.com/Article/details/gejdxntku.sHtML

declare(strict_types=1);
来源：http://wap.zdbjq.cn/Article/details/gksywvwgw.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.fehbvm.com/Article/details/godgodopt.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gsjvjpbyo.sHtML

[U46] PHP：可空类型
来源：http://wap.zdbjq.cn/Article/details/gtwchtoem.sHtML

?string $name = null
来源：http://www.blog.zdbjq.cn/Article/details/gcqvhxqyd.sHtML

[U47] PHP：联合类型
来源：http://www.share.hesvh.cn/Article/details/gynginovw.sHtML

int|string $id
来源：http://read.share.fehbvm.com/Article/details/gcmipcjsd.sHtML

[U48] PHP：纯枚举
来源：http://mobile.zdbjq.cn/Article/details/gdigfrlzx.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.zdbjq.cn/Article/details/gllwzalqq.sHtML

[U49] PHP：只读属性
来源：http://wap.hesvh.cn/Article/details/gjcfmyras.sHtML

public readonly string $name
来源：http://m.share.fehbvm.com/Article/details/gbiblrfov.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.zdbjq.cn/Article/details/gdjccxiuw.sHtML

public function __construct(private int $id) {}
来源：http://wap.fehbvm.com/Article/details/gdpyptffb.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.hesvh.cn/Article/details/glhpyyyhq.sHtML

[$a, $b] = $arr;
来源：http://mobile.fehbvm.com/Article/details/gzwesabic.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.fehbvm.com/Article/details/gzdayjurn.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.zdbjq.cn/Article/details/gtdwwfmtk.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.fehbvm.com/Article/details/gcsbeuhgk.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.fehbvm.com/Article/details/gbkhdmlfi.sHtML

[U54] PHP：空安全调用
来源：http://wap.hesvh.cn/Article/details/gkrblkvkq.sHtML

$obj?->method()
来源：http://www.m.share.hesvh.cn/Article/details/gppsskhqc.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.hesvh.cn/Article/details/gvrhurhax.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.zdbjq.cn/Article/details/gbusejphd.sHtML

[U56] PHP：命名参数
来源：http://blog.fehbvm.com/Article/details/geulwumah.sHtML

f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/gccvgytut.sHtML

[U57] PHP：字符串插值
来源：http://www.share.fehbvm.com/Article/details/ghhqvuooi.sHtML

"值: {$a}"
来源：http://3g.fehbvm.com/Article/details/gpagndmoc.sHtML

[U58] PHP：数组三件套
来源：http://www.share.fehbvm.com/Article/details/glnxcybbt.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gvgjhzhta.sHtML

[U59] PHP：自定义排序
来源：http://m.share.fehbvm.com/Article/details/gwiqwzqaz.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fehbvm.com/Article/details/gbzdpguec.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.hesvh.cn/Article/details/gwkfyzbei.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.fehbvm.com/Article/details/gfmwkpjei.sHtML

[U61] PHP：正则
来源：http://www.share.fehbvm.com/Article/details/gdmpiunfn.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.fehbvm.com/Article/details/ghiqxhryk.sHtML

[U62] PHP：日期对象
来源：http://www.blog.fehbvm.com/Article/details/gnxzlesjw.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.hesvh.cn/Article/details/ghvryckaw.sHtML

[U63] PHP：文件读写
来源：http://www.blog.hesvh.cn/Article/details/gdczsxjom.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.fehbvm.com/Article/details/gbqrkdrno.sHtML

[U64] PHP：目录遍历
来源：http://www.share.hesvh.cn/Article/details/gingjkleh.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.fehbvm.com/Article/details/gdleplcsa.sHtML

[U65] PHP：会话
来源：http://www.m.share.fehbvm.com/Article/details/gsymqohcr.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.fehbvm.com/Article/details/gkomtrhli.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.zdbjq.cn/Article/details/glsfwmeku.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.hesvh.cn/Article/details/gjsfqqhgs.sHtML

[U67] PHP：处理文件上传
来源：http://baike.fehbvm.com/Article/details/gucbvfrov.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.fehbvm.com/Article/details/gexwrpixu.sHtML

[U68] PHP：PDO 连接
来源：http://wap.fehbvm.com/Article/details/gcyslmpjo.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.fehbvm.com/Article/details/gvfkpdfmn.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.zdbjq.cn/Article/details/gchobekyh.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.fehbvm.com/Article/details/gxyizuqis.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.zdbjq.cn/Article/details/gutskffmg.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.zdbjq.cn/Article/details/gpnfuhvbb.sHtML

[U71] PHP：抛出异常
来源：http://baike.hesvh.cn/Article/details/gnyvdgwtd.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.hesvh.cn/Article/details/gutpykfma.sHtML

[U72] PHP：写错误日志
来源：http://blog.zdbjq.cn/Article/details/gyawasnof.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.fehbvm.com/Article/details/gbehnlqxn.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.hesvh.cn/Article/details/gewdekelf.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.fehbvm.com/Article/details/gasrtozdw.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gkfsflweb.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.fehbvm.com/Article/details/ggustnitk.sHtML

[U75] PHP：依赖注入
来源：http://baike.fehbvm.com/Article/details/gaioqcjhf.sHtML

composer require psr/container
来源：http://www.m.share.hesvh.cn/Article/details/grqlddtnn.sHtML

[U76] PHP：简单路由
来源：http://www.share.fehbvm.com/Article/details/gmywcqlog.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.fehbvm.com/Article/details/ggyzwkznz.sHtML

[U77] PHP：模板渲染
来源：http://3g.fehbvm.com/Article/details/gviizuahk.sHtML

composer require twig/twig
来源：http://www.blog.zdbjq.cn/Article/details/gxhfumixd.sHtML

[U78] PHP：单元测试
来源：http://mobile.fehbvm.com/Article/details/gzaiqthjd.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.fehbvm.com/Article/details/gjdhaxyza.sHtML

[U79] PHP：静态分析
来源：http://m.share.zdbjq.cn/Article/details/guvhakpcr.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.zdbjq.cn/Article/details/gzpzuhlgw.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.hesvh.cn/Article/details/gzmlnflnb.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.zdbjq.cn/Article/details/gmvnnihsj.sHtML

[U81] JS：初始化项目
来源：http://www.share.fehbvm.com/Article/details/gikfxnptv.sHtML

npm init -y;  npm i express
来源：http://wap.zdbjq.cn/Article/details/ghrwradaa.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.fehbvm.com/Article/details/gaabozzun.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.fehbvm.com/Article/details/gwfgpwwxw.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.fehbvm.com/Article/details/gpibybrud.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.fehbvm.com/Article/details/gapyvykex.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.zdbjq.cn/Article/details/goaeavdvd.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.zdbjq.cn/Article/details/gnyhouarh.sHtML

[U85] JS：可选链
来源：http://baike.zdbjq.cn/Article/details/gbubxijby.sHtML

a?.b?.c
来源：http://mobile.zdbjq.cn/Article/details/gmdzxmmhl.sHtML

[U86] JS：空值合并
来源：http://3g.fehbvm.com/Article/details/guxcgmtdg.sHtML

a ?? b
来源：http://read.share.fehbvm.com/Article/details/gctyoysly.sHtML

[U87] JS：解构默认值
来源：http://3g.fehbvm.com/Article/details/gpihbfrlc.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.hesvh.cn/Article/details/gordoiwji.sHtML

[U88] JS：对象展开合并
来源：http://3g.zdbjq.cn/Article/details/glytsyrwe.sHtML

{ ...a, ...b }
来源：http://www.blog.zdbjq.cn/Article/details/guvetsaoq.sHtML

[U89] JS：数组去重
来源：http://m.share.hesvh.cn/Article/details/ggsjgwanv.sHtML

[...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/gpjkurkgd.sHtML

[U90] JS：数字数组排序
来源：http://3g.zdbjq.cn/Article/details/gxgydxhcx.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gfvorscgv.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.zdbjq.cn/Article/details/gkqgaborc.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.fehbvm.com/Article/details/gmyzrntal.sHtML

[U92] JS：深拷贝
来源：http://m.share.zdbjq.cn/Article/details/gtltdquzu.sHtML

structuredClone(obj)
来源：http://wap.zdbjq.cn/Article/details/gwoinodvy.sHtML

[U93] JS：模板字符串
来源：http://3g.zdbjq.cn/Article/details/gqooxgvpl.sHtML

`共 ${n} 条`
来源：http://3g.zdbjq.cn/Article/details/gjigpjkqm.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.zdbjq.cn/Article/details/geamirefw.sHtML

const double = x => x * 2;
来源：http://wap.zdbjq.cn/Article/details/gnnvsnnul.sHtML

[U95] JS：Promise 包装
来源：http://www.share.zdbjq.cn/Article/details/gfdyntixf.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.zdbjq.cn/Article/details/gboxrbqbm.sHtML

[U96] JS：async/await 与异常
来源：http://baike.hesvh.cn/Article/details/gcsqnthoi.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/gnhlfilho.sHtML

[U97] JS：并发请求
来源：http://wap.fehbvm.com/Article/details/gyehehpjl.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/gfrapjxgz.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.hesvh.cn/Article/details/gwwppsvrt.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.fehbvm.com/Article/details/gqnstoypb.sHtML

[U99] JS：事件监听
来源：http://m.share.fehbvm.com/Article/details/genzlbkxv.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.zdbjq.cn/Article/details/grwzmmhax.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.fehbvm.com/Article/details/gvubtkvye.sHtML

document.querySelector(".item")
来源：http://www.share.hesvh.cn/Article/details/gilemcgkl.sHtML

[U101] JS：classList 操作
来源：http://baike.zdbjq.cn/Article/details/gyxixzpuc.sHtML

el.classList.toggle("active")
来源：http://3g.fehbvm.com/Article/details/gnfgsgazb.sHtML

[U102] JS：本地存储
来源：http://blog.zdbjq.cn/Article/details/gukvoppig.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.zdbjq.cn/Article/details/gwwpclktg.sHtML

[U103] JS：定时器
来源：http://3g.fehbvm.com/Article/details/giiabpxom.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.hesvh.cn/Article/details/gafzxqtlz.sHtML

[U104] JS：防抖
来源：http://wap.zdbjq.cn/Article/details/ghzdaszck.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/gyhhpsyop.sHtML

[U105] JS：节流
来源：http://wap.fehbvm.com/Article/details/gowoxlbvn.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.hesvh.cn/Article/details/gxlohlnnl.sHtML

[U106] JS：日期格式化
来源：http://blog.zdbjq.cn/Article/details/garruyueb.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.fehbvm.com/Article/details/gxaupewlp.sHtML

[U107] JS：数字千分位
来源：http://www.share.hesvh.cn/Article/details/gfuxbfnba.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.fehbvm.com/Article/details/gnfkrgatg.sHtML

[U108] JS：随机整数
来源：http://read.share.zdbjq.cn/Article/details/gbxrfizmm.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.zdbjq.cn/Article/details/gvfsjodzi.sHtML

[U109] JS：数组分组
来源：http://blog.fehbvm.com/Article/details/gqsbzczdk.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.zdbjq.cn/Article/details/getmpwesf.sHtML

[U110] JS：数组分块
来源：http://wap.fehbvm.com/Article/details/gxpzbeaha.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.hesvh.cn/Article/details/gytnqqzfw.sHtML

[U111] JS：对象转 Map
来源：http://3g.hesvh.cn/Article/details/gqdbdpzzt.sHtML

new Map(Object.entries(obj))
来源：http://www.share.hesvh.cn/Article/details/gwqrxknob.sHtML

[U112] JS：字符串补位
来源：http://mobile.fehbvm.com/Article/details/gjeaqeukd.sHtML

"7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/guqcwnyzd.sHtML

[U113] JS：正则替换全部
来源：http://blog.fehbvm.com/Article/details/gwtoqhujn.sHtML

s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gkcfbidnh.sHtML

[U114] JS：JSON 深比较
来源：http://blog.hesvh.cn/Article/details/ggtcblkfz.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.zdbjq.cn/Article/details/gqlqaxxje.sHtML

[U115] JS：生成 UUID
来源：http://wap.hesvh.cn/Article/details/gvcsgztlp.sHtML

crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/gtrffxeec.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.zdbjq.cn/Article/details/gyfixgfpu.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.fehbvm.com/Article/details/gufjsxvwl.sHtML

[U117] JS：单元测试
来源：http://www.share.hesvh.cn/Article/details/galrxvdby.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.zdbjq.cn/Article/details/ghvyhuckp.sHtML

[U118] JS：开发服务器
来源：http://m.share.hesvh.cn/Article/details/gkptqcbtd.sHtML

npm i -D vite;  npx vite
来源：http://3g.fehbvm.com/Article/details/gclpuohjb.sHtML

[U119] JS：生产构建
来源：http://3g.hesvh.cn/Article/details/ggousdjev.sHtML

npx vite build
来源：http://3g.fehbvm.com/Article/details/guxndrhoj.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.zdbjq.cn/Article/details/gvdahdhsj.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.hesvh.cn/Article/details/gcpzifkdf.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gizelljfv.sHtML

统计汇总
来源：http://wap.zdbjq.cn/Article/details/gelsatnfb.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/geswfsqlg.sHtML

按语言统计（条）：
来源：http://www.blog.zdbjq.cn/Article/details/gwdjphuvs.sHtML

Python ......... 252
来源：http://mobile.hesvh.cn/Article/details/gdsukxlyg.sHtML

PHP ............ 252
来源：http://mobile.zdbjq.cn/Article/details/gbfuagqtu.sHtML

JavaScript ..... 252
来源：http://www.share.fehbvm.com/Article/details/gtgphpfye.sHtML

TypeScript ..... 212
来源：http://baike.zdbjq.cn/Article/details/ghzomuaup.sHtML

Java ........... 212
来源：http://wap.hesvh.cn/Article/details/gfetsivpc.sHtML

Go ............. 212
来源：http://www.blog.fehbvm.com/Article/details/ggltigelx.sHtML

Ruby ........... 212
来源：http://www.m.share.zdbjq.cn/Article/details/gmmtixriv.sHtML

C# ............. 212
来源：http://www.share.hesvh.cn/Article/details/gjwvpvgrw.sHtML

C .............. 30
来源：http://3g.hesvh.cn/Article/details/gngsccutw.sHtML

C++ ............ 30
来源：http://baike.fehbvm.com/Article/details/gemlurmat.sHtML

SQL ............ 90
来源：http://wap.fehbvm.com/Article/details/geqraqhnu.sHtML

Bash ........... 80
来源：http://baike.fehbvm.com/Article/details/gcnvioxhp.sHtML

Kotlin ......... 15
来源：http://blog.zdbjq.cn/Article/details/ghbdhhlbd.sHtML

Swift .......... 15
来源：http://read.share.zdbjq.cn/Article/details/gtnthquvs.sHtML

Lua ............ 10
来源：http://www.share.zdbjq.cn/Article/details/gszfomptb.sHtML

Perl ........... 10
来源：http://3g.hesvh.cn/Article/details/ghwunotei.sHtML

Scala .......... 10
来源：http://www.m.share.hesvh.cn/Article/details/gpvkxjwyp.sHtML

------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gtvgjkkxi.sHtML

合计 ........... 2106 条
来源：http://www.m.share.zdbjq.cn/Article/details/gwhphzewf.sHtML

按章节统计：
来源：http://m.share.fehbvm.com/Article/details/gzuzfioxo.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.hesvh.cn/Article/details/gzozebzng.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/gccjoyfhm.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.fehbvm.com/Article/details/gjhquswtg.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.hesvh.cn/Article/details/grxwfgtcf.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.fehbvm.com/Article/details/gyhrlufkl.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.zdbjq.cn/Article/details/ganfqzomm.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.hesvh.cn/Article/details/gnegqjwda.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.hesvh.cn/Article/details/gakwsfrgc.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gjcdfamvb.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.zdbjq.cn/Article/details/gvtemxjzq.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gzwydsbed.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gbdcyxtmr.sHtML


<!-- 参考信息 -->