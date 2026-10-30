代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://baike.fehbvm.com/Article/details/ggkgthbew.sHtML

[T55] Scala：集合过滤
来源：http://blog.hesvh.cn/Article/details/gdrfpalbz.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.fehbvm.com/Article/details/gyqsigvkj.sHtML

[T56] Scala：样例类
来源：http://read.share.zdbjq.cn/Article/details/gmxhsbnfb.sHtML

case class User(name: String, age: Int)
来源：http://read.share.hesvh.cn/Article/details/gdbbiluxr.sHtML

[T57] Scala：模式匹配
来源：http://wap.fehbvm.com/Article/details/gvektbfzn.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.hesvh.cn/Article/details/guogtmpty.sHtML

[T58] Scala：函数定义
来源：http://m.share.zdbjq.cn/Article/details/gyssejhwb.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.zdbjq.cn/Article/details/gvomhjomq.sHtML

[T59] Scala：循环
来源：http://3g.fehbvm.com/Article/details/gkwreosxp.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.hesvh.cn/Article/details/gclrbfcnb.sHtML

[T60] Scala：折叠
来源：http://baike.hesvh.cn/Article/details/gylquayij.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.hesvh.cn/Article/details/ghrpnfwvy.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gsexpbwlb.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.hesvh.cn/Article/details/gycznpedc.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/grjycjglh.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.fehbvm.com/Article/details/gncxmlvcy.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.fehbvm.com/Article/details/gyleqqsmk.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.hesvh.cn/Article/details/gjngqojrv.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.fehbvm.com/Article/details/guunjqrrr.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.hesvh.cn/Article/details/gehuwfhrk.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.zdbjq.cn/Article/details/grmggnled.sHtML

[U04] Py：变量调试打印
来源：http://wap.zdbjq.cn/Article/details/gicgmggfu.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.zdbjq.cn/Article/details/goyrmtmva.sHtML

[U05] Py：列表去重且保序
来源：http://wap.hesvh.cn/Article/details/gygbjzhpk.sHtML

list(dict.fromkeys(arr))
来源：http://wap.fehbvm.com/Article/details/gbkfnfurr.sHtML

[U06] Py：合并两个字典
来源：http://m.share.zdbjq.cn/Article/details/gsanpwzfd.sHtML

{**a, **b}
来源：http://mobile.fehbvm.com/Article/details/gkxofrsog.sHtML

[U07] Py：反转字典键值
来源：http://3g.fehbvm.com/Article/details/gtmzxsceo.sHtML

{v: k for k, v in d.items()}
来源：http://3g.fehbvm.com/Article/details/gcxfeowta.sHtML

[U08] Py：展平二维列表
来源：http://blog.zdbjq.cn/Article/details/gevftzbfq.sHtML

[y for x in nested for y in x]
来源：http://www.blog.hesvh.cn/Article/details/gitbhlacn.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.hesvh.cn/Article/details/gjvwncxry.sHtML

max(d, key=d.get)
来源：http://blog.fehbvm.com/Article/details/gpbhneuqq.sHtML

[U10] Py：按值排序字典
来源：http://read.share.hesvh.cn/Article/details/gszvyedyh.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.zdbjq.cn/Article/details/gapchaxwp.sHtML

[U11] Py：生成器表达式
来源：http://mobile.zdbjq.cn/Article/details/gmcihehkz.sHtML

(x * 2 for x in arr)
来源：http://m.share.fehbvm.com/Article/details/gbcnrukun.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.fehbvm.com/Article/details/gdfcjnpak.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.hesvh.cn/Article/details/gzswfcxzz.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.fehbvm.com/Article/details/gdbnegfvz.sHtML

deque(maxlen=10)
来源：http://www.blog.zdbjq.cn/Article/details/gkgfuvnvj.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.zdbjq.cn/Article/details/gdrlurbth.sHtML

defaultdict(list)
来源：http://www.share.hesvh.cn/Article/details/gtdqjpunm.sHtML

[U15] Py：高精度计时
来源：http://read.share.hesvh.cn/Article/details/gohkxvqbg.sHtML

t = time.perf_counter()
来源：http://www.m.share.zdbjq.cn/Article/details/gzvmxfrbs.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.fehbvm.com/Article/details/gryamksre.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.zdbjq.cn/Article/details/ggwokubxh.sHtML

[U17] Py：初始化日志
来源：http://baike.hesvh.cn/Article/details/gamgikyzx.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.hesvh.cn/Article/details/gbunqpavt.sHtML

