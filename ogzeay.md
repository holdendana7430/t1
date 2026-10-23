代发 wailian999

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3zcdmurof.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3qzvrqqsd.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3lmidwprh.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3qdbfckbk.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3jqeqiywk.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3allemdri.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3ueldyjun.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3ymjkqgyn.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3lcatxlga.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3uqustqah.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3bzkvyqhu.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3wjmjptgs.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3qxvbyddv.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3djjwqzcg.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3bpokxgzy.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3ubjarzdr.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3qjzgdggt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3svlugezo.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zxlflwto.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3spdyadzw.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3dnyifyjo.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3kmwdiswk.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3wljnrfbv.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3myhaudcl.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3tmvsnvpn.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3yhhgyjrs.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3iqpyeqof.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3aucngyil.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3rrcyeqgx.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3msgzczhs.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3pvfkzumf.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3dwsbrtgf.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3wsekfhzc.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3buwahzct.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3fviohpjb.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3rkbzogpu.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3hqblrnpi.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3rptscqun.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3gbialkdw.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3efdnosxp.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3dmpptzen.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3xgpsjngy.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3mdsgfmvc.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ratuypwe.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3hmfqmqxa.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3glmnrjtk.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3gpmugfaz.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3rukynbvm.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3myufvicv.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3lwpefesq.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3ookpkyux.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3ffkwbcnh.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3iqshzwph.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3wxyiwsrw.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3lfoxdfdf.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3itqcinjw.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3pbkjqjco.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3zrzsvlfx.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3jvwndvob.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3ldrnyift.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3qbkwyktd.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3obyrduhy.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3ogrzcfgl.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3pbsyaipo.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3guytghgg.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3tvveifhp.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3rqdbsnis.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3qhgzgoab.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3iexkimrq.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3rxklpzjt.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3wsriifxl.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3tqdsvgvq.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3xncyxrqm.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3unhhrcwc.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3prklivqs.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3sfxjsrlj.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3lrzjvgcz.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3yetvladz.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3dqrfuoya.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3chvnwyeg.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3zaujbgtn.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3uotohtsn.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3akodvlnw.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3uawltowa.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3ocjegkpq.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3glqfmudf.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3bmypfsfn.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3idoffmeq.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3prluerhg.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3wpnrvujr.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3biyotodz.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3pyugpnwd.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3ftyzxwln.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3cxbesovs.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3kecazpys.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3ymgadpbt.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3zwccgadv.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3hrxjuyxp.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3dkntmzqd.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3iwaknldg.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3fnlmatsa.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3atqajphc.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3fzkzkshy.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3psgvxizb.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3isqucyjj.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3oleafngd.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3atslxlvc.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3nzedgyeh.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3surzifkp.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gdkcshuy.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3xhmrzjum.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3fpurgyge.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3nurfbapt.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3ivsyveyx.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3dkfrikie.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3ywdkcstv.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3kcjspuxv.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3djnlkaid.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3yvoekqpp.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3jwuliibm.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3qtzoxtty.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3bzkhipak.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3sohcupip.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3fnqrillq.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3jteoekdy.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3jjlqnekr.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3ecffjtfk.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3pctvzmtc.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3lphghtxk.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3aiwlxbqz.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3cqsjgiom.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3onmbobec.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3yquwzhax.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3dwtospfu.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3xjnvasug.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xcpsvgxx.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3dpdhnado.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3voizqjck.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3fhicdgeb.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3mjtsbddh.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3ugdkccjv.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3gmkccbax.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3robtzalh.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3dpvpjare.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3ucmlmxds.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3qgiybywu.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3pdxnqfya.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3jzwkbfke.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3amagycmp.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3lshonhyo.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3yhgjzpza.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3jyobtzws.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3kwokqbfe.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3feplimbd.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3hjazlwvn.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3kzwpytfz.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3svscnuvj.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3zyjtwnup.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3zbeelhnl.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3wkqfwkyj.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3npmcfulz.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3byddupfq.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3celbsbzz.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3lohzhsfk.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3qciomwmr.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3vpvczwfp.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3fnsneboz.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3dntbkxro.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3jkgvdzpx.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3uyydbljg.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3qwpuswen.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3ofnoiuzx.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3tkgcxqid.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3obapzdlf.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3laquqhse.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3yzfjnrlo.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3ktlrjfpy.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3nsvdmiyp.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3olbjgfhb.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3xrvggqse.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3uyvrdoip.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3mwkfpozx.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3pdeibync.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3nbjhwqjd.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3cajxwdjg.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3vuneulik.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3uaypbndh.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3htdevtxn.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3iwsooout.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3crnmhxet.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3ezrdtbuc.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3pasqrbjx.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3hweatusm.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3lyunamwh.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3ynsiutao.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3yfamlmno.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3sxghsgrt.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3xmauqpsk.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3jyzgtuas.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3lmetfrlm.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3qdagotjc.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3apvakelk.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3dysbmvha.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ynsriagg.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3roaaocfe.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3iebtnjrr.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3wumkiptk.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3qflqsege.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3kziywoee.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3azzzfque.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3aqcxnqku.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3wbenapjx.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3trnsdgqp.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3dmnuoiiq.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3kmpfhntc.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3wexfqcbs.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3vmvuiirl.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3ezzjkbrw.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3yvvysiar.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3zpkkquwf.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3fbzcypdy.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3dgkddcrm.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3enogncil.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3mjwvxvfu.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3iwdouxgn.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3cvbrlief.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3avpnvihk.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3nsayhcgo.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3wulgqkbm.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3wkyziruo.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3hrxwrfid.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3yratxeqw.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3rommyfia.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3gftqmyce.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3shnthwuq.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3pjhwrgzl.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3beliwggo.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3ebbbliio.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3pyacbofq.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3cpdeppsh.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3txvihpca.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3fetbdktm.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3jexuyxbm.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3dsnocbjg.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3omsipxte.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3uzfsxxof.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3vslgygtk.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3szcywwqv.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3ufauzinl.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3zlyqyvjl.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3rzwdsztj.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3cvydhclc.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3eoqafapp.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3rexhdxak.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3riaomxab.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3dtktbuxa.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3saoooemb.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3hrlqblaz.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3jilqdtwb.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3xczqyluy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iqqfxyie.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3teulyyqq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pwelkkfm.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3yytvhaht.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3hrqvgghb.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3pfsclqel.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3hruvpolm.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3riluxakm.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3wzzptxsd.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3xyqghxra.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3koaepjio.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3svveqgck.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3tkburidf.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3zyelndyh.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3scbhbvxf.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3pmethhpc.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3fpdjvjey.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3vucnrqay.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3yofqcxsm.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3pjnqjwxq.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3wfbdivet.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3pukzxosl.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3thwksvyz.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3oybsdiah.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3axawmzqa.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3auayackk.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3olpdtopn.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3ygitnhwt.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3lsfxbekx.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3ihlwpbwa.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3diyzvlsl.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3mhucdtme.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3cxvghnja.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3pczheftj.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3asgzlujg.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3zerskhkd.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3tvwjryip.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3vzdlcbpm.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3cefrlsdp.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3acpqhszi.html


<!-- 参考信息 -->