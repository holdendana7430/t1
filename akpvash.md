代发 wailian999

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.hesvh.cn/Article/details/gtaribzhu.sHtML

[T51] Scala：Hello World
来源：http://www.share.fehbvm.com/Article/details/gecacpqjk.sHtML

println("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gtxcuoziz.sHtML

[T52] Scala：变量
来源：http://baike.hesvh.cn/Article/details/gdkemcakv.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gschfyype.sHtML

[T53] Scala：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gvowymbdj.sHtML

s"值: $b"
来源：http://www.blog.fehbvm.com/Article/details/gfwjybmdq.sHtML

[T54] Scala：集合映射
来源：http://mobile.hesvh.cn/Article/details/ggccqinkv.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.zdbjq.cn/Article/details/gooilyqod.sHtML

[T55] Scala：集合过滤
来源：http://www.share.hesvh.cn/Article/details/gvgzviwur.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.hesvh.cn/Article/details/gthfolwox.sHtML

[T56] Scala：样例类
来源：http://wap.zdbjq.cn/Article/details/gapsbujbi.sHtML

case class User(name: String, age: Int)
来源：http://wap.zdbjq.cn/Article/details/ggjzevrvi.sHtML

[T57] Scala：模式匹配
来源：http://baike.hesvh.cn/Article/details/giegcunur.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.hesvh.cn/Article/details/gwhbiqkwg.sHtML

[T58] Scala：函数定义
来源：http://read.share.zdbjq.cn/Article/details/gaoweswkn.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.fehbvm.com/Article/details/gcembyuho.sHtML

[T59] Scala：循环
来源：http://baike.zdbjq.cn/Article/details/gljpvpvfg.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.hesvh.cn/Article/details/gutgmanan.sHtML

[T60] Scala：折叠
来源：http://www.blog.hesvh.cn/Article/details/gqziknuif.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.zdbjq.cn/Article/details/ghxrlwntp.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gdxrkxtjm.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.hesvh.cn/Article/details/gyblieqcb.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gczejwjem.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.fehbvm.com/Article/details/gkjrxpwod.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.fehbvm.com/Article/details/goerdfiaw.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.fehbvm.com/Article/details/gdhdqpune.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.fehbvm.com/Article/details/gsazomytm.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.fehbvm.com/Article/details/gxewlwplk.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.zdbjq.cn/Article/details/geqicussq.sHtML

[U04] Py：变量调试打印
来源：http://read.share.hesvh.cn/Article/details/gxqobibgy.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.zdbjq.cn/Article/details/gbfevhrco.sHtML

[U05] Py：列表去重且保序
来源：http://baike.hesvh.cn/Article/details/golhiefgx.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.zdbjq.cn/Article/details/gwmicnhpp.sHtML

[U06] Py：合并两个字典
来源：http://m.share.fehbvm.com/Article/details/ghddfldyn.sHtML

{**a, **b}
来源：http://www.share.fehbvm.com/Article/details/gbfjupboj.sHtML

[U07] Py：反转字典键值
来源：http://blog.zdbjq.cn/Article/details/gusjfbgau.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.fehbvm.com/Article/details/gjysqyxva.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.fehbvm.com/Article/details/gzydfdnsc.sHtML

[y for x in nested for y in x]
来源：http://www.blog.hesvh.cn/Article/details/gpqaybkei.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.zdbjq.cn/Article/details/gronpgvmd.sHtML

max(d, key=d.get)
来源：http://www.share.zdbjq.cn/Article/details/gqquzbvdz.sHtML

[U10] Py：按值排序字典
来源：http://blog.hesvh.cn/Article/details/gkalkqaiz.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.hesvh.cn/Article/details/ghxoaftii.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.hesvh.cn/Article/details/gpsdqwzeh.sHtML

(x * 2 for x in arr)
来源：http://baike.hesvh.cn/Article/details/gaemlhply.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.hesvh.cn/Article/details/gnuysrttn.sHtML

Counter(arr).most_common(3)
来源：http://blog.hesvh.cn/Article/details/gthjzejjb.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.zdbjq.cn/Article/details/gayinqhnv.sHtML

deque(maxlen=10)
来源：http://www.m.share.fehbvm.com/Article/details/gipfdsgku.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.fehbvm.com/Article/details/ghrxcsxvo.sHtML

defaultdict(list)
来源：http://read.share.hesvh.cn/Article/details/gdnlacnkb.sHtML

[U15] Py：高精度计时
来源：http://www.blog.fehbvm.com/Article/details/ggtronpag.sHtML

t = time.perf_counter()
来源：http://www.share.hesvh.cn/Article/details/ghldlsibw.sHtML

[U16] Py：命令行参数解析
来源：http://3g.fehbvm.com/Article/details/goarqbmjt.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.zdbjq.cn/Article/details/gqqoyvzqg.sHtML

[U17] Py：初始化日志
来源：http://www.blog.zdbjq.cn/Article/details/gyuvnanjj.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.fehbvm.com/Article/details/galnnqutl.sHtML

[U18] Py：预编译正则
来源：http://www.blog.fehbvm.com/Article/details/gfygynzjp.sHtML

pat = re.compile(r"\d+")
来源：http://3g.hesvh.cn/Article/details/gjtpqrcvk.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.fehbvm.com/Article/details/gzvmyeaxt.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.hesvh.cn/Article/details/gwampsaml.sHtML

[U20] Py：缓存函数结果
来源：http://3g.zdbjq.cn/Article/details/ggltragsb.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.hesvh.cn/Article/details/gsegihwtx.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.hesvh.cn/Article/details/gwddhtuwj.sHtML

@contextlib.contextmanager
来源：http://wap.zdbjq.cn/Article/details/gyutavfgg.sHtML

[U22] Py：矩阵转置
来源：http://www.share.zdbjq.cn/Article/details/gbteleyib.sHtML

list(zip(*m))
来源：http://baike.zdbjq.cn/Article/details/gncfonuay.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.fehbvm.com/Article/details/gnjgftskh.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.hesvh.cn/Article/details/gniwuzsxn.sHtML

[U24] Py：路径操作
来源：http://baike.zdbjq.cn/Article/details/guebczmwt.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/giahcncri.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.zdbjq.cn/Article/details/gfmsqhmck.sHtML

csv.DictReader(f)
来源：http://www.m.share.hesvh.cn/Article/details/glhywhcns.sHtML

[U26] Py：并发下载
来源：http://wap.zdbjq.cn/Article/details/gkoollnkz.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.fehbvm.com/Article/details/gqorlyxet.sHtML

[U27] Py：异步 HTTP
来源：http://wap.fehbvm.com/Article/details/gdlmqgfcs.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.zdbjq.cn/Article/details/gxbibdxju.sHtML

[U28] Py：类型别名
来源：http://www.m.share.fehbvm.com/Article/details/gwnbhbpom.sHtML

UserId = int
来源：http://www.share.hesvh.cn/Article/details/gkcgsgyib.sHtML

[U29] Py：属性校验
来源：http://www.share.hesvh.cn/Article/details/gbmoydssh.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.zdbjq.cn/Article/details/gsjiaqzmd.sHtML

[U30] Py：数据类
来源：http://read.share.hesvh.cn/Article/details/gbosflenw.sHtML

@dataclass(slots=True)
来源：http://www.blog.fehbvm.com/Article/details/gaibeezyu.sHtML

[U31] Py：单测
来源：http://wap.fehbvm.com/Article/details/ggphncspp.sHtML

python -m pytest -q
来源：http://blog.hesvh.cn/Article/details/gqhrubbjr.sHtML

[U32] Py：代码格式化
来源：http://www.blog.hesvh.cn/Article/details/gdqkoladq.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.zdbjq.cn/Article/details/gqvndvjvd.sHtML

[U33] Py：打包发布
来源：http://m.share.zdbjq.cn/Article/details/gmefwbvic.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.zdbjq.cn/Article/details/gmojikkgw.sHtML

[U34] Py：判断编码
来源：http://read.share.zdbjq.cn/Article/details/guhpswbdd.sHtML

chardet.detect(raw)
来源：http://3g.hesvh.cn/Article/details/ggevmafwd.sHtML

[U35] Py：发送邮件
来源：http://baike.zdbjq.cn/Article/details/gdyuowydh.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.hesvh.cn/Article/details/gvsqdccix.sHtML

[U36] Py：定时任务
来源：http://wap.zdbjq.cn/Article/details/glcohscik.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.fehbvm.com/Article/details/gwfjtoygr.sHtML

[U37] Py：读写 Excel
来源：http://mobile.fehbvm.com/Article/details/gzrsbyndo.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.fehbvm.com/Article/details/gpnhginjb.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.hesvh.cn/Article/details/gxnvptvso.sHtML

Path(__file__).resolve().parent
来源：http://3g.hesvh.cn/Article/details/gimjgbwvp.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.zdbjq.cn/Article/details/gaamurylk.sHtML

sys.stdout.isatty()
来源：http://3g.fehbvm.com/Article/details/gkyxkkyoo.sHtML

[U40] Py：打印到标准错误
来源：http://baike.zdbjq.cn/Article/details/gypleiqec.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.hesvh.cn/Article/details/gunqpxlqu.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.zdbjq.cn/Article/details/gkuvdiike.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.hesvh.cn/Article/details/ggryukgvm.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.fehbvm.com/Article/details/gnwuiqdzg.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.fehbvm.com/Article/details/gojmqemuf.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.fehbvm.com/Article/details/gsvmitguc.sHtML

namespace App\Http;
来源：http://www.share.zdbjq.cn/Article/details/gnwzmgbur.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.zdbjq.cn/Article/details/gnknwfvcz.sHtML

declare(strict_types=1);
来源：http://www.blog.hesvh.cn/Article/details/gfbmviatw.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.fehbvm.com/Article/details/goazqabbj.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gqoyqqtlu.sHtML

[U46] PHP：可空类型
来源：http://read.share.fehbvm.com/Article/details/gnszlbxst.sHtML

?string $name = null
来源：http://www.m.share.zdbjq.cn/Article/details/geitrjian.sHtML

[U47] PHP：联合类型
来源：http://m.share.zdbjq.cn/Article/details/gwmqlehrf.sHtML

int|string $id
来源：http://mobile.hesvh.cn/Article/details/gonrccdpx.sHtML

[U48] PHP：纯枚举
来源：http://mobile.fehbvm.com/Article/details/gsakoolsi.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.fehbvm.com/Article/details/gkudcplkr.sHtML

[U49] PHP：只读属性
来源：http://baike.fehbvm.com/Article/details/gncbvietk.sHtML

public readonly string $name
来源：http://www.share.hesvh.cn/Article/details/gvckhtqgn.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.hesvh.cn/Article/details/gvsgszqhi.sHtML

public function __construct(private int $id) {}
来源：http://blog.zdbjq.cn/Article/details/gpvcyrirb.sHtML

[U51] PHP：数组解构
来源：http://wap.zdbjq.cn/Article/details/genrxkijh.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.fehbvm.com/Article/details/gfcmurzho.sHtML

[U52] PHP：箭头函数
来源：http://mobile.hesvh.cn/Article/details/gelmegyhn.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.hesvh.cn/Article/details/gytktcllx.sHtML

[U53] PHP：空合并运算符
来源：http://blog.fehbvm.com/Article/details/gzxzuverj.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.hesvh.cn/Article/details/gbxazwnhs.sHtML

[U54] PHP：空安全调用
来源：http://mobile.hesvh.cn/Article/details/glfusokdy.sHtML

$obj?->method()
来源：http://baike.fehbvm.com/Article/details/gwukkbfer.sHtML

[U55] PHP：match 表达式
来源：http://wap.zdbjq.cn/Article/details/gncoeutzq.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.zdbjq.cn/Article/details/gvrhkhhxi.sHtML

[U56] PHP：命名参数
来源：http://mobile.hesvh.cn/Article/details/gwyvrffgx.sHtML

f(a: 1, b: 2)
来源：http://read.share.hesvh.cn/Article/details/gzbwnuwei.sHtML

[U57] PHP：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gryndvrdr.sHtML

"值: {$a}"
来源：http://www.blog.zdbjq.cn/Article/details/gdlmfjrgo.sHtML

[U58] PHP：数组三件套
来源：http://m.share.zdbjq.cn/Article/details/gcmmdvqva.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gyhhqjfzu.sHtML

[U59] PHP：自定义排序
来源：http://mobile.zdbjq.cn/Article/details/gzvciosdl.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.zdbjq.cn/Article/details/gtdmvcygi.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.zdbjq.cn/Article/details/gujoecbde.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.fehbvm.com/Article/details/gxvtgurum.sHtML

[U61] PHP：正则
来源：http://mobile.zdbjq.cn/Article/details/gctvtbgyi.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gfgcixzgo.sHtML

[U62] PHP：日期对象
来源：http://www.share.zdbjq.cn/Article/details/gpwsuwtsu.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.hesvh.cn/Article/details/gkvizrhuc.sHtML

[U63] PHP：文件读写
来源：http://blog.fehbvm.com/Article/details/gsedbxmmh.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.fehbvm.com/Article/details/glwmmsztt.sHtML

[U64] PHP：目录遍历
来源：http://baike.fehbvm.com/Article/details/gzgrlrrzp.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.fehbvm.com/Article/details/gnwnjdows.sHtML

[U65] PHP：会话
来源：http://www.m.share.hesvh.cn/Article/details/gkvjgcoop.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gkskjzrwn.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.hesvh.cn/Article/details/gmtyzhzte.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.zdbjq.cn/Article/details/gztxrruce.sHtML

[U67] PHP：处理文件上传
来源：http://blog.fehbvm.com/Article/details/gmzdglfcz.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.hesvh.cn/Article/details/gxqccdeap.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.zdbjq.cn/Article/details/gkgcpllma.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.fehbvm.com/Article/details/gjnlqzfvz.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.zdbjq.cn/Article/details/gnpxgbxsf.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.hesvh.cn/Article/details/gxtxjvkcw.sHtML

[U70] PHP：PDO 事务
来源：http://baike.fehbvm.com/Article/details/gmlosrycn.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.fehbvm.com/Article/details/gddgzdluk.sHtML

[U71] PHP：抛出异常
来源：http://baike.fehbvm.com/Article/details/gmsqhxizb.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.fehbvm.com/Article/details/gkysmevks.sHtML

[U72] PHP：写错误日志
来源：http://baike.hesvh.cn/Article/details/ghjdiljul.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.zdbjq.cn/Article/details/gjsqhpbsn.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.fehbvm.com/Article/details/gurrsyxtw.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.zdbjq.cn/Article/details/ggswecyzf.sHtML

[U74] PHP：读取环境变量
来源：http://baike.fehbvm.com/Article/details/gignyvecg.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.fehbvm.com/Article/details/gxvntgobt.sHtML

[U75] PHP：依赖注入
来源：http://blog.fehbvm.com/Article/details/gnyzhgpzs.sHtML

composer require psr/container
来源：http://baike.zdbjq.cn/Article/details/gtmkrtkdx.sHtML

[U76] PHP：简单路由
来源：http://blog.zdbjq.cn/Article/details/ghwsrlsmu.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.zdbjq.cn/Article/details/greqcijdd.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.hesvh.cn/Article/details/gjjuipgkz.sHtML

composer require twig/twig
来源：http://www.m.share.zdbjq.cn/Article/details/ggriyhaev.sHtML

[U78] PHP：单元测试
来源：http://mobile.zdbjq.cn/Article/details/gkoakvkxm.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.zdbjq.cn/Article/details/glphlowfk.sHtML

[U79] PHP：静态分析
来源：http://mobile.zdbjq.cn/Article/details/gyieepwry.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.hesvh.cn/Article/details/gmjcqwdhl.sHtML

[U80] PHP：代码规范修复
来源：http://blog.zdbjq.cn/Article/details/gpvsysgwk.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.zdbjq.cn/Article/details/gkqsuyavv.sHtML

[U81] JS：初始化项目
来源：http://baike.fehbvm.com/Article/details/gdbochzcy.sHtML

npm init -y;  npm i express
来源：http://mobile.hesvh.cn/Article/details/gphhrphdg.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.hesvh.cn/Article/details/gxvvwvrqs.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.fehbvm.com/Article/details/gyqmqsafa.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.fehbvm.com/Article/details/gumnolvvn.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.hesvh.cn/Article/details/gbfiaupib.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.hesvh.cn/Article/details/ggscnxaet.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.zdbjq.cn/Article/details/gdewbhhdf.sHtML

[U85] JS：可选链
来源：http://read.share.hesvh.cn/Article/details/gfliipdhx.sHtML

a?.b?.c
来源：http://wap.fehbvm.com/Article/details/gfnthxbuj.sHtML

[U86] JS：空值合并
来源：http://www.m.share.fehbvm.com/Article/details/gaxhorlfm.sHtML

a ?? b
来源：http://m.share.hesvh.cn/Article/details/gofcnmrxf.sHtML

[U87] JS：解构默认值
来源：http://3g.fehbvm.com/Article/details/gegsvjpjc.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.fehbvm.com/Article/details/gogzjgwbx.sHtML

[U88] JS：对象展开合并
来源：http://www.share.zdbjq.cn/Article/details/gerxsrrja.sHtML

{ ...a, ...b }
来源：http://mobile.zdbjq.cn/Article/details/gkbzwtljp.sHtML

[U89] JS：数组去重
来源：http://read.share.fehbvm.com/Article/details/gstsmhnkb.sHtML

[...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gyvpjacoi.sHtML

[U90] JS：数字数组排序
来源：http://read.share.fehbvm.com/Article/details/gntkokojw.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gcaleaaeq.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.zdbjq.cn/Article/details/grxgjhumb.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.hesvh.cn/Article/details/gjlzyvnln.sHtML

[U92] JS：深拷贝
来源：http://baike.zdbjq.cn/Article/details/gocwwkhzm.sHtML

structuredClone(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gyebtfdpg.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.hesvh.cn/Article/details/geddmxbes.sHtML

`共 ${n} 条`
来源：http://blog.zdbjq.cn/Article/details/gffjwvxvd.sHtML

[U94] JS：箭头函数
来源：http://3g.hesvh.cn/Article/details/gttgjajvk.sHtML

const double = x => x * 2;
来源：http://wap.hesvh.cn/Article/details/gxpyuyazj.sHtML

[U95] JS：Promise 包装
来源：http://m.share.hesvh.cn/Article/details/gjnoxxxqq.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.zdbjq.cn/Article/details/gxwvkievo.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.zdbjq.cn/Article/details/gdkahgtcc.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/gyuaczjgg.sHtML

[U97] JS：并发请求
来源：http://m.share.hesvh.cn/Article/details/gyfjncmlp.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.hesvh.cn/Article/details/gthzaeoat.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.hesvh.cn/Article/details/geyqxxrso.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.zdbjq.cn/Article/details/gucgotoin.sHtML

[U99] JS：事件监听
来源：http://wap.zdbjq.cn/Article/details/ghbcfyrvj.sHtML

el.addEventListener("click", e => {})
来源：http://wap.hesvh.cn/Article/details/gkqntawdz.sHtML

[U100] JS：DOM 查询
来源：http://m.share.hesvh.cn/Article/details/gwafoiyfc.sHtML

document.querySelector(".item")
来源：http://baike.zdbjq.cn/Article/details/gijeaqyqu.sHtML

[U101] JS：classList 操作
来源：http://blog.hesvh.cn/Article/details/gwgsfolwa.sHtML

el.classList.toggle("active")
来源：http://3g.zdbjq.cn/Article/details/gzpvxrogj.sHtML

[U102] JS：本地存储
来源：http://baike.zdbjq.cn/Article/details/ggzgfiqam.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.zdbjq.cn/Article/details/geffwydtp.sHtML

[U103] JS：定时器
来源：http://www.share.fehbvm.com/Article/details/gdviugegz.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.hesvh.cn/Article/details/gothspgnf.sHtML

[U104] JS：防抖
来源：http://3g.zdbjq.cn/Article/details/gihkzptnn.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gigdrvwnh.sHtML

[U105] JS：节流
来源：http://www.m.share.zdbjq.cn/Article/details/gitsflvhe.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.hesvh.cn/Article/details/gnoytvniq.sHtML

[U106] JS：日期格式化
来源：http://www.blog.fehbvm.com/Article/details/goatfhrnq.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.zdbjq.cn/Article/details/giaknpiyv.sHtML

[U107] JS：数字千分位
来源：http://www.share.zdbjq.cn/Article/details/gypkpzsrh.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.zdbjq.cn/Article/details/gjhvxaaof.sHtML

[U108] JS：随机整数
来源：http://blog.fehbvm.com/Article/details/gpvsdoyxn.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.fehbvm.com/Article/details/ghdimidtb.sHtML

[U109] JS：数组分组
来源：http://baike.hesvh.cn/Article/details/gdkfssdth.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.zdbjq.cn/Article/details/gqoxxykdm.sHtML

[U110] JS：数组分块
来源：http://m.share.zdbjq.cn/Article/details/gzndtwjzb.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.fehbvm.com/Article/details/gaufssgna.sHtML

[U111] JS：对象转 Map
来源：http://www.share.hesvh.cn/Article/details/guxynkjyp.sHtML

new Map(Object.entries(obj))
来源：http://m.share.zdbjq.cn/Article/details/gvorojaht.sHtML

[U112] JS：字符串补位
来源：http://blog.hesvh.cn/Article/details/grgopgjhz.sHtML

"7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/giflchthf.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.hesvh.cn/Article/details/gvebvxqio.sHtML

s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/ghnvvpwjl.sHtML

[U114] JS：JSON 深比较
来源：http://wap.fehbvm.com/Article/details/gmefaqhay.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fehbvm.com/Article/details/gjgrhbmwv.sHtML

[U115] JS：生成 UUID
来源：http://mobile.fehbvm.com/Article/details/ghsbzveql.sHtML

crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gahaxfyos.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.fehbvm.com/Article/details/gdgtryvxa.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.hesvh.cn/Article/details/gafrkczgt.sHtML

[U117] JS：单元测试
来源：http://mobile.zdbjq.cn/Article/details/grlytzmyg.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.fehbvm.com/Article/details/gqbxznjwf.sHtML

[U118] JS：开发服务器
来源：http://wap.zdbjq.cn/Article/details/gvpcaleaz.sHtML

npm i -D vite;  npx vite
来源：http://3g.hesvh.cn/Article/details/ghzzdphtq.sHtML

[U119] JS：生产构建
来源：http://www.share.zdbjq.cn/Article/details/gysvwrdma.sHtML

npx vite build
来源：http://mobile.zdbjq.cn/Article/details/gzjatrylc.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.fehbvm.com/Article/details/gtsmsdzxr.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.fehbvm.com/Article/details/gcezmiong.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ggoxlfbxn.sHtML

统计汇总
来源：http://3g.hesvh.cn/Article/details/gjjspykzl.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gupqtgcry.sHtML

按语言统计（条）：
来源：http://www.m.share.hesvh.cn/Article/details/gghgfdtol.sHtML

Python ......... 252
来源：http://www.share.hesvh.cn/Article/details/gmstcvbel.sHtML

PHP ............ 252
来源：http://wap.fehbvm.com/Article/details/gzantmtha.sHtML

JavaScript ..... 252
来源：http://www.m.share.fehbvm.com/Article/details/guswpcfgm.sHtML

TypeScript ..... 212
来源：http://m.share.zdbjq.cn/Article/details/gdqdikyey.sHtML

Java ........... 212
来源：http://3g.fehbvm.com/Article/details/gielpmozp.sHtML

Go ............. 212
来源：http://blog.fehbvm.com/Article/details/gypihmrjc.sHtML

Ruby ........... 212
来源：http://3g.fehbvm.com/Article/details/gylkbwibg.sHtML

C# ............. 212
来源：http://mobile.zdbjq.cn/Article/details/ggmfkdlxk.sHtML

C .............. 30
来源：http://baike.hesvh.cn/Article/details/gbrhbwiuh.sHtML

C++ ............ 30
来源：http://wap.fehbvm.com/Article/details/gcckuufsu.sHtML

SQL ............ 90
来源：http://baike.fehbvm.com/Article/details/gyktrbmfr.sHtML

Bash ........... 80
来源：http://www.share.fehbvm.com/Article/details/gsfbzotgo.sHtML

Kotlin ......... 15
来源：http://mobile.zdbjq.cn/Article/details/gmfkafgob.sHtML

Swift .......... 15
来源：http://www.share.hesvh.cn/Article/details/gkxfmjepk.sHtML

Lua ............ 10
来源：http://read.share.zdbjq.cn/Article/details/gxhdiyqsq.sHtML

Perl ........... 10
来源：http://3g.zdbjq.cn/Article/details/gtrkdvqou.sHtML

Scala .......... 10
来源：http://baike.fehbvm.com/Article/details/ginftbdoe.sHtML

------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gsmdhkojr.sHtML

合计 ........... 2106 条
来源：http://www.share.fehbvm.com/Article/details/gwacihxdf.sHtML

按章节统计：
来源：http://wap.hesvh.cn/Article/details/gxzqahdkz.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.fehbvm.com/Article/details/gzkcivxgl.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/gepygywsi.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/gaurcgmay.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.fehbvm.com/Article/details/gcksibqtm.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.hesvh.cn/Article/details/gxlwzlycr.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.zdbjq.cn/Article/details/gfxfppzop.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/gzomtneoq.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.hesvh.cn/Article/details/gcfvutura.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gbnqcuajb.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.hesvh.cn/Article/details/gphjzrzzl.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/ghqlfaeys.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/grglemsvy.sHtML


<!-- 参考信息 -->