[U18] Py：预编译正则
来源：http://blog.hesvh.cn/Article/details/gpaopeenj.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.hesvh.cn/Article/details/gwttvrogi.sHtML

[U19] Py：正则替换带回调
来源：http://blog.hesvh.cn/Article/details/gpwlzaeth.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.hesvh.cn/Article/details/grbpljogw.sHtML

[U20] Py：缓存函数结果
来源：http://3g.hesvh.cn/Article/details/gexceszzf.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.zdbjq.cn/Article/details/gzzthwzvj.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.fehbvm.com/Article/details/gzcidtjol.sHtML

@contextlib.contextmanager
来源：http://m.share.hesvh.cn/Article/details/gdoapqimf.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.zdbjq.cn/Article/details/gdppvuepw.sHtML

list(zip(*m))
来源：http://mobile.hesvh.cn/Article/details/glyutdzhp.sHtML

[U23] Py：分块读取大文件
来源：http://blog.hesvh.cn/Article/details/grcwjyuxl.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.hesvh.cn/Article/details/gxhbnqzej.sHtML

[U24] Py：路径操作
来源：http://www.m.share.hesvh.cn/Article/details/gxlgwxsnr.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.zdbjq.cn/Article/details/gvskulhns.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.hesvh.cn/Article/details/glqianmid.sHtML

csv.DictReader(f)
来源：http://mobile.hesvh.cn/Article/details/gkbfgjmep.sHtML

[U26] Py：并发下载
来源：http://www.share.hesvh.cn/Article/details/gqxglxxgm.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.fehbvm.com/Article/details/gtkaxdzih.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.hesvh.cn/Article/details/grouuppob.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.zdbjq.cn/Article/details/gsyxlhjmm.sHtML

[U28] Py：类型别名
来源：http://read.share.zdbjq.cn/Article/details/gxsymabxw.sHtML

UserId = int
来源：http://wap.zdbjq.cn/Article/details/gcylqpkdi.sHtML

[U29] Py：属性校验
来源：http://www.blog.fehbvm.com/Article/details/giiyymnhe.sHtML

@property 与 @x.setter 配合
来源：http://3g.fehbvm.com/Article/details/gluubkkca.sHtML

[U30] Py：数据类
来源：http://baike.hesvh.cn/Article/details/grvqfmqit.sHtML

@dataclass(slots=True)
来源：http://baike.fehbvm.com/Article/details/ggrwgqmwr.sHtML

[U31] Py：单测
来源：http://read.share.hesvh.cn/Article/details/gwkksbjcc.sHtML

python -m pytest -q
来源：http://m.share.fehbvm.com/Article/details/gshzidxrg.sHtML

[U32] Py：代码格式化
来源：http://wap.hesvh.cn/Article/details/gxhxxktnd.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.fehbvm.com/Article/details/ghcpnhdxa.sHtML

[U33] Py：打包发布
来源：http://blog.zdbjq.cn/Article/details/ggiwkckte.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.zdbjq.cn/Article/details/gmreuqrnl.sHtML

[U34] Py：判断编码
来源：http://www.m.share.zdbjq.cn/Article/details/gfeuenahr.sHtML

chardet.detect(raw)
来源：http://www.blog.hesvh.cn/Article/details/gcipyujuv.sHtML

[U35] Py：发送邮件
来源：http://read.share.hesvh.cn/Article/details/gabsqwssa.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.hesvh.cn/Article/details/gbawwbdiy.sHtML

[U36] Py：定时任务
来源：http://m.share.zdbjq.cn/Article/details/gcxlvbkat.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.zdbjq.cn/Article/details/ggvmtmlqz.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.fehbvm.com/Article/details/gewcesoay.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.fehbvm.com/Article/details/gwahcjpqq.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.hesvh.cn/Article/details/gttsvvypw.sHtML

Path(__file__).resolve().parent
来源：http://3g.zdbjq.cn/Article/details/glmbnriwy.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.zdbjq.cn/Article/details/gmxrxdlhb.sHtML

sys.stdout.isatty()
来源：http://3g.hesvh.cn/Article/details/gjjeoeotd.sHtML

[U40] Py：打印到标准错误
来源：http://3g.fehbvm.com/Article/details/gadubnrvc.sHtML

