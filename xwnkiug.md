代发 wailian999

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.fehbvm.com/Article/details/gxujswsye.sHtML

[T51] Scala：Hello World
来源：http://read.share.hesvh.cn/Article/details/gttrtzuix.sHtML

println("Hello")
来源：http://wap.hesvh.cn/Article/details/gjngedwox.sHtML

[T52] Scala：变量
来源：http://wap.zdbjq.cn/Article/details/gdahchgrm.sHtML

val a = 1;  var b = 2
来源：http://read.share.zdbjq.cn/Article/details/gkyzbzoat.sHtML

[T53] Scala：字符串插值
来源：http://baike.fehbvm.com/Article/details/goqkboxwp.sHtML

s"值: $b"
来源：http://baike.zdbjq.cn/Article/details/gmuxmguzh.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.fehbvm.com/Article/details/gptznwfpw.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.fehbvm.com/Article/details/glytzjzlv.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.fehbvm.com/Article/details/galftsjxv.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.hesvh.cn/Article/details/garsycced.sHtML

[T56] Scala：样例类
来源：http://www.share.fehbvm.com/Article/details/guahdfsau.sHtML

case class User(name: String, age: Int)
来源：http://3g.fehbvm.com/Article/details/gculwjxvj.sHtML

[T57] Scala：模式匹配
来源：http://baike.fehbvm.com/Article/details/gvbkfmsze.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.zdbjq.cn/Article/details/gleqzylmw.sHtML

[T58] Scala：函数定义
来源：http://mobile.fehbvm.com/Article/details/gvwlgluol.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.zdbjq.cn/Article/details/gknzjvxzl.sHtML

[T59] Scala：循环
来源：http://3g.hesvh.cn/Article/details/gduhyyula.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.hesvh.cn/Article/details/gtdaqqqtz.sHtML

[T60] Scala：折叠
来源：http://wap.zdbjq.cn/Article/details/grvjsbqks.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.fehbvm.com/Article/details/gyfkelnaw.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ghtjmszlu.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.fehbvm.com/Article/details/ggoaumise.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gkisdgrah.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.hesvh.cn/Article/details/gysqieqmf.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.fehbvm.com/Article/details/glzcfreqw.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.fehbvm.com/Article/details/gdzekygsh.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.fehbvm.com/Article/details/gpfoemykp.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.hesvh.cn/Article/details/gfqxdxuqm.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.zdbjq.cn/Article/details/gpeullsdo.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.zdbjq.cn/Article/details/gzbvwkjka.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fehbvm.com/Article/details/gtbzdiytu.sHtML

[U05] Py：列表去重且保序
来源：http://baike.zdbjq.cn/Article/details/gquqkmiaz.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.fehbvm.com/Article/details/gxwkbwxpx.sHtML

[U06] Py：合并两个字典
来源：http://baike.fehbvm.com/Article/details/gxzihjxip.sHtML

{**a, **b}
来源：http://www.share.fehbvm.com/Article/details/gpbgihbwe.sHtML

[U07] Py：反转字典键值
来源：http://baike.hesvh.cn/Article/details/gnbldtigu.sHtML

{v: k for k, v in d.items()}
来源：http://3g.fehbvm.com/Article/details/gmdmxhcgh.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.fehbvm.com/Article/details/gxvpeviqe.sHtML

[y for x in nested for y in x]
来源：http://www.share.hesvh.cn/Article/details/guczscpyr.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.fehbvm.com/Article/details/glxuivuty.sHtML

max(d, key=d.get)
来源：http://www.blog.fehbvm.com/Article/details/gigvrapek.sHtML

[U10] Py：按值排序字典
来源：http://wap.hesvh.cn/Article/details/gjsiflith.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.zdbjq.cn/Article/details/gtfqstnxs.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.hesvh.cn/Article/details/guurrgjex.sHtML

(x * 2 for x in arr)
来源：http://mobile.hesvh.cn/Article/details/gmngpcmiy.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.zdbjq.cn/Article/details/gfzlgmgsl.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gwaxvijzq.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.zdbjq.cn/Article/details/ggffnpckw.sHtML

deque(maxlen=10)
来源：http://blog.hesvh.cn/Article/details/gzisferyd.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.fehbvm.com/Article/details/gbrzqbxla.sHtML

