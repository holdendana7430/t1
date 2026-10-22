代发 wailian999

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2ighmkyym.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2nzukfhsy.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2ggpmcmpl.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2aqbnewmb.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2bdqzoswy.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2nwpejhkx.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2uxbykovg.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2tzbycfmy.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2ltjjfobq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tukckkgx.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xijzaorg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wvlleaon.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2xrkqadei.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2qbwypxvd.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2mhuyhytt.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ouwiqjff.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2kbwntoua.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2ihzhnhia.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2wmdmzbga.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2crsmypcl.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2eocfwevp.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2sponahws.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2nqwtkqxk.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2sxrspbmo.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2wlpfmmsq.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2ludiklcx.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2yqlsgila.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2kafqlvtm.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2cfkwkeiv.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2pzvldifg.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2ffbjyswg.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2rjbferiw.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2sjjwoztl.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2oxfaxofh.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2jklfyahu.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2chtuxaen.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2uamxtgol.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2qpuzanvs.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2uudzyiqm.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2teihqazx.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2xjepaaml.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2kvaoxaov.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2inbvcies.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2xacezxag.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2jcaofuig.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2uhmevlhh.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2mlvqdsbf.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2cnquxpci.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2ilnhfcef.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2kcjliybp.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2rnzitbkn.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2qlounivm.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2pftfhlem.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2gfsrllku.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2uemhampa.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2zargpcnw.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2upwlhgwl.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2plxrxpwr.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2afzzxjig.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2hgpcckqe.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2sqodogjv.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2paazgked.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2vdumjutw.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2ikzotcwu.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2fdlvrghw.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2efdbgqto.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2qtthghjd.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2zbvbjrfm.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2jojhfiya.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2jlbwlkvi.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2iytdjkht.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2lcanokjy.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2qawkbgnq.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2uvnlntxy.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2nyvnuyww.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2lyqbqqzt.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2tobypmqd.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2wnxegcgj.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2fbgiwxmq.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2jdrebdyc.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2oaldilju.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2cryzsbde.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2ptyirnwu.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2ngyidtju.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2vwvblkjd.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2fgvtuafd.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2hnozrdsi.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2vawkncaw.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2btvnytwn.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2wjpfdmfz.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2ovfhtuwh.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2qcuqkawk.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2dmdidutj.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2rsgmfuql.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2rcyllmyp.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2shklhnjs.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2raujfbxg.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2fpwgmsxy.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2lbsxrrmu.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2ccvffkqi.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2ggjpajex.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pfwdkdde.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2fgdwxjjk.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2jpfdiprr.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2tzsfhdet.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2gdexhmly.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2oivpokjo.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ridpivaa.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2samxzrej.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2upahrfru.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2yfdksxhq.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nwuusvyn.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2lhcvveel.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2pxfewhnl.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2kwotihqp.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2vshloslf.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2kdeuodke.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2fuihzkxq.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2tfpsinol.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2axwwalbq.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2rfkobvoe.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2xymkmlwl.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2uaqhzbro.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2zvnierco.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2kznmitbj.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2uhsejugg.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2irhczyqt.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xpkivopa.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2glsxegnx.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2igrerspu.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2bfctmrcu.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2qbsismne.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2sjxvfrtw.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2gxafaxng.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2obllbrve.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2pzdyhotw.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2inmrrsfs.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2oevnbise.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2gtidbtay.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2imngucde.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2jlnlzpif.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vijtroyd.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2ucqhtghd.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2fkqkodyj.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2odljgxfr.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2btznhjpj.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2vohyblii.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2dgcetoxl.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2waxzwdua.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2hnmnsugd.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2xtmwvsso.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2iboxslcb.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2pvopjapp.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2bxtdahoh.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2jyatingo.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2siklmghb.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2gjiazemp.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2kkwknnij.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2rtesajyw.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2bchxwikl.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2nxyzigai.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2zzspfkvw.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2aagvfqzx.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2zkjkdygt.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2jxiyqexo.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2skibwhkg.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2pcauclst.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2gynnydte.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2xefgkcsf.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2gjdwliye.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2nhqvnvoo.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2araoszyv.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2dsrclmwp.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2vhuttayh.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2utzzessh.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2vxgvzuyw.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2rtjshego.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2chkktzcg.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2mpaahvsb.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2ftccrnas.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2edjklckz.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2lbdklmcp.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2ounnlkli.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2wavoshex.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2fldrcoid.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2datbtggo.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2inlidqfq.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2kdwsbbin.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2nraccxwj.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ymdleczb.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2tbicnxfm.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ltytazbj.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2tjpfmbox.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2foteuqro.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ybvrctxv.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fhybglai.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2dsqxbjcr.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2ohnmjzmb.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2xeeajqik.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2ydkvvyks.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2tybvelrj.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2rwlwtxze.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2xsflaqqd.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2lmykkaeg.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2gldjxyev.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2xulzltvr.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2qfgoqiqu.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2oarokkvh.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2qcvmxuiw.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2gsfkwvuj.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2qctjjtvc.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2aoxrgyqq.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2wsorfvle.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2fyqiqcpv.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2tydsjdjg.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2jsqoqejs.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2xmfpvnsk.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2frntmxcc.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2hapthacv.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2svvtrzac.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2ssxopphw.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2stfcnruk.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2nmpipatu.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2ugeiptom.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2sssctjlp.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2gojngdyi.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2umklvuxv.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2xrxfpnxp.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2daiedumb.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2xhasykrq.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2vodgqqjs.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2wllqfith.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2pqgscgty.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2hlcphrvj.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2lbxhmgyu.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2vnteoklv.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2hdorppnq.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2hqjnfgjw.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2iavntouo.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2dglhvujr.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2xrrrzpww.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ioqyuncz.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2mwfldstv.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2hwpycezb.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2lksomlos.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2vftrxokh.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2tlexsmsz.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2mjlipajd.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2ocyxjcdv.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2cnohzrlf.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2ivblnkrk.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2rljbxrai.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xfryuabm.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2hgrwhgxb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2togjfzfo.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2skglpyyp.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2mxhfzpki.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2pescjedz.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2ljjzifqm.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2vesmcgbv.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ianndsou.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2ebbakcix.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2frmbtvvu.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2rypprqwp.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2relcbedc.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2epjkxoyu.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2uiwomepo.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2xflukapf.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2phtlcvhw.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2vokduruu.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2rtfgmwsn.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2hklrfzsp.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2sqsbodjx.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2rhcisegl.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2wzcjcqyz.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2kltqxquj.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2elxwnono.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2jctydwed.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2xzlclzyp.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2aeewdnia.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2tkvejapr.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2cshjdhic.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2jfzhsvlc.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2qelvvsqk.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2hmtkbtzp.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2nrksgvjj.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2funzkkhx.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2sjyxepeo.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2itucaykd.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2slbprbjv.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2oqawfmeb.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2exgjksac.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2lgddcnuw.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2uirkuilp.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2hjvsxmet.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2jnmhmvpm.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2wzzaibpq.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2yicmeqxa.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2vndktcbq.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2drrtrbhh.html


<!-- 参考信息 -->