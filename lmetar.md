代发 wailian999

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2nsjqsjxf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ogpwnyek.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2liclbpkl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gigkheqt.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2xnkyezgl.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2xbochrng.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2aeyuvltl.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2hkbjceyz.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2ksxqlslm.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2eoueurmb.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2vrmgzepl.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2yxwtycqf.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2bgznmqfl.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2pakfxtam.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2wgldhqwu.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2alnxmjkf.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2rwurnieh.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2pymomets.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2trakpfph.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2vqeudtsd.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2bgtqiucv.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2hogaktof.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2qkmtlkhk.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2qdwvsjsh.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2xnodnhqt.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2yayedkia.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2kzuszhxa.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2heucydjl.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2fymswdqr.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2uciynzuq.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2vuotlhvq.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2dcvfhifs.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2ijzvzdql.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2wkapjiew.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2pekujvev.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2jkxptxoo.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2vhtfcoie.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2aobvohat.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2zcuwbnyn.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2urrtaifk.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2betkscsc.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2ofkhrdsu.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2goztylfp.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2tlreaijv.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2tzslkced.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2dustcfgk.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2dnyvecvg.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2xtghtckk.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2vtnolzvz.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2xddiajdu.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2jykzmezp.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2vyukfcaj.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2xvulgyij.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2tplzxmsx.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2fdbaewvw.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2kvulwcpz.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2amxbuisb.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2bxfbtcbs.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2xfickaiv.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2axnzmldo.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2ktyqonyv.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2eaauxdpi.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2keoinjvb.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2wiookvrw.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2jrvmmhne.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2rnmmxlxf.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2buxgnxkl.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2mwvnwtga.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2xdkqyigj.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2ftcuptno.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2xrsooqeu.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2piuikbtk.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2vdiujagn.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2eqciipdm.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2egrsipmb.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2gftcpfyo.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2eqmkaebn.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2kshdgghf.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2cirxjefo.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2spybffhv.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2meehvaxw.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2sgcofdql.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2nezktnkq.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2dqzrduou.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2guvazhtn.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2xwrzwhyi.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2hcxzxvlx.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2inkqmawi.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2haivnmme.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2pgaduilm.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2raflysjv.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2qxxfnjoy.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2ziwzzbcb.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2gfngasix.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2ueedjyhd.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2zlcdclbf.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2vpmbespw.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2glclpvhp.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2fzllelxt.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2qqhmwlav.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2zexrydxa.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2ccquebio.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2rtixcvtn.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2hmwbupdh.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2jsiaozzk.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2anxzverw.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2blgycaoo.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2mbqymiff.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2kswndnuv.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2xarcsuuj.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2jvluoqqb.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2fkgafdux.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2ubosehrn.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2oplldeyj.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2ohzqubjz.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2eiegpstj.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ifqeyrkf.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2efqasuul.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2zggnbidn.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2riibacfd.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2walispnd.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ytcrfvba.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2axkhxvev.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2phijwjuu.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2bqedugpe.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2uoqkhpwc.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2atdgehca.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2iygnhbhy.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2hwqovloa.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2vhwrcxvn.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2yvlrnklm.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2nvtyxirk.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2zyhlpoiw.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2uguprgit.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2qlnpimpc.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2txlyyxxe.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2hdeqlasa.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2cmpwdxvc.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2awocscxv.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2rzrcgytx.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2rfawarhk.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2qijqadmv.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2ajpfazlv.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2ljsjugbj.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2uildyyzh.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2lckaqbyc.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2kltgeqnq.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2ngwwknse.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2krhfyvnh.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2yprrhyax.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2imayfljc.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2kbsuzkfj.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2pfwimaog.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2scbdfgej.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2fpagwals.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2piffddmk.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2roboebix.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2hmohtcwx.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2fqykwldi.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2ycrxmxdd.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2pcjecjzn.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2dcdlonwi.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2wtdlswpv.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2uryhzjyq.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2hsqpacfi.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2hwzlyzwb.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2tnsajdbu.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2fjxagiwu.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2mvcypxpc.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2xfoyakjn.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2pimkpvkp.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2ognxawcl.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2wjnyltdp.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2jostvgpq.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2vsbeqdrk.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2yrufjfgu.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2zcfvjnqe.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2dyshuyaj.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2zbmcyhrz.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2gumxbszp.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2xtmdfbve.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2nvgssdjc.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2jewqowkd.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2vrgfuhfd.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2sggnniky.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2uoinsnnb.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2vvmkolfg.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2alzxwhso.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2wjzgrxcv.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2agjdcbmq.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2zlylfqnn.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2acovvfju.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2dewpnbpp.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2pnatmpmi.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2ryuqwnah.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2ciormulk.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2avgpliob.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2erftzzgo.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2lyzdnkpo.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2aqqeixjo.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2eduaycqa.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2xjatkhsk.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2zegnvdet.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2wtgbjltc.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2opgdhjsl.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2yzvhhxaf.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2usjjhhcu.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2brabkygm.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2vkxdujlh.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2uhcymhfb.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2cnpyvise.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2buiowafa.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2rabqjgks.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2duflsmgs.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2esuwceit.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2nzqtyhsz.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2jszsypdr.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2oitsrxfx.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2usvmjgug.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2bminndui.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2mpgqsnkw.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2pztvaspd.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2othfhzfp.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2tegbnuci.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2zvpdcafb.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2xfmmqcpi.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2nrezonzw.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2elgmtthl.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2rbvtrosf.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2oijllchf.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2pafrwksf.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2yrsertns.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2ukajpdun.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2bzymscth.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2fohazjpp.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2ipgqzunu.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2qixygaqv.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2lbtndmcn.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2iiphqpps.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2itmjsoai.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2npkuwiky.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2vegwvtua.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2mtkvypwx.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2iyouxclu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jzlmfbfc.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2lvpcwlkq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fyyqhctj.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2vibacial.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2qnlvqoav.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2gfmqazju.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2xxakjlfg.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2lvaoxpmf.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2sbvpplbd.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2dqrotjgc.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2cddrzcgj.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2pavizgxg.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2jdnklwwa.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2jqslzvcq.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2ykmajmza.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2gsdidlje.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2nlbprvhe.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2ypglkice.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2rryaxyyh.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2dhlqfnzp.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2kkwtqkvb.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2hsfwahnd.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2vsjzjnfh.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2fmxuqtls.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2wbigxfuj.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2isqyydyk.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2zagswghr.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2feajhexq.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2lnaedfiw.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2shnjorjz.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2gnktkhbc.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2tqpgkvek.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2fxnsrdkc.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2xixytkih.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2vztrjmue.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2fnxozsfg.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2rokpynjd.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2bisnvcrt.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2ykmerhff.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2wrrlkzyw.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2algadpat.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2zskffhcv.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2iknnnnxb.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2zljmpsrd.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2gnncbncd.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2wbxyvres.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2ebmpkbzg.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2bnksvzua.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2whvnfjgj.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2jxaojzca.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2hbutjlya.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2aggvukah.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2dqpxtvaf.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2mgwahdev.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2ammcyzto.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2qrvvhfyr.html


<!-- 参考信息 -->