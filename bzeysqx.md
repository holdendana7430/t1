代发 wailian999

while (my $line = <$fh>) { print $line; }
来源：http://www.share.hesvh.cn/Article/details/gkpkulray.sHtML

[T51] Scala：Hello World
来源：http://3g.fehbvm.com/Article/details/ghjxxnyae.sHtML

println("Hello")
来源：http://3g.hesvh.cn/Article/details/gyzlvwsnu.sHtML

[T52] Scala：变量
来源：http://read.share.fehbvm.com/Article/details/goxhtycpj.sHtML

val a = 1;  var b = 2
来源：http://read.share.zdbjq.cn/Article/details/gdxdopkna.sHtML

[T53] Scala：字符串插值
来源：http://baike.fehbvm.com/Article/details/grwhkbqba.sHtML

s"值: $b"
来源：http://baike.fehbvm.com/Article/details/gmrzmhdvm.sHtML

[T54] Scala：集合映射
来源：http://baike.fehbvm.com/Article/details/gurbymizl.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.fehbvm.com/Article/details/gaejbwkeu.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.fehbvm.com/Article/details/ghgmigrwi.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.zdbjq.cn/Article/details/glnxvpxum.sHtML

[T56] Scala：样例类
来源：http://wap.zdbjq.cn/Article/details/gfdhehufi.sHtML

case class User(name: String, age: Int)
来源：http://3g.fehbvm.com/Article/details/gadroyfpl.sHtML

[T57] Scala：模式匹配
来源：http://baike.zdbjq.cn/Article/details/gjlfpzdpx.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.zdbjq.cn/Article/details/gohgudnfs.sHtML

[T58] Scala：函数定义
来源：http://blog.zdbjq.cn/Article/details/guwurovhx.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.zdbjq.cn/Article/details/gjurqvwox.sHtML

[T59] Scala：循环
来源：http://3g.hesvh.cn/Article/details/gysfmwxil.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.zdbjq.cn/Article/details/gklltysfu.sHtML

[T60] Scala：折叠
来源：http://mobile.fehbvm.com/Article/details/gmqvwrygg.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.zdbjq.cn/Article/details/gntptlspr.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gtiggjmhu.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.hesvh.cn/Article/details/gvfqsbdsp.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gdjbmcigg.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.fehbvm.com/Article/details/ghrcufctc.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.zdbjq.cn/Article/details/gelczfggz.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.hesvh.cn/Article/details/gcxhtpyct.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.hesvh.cn/Article/details/gkgjhcqca.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.fehbvm.com/Article/details/gbckoziiz.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.zdbjq.cn/Article/details/gjtxxqbww.sHtML

[U04] Py：变量调试打印
来源：http://blog.hesvh.cn/Article/details/gvmewxzmi.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.hesvh.cn/Article/details/gczwzafqv.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.zdbjq.cn/Article/details/gkjuykmre.sHtML

list(dict.fromkeys(arr))
来源：http://blog.hesvh.cn/Article/details/glagiakxo.sHtML

[U06] Py：合并两个字典
来源：http://www.share.hesvh.cn/Article/details/gphpkfzyk.sHtML

{**a, **b}
来源：http://wap.hesvh.cn/Article/details/gsgykxfbv.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.fehbvm.com/Article/details/gtmcahcwm.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.hesvh.cn/Article/details/gouvrussi.sHtML

[U08] Py：展平二维列表
来源：http://read.share.hesvh.cn/Article/details/gqvicyzqi.sHtML

[y for x in nested for y in x]
来源：http://3g.hesvh.cn/Article/details/gixuurbxv.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.zdbjq.cn/Article/details/gbymkvlta.sHtML

max(d, key=d.get)
来源：http://3g.hesvh.cn/Article/details/gvimdnsoe.sHtML

[U10] Py：按值排序字典
来源：http://blog.hesvh.cn/Article/details/gehxwtkak.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.fehbvm.com/Article/details/gdwdkidos.sHtML

[U11] Py：生成器表达式
来源：http://wap.fehbvm.com/Article/details/goznmldnf.sHtML

(x * 2 for x in arr)
来源：http://www.share.zdbjq.cn/Article/details/gkgqnwqsp.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.hesvh.cn/Article/details/gjmnltqyb.sHtML

Counter(arr).most_common(3)
来源：http://wap.fehbvm.com/Article/details/gqqfbncex.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.fehbvm.com/Article/details/gmgcvvrtr.sHtML