print("err", file=sys.stderr)
来源：http://www.share.hesvh.cn/Article/details/gxnxjlyfn.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.fehbvm.com/Article/details/gjyqcvrea.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.fehbvm.com/Article/details/gpxvszuya.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.fehbvm.com/Article/details/gqmexsdol.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.hesvh.cn/Article/details/gqfndsbgu.sHtML

[U43] PHP：声明命名空间
来源：http://3g.zdbjq.cn/Article/details/gfrxautef.sHtML

namespace App\Http;
来源：http://www.blog.zdbjq.cn/Article/details/guxzsofgb.sHtML

[U44] PHP：开启严格类型
来源：http://wap.fehbvm.com/Article/details/ghohjxnvc.sHtML

declare(strict_types=1);
来源：http://blog.zdbjq.cn/Article/details/gutpztiaw.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.zdbjq.cn/Article/details/gkjplamqo.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/gybhdizvu.sHtML

[U46] PHP：可空类型
来源：http://www.blog.fehbvm.com/Article/details/giyngbyis.sHtML

?string $name = null
来源：http://3g.fehbvm.com/Article/details/gtoktusxx.sHtML

[U47] PHP：联合类型
来源：http://mobile.hesvh.cn/Article/details/gnbtwpchy.sHtML

int|string $id
来源：http://blog.zdbjq.cn/Article/details/ghsgixguq.sHtML

[U48] PHP：纯枚举
来源：http://m.share.hesvh.cn/Article/details/gghqnhogc.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.fehbvm.com/Article/details/gelssisgl.sHtML

[U49] PHP：只读属性
来源：http://www.share.fehbvm.com/Article/details/gtarevyvz.sHtML

public readonly string $name
来源：http://www.share.zdbjq.cn/Article/details/gakznzwwz.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.zdbjq.cn/Article/details/ghqkqndxu.sHtML

public function __construct(private int $id) {}
来源：http://read.share.fehbvm.com/Article/details/gjcolblad.sHtML

[U51] PHP：数组解构
来源：http://blog.hesvh.cn/Article/details/gbntybvik.sHtML

[$a, $b] = $arr;
来源：http://mobile.fehbvm.com/Article/details/gskxvnhvk.sHtML

[U52] PHP：箭头函数
来源：http://read.share.fehbvm.com/Article/details/gmespsnrq.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.fehbvm.com/Article/details/gnrkcmaht.sHtML

[U53] PHP：空合并运算符
来源：http://blog.zdbjq.cn/Article/details/gpbbjhvjm.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.fehbvm.com/Article/details/gopqfwtxf.sHtML

[U54] PHP：空安全调用
来源：http://wap.hesvh.cn/Article/details/gclguftam.sHtML

$obj?->method()
来源：http://m.share.fehbvm.com/Article/details/gufhgcmft.sHtML

[U55] PHP：match 表达式
来源：http://www.share.zdbjq.cn/Article/details/geaweqero.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.hesvh.cn/Article/details/gzmgebnxm.sHtML

[U56] PHP：命名参数
来源：http://wap.fehbvm.com/Article/details/gtnezlasa.sHtML

f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/gbzvpukrc.sHtML

[U57] PHP：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gwrfrdgjy.sHtML

"值: {$a}"
来源：http://mobile.fehbvm.com/Article/details/gwjflzemx.sHtML

[U58] PHP：数组三件套
来源：http://3g.zdbjq.cn/Article/details/gavrucxvy.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.fehbvm.com/Article/details/ghehcnwsr.sHtML

[U59] PHP：自定义排序
来源：http://mobile.fehbvm.com/Article/details/grasjefmw.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gknpyspqo.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.hesvh.cn/Article/details/grovzacml.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.fehbvm.com/Article/details/gnjgbsgkg.sHtML

[U61] PHP：正则
来源：http://baike.zdbjq.cn/Article/details/gidejcomn.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.fehbvm.com/Article/details/gemjivier.sHtML

[U62] PHP：日期对象
来源：http://m.share.fehbvm.com/Article/details/gycewmhzx.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.zdbjq.cn/Article/details/gzbwzrjav.sHtML

[U63] PHP：文件读写
来源：http://blog.fehbvm.com/Article/details/gjpekxlqt.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.zdbjq.cn/Article/details/gogkdayjd.sHtML

[U64] PHP：目录遍历
来源：http://read.share.fehbvm.com/Article/details/ggfsdjgzk.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.zdbjq.cn/Article/details/gwekthimc.sHtML

