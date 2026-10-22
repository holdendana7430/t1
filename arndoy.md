代发 wailian999

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ntmxzjen.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2fgcdxnha.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2wjgpaqkn.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2tkamdbtj.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2oybqbaxd.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2okgfryld.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2atlwtjdg.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2lsoxhrcv.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2tqtzveyb.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2kxmdtzgt.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2tykdionm.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2jpfitgdm.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2hhbwynwl.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2uktkliwb.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2xyziigcm.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2djadrfvx.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2ofztkcpp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ouzombhr.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ornmllzm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xqajwiit.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2ksbunczv.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2norcaccp.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2kyalhmmy.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2bnyhpsjj.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2xoyiedxf.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2yfclcmbh.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2bigouvkp.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2uunzogiq.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2dycbcshe.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2klpvtlqw.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2zjqimgsk.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2txdfmeee.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2hqcekzli.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2zddiikwd.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2vjbcsnkb.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2gidozcoi.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2pvgoufmo.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2tslzltrh.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2upfqgugg.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2qeyitozy.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2qdiedwka.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2gwxeprii.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2soheifgu.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2xaawlnzn.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2kmlpkyxj.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2qcxxtetz.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2dlxkeyum.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2iizpwlhs.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2azgusufa.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2qmmxhmdv.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2xwpjjbhf.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2blbjxgib.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2mldpigav.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2qsarhjll.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2dmqbaboo.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2dngxgxuo.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2riizjrvl.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2nyyuzgcx.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2idmlbnoa.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2trcacupm.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2xlhzhkpp.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2mpzbnkco.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2kaotqkot.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2pogprfwu.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2vnxjhrtr.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2xvuiscna.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2nfeawjnz.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2samsosjn.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2myhxanxu.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2ldfjdihq.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2qholctuo.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2yfyxambz.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2bqrxblop.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2ikmhjtze.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2bptlheav.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2soiehclp.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2tlxmbaoh.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2gzwwfssi.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2kacinrve.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2roizlcqj.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2wxgflxoj.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2jijzvoyz.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2oibmcxzn.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2lntqohjq.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2afgifutf.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2acvxxixv.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2qwtvmpvg.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2wkyxxqbw.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2anbycbvn.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2wubuvyhk.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2rddcfrsd.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2vtipcebe.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2kzfudkkt.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2lmadgswj.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2cbujfveq.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2pgnlvylo.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2ggioytco.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2swwmxkhg.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2dzpmqdaf.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2idfacatb.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2xrdugvrm.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2jteywubz.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2lozvwmaf.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2gnmuzarh.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2ntkxqwxk.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2utjsxupy.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2ovbkzbpy.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2zbmxniik.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2ypnrmgii.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2uskkkiij.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2rgdyvptv.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2mvbishvs.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2kqjikgmh.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2lblnlqes.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2xiabuacg.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2enbfcsnb.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2cofxvftf.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2bvpaqvil.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2nwnbcpqu.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2cfhdcyoz.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2ctjbnfet.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2arvduqyu.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2lwpgrgqg.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2gvjvbkjz.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2zjiokinl.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2onbynzop.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2xhcsbeej.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2gjprvayf.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ykdungxa.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2zqzycnfd.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2byfwqzqg.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mfzjelag.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ikyimuzv.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2avjviilu.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2lgrekchj.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2nuyolgwp.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2dbrvtfus.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2hqpwtbeu.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2msullypy.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2tjnunqcf.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2tyecoirl.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2dvwuwknk.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2asabsxin.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2jzuvtczd.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2llwmhsls.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2hijsgoey.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2shtjbadn.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2icquyunj.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2qljjpqsh.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2esfkdaju.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2ktcogyjr.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2wianmcur.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2bjtzigoh.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2ichalswe.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2sgteursd.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2afqoipmv.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2fdizkzub.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2stipljvo.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2qqvqydwq.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2vjufhamq.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2hmsgihiv.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2edudctps.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2nzkawelv.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2jrfcffah.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2hpnkgrqf.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2fqwfntxf.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2vgcvsyut.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2jtebtjbs.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2bbcutxkt.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2aevfdale.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2axsbboto.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2bcyfffdh.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2onsumjhm.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2xnaalvgw.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2ocywpjre.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2oszppuze.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2mmtfbqdz.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2sekhnerg.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2gxsmiayv.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2pmppxapm.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2oxthtuyb.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2jszlztww.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2kerjgjbb.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2xqgvzher.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2hefuonbt.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2slzlttxp.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2fegaoepi.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2bebrfefs.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2yclquapu.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2zskgrjou.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2lfeejlsp.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2qdyrllum.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2uhcrvtee.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2wyhagnfm.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2bzjlgrjf.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2jofwyhbc.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2kduaeqon.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2jqusclxg.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2pzenofdc.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2rklvjcbq.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2xxxbnrke.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2kskqrtus.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2xxekiuwt.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2mmokmfkf.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vljeusch.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2zinjkjlr.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2dvymuxha.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2lqmwpkwx.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2sjmgicse.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2ivhwlpkx.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2uirxawxt.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2mcssxvtv.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2cqimxlgi.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2vohlekgq.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2gnlbbtoi.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2nvrzbfkq.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2zzwhbdot.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2dthovznf.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2ptryetuv.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2ijhofdfn.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2vjmjmfcn.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2fypwzpct.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2wfactfzf.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2zeabmfct.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2xshivmln.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2eeuslitw.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2qtaypemo.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2judykfba.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2csikflrh.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ruiwweym.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2yauwaqgk.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2yihypnmp.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2ztklamrk.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2skaihuyd.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2uvzpetat.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2obxaweow.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2oajpbbur.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2zxqiepav.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2tmcnucle.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2iokzlhxm.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2otmflfdz.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2ftfrdgrl.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2uhiyiksx.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2eztluuni.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2pyidwrou.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ylrtbfam.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2kjllefkw.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2dioqddvh.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2xstucxdk.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2rlgbtgwy.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2lnokakru.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2uedadkmk.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2sravcjab.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2dsqislst.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2ubdrxehb.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2enfryzno.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2xfesdtui.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2trpaltfs.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2buqsqkto.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2vnlivrvt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vnudzyvx.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2vnptyzoe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qlyintvk.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2mwrghlpk.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2volxmsaw.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2ahalkmjo.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2kbqhifro.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2opiedyel.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2cjlmfwme.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2brtlcsxb.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2wfotbgcv.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2uvmcueuu.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2mckcnbvj.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2cperzbsh.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2xekeugbh.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2atkioaru.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2veseuioi.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2jcfhtknp.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2dbzzfpkp.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2crbtzfwf.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2hjhsfjxo.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2gtmlegvm.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2qoabywjg.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2ycmsexcj.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2mtrqdpmz.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2epqibgaf.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2bmyzmzrp.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2pesnumme.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2qqihlgwo.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2pseztntc.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2awivwsty.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2jzartscj.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2qxduuhpx.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2hmhmcfmw.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2enaihawa.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2bwqdjdty.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2xmwhwhoi.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2osjmkrlg.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2gahadfzn.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2bdvarzut.html


<!-- 参考信息 -->