代发 wailian999

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3apnyuyxb.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3soklddnb.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3sodphgqg.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3xwipkxnu.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3hqrygela.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3xlqcnajn.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3ytppggyz.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3kpvjhfrt.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qlkrjswe.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3kwzjfngz.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3lqjzssoh.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3mxgovlan.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3piixvwpz.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3wjzzvryo.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3scplhmjj.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3rbrwenge.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3gnpvoteo.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3duqypwta.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3vzyesywd.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3bfwruyls.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3xbttimkr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xahaljgm.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wcyoyktq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oyzafxkt.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3djhsnoom.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3bcbxvzkn.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3htpcsppf.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xemqmxnt.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3zxspreio.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3fhqrptph.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3lvsmxpbs.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3vxcifqbc.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3fmlgnpiw.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3wdtlfpdd.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3vxdonvhs.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3dpnvmivr.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3ibqtdsue.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3ttdvpwak.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3snqxdjul.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3rcooxbnj.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3fefgyvkw.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3rdzoaftt.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3wwffzhcv.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3ykeyocjl.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3wkeqfjqt.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yedwbxee.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3znbhpotf.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3waoxqjlf.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3vrkzmade.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3adffnxtk.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3wcsdiqck.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3ffudtuws.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3xpvitubz.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3isggwkwb.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3fsweuiyr.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3hcxrcgef.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3iuxhpvro.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3sovmhspg.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3vbfotouk.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3mflmpesd.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3awbhpqft.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3scsoscuq.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3sgoucntk.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3zhaivpcr.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3ldxfhndv.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3yozudlwx.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3iucljbwh.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3epeiuugo.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3dptlauza.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3ovdwridk.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3gqnpktlm.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3dhhllwah.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3kptwcdrx.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3candvtpo.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3hrctluzo.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3apwsatae.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3asdfphbz.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3umyawris.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3szgmcyvm.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3pftlanfd.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3kedslfvx.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3jedijfqi.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3nppsrdbd.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3djqrzoiw.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3mmmhhqga.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3stjbamll.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3izlzxomj.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3pvmnyyys.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3rvovlrwd.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3oftycknh.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3kmbplcww.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3gmgockdn.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3giajyzdj.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3jzpoljuo.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3rlcizytg.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3uquuyibi.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3lawbotfa.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3uzemattm.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3iwhgwnto.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3rwwnpmya.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3tnrwbojr.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3fhobkyda.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3ipqmfais.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3nhgagncu.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3jfwcnsay.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3geuskekb.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3fsgvdqmv.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3pspykgiq.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3jqmegvuo.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3ckralxqa.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3ouxeeazs.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3ucyxyndi.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3ctbycvij.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vzsafgil.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3ppdzlzlk.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3chlujtms.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3tfytvalf.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3yejayevx.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3hsnyzyhl.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ibdqqvld.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3jcatmwbj.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3okvatnpl.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3euclsegf.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xiizyhsc.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3mgqyqysy.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3bmzrrxia.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3ssxxhneu.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3faojzzjs.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3vyhtwehs.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3jddirdbj.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3fxateerf.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3rghwtiya.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ratwxxay.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3atliwndi.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3gakkgtzz.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pmbazdlw.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3lkbcwwkm.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3ikeqpnkb.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3zzmzpyat.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3brkxxlmg.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3baabetzo.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3yxyegvye.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3ptrqmoes.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ajwjllft.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3txxyqqhw.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3lrczgtch.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3rpagryep.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3jqjlnooo.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3cvjdkovf.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3ouwajkpu.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3fjshpzra.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3jdeeaaoj.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3smubjxtn.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3adamhppw.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3wyceeqgh.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3dwwescrc.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3vpxebuju.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3krjtqhca.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3utmfasqj.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3krpujjab.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3awfqcqpi.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3wksqzdjx.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3kvelnhty.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3lqrrpwam.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3xrvowesn.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3iitcxqka.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3pmvkahje.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3ctygxujk.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3lgkmqodb.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3pqodibki.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3shklozbw.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3siqikifs.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3dzswlfcm.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3pjrijpwg.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3sdvpwzud.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3dyiixraz.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3qusyvjem.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3rfadfbfx.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3phcyynik.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3tnwoxpqs.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3jhcrjozk.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3kkyrrpks.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3utbnscoo.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3jtvyafie.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3fdxtwnkp.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3joabcyea.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3lkrarvmn.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3msxolwko.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3qaygbtcl.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3rjuigcws.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3flvmatrt.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3uyfomhgj.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3wecblgdu.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3wcbeukwo.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3uujpbpwi.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3wprgmose.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3ctzllzko.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3jzzhwszh.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3clebindx.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3rifpegnp.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3pxbyfxgw.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3iehxzojk.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3cjmoogqd.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3lnwwfxjc.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3yfdysjqv.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3locupfie.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3kuohfymc.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wxyunzps.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3iutpubyx.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3tcvrfxnc.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3otgwglfa.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3kghsyqne.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3tpqyarcs.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3tslrvpie.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3lohzarif.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3avaqcfms.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3augrfgwn.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3wftfpfxz.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3zcaakmmv.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3pbqhocej.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3amgowyjf.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3bhihvnlb.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3viimetxq.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3zsebpcie.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3rdxvkhas.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3qovutzkm.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3leeduiqh.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3kldbawfq.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3nrtycmdy.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3uiniaptk.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3iqmtcaev.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3dxexoagi.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3drdfsjfs.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3xmjwarxh.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3fltmfaiq.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3glodeqfg.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3tkuozwyy.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3iocmukcv.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3agdusgfc.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3nielxzhj.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3vsqmhlrf.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3drkzrzyp.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3qgtwlrud.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3igwgvlju.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3kqglcbba.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3yazmamll.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3hembrkch.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3hmzsqjwu.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3ahhgazzx.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xryjxcbv.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3ajpvosqc.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3hmbodzwe.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3kqdrorbo.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3nbvfrqcv.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3zvnpdypl.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ivwfmjql.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3ykrhywtf.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3xbqjktyt.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3jiyvpdoh.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3icwvtlia.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3pafulgcq.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3uywdanbf.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3xqmjplvk.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3gbovlcya.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oipzbgfo.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3kopihqik.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qnqvdsbq.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3yubazqii.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3mgxkjwtz.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3rnzgbomh.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3myawfpif.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3sczrapby.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3tiubgprq.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3ukzzrimj.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3avrpzlya.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3fpuaemei.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3flphvsex.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3ibgzvmzb.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3fluntlnm.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3vlkoddls.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3irysapwu.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3wvqsoxmt.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3psgwaibv.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3tolrhpxp.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3esvvskfk.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3cttjkugn.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3iymerdap.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3inysfaqv.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3rvyanqyl.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3kfknebua.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3xtgewuwd.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3brhljbej.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3fexqljfh.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3cqgviuki.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3zoxhrhuz.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3gdhzfxef.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3fsqblxii.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3evxohbut.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3hoyarrct.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ofvdxpmu.html


<!-- 参考信息 -->