defaultdict(list)
来源：http://3g.hesvh.cn/Article/details/gfltnqcsg.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.fehbvm.com/Article/details/ggniqjbmo.sHtML

t = time.perf_counter()
来源：http://www.m.share.fehbvm.com/Article/details/georddzmc.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.zdbjq.cn/Article/details/gnqmcnqsg.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.fehbvm.com/Article/details/gymzzodmd.sHtML

[U17] Py：初始化日志
来源：http://www.blog.hesvh.cn/Article/details/grduuyflc.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.fehbvm.com/Article/details/guhdmaydz.sHtML

[U18] Py：预编译正则
来源：http://baike.fehbvm.com/Article/details/gfhvpysaz.sHtML

pat = re.compile(r"\d+")
来源：http://baike.zdbjq.cn/Article/details/gxuqufhma.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.fehbvm.com/Article/details/gutiuljdd.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.fehbvm.com/Article/details/gdubaucsr.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.fehbvm.com/Article/details/gcwxpjjax.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.hesvh.cn/Article/details/gbtbiklda.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.fehbvm.com/Article/details/gxkmdlrgf.sHtML

@contextlib.contextmanager
来源：http://read.share.zdbjq.cn/Article/details/gmqrpkxso.sHtML

[U22] Py：矩阵转置
来源：http://3g.hesvh.cn/Article/details/gmofifbvf.sHtML

list(zip(*m))
来源：http://read.share.fehbvm.com/Article/details/gshirgomx.sHtML

[U23] Py：分块读取大文件
来源：http://3g.hesvh.cn/Article/details/gabkcemkc.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.hesvh.cn/Article/details/gnzmowfaz.sHtML

[U24] Py：路径操作
来源：http://3g.fehbvm.com/Article/details/glyvvsbuj.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.fehbvm.com/Article/details/gsafgoqlg.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.hesvh.cn/Article/details/gbqzymduv.sHtML

csv.DictReader(f)
来源：http://read.share.hesvh.cn/Article/details/gtschcglk.sHtML

[U26] Py：并发下载
来源：http://wap.zdbjq.cn/Article/details/gtjqirhnp.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.hesvh.cn/Article/details/gaxqwjmju.sHtML

[U27] Py：异步 HTTP
来源：http://3g.zdbjq.cn/Article/details/gtincegtp.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.hesvh.cn/Article/details/gxkkadkxm.sHtML

[U28] Py：类型别名
来源：http://www.m.share.zdbjq.cn/Article/details/gacaipivu.sHtML

UserId = int
来源：http://wap.zdbjq.cn/Article/details/gvqtqtplf.sHtML

[U29] Py：属性校验
来源：http://www.share.hesvh.cn/Article/details/gsbwgbcid.sHtML

@property 与 @x.setter 配合
来源：http://www.share.hesvh.cn/Article/details/gygjjkyqg.sHtML

[U30] Py：数据类
来源：http://www.share.hesvh.cn/Article/details/grvtpajac.sHtML

@dataclass(slots=True)
来源：http://www.share.hesvh.cn/Article/details/guomydlxi.sHtML

[U31] Py：单测
来源：http://read.share.hesvh.cn/Article/details/grkawtjdt.sHtML

python -m pytest -q
来源：http://read.share.hesvh.cn/Article/details/gsljowlqc.sHtML

[U32] Py：代码格式化
来源：http://www.blog.zdbjq.cn/Article/details/gpqljopvv.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.hesvh.cn/Article/details/gucfpmkik.sHtML

[U33] Py：打包发布
来源：http://mobile.hesvh.cn/Article/details/gnnxlkekq.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.fehbvm.com/Article/details/gnqpdnmof.sHtML

[U34] Py：判断编码
来源：http://www.blog.zdbjq.cn/Article/details/gfmzhrbpz.sHtML

chardet.detect(raw)
来源：http://m.share.zdbjq.cn/Article/details/gcgtuoefg.sHtML

[U35] Py：发送邮件
来源：http://baike.zdbjq.cn/Article/details/giutqsmlj.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.fehbvm.com/Article/details/gdwbjtjfe.sHtML

[U36] Py：定时任务
来源：http://mobile.fehbvm.com/Article/details/gmbwvzspx.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.hesvh.cn/Article/details/gnodpmfaw.sHtML