[U65] PHP：会话
来源：http://www.m.share.hesvh.cn/Article/details/gajbfbpvl.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.hesvh.cn/Article/details/gwmuugvru.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.hesvh.cn/Article/details/gxqtuuuhg.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.fehbvm.com/Article/details/gyftmtazq.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.zdbjq.cn/Article/details/gswmoxjpv.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.hesvh.cn/Article/details/gawvqrkbt.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.fehbvm.com/Article/details/gcflkuwjd.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.fehbvm.com/Article/details/gowqkehyo.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.hesvh.cn/Article/details/gtsnlywvx.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.zdbjq.cn/Article/details/gsafiauwm.sHtML

[U70] PHP：PDO 事务
来源：http://3g.zdbjq.cn/Article/details/giqdtxqqe.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.hesvh.cn/Article/details/gkukwuevf.sHtML

[U71] PHP：抛出异常
来源：http://3g.zdbjq.cn/Article/details/gtjsfzvdh.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.fehbvm.com/Article/details/gkldsggcf.sHtML

[U72] PHP：写错误日志
来源：http://3g.hesvh.cn/Article/details/glohapxdn.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.zdbjq.cn/Article/details/gnrvmzskm.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.hesvh.cn/Article/details/ghnvfcwrx.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.fehbvm.com/Article/details/gqvqknpjl.sHtML

[U74] PHP：读取环境变量
来源：http://wap.hesvh.cn/Article/details/gfeosvqsm.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.hesvh.cn/Article/details/gtjmceatr.sHtML

[U75] PHP：依赖注入
来源：http://wap.fehbvm.com/Article/details/gettcxsxi.sHtML

composer require psr/container
来源：http://3g.hesvh.cn/Article/details/gavjraxnn.sHtML

[U76] PHP：简单路由
来源：http://www.blog.zdbjq.cn/Article/details/guhryroik.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.fehbvm.com/Article/details/glbdrcmcu.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.fehbvm.com/Article/details/gahvidndd.sHtML

composer require twig/twig
来源：http://wap.hesvh.cn/Article/details/gspqdbujp.sHtML

[U78] PHP：单元测试
来源：http://m.share.hesvh.cn/Article/details/gitcvudfi.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.fehbvm.com/Article/details/gjpbzyjpl.sHtML

[U79] PHP：静态分析
来源：http://read.share.zdbjq.cn/Article/details/goothfkeo.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.fehbvm.com/Article/details/gtntqaccz.sHtML

[U80] PHP：代码规范修复
来源：http://wap.zdbjq.cn/Article/details/gmcevqcje.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.zdbjq.cn/Article/details/gtzyxbhon.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.hesvh.cn/Article/details/ggvkhszli.sHtML

npm init -y;  npm i express
来源：http://www.share.fehbvm.com/Article/details/gadcunbwz.sHtML

[U82] JS：package.json 脚本
来源：http://3g.hesvh.cn/Article/details/gjnmrlrib.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.zdbjq.cn/Article/details/gnxqtwbeu.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.fehbvm.com/Article/details/goozktlgi.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.zdbjq.cn/Article/details/grgduenol.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.hesvh.cn/Article/details/gxekvdmds.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.zdbjq.cn/Article/details/geaorcruq.sHtML

[U85] JS：可选链
来源：http://read.share.hesvh.cn/Article/details/gaicavqae.sHtML

a?.b?.c
来源：http://read.share.hesvh.cn/Article/details/gwydknpdf.sHtML

[U86] JS：空值合并
来源：http://www.share.zdbjq.cn/Article/details/gavghhyca.sHtML

a ?? b
来源：http://baike.zdbjq.cn/Article/details/gpbsoarvu.sHtML

[U87] JS：解构默认值
来源：http://read.share.zdbjq.cn/Article/details/goobuidie.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.hesvh.cn/Article/details/gurkvclcd.sHtML

[U88] JS：对象展开合并
来源：http://wap.hesvh.cn/Article/details/gxeifnxej.sHtML

{ ...a, ...b }
来源：http://3g.zdbjq.cn/Article/details/gephalhqc.sHtML

[U89] JS：数组去重
来源：http://wap.hesvh.cn/Article/details/gmycuatgz.sHtML

