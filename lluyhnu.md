代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.fanxiaobao.xyz/Article/details/gwalyopqh.sHtML

[T59] Scala：循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghiloeexf.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/galjzyxqt.sHtML

[T60] Scala：折叠
来源：http://blog.fanxiaobao.xyz/Article/details/gonnobghy.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpfjjhbty.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gntrpkgjj.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gvfkcfknc.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gvxktklsh.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.fanxiaobao.xyz/Article/details/guiadactk.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjtdxqysx.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.fanxiaobao.xyz/Article/details/golxmzdcq.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gheubltgs.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fanxiaobao.xyz/Article/details/gbetzyfiz.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.fanxiaobao.xyz/Article/details/gnfgkaljp.sHtML

[U04] Py：变量调试打印
来源：http://3g.fanxiaobao.xyz/Article/details/gqmqbtqoy.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fanxiaobao.xyz/Article/details/gntlgukdb.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.fanxiaobao.xyz/Article/details/gptgopxpf.sHtML

list(dict.fromkeys(arr))
来源：http://blog.fanxiaobao.xyz/Article/details/gbsszqcog.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glbaziaok.sHtML

{**a, **b}
来源：http://baike.fanxiaobao.xyz/Article/details/gdexzyqiu.sHtML

[U07] Py：反转字典键值
来源：http://read.share.fanxiaobao.xyz/Article/details/gphojbghg.sHtML

{v: k for k, v in d.items()}
来源：http://3g.fanxiaobao.xyz/Article/details/gtngwhpoy.sHtML

[U08] Py：展平二维列表
来源：http://wap.fanxiaobao.xyz/Article/details/gudagvttz.sHtML

[y for x in nested for y in x]
来源：http://www.share.fanxiaobao.xyz/Article/details/gybedwcas.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.fanxiaobao.xyz/Article/details/gmyqvjsry.sHtML

max(d, key=d.get)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjhwgfwrt.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grdgrrlzf.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.fanxiaobao.xyz/Article/details/gbgvbeuab.sHtML

[U11] Py：生成器表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gphpnalko.sHtML

(x * 2 for x in arr)
来源：http://wap.fanxiaobao.xyz/Article/details/gaxoksnuu.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.fanxiaobao.xyz/Article/details/gwomxnvov.sHtML

Counter(arr).most_common(3)
来源：http://baike.fanxiaobao.xyz/Article/details/gwwuihqdg.sHtML

[U13] Py：固定长度队列
来源：http://www.share.fanxiaobao.xyz/Article/details/gbabxurxj.sHtML

deque(maxlen=10)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggdjakiso.sHtML

[U14] Py：分组收集到列表
来源：http://3g.fanxiaobao.xyz/Article/details/glpmgifih.sHtML

defaultdict(list)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpsbwkbtl.sHtML

[U15] Py：高精度计时
来源：http://m.share.fanxiaobao.xyz/Article/details/giaivahgn.sHtML

t = time.perf_counter()
来源：http://blog.fanxiaobao.xyz/Article/details/gkprysbpn.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqyookab.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.fanxiaobao.xyz/Article/details/ghoubsqxa.sHtML

[U17] Py：初始化日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gdnohmibc.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.fanxiaobao.xyz/Article/details/gdsnrxonk.sHtML

[U18] Py：预编译正则
来源：http://www.share.fanxiaobao.xyz/Article/details/gqlhyebaz.sHtML

pat = re.compile(r"\d+")
来源：http://blog.fanxiaobao.xyz/Article/details/gdlhiynuj.sHtML

[U19] Py：正则替换带回调
来源：http://wap.fanxiaobao.xyz/Article/details/gpknebzkc.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.fanxiaobao.xyz/Article/details/gptqeaonl.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.fanxiaobao.xyz/Article/details/gkmnxzgpa.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwdseetjj.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.fanxiaobao.xyz/Article/details/ghcijwwsz.sHtML

@contextlib.contextmanager
来源：http://read.share.fanxiaobao.xyz/Article/details/gvkxkoqrm.sHtML

[U22] Py：矩阵转置
来源：http://read.share.fanxiaobao.xyz/Article/details/gwunelicq.sHtML