[U37] Py：读写 Excel
来源：http://m.share.zdbjq.cn/Article/details/gcbbfsnhn.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.zdbjq.cn/Article/details/gpucxxxif.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.hesvh.cn/Article/details/gafdhkozk.sHtML

Path(__file__).resolve().parent
来源：http://blog.zdbjq.cn/Article/details/gqsaonkfr.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.zdbjq.cn/Article/details/gbvtdmadx.sHtML

sys.stdout.isatty()
来源：http://mobile.fehbvm.com/Article/details/gangklgll.sHtML

[U40] Py：打印到标准错误
来源：http://wap.hesvh.cn/Article/details/gkfwspeit.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.zdbjq.cn/Article/details/gfshsazks.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.fehbvm.com/Article/details/gjsliuwmp.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.fehbvm.com/Article/details/gyhdzmfmy.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.zdbjq.cn/Article/details/gxwpuyyem.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.zdbjq.cn/Article/details/gkecutpnx.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.zdbjq.cn/Article/details/gobpzmhmq.sHtML

namespace App\Http;
来源：http://www.blog.fehbvm.com/Article/details/gljqgrsvw.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.zdbjq.cn/Article/details/gjsuqzvya.sHtML

declare(strict_types=1);
来源：http://baike.fehbvm.com/Article/details/gnsdifbdx.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.zdbjq.cn/Article/details/glvwlojwq.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gnigxpkfz.sHtML

[U46] PHP：可空类型
来源：http://read.share.hesvh.cn/Article/details/gtcgvdrbt.sHtML

?string $name = null
来源：http://blog.hesvh.cn/Article/details/gvhiemsak.sHtML

[U47] PHP：联合类型
来源：http://baike.fehbvm.com/Article/details/grmolzsux.sHtML

int|string $id
来源：http://baike.zdbjq.cn/Article/details/gputblvfw.sHtML

[U48] PHP：纯枚举
来源：http://blog.hesvh.cn/Article/details/gcxbkrlgn.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.hesvh.cn/Article/details/gbilbwlqo.sHtML

[U49] PHP：只读属性
来源：http://baike.zdbjq.cn/Article/details/gjqcwijvc.sHtML

public readonly string $name
来源：http://www.blog.hesvh.cn/Article/details/gollztrwh.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.zdbjq.cn/Article/details/gdejjjlke.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.hesvh.cn/Article/details/geeavebaf.sHtML

[U51] PHP：数组解构
来源：http://m.share.fehbvm.com/Article/details/gzcuylkvc.sHtML

[$a, $b] = $arr;
来源：http://www.blog.hesvh.cn/Article/details/gwkjzsgpc.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.zdbjq.cn/Article/details/gjemjegzv.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.fehbvm.com/Article/details/giuhrkvgj.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.hesvh.cn/Article/details/gbpugrjbd.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.fehbvm.com/Article/details/gswlocnux.sHtML

[U54] PHP：空安全调用
来源：http://m.share.zdbjq.cn/Article/details/gipuofaed.sHtML

$obj?->method()
来源：http://baike.hesvh.cn/Article/details/ggujswsvt.sHtML

[U55] PHP：match 表达式
来源：http://read.share.zdbjq.cn/Article/details/gmpeyvyvw.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.zdbjq.cn/Article/details/gqjpuslcz.sHtML

[U56] PHP：命名参数
来源：http://read.share.zdbjq.cn/Article/details/gebybbdwt.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/gtveorwqk.sHtML

[U57] PHP：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gpsawwfvu.sHtML

"值: {$a}"
来源：http://blog.zdbjq.cn/Article/details/gfcdzxwcg.sHtML

[U58] PHP：数组三件套
来源：http://mobile.zdbjq.cn/Article/details/ggttbatil.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.zdbjq.cn/Article/details/gbizcuoxu.sHtML

[U59] PHP：自定义排序
来源：http://mobile.fehbvm.com/Article/details/gmcmfrcfv.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.hesvh.cn/Article/details/gfebbexex.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.hesvh.cn/Article/details/gbhcjjfpn.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.zdbjq.cn/Article/details/gigxnynod.sHtML

[U61] PHP：正则
来源：http://mobile.hesvh.cn/Article/details/gasffvatj.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/ggsmzwckv.sHtML

[U62] PHP：日期对象
来源：http://baike.zdbjq.cn/Article/details/gxeshzqlr.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.fehbvm.com/Article/details/gxbbvbnzi.sHtML

