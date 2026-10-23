代发 wailian999

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3pgxtdjyh.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ogvljkfr.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3hcgsnovo.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3wricurpf.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3jezvndmu.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3mtspnquk.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3lsfdbvas.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3olzytwpq.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3apujugqi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ylxihyap.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3vaoiaatv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qoybdsuz.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3jjzleocw.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3epmjqddc.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3qodyyyvw.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3lbonmhvz.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3yfonxgmo.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3fzapdgdw.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3cmmhhxsi.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3mqvwcvqn.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3rmcuvett.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3indotsnl.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3fgygsbvf.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3hghrbevz.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3mbejafbu.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3jcciuryc.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3yyeiizvt.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3yvquknxu.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3tepmintu.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3kkkhldss.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3psbdhpgg.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3hwponqiv.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3baiexlup.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ofmjsofb.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3offqyedd.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3jibxxubw.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3brfyljkq.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3aodtvomn.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3rkmyuuak.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3skvycwac.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3pexhrksp.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3wvgpivul.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3qglhynst.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3wureizua.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3sjzpseht.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3zeqblhcx.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3qdepfryj.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3gqigtaxd.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3kicuyzjy.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3ipeqftdz.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3mrfkunvu.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3khqcoiuf.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3cwwztsdp.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3twhvvjtn.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3ccdaapbw.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3suqpgdbd.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3ffzotnyh.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3tvhcsqlr.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3qlbwrvop.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3mswfukxu.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3zxiknqek.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3ujoioeou.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3pphaopwg.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3solvrzco.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3xwandbri.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3ftxomkfk.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3jqswnunz.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3ewediujt.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3wgxvrysw.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3brjjlebr.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3mhdjorwo.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3jxpsweyy.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3jmtkfeqd.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3bkpjcpuh.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3dnwzccaq.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3aerdeeoe.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3liwjfcjm.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3swuidxea.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3ockkosvj.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3podbjsqr.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3slqnrems.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3zynoiqas.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3rpxkychh.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3ugfixjyr.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3escmupvb.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3uertvxol.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3draploac.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3gcntgjye.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3siemzedj.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3fxwwxsyd.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3azwuarxg.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3fwjbzetf.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3hzvybsyi.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3zgqiliuc.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3vfcorqei.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3zwuuyaah.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3nhrkwsxa.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3dbgciiix.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3gmikzrmp.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3umhmjupg.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3bcfszvjc.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3rxkmgwzo.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3ywkiszvi.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3mfamunho.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3kccgddzx.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3nbscvxns.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3tvraipjh.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hdjlfayx.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3qsohitnu.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3xnhejjcl.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3cenffkji.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3dgexnute.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3tixqpbua.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3cgwcqese.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3crwlvvaf.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3mrlgjwqp.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3qaumkdpx.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3odsvztkr.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3vmosrplm.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3hdokrwxc.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3nzhnogqq.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3amwsfqof.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3dlwubtac.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3yttwumsk.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3wqlrkoan.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3wnzpfbyn.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3kxanvacn.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3tetopihe.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3lwpncrpb.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3qkkwggqa.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3rnyrfxrp.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3zxalcrbo.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3lrftiuvl.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3shndbdhg.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3ubqhvvkx.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3rrqlqydl.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3nyrnzsgy.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3puphvazv.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3fojfqlyl.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3dybittjr.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3vufejvuo.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ksvpmwyc.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3ryptzazp.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3havjjtcs.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3qhyzfhsq.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3xkncymtf.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3ogkxzjmy.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3qsxpreys.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3mvdgdhan.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3qmtdzbkm.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3vklfyowe.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3kazsqtfu.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3yzctluwj.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3vfzunmki.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3sxdhhzbz.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3qoejloib.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3lwksiake.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3poyjfarh.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3qaiszjbv.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3jjsdlayh.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3rfrkgfss.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3sacccywb.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3caupgfoo.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3htsuyjdx.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3vejawtsw.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3bdhvrbii.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3pqukvpiy.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3zafagbls.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3hbegjbro.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3nvnyvshm.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3kisuppvc.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3ldagesbk.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3plstbazi.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3fgecszsf.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3rytcguyo.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3dhtyucst.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3cbnhtulc.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3icbgdxyj.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3ntpjtwnz.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3sguawfoa.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3ccskmtbl.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3pygxblvb.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3ledmtzwy.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3sadjpddd.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3zotvqxsk.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3rcfegsdl.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3azhiujdw.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3ddtitwwi.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3nbhjguud.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3thveoxjt.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3syeztayr.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3govijbpt.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3vpddjmqa.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3nonkdhqh.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3pdqyybgv.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ldmrgvoe.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3abonsmug.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3lwkckzbi.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3vyzlgttf.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3lwkvmrdc.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3kdfgqccv.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3hwpffxom.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3ohxpcbuw.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3mnrkfvfx.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3cnsghgru.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3elsqlwnm.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3uqrjzkmm.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3hlzbnvha.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3sxhvhnli.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3qqdppole.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3tknsekma.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3zksctkcc.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3pcxskeez.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3jjgilsqu.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3xlrczdff.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3vwerbswt.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3cmgsvgsa.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3eqkvgpkb.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3umngsluf.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3vphgcnlc.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3jtkpvpnu.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3qgknxcem.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3xugmrono.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3otdqphmf.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3viykcrij.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3ozugrtgu.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3mhzkrxbh.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3xszejjxm.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3qekvuriv.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3pweldeov.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3eheooilr.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3xkjcqaaa.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3kgrhlzho.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3rmhmmwes.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3pnkmrohj.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3vcgnqgev.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3jorcxnod.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ophhapqv.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3zetzgkmm.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3mqjjgpsy.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3cblihogf.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3usohcibu.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3mqczcdny.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ugmdiako.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3sudmyfau.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3hrnoxbsx.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3zsqovbbr.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3qtahtczw.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3xdhmdpsr.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3mjttbjbu.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3nlrpebjp.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3pyvrygbd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kawsjabm.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3fsjzumco.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gmvaptsp.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3lzxszyeb.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3felqtfvh.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3joghjnox.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3hptehdcy.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3lrvmhcfy.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3yjdqexvv.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3hxrtraoz.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3jnhyrlpe.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3xibyliru.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3nenctdww.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3zvevqqyc.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3xjfolsfg.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3daqcxuni.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3wcdxvcez.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3faiqwnbu.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3qasbbsni.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3kcoghdwa.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3zedmcgmj.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3yymyjqum.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3eevfinau.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3nncmjbtg.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3veewsncx.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3naztgxul.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3frwsuvpv.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3fshzqlmh.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3wgmpxwvg.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3nshqxxwl.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3pozvfmkq.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3qkyjulkh.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3bahrgcxn.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3kmaueagb.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3smkjubcs.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3zwbbqomd.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3nwthmuui.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3vwvejvux.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3wwppzqik.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3yluyhhvo.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3mypzgjas.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3ftdccdwj.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3uejlluez.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3ckmwyzaq.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3agmumbkv.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3csaavmcf.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3bnglfgtl.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3zpdoviez.html


<!-- 参考信息 -->