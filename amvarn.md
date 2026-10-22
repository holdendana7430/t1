代发 wailian999

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2amiqpuoq.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ayymfafq.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2uirnnasq.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2otxonets.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2yeoseaak.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2peygugnb.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2zmgjhtgp.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2ofelbpyf.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2mixnymah.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2miorwlpv.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qdjxtjdc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hoelckba.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2tiwfahhu.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2hqrtvijg.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2iqtgdnff.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bqrmkdsx.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2xoauwsyw.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2zzngjrhi.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2ahkpvaik.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2ateiqorv.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2xfpawejl.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2feuvsssv.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2fbwszoor.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2galearvr.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2zxkdqptw.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2ytbyyzco.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2lmgbqvzc.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2zqfgdkdz.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2ofhntiyu.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2kxratcyx.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2fjojsssv.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2jslaevzn.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2gibdufii.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qoudvjvo.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2gifzqwru.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2omrumjpi.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2pjvdbhym.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2tglhaqzk.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2vrvunucd.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2rutoniyb.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2qwbmhtzy.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2oterdbjd.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2sdzpebdu.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2pwwbbdod.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2abjwcegk.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2cubtmbdy.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2wknyqlyw.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2zudfscwv.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2bujmgbni.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2liqhdgdp.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2rqpyaifi.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2twbppnqo.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2yqpyjuny.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2lxmjdxwz.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2jzaprsgs.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2jibczqwj.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2ofinauki.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2upwytmks.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2gtrorvev.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2qeuuokgs.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2gqcgyrlh.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2jydphyab.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2ecosvbus.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2tnnmalws.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2qsjvzalt.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2cnokcbmc.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2xabvdpmq.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2oxrtivwr.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2tuqngsof.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2rzqztsig.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2wnfjpkwu.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2rbzugpwu.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2necwfurm.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2qwheoagt.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2buixjuec.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2iggztvap.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2siwzgihx.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2airatqqp.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2diozutrk.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2dxmhjtkb.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2hffkpxog.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2ttowkjzn.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2rawvexew.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2wajksduy.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2xulfnvfy.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2tzgtiejf.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2yjomwrcx.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2uddgrvcn.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2awmxzrgw.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2semkpjln.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2kbwnsxzr.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2vjnzuabl.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2jptvcjrd.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2kjazepbk.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2hsineiuy.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2ykavyvmb.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2ufjdqjwx.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2abarbbmd.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2fjjdwapd.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2nkztudec.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2adxnwwmi.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2kjqdubhx.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2livhzyem.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2imaysemy.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2twpronie.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2vnqbszzg.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2fcnlyufw.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mcdlctyx.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2inyaqcmk.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2ritkevnw.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2fchwjpnd.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2ujxtwywf.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2zwinsgai.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2ucjdfzwo.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2wealrnxy.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2tvvvdyzy.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2ewypekey.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2fgpviwfe.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2tkdkekpj.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2krqhwhja.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2izbwstdu.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2bbrugypt.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2fzhdwtyu.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nsuasjie.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2adqajrth.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2tgffrcxi.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2elhbykij.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2owreyaed.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2xifbewhh.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2gqqoidic.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2mvnzkmhc.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2jaglfsxl.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2pvmynmud.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2onkccrvn.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2edyijjhz.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2qzsxyhrx.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2avlfhuzn.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2rqvwggfe.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2kfcgvlii.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2hhpxxnem.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2ggxpwwgf.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2iiwogqqr.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2szuwjlmw.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2buatfhxk.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2thohjejj.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2ftbiwqrp.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2cjoodsmk.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2ppfjlifi.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2xifjlriv.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2fanfogpu.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2iybgettj.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2sosbklvd.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2vdrfqkxq.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2pqqyemal.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2hjtbccnd.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2kzamsjpk.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2vlgsilgc.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2cswfmxpn.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2azoikoon.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2ttnuofrt.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2ocltvfki.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2oyzkxxgl.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2qmdtejuf.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2phwgmkbx.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2zajkchdy.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2bvofbkty.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2betmarrk.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2wtafmjwe.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2ghzcwstg.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2dphwibex.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2tzoxbzio.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2wcfdivfb.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2vyrkcyee.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2wwltoxau.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2wqznveux.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2jydgqkut.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2pdkxznpj.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2syqucapf.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2ftbjqhay.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2lxzbfxez.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2slxlptdi.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2vqivqyed.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2pyddmxjp.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2vnxnbqsi.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2lkystmxn.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2lmowmkra.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2uikeqcnk.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2hiucpshs.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2kuxdsojn.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2dyyzvxyu.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2xxlubyrt.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2tmipnvjk.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2vlvjvwpm.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2lhdipmdt.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2bfuuevhg.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2edpfmvyr.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2leqwdbfk.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2vgezakjc.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2ysqfpuny.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2synsdmhw.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2mwrblvcv.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2dvfhtlbn.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2meavmeff.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2lcrslqfa.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2apgehnto.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2woygnwav.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2jmabyqwq.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2qduutpzp.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2lierrfht.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2bbaqwkgb.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2mgcgsxaq.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2umaittdc.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2kavwqshd.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2eddqrxtw.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2aqxhqxxx.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2cnjlgadc.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2diseypsh.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2txkylsvd.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2ykzfhnkm.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2cjiqbsql.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2rjdykhjb.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2qixnyfyo.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2jiktffxp.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2jpotjnbi.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2xbwluqnk.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2tkkjfwaf.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2ulnaorlu.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2odwpqnnc.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2pmilkqyy.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2lwucpxgk.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2wpwlmdht.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2jadlcuob.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2fdzjqvks.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2eubyspls.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2zstaeqoz.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2osieooda.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2yjmoadre.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2tnubkdsn.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2tlilxahj.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2rhknsclq.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2emuftapz.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2fwddzyeo.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2kkjsqout.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2etepfyrx.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2abrgwifa.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2phgixhoc.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2pxopjyym.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2yyohapiw.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2kkzuoqrz.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2lxxgruat.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2jtmeajgn.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2knzyapwd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bosmamuk.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2qhroffzh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ejkyetqa.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2erxnenyh.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2uvoyhimo.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2ssejfobc.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2hvoifash.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2fldgllcf.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2sufohtnj.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2apdrivbv.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2wgxhlzlv.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2mmhbaoly.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2jektardo.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2bvdvgmli.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2flsgsxxf.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2nylbzwrq.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2mjotqjii.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2ibvudsio.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2rntswlun.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2jvlzyhpj.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2pdytxeih.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2vvekfmil.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2djjchjhd.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2wopwcauj.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2yrjbaleo.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2itiecbac.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2wdnlpfpc.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2yoxkgiov.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2kpscyewm.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2oacgotso.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2iubqmceh.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2swdzttin.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2zmdtqknl.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2lgxsbiaz.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ercyitey.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2bxznybqc.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2drlwxbkl.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2wvaqqqxa.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2wciwbayv.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2bzewvivo.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2qoaywkav.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2lwcyfvno.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2gedztcrf.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2doewknnq.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2ntugfxde.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2bjbludnv.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2ratjwngr.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2bjhlodnd.html


<!-- 参考信息 -->