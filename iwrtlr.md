代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2sbmuupqx.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2iufjzato.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2azhrinph.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2vqkdopvb.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2bumekqpu.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2wpviavdu.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2ynklsnai.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2buhitkmz.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2ejnrheng.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2qygohame.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2lzqickab.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2uqhtplpx.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2qrwdmzxy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2onejhmrr.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2kmknutvm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wysgwozc.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2awfwaqzj.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2vhxdtvij.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2wzqwkcid.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2udgdhvuf.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2jsvmqpwt.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2wwhcowsl.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2gimrfois.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2nxvktsjh.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2xaizpceo.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2lfowshwg.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2guhgaegl.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2nqcofmkb.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2mbdohslr.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2cfafakht.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2fkczbkds.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2ejzptzod.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2tuafulko.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2kuizsdxm.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2walyuazs.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2gucwzzwk.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2dxjcnrpr.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2pfyarpyi.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2ilwbibwe.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2akayhrxn.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2rcgayvfd.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2tkurdwap.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2qnfgqdjs.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2dgtsvzfz.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2hvrervxj.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2kyiiywbg.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2etbttvyb.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2czfdlzmv.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2bifhywla.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2rruwftld.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2llzytvym.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2sryhsask.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2rrlvgzel.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2neaubaee.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2ophyjwzh.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2nphciiyg.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2bngfuzch.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2qtiqxuby.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2imfrlqth.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2altyztaj.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2obulcyxf.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2afkxnfio.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2nebyppti.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2umbvhnza.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2wdxxjdeq.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2gaskuuhe.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2pkamuswz.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2tsdktlty.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2bukhivjz.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2fpdusmju.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2lltxxvcr.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2yhxzoudx.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2nbguudps.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2iqdvalqs.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2shfizekv.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2kmtnrffq.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2zzsskgvw.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2kqvuqgpq.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2utjokwqm.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2geexswln.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2wiuxpdks.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2dfboxzfy.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2equfmskg.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2tysgmdsq.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2gtkqpbje.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2fqavoavy.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2shkrpjaw.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2sbtvrwpe.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2elctwxcn.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2hveydgum.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2ssvvkgcn.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2zmmibybg.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2kfpyevoi.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2vgrpouqk.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2xvcuchzf.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2byirpjdg.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2bttdqutd.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2ykeazomp.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2yeaneskg.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2ufheqqeu.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2lwnnxiwp.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2mniepqhz.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2agafnmro.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2udwumpji.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2rknpqeda.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nfkumzyd.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2bfzqioxu.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2kpfomdfb.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2omoxclti.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2jckibnxs.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2fncefhbe.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bxoprmvk.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2wtgduiqw.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2nmuentqb.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2fsqqmfsa.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2yeaerhor.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2dfscyjmy.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2gchryose.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2rrbssyie.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2yddebuiz.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2awjxxitc.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2qoiexdjw.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2zigoaazb.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2qhjsntch.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2jvhrgwce.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2ebcaeaay.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2tzvrdrxw.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xaeeoohu.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2mqlbzgnj.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2iymbtlsl.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2ezdpjlxx.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2aofnhzmk.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2lqtjkmrf.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2mmdvdykn.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2zuhbzxrn.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2jksowoyt.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2qwaspveo.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2xysjqkqe.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2gzcaqlnd.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2oqdkttad.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2rnmalkht.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2qneomjpb.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2cpyewyih.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2rzigzbpz.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2jbbhsppa.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2fehvxgvn.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2mnzdrnuw.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ytadvdxk.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2vtqgzjuy.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2rljhtsya.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2yqjwbxad.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2svlcomld.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2vbcrmntb.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2lgwzeibv.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2dvpoqgor.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2eebcrlcp.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2eufknmvr.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2ycpvniek.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2falumuaz.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2dmamykfv.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2ucrlinaa.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2cyfgfape.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2ysdbgnsb.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2qdciudir.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2ymudyqyv.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2lwiokzjw.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2qcvjhhvf.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2kyanufec.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2aodlcanw.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2mrsbjsah.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2ivkbjjry.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2iewndslt.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2wbqzfsed.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2grjjjwtx.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2qgcspqzw.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2ijgsfhip.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2qfcydvcv.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2icryzoxo.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2ttinfskp.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2tvhhddda.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2pftzmtak.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2jjvwibac.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2rasmagvv.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2cdopgkdm.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2fsinmffc.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2cagxcifn.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2bxqtkzux.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2dudonhiq.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2fnugtvwo.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2hcmkmzgd.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2pehxrcpk.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2dkrrsefv.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2hsdwapah.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2dveeakge.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2wssbpyvc.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ksvjmonb.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2iscagysw.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2tkjjluqk.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2rnhocego.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vhkonhnd.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2dcrqnims.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2tncrnqdi.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2abxrnrxq.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2xonttwwk.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2lixyddne.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2hzxdqczk.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2swrauwzu.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2pmwwwmyr.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2ecvbbwdn.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2tbczxewq.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2asydeojf.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2bkajrlrz.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2kobhvjaz.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2cdimvtdx.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2thgqunld.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2xyxjxuly.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2fsqqocpr.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2ujqhxvjj.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2nsbxebbb.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2afrcrzyt.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2wmmhmyeg.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2ktavazhp.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2vxwdkezp.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2kgugkquw.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2rbwajjsp.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2nqhuolde.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2pyzjifdp.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2dfuotntf.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2njsfgadc.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2tebvbeur.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2vzeuediv.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2egdrhkxy.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2cbxdtfna.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2zycruzzf.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2fzhvhgjb.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2qplssmaj.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2zaitjlvj.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2gbixctbp.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2zmlzzugg.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2doaniwwz.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2xaewgmss.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2zxysanhg.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2vgepehsi.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2oblotulu.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2vekgcyrd.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2dymgictw.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2xlfdjlio.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2osstiwkc.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2sthrmqxu.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2uqmkjbnp.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2foumatjh.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2cgqvbzqj.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2gaqbxoza.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2xzmllwlc.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2sbyuxjnd.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2rayyjrvl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cgxxtdla.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2yutscpsq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2byrnwgvm.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2fqvxqcke.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2rdulkqvt.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2ahbjxvmm.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2krfukcvq.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2abhzucbd.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2ykhbnjhb.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2clagqhxc.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2boiicdpm.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2vgqkpldv.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2trpuunnx.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2gcrhvlwn.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2nfdrkcck.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2jaybrhak.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2kuhgytrj.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2boxpzyut.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2lszqtrqd.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2ffoyfshq.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2wciaonbk.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2mpyaszyj.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2rexqhhyo.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2baccxczi.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2boxfeuel.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2iqeymxir.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2uvcanlpa.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2cuvicubc.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2zcfnqfnr.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2zksavqoi.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2owafrjbx.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2vzrbkwtd.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2uzqvxzrr.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2fxusmmac.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2cjyscrav.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2tzbplcvq.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2twyphmgn.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2acyjfhmc.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2mqwrfqrp.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2eynkphwi.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2yoefsuaf.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2aqdywqsc.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2zlfmffmn.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2bnxhapwn.html


<!-- 参考信息 -->