代发 wailian999

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3qlkauwri.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3fnplgkza.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3xcvjrchd.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3tycqvycc.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3iwlfoney.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3tnikmmlg.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3iboksjek.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3macdsefa.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3fevuvshd.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3nvhxcgli.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3ixojtihr.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3hbeujioy.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3jlmaqtnz.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3dinthxjr.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3nniosolx.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3lgadjylf.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3jggsgnyf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pmnlgmnp.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3bjbjlnbq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qajicmbs.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3saqckgtp.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3gzzhfzwd.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3edgzhugl.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3ldewschb.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3ymsmeuxu.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3yessulhq.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3wwzfhwkn.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3guelstrz.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3scknvfvl.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3ztymscve.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3hvmbujeu.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3jfmdvweh.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3wwsldxkf.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3oriujhha.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3oqgghjcf.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3bwwhfbhm.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3ydhtpyvf.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3uelnskyr.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3qktjtmtf.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3bjakxpjl.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ckkmjmni.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3bsdwypxf.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3ghxqllfc.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3xaymdewp.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3qgvehyhj.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3rkcvsoxa.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3jezoydkl.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3alxqfhza.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3zzzeritn.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3bmtxaryt.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3skmjtlsu.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3beyyhsuk.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3iukqrfqg.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3yaqqhutf.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3iudmgolq.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3djeefqdc.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3lddymwib.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3gsnfzvmz.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3simphaou.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3xuehcwde.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3xjhkoyvw.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3vfgzjejw.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3kunufywr.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3mzjneahf.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3jbhgucyp.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3aymohmsv.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3utdedtkd.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3hbkmcqjy.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3xlxlbvrf.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3yveqjpnc.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3yqypbgob.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3ayirnxoh.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3fsrryjwx.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3omcmyopk.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3ymjocqbs.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3amdkqcco.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3fneeewyv.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3xuriurgs.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3rverfuiu.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3zwuxlqzi.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3iwrjukrg.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3usyfwqnz.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3hkfetoaj.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3tvpgoqnp.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3mjxifeyf.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3jtxgszvu.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3erarmhnz.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3xvvmtlie.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3ofgedxwk.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3cmbzozxz.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3onkplbdr.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3zqdbkoyr.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3eamkzbuy.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3wtfclwig.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3ndelfvcy.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3zuucelzv.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3odohtmpj.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3qxfarlhr.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3prieyvvu.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3fxctiren.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3cboxpqak.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3ocncqkdo.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3yjmmttgf.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3srvyinhb.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3cmybjteg.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3nbtniybh.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3edmmpfaf.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3tzpjqxlh.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3dyaydemv.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3spmfcqqy.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3qiqpbfkb.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3yxphcjgt.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3vdtfqvwv.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3lvazrweu.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3bmcrrjrf.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3mtwrypfc.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3jsjoojii.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3itqoyagb.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3fddqkhrt.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tktjnpab.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3fxhgabsy.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3jyumgggm.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3nvnlirhb.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3tmdxbvjx.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3awigccox.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3ourehzmv.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3djfiuyxq.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3mljoefir.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3skxnxitr.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3ahdzybll.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3fafuybqf.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3gbvcmnmu.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3tjueavwg.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3tnnstvgm.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3jotafdfb.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3zbkzzsdk.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3zvxnzecb.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3mdgbrimx.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3ifcmmkgd.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3wxxuuagg.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3gmdvlthz.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3uijlonmp.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3jkojfxmp.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3nutlrmtm.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3dkpuucwf.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3qlfcneef.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3cfqacply.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3zmodhbzf.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3xymvpxmm.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3uiidhozf.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3ilmsswzv.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3isxuthut.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3brvqdzwg.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3pndxuzbd.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3lweffbxy.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3moluhrmg.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3nnspcfbj.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3jexcmmhj.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3yeryxeoi.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3bccfkpdc.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3mcqgjdod.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3sxpqatmo.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3kivqggrz.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3plehunrp.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3lbothmln.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3njkazfsk.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3sopvagvd.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3ymlvtifl.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3fgigccgw.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3rlqxsnsc.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3wkvjmfgv.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3hbhzytzt.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3dcxmalto.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3qtlsrqxa.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3rnvsmwpd.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3evbemzmx.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3bbymdhgf.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3tpcsmyyz.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3malkfhds.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3egfemlnm.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3cjulpart.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3rsnuxfbs.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3acjimeff.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3rchejldd.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3wxbxvyno.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3lpumklij.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3gbxhhmoc.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3hmpidvsi.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3dbmnqeha.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3ckhbedtp.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3qoubjibk.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3stkxbuhd.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3yfbcqyad.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3dhidsryd.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3qlwxwqfo.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3jepczdke.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3stmivblg.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3aimougyu.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3noeoxfuf.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3pngilbom.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3hyqhiyuk.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3tozqjeon.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3dgwvmkma.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3yetmnhsp.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qertrwbv.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3vgjccbxd.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3uqhiajbb.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3wrxdvrtd.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3qhgixoij.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3fvdcsulq.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3tazedgkk.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3vnzdhbnv.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3mgvogtfw.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3kofyuhcc.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3kafdbkdy.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3lfyiqghi.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3saqanhmy.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3jjukywgn.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3tojuijls.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3eynszunt.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3jbvemqbp.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3osixyiqp.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3vmsdybxs.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3wynbggja.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3tugasamw.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3tehiodkc.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3pezugyde.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3yjnslxio.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3yibukkkz.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3gmlmbylg.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ozxrrkky.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3ujcjljwq.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3wiznvbgl.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3xbbzcqhl.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3wkdmjkak.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3myzkxbet.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3ggpneiwz.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3ietjzdxq.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3okemmsyn.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3knautvxu.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3zmwtetlo.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3inzohpko.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3sknlpcgx.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ebbdrqrd.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3zftaqoqj.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3tjoiadmc.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3gtzrzkmu.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3cjyghokt.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3ydxcuxop.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3hmdltbta.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3zdxodfvm.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3mllblljd.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3wibacxaf.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3xartgmht.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3pmhmjbvn.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3ccebsvlk.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3klylsovr.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3mjfiypcu.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3rhraknib.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3lxxcdtqv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zwcgxklz.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3vmfyeljl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wymtvsds.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3iymwhwyd.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3cvaeojtu.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3wxpbaeho.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3lityxzmw.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3knbiqkjn.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3mjwyrpst.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3eekuthmg.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3tfdebuqg.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3egzuflif.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3jqbbrrqz.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3snwrbqta.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3gehhokwt.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3fhzxjcmk.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3lohpbzct.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3whjhgbyw.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3qcyoiayb.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3inqjgcec.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3jryzemft.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3uxjvvtfq.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3kqsadjpw.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3elwztnvm.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3fxcohqrm.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3zunxdpvj.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3hggtblne.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3panviixr.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3gqdzjqrr.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3kcjjaofn.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3xnydehev.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3etwakhhx.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3dtaisdrj.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3dmutnqpc.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3apwieuze.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3peaxzxou.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3toeqtyyv.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3vzvbzppr.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3hrfgakwf.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3njkpjrky.html


<!-- 参考信息 -->