deque(maxlen=10)
来源：http://www.m.share.fehbvm.com/Article/details/gogpeifkw.sHtML

[U14] Py：分组收集到列表
来源：http://baike.zdbjq.cn/Article/details/gpikedmku.sHtML

defaultdict(list)
来源：http://read.share.fehbvm.com/Article/details/giuzwdjro.sHtML

[U15] Py：高精度计时
来源：http://3g.hesvh.cn/Article/details/gmnlialkd.sHtML

t = time.perf_counter()
来源：http://read.share.zdbjq.cn/Article/details/gkpswfmfr.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.zdbjq.cn/Article/details/gbninuhoz.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fehbvm.com/Article/details/gvzmwoejf.sHtML

[U17] Py：初始化日志
来源：http://baike.zdbjq.cn/Article/details/gwzjbrrdm.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.zdbjq.cn/Article/details/gerucfmnk.sHtML

[U18] Py：预编译正则
来源：http://www.blog.hesvh.cn/Article/details/ghzhprjva.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.hesvh.cn/Article/details/ghquvydad.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.fehbvm.com/Article/details/ghrgxogoq.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.zdbjq.cn/Article/details/gyikvusux.sHtML

[U20] Py：缓存函数结果
来源：http://blog.hesvh.cn/Article/details/gigtmctkr.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.fehbvm.com/Article/details/gvivezfuz.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.hesvh.cn/Article/details/gcuvpzcrt.sHtML

@contextlib.contextmanager
来源：http://m.share.fehbvm.com/Article/details/gemdkpvvp.sHtML

[U22] Py：矩阵转置
来源：http://mobile.fehbvm.com/Article/details/gevsfkdkc.sHtML

list(zip(*m))
来源：http://read.share.zdbjq.cn/Article/details/gqjruprpz.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.zdbjq.cn/Article/details/gmfhhsbvm.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.fehbvm.com/Article/details/gvpwmjhly.sHtML

[U24] Py：路径操作
来源：http://www.blog.fehbvm.com/Article/details/guzfgngyr.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.zdbjq.cn/Article/details/gdkoaxqhg.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.zdbjq.cn/Article/details/gfpuxbgug.sHtML

csv.DictReader(f)
来源：http://3g.hesvh.cn/Article/details/glgrynylt.sHtML

[U26] Py：并发下载
来源：http://read.share.hesvh.cn/Article/details/gnbhqxezb.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.fehbvm.com/Article/details/gnmwsrldk.sHtML

[U27] Py：异步 HTTP
来源：http://3g.zdbjq.cn/Article/details/gxodirljh.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.fehbvm.com/Article/details/gyyqjxjyl.sHtML

[U28] Py：类型别名
来源：http://www.share.fehbvm.com/Article/details/gnfxhqzil.sHtML

UserId = int
来源：http://www.m.share.fehbvm.com/Article/details/gnxrvlhoq.sHtML

[U29] Py：属性校验
来源：http://www.m.share.fehbvm.com/Article/details/grpekqxka.sHtML

@property 与 @x.setter 配合
来源：http://m.share.fehbvm.com/Article/details/gjarnenxj.sHtML

[U30] Py：数据类
来源：http://www.share.fehbvm.com/Article/details/gwgdybnoc.sHtML

@dataclass(slots=True)
来源：http://www.m.share.hesvh.cn/Article/details/gzyyopyol.sHtML

[U31] Py：单测
来源：http://www.share.zdbjq.cn/Article/details/ganpyxxqx.sHtML

python -m pytest -q
来源：http://baike.zdbjq.cn/Article/details/gzndyabfa.sHtML

[U32] Py：代码格式化
来源：http://3g.fehbvm.com/Article/details/gokllmkjb.sHtML

ruff format . && ruff check --fix .
来源：http://blog.hesvh.cn/Article/details/gqcsqxltf.sHtML

[U33] Py：打包发布
来源：http://www.m.share.zdbjq.cn/Article/details/gsfmyzhny.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.zdbjq.cn/Article/details/ggoluawva.sHtML

[U34] Py：判断编码
来源：http://www.m.share.hesvh.cn/Article/details/gdbtrhmuc.sHtML

chardet.detect(raw)
来源：http://baike.hesvh.cn/Article/details/gjyxdsfgp.sHtML

[U35] Py：发送邮件
来源：http://m.share.hesvh.cn/Article/details/guutmtsnc.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.fehbvm.com/Article/details/gvdiroeuu.sHtML

