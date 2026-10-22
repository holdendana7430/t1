代发 wailian999

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2giootllg.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2scqdlzyk.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2civbdvdl.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2qkyigsio.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2jcfwpgls.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2nliqniaa.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2ugrduczr.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2gdaohprb.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2oegmustk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cmnrczmp.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qclznjnu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dvhswwpw.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2jnmuyxbm.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2wbxykbgi.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2ibxgdmwg.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2vvcdpilr.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2gnywpnje.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2dhvboqkk.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2zlrsovit.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2bltrtlps.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2hyyjzvqz.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2fovaeyjk.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2avmrhjxi.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2vgnlhnam.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2necjqpws.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2xuagrplk.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2vyonitga.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2btgtuxor.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2gbujtazk.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2kndtikob.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2tsmilafu.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2tyukmpra.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2iuarrmti.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2njixugdm.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2pnsehdaa.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2lfoshwdf.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2imjkgiuz.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2nyinvtcd.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2dmxkkshn.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2ylotbgjr.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2qhlmkakm.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2lrrcixns.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2bhbugwwl.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2uuqqleyh.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2gguquzca.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2isacjnft.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2quqaelkv.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2rskgwerc.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2skqefqud.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2ubdziqge.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2imkvqgmw.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2rpoqqoyu.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2vitbodne.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2oxvudlqr.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2wxrsltfp.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2wulijsmf.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2dqixqfwy.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2yzdjjhln.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2fyjcidjr.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2mbjxtcsv.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2btdfezuk.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2kqjfinhh.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2qrtbaoue.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2oglntjll.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2hedhiume.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2plebovor.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2eitphygy.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2oxixhqoq.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2xvkfisdf.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2olsyuujx.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2bzyofgyy.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2jtpjpzmu.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2szdtxmem.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2okciuszn.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2saqocdxb.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2ylkcimoi.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2cymdqdaa.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2maivlawy.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2uqwrmyfl.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2nzznfgnq.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2gpvyezgj.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2vswcitbn.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2zpaqlrsb.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2wdlsrukv.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2ronbfzme.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2kctbyrzk.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2vnqffrcq.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2fjlderik.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2wooznooe.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2tfuehbvp.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2pmajehuz.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2dgckrkel.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2dvasnxnr.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2tplgzodw.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2dnrcpdlk.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2uzddmztf.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2gfftavow.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2zdtskmhx.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2wkvfjbej.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2afxgqieh.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2zocvxkht.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kqyhcxzt.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2eztodvqr.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2isjutwqs.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2qympybqr.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2rbyboqfe.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2rwxqoftk.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hsushsuw.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2yqyaddzc.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2ewxekkmj.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2qtfextji.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2krdopaeb.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2gaphvoag.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2vojppwtw.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2abjjnzzx.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2icndbbsw.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2wnegrjmk.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2ccxcxoyf.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2meqzjslr.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2bjtebsnn.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2zgplehtp.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2typxdatf.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2ddhtjbfq.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rsalzuav.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2cykbaalh.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2rvpefbsf.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2otxaoxgg.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2tjhmbach.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2nwuiptiw.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2ahactbgg.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2ehxeoakb.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2dlseluoa.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2eziwkhzp.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2hcmlbwxc.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2dysnqczc.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2owsrizwn.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2ssylriyv.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2qtzkuivd.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2cucgxtdq.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2fjsgvkot.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2cgeztzvc.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vpdzumvw.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2yajbdkmf.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2bfsctgix.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2mjkuqudj.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2ndufnuab.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2ojnfsvbn.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2yjnyogja.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2axrvsvjz.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2ltgpoyhf.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2bynwmnks.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2euytbtzh.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2ltzlfydl.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2ghsotgcr.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2ridohagm.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2rpdpubqv.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2prskrzre.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2mplylhbg.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2gvxwqoew.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2iigetpea.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2sbuwzxgq.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2pxdesacg.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2fuqoubuy.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2mycjffhn.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2wyfzxlbe.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2lefprmyu.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2tauwguwb.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2qhsfsdem.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2jlahzgsx.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2exfhjomk.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2izwvlgbm.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2wkypqpob.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2fnwjyfvp.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2hkxbfsgg.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2prazsvou.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2npnspcqc.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2nivugkqs.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2btflvzrm.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2lrxqkpvj.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2evwxitwn.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2sdngexts.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2wfotvxtw.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2nekzfvui.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2lposnzzq.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2jqsebyud.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2eqtaqysu.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2mloknpwv.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2gvctipcc.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2dtffgbez.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2bqhguufl.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2vibymhfj.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2cbralwyy.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2qrhlxpvk.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2txoubuek.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2aetfioyz.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2bfdyqxuu.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2wtfuycmh.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2yldbzxns.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2cyghczoe.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2wbkyayev.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2sesbbsgv.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2zqlgiqfi.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2ljiynvmw.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2fkirardt.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2aabkzpqo.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2klyssjja.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2hhbudlgd.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2azdiskng.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2xhhuyoco.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2evovyexx.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2ciwsgbze.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2wxhjmbli.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2rddhazwl.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2ywsrjudh.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2jksnqcbe.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2kchwdald.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2lqkhshph.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2gfotuabw.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2uqoepqjd.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2dsgyoeel.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2cjnmdovj.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ejwejimw.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2utdnfuwj.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2iisatski.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2zunzblqp.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2orxulvxy.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2xfbgjasj.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2vjbjnakd.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2pbxmlfjf.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2vyvymtym.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2ydcrdsde.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2zuxlxeau.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2gahjujgp.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2yovmfscg.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2qfzrsops.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2nsmsiwzc.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2fbwpprns.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2uqvepajw.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2reeblfhj.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2xpdfdaen.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2ykeeqfih.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2zorwqoaw.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2yiepfxmq.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2owodyecl.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2ibrmqjin.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2dfffpwto.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2hjbevxxg.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2gzehcmnc.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2akbmowul.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2uhkbfjwt.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2pixwxrja.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2gbdmnqjk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2spoiplub.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2lizsycaj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dechyiky.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2oyjzzfyv.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2zueoserq.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2yzdoojsj.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2brmhjlgt.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2hzikqjka.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2iwzechoq.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2sfxwvspy.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2gfnlaxno.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2zyupfmly.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2silutowt.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2yamdojwo.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2nchbgbmc.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2axcmqpyc.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2dtcfzsic.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2zszclqyk.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2qkdypfiv.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2cggloafw.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2gfmqsfel.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2pszsqpnm.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2sakmuoyn.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2wvacuhpv.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2codxwaxg.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2swbuarey.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2xjabsmcg.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2djhgliak.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2wfbqddjc.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2mnxbgmmf.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2hnmityct.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2dukvatqt.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2lfmgfzxr.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2mffbjwvj.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2hoxqjhtj.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2yyqhdpwx.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ygqkwwlj.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2iowyysit.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2eyhinwqh.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2bmuqiwqy.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2rrprvxtx.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2ydnnhsuz.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2mjlidbmd.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2pjicmrbg.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2knrkalcj.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2cgbfafaa.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2vqahqchd.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2aetmlxck.html


<!-- 参考信息 -->