代发 wailian999

[U01] Py：创建虚拟环境
来源：http://read.share.fanxiaobao.xyz/Article/details/giatradot.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.fanxiaobao.xyz/Article/details/ghrjmvzwy.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fanxiaobao.xyz/Article/details/gxdwkvlis.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.fanxiaobao.xyz/Article/details/grfzfmdxv.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.fanxiaobao.xyz/Article/details/gqwyllwux.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.fanxiaobao.xyz/Article/details/gskkwdyfr.sHtML

[U04] Py：变量调试打印
来源：http://baike.fanxiaobao.xyz/Article/details/gfazktaqx.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fanxiaobao.xyz/Article/details/gfbayiodf.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.fanxiaobao.xyz/Article/details/gmwwdxglf.sHtML

list(dict.fromkeys(arr))
来源：http://wap.fanxiaobao.xyz/Article/details/giwmqygmf.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gerqmitfa.sHtML

{**a, **b}
来源：http://3g.fanxiaobao.xyz/Article/details/gsjskyvcz.sHtML

[U07] Py：反转字典键值
来源：http://wap.fanxiaobao.xyz/Article/details/gvogjqewu.sHtML

{v: k for k, v in d.items()}
来源：http://blog.fanxiaobao.xyz/Article/details/grvklyjnd.sHtML

[U08] Py：展平二维列表
来源：http://blog.fanxiaobao.xyz/Article/details/gnmanzsws.sHtML

[y for x in nested for y in x]
来源：http://www.share.fanxiaobao.xyz/Article/details/gmvsftwdr.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwimyvfaw.sHtML

max(d, key=d.get)
来源：http://baike.fanxiaobao.xyz/Article/details/gvskljqxi.sHtML

[U10] Py：按值排序字典
来源：http://baike.fanxiaobao.xyz/Article/details/gtaqycvtk.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.fanxiaobao.xyz/Article/details/guktcuuvk.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjtmlnwo.sHtML

