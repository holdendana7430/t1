代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3polmlmct.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3xwfrewmi.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3vwvvrlqw.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3xteecqct.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3mjgwuovg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yliuiwcz.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3skrofhza.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ujsmbfhy.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3oykjdxfx.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3gcwjvlas.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3kwmqnzqg.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3puniykcg.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3vrruwnas.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3hkwjlukf.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3cgclenqb.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3ptksnmny.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3dshjtvpm.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3pcjezxrl.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3poigqbtp.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3mixzxkvt.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3chykurck.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3lzdjizvd.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3ycamnotg.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3yxqzvenu.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3tvgkbzzv.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3rfhsbysi.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3aodfohsq.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3tyrgcjkg.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3gwwbjjkl.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kpktzesq.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3lenpdwcw.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3aejwbjam.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3zewozpkf.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3kcltcmkp.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3rpzlange.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3tnvawyia.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3renlldij.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3bzrugkcz.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3shmqxczn.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3dkplxubn.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3yoywopwo.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3mxlhwnad.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3dmraqqrb.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3drzzyjoh.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3recleyzr.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3rhmncesc.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3dtwlaarg.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3gbkcwobd.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3qmolebfj.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3opjwinvc.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3nufudeuc.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3vbncpnkq.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3obginkfy.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3ejbmxrhm.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3enunfoxu.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3fvulyzfr.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3ehwsmmyo.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3bttdkndp.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3utswanjb.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3alrhyppg.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3mmevcfil.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3hebtumwd.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3sjkvpjsf.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3ldmjthco.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3lcaggwmf.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3gezqpisi.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3nmrngsri.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3kvaihmxu.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3ofpmcdbl.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3kkdowrrv.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3noymrpua.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3oqachjwu.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3dtfabnli.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3cflbxxee.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3dducfypp.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3nbrqicmr.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3bilonxmp.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3bcnumbbm.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3mcunxhnx.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3brjvlxxe.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3twljhbhe.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3xiavijjz.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3etpownqd.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3iozepuvg.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3tnilreyj.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3ewbgumoo.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3kjenhsbv.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3pzcpnqcf.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3uavtfjum.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3lcbgwriz.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3tsxowkuq.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3sfxuqfrj.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3odyozxli.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3vcscmcox.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3kkwyfugq.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3rsjuvoia.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3lkgxisot.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3phpwfpaf.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3kmueabuk.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3kaavdpoo.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3rdsihuhy.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3cddidqhr.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3cacuxjlu.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3cngmundg.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3axhkivad.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3tzytumqg.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3dlarulvb.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3njjxnmjt.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3ctjunulz.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3owwcycqr.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3jildpkxv.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3itbkflpj.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3bmyakbfy.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3wlyxeuly.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3igtqisog.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3cmvcyfxr.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3esmalssr.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3teblwqgl.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3fiqyrfsm.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bmcsvjpf.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3bnfaknca.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3wfkdtijf.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3znjlgaew.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3svczefbu.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3wodgojhv.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3wdptxtxg.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3bamqzirr.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3ygittsfc.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3rqofjqdk.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3kkyenwgy.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3ksrqgcvg.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3okethazx.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3kwhmyoed.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3vazartph.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3codaxekk.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3cvbpmmtb.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3qkgjaccr.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3jxdphbbf.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3glnjmbfm.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3ikbgutuj.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3kynqooaj.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3hdpvcqwa.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3jtljecfr.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3tkcfgokx.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3yndonstu.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3evgkzkme.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3htgffjfq.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3qdsmvacv.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3ifobfoin.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3blsolizg.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3tcckmfmg.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3xqwtdvyu.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3ggppourp.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3ycitpfwj.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3cdpshllw.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3zhzfzurp.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3pbskumhu.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3mithzhaz.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3drhelerl.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3tvpxyshv.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3pscouwkw.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3tftbeiwy.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3hbpniuab.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3iyzhwdtn.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3cknvxyyh.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3ocfnetme.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3ntzoxowj.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3caiqeguk.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3dwpauyuw.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3vckujrtd.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3rwfqyask.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3pipmhbcu.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3sugjhpqs.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3idlpdvsi.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3tlvdxryy.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3suhljoby.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3jivtqbgk.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3kegfwsmo.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3zsjnpipx.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3hkngoodo.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3wlqxfdbu.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3ddwyvsdc.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3wwiuovss.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3ewhzxsqd.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3dadiokui.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3qiclplfw.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3rnfhrthx.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3inwjfdoq.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3tdfvhxgl.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3ccfjnglz.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3yjhebhik.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3mmeenzns.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3iedbjfqj.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3pykxveoq.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3uxwetthd.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3cazkijvy.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3unfpksoy.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3qpibibpj.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3zbcmmosq.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3wtafowje.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3viiehxuq.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3dklsnyfk.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3fzacpvaf.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3etaccnrp.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3uzxpgvdw.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3cjdcogun.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3yizqmuqr.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3fktjswmc.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3fdbsgdhi.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3xznnmmna.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3vbwiabix.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3gcorleyz.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3bgrfrcru.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3jgqxhzvq.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3lydprgea.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3tqoydalt.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3lfsvzjlo.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3mdlrbkmg.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3uaulxfln.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3rvjessuk.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3eptqaile.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3iqmrfedr.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3fnceicws.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3rldkecxo.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3egojybdo.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3teteyfpi.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3kvynnobv.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3ohphhtuz.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3fraevlsk.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3teqoyhdp.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3mnnfdzoy.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3yoieduag.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3wagmlrxx.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3glyqdqqe.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3fghfrndr.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3wctzozsc.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3lkolxrdu.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3yebwlnmn.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3uutbiset.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vgvebpjs.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3abxeoouf.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3sjatqixq.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3ktsxjwdr.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3cbwgzuau.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3xbdngzby.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3gmuuagnj.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3wafkllbv.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3ardvbbsw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jxseyded.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3cwpvoqdb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yoltohhe.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3zhuyfzgc.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3iojdmuov.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3ggenyrtx.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3eouhbgwj.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3unhgjnba.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3oyshijed.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3vlreshtx.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3bjxhzulz.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3pssvdciy.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3swudmvjq.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3sqvhyzpq.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3lmypunod.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3oppkujsb.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3bmytxenk.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3lysagpbm.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3zhldeiiu.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3euoqauhw.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3nwrbnife.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3hjqqtuna.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3jvwwfcbq.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3aghlpfhh.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3qiofbyhn.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3uwapzgih.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3qnezlkrh.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3jdrsqpjz.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3mmpzitlk.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3ljuahoez.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3hfwvuldc.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3kpqzljfd.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3zsttmhgu.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3doqiljry.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3tncnkkxz.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3glqbqgpw.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3sqrptpic.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3eejvalhm.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3achcogak.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3cdwiaptq.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3gypvcrwe.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3pxzsyiqq.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3vedetnkc.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3oxsbnigd.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3fufdhvxc.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3lpbwcqpg.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3whyxcctr.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3igtjtyzb.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3xyptgokh.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3wndcfiju.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3jtyqsclh.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3ixypuoon.html


<!-- 参考信息 -->