代发 wailian999

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2mbgveyug.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lejvjhnr.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2kpeqbycm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aeokcpon.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2zpqzqhyi.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2uhvoyixa.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2ztkivdew.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2efhocgwt.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2wzdikxkd.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2maeuktuq.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2nieveevf.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2qwainxem.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2tpjzsgdb.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2yzmiisib.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2bpzrjxpu.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2vlczkfcc.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2iuebtemf.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2zqoglbfy.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2iebakjji.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2ibjsockt.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2zswfywgi.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2xjmepvod.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2xewhqtwh.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2iegurozg.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2qxkshjrm.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2pjexyxpw.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2wsfvidkh.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2zqzccncp.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2mtvwfewi.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2albrphlp.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2oravsxby.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2iodnniod.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2igaduncd.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2qhdzavhl.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2wszarofr.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2tmdzvfcx.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2fkimvqje.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2qtqzjzkl.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2rtdtrzkp.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2sjxavtlt.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2yjnxtbzx.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2dahmtsod.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2mxglmfcf.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2qirqkvlt.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2rvzrjynu.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2fblmbgjx.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2azyyauei.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2zkthkglu.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2pedoqxoa.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2lpnvgjpb.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2dtoeuqpx.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2klgwrpjp.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2tgmblrrt.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2pszdwplp.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2usfybegx.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2hueqitan.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2rulbyukh.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2vgswgjym.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2exvgenmu.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2xtgcsods.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2htsajulu.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2amoqogng.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2ahualxyd.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2bkkodhoi.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2rlfiueda.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2jjmravfk.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2uflpfhbo.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2fqitqulv.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2baveefft.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2yqkjpddz.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2hjykgeru.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2eocervgd.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2vzckycif.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2jpqifmso.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2oihfxajo.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2krfqtdau.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2pspifnao.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2lnmjbdxp.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2dyibjjwb.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2arpwoujo.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2emlyawnp.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2onedyyva.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2jipzkaqi.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2gxbyebfb.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2jtwrpueh.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2akxjdbye.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2sjffhmwr.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2zgjigvwq.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2uhlbmpmn.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2kqumyqlx.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2ofptxoox.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2hxsmxhhv.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2zweioxat.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2betcznwo.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2eyvuzeyf.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2jdpgtffi.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2xlcbjeqk.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2wsrzsakw.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2bngfmwsv.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2qykoomhr.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2jsquiqxj.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2tzxviyki.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2kqiptcaa.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ckgvxuxf.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2vvuqsjbw.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2nmtgernz.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2okhiejhg.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2ttpajzim.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2jfzsdyej.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2dehjamkx.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2jsiogbbt.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2ohzomaxc.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2mdmjzwjo.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2gxlgriew.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2rvgtwscl.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2deifgimj.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2uypzyitz.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2axaxkxdu.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2doogcgnw.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2ptcqbxut.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2kacthbbg.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2aktzhjfi.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2mgfztlwq.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ixmagazz.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2nsuwfqjl.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2dyyyjdzj.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2mwlwzhby.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2nbgihpwf.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2juhmvtpz.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2fsqeecfs.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2iwealspq.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2zorpnnvr.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2bnjqmrku.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2efjauomu.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2ncwjnkhm.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2nsgbujgy.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2lmainxra.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2fkoklwtl.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2zxofjvvj.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2jsusvfkw.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2ovdasprd.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2nonolpmf.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2zfgktexm.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2xroewnql.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2bstxypaf.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2goetdgok.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2hafvibvf.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2lojqqjfb.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2dpqbnvsg.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2ftcdxgab.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2qsapswnd.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2wkmazjjs.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2ywjtowaj.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2kbewwics.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2bvnpxkcv.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2ttjgtlhx.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2cofionqb.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2edzdqeaa.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2uimjubbc.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2qnfzgrdf.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2dvdnqbot.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2fxcaxxug.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2wwkybjyz.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2dlddyyvd.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2psrzmgmt.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2zzmplzge.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2kfyymcrz.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2dfznkgib.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2pxownkxs.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2elenpgsn.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2bamlptfx.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2uolhmiob.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2aynlgdyk.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2pofecxgd.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2ebrizzkw.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2gsmibabc.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2spxrdrdy.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2kmhdtwau.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2ekpryara.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2lekjqzlp.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2syeooltj.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2sasnezqd.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2lsvlafcd.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2poszatfz.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2erwknvvk.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2iflbkqpo.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2bnfdnzbv.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2quynennm.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2fjsdqhyt.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2vrkttvrh.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2upiehyum.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2kcamyjgx.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2etklqilt.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2zkybupcq.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2lgcmgalo.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2aveoawnv.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2alhjpuja.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2gehmzikc.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2sokonpee.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2nwqjbsiu.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2suzoqxgo.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2ulmdzujx.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2pqysycff.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2kkbqgfrr.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2jkvnonna.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2lidvahcj.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2mandsfah.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2fboxdarf.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2lcnxyzwk.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2iivuwdsl.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2lagejlmr.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2eytvhqoh.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2lwilywnu.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2vxcufuce.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2sjlxxldu.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2eaozuxom.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2zdsxrbgh.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2lydovmvs.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2beazvuox.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2woylvpqz.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2fllkfcfg.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2nuhjpyio.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2wyzcjhbh.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2qbchazfs.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2kofilpqw.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2bjsbinre.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2qkshypyx.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2vusnhimt.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2kpxizpmf.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2eidvgeya.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2iqhpdmyk.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2nyhbssrr.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2txpftare.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2qcihbejj.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2qmljrpui.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wlvqzrmj.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2kotocdvi.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2wrcsiqng.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2wqhcxycm.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2qjrvwema.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2wcjsxxlg.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2zmgqvrxc.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2npiyltax.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2hoebpmmf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zqtzxorh.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2uwsnxkbg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bknsiswi.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2odzncnjy.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2xwwzvduo.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2ezzvdvhh.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2owphmdmk.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2kymmkclj.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2jncxhxws.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2eaihxkkl.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2uofolqsu.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2yuttrwyb.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2ftxinvig.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2succqfnw.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2xerfzfcp.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2ldydenow.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2yevxsevc.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2pmqwvqnu.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2jvfvydyk.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2zshgetfr.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2poxwdeye.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2gaosefij.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2afdsgxbg.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2oobikrea.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2lrssldpp.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2ooynncoo.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2qfkaredr.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2yfcufahv.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2oebjpqop.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2uustkjtn.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2qanxyunj.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2usvvtceo.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2gbuiuslx.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2yyaggllt.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ukstmncc.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2vjlxfvce.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2hssqzwqq.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2ndtqomgy.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2enhzzili.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2abcjdklo.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2wcpnambc.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2xlhhxvkc.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2kzycydsm.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2fhatlplr.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2trpwggdz.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2dxrjdegw.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2ofgiekvj.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2oeiaxpyi.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2mlqwveol.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2lcfnexpp.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2rgimfvlx.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2uuoufhuv.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2wwlczane.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2spdwcomm.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2vmsxgfbc.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2jbbkdyqp.html


<!-- 参考信息 -->