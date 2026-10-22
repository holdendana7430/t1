代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2htmooxxr.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2tckcrlly.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2moeukkkp.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2obsjbyia.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2wqytbpev.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2mqslottc.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2qwffvnkp.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2ujfenfje.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2xpnfudnw.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2qdcsbkaz.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2oanhczrl.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2ohyxgfkq.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2iiglvwif.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nbhyzbxs.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2iymoghhf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qzefjqhz.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2qxffihpo.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2wnanxjgf.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2vntawcnn.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hpqnpojv.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2iexvcjti.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2conflsoe.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2tlhilnma.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2kfxytrlm.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2pwmkqshh.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2lewuiegq.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2wpimhcif.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2sixnblsa.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2jnizdyqx.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2pkbvqjtl.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2zfxjcvxe.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2ezzakpct.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2mvjfqoyw.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2mvtkezog.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2vxpjenwo.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2ztnnpoga.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ovckkhog.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xyddqoem.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2mqcfjubw.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2kvgfhttr.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2wglptccy.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2tyoaivmk.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2lnhythcx.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2qvrfywma.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2jaivdqec.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2gchutqkd.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2ynmvpgnm.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2oujrwnfl.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2svcpkovc.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2jdnpzpld.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2liwpwhak.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2afxhlqhk.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2fmnmpzgb.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2okjvxnyn.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2ytnctdzm.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2tzrdxqnz.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2nneaqaym.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2qexzihly.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2mybirnkw.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2puchfddw.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2bkcjnjlh.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2ydwjgnzj.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2cfuiodsd.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2bwnypuhf.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2spsetwhf.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2lklfbtby.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2aoenuzkt.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2emqegwyf.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2maootslq.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2gvcqgwoo.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2bmabzgrg.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2fjedwnoo.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2zhkwewlw.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2jidgtnsz.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2sheqqyge.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2dpjpwulw.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2oznfhgpq.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2moqjvdyn.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ycgdlwnf.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2locxqhnm.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2hrweaqyi.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2juuaesxy.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2eyhmizwv.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2mdxkryqp.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2tqeaubdc.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2irfizwym.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2ijggxwqk.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2jsivgane.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2thpdxlgq.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2hutvrbic.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2kruxnrbb.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2brqguwqc.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2ktzyiqlf.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2ccpdotor.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2dkmwxqdm.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2gmjpfrgt.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2epsaoaap.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2lafmqefs.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2ddnyzqgg.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2mebyvzyv.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2fidhxwga.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2dbvhvaej.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2cpcqvxgw.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2qjwigrog.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2osethvar.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2jdjholqc.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2mdbkghat.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2ovrlsueo.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2rxharjjk.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2anvksdlb.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2aqrwsftm.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mjirjbsm.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2rtfxfjpy.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2prjdmtsf.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2cztjffcx.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2edyjntjk.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2lbazszia.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2jftuvhhg.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2trojbnag.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2jxzwyait.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2cmznvbru.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2hbpkjdxh.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2dcdvtvdx.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2sdhofkvi.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2dwhwdwmq.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2moipvcce.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2gisaumsq.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2waqlxfeb.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2qekrphol.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2gqdmbwze.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2ljhcjrvk.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2hsulkbzd.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2hsykefvr.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2gvuflnlz.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2bsigasdu.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2kjafzese.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2qkmdugkl.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2bixuvzbl.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2qrfzjbou.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2krukvzos.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2goagrbod.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2untbgibk.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2xkztnxyq.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2rekfzxoi.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2cfoqksoh.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2szudmobt.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2djvzjdtx.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2yeapcupw.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2dofjeugh.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2jkhqmkvm.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2tvejflyq.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2thslzrct.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2gtrwykmb.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2fvrftzyn.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2bjmetmhm.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2rnlzntwc.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2fqmfqdef.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2rtnafdps.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2igjhgjzw.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2ltldoqbq.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2qszenqrt.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2ufftnjjd.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2ykfhuvrq.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2bccxtnzk.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2urvsznbj.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2pocsebdq.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2ftfanslm.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2vloboxwt.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2cdbaiwlf.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2yiibqahf.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2eeighqzv.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2tpajscpb.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2aqsitjns.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2jjusmozx.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2ozyywtse.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2fingitmm.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2bojqgntn.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2hdccjamm.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2gatpspmu.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2bjqfxwbr.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2bkyceltq.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2braajnaq.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2vxyzhkht.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2qtwxpgoz.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2vwqqoqax.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2wcxwqjka.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2sjbpsorn.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2bzmhnbjg.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2peogqexb.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2cjgvfabs.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2mrrqutxy.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2nutjufgg.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2wsfqgoln.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2xyzevjjs.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2xyypedux.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2toxuserw.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2hlvaxwyf.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2iajwpjmp.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2oishelcq.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2afxsbicc.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2yqeecryq.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2raotmklt.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2pegdcfon.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2bzzipidj.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2thduvtjf.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2lrqxhpzc.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2swtwsxxz.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2xkvleunr.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2eurstoyv.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2fttexfqg.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2dmtvmwvi.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2qhqlknqm.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2pxhsfdou.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2zzsvsjaa.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2bdorovbi.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2usovkfbb.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2uqrnohlt.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2awqcdqyd.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2rqdeytbb.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2ketgsiwt.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2hathmqjt.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2muldksjt.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2iplnbsrd.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2mkxtocvr.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2rweygrhg.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2ibbcuvrx.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2fucnjgks.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2flpdrnqs.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2bdhvumkf.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2xyzehjxt.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2jftocgpq.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2iyjmfljb.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2jruzudvp.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2fgqariui.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2oywtuosy.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2lfkrtaiq.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2oydfzzgh.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2xptqruto.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2cdtqrfyw.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2xwpegwke.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2ymwfwpwe.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2tvcddkre.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2ynmmpaob.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2nxwhlqfu.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2axkiwtfq.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2zglpejml.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2wieibvkv.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2mcrnugzm.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2iwdtyozt.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2wvkxkyjr.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2iqkmurou.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2zmqizyya.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2senbbosd.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2yulkoigj.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2igdxyfuf.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2czovinmf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cyfckixm.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2eaapgbqr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hgnxagba.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2qjmewcul.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2sofuxzri.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2xoxfdhdt.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2csaslhdh.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2kskynkpf.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2ebdrxwju.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2qkbcmmym.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ajmdgkgv.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2igahoktv.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2qtkfhvwv.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2modggvio.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2kxrmlgmu.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2qaygfhjv.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2qesrchip.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2mvaomwqu.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2foeqeczq.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2dpvsirwz.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2hdpyngzt.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2vtydbshs.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2ukhyjhry.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2xawagesf.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2rvuendfl.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2uzxkliqv.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2fmjwmbvf.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2wzistsyy.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2nknfpiju.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2gragwtwu.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2bfdffzsc.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2gbqxghfw.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2qlpmuhgk.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2jhykkuwm.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ulclhxkr.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2qrokvydp.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2sqtpbgnk.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2djlyysqn.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2ofwwbnqq.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2criwqaxv.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2thvdwsts.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2jgsmcpqx.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2mdqplmcr.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2akwpfghn.html


<!-- 参考信息 -->