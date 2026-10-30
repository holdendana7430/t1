代发 wailian999

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.hesvh.cn/Article/details/gvvbmamio.sHtML

[T51] Scala：Hello World
来源：http://wap.fehbvm.com/Article/details/gruegmrpz.sHtML

println("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gdcjiehhm.sHtML

[T52] Scala：变量
来源：http://mobile.fehbvm.com/Article/details/gwektsblt.sHtML

val a = 1;  var b = 2
来源：http://wap.fehbvm.com/Article/details/gxeukfhpw.sHtML

[T53] Scala：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gyizuzswm.sHtML

s"值: $b"
来源：http://blog.hesvh.cn/Article/details/gtoskfzpg.sHtML

[T54] Scala：集合映射
来源：http://blog.fehbvm.com/Article/details/gkejhpgnt.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.zdbjq.cn/Article/details/gyciucshy.sHtML

[T55] Scala：集合过滤
来源：http://mobile.fehbvm.com/Article/details/guataucwt.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.hesvh.cn/Article/details/gckkkbwyg.sHtML

[T56] Scala：样例类
来源：http://3g.hesvh.cn/Article/details/gadvvplos.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.fehbvm.com/Article/details/gcbroyifa.sHtML

[T57] Scala：模式匹配
来源：http://wap.fehbvm.com/Article/details/gwwkbsdgf.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.zdbjq.cn/Article/details/grpbvbnhu.sHtML

[T58] Scala：函数定义
来源：http://baike.zdbjq.cn/Article/details/gxfshprat.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.zdbjq.cn/Article/details/gqcbilwyy.sHtML

[T59] Scala：循环
来源：http://www.share.hesvh.cn/Article/details/gsgzscfwb.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.fehbvm.com/Article/details/gogncvcon.sHtML

[T60] Scala：折叠
来源：http://baike.fehbvm.com/Article/details/gxxkoteha.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.zdbjq.cn/Article/details/grzogocua.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ghrqidykn.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.hesvh.cn/Article/details/gezcffubv.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gfyjcrgti.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.fehbvm.com/Article/details/gxmigxwty.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.zdbjq.cn/Article/details/gnyeoducu.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.fehbvm.com/Article/details/gdhoiohjv.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.hesvh.cn/Article/details/gznvcbmks.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.hesvh.cn/Article/details/gtanuxwsb.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.zdbjq.cn/Article/details/gboyujhir.sHtML

[U04] Py：变量调试打印
来源：http://baike.hesvh.cn/Article/details/geudteobu.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.fehbvm.com/Article/details/glpkddndq.sHtML

[U05] Py：列表去重且保序
来源：http://blog.fehbvm.com/Article/details/gomtortfw.sHtML

list(dict.fromkeys(arr))
来源：http://3g.zdbjq.cn/Article/details/gxyyuuyhu.sHtML

[U06] Py：合并两个字典
来源：http://www.share.zdbjq.cn/Article/details/gdegboioc.sHtML

{**a, **b}
来源：http://mobile.fehbvm.com/Article/details/gthelttwg.sHtML

[U07] Py：反转字典键值
来源：http://blog.zdbjq.cn/Article/details/gzydebopm.sHtML

{v: k for k, v in d.items()}
来源：http://wap.zdbjq.cn/Article/details/gqymiyxtz.sHtML

[U08] Py：展平二维列表
来源：http://baike.hesvh.cn/Article/details/gqwwauuqa.sHtML

[y for x in nested for y in x]
来源：http://read.share.zdbjq.cn/Article/details/gcwvpptar.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.zdbjq.cn/Article/details/gexeaprhz.sHtML

max(d, key=d.get)
来源：http://wap.hesvh.cn/Article/details/gnylldpke.sHtML

[U10] Py：按值排序字典
来源：http://blog.hesvh.cn/Article/details/gjracxeez.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.zdbjq.cn/Article/details/glesvoozu.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.fehbvm.com/Article/details/gokrlaftp.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.fehbvm.com/Article/details/gsfcbswrt.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.zdbjq.cn/Article/details/giubphfsq.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.hesvh.cn/Article/details/gyhogmvtc.sHtML

[U13] Py：固定长度队列
来源：http://baike.zdbjq.cn/Article/details/gqrnmvlxq.sHtML

deque(maxlen=10)
来源：http://3g.zdbjq.cn/Article/details/gmffpqepr.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.fehbvm.com/Article/details/gbuwdszxo.sHtML

defaultdict(list)
来源：http://3g.fehbvm.com/Article/details/gzquambuj.sHtML

[U15] Py：高精度计时
来源：http://3g.fehbvm.com/Article/details/gzxbfltxe.sHtML

t = time.perf_counter()
来源：http://www.m.share.zdbjq.cn/Article/details/gjniiuwnc.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.zdbjq.cn/Article/details/gdtucjtce.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fehbvm.com/Article/details/gubvwgjpo.sHtML

[U17] Py：初始化日志
来源：http://blog.zdbjq.cn/Article/details/gachghwme.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.hesvh.cn/Article/details/gglcgqlwe.sHtML

[U18] Py：预编译正则
来源：http://baike.zdbjq.cn/Article/details/gnahpkhik.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.hesvh.cn/Article/details/gvolbwdwo.sHtML

[U19] Py：正则替换带回调
来源：http://blog.zdbjq.cn/Article/details/gujjwkttp.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.zdbjq.cn/Article/details/gwzmwojez.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.hesvh.cn/Article/details/gbjrqbukk.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.fehbvm.com/Article/details/gfypvfkpf.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.fehbvm.com/Article/details/gbvxhgxxd.sHtML

@contextlib.contextmanager
来源：http://m.share.zdbjq.cn/Article/details/gkwcvtopa.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.zdbjq.cn/Article/details/gtvijvayy.sHtML

list(zip(*m))
来源：http://blog.fehbvm.com/Article/details/gsfncdivi.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.zdbjq.cn/Article/details/gpbcihgdn.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.zdbjq.cn/Article/details/groppngrq.sHtML

[U24] Py：路径操作
来源：http://m.share.zdbjq.cn/Article/details/gbdhhuamq.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.fehbvm.com/Article/details/gjygjwjqn.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.zdbjq.cn/Article/details/glvaxciji.sHtML

csv.DictReader(f)
来源：http://m.share.zdbjq.cn/Article/details/gmudfvbgu.sHtML

[U26] Py：并发下载
来源：http://wap.zdbjq.cn/Article/details/gnaqgxhzs.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.zdbjq.cn/Article/details/gkbrlxxht.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.fehbvm.com/Article/details/gcnssufid.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.fehbvm.com/Article/details/gfcelorrp.sHtML

[U28] Py：类型别名
来源：http://www.share.fehbvm.com/Article/details/gmctasnoa.sHtML

UserId = int
来源：http://www.blog.fehbvm.com/Article/details/gwkajfxys.sHtML

[U29] Py：属性校验
来源：http://read.share.hesvh.cn/Article/details/gqzjdrobg.sHtML

@property 与 @x.setter 配合
来源：http://read.share.zdbjq.cn/Article/details/goklxmtsj.sHtML

[U30] Py：数据类
来源：http://read.share.fehbvm.com/Article/details/gogaqzgrx.sHtML

@dataclass(slots=True)
来源：http://mobile.hesvh.cn/Article/details/gutyiaayt.sHtML

[U31] Py：单测
来源：http://baike.fehbvm.com/Article/details/gtjfcaxgf.sHtML

python -m pytest -q
来源：http://m.share.fehbvm.com/Article/details/gexlauhze.sHtML

[U32] Py：代码格式化
来源：http://baike.hesvh.cn/Article/details/gsnztnvgl.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.zdbjq.cn/Article/details/gpthshcfw.sHtML

[U33] Py：打包发布
来源：http://www.m.share.fehbvm.com/Article/details/gnwetuoch.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.hesvh.cn/Article/details/gkgqpyyog.sHtML

[U34] Py：判断编码
来源：http://www.share.hesvh.cn/Article/details/grscjsfjl.sHtML

chardet.detect(raw)
来源：http://baike.zdbjq.cn/Article/details/gfqplepls.sHtML

[U35] Py：发送邮件
来源：http://mobile.zdbjq.cn/Article/details/gjmuhcaxm.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.fehbvm.com/Article/details/gnsezrrwg.sHtML

[U36] Py：定时任务
来源：http://blog.fehbvm.com/Article/details/goqmyrwhy.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.fehbvm.com/Article/details/gtnhhslnx.sHtML

[U37] Py：读写 Excel
来源：http://blog.fehbvm.com/Article/details/gcqmxqtet.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.fehbvm.com/Article/details/gvptldpbc.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.fehbvm.com/Article/details/garufomry.sHtML

Path(__file__).resolve().parent
来源：http://wap.zdbjq.cn/Article/details/grrhwqqxu.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.hesvh.cn/Article/details/gqgkrwzjz.sHtML

sys.stdout.isatty()
来源：http://m.share.hesvh.cn/Article/details/gtsrvlsol.sHtML

[U40] Py：打印到标准错误
来源：http://baike.fehbvm.com/Article/details/gtyprarpv.sHtML

print("err", file=sys.stderr)
来源：http://m.share.fehbvm.com/Article/details/gpxvxfyrh.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.fehbvm.com/Article/details/godsgebkj.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.fehbvm.com/Article/details/gpziojpny.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.fehbvm.com/Article/details/gdztjdfah.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.fehbvm.com/Article/details/gmysdsgey.sHtML

[U43] PHP：声明命名空间
来源：http://wap.fehbvm.com/Article/details/ghqqszlps.sHtML

namespace App\Http;
来源：http://mobile.fehbvm.com/Article/details/ghwtfulne.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.fehbvm.com/Article/details/grpvaotwn.sHtML

declare(strict_types=1);
来源：http://wap.fehbvm.com/Article/details/gqzyetzsn.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.hesvh.cn/Article/details/gwfpjklfm.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gqsytdjkt.sHtML

[U46] PHP：可空类型
来源：http://read.share.zdbjq.cn/Article/details/gthzrlxlw.sHtML

?string $name = null
来源：http://www.share.hesvh.cn/Article/details/goxjjskuw.sHtML

[U47] PHP：联合类型
来源：http://baike.zdbjq.cn/Article/details/grdbaxjyw.sHtML

int|string $id
来源：http://3g.fehbvm.com/Article/details/gqjcoysnp.sHtML

[U48] PHP：纯枚举
来源：http://blog.zdbjq.cn/Article/details/ggfazambl.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.fehbvm.com/Article/details/gvbfpugip.sHtML

[U49] PHP：只读属性
来源：http://blog.fehbvm.com/Article/details/gkrikrhhn.sHtML

public readonly string $name
来源：http://m.share.fehbvm.com/Article/details/glmaygqlv.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.hesvh.cn/Article/details/gsbgezbor.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.fehbvm.com/Article/details/goiroxebk.sHtML

[U51] PHP：数组解构
来源：http://www.share.fehbvm.com/Article/details/gbpgqulvf.sHtML

[$a, $b] = $arr;
来源：http://3g.hesvh.cn/Article/details/grplcbune.sHtML

[U52] PHP：箭头函数
来源：http://read.share.hesvh.cn/Article/details/giplkzppl.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.fehbvm.com/Article/details/gfgtlewko.sHtML

[U53] PHP：空合并运算符
来源：http://wap.hesvh.cn/Article/details/gwhrdrbnl.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.fehbvm.com/Article/details/gsxmnznhi.sHtML

[U54] PHP：空安全调用
来源：http://m.share.fehbvm.com/Article/details/gkoiirskc.sHtML

$obj?->method()
来源：http://www.blog.zdbjq.cn/Article/details/glkpowufz.sHtML

[U55] PHP：match 表达式
来源：http://wap.hesvh.cn/Article/details/grjjzbiez.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.fehbvm.com/Article/details/gxmukmszc.sHtML

[U56] PHP：命名参数
来源：http://baike.fehbvm.com/Article/details/gxoanptzu.sHtML

f(a: 1, b: 2)
来源：http://blog.zdbjq.cn/Article/details/gwmgcpbwg.sHtML

[U57] PHP：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gpeuzietq.sHtML

"值: {$a}"
来源：http://www.share.zdbjq.cn/Article/details/gqfzqtyvj.sHtML

[U58] PHP：数组三件套
来源：http://read.share.zdbjq.cn/Article/details/gpkeqzuma.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gwmjfuafn.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.hesvh.cn/Article/details/glgmgdotc.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.hesvh.cn/Article/details/grkvgvcfm.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.hesvh.cn/Article/details/gpcgtiwvg.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.zdbjq.cn/Article/details/gpaeugvdf.sHtML

[U61] PHP：正则
来源：http://www.share.fehbvm.com/Article/details/gqktiduwc.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gwkvwhetc.sHtML

[U62] PHP：日期对象
来源：http://3g.fehbvm.com/Article/details/gutcvwmxg.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.fehbvm.com/Article/details/ggjztyuuu.sHtML

[U63] PHP：文件读写
来源：http://www.blog.fehbvm.com/Article/details/goasahmdh.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.zdbjq.cn/Article/details/gkjmrxapi.sHtML

[U64] PHP：目录遍历
来源：http://mobile.hesvh.cn/Article/details/guyndkgto.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.hesvh.cn/Article/details/gxdmbuxww.sHtML

[U65] PHP：会话
来源：http://baike.hesvh.cn/Article/details/glzgphnuk.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gsmcjmsss.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.hesvh.cn/Article/details/gxaezezqp.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.zdbjq.cn/Article/details/gkkvhrylr.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.hesvh.cn/Article/details/gqpotlpfy.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.fehbvm.com/Article/details/gjcfdthvu.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.hesvh.cn/Article/details/grxaznasl.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.fehbvm.com/Article/details/ghzhimcje.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.fehbvm.com/Article/details/gmiatugps.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.fehbvm.com/Article/details/gdbapwmhz.sHtML

[U70] PHP：PDO 事务
来源：http://baike.hesvh.cn/Article/details/gjgyxurep.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.fehbvm.com/Article/details/ggavndzyi.sHtML

[U71] PHP：抛出异常
来源：http://read.share.hesvh.cn/Article/details/gksnyziuu.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.hesvh.cn/Article/details/gcqjckako.sHtML

[U72] PHP：写错误日志
来源：http://baike.fehbvm.com/Article/details/gibxckcgz.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.fehbvm.com/Article/details/gkaugljth.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.hesvh.cn/Article/details/gzlybtygm.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.zdbjq.cn/Article/details/gbinlmdca.sHtML

[U74] PHP：读取环境变量
来源：http://wap.zdbjq.cn/Article/details/gmsiefuhs.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.fehbvm.com/Article/details/ggksyqgwa.sHtML

[U75] PHP：依赖注入
来源：http://read.share.hesvh.cn/Article/details/gurkkqbve.sHtML

composer require psr/container
来源：http://baike.hesvh.cn/Article/details/gzltvebfp.sHtML

[U76] PHP：简单路由
来源：http://blog.hesvh.cn/Article/details/gkyimijww.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.hesvh.cn/Article/details/gzfsoalef.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.zdbjq.cn/Article/details/gicyxgelz.sHtML

composer require twig/twig
来源：http://www.m.share.hesvh.cn/Article/details/gtuyukzdb.sHtML

[U78] PHP：单元测试
来源：http://www.share.fehbvm.com/Article/details/gfjglktmb.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.hesvh.cn/Article/details/gqqqlnzho.sHtML

[U79] PHP：静态分析
来源：http://mobile.zdbjq.cn/Article/details/gjwnfkvbl.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.zdbjq.cn/Article/details/grhhgmeid.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.hesvh.cn/Article/details/ggiqryykz.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.fehbvm.com/Article/details/grkbopwzp.sHtML

[U81] JS：初始化项目
来源：http://mobile.fehbvm.com/Article/details/gmexwkoed.sHtML

npm init -y;  npm i express
来源：http://www.blog.zdbjq.cn/Article/details/gderpjhlz.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.zdbjq.cn/Article/details/gedtddtqr.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.hesvh.cn/Article/details/gyodevraw.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.fehbvm.com/Article/details/ghhokvnvc.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.zdbjq.cn/Article/details/gewoubfrq.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.hesvh.cn/Article/details/galuqrwtu.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.hesvh.cn/Article/details/gaqsjspgf.sHtML

[U85] JS：可选链
来源：http://mobile.fehbvm.com/Article/details/ghcvemrwo.sHtML

a?.b?.c
来源：http://m.share.zdbjq.cn/Article/details/gpjeluodx.sHtML

[U86] JS：空值合并
来源：http://www.m.share.zdbjq.cn/Article/details/gwbnzsmlm.sHtML

a ?? b
来源：http://m.share.fehbvm.com/Article/details/gdwvvlici.sHtML

[U87] JS：解构默认值
来源：http://3g.zdbjq.cn/Article/details/ghcpqsjoi.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.hesvh.cn/Article/details/gtbgfsoga.sHtML

[U88] JS：对象展开合并
来源：http://baike.hesvh.cn/Article/details/gjzodhdwv.sHtML

{ ...a, ...b }
来源：http://www.share.zdbjq.cn/Article/details/gbukgkxiw.sHtML

[U89] JS：数组去重
来源：http://www.m.share.zdbjq.cn/Article/details/gxtqtcgvf.sHtML

[...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gjfwkkwfz.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.zdbjq.cn/Article/details/gecfvxjtl.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/gnakibipu.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.fehbvm.com/Article/details/glrewdcvq.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.hesvh.cn/Article/details/guackfbob.sHtML

[U92] JS：深拷贝
来源：http://3g.hesvh.cn/Article/details/gookaazfe.sHtML

structuredClone(obj)
来源：http://m.share.hesvh.cn/Article/details/gfmansjsu.sHtML

[U93] JS：模板字符串
来源：http://read.share.zdbjq.cn/Article/details/gwgukvkkx.sHtML

`共 ${n} 条`
来源：http://www.m.share.fehbvm.com/Article/details/gakaeybyc.sHtML

[U94] JS：箭头函数
来源：http://read.share.hesvh.cn/Article/details/gknuhkwtm.sHtML

const double = x => x * 2;
来源：http://www.blog.zdbjq.cn/Article/details/grnaaeubj.sHtML

[U95] JS：Promise 包装
来源：http://m.share.hesvh.cn/Article/details/gbdapazde.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.zdbjq.cn/Article/details/gmsobflyj.sHtML

[U96] JS：async/await 与异常
来源：http://blog.hesvh.cn/Article/details/gfhqkltcu.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/gimdzzmet.sHtML

[U97] JS：并发请求
来源：http://mobile.hesvh.cn/Article/details/garldrevf.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/grhnmpoep.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.hesvh.cn/Article/details/goqptinio.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.hesvh.cn/Article/details/gjtiylnne.sHtML

[U99] JS：事件监听
来源：http://baike.zdbjq.cn/Article/details/gseueieku.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.zdbjq.cn/Article/details/gwlefsdih.sHtML

[U100] JS：DOM 查询
来源：http://www.share.hesvh.cn/Article/details/gbuqitbyg.sHtML

document.querySelector(".item")
来源：http://read.share.hesvh.cn/Article/details/gtctruwda.sHtML

[U101] JS：classList 操作
来源：http://www.blog.zdbjq.cn/Article/details/giwrkhrdp.sHtML

el.classList.toggle("active")
来源：http://mobile.fehbvm.com/Article/details/gurvmhkok.sHtML

[U102] JS：本地存储
来源：http://m.share.fehbvm.com/Article/details/gpjorwnxd.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.fehbvm.com/Article/details/goxzssprs.sHtML

[U103] JS：定时器
来源：http://www.share.zdbjq.cn/Article/details/grvgcjcep.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.zdbjq.cn/Article/details/gijgalegt.sHtML

[U104] JS：防抖
来源：http://baike.hesvh.cn/Article/details/garxjpuwv.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/gsszfvjqb.sHtML

[U105] JS：节流
来源：http://www.share.fehbvm.com/Article/details/gabdqxxqo.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.fehbvm.com/Article/details/gagivhfuz.sHtML

[U106] JS：日期格式化
来源：http://blog.zdbjq.cn/Article/details/gasdsuyxk.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.fehbvm.com/Article/details/gmbbkiiqu.sHtML

[U107] JS：数字千分位
来源：http://www.blog.zdbjq.cn/Article/details/gmragqcrm.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.hesvh.cn/Article/details/gymjadztf.sHtML

[U108] JS：随机整数
来源：http://wap.zdbjq.cn/Article/details/gtlrzgofk.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.zdbjq.cn/Article/details/gxdssudma.sHtML

[U109] JS：数组分组
来源：http://blog.hesvh.cn/Article/details/gepqkifkl.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.hesvh.cn/Article/details/ghwpmtgej.sHtML

[U110] JS：数组分块
来源：http://blog.hesvh.cn/Article/details/gnmutvqio.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.hesvh.cn/Article/details/gjtbxctnu.sHtML

[U111] JS：对象转 Map
来源：http://www.share.fehbvm.com/Article/details/gxiupvwoa.sHtML

new Map(Object.entries(obj))
来源：http://m.share.fehbvm.com/Article/details/ggvplorpr.sHtML

[U112] JS：字符串补位
来源：http://read.share.hesvh.cn/Article/details/gaaedjktg.sHtML

"7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gmxwgmrvr.sHtML

[U113] JS：正则替换全部
来源：http://read.share.zdbjq.cn/Article/details/gzfcnbuwb.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gcbwkwlan.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.fehbvm.com/Article/details/gbmjlihld.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.hesvh.cn/Article/details/ghwxfulro.sHtML

[U115] JS：生成 UUID
来源：http://3g.zdbjq.cn/Article/details/ggyncaszk.sHtML

crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/gfuifoezl.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.zdbjq.cn/Article/details/giwsoznms.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.hesvh.cn/Article/details/gawadiywn.sHtML

[U117] JS：单元测试
来源：http://3g.zdbjq.cn/Article/details/gjbosnqwc.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.hesvh.cn/Article/details/gypoliwug.sHtML

[U118] JS：开发服务器
来源：http://3g.zdbjq.cn/Article/details/grzebmfom.sHtML

npm i -D vite;  npx vite
来源：http://baike.fehbvm.com/Article/details/genowutfl.sHtML

[U119] JS：生产构建
来源：http://www.blog.hesvh.cn/Article/details/gjozqqsso.sHtML

npx vite build
来源：http://baike.fehbvm.com/Article/details/gazecddrt.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.fehbvm.com/Article/details/gngdqgull.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.zdbjq.cn/Article/details/gfrznmgps.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gxbhxejyy.sHtML

统计汇总
来源：http://baike.fehbvm.com/Article/details/gpioyhxrx.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gwrpdhhmg.sHtML

按语言统计（条）：
来源：http://www.blog.zdbjq.cn/Article/details/gnrdhikzm.sHtML

Python ......... 252
来源：http://read.share.hesvh.cn/Article/details/gryyntfrv.sHtML

PHP ............ 252
来源：http://blog.hesvh.cn/Article/details/gkpxteeoq.sHtML

JavaScript ..... 252
来源：http://baike.zdbjq.cn/Article/details/gifobwkpb.sHtML

TypeScript ..... 212
来源：http://www.m.share.fehbvm.com/Article/details/gitikiiyq.sHtML

Java ........... 212
来源：http://www.share.zdbjq.cn/Article/details/givdmtltd.sHtML

Go ............. 212
来源：http://www.share.zdbjq.cn/Article/details/glgjdklef.sHtML

Ruby ........... 212
来源：http://3g.fehbvm.com/Article/details/gzmabvumu.sHtML

C# ............. 212
来源：http://read.share.hesvh.cn/Article/details/gdkimluqy.sHtML

C .............. 30
来源：http://baike.zdbjq.cn/Article/details/gfjamemqw.sHtML

C++ ............ 30
来源：http://3g.zdbjq.cn/Article/details/gwidrfatw.sHtML

SQL ............ 90
来源：http://read.share.zdbjq.cn/Article/details/gldyjudmq.sHtML

Bash ........... 80
来源：http://www.blog.hesvh.cn/Article/details/gxmzmiccc.sHtML

Kotlin ......... 15
来源：http://read.share.hesvh.cn/Article/details/gddfjrjec.sHtML

Swift .......... 15
来源：http://read.share.hesvh.cn/Article/details/gzuodirjx.sHtML

Lua ............ 10
来源：http://wap.hesvh.cn/Article/details/gdzftufod.sHtML

Perl ........... 10
来源：http://www.blog.fehbvm.com/Article/details/gcnwbqqzy.sHtML

Scala .......... 10
来源：http://mobile.fehbvm.com/Article/details/ggfqqejfc.sHtML

------------------------------------
来源：http://baike.fehbvm.com/Article/details/gdhsbdtxn.sHtML

合计 ........... 2106 条
来源：http://wap.fehbvm.com/Article/details/goocpapls.sHtML

按章节统计：
来源：http://3g.zdbjq.cn/Article/details/gytbazrzb.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.zdbjq.cn/Article/details/ggyalcchr.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.hesvh.cn/Article/details/geflahths.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.hesvh.cn/Article/details/gmnptkfet.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.hesvh.cn/Article/details/goxevxifc.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.zdbjq.cn/Article/details/gghahgcan.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.zdbjq.cn/Article/details/gtxdsymkm.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.zdbjq.cn/Article/details/giwqelvnu.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.zdbjq.cn/Article/details/gvjpoolcn.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gstommjgz.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.hesvh.cn/Article/details/gleaqfdop.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/grbdyokto.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/guwlocbyt.sHtML


<!-- 参考信息 -->