list(zip(*m))
来源：http://wap.fanxiaobao.xyz/Article/details/gqltjztqq.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxmhhppxw.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.fanxiaobao.xyz/Article/details/gipvpfcsk.sHtML

[U24] Py：路径操作
来源：http://wap.fanxiaobao.xyz/Article/details/gbgyfzjot.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.fanxiaobao.xyz/Article/details/guxtniasl.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.fanxiaobao.xyz/Article/details/gvefongrz.sHtML

csv.DictReader(f)
来源：http://blog.fanxiaobao.xyz/Article/details/gxoxhfuyx.sHtML

[U26] Py：并发下载
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnkhscofd.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxajbmzim.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.fanxiaobao.xyz/Article/details/goohnuolf.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.fanxiaobao.xyz/Article/details/gicbasttx.sHtML

[U28] Py：类型别名
来源：http://www.share.fanxiaobao.xyz/Article/details/gkgvjstrz.sHtML

UserId = int
来源：http://blog.fanxiaobao.xyz/Article/details/gfuglkjqg.sHtML

[U29] Py：属性校验
来源：http://www.share.fanxiaobao.xyz/Article/details/greueatna.sHtML

@property 与 @x.setter 配合
来源：http://3g.fanxiaobao.xyz/Article/details/gjuwqoszm.sHtML

[U30] Py：数据类
来源：http://read.share.fanxiaobao.xyz/Article/details/gricsqqud.sHtML

@dataclass(slots=True)
来源：http://wap.fanxiaobao.xyz/Article/details/gmvsfwvwr.sHtML

[U31] Py：单测
来源：http://3g.fanxiaobao.xyz/Article/details/gaasyhwfu.sHtML

python -m pytest -q
来源：http://m.share.fanxiaobao.xyz/Article/details/gwsmqelnl.sHtML

[U32] Py：代码格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gurpbludx.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnitldxxm.sHtML

[U33] Py：打包发布
来源：http://m.share.fanxiaobao.xyz/Article/details/gzcvavwdw.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.fanxiaobao.xyz/Article/details/gjcbwryid.sHtML

[U34] Py：判断编码
来源：http://m.share.fanxiaobao.xyz/Article/details/gmkxgyfcp.sHtML

chardet.detect(raw)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwcughnrr.sHtML

[U35] Py：发送邮件
来源：http://baike.fanxiaobao.xyz/Article/details/gkftnmbzb.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.fanxiaobao.xyz/Article/details/gksojkgsu.sHtML

[U36] Py：定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/guykpvpji.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.fanxiaobao.xyz/Article/details/gbjwkihtt.sHtML

[U37] Py：读写 Excel
来源：http://mobile.fanxiaobao.xyz/Article/details/gpaiiesvd.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.fanxiaobao.xyz/Article/details/glpubrwiv.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.fanxiaobao.xyz/Article/details/gtqdwmqzf.sHtML

Path(__file__).resolve().parent
来源：http://wap.fanxiaobao.xyz/Article/details/grqnlqyzx.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.fanxiaobao.xyz/Article/details/gwfparfyl.sHtML

sys.stdout.isatty()
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghfvmbuyw.sHtML

[U40] Py：打印到标准错误
来源：http://wap.fanxiaobao.xyz/Article/details/gtsplhafg.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtipbyesj.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.fanxiaobao.xyz/Article/details/gaoshhqmi.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.fanxiaobao.xyz/Article/details/gmhsjthgm.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.fanxiaobao.xyz/Article/details/gfbklzwtw.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gshaqbskn.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjjgjcyxg.sHtML

namespace App\Http;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmylczldb.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdqlnbfug.sHtML

declare(strict_types=1);
来源：http://wap.fanxiaobao.xyz/Article/details/gkhcchxne.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.fanxiaobao.xyz/Article/details/gkanequys.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtnqjeyhk.sHtML

[U46] PHP：可空类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gocpshgiw.sHtML

?string $name = null
来源：http://read.share.fanxiaobao.xyz/Article/details/gzezcjnlj.sHtML

[U47] PHP：联合类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gncilsbbw.sHtML

