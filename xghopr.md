代发 wailian999

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3mlwopcea.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3ginuerak.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3ximnrgaf.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3jckoixod.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3mwpoqcgt.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3qjcnwuaj.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3qwgudyuo.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3gzxcemct.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3xqjotmyb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3poqgdldu.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3vgxyfhlm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cjtfumjk.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3gtfmegcm.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3ommrxjpu.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3jjnglfbk.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vcuqmsgt.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3zaryvnlk.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3brzzyjsh.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3zxurvdwz.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3nimztpyz.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3yeiqfjrj.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3jbkykbhm.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3uujsiapb.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3hggcsjra.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3oyqwwqys.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3fieuaopz.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3mdiwzwvy.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3ypeurixh.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3clvjoeym.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3igjkqukn.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3xzzhlizn.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3dbvglkxf.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3sunwqddn.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3ykgpjfpy.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3rwztrgwe.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3pzbiatqx.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3lbapjlyj.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3zvqlahix.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3keyeyucd.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3ysxuocpq.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3vxopyjsm.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3evgbakbz.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3ejtxspru.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3efyaismk.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3cicvqbmv.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3uxnmwgvi.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3nqbcesge.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3dmuvuela.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3rwqwdysw.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3ipzvbpsv.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3vqsruogo.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3jbwyqvlp.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3afvqpmgd.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3oqmmneqz.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3kzcfmasz.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3xnmsxvya.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3dkwvntdi.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3ebperijl.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3xsdkfpuu.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3bzcekpma.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3khxpsyki.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3ojrtbsad.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3jcrbuibg.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3anwmbyfr.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3kxwvgubw.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3tqbjawgk.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3jcevfnrx.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3udgachzo.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3vyhelsqh.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3xhhcykve.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3lgcqweee.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3gzcddtfi.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3mwtachka.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3fzftlbev.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3qyacteea.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3nkknuorj.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3ctpbdrvi.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3azxsoywd.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3zictpjwu.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3xioxpvjy.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3ztbrdquo.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3rcewetqz.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3fmfwcffw.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3izzyvoou.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3smjbjgqv.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3tfxtlkxs.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3skminaig.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3slianmsz.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3phlkwufg.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3zojnqxuq.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3gcbzbgcs.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3liciufkr.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3bqvyjxxt.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3hmlucymd.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3aqciunmv.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3tvnbccbj.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3ygunwlvk.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3shzxplae.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3bafbtnxu.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3sgdmteei.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3eduetplp.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3zmyeqytz.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3vmqbwbqw.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3vmbbzcvn.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3evkwhfhb.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3xjhafhev.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3bohffdtd.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rjjqbesp.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3awvyuitk.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3qiabvjai.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3vpdkvrrg.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3bojdiiia.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3bjjcjfjs.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3daycjvqi.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3vynndrih.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3oofiaomj.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3aujkskru.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3gtgbdlfe.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3kuezeoby.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3dndnyyiv.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ixtqwaai.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3zqqkzlpt.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3ueukggnv.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3wxohhyhm.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3sifdiobd.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3wgcveffe.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3skizmiut.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3qtvbrzbk.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3noytjaea.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3khyajrgg.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3kazhhgrz.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3dysjsbnr.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3yykneuzs.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3sgcppewt.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3oxpbawsu.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3hghlfwjs.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3gfvgntdt.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3cpxxoygj.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3prrqfoao.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3ojqzhqlw.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3frlywqns.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3vkwgdqmr.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3ktymtqlg.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3uyylpzzs.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3uflqnyfy.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3rlzefivl.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3gjpqghhe.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3zygxjigj.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3fhbwpvmo.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3jbfyuapv.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3gjbtztat.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3pmbzurcw.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3brpnvbxo.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3hcmnpwex.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3fylrqpru.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3frhdmwjl.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3qzdvhyfl.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3cdmtupcv.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3rxokliwh.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3uhaknyei.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3wkriudwd.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3tllsuhvd.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3srfsplko.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3kqhzcjfi.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3urdukghu.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3ikdssasw.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3ctuiagna.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3xawvjuto.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3scwkarvx.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3huebqsnu.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3kmageruh.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3qvubxpzf.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3dyulrpiy.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3jszqyfiq.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3tsottrlz.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3aamxwfme.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3lqbkksjq.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3owmetzqr.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3uuhmcjqq.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3jgfcfmkf.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3jnxpysnf.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3wjakkxzv.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3vvhewzjq.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3siugljxv.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3dvtvgwyx.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3idvbbsso.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3foucwhng.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3obtarmwf.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3xrvfszrl.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3xheghokl.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3jsmrigyb.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ololqdrp.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3pygpyzgm.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3eygujvle.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3offnthey.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3bmwfqsrw.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vcqmuraf.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3mmbarzfm.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3uvtdjhec.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3fbngyuyh.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3qyvzxdtv.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3snwgtete.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3eahcqwwy.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3mnwwarrl.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3iszqjmtt.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3qqntfnzc.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3bzdrbaay.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3blcvprfr.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3qmmqfclu.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3ifezjgyj.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3lrhtyzro.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3aegpwfuo.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3dlywgmmx.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3bhetytbn.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3ukbpogfj.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3bwscoabf.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3nfieumig.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3indetabj.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3cnmgatxp.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3hhubbfvl.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3usyqgzru.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3ahhfemoj.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3uuftdvmh.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3euoullin.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3lbxbfune.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3nzyzofre.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3qcfalmcg.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3hxigjpql.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3pendpmsc.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3qvvngswc.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3gifvlufi.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3rvhthrdl.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3dizgcgff.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3mlzklexu.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3baljdfoy.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ibhlojbw.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3yyqnrvzg.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3yvpijxcr.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3spmgivjb.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3cmzrijap.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3mpzfizwb.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3eljlcdrs.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3rjyyglwh.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gnrcszvv.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3mrxjfirz.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3dtcjavbr.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3fmsglguz.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3wnnokyqk.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3xhctnsxt.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3hlafrbau.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3unxsgwmw.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3jwzrzzyo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mvdisqgv.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3lsllgjse.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lasrkllg.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3bvmrfruc.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3qngbnrdm.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3vfinndnh.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3mjqudgzs.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3ymriniav.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3iktztble.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3qrbovyzq.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3yfakdukk.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3voxblpai.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3jkptlksr.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3uxnljdee.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3ecqlrukm.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3dihpzcrg.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3jgxlgdxi.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3cmzkoqnn.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3bhcvzlmx.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3tnbrwydq.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3lgnpukdp.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3wmrgtxce.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3qdpzdfdj.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3jetyfyzf.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3kugycrjc.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3dddmybuv.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3ydfknmxc.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3gsoqpgzy.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3wrymnhdi.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3bxiiqazm.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3tizudzud.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3vnapdbvf.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3vhgaqvgg.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3wkselfsz.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3pcutsgbo.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3mubqjskm.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3aouapzes.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3pxhwzgqo.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3jwkivnhc.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3bfgvejqm.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3pcitpnmb.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3cbdgvcoi.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3jtnkspnx.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3monasytn.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3hzqoapzt.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ztmaemqm.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3uxcqthtn.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3cqixlybe.html


<!-- 参考信息 -->