[U63] PHP：文件读写
来源：http://www.share.hesvh.cn/Article/details/gxfexsppy.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.hesvh.cn/Article/details/gttbhjfkc.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.hesvh.cn/Article/details/givzdlleo.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.fehbvm.com/Article/details/gitrwzstx.sHtML

[U65] PHP：会话
来源：http://blog.zdbjq.cn/Article/details/gspmtfnvt.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gegkjcwsh.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.hesvh.cn/Article/details/gtpxunsfe.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.fehbvm.com/Article/details/gmlizciww.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.zdbjq.cn/Article/details/gkjniofdl.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.hesvh.cn/Article/details/glbgggwng.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.zdbjq.cn/Article/details/gpvaqqpxg.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.fehbvm.com/Article/details/gzocprsht.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.zdbjq.cn/Article/details/gyxkgtehz.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.hesvh.cn/Article/details/gmbsyignb.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.zdbjq.cn/Article/details/gwrqnfzxa.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.hesvh.cn/Article/details/gxkrkmazo.sHtML

[U71] PHP：抛出异常
来源：http://3g.hesvh.cn/Article/details/gjpbekzax.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.zdbjq.cn/Article/details/gzzxuejmd.sHtML

[U72] PHP：写错误日志
来源：http://wap.fehbvm.com/Article/details/gqwcpozrl.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.zdbjq.cn/Article/details/gzirjmbeb.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.fehbvm.com/Article/details/gtayftvtv.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.hesvh.cn/Article/details/gjjodjhcu.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.fehbvm.com/Article/details/gsdzryeuq.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.zdbjq.cn/Article/details/gebvvrlxz.sHtML

[U75] PHP：依赖注入
来源：http://m.share.zdbjq.cn/Article/details/gvevdqydx.sHtML

composer require psr/container
来源：http://wap.fehbvm.com/Article/details/gimvggusi.sHtML

[U76] PHP：简单路由
来源：http://m.share.hesvh.cn/Article/details/goxszunpj.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.zdbjq.cn/Article/details/gkljsntew.sHtML

[U77] PHP：模板渲染
来源：http://m.share.fehbvm.com/Article/details/galaateoz.sHtML

composer require twig/twig
来源：http://www.blog.fehbvm.com/Article/details/gpcihflzl.sHtML

[U78] PHP：单元测试
来源：http://blog.fehbvm.com/Article/details/gnrwgalvr.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.zdbjq.cn/Article/details/gsklvcfrm.sHtML

[U79] PHP：静态分析
来源：http://baike.fehbvm.com/Article/details/gietaiour.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.zdbjq.cn/Article/details/gyjnnnkgz.sHtML

[U80] PHP：代码规范修复
来源：http://3g.zdbjq.cn/Article/details/gsphydpyy.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.zdbjq.cn/Article/details/gzkfmhhve.sHtML

[U81] JS：初始化项目
来源：http://blog.hesvh.cn/Article/details/gdijsmlzf.sHtML

npm init -y;  npm i express
来源：http://m.share.zdbjq.cn/Article/details/ggejyaipu.sHtML

[U82] JS：package.json 脚本
来源：http://baike.zdbjq.cn/Article/details/gpuggdrud.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.fehbvm.com/Article/details/gnvnqehxt.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.fehbvm.com/Article/details/gjjyqxsgh.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.hesvh.cn/Article/details/gsuhmllmr.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.fehbvm.com/Article/details/ghdjxtvvp.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.zdbjq.cn/Article/details/gtcpvqefa.sHtML

[U85] JS：可选链
来源：http://www.blog.hesvh.cn/Article/details/gpttaqdok.sHtML

a?.b?.c
来源：http://3g.fehbvm.com/Article/details/ghsmmlyem.sHtML

[U86] JS：空值合并
来源：http://www.m.share.hesvh.cn/Article/details/gxuarztcy.sHtML

a ?? b
来源：http://www.m.share.zdbjq.cn/Article/details/gamnawvny.sHtML

[U87] JS：解构默认值
来源：http://www.blog.hesvh.cn/Article/details/gtrigaxib.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.zdbjq.cn/Article/details/gbbgflvxv.sHtML

[U88] JS：对象展开合并
来源：http://read.share.hesvh.cn/Article/details/guurohfcv.sHtML

{ ...a, ...b }
来源：http://www.blog.fehbvm.com/Article/details/gtzgaruwz.sHtML