[U36] Py：定时任务
来源：http://blog.hesvh.cn/Article/details/gynvcingp.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.zdbjq.cn/Article/details/gbowzqkog.sHtML

[U37] Py：读写 Excel
来源：http://mobile.fehbvm.com/Article/details/giupqnikf.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.hesvh.cn/Article/details/gklwqlswc.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.hesvh.cn/Article/details/gqaxixrvf.sHtML

Path(__file__).resolve().parent
来源：http://baike.zdbjq.cn/Article/details/gbkgadfvc.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.zdbjq.cn/Article/details/gsfxaenpf.sHtML

sys.stdout.isatty()
来源：http://www.blog.hesvh.cn/Article/details/guqfculif.sHtML

[U40] Py：打印到标准错误
来源：http://3g.hesvh.cn/Article/details/gjghsfqww.sHtML

print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/guzjqejze.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.zdbjq.cn/Article/details/gbfiemair.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.zdbjq.cn/Article/details/gdovmuhbi.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.hesvh.cn/Article/details/ghhahubip.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.hesvh.cn/Article/details/gerwghyrd.sHtML

[U43] PHP：声明命名空间
来源：http://blog.zdbjq.cn/Article/details/gguadjggo.sHtML

namespace App\Http;
来源：http://baike.zdbjq.cn/Article/details/gkyduzmwu.sHtML

[U44] PHP：开启严格类型
来源：http://3g.fehbvm.com/Article/details/gbffmklxj.sHtML

declare(strict_types=1);
来源：http://www.blog.zdbjq.cn/Article/details/gtrxvfjvy.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.fehbvm.com/Article/details/gnfjuluqf.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gbiqugvrz.sHtML

[U46] PHP：可空类型
来源：http://blog.fehbvm.com/Article/details/guxkgxqey.sHtML

?string $name = null
来源：http://read.share.fehbvm.com/Article/details/gldqmkisy.sHtML

[U47] PHP：联合类型
来源：http://mobile.hesvh.cn/Article/details/gcipdplja.sHtML

int|string $id
来源：http://wap.hesvh.cn/Article/details/gyjrvmmfm.sHtML

[U48] PHP：纯枚举
来源：http://baike.zdbjq.cn/Article/details/gxrqvjipf.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.zdbjq.cn/Article/details/ggdqovuum.sHtML

[U49] PHP：只读属性
来源：http://3g.zdbjq.cn/Article/details/gbmskcozc.sHtML

public readonly string $name
来源：http://mobile.fehbvm.com/Article/details/guofgfhhw.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.zdbjq.cn/Article/details/gnhjosskp.sHtML

public function __construct(private int $id) {}
来源：http://baike.fehbvm.com/Article/details/greiesyym.sHtML

[U51] PHP：数组解构
来源：http://mobile.zdbjq.cn/Article/details/gbktgqxai.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.hesvh.cn/Article/details/gxcndwuho.sHtML

[U52] PHP：箭头函数
来源：http://blog.fehbvm.com/Article/details/gkwhpcgzo.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.hesvh.cn/Article/details/geuhvyrzf.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.zdbjq.cn/Article/details/gdiofedye.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.zdbjq.cn/Article/details/gmumzhhhn.sHtML

[U54] PHP：空安全调用
来源：http://www.share.hesvh.cn/Article/details/gjldaeqzb.sHtML

$obj?->method()
来源：http://www.m.share.zdbjq.cn/Article/details/gpamuosyh.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.hesvh.cn/Article/details/ggekxfgdr.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.hesvh.cn/Article/details/gvklyxtcx.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.fehbvm.com/Article/details/ggqxngurv.sHtML

f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/gvbqzpttu.sHtML

[U57] PHP：字符串插值
来源：http://mobile.hesvh.cn/Article/details/guyajdmcw.sHtML

"值: {$a}"
来源：http://wap.hesvh.cn/Article/details/gtcmedpug.sHtML

[U58] PHP：数组三件套
来源：http://3g.fehbvm.com/Article/details/gauomawez.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.fehbvm.com/Article/details/gcidoiwnn.sHtML

[U59] PHP：自定义排序
来源：http://read.share.fehbvm.com/Article/details/gikfqfguv.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.zdbjq.cn/Article/details/gkbfonnbx.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.fehbvm.com/Article/details/gwpqoldlm.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.fehbvm.com/Article/details/gfxxxmzeh.sHtML

