代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3htqduprx.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3ddmagkyw.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3uxuaftyq.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3eiyzkpht.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3kigjpzna.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3easwhfub.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3rzxwarau.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3bwwjsovs.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3jhkiorbj.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3majtiqem.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3xeolxxav.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3kmbhkpnl.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3nboxhiig.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qvshwumv.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3owuknunc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jdvwurjc.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3dkddriva.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3sjtashax.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3qpuepznd.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3bixsvuct.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3dxhievml.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3kwlglndt.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3kejcqkvu.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3dbnwbxmb.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3ofysqrtq.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3wqyokbww.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3sraxftey.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3vibjjkmx.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3luueygte.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3bqhyemps.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3rbgprtyb.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3qromtcli.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3cwbbbsaw.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3kdjaazzj.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3ivgkietr.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3eqtbdkqi.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3bsvezatr.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wlnpqxkn.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3ynpacqje.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3svzctmmb.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3zxjxmqky.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3wacxdjmt.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3cxqdotec.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3abqgpdlw.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3zmrjpstb.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3ywzxvdqo.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3bhkupbrj.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3futnjdnp.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3tyeammkv.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3gveoiqpe.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3rjaodgnb.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3liqchlkj.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3jebqqkrh.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3ngfhksmx.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3fhldzyam.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3vhdcbsfu.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3cejfenny.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3dwzcxeey.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3ucnzduuq.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3kibwodzk.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3rzeiyxbj.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3jkwvudix.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3yksvvhjb.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3oolkqauo.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3qfljdozl.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3axsldsvk.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3dofhagvy.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3ybukppot.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3mniofgeq.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3drazzsbd.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3ltosxvaa.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3hbdyjegb.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3kwevcpzu.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3qknyrotc.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3cudjfetf.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3ixnufgsr.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3jqfxejuf.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3zsrjomyr.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3enkrfuwi.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3grmkaxaw.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3youbefii.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3fkzzqwtt.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3aoyknoqz.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3xnpwetva.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3opcckzdg.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3ooqdkuzs.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3ejauaaoo.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3pscgpyyq.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3wppuxmfu.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3tzfhiztb.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3htasamfu.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3xkokslux.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3zprlrjtm.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3brgttvlw.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3qsphmeiu.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3ummgtqeu.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3oygnbdcy.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3tijgyicw.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3apcnlwuu.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3azyppqnk.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3miamalde.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3rtfhyxgu.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3tnvaayfo.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3jucrcozh.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3vijvsrsr.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lrebpqbk.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3ogrrmqdy.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3ukrjattf.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3xlrcumfb.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3pwdbewpy.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3vcezoudj.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vkjvjxbk.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3fvxsmdzz.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3bnxokjoi.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3kbfhakci.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3sodtktut.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3odlqltel.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3fptdapmp.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3zubiknnp.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3afudwyfp.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3izfmkgqw.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3tefzflbh.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3xxhlhffy.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3ywhaufwq.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3zbjhayjn.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3pexymrgd.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3vuyeqcbw.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3nuhfvrow.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3bbvppdqm.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3tqexmhmt.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3idslbflk.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jlgwngww.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3tufhyxzd.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3fybnmqvj.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3lapioblf.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3rqnbxbij.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3nrhkjibr.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3kibjbfcc.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3nceccstm.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3rlsjqjoa.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3hcqslyot.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3njsrdznk.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ibsxzcbk.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3ogsamnjf.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3huvxozkg.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3nnzbzyyl.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3cbmvdnpz.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3brmzpkpc.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3zsjqikjb.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3idbdyokk.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3jbacyvdj.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3onpmxkwi.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3hklfcjjh.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3eldgecam.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3yhibkaln.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3blxxjdnc.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3yjdrjjvr.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3byybbsbo.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3nzzwkmrm.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3owgqtvma.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3exyqaqad.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3hibbkadf.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3ohgwdssg.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3hcafwykw.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3kjazcygi.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3jjgezzby.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3vdepyfht.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3vleyskqt.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3tuvanlrg.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3naoixrwn.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3ocyxuska.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3lhwhntmt.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3lkdwowdj.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3pqkzwjoy.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3ydlwyrtk.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3dfofbges.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3bvemecti.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3oygllrsr.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3yshowfgn.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3hgpcrlrb.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3pcbtvbdg.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3etvftitt.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3ditoiuml.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3kygwdynf.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3lkbkwynh.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3tyfdrlvb.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3swzifivj.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3oolmvvoy.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3itvorbga.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3vpupczbh.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3ctolcbbb.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3uuepvxbg.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3hhszrnvx.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3emqkfckj.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3jbtfqhrg.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3eaufmqtc.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3szgifrxo.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3dmwrtyoz.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3cetvnbif.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3iyoiobel.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ggyijshn.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3jubhbary.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3zcslwpff.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3gcqmefoj.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3ksvckanb.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3vwibyzng.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3kqzlotjy.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3zdxqnqxt.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3cchbsnzq.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3judwsrnj.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ruilertt.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3uazflpqe.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3wzgvtkya.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3mparzgxn.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3bpwsnpmm.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3ncqprpbv.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3pdieqlnm.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3usascoic.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3jokittqn.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3aajrzqqq.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3udszofaq.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3kfmlpbqd.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3cjirzxoi.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3fvahntam.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3dbnbdjmi.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3fggrfffo.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3cajyjtly.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3agkqakzq.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3unzsxerm.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3kjqvegcf.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3wmhmsscf.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3ytrjxsyp.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3tkgnofby.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3ibvdiedv.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3xqwimqtm.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3zfreflji.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3dggzyecz.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3jnvcqfun.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3yvcrsvxb.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3cjqevotk.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3ctfqmmfg.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3mrdtboxq.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3kmdbfgil.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3xtzfvymq.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3dqfqyxvi.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3tigtyoqe.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3dmiepuyf.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3drhuokej.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3ojnkajfd.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3guefqdob.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3rifmkrda.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3wdqhhbzq.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3hkcsofzj.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3esdnnsoi.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3ddlcljea.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3anuiqynx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nikjuvts.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3xckjsqzx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bvcnsrfo.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3rxlqnoed.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3cjndwold.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3qfyuybnh.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3bsnevytn.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3bluqbcjk.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3yocmtkql.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3lgdzeegl.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3qjxybghv.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3fifdvido.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3nwqxejls.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3fdairlij.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3szvjokhe.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3smiugxuv.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3dvmxsfej.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3zvfudtsc.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3cwskpsal.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3paldlxyw.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3tswvqemm.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3qruysicz.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3cymtzsnw.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3cwfscyzd.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3hheajlop.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3porslzhb.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3opkhzbzu.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3ghlirwfs.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3yvmpdqvd.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3ezuuwlpf.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3phgqrgfh.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3ykxuhqap.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3rlqtrqtw.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3vuitptvx.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3gqhxqeks.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3vpvlpywl.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ndccahis.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3whsjixka.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3erngloue.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3qrjjtxqt.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3ugloatqw.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3zmxctlmj.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3rhfazdxy.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3gutxrazp.html


<!-- 参考信息 -->