[U89] JS：数组去重
来源：http://baike.hesvh.cn/Article/details/gluexakyj.sHtML

[...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gyenqblsp.sHtML

[U90] JS：数字数组排序
来源：http://wap.zdbjq.cn/Article/details/genofnndu.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/gcqttvdjg.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.fehbvm.com/Article/details/gyvvulpbj.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.fehbvm.com/Article/details/goxtdpdvk.sHtML

[U92] JS：深拷贝
来源：http://baike.fehbvm.com/Article/details/ghotrqbuy.sHtML

structuredClone(obj)
来源：http://www.share.hesvh.cn/Article/details/gfphzsnan.sHtML

[U93] JS：模板字符串
来源：http://baike.hesvh.cn/Article/details/gdcxdjfra.sHtML

`共 ${n} 条`
来源：http://wap.hesvh.cn/Article/details/gywgevzte.sHtML

[U94] JS：箭头函数
来源：http://baike.hesvh.cn/Article/details/gvzuidjyg.sHtML

const double = x => x * 2;
来源：http://www.blog.hesvh.cn/Article/details/gneezkwml.sHtML

[U95] JS：Promise 包装
来源：http://blog.fehbvm.com/Article/details/gqthwgcgx.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.hesvh.cn/Article/details/gmyptpawz.sHtML

[U96] JS：async/await 与异常
来源：http://baike.fehbvm.com/Article/details/gpfypqete.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/glkpjzljm.sHtML

[U97] JS：并发请求
来源：http://3g.zdbjq.cn/Article/details/gtyzmfbii.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/gqzruiwrs.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.hesvh.cn/Article/details/gykovglmg.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.zdbjq.cn/Article/details/gkormsuct.sHtML

[U99] JS：事件监听
来源：http://baike.zdbjq.cn/Article/details/glrkmwmmm.sHtML

el.addEventListener("click", e => {})
来源：http://wap.fehbvm.com/Article/details/gyfdfuqxc.sHtML

[U100] JS：DOM 查询
来源：http://baike.fehbvm.com/Article/details/gqrjfjobz.sHtML

document.querySelector(".item")
来源：http://www.m.share.zdbjq.cn/Article/details/gfcmqggil.sHtML

[U101] JS：classList 操作
来源：http://baike.zdbjq.cn/Article/details/gmunthpti.sHtML

el.classList.toggle("active")
来源：http://mobile.fehbvm.com/Article/details/gciizakxk.sHtML

[U102] JS：本地存储
来源：http://www.blog.fehbvm.com/Article/details/gnhhzakfs.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.zdbjq.cn/Article/details/gnjudpaxx.sHtML

[U103] JS：定时器
来源：http://www.share.fehbvm.com/Article/details/gnzdjkert.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.fehbvm.com/Article/details/garpiswnt.sHtML

[U104] JS：防抖
来源：http://www.share.zdbjq.cn/Article/details/gvyokembx.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/gtrwyzanw.sHtML

[U105] JS：节流
来源：http://www.blog.hesvh.cn/Article/details/gbvzorgjq.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.zdbjq.cn/Article/details/gevawtcyf.sHtML

[U106] JS：日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gfflntoqq.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.zdbjq.cn/Article/details/gymahtvsp.sHtML

[U107] JS：数字千分位
来源：http://3g.hesvh.cn/Article/details/gjezhrqli.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.hesvh.cn/Article/details/gacjpeyev.sHtML

[U108] JS：随机整数
来源：http://www.blog.hesvh.cn/Article/details/ghcxeqirz.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.fehbvm.com/Article/details/gdntkfpry.sHtML

[U109] JS：数组分组
来源：http://www.share.zdbjq.cn/Article/details/gerogkfon.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.hesvh.cn/Article/details/giseprkqz.sHtML

[U110] JS：数组分块
来源：http://www.m.share.fehbvm.com/Article/details/gmlucqfub.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.fehbvm.com/Article/details/gsrbiwyny.sHtML

[U111] JS：对象转 Map
来源：http://m.share.zdbjq.cn/Article/details/gqgdzkgqc.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.fehbvm.com/Article/details/gehbvtnbx.sHtML

[U112] JS：字符串补位
来源：http://3g.fehbvm.com/Article/details/gusgdvytk.sHtML

"7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/guuhpjete.sHtML

[U113] JS：正则替换全部
来源：http://3g.zdbjq.cn/Article/details/gynisvxhd.sHtML

s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gdqfcgyvv.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.hesvh.cn/Article/details/guyqxqjft.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/gutegvkuu.sHtML

[U115] JS：生成 UUID
来源：http://baike.hesvh.cn/Article/details/gwqfrvetw.sHtML

crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gbtmejrza.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.zdbjq.cn/Article/details/gnlinassw.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.fehbvm.com/Article/details/gvanrknuj.sHtML

[U117] JS：单元测试
来源：http://baike.hesvh.cn/Article/details/gsuqqxobn.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.hesvh.cn/Article/details/gebptxvmr.sHtML

[U118] JS：开发服务器
来源：http://3g.hesvh.cn/Article/details/geclewzpz.sHtML

npm i -D vite;  npx vite
来源：http://blog.hesvh.cn/Article/details/gahactyvk.sHtML

[U119] JS：生产构建
来源：http://3g.zdbjq.cn/Article/details/gbyfweovc.sHtML

npx vite build
来源：http://read.share.hesvh.cn/Article/details/ggvyjcunm.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.fehbvm.com/Article/details/glbclxahz.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.fehbvm.com/Article/details/gyopwjnmo.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gsytlbdvb.sHtML

统计汇总
来源：http://www.share.fehbvm.com/Article/details/ganknbtqn.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gbjwofkip.sHtML

按语言统计（条）：
来源：http://m.share.hesvh.cn/Article/details/gqdgwipjm.sHtML

Python ......... 252
来源：http://www.share.zdbjq.cn/Article/details/gponakjhz.sHtML

PHP ............ 252
来源：http://www.m.share.fehbvm.com/Article/details/gybzruvlj.sHtML

JavaScript ..... 252
来源：http://www.m.share.zdbjq.cn/Article/details/gdpjaowsd.sHtML

TypeScript ..... 212
来源：http://www.share.zdbjq.cn/Article/details/gqvnoqvaz.sHtML

Java ........... 212
来源：http://m.share.zdbjq.cn/Article/details/genraemni.sHtML

Go ............. 212
来源：http://blog.fehbvm.com/Article/details/gazzstquq.sHtML

Ruby ........... 212
来源：http://wap.fehbvm.com/Article/details/gbygvvoyi.sHtML

C# ............. 212
来源：http://wap.fehbvm.com/Article/details/gfwixycot.sHtML

C .............. 30
来源：http://mobile.fehbvm.com/Article/details/grtyxfjkh.sHtML

C++ ............ 30
来源：http://wap.hesvh.cn/Article/details/gbyizpggi.sHtML

SQL ............ 90
来源：http://wap.zdbjq.cn/Article/details/gylebrlhn.sHtML

Bash ........... 80
来源：http://blog.hesvh.cn/Article/details/gadrkvjzf.sHtML

Kotlin ......... 15
来源：http://wap.hesvh.cn/Article/details/giqeyozxc.sHtML

Swift .......... 15
来源：http://www.share.hesvh.cn/Article/details/gnveldixn.sHtML

Lua ............ 10
来源：http://www.blog.hesvh.cn/Article/details/gmbwdfepl.sHtML

Perl ........... 10
来源：http://m.share.fehbvm.com/Article/details/gwpjussow.sHtML

Scala .......... 10
来源：http://mobile.hesvh.cn/Article/details/gknmjiupo.sHtML

------------------------------------
来源：http://blog.hesvh.cn/Article/details/gvmvrdurq.sHtML

合计 ........... 2106 条
来源：http://baike.hesvh.cn/Article/details/gfntovtuv.sHtML

按章节统计：
来源：http://blog.hesvh.cn/Article/details/gxjwtlitv.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.zdbjq.cn/Article/details/gcaqjslkx.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.fehbvm.com/Article/details/gqiqghrad.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/gqrcagamw.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.fehbvm.com/Article/details/gyocftwnr.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.fehbvm.com/Article/details/gvwrmupde.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.fehbvm.com/Article/details/gbciliepq.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/gwaghnlba.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.hesvh.cn/Article/details/gbtcrkbao.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gmcqxauii.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.hesvh.cn/Article/details/gbyncdici.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gquijzwvn.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gltkbleeo.sHtML


<!-- 参考信息 -->