[U61] PHP：正则
来源：http://blog.zdbjq.cn/Article/details/guivupseg.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.hesvh.cn/Article/details/ghpjonclb.sHtML

[U62] PHP：日期对象
来源：http://wap.hesvh.cn/Article/details/gjmltdxrn.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.fehbvm.com/Article/details/gigrydqgo.sHtML

[U63] PHP：文件读写
来源：http://www.share.hesvh.cn/Article/details/gmgdtzybn.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.hesvh.cn/Article/details/gnovwtihd.sHtML

[U64] PHP：目录遍历
来源：http://m.share.hesvh.cn/Article/details/gioaldyau.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.zdbjq.cn/Article/details/gmdmarbsk.sHtML

[U65] PHP：会话
来源：http://wap.hesvh.cn/Article/details/gkdhpzlsy.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gixpgqytl.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.fehbvm.com/Article/details/ggjiqdeda.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.hesvh.cn/Article/details/gkqcegddn.sHtML

[U67] PHP：处理文件上传
来源：http://wap.hesvh.cn/Article/details/gshtwaocy.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.hesvh.cn/Article/details/goipntcgk.sHtML

[U68] PHP：PDO 连接
来源：http://wap.fehbvm.com/Article/details/gzukszyjz.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.hesvh.cn/Article/details/gplevyfnc.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.zdbjq.cn/Article/details/gmsvtoqsf.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.fehbvm.com/Article/details/gydchzmpe.sHtML

[U70] PHP：PDO 事务
来源：http://wap.hesvh.cn/Article/details/gwwjokuxj.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.hesvh.cn/Article/details/gxcftqppr.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.hesvh.cn/Article/details/gccqzsjcq.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.fehbvm.com/Article/details/ggpxkrlar.sHtML

[U72] PHP：写错误日志
来源：http://read.share.fehbvm.com/Article/details/gkdfoequc.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.fehbvm.com/Article/details/gxhsxjvkh.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.hesvh.cn/Article/details/gxtvnysog.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.hesvh.cn/Article/details/gnwgfwtkx.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.zdbjq.cn/Article/details/ghyvqdstc.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.hesvh.cn/Article/details/grqsutuiu.sHtML

[U75] PHP：依赖注入
来源：http://mobile.fehbvm.com/Article/details/gzmsvnhst.sHtML

composer require psr/container
来源：http://mobile.fehbvm.com/Article/details/gisblxzfy.sHtML

[U76] PHP：简单路由
来源：http://mobile.fehbvm.com/Article/details/gdfmimtny.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.fehbvm.com/Article/details/gnhwmruia.sHtML

[U77] PHP：模板渲染
来源：http://mobile.fehbvm.com/Article/details/glyjrfuro.sHtML

composer require twig/twig
来源：http://www.m.share.hesvh.cn/Article/details/gcvtgivho.sHtML

[U78] PHP：单元测试
来源：http://3g.zdbjq.cn/Article/details/glrxytvwp.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.zdbjq.cn/Article/details/gkvelwtrw.sHtML

[U79] PHP：静态分析
来源：http://blog.fehbvm.com/Article/details/gppafwdfz.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.hesvh.cn/Article/details/ggfdydizf.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.zdbjq.cn/Article/details/gmzglfkac.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.fehbvm.com/Article/details/gspvxepky.sHtML

[U81] JS：初始化项目
来源：http://www.blog.fehbvm.com/Article/details/gnumutrxf.sHtML

npm init -y;  npm i express
来源：http://www.m.share.hesvh.cn/Article/details/gfmhjzdrm.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.fehbvm.com/Article/details/gmlrpgrxx.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.hesvh.cn/Article/details/gakikaolu.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.hesvh.cn/Article/details/gxxkpqkzx.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.hesvh.cn/Article/details/gxubjdupl.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.hesvh.cn/Article/details/gvterfftj.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.hesvh.cn/Article/details/gvnbfzquy.sHtML

[U85] JS：可选链
来源：http://blog.hesvh.cn/Article/details/gutnfkjxl.sHtML

a?.b?.c
来源：http://blog.zdbjq.cn/Article/details/gaiahjwir.sHtML

[U86] JS：空值合并
来源：http://mobile.hesvh.cn/Article/details/gygierrjq.sHtML

a ?? b
来源：http://wap.hesvh.cn/Article/details/gphylnner.sHtML

[U87] JS：解构默认值
来源：http://read.share.hesvh.cn/Article/details/gixoudrst.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.zdbjq.cn/Article/details/gswsohndd.sHtML

