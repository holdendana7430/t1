代发 wailian999

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2lfoafxks.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2ozepjvzk.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2rcrkzwcf.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2apvtkzgb.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2iwmndaqr.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2jcgqpenb.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2qvlstpqv.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2pivullbo.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2cwjfnlok.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hfrehuts.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ggfqvyak.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wmpvvsxh.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2wyopqtow.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2flizactm.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2gxjfmaar.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2cetmgfsr.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2kbnisetq.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2yzwvqqtc.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2kzpahaxc.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2qfhetgsf.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2csalomzd.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2dhoxyylk.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2hhuxrdde.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2jpulrygq.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2lzvkbkbf.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2jevjgflg.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2mvekworh.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2yyaelzmd.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2furuzizs.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2trrtanpi.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2peucqzmr.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2xlbijzgk.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2vqwdwhtg.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tkrhqqxk.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2uggpqlhp.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2cbdlkfrs.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2avhqwjpb.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2fhysilnn.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2vzoonjku.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2haidlhkj.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2jksxnoho.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2uzbzkjgk.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2hyvwrqgu.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2sgnczgmu.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2tcaptgvf.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2vydsnypy.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2zpannnom.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2wbghzuht.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2zjifvoxn.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2yogcdqyh.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2ickzlytm.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2jzfgceov.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2nigjuqod.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2birnttnt.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2ljesndnn.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2lsydqqam.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2cozmqahx.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2ravvqkqo.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2vzxhzidt.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2vvukuqxp.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2siiorpnh.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2nqjxhmti.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2dvxwxwvq.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2vtiinfns.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2yjppzhdy.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2golprzvt.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2videisty.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2ppmhdpcn.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2vhpjgqwm.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2hofqymrc.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2wupznyzj.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2pfjxyvct.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2wzdqqanf.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2uxcdcsvl.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2ttipnrei.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2pkeihnpm.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2pqtyojjs.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2gaenkdaw.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2arvrngsf.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2xvwvfbjv.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2xjgdifdw.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2idlvythd.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2rjvytolt.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2lsjewkhr.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2kzewemxm.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2tixwpbvm.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2qplgqiym.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2pdxpbfen.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2kwhgskyg.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2vxjbljwb.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2ifbruxgp.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2ivwjeniz.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2opkdhzgl.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2txbsrdah.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2paspstov.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2gfhtvhmq.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2dgkljanw.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2zwdfbkox.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2nudmiyha.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2jiswvxqk.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2ahhyzgra.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2thmczeli.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2nnlokitr.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2dvlgvkef.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2qdhprhes.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2urtzpush.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2habehjfg.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2svqiyaip.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2zvgbkmtx.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2hxautnly.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2kbkscpfh.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2rsbntisi.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2vhrhzlay.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2tdqyxekk.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2yszhoeak.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2ydfjeuqw.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2ncilunkq.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2sycdfcwl.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2pfhyxpar.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2lxoqhmkf.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2uhcmgafn.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2sjttkobm.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2irjkrnpp.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ebzpqclb.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2bzjzbssk.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2cdrqxxbv.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2kteuxwpr.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vdwanllu.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2qyulzrzr.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2pctpkwvj.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2zhkjcyfk.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2tzjjefyo.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2ugchvyjy.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2qiiuegkj.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2usfqofqr.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2qdmgzjov.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2gdoknopz.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2kreqeauo.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rrptrczk.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2sdyqilse.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2hvocybft.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2amravdac.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2nsnjqzeo.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2kbbnmogv.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2oybyeoor.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2guuuqshu.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2vmiteywp.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2qyxmfhqy.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2weipkcxn.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2cnhmdczk.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2wjomezcx.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2lewqhigu.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2fgdjutzv.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2dfpkbtpx.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2okcavtfn.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2qwkhlypl.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2wtbpcngr.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2rgpthcsv.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2dgivnucp.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2aunlmfpt.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2vbyoubur.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2epdmfkcp.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2yxkoasld.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2sjxzpdcr.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2yxswrkmo.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2fdunkppi.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2qirwzddx.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2zbokjhhe.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2tnibqujt.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2udcuseec.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2mivdotmi.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2jezmmzxv.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2xzwfkwju.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2iihxtxmi.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2crnhithh.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2qqibuguh.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2zxtbtqqu.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2vkajondt.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2mucpmapv.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2xfbzzzxh.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2ijmuethd.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2ektuaubb.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2ylubziuk.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2kgtnilor.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2liqgsiny.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2ttujebfx.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2nfdmwfbo.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2sjeyxbrf.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2bsrmotns.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2xqgavpwf.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2rurpnpyx.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2wesykabc.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2orbansjr.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2txutytlk.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2iqvpbbyn.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2pihakleb.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fhzxezev.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2eptctbcv.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2qaspeoin.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2whcwdgck.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2lbfrkahz.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2sfpwoiye.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2wypfjkfq.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2mfgwmisq.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2usztzome.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2hmmpcozr.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2bpbwzpbo.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2orvgxdhn.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2sqifvcko.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2jghilrfr.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2ljwwsuej.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2irebrsqo.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2eqscxfpm.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2dcpcsvbd.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2mlyatouk.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2medhwpal.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2jwqkfbgx.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2nhomclnb.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2xueboezv.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2nxdtrdrg.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2ruvxgirs.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2nzmepizx.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2uqgquihz.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2olhrzqyz.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2iibqaqae.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2ryhmimwm.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2gitqxdko.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2pvemgnvw.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2rlqidylk.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2iihclhvq.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2tfwphegj.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2icyqndkl.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2sikokiqg.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2wdzrwndw.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2dpcuvnpk.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2bpmcbigf.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2inbkgkbc.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2emhmxzcz.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2zyioyrsg.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2roygemmc.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2xdqpvupz.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2dnfwochi.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2ixbszvko.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2ywgynhxe.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2sklioicj.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2guwztfgi.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2reyjifbx.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2mccsdjlq.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2udkvbygb.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2xegadods.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2wblqiwtv.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2gstpdtbu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rzgkmmvp.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2mptpznnt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nqeyadlg.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2immizyah.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2dltakfpb.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2owcbvadl.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2dshlnyig.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2vmvhdgae.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2gregzipy.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2pjpfqyff.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2fuvcqjoy.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2dplxqtrh.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2ixmvkgkw.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2jgycxspf.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2zdfatjyp.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2cileylac.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2hphsbgqu.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2gkgjxgji.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2ztzsmtqx.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2lamoesib.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2mvhvsmks.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ittzzwfh.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2tuzwlzmb.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2oyxyxddr.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2yiicrtqa.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2drxoikfg.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2tztgmqkz.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2wqeojmiu.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2mqnhbikr.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2bxufaqje.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2qfrdhpny.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2fmcqfahk.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2rzmresnl.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2vutoxjkw.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2mxcaqlcz.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2khykubwd.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2nfnbptao.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2ppajlqnd.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2rsvcxank.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2clvdjtcj.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2faxsmthu.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2okqffnvr.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2vvcsglcm.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2ghkvhlrw.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2rueooxld.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2xgmcclsz.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2ytlonxum.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2jktejwbc.html


<!-- 参考信息 -->