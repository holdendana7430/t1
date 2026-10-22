代发 wailian999

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2nqgrsfjx.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2mqmrxnjb.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2gdntnnnd.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2dprxszqg.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gucbbrmf.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2qglgjebm.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2dutitnei.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2dqbctwsq.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2dvysulxz.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2wdctsfpi.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2dvxvmmov.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2qzpnyjmr.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2myheqiyy.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2srpxkxen.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2cafihsjr.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2izovealb.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2uuszeukv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kiccdkxy.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2mzfsspee.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bybnrsgx.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2dlehqjlk.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2ukypsoho.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2rdxjmhni.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2jjqtwbta.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2vqiqctvm.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2tqnkmhmc.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2qnnrzhzn.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2anlkrqgn.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2ywjygqxg.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2slwwkjoj.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2gygywajx.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2wucgvsml.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2jmksqbsr.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2esewbykb.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2hecufcsj.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2qrclbnhj.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2osmldlxu.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2nnolfrvr.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2nxdaxwmn.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2tsfqytbt.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2fxvabcso.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2kgqllfyy.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2lfhinumz.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2ivezxtaj.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2xwnqmjvf.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2zyntrepy.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2keecrelt.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2hfxmrkaz.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2rqgabhyo.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2fysumiyd.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2mjljmynx.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2wwmejkpa.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2hogvsxgm.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2hdobvbzz.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2xfgaymya.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2wvxwdytv.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2swyygexy.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2zspsliqx.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2hbdmnmth.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2wklqtzii.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2pzwbotcg.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2mmmpiiem.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2hpmiqlqj.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2qodocwea.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2cgblgvai.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2bkjxfulf.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2zhrmhgxy.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2xokpxhlo.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2yfifwpkq.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2alcxyvnk.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2xzlbzdzp.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2wjhpfhlj.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2tvjljlpk.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2wmyageip.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2qvcbbgst.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2duiqxhyt.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2rbwfwttb.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2hsssedwj.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2ugugjwue.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2qggxgmpe.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2zvjdtwrd.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2amefbkux.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2zjeescjd.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2cdehfgaa.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2styqeqsx.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2uzqclhza.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2olvtehzu.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2iuyfkmeu.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2hefxypoo.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2sucebjwq.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2mjlmzmrc.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2nwdyusbg.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2rlgtxtbe.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2bnuvaupg.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2ufrfrqdb.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2povkfrfm.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2ewbapbxi.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2bkiknnuw.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2ejelupkw.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2bdrawujk.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2srlsncor.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2ebrvvctg.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2qfzsirbe.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2tvmuwfwd.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2klbfzahf.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2zjsvxbam.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2mjdzjzad.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2ljnarelf.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2fiuqzyzd.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2vcmeksdu.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2oofwjewq.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2xsmtjnfq.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2hkqiywga.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2npkeaqgh.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2ufwccprc.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rhaeplad.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2jdwffxhx.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2kxrknohh.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2bdhdozrm.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2hwpaclrb.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2whafuyrd.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2lquopeik.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2tyarhfvm.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2hcivyfxq.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2vjarffnl.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2xggnbgxq.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2krvezyet.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2qsfthljp.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2jjbfunah.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2wywtqxnh.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2ngawqeia.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2yfdstodm.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2pirsskfq.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2qyscxjsz.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2doutbjrj.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2uhuvsija.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2idhtevll.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ceeatzrr.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2dpsfbpub.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2cuxllwun.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2icrmxecb.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2cljeuxej.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2dnroqpdc.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2aiocfmdr.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2phusyeml.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2xxmjdgfe.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vrezvxng.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2pbsoftje.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2tpecbiuf.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wphebicp.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2pynzllwt.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2cwlucvmg.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2fkxrmzar.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2hyjlihsa.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2kymwfgyz.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2ukyorfhw.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2jmatewqe.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2uichflwp.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2okeqeiwd.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2afffpuby.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2xglzfbem.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2rkgdoapw.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2wtulxeby.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2pkbptowk.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2ehrqatgl.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2hmbwkmct.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2rrfggkbf.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2vttjjdpm.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2qelhfbgr.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2cpejnhna.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2pjugfutn.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2jvvhowjg.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2wbmxwigu.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2xaexpdbp.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2cwdkmett.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2zsfpkvrq.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2zczjnjda.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2pzdkaltl.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2muztsrfi.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2djhbxvyu.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2agpdufsa.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2spfnjlij.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2lkdolsbf.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2iscqgjmx.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2rjssiqlg.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2qnqllsie.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2swrmdkur.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2gavfuylu.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2embpgylt.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2vacdcvxq.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2bfijhhuk.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2nsdcqonv.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2zshikpov.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2hszibybs.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2yuqfsmyn.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2jvgudaod.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2xvvgytrs.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2xcwreeyv.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2zfwmboey.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ojwwxejg.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jxiiiovr.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2mstfvrra.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ahcrkqhm.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xzqcysco.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2msswgpal.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2vsaeoeyt.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2gnszjdft.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2lxqsosqg.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2vcgrueie.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2gcpzwgwj.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2yqqckzmz.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ovfrlktz.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2ucawjrma.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2gjzprexs.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2qiquaowz.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2zugdgngj.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2cwuzravz.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2rjmhwaeq.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2cexerydr.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2pdmtwpcr.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2iwewwiwx.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2qtszfhmr.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2asvigmxz.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2hrvbmgwu.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2tebppesz.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2tigmlnze.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2cuzdxlqj.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2itbqkach.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2qnawaqfs.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2tztdmsps.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2fbthmoae.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2avoqqkqn.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2tflssitx.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2lckekiqf.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2vkltfplg.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2jgwzkitf.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2xiydzfud.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2ntkhzphg.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2onbyvifr.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2pmaswtgv.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2wngcetkk.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2avrymkyw.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2puzveepo.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2tidiuklw.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2ojpsbyhh.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2fiiajvhy.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2ldmzxgev.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2hpqajbqn.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2imninppf.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2fmwefmft.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2nigynwma.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2pmaosrrk.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2ufqppioz.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2ojyvwhyk.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2dtfueptv.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2hzatdadh.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2unennfmf.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2wksoytcz.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2vcitaoeb.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2dcmzgpkq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nohbldvp.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2qteueobb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hvtuzdxw.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2zxoqwqyk.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2ooaqapqd.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2hpkvrsgr.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2vyrvmlvk.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2knlcxpok.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2vgmcjqki.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2prehnfye.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2kuobiwem.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2mgucsbso.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2bhlgrzxa.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2qxwzpiiv.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2dgufadtg.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2vgbveluo.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2lgtpcubs.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2xmlazpaz.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2rueoguab.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2nomyckdg.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2mntotenn.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2igsddmtr.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2uipbbxiu.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2xfyargpi.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2bpfwupmg.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2rlffaadg.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2gbckmvzm.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2qmuqosmp.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2giegraxx.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2nwqortnl.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2guemeztv.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2voiktnrx.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2spibnysw.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2wywzqcww.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2xnmhtbsn.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2hsbnitxt.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2jwrmfwah.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2kxoaqtgi.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2bzaxjgve.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2blactlfu.html


<!-- 参考信息 -->