(x * 2 for x in arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gnltivdcf.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.fanxiaobao.xyz/Article/details/ghinblksi.sHtML

Counter(arr).most_common(3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gruuhwsry.sHtML

[U13] Py：固定长度队列
来源：http://blog.fanxiaobao.xyz/Article/details/gtnnxdzir.sHtML

deque(maxlen=10)
来源：http://wap.fanxiaobao.xyz/Article/details/gtqsedkrr.sHtML

[U14] Py：分组收集到列表
来源：http://3g.fanxiaobao.xyz/Article/details/gerfcjtrj.sHtML

defaultdict(list)
来源：http://www.blog.fanxiaobao.xyz/Article/details/getczsjve.sHtML

[U15] Py：高精度计时
来源：http://baike.fanxiaobao.xyz/Article/details/gfeikrufw.sHtML

t = time.perf_counter()
来源：http://baike.fanxiaobao.xyz/Article/details/gmwoctdnl.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fanxiaobao.xyz/Article/details/glmyczcms.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnembvzkk.sHtML

[U17] Py：初始化日志
来源：http://wap.fanxiaobao.xyz/Article/details/gwawirnnc.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.fanxiaobao.xyz/Article/details/gihtdxmen.sHtML

[U18] Py：预编译正则
来源：http://m.share.fanxiaobao.xyz/Article/details/gkwatmqvc.sHtML

pat = re.compile(r"\d+")
来源：http://wap.fanxiaobao.xyz/Article/details/gublhikle.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.fanxiaobao.xyz/Article/details/gkpmyevqz.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.fanxiaobao.xyz/Article/details/gtwtyqook.sHtML

[U20] Py：缓存函数结果
来源：http://3g.fanxiaobao.xyz/Article/details/gqpcmwrpb.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.fanxiaobao.xyz/Article/details/gamyudtbi.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.fanxiaobao.xyz/Article/details/gusrcmoiw.sHtML

@contextlib.contextmanager
来源：http://baike.fanxiaobao.xyz/Article/details/gpkoaykep.sHtML

[U22] Py：矩阵转置
来源：http://wap.fanxiaobao.xyz/Article/details/gtzexzuzp.sHtML

list(zip(*m))
来源：http://wap.fanxiaobao.xyz/Article/details/gdcxccehs.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gchpvyhme.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnxvxgryz.sHtML

[U24] Py：路径操作
来源：http://wap.fanxiaobao.xyz/Article/details/gggqtlobe.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/gegxaqcwp.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gppdrkhtg.sHtML

csv.DictReader(f)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpqqaexpm.sHtML

[U26] Py：并发下载
来源：http://wap.fanxiaobao.xyz/Article/details/grciivouo.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.fanxiaobao.xyz/Article/details/ghxhjurad.sHtML

[U27] Py：异步 HTTP
来源：http://3g.fanxiaobao.xyz/Article/details/gbinzbddf.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guukqdmaa.sHtML

[U28] Py：类型别名
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqnpaitsd.sHtML

UserId = int
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghaugjhml.sHtML

[U29] Py：属性校验
来源：http://read.share.fanxiaobao.xyz/Article/details/gkdnndnse.sHtML

@property 与 @x.setter 配合
来源：http://baike.fanxiaobao.xyz/Article/details/ghhsafuzt.sHtML

[U30] Py：数据类
来源：http://mobile.fanxiaobao.xyz/Article/details/gkclbfsxf.sHtML

@dataclass(slots=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmjkpijkd.sHtML

[U31] Py：单测
来源：http://baike.fanxiaobao.xyz/Article/details/gbwgsqajs.sHtML

python -m pytest -q
来源：http://baike.fanxiaobao.xyz/Article/details/gpzrvrfab.sHtML

[U32] Py：代码格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gbbxbwjpd.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.fanxiaobao.xyz/Article/details/gyftiaixw.sHtML

[U33] Py：打包发布
来源：http://www.share.fanxiaobao.xyz/Article/details/gmueifltm.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.fanxiaobao.xyz/Article/details/ghjyfipwz.sHtML

[U34] Py：判断编码
来源：http://blog.fanxiaobao.xyz/Article/details/grhmmbtdt.sHtML

chardet.detect(raw)
来源：http://3g.fanxiaobao.xyz/Article/details/gdgjxwwuj.sHtML

[U35] Py：发送邮件
来源：http://www.blog.fanxiaobao.xyz/Article/details/giiiendhx.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghzkiluin.sHtML

[U36] Py：定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gleyxspqa.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gugngtvcm.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwxneohts.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.fanxiaobao.xyz/Article/details/gmhzfaizr.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.fanxiaobao.xyz/Article/details/gssmejczb.sHtML

Path(__file__).resolve().parent
来源：http://wap.fanxiaobao.xyz/Article/details/gsdngspvd.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.fanxiaobao.xyz/Article/details/gcttxiyiw.sHtML

sys.stdout.isatty()
来源：http://3g.fanxiaobao.xyz/Article/details/gkedltrtw.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.fanxiaobao.xyz/Article/details/gftiqckjq.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwdxevgzf.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.fanxiaobao.xyz/Article/details/gfebrfslp.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.fanxiaobao.xyz/Article/details/gfulfxwlu.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.fanxiaobao.xyz/Article/details/gfcfwchjl.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggbpcntmu.sHtML

[U43] PHP：声明命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/gutybhbct.sHtML

namespace App\Http;
来源：http://mobile.fanxiaobao.xyz/Article/details/gsicrnusc.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkocmewyi.sHtML

declare(strict_types=1);
来源：http://wap.fanxiaobao.xyz/Article/details/gscxxzszc.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gosqpqvtj.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkkuudetd.sHtML

[U46] PHP：可空类型
来源：http://blog.fanxiaobao.xyz/Article/details/gkzgfjuom.sHtML

?string $name = null
来源：http://3g.fanxiaobao.xyz/Article/details/ggjiuiiqu.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gspkvdxae.sHtML

int|string $id
来源：http://m.share.fanxiaobao.xyz/Article/details/guxymogxk.sHtML

[U48] PHP：纯枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gwagrxoyw.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gszcxxkgl.sHtML

[U49] PHP：只读属性
来源：http://baike.fanxiaobao.xyz/Article/details/gloyeestl.sHtML

public readonly string $name
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsdrbkcpc.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.fanxiaobao.xyz/Article/details/gjatxvtib.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxrmalaep.sHtML

[U51] PHP：数组解构
来源：http://www.share.fanxiaobao.xyz/Article/details/gkmnyywoi.sHtML

[$a, $b] = $arr;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghlwhwbdy.sHtML

[U52] PHP：箭头函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gwutjtshj.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxcjtapgq.sHtML

[U53] PHP：空合并运算符
来源：http://wap.fanxiaobao.xyz/Article/details/gprpilgjn.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.fanxiaobao.xyz/Article/details/gisolxdpe.sHtML

[U54] PHP：空安全调用
来源：http://baike.fanxiaobao.xyz/Article/details/gysgfkdpx.sHtML

$obj?->method()
来源：http://read.share.fanxiaobao.xyz/Article/details/gylpgwomx.sHtML

[U55] PHP：match 表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gxewodfrl.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.fanxiaobao.xyz/Article/details/gskknucay.sHtML

[U56] PHP：命名参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gdjjwxiqp.sHtML

f(a: 1, b: 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gseoqepkq.sHtML

[U57] PHP：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmedfwxx.sHtML

"值: {$a}"
来源：http://wap.fanxiaobao.xyz/Article/details/gpnaltnif.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmezxsbdj.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkhsmjmqv.sHtML

[U59] PHP：自定义排序
来源：http://m.share.fanxiaobao.xyz/Article/details/grohoowon.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpswsfjji.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmvwiizpy.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.fanxiaobao.xyz/Article/details/gfwtbtpir.sHtML

[U61] PHP：正则
来源：http://m.share.fanxiaobao.xyz/Article/details/gftjdlexy.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.fanxiaobao.xyz/Article/details/gieabwekm.sHtML

[U62] PHP：日期对象
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmbzswxx.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.fanxiaobao.xyz/Article/details/glkugluxd.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gogfngwil.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.fanxiaobao.xyz/Article/details/giyibvphk.sHtML

[U64] PHP：目录遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gogoalgws.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.fanxiaobao.xyz/Article/details/gyzimcjdy.sHtML

[U65] PHP：会话
来源：http://m.share.fanxiaobao.xyz/Article/details/gyqxcbuag.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gkinzcvzv.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.fanxiaobao.xyz/Article/details/gtzlxsxpn.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.fanxiaobao.xyz/Article/details/gxfydptnl.sHtML

[U67] PHP：处理文件上传
来源：http://3g.fanxiaobao.xyz/Article/details/gnqwsbevf.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.fanxiaobao.xyz/Article/details/gljtmchrd.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqapfegua.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.fanxiaobao.xyz/Article/details/gucerxygd.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.fanxiaobao.xyz/Article/details/gnkklnxhu.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxryeohkn.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gikbtdfqn.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaclqavtk.sHtML

[U71] PHP：抛出异常
来源：http://3g.fanxiaobao.xyz/Article/details/grxhbfbpg.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grzkufduj.sHtML

[U72] PHP：写错误日志
来源：http://wap.fanxiaobao.xyz/Article/details/gowwfatgw.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glzqfizxg.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.fanxiaobao.xyz/Article/details/gxzphzvwo.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwuzdpehf.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gwnbbwhfo.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.fanxiaobao.xyz/Article/details/gxuaefgqd.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.fanxiaobao.xyz/Article/details/gegfgwkpi.sHtML

composer require psr/container
来源：http://mobile.fanxiaobao.xyz/Article/details/gwjntjyfa.sHtML

[U76] PHP：简单路由
来源：http://baike.fanxiaobao.xyz/Article/details/gcpyagcen.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.fanxiaobao.xyz/Article/details/ghzupxaxy.sHtML

[U77] PHP：模板渲染
来源：http://blog.fanxiaobao.xyz/Article/details/gbzjdqbev.sHtML

composer require twig/twig
来源：http://wap.fanxiaobao.xyz/Article/details/gngdetwrt.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gghhyxrmd.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.fanxiaobao.xyz/Article/details/glveaguyj.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsyadqufv.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.fanxiaobao.xyz/Article/details/genwojdnt.sHtML

[U80] PHP：代码规范修复
来源：http://wap.fanxiaobao.xyz/Article/details/gawxthngx.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnsydsvdu.sHtML

[U81] JS：初始化项目
来源：http://read.share.fanxiaobao.xyz/Article/details/gipkgqecz.sHtML

npm init -y;  npm i express
来源：http://wap.fanxiaobao.xyz/Article/details/gyobwtdit.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.fanxiaobao.xyz/Article/details/gwshtefeb.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.fanxiaobao.xyz/Article/details/gyorwdeij.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.fanxiaobao.xyz/Article/details/gbfnsgvdg.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.fanxiaobao.xyz/Article/details/girgkwgwz.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsyceggil.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.fanxiaobao.xyz/Article/details/gvlpwxxnj.sHtML

[U85] JS：可选链
来源：http://baike.fanxiaobao.xyz/Article/details/grhfsnuex.sHtML

a?.b?.c
来源：http://m.share.fanxiaobao.xyz/Article/details/gmgspswew.sHtML

[U86] JS：空值合并
来源：http://read.share.fanxiaobao.xyz/Article/details/gaozcgsrl.sHtML

a ?? b
来源：http://m.share.fanxiaobao.xyz/Article/details/guurhpsho.sHtML

[U87] JS：解构默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/gngtgxvjm.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjjmtfigy.sHtML

[U88] JS：对象展开合并
来源：http://baike.fanxiaobao.xyz/Article/details/gigtfxygq.sHtML

{ ...a, ...b }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggkaubjjm.sHtML

[U89] JS：数组去重
来源：http://mobile.fanxiaobao.xyz/Article/details/gnhczsqze.sHtML

[...new Set(arr)]
来源：http://read.share.fanxiaobao.xyz/Article/details/grbeeazni.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkklzmzwm.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gadlprsla.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gtzjrzkox.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.fanxiaobao.xyz/Article/details/gnceaswec.sHtML

[U92] JS：深拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gvrjnorot.sHtML

structuredClone(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjpkpaxpb.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmapbatcg.sHtML

`共 ${n} 条`
来源：http://m.share.fanxiaobao.xyz/Article/details/ggxunsegi.sHtML

[U94] JS：箭头函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gvmjkqxod.sHtML

const double = x => x * 2;
来源：http://3g.fanxiaobao.xyz/Article/details/gtxuiyfpc.sHtML

[U95] JS：Promise 包装
来源：http://www.share.fanxiaobao.xyz/Article/details/gkbjvqtsr.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.fanxiaobao.xyz/Article/details/gbazxrjir.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.fanxiaobao.xyz/Article/details/gcybgtuwu.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gpekxdgma.sHtML

[U97] JS：并发请求
来源：http://read.share.fanxiaobao.xyz/Article/details/glwacohph.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdtksqiqr.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.fanxiaobao.xyz/Article/details/gfniojwik.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.fanxiaobao.xyz/Article/details/gqxadkoog.sHtML

[U99] JS：事件监听
来源：http://baike.fanxiaobao.xyz/Article/details/giajqjfmo.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.fanxiaobao.xyz/Article/details/gesixmrvr.sHtML

[U100] JS：DOM 查询
来源：http://blog.fanxiaobao.xyz/Article/details/ggkkaaxji.sHtML

document.querySelector(".item")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcfmryesi.sHtML

[U101] JS：classList 操作
来源：http://mobile.fanxiaobao.xyz/Article/details/ggtrjwnrq.sHtML

el.classList.toggle("active")
来源：http://baike.fanxiaobao.xyz/Article/details/gmtclzigd.sHtML

[U102] JS：本地存储
来源：http://mobile.fanxiaobao.xyz/Article/details/gmqyzlrmk.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.fanxiaobao.xyz/Article/details/gaxijgkuu.sHtML

[U103] JS：定时器
来源：http://wap.fanxiaobao.xyz/Article/details/gugmllwlr.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.fanxiaobao.xyz/Article/details/gvtyrinsm.sHtML

[U104] JS：防抖
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqreqklvk.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/grizzpbqe.sHtML

[U105] JS：节流
来源：http://blog.fanxiaobao.xyz/Article/details/gtzqgnzfh.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gntqdcelm.sHtML

[U106] JS：日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gbnlsbzho.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.fanxiaobao.xyz/Article/details/gviynlgjs.sHtML

[U107] JS：数字千分位
来源：http://m.share.fanxiaobao.xyz/Article/details/gmjvgdvbr.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.fanxiaobao.xyz/Article/details/gwuwseflh.sHtML

[U108] JS：随机整数
来源：http://3g.fanxiaobao.xyz/Article/details/giracwutx.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.fanxiaobao.xyz/Article/details/ginwrihtv.sHtML

[U109] JS：数组分组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkusybcwf.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtsmjxwkp.sHtML

[U110] JS：数组分块
来源：http://baike.fanxiaobao.xyz/Article/details/gaamltiqw.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.fanxiaobao.xyz/Article/details/gzdnhdene.sHtML

[U111] JS：对象转 Map
来源：http://3g.fanxiaobao.xyz/Article/details/gymvjdrwo.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gccbutmxo.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/galulhsll.sHtML

"7".padStart(3, "0")
来源：http://blog.fanxiaobao.xyz/Article/details/gqninnxke.sHtML

[U113] JS：正则替换全部
来源：http://wap.fanxiaobao.xyz/Article/details/gfztzlzra.sHtML

s.replaceAll("a", "b")
来源：http://read.share.fanxiaobao.xyz/Article/details/gzlxebegu.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gwlqvmhhd.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fanxiaobao.xyz/Article/details/glsrecoso.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glodhgspd.sHtML

crypto.randomUUID()
来源：http://blog.fanxiaobao.xyz/Article/details/glbuktnyb.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glrnmlhsz.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gaapbvkyg.sHtML

[U117] JS：单元测试
来源：http://wap.fanxiaobao.xyz/Article/details/gnkcuelwh.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.fanxiaobao.xyz/Article/details/gnqohusjw.sHtML

[U118] JS：开发服务器
来源：http://m.share.fanxiaobao.xyz/Article/details/gdroosypo.sHtML

npm i -D vite;  npx vite
来源：http://3g.fanxiaobao.xyz/Article/details/gvgdyoldi.sHtML

[U119] JS：生产构建
来源：http://blog.fanxiaobao.xyz/Article/details/gqksoqepv.sHtML

npx vite build
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsevnnzks.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.fanxiaobao.xyz/Article/details/girtvkjaz.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwysqndy.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glzxymncj.sHtML

统计汇总
来源：http://blog.fanxiaobao.xyz/Article/details/gtpinxipz.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/giueehmyp.sHtML

按语言统计（条）：
来源：http://baike.fanxiaobao.xyz/Article/details/gxxdcwqvf.sHtML

Python ......... 252
来源：http://3g.fanxiaobao.xyz/Article/details/gcpyzehak.sHtML

PHP ............ 252
来源：http://baike.fanxiaobao.xyz/Article/details/gfkbamomj.sHtML

JavaScript ..... 252
来源：http://www.share.fanxiaobao.xyz/Article/details/gjtopijlt.sHtML

TypeScript ..... 212
来源：http://m.share.fanxiaobao.xyz/Article/details/ggmsuaffo.sHtML

Java ........... 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmpdzxdjo.sHtML

Go ............. 212
来源：http://wap.fanxiaobao.xyz/Article/details/gtysdkdga.sHtML

Ruby ........... 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gbeowavrc.sHtML

C# ............. 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gdrvskkkz.sHtML

C .............. 30
来源：http://m.share.fanxiaobao.xyz/Article/details/gzuckzhka.sHtML

C++ ............ 30
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grdguujtj.sHtML

SQL ............ 90
来源：http://wap.fanxiaobao.xyz/Article/details/gfrtjiojo.sHtML

Bash ........... 80
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqxcxjvg.sHtML

Kotlin ......... 15
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggxykcasa.sHtML

Swift .......... 15
来源：http://m.share.fanxiaobao.xyz/Article/details/gwhqvfvoz.sHtML

Lua ............ 10
来源：http://3g.fanxiaobao.xyz/Article/details/gmvdapwew.sHtML

Perl ........... 10
来源：http://m.share.fanxiaobao.xyz/Article/details/giuxqlfry.sHtML

Scala .......... 10
来源：http://mobile.fanxiaobao.xyz/Article/details/gghwqtnfh.sHtML

------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzwflmkok.sHtML

合计 ........... 2106 条
来源：http://www.share.fanxiaobao.xyz/Article/details/ggofuaajj.sHtML

按章节统计：
来源：http://www.share.fanxiaobao.xyz/Article/details/givhjkhav.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.fanxiaobao.xyz/Article/details/gegiupnqv.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.fanxiaobao.xyz/Article/details/gdetbvrds.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.fanxiaobao.xyz/Article/details/gyhvgktzw.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.fanxiaobao.xyz/Article/details/gxjvfixys.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.fanxiaobao.xyz/Article/details/gqwnidhcm.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.fanxiaobao.xyz/Article/details/gkgqcoplj.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.fanxiaobao.xyz/Article/details/grccjkpuc.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.fanxiaobao.xyz/Article/details/gjlolhtwv.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnudugvds.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjhpfgnww.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/gzzmjesuk.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/gcyjctydo.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnnahutoy.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.fanxiaobao.xyz/Article/details/gkxtutbdo.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.fanxiaobao.xyz/Article/details/giclruflk.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/gpkymuxvr.sHtML

Q SQL 专题                              90
来源：http://read.share.fanxiaobao.xyz/Article/details/gwlimwezl.sHtML

R Bash 专题                             80
来源：http://blog.fanxiaobao.xyz/Article/details/gjtymjqmd.sHtML

S C / C++ 专题                          60
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvwcuxnhf.sHtML

T 其他语言补充                          60
来源：http://m.share.fanxiaobao.xyz/Article/details/gyhfiqezd.sHtML

U 高频实用片段                         120
来源：http://baike.fanxiaobao.xyz/Article/details/gckjknnpd.sHtML

------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/gjfbxjiwa.sHtML

合计                                  2106 条
来源：http://3g.fanxiaobao.xyz/Article/details/geajtkgbh.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gxrzgwqkq.sHtML

使用提醒
来源：http://mobile.fanxiaobao.xyz/Article/details/grkiksfig.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/gjtkikuqq.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpxrlopbd.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghwntovgi.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.fanxiaobao.xyz/Article/details/gtptvackw.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.fanxiaobao.xyz/Article/details/gfocsuygy.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.fanxiaobao.xyz/Article/details/gzwsaotem.sHtML

—— 文件结束 ——
来源：http://blog.fanxiaobao.xyz/Article/details/gbfdohobt.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gnuhzctkx.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbdcymeix.sHtML

Common Programming Examples Cheat Book
来源：http://3g.fanxiaobao.xyz/Article/details/gqnbcxdpq.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/godoedgqe.sHtML


<!-- 参考信息 -->