int|string $id
来源：http://m.share.fanxiaobao.xyz/Article/details/gvfoljaac.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/geyoqhkkg.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gfqovnrai.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbgkujbct.sHtML

public readonly string $name
来源：http://wap.fanxiaobao.xyz/Article/details/grubxbigd.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.fanxiaobao.xyz/Article/details/gkulekatb.sHtML

public function __construct(private int $id) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gxcjvgnyh.sHtML

[U51] PHP：数组解构
来源：http://www.share.fanxiaobao.xyz/Article/details/grrbaumpl.sHtML

[$a, $b] = $arr;
来源：http://mobile.fanxiaobao.xyz/Article/details/gcgnulpdh.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gafuuvgzo.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.fanxiaobao.xyz/Article/details/gdzdyoold.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxvwbemso.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.fanxiaobao.xyz/Article/details/gztiqeusb.sHtML

[U54] PHP：空安全调用
来源：http://3g.fanxiaobao.xyz/Article/details/gacjvizou.sHtML

$obj?->method()
来源：http://mobile.fanxiaobao.xyz/Article/details/gpbefpfvu.sHtML

[U55] PHP：match 表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gnofzrmwf.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.fanxiaobao.xyz/Article/details/gfcpaxtsf.sHtML

[U56] PHP：命名参数
来源：http://wap.fanxiaobao.xyz/Article/details/gzgxuypyz.sHtML