[...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/ghpapztjc.sHtML

[U90] JS：数字数组排序
来源：http://blog.fehbvm.com/Article/details/gezsjblpb.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gjuyyregx.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.hesvh.cn/Article/details/glpmlvyou.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.fehbvm.com/Article/details/gjerxjimo.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gnrmiblgb.sHtML

structuredClone(obj)
来源：http://read.share.fehbvm.com/Article/details/gczcductt.sHtML

[U93] JS：模板字符串
来源：http://baike.hesvh.cn/Article/details/gcighxdvx.sHtML

`共 ${n} 条`
来源：http://3g.hesvh.cn/Article/details/gyjxxebbt.sHtML

[U94] JS：箭头函数
来源：http://m.share.zdbjq.cn/Article/details/glfwzlhbp.sHtML

const double = x => x * 2;
来源：http://blog.fehbvm.com/Article/details/gacfkbkaa.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.hesvh.cn/Article/details/gqknngctv.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.fehbvm.com/Article/details/gdjhqrrhy.sHtML

[U96] JS：async/await 与异常
来源：http://3g.zdbjq.cn/Article/details/gawnnldus.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/glqojonxz.sHtML

[U97] JS：并发请求
来源：http://m.share.fehbvm.com/Article/details/gfpacjmto.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gpghbiocu.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.fehbvm.com/Article/details/gsduopgjo.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.zdbjq.cn/Article/details/gsraadahv.sHtML

[U99] JS：事件监听
来源：http://www.blog.fehbvm.com/Article/details/gfnwpqpyo.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.fehbvm.com/Article/details/gbyrdpeao.sHtML

[U100] JS：DOM 查询
来源：http://blog.hesvh.cn/Article/details/ghkhoyowq.sHtML

document.querySelector(".item")
来源：http://blog.hesvh.cn/Article/details/gzercegdj.sHtML

[U101] JS：classList 操作
来源：http://baike.fehbvm.com/Article/details/gptyjzvlu.sHtML

el.classList.toggle("active")
来源：http://read.share.hesvh.cn/Article/details/gpfigiusv.sHtML

[U102] JS：本地存储
来源：http://baike.zdbjq.cn/Article/details/gofmsjrxl.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.zdbjq.cn/Article/details/grusvqrcr.sHtML

[U103] JS：定时器
来源：http://www.blog.fehbvm.com/Article/details/gyavlgnvq.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.hesvh.cn/Article/details/gncvrtaiu.sHtML

[U104] JS：防抖
来源：http://blog.zdbjq.cn/Article/details/gnetribes.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gkppxavxe.sHtML

[U105] JS：节流
来源：http://read.share.fehbvm.com/Article/details/gxueobttq.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.hesvh.cn/Article/details/gyinmplof.sHtML

[U106] JS：日期格式化
来源：http://baike.zdbjq.cn/Article/details/glkqrmqbp.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.zdbjq.cn/Article/details/gsqcnknbl.sHtML

[U107] JS：数字千分位
来源：http://read.share.zdbjq.cn/Article/details/gdoyqotxp.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.fehbvm.com/Article/details/gwnyakibc.sHtML

[U108] JS：随机整数
来源：http://m.share.zdbjq.cn/Article/details/gblwfnqei.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.zdbjq.cn/Article/details/guiykzazv.sHtML

[U109] JS：数组分组
来源：http://m.share.zdbjq.cn/Article/details/gfmtarhjg.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.hesvh.cn/Article/details/gmpwzdjmb.sHtML

[U110] JS：数组分块
来源：http://www.blog.zdbjq.cn/Article/details/gwxiaxbtj.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.fehbvm.com/Article/details/gyrgowdtu.sHtML

[U111] JS：对象转 Map
来源：http://baike.zdbjq.cn/Article/details/gwqugfwyq.sHtML

new Map(Object.entries(obj))
来源：http://mobile.zdbjq.cn/Article/details/gbbrvpevo.sHtML

[U112] JS：字符串补位
来源：http://blog.fehbvm.com/Article/details/glphnlpzv.sHtML

"7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gyedumeci.sHtML

[U113] JS：正则替换全部
来源：http://m.share.fehbvm.com/Article/details/gkxghqrcw.sHtML

s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gechgzkue.sHtML

[U114] JS：JSON 深比较
来源：http://baike.fehbvm.com/Article/details/glbeglkjc.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fehbvm.com/Article/details/gfemgoeew.sHtML

[U115] JS：生成 UUID
来源：http://baike.hesvh.cn/Article/details/gibyjctsf.sHtML

crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/gvlhyknvv.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.zdbjq.cn/Article/details/gkwmuvpbk.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.hesvh.cn/Article/details/gqsobfvqk.sHtML

[U117] JS：单元测试
来源：http://wap.hesvh.cn/Article/details/glzzyzhhb.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.zdbjq.cn/Article/details/gmdhysbhk.sHtML

[U118] JS：开发服务器
来源：http://wap.hesvh.cn/Article/details/gefrjtisk.sHtML

npm i -D vite;  npx vite
来源：http://mobile.hesvh.cn/Article/details/gvowbdthp.sHtML

[U119] JS：生产构建
来源：http://mobile.fehbvm.com/Article/details/gisfwfkxj.sHtML

npx vite build
来源：http://www.m.share.fehbvm.com/Article/details/gfgicfzeg.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.zdbjq.cn/Article/details/gcvpncjea.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.zdbjq.cn/Article/details/giiidnsyh.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gplumqyvt.sHtML

统计汇总
来源：http://3g.fehbvm.com/Article/details/gbxvoxrxx.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gsnimirhd.sHtML

按语言统计（条）：
来源：http://3g.fehbvm.com/Article/details/gtepgjkgh.sHtML

Python ......... 252
来源：http://baike.fehbvm.com/Article/details/gelzgropc.sHtML

PHP ............ 252
来源：http://blog.fehbvm.com/Article/details/ghumcmlon.sHtML

JavaScript ..... 252
来源：http://wap.fehbvm.com/Article/details/gspoyvnsk.sHtML

TypeScript ..... 212
来源：http://wap.hesvh.cn/Article/details/gwcvrzfls.sHtML

Java ........... 212
来源：http://baike.hesvh.cn/Article/details/gskatronw.sHtML

Go ............. 212
来源：http://3g.fehbvm.com/Article/details/gcamvysgo.sHtML

Ruby ........... 212
来源：http://www.m.share.fehbvm.com/Article/details/gbeaopthc.sHtML

C# ............. 212
来源：http://read.share.hesvh.cn/Article/details/gsktsazhv.sHtML

C .............. 30
来源：http://www.m.share.fehbvm.com/Article/details/gxohluzkr.sHtML

C++ ............ 30
来源：http://baike.zdbjq.cn/Article/details/gcjxqwbjg.sHtML

SQL ............ 90
来源：http://www.share.hesvh.cn/Article/details/gqmaukszz.sHtML

Bash ........... 80
来源：http://www.m.share.hesvh.cn/Article/details/gfmudlten.sHtML

Kotlin ......... 15
来源：http://blog.hesvh.cn/Article/details/gekqeykjj.sHtML

Swift .......... 15
来源：http://3g.zdbjq.cn/Article/details/grdzjmhld.sHtML

Lua ............ 10
来源：http://wap.zdbjq.cn/Article/details/givrjannt.sHtML

Perl ........... 10
来源：http://www.share.zdbjq.cn/Article/details/glvmvycpt.sHtML

Scala .......... 10
来源：http://mobile.hesvh.cn/Article/details/gybutvqri.sHtML

------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gklneadzw.sHtML

合计 ........... 2106 条
来源：http://www.m.share.fehbvm.com/Article/details/ghayfayyx.sHtML

按章节统计：
来源：http://mobile.hesvh.cn/Article/details/gccljtlwr.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.fehbvm.com/Article/details/gzjmdipyv.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/glwnvvyob.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.zdbjq.cn/Article/details/gsumknhjv.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.zdbjq.cn/Article/details/gjyqmrcro.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.fehbvm.com/Article/details/gyzudbdhm.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.zdbjq.cn/Article/details/gpsvmzeaw.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.hesvh.cn/Article/details/gwbzcjloc.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.zdbjq.cn/Article/details/girwcndly.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/giuwzqpyg.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.fehbvm.com/Article/details/gtwqwiabc.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gyhytidda.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gajbtjgde.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gixxuinzh.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.fehbvm.com/Article/details/glojhlbsm.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.fehbvm.com/Article/details/gcunkxftu.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gufeabulz.sHtML

Q SQL 专题                              90
来源：http://mobile.zdbjq.cn/Article/details/gwavmixls.sHtML

R Bash 专题                             80
来源：http://wap.hesvh.cn/Article/details/gzfoniqjy.sHtML

S C / C++ 专题                          60
来源：http://baike.hesvh.cn/Article/details/gsznnjkit.sHtML

T 其他语言补充                          60
来源：http://wap.zdbjq.cn/Article/details/gtsmpvxzd.sHtML


<!-- 参考信息 -->