[U88] JS：对象展开合并
来源：http://blog.zdbjq.cn/Article/details/gzvbcralg.sHtML

{ ...a, ...b }
来源：http://mobile.hesvh.cn/Article/details/gspssxzhm.sHtML

[U89] JS：数组去重
来源：http://baike.fehbvm.com/Article/details/gzdxwqfov.sHtML

[...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/gvgdhhikp.sHtML

[U90] JS：数字数组排序
来源：http://mobile.fehbvm.com/Article/details/gdwirzqso.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gxnzveljr.sHtML

[U91] JS：对象键值遍历
来源：http://3g.fehbvm.com/Article/details/gvsifwwza.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.fehbvm.com/Article/details/gklkxmdwb.sHtML

[U92] JS：深拷贝
来源：http://www.blog.fehbvm.com/Article/details/gcobybbjx.sHtML

structuredClone(obj)
来源：http://www.blog.hesvh.cn/Article/details/gsmpbxpan.sHtML

[U93] JS：模板字符串
来源：http://read.share.zdbjq.cn/Article/details/goldbdvxx.sHtML

`共 ${n} 条`
来源：http://www.m.share.zdbjq.cn/Article/details/gutwvucyh.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.zdbjq.cn/Article/details/gyzrfvrwx.sHtML

const double = x => x * 2;
来源：http://baike.zdbjq.cn/Article/details/ggnqeeojv.sHtML

[U95] JS：Promise 包装
来源：http://blog.hesvh.cn/Article/details/gxufcvstz.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.hesvh.cn/Article/details/gqgrgfgxo.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.zdbjq.cn/Article/details/gnxpolqsw.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/gzlznfbvu.sHtML

[U97] JS：并发请求
来源：http://www.blog.hesvh.cn/Article/details/geqmqbvip.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/glltoeafj.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.hesvh.cn/Article/details/glzkyzzrb.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.hesvh.cn/Article/details/gggomfiji.sHtML

[U99] JS：事件监听
来源：http://www.share.zdbjq.cn/Article/details/gkcsisree.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.zdbjq.cn/Article/details/gguwsvvvo.sHtML

[U100] JS：DOM 查询
来源：http://baike.hesvh.cn/Article/details/gxzzbwggu.sHtML

document.querySelector(".item")
来源：http://www.blog.fehbvm.com/Article/details/gsrdqidqv.sHtML

[U101] JS：classList 操作
来源：http://www.blog.zdbjq.cn/Article/details/gackrmcgw.sHtML

el.classList.toggle("active")
来源：http://baike.zdbjq.cn/Article/details/gutwflgaw.sHtML

[U102] JS：本地存储
来源：http://blog.zdbjq.cn/Article/details/gcuikomwq.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.fehbvm.com/Article/details/guebvinfp.sHtML

[U103] JS：定时器
来源：http://baike.fehbvm.com/Article/details/giyhltkwe.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.zdbjq.cn/Article/details/glskvxggg.sHtML

[U104] JS：防抖
来源：http://baike.hesvh.cn/Article/details/gquptpmog.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/gszjukmiv.sHtML

[U105] JS：节流
来源：http://m.share.hesvh.cn/Article/details/gketmgqez.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.zdbjq.cn/Article/details/gxqyjdkal.sHtML

[U106] JS：日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gbxargxpp.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.hesvh.cn/Article/details/gljneijeq.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.zdbjq.cn/Article/details/gguuenolh.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.fehbvm.com/Article/details/gcnorjxop.sHtML

[U108] JS：随机整数
来源：http://m.share.fehbvm.com/Article/details/gjritkiva.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.fehbvm.com/Article/details/gwheuouwk.sHtML

[U109] JS：数组分组
来源：http://mobile.hesvh.cn/Article/details/gcyazjnzb.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.hesvh.cn/Article/details/ghptnamsg.sHtML

[U110] JS：数组分块
来源：http://3g.fehbvm.com/Article/details/gtkvwgfei.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.fehbvm.com/Article/details/gsskyophm.sHtML

[U111] JS：对象转 Map
来源：http://wap.fehbvm.com/Article/details/gcmxytuix.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.zdbjq.cn/Article/details/gpcodbxgf.sHtML

[U112] JS：字符串补位
来源：http://3g.fehbvm.com/Article/details/gwyehejwm.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/ghegegvlx.sHtML

[U113] JS：正则替换全部
来源：http://www.share.zdbjq.cn/Article/details/gczvrqzxk.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gtzyxinnq.sHtML

[U114] JS：JSON 深比较
来源：http://blog.hesvh.cn/Article/details/gpkeurpyz.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fehbvm.com/Article/details/gsyjlhnaw.sHtML

[U115] JS：生成 UUID
来源：http://read.share.zdbjq.cn/Article/details/gxkrudiqn.sHtML

crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gsobdtugi.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.fehbvm.com/Article/details/gxosxwhnk.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.hesvh.cn/Article/details/gxtbuwvyk.sHtML

[U117] JS：单元测试
来源：http://blog.fehbvm.com/Article/details/gqdphfxla.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.hesvh.cn/Article/details/gptlezdpo.sHtML

[U118] JS：开发服务器
来源：http://www.share.hesvh.cn/Article/details/gwujtdrul.sHtML

npm i -D vite;  npx vite
来源：http://wap.zdbjq.cn/Article/details/gnlljtifc.sHtML

[U119] JS：生产构建
来源：http://mobile.fehbvm.com/Article/details/gtyjleuna.sHtML

npx vite build
来源：http://m.share.hesvh.cn/Article/details/guaujzmoh.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.fehbvm.com/Article/details/grwkojftx.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.fehbvm.com/Article/details/gzbknhtfs.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gdphwbqnh.sHtML

统计汇总
来源：http://mobile.hesvh.cn/Article/details/ghwqwjxol.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/goffgmjft.sHtML

按语言统计（条）：
来源：http://mobile.zdbjq.cn/Article/details/goiptkxew.sHtML

Python ......... 252
来源：http://read.share.hesvh.cn/Article/details/gujmhnqtc.sHtML

PHP ............ 252
来源：http://www.blog.fehbvm.com/Article/details/gkkkdsltm.sHtML

JavaScript ..... 252
来源：http://baike.zdbjq.cn/Article/details/gwwrjsvhv.sHtML

TypeScript ..... 212
来源：http://wap.fehbvm.com/Article/details/gpnvqfaof.sHtML

Java ........... 212
来源：http://www.share.zdbjq.cn/Article/details/goqxvseth.sHtML

Go ............. 212
来源：http://www.m.share.zdbjq.cn/Article/details/gaappjhuv.sHtML

Ruby ........... 212
来源：http://blog.zdbjq.cn/Article/details/gyigairaw.sHtML

C# ............. 212
来源：http://blog.fehbvm.com/Article/details/gukblwdls.sHtML

C .............. 30
来源：http://www.m.share.fehbvm.com/Article/details/glbvqxyao.sHtML

C++ ............ 30
来源：http://www.m.share.fehbvm.com/Article/details/gjqifcpyj.sHtML

SQL ............ 90
来源：http://mobile.hesvh.cn/Article/details/glmwyymsc.sHtML

Bash ........... 80
来源：http://read.share.zdbjq.cn/Article/details/gmcvulrld.sHtML

Kotlin ......... 15
来源：http://read.share.hesvh.cn/Article/details/gflawpdcv.sHtML

Swift .......... 15
来源：http://blog.fehbvm.com/Article/details/gifwqcaib.sHtML

Lua ............ 10
来源：http://wap.hesvh.cn/Article/details/gtewqkvfo.sHtML

Perl ........... 10
来源：http://www.share.hesvh.cn/Article/details/gbcyxqbhp.sHtML

Scala .......... 10
来源：http://www.m.share.zdbjq.cn/Article/details/ghjuihsoi.sHtML

------------------------------------
来源：http://m.share.fehbvm.com/Article/details/goovkiurh.sHtML

合计 ........... 2106 条
来源：http://baike.zdbjq.cn/Article/details/gthgdjhze.sHtML

按章节统计：
来源：http://m.share.hesvh.cn/Article/details/govvvxixm.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.hesvh.cn/Article/details/gzlmmlndh.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/gpxnodhxf.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/gutubsclw.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.zdbjq.cn/Article/details/gxqhxygsm.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.hesvh.cn/Article/details/gvmzbswxc.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.hesvh.cn/Article/details/gfuytqwow.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.zdbjq.cn/Article/details/gkmvjdnsw.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.hesvh.cn/Article/details/goswnkzsq.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/ggarpftvz.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.hesvh.cn/Article/details/gpxnmrinc.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/ggqhschjs.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gaqskvhdn.sHtML


<!-- 参考信息 -->