f(a: 1, b: 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkliiiige.sHtML

[U57] PHP：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gxpsmtyne.sHtML

"值: {$a}"
来源：http://baike.fanxiaobao.xyz/Article/details/gkqwrmtcc.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcwedinod.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.fanxiaobao.xyz/Article/details/gwreexqok.sHtML

[U59] PHP：自定义排序
来源：http://m.share.fanxiaobao.xyz/Article/details/glpaqkleq.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjjquzsii.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.fanxiaobao.xyz/Article/details/giwjomyuj.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.fanxiaobao.xyz/Article/details/gptwdgwln.sHtML

[U61] PHP：正则
来源：http://m.share.fanxiaobao.xyz/Article/details/gvonufmdm.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmupglppg.sHtML

[U62] PHP：日期对象
来源：http://www.share.fanxiaobao.xyz/Article/details/gnfcebrcy.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.fanxiaobao.xyz/Article/details/gttohwpnz.sHtML

[U63] PHP：文件读写
来源：http://read.share.fanxiaobao.xyz/Article/details/gfmzxmlye.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmltjkwic.sHtML

[U64] PHP：目录遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gqgmcdatc.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.fanxiaobao.xyz/Article/details/gcyumzltn.sHtML

[U65] PHP：会话
来源：http://read.share.fanxiaobao.xyz/Article/details/gbpkivkyu.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gydremgpn.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.fanxiaobao.xyz/Article/details/gqtlmwkqa.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gymwzejug.sHtML

[U67] PHP：处理文件上传
来源：http://wap.fanxiaobao.xyz/Article/details/gmfysifkt.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.fanxiaobao.xyz/Article/details/ggozqkyce.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gclxwqcnt.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.fanxiaobao.xyz/Article/details/ghjmqmvqm.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.fanxiaobao.xyz/Article/details/gofiygmmd.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.fanxiaobao.xyz/Article/details/gggyzntyw.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gtzfioruk.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.fanxiaobao.xyz/Article/details/grihjgsyr.sHtML

[U71] PHP：抛出异常
来源：http://3g.fanxiaobao.xyz/Article/details/ganskoqxk.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.fanxiaobao.xyz/Article/details/glpthnmxf.sHtML

[U72] PHP：写错误日志
来源：http://blog.fanxiaobao.xyz/Article/details/gttoeqbhi.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.fanxiaobao.xyz/Article/details/gzaknjblq.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.fanxiaobao.xyz/Article/details/gvvlpcaan.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwrczrnci.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gprfyrjat.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.fanxiaobao.xyz/Article/details/gbjcwwpyy.sHtML

[U75] PHP：依赖注入
来源：http://www.share.fanxiaobao.xyz/Article/details/gjzldnrhj.sHtML

composer require psr/container
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwxorpafw.sHtML

[U76] PHP：简单路由
来源：http://baike.fanxiaobao.xyz/Article/details/gdyjsnzlx.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.fanxiaobao.xyz/Article/details/gazdwtbtx.sHtML

[U77] PHP：模板渲染
来源：http://wap.fanxiaobao.xyz/Article/details/ggdganhuf.sHtML

composer require twig/twig
来源：http://blog.fanxiaobao.xyz/Article/details/geexlimcr.sHtML

[U78] PHP：单元测试
来源：http://3g.fanxiaobao.xyz/Article/details/gnrygefim.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.fanxiaobao.xyz/Article/details/gynlkibti.sHtML

[U79] PHP：静态分析
来源：http://wap.fanxiaobao.xyz/Article/details/gpquhljzd.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.fanxiaobao.xyz/Article/details/gcwutnbvr.sHtML

[U80] PHP：代码规范修复
来源：http://3g.fanxiaobao.xyz/Article/details/gsudghtaw.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.fanxiaobao.xyz/Article/details/gbznsjmrp.sHtML

[U81] JS：初始化项目
来源：http://read.share.fanxiaobao.xyz/Article/details/gysvpqzfv.sHtML

npm init -y;  npm i express
来源：http://mobile.fanxiaobao.xyz/Article/details/gxtpamfbh.sHtML

[U82] JS：package.json 脚本
来源：http://wap.fanxiaobao.xyz/Article/details/gpmusjblt.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.fanxiaobao.xyz/Article/details/guzhpxyaj.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbpeiqhrz.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.fanxiaobao.xyz/Article/details/gtkbcboem.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.fanxiaobao.xyz/Article/details/gsaviuquv.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.fanxiaobao.xyz/Article/details/geqigbtbx.sHtML

[U85] JS：可选链
来源：http://www.blog.fanxiaobao.xyz/Article/details/gabdmlhws.sHtML

a?.b?.c
来源：http://baike.fanxiaobao.xyz/Article/details/gswlntyef.sHtML

[U86] JS：空值合并
来源：http://read.share.fanxiaobao.xyz/Article/details/gvtxyrlvu.sHtML

a ?? b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gafycvpiu.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guqyfmqny.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.fanxiaobao.xyz/Article/details/gxqqputkk.sHtML

[U88] JS：对象展开合并
来源：http://baike.fanxiaobao.xyz/Article/details/glgzfialr.sHtML

{ ...a, ...b }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdkrdknaj.sHtML

[U89] JS：数组去重
来源：http://www.share.fanxiaobao.xyz/Article/details/gkdkmcpif.sHtML

[...new Set(arr)]
来源：http://blog.fanxiaobao.xyz/Article/details/gsfgrbppa.sHtML

[U90] JS：数字数组排序
来源：http://blog.fanxiaobao.xyz/Article/details/gginpcnht.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqcxflooh.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grglhojah.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.fanxiaobao.xyz/Article/details/gjdnhxrby.sHtML

[U92] JS：深拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gvibnzbtd.sHtML

structuredClone(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/gjhvcpiyt.sHtML

[U93] JS：模板字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gpqwheppu.sHtML

`共 ${n} 条`
来源：http://baike.fanxiaobao.xyz/Article/details/glmoftkpc.sHtML

[U94] JS：箭头函数
来源：http://baike.fanxiaobao.xyz/Article/details/gfjxzoxsq.sHtML

const double = x => x * 2;
来源：http://3g.fanxiaobao.xyz/Article/details/garmnglgz.sHtML

[U95] JS：Promise 包装
来源：http://blog.fanxiaobao.xyz/Article/details/golcqnguu.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gllingdij.sHtML

[U96] JS：async/await 与异常
来源：http://wap.fanxiaobao.xyz/Article/details/gxedqrrte.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjgkbcevs.sHtML

[U97] JS：并发请求
来源：http://3g.fanxiaobao.xyz/Article/details/guhjtlafy.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guedxvrmw.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdvhmnzla.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.fanxiaobao.xyz/Article/details/gjbgelhxt.sHtML

[U99] JS：事件监听
来源：http://wap.fanxiaobao.xyz/Article/details/gkgdyizha.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwixgcudu.sHtML

[U100] JS：DOM 查询
来源：http://blog.fanxiaobao.xyz/Article/details/gkeefsucm.sHtML

document.querySelector(".item")
来源：http://wap.fanxiaobao.xyz/Article/details/gyauvywfn.sHtML

[U101] JS：classList 操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gxkrsumcq.sHtML

el.classList.toggle("active")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghtjusedi.sHtML

[U102] JS：本地存储
来源：http://www.share.fanxiaobao.xyz/Article/details/gwboytkis.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.fanxiaobao.xyz/Article/details/gcnjkulmr.sHtML

[U103] JS：定时器
来源：http://read.share.fanxiaobao.xyz/Article/details/gnjbwzyxx.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.fanxiaobao.xyz/Article/details/gckdrqbdp.sHtML

[U104] JS：防抖
来源：http://3g.fanxiaobao.xyz/Article/details/glwzrmhtw.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fanxiaobao.xyz/Article/details/guwhiiotc.sHtML

[U105] JS：节流
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtsonwzad.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/grqvcinny.sHtML

[U106] JS：日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gjtwhhwtt.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gucllkgzl.sHtML

[U107] JS：数字千分位
来源：http://read.share.fanxiaobao.xyz/Article/details/gqiejxrhe.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohqdwnsv.sHtML

[U108] JS：随机整数
来源：http://read.share.fanxiaobao.xyz/Article/details/glpytmslx.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.fanxiaobao.xyz/Article/details/gsngzvqxp.sHtML

[U109] JS：数组分组
来源：http://www.share.fanxiaobao.xyz/Article/details/gjsmolfng.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.fanxiaobao.xyz/Article/details/gaeztgked.sHtML

[U110] JS：数组分块
来源：http://www.share.fanxiaobao.xyz/Article/details/gqgwamtgr.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.fanxiaobao.xyz/Article/details/gxpxqcwzz.sHtML

[U111] JS：对象转 Map
来源：http://mobile.fanxiaobao.xyz/Article/details/ghfcwozff.sHtML

new Map(Object.entries(obj))
来源：http://blog.fanxiaobao.xyz/Article/details/grukxmwyz.sHtML

[U112] JS：字符串补位
来源：http://mobile.fanxiaobao.xyz/Article/details/gvdvkgnpr.sHtML

"7".padStart(3, "0")
来源：http://wap.fanxiaobao.xyz/Article/details/gscqvkykr.sHtML

[U113] JS：正则替换全部
来源：http://mobile.fanxiaobao.xyz/Article/details/gotmihxyy.sHtML

s.replaceAll("a", "b")
来源：http://baike.fanxiaobao.xyz/Article/details/gkmxfcoes.sHtML

[U114] JS：JSON 深比较
来源：http://baike.fanxiaobao.xyz/Article/details/gulhggaaq.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fanxiaobao.xyz/Article/details/gpkoumltu.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqqulbvyp.sHtML

crypto.randomUUID()
来源：http://m.share.fanxiaobao.xyz/Article/details/gxmeqnwst.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.fanxiaobao.xyz/Article/details/ghatnfnbd.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwxbsmwh.sHtML

[U117] JS：单元测试
来源：http://3g.fanxiaobao.xyz/Article/details/geazzgkxl.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.fanxiaobao.xyz/Article/details/gdwkmblwp.sHtML

[U118] JS：开发服务器
来源：http://read.share.fanxiaobao.xyz/Article/details/gdpqnurev.sHtML

npm i -D vite;  npx vite
来源：http://mobile.fanxiaobao.xyz/Article/details/gwewbwcro.sHtML

[U119] JS：生产构建
来源：http://www.share.fanxiaobao.xyz/Article/details/gbelsxhon.sHtML

npx vite build
来源：http://3g.fanxiaobao.xyz/Article/details/gkwzqzbtd.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.fanxiaobao.xyz/Article/details/gaobenmyp.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.fanxiaobao.xyz/Article/details/grexiujeh.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gsrafjmuf.sHtML

统计汇总
来源：http://wap.fanxiaobao.xyz/Article/details/gxwsiqthb.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gsbbfxkyo.sHtML

按语言统计（条）：
来源：http://blog.fanxiaobao.xyz/Article/details/gqwmhwplx.sHtML

Python ......... 252
来源：http://blog.fanxiaobao.xyz/Article/details/gzqjictap.sHtML

PHP ............ 252
来源：http://3g.fanxiaobao.xyz/Article/details/gvatytnmq.sHtML

JavaScript ..... 252
来源：http://m.share.fanxiaobao.xyz/Article/details/gerfutmfy.sHtML

TypeScript ..... 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwweqrjuz.sHtML

Java ........... 212
来源：http://blog.fanxiaobao.xyz/Article/details/gazasjkpg.sHtML

Go ............. 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gppdhdvcb.sHtML

Ruby ........... 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvhlldlgv.sHtML

C# ............. 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gbdngwmrb.sHtML

C .............. 30
来源：http://wap.fanxiaobao.xyz/Article/details/gpyhqobjg.sHtML

C++ ............ 30
来源：http://m.share.fanxiaobao.xyz/Article/details/guyctpvzi.sHtML

SQL ............ 90
来源：http://m.share.fanxiaobao.xyz/Article/details/grylycrex.sHtML

Bash ........... 80
来源：http://m.share.fanxiaobao.xyz/Article/details/gfpeikvft.sHtML

Kotlin ......... 15
来源：http://read.share.fanxiaobao.xyz/Article/details/ghnqxqtxq.sHtML

Swift .......... 15
来源：http://www.share.fanxiaobao.xyz/Article/details/gxztfzlkj.sHtML

Lua ............ 10
来源：http://www.share.fanxiaobao.xyz/Article/details/giavomwvi.sHtML

Perl ........... 10
来源：http://3g.fanxiaobao.xyz/Article/details/gxnymkeil.sHtML

Scala .......... 10
来源：http://baike.fanxiaobao.xyz/Article/details/gownuxbyf.sHtML

------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/gesdmqipk.sHtML

合计 ........... 2106 条
来源：http://mobile.fanxiaobao.xyz/Article/details/gcvkcwwyr.sHtML

按章节统计：
来源：http://wap.fanxiaobao.xyz/Article/details/grtwirsgm.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.fanxiaobao.xyz/Article/details/glbvzupvl.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.fanxiaobao.xyz/Article/details/gaplcanxu.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.fanxiaobao.xyz/Article/details/grokvtsam.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.fanxiaobao.xyz/Article/details/glfaybjyv.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.fanxiaobao.xyz/Article/details/gmlmllcoi.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.fanxiaobao.xyz/Article/details/gwtjrzuml.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.fanxiaobao.xyz/Article/details/gzsizpkre.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.fanxiaobao.xyz/Article/details/gvjeqshhs.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/gkbdyegev.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.fanxiaobao.xyz/Article/details/gfycjcymd.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/grrvgqogs.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gkroanfuz.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/ghphmfhac.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.fanxiaobao.xyz/Article/details/gozmcrbsb.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.fanxiaobao.xyz/Article/details/gyoetmrbd.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/ghdoncoex.sHtML

Q SQL 专题                              90
来源：http://www.blog.fanxiaobao.xyz/Article/details/gababfuzc.sHtML

R Bash 专题                             80
来源：http://blog.fanxiaobao.xyz/Article/details/gcqsxpbwo.sHtML

S C / C++ 专题                          60
来源：http://www.share.fanxiaobao.xyz/Article/details/glochzzac.sHtML

T 其他语言补充                          60
来源：http://www.share.fanxiaobao.xyz/Article/details/gdeegqazm.sHtML

U 高频实用片段                         120
来源：http://blog.fanxiaobao.xyz/Article/details/gfjbhygbo.sHtML

------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/gndwpisva.sHtML

合计                                  2106 条
来源：http://mobile.fanxiaobao.xyz/Article/details/gvzalltkn.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/gquazcekj.sHtML

使用提醒
来源：http://read.share.fanxiaobao.xyz/Article/details/ggyfoaeyz.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/gjbrmshyu.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.fanxiaobao.xyz/Article/details/gdwrlvdhq.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giyxzuljs.sHtML


<!-- 参考信息 -->