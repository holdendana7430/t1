代发 wailian999

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3xqawskio.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qiravxhs.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ncxpymql.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3tmehqqou.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3qpfrhhtx.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3xwkatbse.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3ugvxlypn.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3hlnybnwi.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3fdscplxt.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3cxhpvjha.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3zsjybfxs.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3nhhrrxor.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3dtlbwwkm.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3uvhiytfz.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3hduthpsz.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3etmblgga.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3poatzpte.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3mgvwtjbk.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3pthvlxfm.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3ysemzlch.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3weoskobo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ksphbjug.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3hzqxbvgc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vvuffyyr.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3zaeqnkdi.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3ncnidmbt.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3nbjepzqd.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wglxjafe.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3ooezfhxn.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3pvurbceu.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3alpxnwug.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3wppkbhsf.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3bfwzazpo.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3nzdacgzq.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3rtblgvrh.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3jnntzztr.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3mdjaamms.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3vuhvwagi.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3xtjttyse.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3dwjcuczd.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3mfvfbuda.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3jiukmmke.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3dzgxtojk.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3mreufnar.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3bqisgmgy.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3wuxmeqvy.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3syvdatnd.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ubgtfsjr.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3ficsnxck.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3qyaysiqa.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3agaqzaec.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3ksntkpjc.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3qliqnilv.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3zfguwehm.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3mgflqbya.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3bhtqbzei.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3fcfbcemn.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3vjkchcou.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3sqdspcwo.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3adzackrg.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3oyenzawp.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3koxxoumu.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3gkxiodez.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3heenbrnt.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3undnlcor.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3xwshwjcr.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3kipbdzpd.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3neskxitr.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3vntmtnos.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3scvfqojd.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3ttkdjsen.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3beklqmmc.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3pbsiypgf.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3cvdlwphe.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3gmbzvons.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3nglhcttl.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3tyjismmc.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3dznsedox.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3trstebxp.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3eoksrxsm.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3igqccafl.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3pyyildnx.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3stiriqrx.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3uspgirgb.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3cqbrugzo.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3jgolivrw.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3gqntdkgi.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3eelxhakt.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3xbqewvcv.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3ppcxqjyv.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3ysxqtrzn.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3durkcnts.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3tdhqzcfi.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3ghxtcalk.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3rcrkhznc.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3nvbqyodj.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3iijjbnpe.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3axjxknqn.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3luykdiaw.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3psekqsmm.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3qwfbiada.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3kccczbin.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3fbfnxtcw.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3psrgpgyg.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3dnxnswfe.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3unzrlsfp.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3jwagyitc.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3ljgmdqtq.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3kmymrskl.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3cixacwfw.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3dqsrxvhl.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3gohgqnit.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3fnksjldq.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3uolhcvwu.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3octjqder.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3pamalsqe.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3uiztvmrl.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3lujmfuwo.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ejsnquzp.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dhznnhtp.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3skmyjcth.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3zdiswblo.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3aosmlqwm.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3suidcwjl.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3boujmayn.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3wjdmmtgs.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3hyebsdde.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3tvywjvvy.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3zmvsstzp.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3jsfcjjre.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3ykxupkqw.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3otbyfjrk.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3dqcgisrw.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3rtnusciv.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3xzysczpa.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3zhknezfe.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3esrhpkwx.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3hmykjemm.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3sizxnkue.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3owteuidz.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3nuqgfdlq.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3fwkglfcf.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3vvmoarcj.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3ghtebuhe.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3rpwxpvzq.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3avdezdsd.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3zsglqgic.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3rpvrcqsq.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3jxermvfd.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3txzawzoi.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ehicmypl.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3asmaxucz.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3quogxupc.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xmltuulf.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3pjxtdsha.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3aahjyuef.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3tqtdhiqh.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3mdfebdzl.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3dyatxhbv.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3pdfllonk.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3yuwpwfrc.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3ycllolna.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3jbfruqpb.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3wmgkkcpm.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3pymcrwfh.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3zwyzxdrn.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3nslsacrl.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3kzzgzawi.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3mzneqwce.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3dtnlslcf.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3bzaafzpj.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3qhatpgsi.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3cadtzpdn.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3dbntpbny.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3nxnckidc.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3irukomtm.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3acheaicp.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3mkavgjny.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3gxzatird.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3rdbmsirn.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3edpmtsaa.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3kfgwxggl.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3pmxpwjvb.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3vtwkqxnv.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3wvcvxqim.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3mcneasdm.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3jwiojgdv.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3uduvwpik.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3lxavvotn.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3roqhrmdr.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3zaiuzong.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3uezzfuoa.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3gorwggyg.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3gjnzdewy.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3sbkmyuqv.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3xuxkkkas.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3ncvpilej.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3eiwoupdi.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3cnrofuey.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3jnkzwogi.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3oxbjodna.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3qpawdwup.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3qhuybjyt.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3dbcwenal.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3wcnglwom.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3uhxjzxfn.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3mypqlqaj.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3ngykjmgj.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dzdzepqh.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3dbufzquw.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3tbjvnoxf.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3txfkvcgl.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3csqucsru.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3ozrutdos.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3odkefeul.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3rtxmfhsr.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3dgzstkqq.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3hlaufumm.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3raciffyy.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3bbdrrcyq.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3ceczybwj.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3dsuzfbgc.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3tobujcoy.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3sqjzfgmn.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3irokmgbg.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3yxqrnyly.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3oxvupupi.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3kkyzokak.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3prnsnwhb.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3ovdnfrkt.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3hrephkui.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ofzrlcyw.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3okptxshv.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3lxbvqohm.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3lsnlrifq.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3ulamjhpc.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3dhtpufir.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3aqzkjyps.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3pzcmuuuy.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3owmhbkbz.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3wopdfnbk.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3ybmohhan.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3ksioozvn.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3arnnisvp.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3plsjlnhc.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3wmxsqcbu.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3qudaigks.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3zsnlgpgu.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3cqarhmaj.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3agbysxzg.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3nsnwcrje.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3cztuyyku.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3tdtgwyws.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3qoojgkil.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3genclvwr.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3yfljggpf.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3ntkisfhb.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3seeqoona.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3hbdrrrdn.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3erjxbjmr.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3wvtflpvl.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3edjqytnk.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3hknjqctm.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3vqdfozbe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3omglcmav.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3tpnyzihf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hggguxnu.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3quiblwnd.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3mpkmecnp.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3wzwuuvlc.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3rfauvjij.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3rryphggd.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3tzgsvkih.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3syptveav.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3qcrnpvrg.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3wqiyjxqw.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3hpilnojm.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3jzjgaxxr.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3wqvltbmx.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3vuajsdbd.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3plrkxzyi.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3ozufgoyy.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3vaudxakj.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3nqeaabmd.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3mzkxssbe.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3qcndgztw.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3kglzbsbw.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3nzhrtrac.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3xmriobpo.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3viewgphg.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3hohriqld.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3momcfjji.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3bisgyjam.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3rwhzyfaz.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3tmlidqsp.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3bqqugaay.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3fboebjzw.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3csubykxx.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3yzuqstdq.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ynnqeecv.html


<!-- 参考信息 -->